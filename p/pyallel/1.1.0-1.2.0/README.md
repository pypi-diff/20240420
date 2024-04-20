# Comparing `tmp/pyallel-1.1.0.tar.gz` & `tmp/pyallel-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyallel-1.1.0.tar", max compression
+gzip compressed data, was "pyallel-1.2.0.tar", max compression
```

## Comparing `pyallel-1.1.0.tar` & `pyallel-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     1069 2023-12-10 12:28:31.474872 pyallel-1.1.0/LICENSE
--rw-r--r--   0        0        0     3570 2024-03-10 13:51:48.671607 pyallel-1.1.0/README.md
--rw-r--r--   0        0        0     1047 2024-03-10 13:51:58.483694 pyallel-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-10 12:28:31.486873 pyallel-1.1.0/src/pyallel/__init__.py
--rw-r--r--   0        0        0      893 2024-02-24 08:46:35.646124 pyallel-1.1.0/src/pyallel/colours.py
--rw-r--r--   0        0        0      564 2024-03-03 05:35:35.595476 pyallel-1.1.0/src/pyallel/constants.py
--rw-r--r--   0        0        0      368 2023-12-10 16:41:29.922819 pyallel-1.1.0/src/pyallel/errors.py
--rw-r--r--   0        0        0     2158 2024-03-10 11:27:14.288084 pyallel-1.1.0/src/pyallel/main.py
--rw-r--r--   0        0        0     2380 2024-03-10 13:50:47.559062 pyallel-1.1.0/src/pyallel/parser.py
--rw-r--r--   0        0        0    13074 2024-03-10 13:46:48.392932 pyallel-1.1.0/src/pyallel/process.py
--rw-r--r--   0        0        0        0 2023-12-10 12:28:32.010876 pyallel-1.1.0/src/pyallel/py.typed
--rw-r--r--   0        0        0     4478 1970-01-01 00:00:00.000000 pyallel-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-12-10 12:28:31.474872 pyallel-1.2.0/LICENSE
+-rw-r--r--   0        0        0     4334 2024-04-20 11:06:03.145124 pyallel-1.2.0/README.md
+-rw-r--r--   0        0        0     1047 2024-04-20 10:58:17.449054 pyallel-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-10 12:28:31.486873 pyallel-1.2.0/src/pyallel/__init__.py
+-rw-r--r--   0        0        0      893 2024-04-13 11:42:32.468688 pyallel-1.2.0/src/pyallel/colours.py
+-rw-r--r--   0        0        0      564 2024-04-20 09:08:17.203906 pyallel-1.2.0/src/pyallel/constants.py
+-rw-r--r--   0        0        0      368 2023-12-10 16:41:29.922819 pyallel-1.2.0/src/pyallel/errors.py
+-rw-r--r--   0        0        0     2190 2024-04-20 09:42:35.756227 pyallel-1.2.0/src/pyallel/main.py
+-rw-r--r--   0        0        0     2799 2024-04-20 10:37:37.130827 pyallel-1.2.0/src/pyallel/parser.py
+-rw-r--r--   0        0        0     1952 2024-04-20 09:15:53.499524 pyallel-1.2.0/src/pyallel/process.py
+-rw-r--r--   0        0        0    10871 2024-04-20 09:16:13.527683 pyallel-1.2.0/src/pyallel/process_group.py
+-rw-r--r--   0        0        0     2919 2024-04-20 10:15:27.504102 pyallel-1.2.0/src/pyallel/process_group_manager.py
+-rw-r--r--   0        0        0        0 2023-12-10 12:28:32.010876 pyallel-1.2.0/src/pyallel/py.typed
+-rw-r--r--   0        0        0     5242 1970-01-01 00:00:00.000000 pyallel-1.2.0/PKG-INFO
```

### Comparing `pyallel-1.1.0/LICENSE` & `pyallel-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyallel-1.1.0/README.md` & `pyallel-1.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -22,26 +22,34 @@
 
 ```
 usage: pyallel [-h] [-t] [-n] [-V] [--colour {yes,no,auto}] [commands ...]
 
 Run and handle the output of multiple executables in pyallel (as in parallel)
 
 positional arguments:
-  commands              list of quoted commands to run e.g "mypy ." "black ."
+  commands              list of quoted commands to run in parallel e.g "mypy ." "black ."
 
                         each command is executed inside a shell, so shell syntax is supported as
-                        if you were running the command directly in a shell, some examples are below:
+                        if you were running the command directly in a shell, some examples are below
 
                              "MYPY_FORCE_COLOR=1 mypy ."          <- provide environment variables
                              "mypy | tee -a mypy.log"             <- use pipes to redirect output
                              "cat > test.log < other.log"         <- use input and output redirection
                              "mypy .; pytest ."                   <- run commands one at a time in sequence
                              "echo \$SHELL" or "\$(echo mypy .)"  <- expand variables and commands to evaluate (must be escaped)
                              "pytest . && mypy . || echo failed!" <- use AND (&&) and OR (||) to run commands conditionally
 
+                        commands can be grouped using the group separator symbol (:::)
+
+                             "echo boil kettle" "sleep 1" ::: "echo make coffee"
+
+                        the above will print "boil kettle" and sleep for 1 second first before printing "make coffee"
+
+                        command groups are ran in the sequence you provide them, and if a command group fails
+                        (if a command fails inside the command group) the rest of the command groups in the sequence are not run
 
 options:
   -h, --help            show this help message and exit
   -t, --no-timer        don't time how long each command is taking
   -n, --non-interactive
                         run in non-interactive mode
   -V, --version         print version and exit
@@ -84,14 +92,17 @@
 
 ```bash
 python -m venv .venv && source .venv/bin/activate && pip install . -r requirements_build.txt && ./build.sh
 ```
 
 ## TODOs
 
+- [x] Add support to have commands depend on other commands (some commands must complete
+      before a given command can start)
+- [ ] Add support to state how many lines a command can use for it's output in interactive mode
 - [ ] Maybe add support to allow the user to provide stdin for commands that request it
       (such as a REPL)
 - [ ] Add custom parsing of command output to support filtering for errors (like vim's
       `errorformat`)
 - [ ] Allow list of files to be provided to supply as input arguments to each command
 - [ ] Allow input to be piped into `pyallel` via stdin to supply as standard input to each
       command
```

