# Comparing `tmp/tsk_monster-0.0.8.tar.gz` & `tmp/tsk_monster-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsk_monster-0.0.8.tar", max compression
+gzip compressed data, was "tsk_monster-0.0.9.tar", max compression
```

## Comparing `tsk_monster-0.0.8.tar` & `tsk_monster-0.0.9.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      363 2024-04-14 06:48:06.638346 tsk_monster-0.0.8/README.md
--rw-r--r--   0        0        0      753 2024-04-14 12:37:29.439176 tsk_monster-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5853 2024-04-14 12:36:51.019552 tsk_monster-0.0.8/tsk_monster/__init__.py
--rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 tsk_monster-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      363 2024-04-14 06:48:06.638346 tsk_monster-0.0.9/README.md
+-rw-r--r--   0        0        0      753 2024-04-14 13:20:25.325167 tsk_monster-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5728 2024-04-14 13:20:21.796386 tsk_monster-0.0.9/tsk_monster/__init__.py
+-rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 tsk_monster-0.0.9/PKG-INFO
```

### Comparing `tsk_monster-0.0.8/pyproject.toml` & `tsk_monster-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tsk-monster"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = ["Gilad Kutiel <giladk@mobileye.com>"]
 readme = "README.md"
 
 [tool.poetry.urls]
 Homepage = "https://tsk.monster"
 Documentation = "https://tsk.monster"
```

### Comparing `tsk_monster-0.0.8/tsk_monster/__init__.py` & `tsk_monster-0.0.9/tsk_monster/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,22 +13,21 @@
     ...         prods=['img1.small.jpg']))
 '''
 
 import logging
 import os
 import queue
 import threading
-from ast import Call
 from collections import defaultdict
 from concurrent.futures import Future, ProcessPoolExecutor
 from dataclasses import dataclass
 from functools import partial
 from inspect import getmembers, isgeneratorfunction
 from pathlib import Path
-from typing import Any, Callable, Generator, List
+from typing import Any, Callable, Generator, List, Tuple, cast
 
 import typer
 from typing_extensions import Annotated
 
 lg = logging.getLogger(__name__)
 
 
@@ -39,22 +38,29 @@
 
 @dataclass
 class prod:
     val: Any
 
 
 @dataclass
-class Job:
+class Cmd:
     description: str
-    gen: Generator[need | prod | Callable, None, None]
+    action: Callable[[], Any]
+
+    @classmethod
+    def from_str(cls, cmd: str):
+        return cls(cmd, partial(os.system, cmd))
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return self.description
 
 
+Job = Generator[need | prod | Cmd, None, None]
+
+
 def run_jobs(*jobs: Job):
     '''Run jobs in parallel, respecting dependencies.
 
     Args:
         *jobs: A list of jobs to run.
 
 
@@ -84,19 +90,20 @@
             return _
 
         with ProcessPoolExecutor() as executor:
             while True:
                 job = q.get()
 
                 try:
-                    item = next(job.gen)
+                    item = next(job)
+                    lg.info(f'Running: {type(item)} {item}')
 
-                    if isinstance(item, Callable):
-                        lg.info(f'Submitting: {job}')
-                        future = executor.submit(item)
+                    if isinstance(item, Cmd):
+                        lg.info(f'Submitting: {item.description}')
+                        future = executor.submit(item.action)
                         future.add_done_callback(add2q(job))
 
                     if isinstance(item, need):
                         lg.debug(f'{job} needs {item.val}')
 
                         if item.val in prods:
                             q.put(job)
@@ -129,57 +136,21 @@
         q.put(job)
 
     q.join()
 
     lg.info('All work completed')
 
 
-@dataclass
-class Cmd:
-    description: str
-    action: Callable[[], Any]
-
-    @classmethod
-    def from_str(cls, cmd: str):
-        return cls(cmd, partial(os.system, cmd))
-
-    def __repr__(self) -> str:
-        return self.description
-
-
-def changed(path: Path):
-    try:
-        tsk = path.with_suffix('.tsk')
-        if not tsk.exists():
-            return True
-
-        return tsk.stat().st_mtime < path.stat().st_mtime
-    finally:
-        tsk.touch()
-
-
 Paths = List[Path | str] | List[Path]
 
 
-def to_paths(paths: Paths) -> List[Path]:
-    return [Path(p) if isinstance(p, str) else p for p in paths]
-
-
-def default_run(needs: List[Path], prods: List[Path]):
-    if not needs and not prods:
-        return True
-
-    return any(map(changed, needs)) or not all(map(Path.exists, prods))
-
-
 def tsk(
-        cmd: str | Cmd, *,
+        *cmds: Cmd | str,
         needs: Paths = [],
-        prods: Paths = [],
-        run: Callable[[List[Path], List[Path]], bool] | bool = default_run) -> Job:
+        prods: Paths = []) -> Job:
     '''Create a file based task.
 
     Examples:
         >>> tsk(
         ...     'wget -O img1.jpg https://picsum.photos/200/300',
         ...     prods=['img1.jpg'])
 
@@ -188,54 +159,72 @@
         needs: A list of files that are needed.
         prods: A list of files that will be produced.
 
     Returns:
         A job.
     '''
 
-    if isinstance(cmd, str):
-        cmd = Cmd.from_str(cmd)
+    def changed(path: Path):
+        try:
+            tsk = path.with_suffix('.tsk')
+            if not tsk.exists():
+                return True
+
+            return tsk.stat().st_mtime < path.stat().st_mtime
+        finally:
+            tsk.touch()
+
+    def to_paths(paths: Paths) -> List[Path]:
+        return [Path(p) if isinstance(p, str) else p for p in paths]
 
     needs = to_paths(needs)
     prods = to_paths(prods)
 
-    def gen(run=run):
+    cmds = tuple([
+        Cmd.from_str(cmd)
+        if isinstance(cmd, str)
+        else cmd
+        for cmd in cmds])
+
+    cmds = cast(Tuple[Cmd], cmds)
+
+    always_run = len(needs) + len(prods) == 0
+
+    def gen():
         for n in needs:
             yield need(n)
 
-        if not isinstance(run, bool):
-            run = run(needs, prods)
-
-        if run:
-            yield cmd.action
+        if always_run or any(map(changed, needs)) or not all(map(Path.exists, prods)):
+            yield from cmds
 
         else:
-            lg.info(f'SKIPPING: {cmd.description}')
+            for cmd in cmds:
+                lg.info(f'SKIPPING: {cmd.description}')
 
         for m in prods:
             if m.exists():
                 yield prod(m)
             else:
                 raise Exception(f'{cmd} failed to produce {m}.')
 
-    return Job(cmd.description, gen())
-
-
-app = typer.Typer()
+    return gen()
 
 
 def load_tasks():
     module = __import__('tskfile')
     return getmembers(module, isgeneratorfunction)
 
 
 def task_names(prefix: str):
     return [name for name, _ in load_tasks() if name.startswith(prefix)]
 
 
+app = typer.Typer()
+
+
 @app.command()
 def tsk_monster(target: Annotated[str, typer.Argument(autocompletion=task_names)]):
     logging.basicConfig(
         level=logging.INFO,
         datefmt='%H:%M:%S',
         format='%(asctime)s - %(levelname)s - %(message)s')
```

### Comparing `tsk_monster-0.0.8/PKG-INFO` & `tsk_monster-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsk-monster
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Author: Gilad Kutiel
 Author-email: giladk@mobileye.com
 Requires-Python: ==3.10.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: typer (>=0.12.3,<0.13.0)
```