### Comparing `pyallel-1.1.0/pyproject.toml` & `pyallel-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyallel"
-version = "1.1.0"
+version = "1.2.0"
 description = "Run and handle the output of multiple executables in pyallel (as in parallel)"
 authors = ["Daniel Black <danielcrblack@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Danthewaann/pyallel"
 repository = "https://github.com/Danthewaann/pyallel"
 keywords = ["parallel", "command", "runner", "executable", "shell", "terminal"]
```

### Comparing `pyallel-1.1.0/src/pyallel/colours.py` & `pyallel-1.2.0/src/pyallel/colours.py`

 * *Files identical despite different names*

### Comparing `pyallel-1.1.0/src/pyallel/constants.py` & `pyallel-1.2.0/src/pyallel/constants.py`

 * *Files identical despite different names*

### Comparing `pyallel-1.1.0/src/pyallel/main.py` & `pyallel-1.2.0/src/pyallel/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 import sys
 import traceback
 
 from pyallel import constants
 from pyallel.colours import Colours
 from pyallel.errors import InvalidExecutableErrors
 from pyallel.parser import Arguments, create_parser
-from pyallel.process import ProcessGroup
+from pyallel.process_group_manager import ProcessGroupManager
 
 
 def main_loop(
-    *commands: str,
+    *args: str,
     colours: Colours,
     interactive: bool = False,
     timer: bool = False,
 ) -> int:
-    process_group = ProcessGroup.from_commands(
-        *commands,
+    process_group_manager = ProcessGroupManager.from_args(
+        *args,
         colours=colours,
         interactive=interactive,
         timer=timer,
     )
 
-    return process_group.stream()
+    return process_group_manager.stream()
 
 
 def run(*args: str) -> int:
     parser = create_parser()
     parsed_args = parser.parse_args(args=args, namespace=Arguments())
 
     if parsed_args.version:
```

### Comparing `pyallel-1.1.0/src/pyallel/parser.py` & `pyallel-1.2.0/src/pyallel/parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,26 +15,34 @@
         msg = "Arguments:\n"
         padding = len(sorted(self.__dict__.keys(), key=len, reverse=True)[0]) + 1
         for field, value in self.__dict__.items():
             msg += f"    {field: <{padding}}: {value}\n"
         return msg
 
 
-COMMANDS_HELP = r"""list of quoted commands to run e.g "mypy ." "black ."
+COMMANDS_HELP = r"""list of quoted commands to run in parallel e.g "mypy ." "black ."
 
 each command is executed inside a shell, so shell syntax is supported as
-if you were running the command directly in a shell, some examples are below:
+if you were running the command directly in a shell, some examples are below
 
      "MYPY_FORCE_COLOR=1 mypy ."          <- provide environment variables
      "mypy | tee -a mypy.log"             <- use pipes to redirect output
      "cat > test.log < other.log"         <- use input and output redirection
      "mypy .; pytest ."                   <- run commands one at a time in sequence
      "echo \$SHELL" or "\$(echo mypy .)"  <- expand variables and commands to evaluate (must be escaped)
      "pytest . && mypy . || echo failed!" <- use AND (&&) and OR (||) to run commands conditionally
 
+commands can be grouped using the group separator symbol (:::)
+
+     "echo boil kettle" "sleep 1" ::: "echo make coffee"
+
+the above will print "boil kettle" and sleep for 1 second first before printing "make coffee"
+
+command groups are ran in the sequence you provide them, and if a command group fails
+(if a command fails inside the command group) the rest of the command groups in the sequence are not run
 """
 
 
 def create_parser() -> ArgumentParser:
     parser = ArgumentParser(
         prog="pyallel",
         description="Run and handle the output of multiple executables in pyallel (as in parallel)",
```

### Comparing `pyallel-1.1.0/src/pyallel/process.py` & `pyallel-1.2.0/src/pyallel/process_group.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 from __future__ import annotations
 
-import signal
-import subprocess
-import tempfile
 import time
 from collections import defaultdict
 from dataclasses import dataclass, field
-from typing import Any, BinaryIO
-from uuid import UUID, uuid4
 
 from pyallel import constants
 from pyallel.colours import Colours
 from pyallel.errors import InvalidExecutableError, InvalidExecutableErrors
+from pyallel.process import Process
 
 
 def get_num_lines(output: str, columns: int | None = None) -> int:
     lines = 0
     columns = columns or constants.COLUMNS()
     for line in output.splitlines():
         line = constants.ANSI_ESCAPE.sub("", line)
@@ -32,17 +28,17 @@
 
 
 @dataclass
 class ProcessGroup:
     processes: list[Process]
     interactive: bool = False
     timer: bool = False
-    output: dict[UUID, list[str]] = field(default_factory=lambda: defaultdict(list))
+    output: dict[int, list[str]] = field(default_factory=lambda: defaultdict(list))
     process_lines: list[int] = field(default_factory=list)
-    completed_processes: set[UUID] = field(default_factory=set)
+    completed_processes: set[int] = field(default_factory=set)
     exit_code: int = 0
     interrupt_count: int = 0
     passed: bool = True
     icon: int = 0
     colours: Colours = field(default_factory=Colours)
 
     def stream(self) -> int:
@@ -79,19 +75,14 @@
 
         return self.exit_code
 
     def stream_non_interactive(self) -> int:
         running_process = None
         interrupted = False
 
-        print(
-            f"{self.colours.dim_on}=>{self.colours.dim_off} {self.colours.white_bold}Running commands...{self.colours.reset_colour}\n{self.colours.dim_on}=>{self.colours.dim_off} ",
-            flush=True,
-        )
-
         while True:
             output = ""
             for process in self.processes:
                 if (
                     running_process is None
                     and process.id not in self.completed_processes
                 ):
@@ -208,54 +199,52 @@
             if not process.end:
                 end = time.perf_counter()
             elapsed = end - process.start
             output += f" {self.colours.dim_on}({format_time_taken(elapsed)}){self.colours.dim_off}"
 
         return output
 
-    def _handle_signal(self, signum: int, _frame: Any) -> None:
+    def handle_signal(self, signum: int) -> None:
         for process in self.processes:
             if self.interrupt_count == 0:
                 process.interrupt()
             else:
                 process.kill()
 
         self.exit_code = 128 + signum
         self.interrupt_count += 1
 
     @classmethod
     def from_commands(
         cls,
         *commands: str,
-        colours: Colours,
+        colours: Colours | None = None,
         interactive: bool = False,
         timer: bool = False,
     ) -> ProcessGroup:
+        colours = colours or Colours()
         processes: list[Process] = []
         errors: list[InvalidExecutableError] = []
 
-        for command in commands:
+        for i, command in enumerate(commands):
             try:
-                processes.append(Process.from_command(command))
+                processes.append(Process.from_command(i + 1, command))
             except InvalidExecutableError as e:
                 errors.append(e)
 
         if errors:
             raise InvalidExecutableErrors(*errors)
 
         process_group = cls(
             processes=processes,
             interactive=interactive,
             timer=timer,
             colours=colours,
         )
 
-        signal.signal(signal.SIGINT, process_group._handle_signal)
-        signal.signal(signal.SIGTERM, process_group._handle_signal)
-
         return process_group
 
     def complete_output(self, tail: int = 20, all: bool = False) -> str:
         num_processes = len(self.processes)
         lines = constants.LINES() - (2 * num_processes)
         remainder = lines % num_processes
         tail = lines // num_processes
@@ -315,75 +304,7 @@
             output += (
                 f"\n{self.colours.yellow_bold}Interrupt!{self.colours.reset_colour}"
             )
         elif self.interrupt_count == 2:
             output += f"\n{self.colours.red_bold}Abort!{self.colours.reset_colour}"
 
         return output
-
-
-@dataclass
-class Process:
-    id: UUID = field(repr=False, compare=False)
-    command: str
-    start: float = 0.0
-    end: float = 0.0
-    _fd: BinaryIO | None = field(init=False, repr=False, compare=False, default=None)
-    _process: subprocess.Popen[bytes] | None = field(
-        init=False, repr=False, compare=False, default=None
-    )
-
-    def run(self) -> None:
-        self.start = time.perf_counter()
-        fd, fd_name = tempfile.mkstemp()
-        self._fd = open(fd_name, "rb")
-        self._process = subprocess.Popen(
-            self.command,
-            stdin=subprocess.DEVNULL,
-            stdout=fd,
-            stderr=subprocess.STDOUT,
-            shell=True,
-        )
-
-    def __del__(self) -> None:
-        if self._fd:
-            self._fd.close()
-
-    def poll(self) -> int | None:
-        if self._process:
-            poll = self._process.poll()
-            if poll is not None and not self.end:
-                self.end = time.perf_counter()
-            return poll
-        return None
-
-    def read(self) -> bytes:
-        if self._fd:
-            return self._fd.read()
-        return b""
-
-    def readline(self) -> bytes:
-        if self._fd:
-            return self._fd.readline()
-        return b""
-
-    def return_code(self) -> int | None:
-        if self._process:
-            return self._process.returncode
-        return None
-
-    def interrupt(self) -> None:
-        if self._process:
-            self._process.send_signal(signal.SIGINT)
-
-    def kill(self) -> None:
-        if self._process:
-            self._process.send_signal(signal.SIGKILL)
-
-    def wait(self) -> int:
-        if self._process:
-            return self._process.wait()
-        return -1
-
-    @classmethod
-    def from_command(cls, command: str) -> Process:
-        return cls(id=uuid4(), command=command)
```

### Comparing `pyallel-1.1.0/PKG-INFO` & `pyallel-1.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyallel
-Version: 1.1.0
+Version: 1.2.0
 Summary: Run and handle the output of multiple executables in pyallel (as in parallel)
 Home-page: https://github.com/Danthewaann/pyallel
 License: MIT
 Keywords: parallel,command,runner,executable,shell,terminal
 Author: Daniel Black
 Author-email: danielcrblack@gmail.com
 Requires-Python: >=3.8,<3.13
@@ -44,26 +44,34 @@
 
 ```
 usage: pyallel [-h] [-t] [-n] [-V] [--colour {yes,no,auto}] [commands ...]
 
 Run and handle the output of multiple executables in pyallel (as in parallel)
 
 positional arguments:
-  commands              list of quoted commands to run e.g "mypy ." "black ."
+  commands              list of quoted commands to run in parallel e.g "mypy ." "black ."
 
                         each command is executed inside a shell, so shell syntax is supported as
-                        if you were running the command directly in a shell, some examples are below:
+                        if you were running the command directly in a shell, some examples are below
 
                              "MYPY_FORCE_COLOR=1 mypy ."          <- provide environment variables
                              "mypy | tee -a mypy.log"             <- use pipes to redirect output
                              "cat > test.log < other.log"         <- use input and output redirection
                              "mypy .; pytest ."                   <- run commands one at a time in sequence
                              "echo \$SHELL" or "\$(echo mypy .)"  <- expand variables and commands to evaluate (must be escaped)
                              "pytest . && mypy . || echo failed!" <- use AND (&&) and OR (||) to run commands conditionally
 
+                        commands can be grouped using the group separator symbol (:::)
+
+                             "echo boil kettle" "sleep 1" ::: "echo make coffee"
+
+                        the above will print "boil kettle" and sleep for 1 second first before printing "make coffee"
+
+                        command groups are ran in the sequence you provide them, and if a command group fails
+                        (if a command fails inside the command group) the rest of the command groups in the sequence are not run
 
 options:
   -h, --help            show this help message and exit
   -t, --no-timer        don't time how long each command is taking
   -n, --non-interactive
                         run in non-interactive mode
   -V, --version         print version and exit
@@ -106,14 +114,17 @@
 
 ```bash
 python -m venv .venv && source .venv/bin/activate && pip install . -r requirements_build.txt && ./build.sh
 ```
 
 ## TODOs
 
+- [x] Add support to have commands depend on other commands (some commands must complete
+      before a given command can start)
+- [ ] Add support to state how many lines a command can use for it's output in interactive mode
 - [ ] Maybe add support to allow the user to provide stdin for commands that request it
       (such as a REPL)
 - [ ] Add custom parsing of command output to support filtering for errors (like vim's
       `errorformat`)
 - [ ] Allow list of files to be provided to supply as input arguments to each command
 - [ ] Allow input to be piped into `pyallel` via stdin to supply as standard input to each
       command
```

