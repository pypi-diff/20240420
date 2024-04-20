# Comparing `tmp/iwashi-2.2.2.tar.gz` & `tmp/iwashi-3.0.0.tar.gz`

## Comparing `iwashi-2.2.2.tar` & `iwashi-3.0.0.tar`

### file list

```diff
@@ -1,47 +1,74 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 iwashi-2.2.2/.python-version
--rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 iwashi-2.2.2/README.rst
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 iwashi-2.2.2/requirements-dev.lock
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 iwashi-2.2.2/requirements.lock
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 iwashi-2.2.2/.github/workflows/pypi.yml
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 iwashi-2.2.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 iwashi-2.2.2/.vscode/settings.json
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/__init__.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/__main__.py
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/helper.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/iwashi.py
--rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitor.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/__init__.py
--rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/bandcamp.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/bitly.py
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/booth.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/fanbox.py
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/fanlink.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/googl.py
--rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/instagram.py
--rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/linktree.py
--rw-r--r--   0        0        0    13078 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/litlink.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/mirrativ.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/misskey.py
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/nicovideo.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/note.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/pagelink.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/pixiv.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/reddit.py
--rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/sketch.py
--rw-r--r--   0        0        0     4452 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/soundcloud.py
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/spotify.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/tiktok.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/twitcasting.py
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/twitch.py
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/twitter.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/youtube/__init__.py
--rw-r--r--   0        0        0     7580 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/youtube/youtube.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/youtube/types/__init__.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/youtube/types/about.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 iwashi-2.2.2/src/iwashi/visitors/youtube/types/ytinitialdata.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 iwashi-2.2.2/tests/visitors/test_youtube.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 iwashi-2.2.2/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 iwashi-2.2.2/LICENSE
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 iwashi-2.2.2/README.md
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 iwashi-2.2.2/pyproject.toml
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 iwashi-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 iwashi-3.0.0/.python-version
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 iwashi-3.0.0/aa copy.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 iwashi-3.0.0/aa.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 iwashi-3.0.0/requirements-dev.lock
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 iwashi-3.0.0/requirements.lock
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 iwashi-3.0.0/.github/scripts/report-failures.sh
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 iwashi-3.0.0/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 iwashi-3.0.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 iwashi-3.0.0/.vscode/settings.json
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/__init__.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/__main__.py
+-rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/helper.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/iwashi.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/throttle.py
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/visitor.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/__init__.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/bandcamp.py
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/booth.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/fanbox.py
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/github.py
+-rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/instagram.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/itchio.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/kofi.py
+-rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/linktree.py
+-rw-r--r--   0        0        0    13215 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/litlink.py
+-rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/mirrativ.py
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/nicovideo.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/note.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/patreon.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/pixiv.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/reddit.py
+-rw-r--r--   0        0        0     7883 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/sketch.py
+-rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/soundcloud.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/spotify.py
+-rw-r--r--   0        0        0    92171 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/tiktok.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/twitcasting.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/twitch.py
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/twitter.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/youtube/__init__.py
+-rw-r--r--   0        0        0     8915 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/youtube/youtube.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/youtube/types/__init__.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/youtube/types/about.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/youtube/types/ytinitialdata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/service_tester.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_bandcamp.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_booth.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_fanbox.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_github.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_instagram.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_itchio.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_kofi.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_link_tree.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_linktree.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_litlink.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_mirrativ.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_nicovideo.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_note.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_patreon.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_pixiv.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_reddit.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_sketch.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_soundcloud.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_spotify.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_tiktok.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_twitcasting.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_twitch.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_twitter.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_youtube.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 iwashi-3.0.0/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 iwashi-3.0.0/LICENSE
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 iwashi-3.0.0/README.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 iwashi-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 iwashi-3.0.0/PKG-INFO
```

### Comparing `iwashi-2.2.2/.github/workflows/pypi.yml` & `iwashi-3.0.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `iwashi-2.2.2/.github/workflows/test.yml` & `iwashi-3.0.0/.github/workflows/test.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,55 @@
 name: test
 
-on: [push]
+on:
+  push:
+  schedule:
+    - cron: "0 0,12 * * *"
 
 jobs:
   test:
-    runs-on: ubuntu-latest
-    permissions:
-      # IMPORTANT: this permission is mandatory for trusted publishing
-      id-token: write
+    runs-on: self-hosted
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v3
         with:
           python-version: "3.x"
+
       - name: Install rye
         uses: eifinger/setup-rye@v1
         with:
-          version: "0.19.0"
           enable-cache: true
           cache-prefix: "rye"
+
       - name: Cache dependencies
         id: cache
         uses: actions/cache@v4
         with:
           path: .venv
           key: pip-${{ runner.os }}-${{ hashFiles('**/requirements*.lock') }}
+
       - name: Install dependencies
         if: steps.cache.outputs.cache-hit != 'true'
         run: |
+          rye config --set-bool behavior.use-uv=true
           rye sync
+
       - name: Run tests
+        id: test
         run: |
           rye run pytest -v --cov=./src --cov-report=xml
+
       - name: Upload coverage reports to Codecov
         uses: codecov/codecov-action@v4.0.1
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
           slug: am230/iwashi
+
+      - name: Report failures
+        if: failure() && steps.test.outcome == 'failure'
+        run: |
+          chmod +x .github/scripts/report-failures.sh
+          ./.github/scripts/report-failures.sh
+        env:
+          WEBHOOK_URL: ${{ secrets.WEBHOOK_URL }}
+          WORKFLOW_URL: https://github.com/${{ github.repository }}/actions/runs/${{ github.run_id }}
```

### Comparing `iwashi-2.2.2/src/iwashi/helper.py` & `iwashi-3.0.0/src/iwashi/helper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import asyncio
 import random
 import re
 import string
 import time
 from typing import Any, Callable
 
@@ -15,31 +16,25 @@
 DEBUG = False
 
 
 def print_result(
     result: Result, indent_level=0, print: Callable[[str], Any] = print
 ) -> None:
     indent = indent_level * "    "
-    print(f"{indent}{result.site_name}")
-    print(f"{indent}│url  : {result.url}")
-    print(f"{indent}│name : {result.title}")
+    print(f"{indent}{result.service.name}")
+    print(f"{indent}|id    : {result.id}")
+    print(f"{indent}│url   : {result.url}")
+    print(f"{indent}│name  : {result.name}")
     print(f"{indent}│links : {result.links}")
     if result.description:
         print(f"{indent}│description: " + result.description.replace("\n", "\\n"))
     for child in result.children:
         print_result(child, indent_level + 1, print)
 
 
-def parse_host(url: str) -> str:
-    match = re.search(r"(https?:\/\/)?(www\.)?(?P<host>[\w.]+)/", url)
-    if match is None:
-        return url
-    return match.group("host")
-
-
 def random_string(length: int) -> str:
     return "".join(random.choice(string.ascii_letters) for _ in range(length))
 
 
 URL_NORMALIZE_REGEX = r"(?P<protocol>https?)?:?\/?\/?(?P<domain>[^.]+\.[^\/]+)(?P<path>[^?#]+)?(?P<query>.+)?"
 
 
@@ -130,7 +125,43 @@
         if key in cache:
             return cache[key]
         result = await func(*args, **kwargs)
         cache[key] = result
         return result
 
     return wrapper
+
+
+class Traverser[T]:
+    def __init__(self, value: T | None = None):
+        self.value = value
+
+    def map[V](self, func: Callable[[T], V], default: V | None = None) -> Traverser[V]:
+        if self.value is None:
+            return TRAVERSE_NONE
+        value = func(self.value)
+        if value is None:
+            return Traverser(default)
+        return Traverser(value)
+
+    def get(self, default: T | None = None) -> T | None:
+        if self.value is None:
+            return default
+        return self.value
+
+    def unwrap(self) -> T:
+        if self.value is None:
+            raise ValueError("Value is None")
+        return self.value
+
+    def is_none(self) -> bool:
+        return self.value is None
+
+
+TRAVERSE_NONE = Traverser(None)
+
+
+def traverse[T](value: T | None) -> Traverser[T]:
+    """
+    Traverse a value that may be None.
+    """
+    return Traverser(value)
```

### Comparing `iwashi-2.2.2/src/iwashi/visitor.py` & `iwashi-3.0.0/src/iwashi/visitor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 from __future__ import annotations
 
 import abc
+from datetime import timedelta
 import re
 from dataclasses import dataclass, field
 from typing import List, Optional, Protocol, Set
 
 import aiohttp
 
+from iwashi.throttle import Throttle
+
 HTTP_REGEX = "(https?://)?(www.)?"
 
 
 @dataclass
 class Result:
+    service: Service
+    id: str
     url: str
-    site_name: Optional[str]
-    title: Optional[str]
+    name: Optional[str]
     description: Optional[str]
     profile_picture: Optional[str]
 
     children: List[Result] = field(default_factory=list)
     links: Set[str] = field(default_factory=set)
 
     def to_list(self) -> List[Result]:
         links: List[Result] = [self]
         for child in self.children:
             links.extend(child.to_list())
         return links
 
 
 class Visitor(Protocol):
-    async def visit(self, url: str, context: Context, **kwargs) -> Result:
+    async def visit(self, url: str, context: Context) -> Result | None:
         ...
 
     def mark_visited(self, url: str) -> None:
         ...
 
     def enqueue_visit(self, url: str, context: Context) -> None:
         ...
 
 
 class FakeVisitor(Visitor):
     def __init__(self):
-        self.queue = []
+        self.queue: List[str] = []
 
     async def visit(self, url, context, **kwargs):
         raise NotImplementedError
 
     async def tree(self, url, context, **kwargs):
         raise NotImplementedError
 
@@ -55,31 +59,32 @@
     def mark_visited(self, url):
         raise NotImplementedError
 
 
 @dataclass
 class Context:
     session: aiohttp.ClientSession
-    url: str
     visitor: Visitor
     parent: Optional[Context] = None
     result: Optional[Result] = None
 
     def create_result(
         self,
-        site_name: str,
+        service: Service,
+        id: str,
         url: str,
         name: Optional[str] = None,
         description: Optional[str] = None,
         profile_picture: Optional[str] = None,
     ) -> Result:
         self.result = Result(
-            site_name=site_name,
+            service=service,
+            id=id,
             url=url,
-            title=name,
+            name=name,
             description=description,
             profile_picture=profile_picture,
         )
 
         if self.parent and self.parent.result:
             self.parent.result.children.append(self.result)
 
@@ -89,38 +94,49 @@
         if self.result is None:
             raise ValueError("Result is not created yet")
         self.result.links.add(url)
 
     def mark_visited(self, url: str) -> None:
         self.visitor.mark_visited(url)
 
-    def create_context(self, url: str) -> Context:
-        return Context(session=self.session, url=url, visitor=self.visitor, parent=self)
+    def create_context(self) -> Context:
+        return Context(session=self.session, visitor=self.visitor, parent=self)
 
     def enqueue_visit(self, url: str) -> None:
-        self.link(url)
+        if self.result is not None:
+            self.link(url)
         self.visitor.enqueue_visit(url, self)
 
 
-class SiteVisitor(abc.ABC):
-    NAME: Optional[str] = None
-    URL_REGEX: Optional[re.Pattern] = None
+class Service(abc.ABC):
+    throttle: Throttle
+
+    def __init_subclass__(cls) -> None:
+        cls.throttle = Throttle(timedelta(seconds=5))
+        return super().__init_subclass__()
+
+    def __init__(self, name: str, regex: re.Pattern):
+        self.name = name
+        self.regex = regex
 
     def match(self, url, context: Context) -> Optional[re.Match]:
-        if self.URL_REGEX is None:
-            raise NotImplementedError()
-        return self.URL_REGEX.match(url)
+        return self.regex.match(url)
 
-    async def normalize(self, context: Context, url: str) -> str | None:
-        return url
+    async def resolve_id(self, context: Context, url: str) -> str | None:
+        match = self.regex.search(url)
+        return match and match.group("id")
 
     @abc.abstractmethod
-    async def visit(self, url, context: Context, **kwargs) -> Optional[Result]:
+    async def visit(self, context: Context, id: str) -> Optional[Result]:
         raise NotImplementedError()
 
     async def visit_url(
-        self, url: str, session: aiohttp.ClientSession
-    ) -> Result | None:
-        visitor = FakeVisitor()
-        context = Context(session=session, url=url, visitor=visitor)
-        await self.visit(url, context)
-        return context.result
+        self, session: aiohttp.ClientSession, url: str
+    ) -> Optional[Result]:
+        async with self.throttle:
+            visitor = FakeVisitor()
+            context = Context(session=session, visitor=visitor)
+            id = await self.resolve_id(context, url)
+            if id is None:
+                return None
+            await self.visit(context, id)
+            return context.result
```

### Comparing `iwashi-2.2.2/src/iwashi/visitors/booth.py` & `iwashi-3.0.0/src/iwashi/service/booth.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,46 @@
 import re
 
 import bs4
 
-from iwashi.helper import HTTP_REGEX
-from iwashi.visitor import Context, SiteVisitor
+from iwashi.helper import HTTP_REGEX, normalize_url
+from iwashi.visitor import Context, Service
 
 
-class Booth(SiteVisitor):
-    NAME = "Booth"
-    URL_REGEX: re.Pattern = re.compile(
-        HTTP_REGEX + r"(?P<id>[\w-]+)\.booth\.pm", re.IGNORECASE
-    )
-
-    async def normalize(self, context: Context, url: str) -> str:
-        match = self.URL_REGEX.match(url)
-        if match is None:
-            return url
-        return f'https://{match.group("id")}.booth.pm'
+class Booth(Service):
+    def __init__(self) -> None:
+        super().__init__(
+            name="Booth",
+            regex=re.compile(HTTP_REGEX + r"(?P<id>[\w-]+)\.booth\.pm", re.IGNORECASE),
+        )
 
-    async def visit(self, url, context: Context, id: str):
-        res = await context.session.get(f"https://{id}.booth.pm")
+    async def visit(self, context: Context, id: str) -> None:
+        url = f"https://{id}.booth.pm"
+        res = await context.session.get(url)
+        res.raise_for_status()
         soup = bs4.BeautifulSoup(await res.text(), "html.parser")
-        name_element = soup.select_one(".home-link-container__nickname")
-        name = name_element is not None and name_element.find("a") or None
-        desc_element = soup.select_one(".description")
-        description = (
-            desc_element is not None
-            and desc_element.find(attrs={"v-html": "formattedDescription"})
-            or None
-        )
+        name_element = soup.select_one(".shop-name")
+        name = name_element.text if name_element is not None else None
+        desc_element = soup.select_one(".booth-description .autolink")
+        description = desc_element.text if desc_element is not None else None
         avater_element = soup.select_one(".avatar-image")
 
         context.create_result(
-            "Booth",
+            self,
+            id=id,
             url=url,
-            name=name.text if name is not None else None,
-            description=description.text if description is not None else None,
+            name=name,
+            description=description,
             profile_picture=avater_element.attrs["style"].split("url(")[1].split(")")[0]
             if avater_element is not None
             else None,
         )
 
         if desc_element is None:
             return
-        for link in desc_element.select(".shop-contacts__link"):
-            link = link.select_one("a")
-            if link is None:
+        for link in soup.select(".booth-description a"):
+            if "href" not in link.attrs:
+                continue
+            normalized_url = normalize_url(link.attrs["href"])
+            if normalized_url is None:
                 continue
-            if "href" in link.attrs:
-                context.enqueue_visit(link.attrs["href"])
+            context.enqueue_visit(normalized_url)
```

### Comparing `iwashi-2.2.2/src/iwashi/visitors/fanbox.py` & `iwashi-3.0.0/src/iwashi/service/fanbox.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,45 @@
 import re
 from typing import List, TypedDict
 
 from loguru import logger
 
 from iwashi.helper import HTTP_REGEX
-from iwashi.visitor import Context, SiteVisitor
+from iwashi.visitor import Context, Service
 
 
-class Fanbox(SiteVisitor):
-    NAME = "Fanbox"
-    URL_REGEX: re.Pattern = re.compile(
-        HTTP_REGEX + r"(?P<id>[\w-]+)\.fanbox\.cc", re.IGNORECASE
-    )
-
-    async def normalize(self, context: Context, url: str) -> str:
-        match = self.URL_REGEX.match(url)
-        if match is None:
-            return url
-        return f'https://{match.group("id")}.fanbox.cc'
+class Fanbox(Service):
+    def __init__(self) -> None:
+        super().__init__(
+            name="Fanbox",
+            regex=re.compile(HTTP_REGEX + r"(?P<id>[\w-]+)\.fanbox\.cc", re.IGNORECASE),
+        )
 
-    async def visit(self, url, context: Context, id: str):
+    async def visit(self, context: Context, id: str):
         url = f"https://{id}.fanbox.cc"
         creator_res = await context.session.get(
             f"https://api.fanbox.cc/creator.get?creatorId={id}",
             headers={
                 "accept": "application/json",
                 "origin": f"https://{id}.fanbox.cc",
                 "referer": f"https://{id}.fanbox.cc/",
             },
         )
+        creator_res.raise_for_status()
         if creator_res.status // 100 == 4:
             logger.warning(f"[Fanbox] Could not find user for {url}")
             return
 
         info: Root = await creator_res.json()
         if "error" in info:
             logger.warning(f"[Fanbox] Could not find user for {url}")
             return
         context.create_result(
-            "Fanbox",
+            self,
+            id=id,
             url=url,
             name=info["body"]["user"]["name"],
             description=info["body"]["description"],
             profile_picture=info["body"]["user"]["iconUrl"],
         )
 
         for link in info["body"]["profileLinks"]:
```

### Comparing `iwashi-2.2.2/src/iwashi/visitors/instagram.py` & `iwashi-3.0.0/src/iwashi/service/instagram.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,159 +1,162 @@
 import re
 from typing import List, TypedDict
 
-import aiohttp
 from loguru import logger
 
-from iwashi.helper import BASE_HEADERS, HTTP_REGEX
-from iwashi.visitor import Context, SiteVisitor
+from iwashi.helper import HTTP_REGEX
+from iwashi.visitor import Context, Service
 
 
-class Instagram(SiteVisitor):
-    NAME = "Instagram"
-    URL_REGEX: re.Pattern = re.compile(
-        HTTP_REGEX + r"instagram\.com/(?P<id>\w+)", re.IGNORECASE
-    )
-
-    async def normalize(self, context: Context, url: str) -> str:
-        match = self.URL_REGEX.match(url)
-        if match is None:
-            return url
-        return f'https://www.instagram.com/{match.group("id")}'
-
-    async def visit(self, url, context: Context, id: str):
-        session = aiohttp.ClientSession(
-            headers={
-                "authority": "www.instagram.com",
-                "accept": "*/*",
-                "accept-language": "en-US,en;q=0.9",
-                "referer": f"https://www.instagram.com/{id}/",
-                "sec-ch-prefers-color-scheme": "dark",
-                "sec-ch-ua": '"Not?A_Brand";v="8", "Chromium";v="108", "Microsoft Edge";v="108"',
-                "sec-fetch-dest": "empty",
-                "sec-fetch-mode": "cors",
-                "sec-fetch-site": "same-origin",
-                "x-asbd-id": "198387",
-                "x-ig-www-claim": "0",
-                "x-requested-with": "XMLHttpRequest",
-            }
-            | BASE_HEADERS,
+class Instagram(Service):
+    def __init__(self) -> None:
+        super().__init__(
+            name="Instagram",
+            regex=re.compile(HTTP_REGEX + r"instagram\.com/(?P<id>\w+)", re.IGNORECASE),
         )
 
-        url = f"https://www.instagram.com/{id}/"
+    async def visit(self, context: Context, id: str):
+        url = f"https://www.instagram.com/{id}"
         res = await context.session.get(url)
+        res.raise_for_status()
         match = re.search(r"\"X-IG-App-ID\": ?\"(?P<id>\d{15})\"", await res.text())
         if match is None:
-            logger.warning(f"[Instagram] No X-IG-App-ID found in {url}")
-            return
+            raise Exception(f"[Instagram] No X-IG-App-ID found in {url}")
         context.session.headers["x-ig-app-id"] = match.group("id")
 
-        csrf_res = await context.session.get(
-            "https://www.instagram.com/ajax/bz?__d=dis"
-        )
-        session.headers.add("x-csrftoken", str(csrf_res.cookies["csrftoken"]))
-
         info_res = await context.session.get(
             f"https://www.instagram.com/api/v1/users/web_profile_info/?username={id}",
         )
+        info_res.raise_for_status()
         if info_res.status // 100 != 2 or info_res.history:
             logger.warning("[Instagram] Blocked by Instagram")
             context.create_result(
-                "Instagram",
+                self,
+                id=id,
                 url=url,
                 name=id,
                 description="Blocked by Instagram",
             )
             return
         info: Root = await info_res.json()
         user = info["data"]["user"]
-        context.create_result("Instagram", url=url, description=user["biography"])
+        context.create_result(
+            self,
+            id=id,
+            url=url,
+            name=user["full_name"],
+            profile_picture=user["profile_pic_url"],
+            description=user["biography"],
+        )
 
         for link in user["bio_links"]:
             context.enqueue_visit(link["url"])
 
 
-class BioLinksItem0(TypedDict):
-    title: str
-    lynx_url: str
+class FriendshipStatus(TypedDict):
+    following: bool
+    blocking: bool
+    is_bestie: bool
+    is_feed_favorite: bool
+    is_restricted: bool
+    muting: bool
+    is_muting_reel: bool
+    outgoing_request: bool
+    followed_by: bool
+    incoming_request: bool
+
+
+class HdProfilePicUrlInfo(TypedDict):
     url: str
-    link_type: str
 
 
 class BiographyWithEntities(TypedDict):
-    raw_text: str
     entities: List
 
 
-class EdgeFollowedBy(TypedDict):
-    count: int
-
-
-class EdgeMutualFollowedBy(TypedDict):
-    count: int
-    edges: List
+class BioLinksItem(TypedDict):
+    link_type: str
+    lynx_url: str
+    title: str
+    url: str
 
 
 class User(TypedDict):
-    biography: str
-    bio_links: List[BioLinksItem0]
+    friendship_status: FriendshipStatus
+    full_name: str
+    gating: None
+    is_memorialized: bool
+    is_private: bool
+    has_story_archive: None
+    username: str
+    is_regulated_c18: bool
+    regulated_news_in_locations: List
+    text_post_app_badge_label: str
+    show_text_post_app_badge: bool
+    eligible_for_text_app_activation_badge: bool
+    hide_text_app_activation_badge_on_text_app: bool
+    pk: str
+    live_broadcast_visibility: None
+    live_broadcast_id: None
+    profile_pic_url: str
+    hd_profile_pic_url_info: HdProfilePicUrlInfo
+    is_unpublished: bool
+    mutual_followers_count: int
+    profile_context_links_with_user_ids: List
     biography_with_entities: BiographyWithEntities
-    blocked_by_viewer: bool
-    restricted_by_viewer: None
-    country_block: bool
+    account_badges: List
+    bio_links: List[BioLinksItem]
+    external_lynx_url: str
     external_url: str
-    external_url_linkshimmed: str
-    edge_followed_by: EdgeFollowedBy
-    fbid: str
-    followed_by_viewer: bool
-    edge_follow: EdgeFollowedBy
-    follows_viewer: bool
-    full_name: str
-    group_metadata: None
-    has_ar_effects: bool
-    has_clips: bool
-    has_guides: bool
-    has_channel: bool
-    has_blocked_viewer: bool
-    highlight_reel_count: int
-    has_requested_viewer: bool
-    hide_like_and_view_counts: bool
-    id: str
-    is_business_account: bool
-    is_professional_account: bool
-    is_supervision_enabled: bool
-    is_guardian_of_viewer: bool
-    is_supervised_by_viewer: bool
-    is_supervised_user: bool
+    ai_agent_type: None
+    has_chaining: bool
+    fbid_v2: str
+    supervision_info: None
+    interop_messaging_user_fbid: str
+    account_type: int
+    biography: str
     is_embeds_disabled: bool
-    is_joined_recently: bool
-    guardian_id: None
-    business_address_json: None
-    business_contact_method: str
-    business_email: None
-    business_phone_number: None
-    business_category_name: None
-    overall_category_name: None
-    category_enum: None
-    category_name: str
-    is_private: bool
+    show_account_transparency_details: bool
     is_verified: bool
-    edge_mutual_followed_by: EdgeMutualFollowedBy
-    profile_pic_url: str
-    profile_pic_url_hd: str
-    requested_by_viewer: bool
+    is_professional_account: None
+    follower_count: int
+    address_street: str
+    city_name: str
+    is_business: bool
+    zip: str
+    category: str
     should_show_category: bool
-    should_show_public_contacts: bool
-    transparency_label: None
-    transparency_product: str
-    username: str
-    connected_fb_page: None
     pronouns: List
+    transparency_label: None
+    transparency_product: None
+    following_count: int
+    media_count: int
+    latest_reel_media: int
+    total_clips_count: int
+    latest_besties_reel_media: int
+    reel_media_seen_timestamp: int
+    id: str
+
+
+class User0(TypedDict):
+    pk: str
+    id: str
+    can_see_organic_insights: bool
+    has_onboarded_to_text_post_app: bool
+
+
+class Viewer(TypedDict):
+    user: User0
 
 
 class Data(TypedDict):
     user: User
+    viewer: Viewer
+
+
+class Extensions(TypedDict):
+    is_final: bool
 
 
 class Root(TypedDict):
     data: Data
-    status: str
+    extensions: Extensions
```

### Comparing `iwashi-2.2.2/src/iwashi/visitors/linktree.py` & `iwashi-3.0.0/src/iwashi/service/linktree.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,36 @@
 import json
 import re
 from typing import List, Optional, TypedDict, Union
 
 import bs4
 
 from iwashi.helper import HTTP_REGEX
-from iwashi.visitor import Context, SiteVisitor
+from iwashi.visitor import Context, Service
 
 
-class Linktree(SiteVisitor):
-    NAME = "Linktree"
-    URL_REGEX: re.Pattern = re.compile(
-        HTTP_REGEX + r"linktr\.ee/(?P<id>\w+)", re.IGNORECASE
-    )
-
-    async def normalize(self, context: Context, url: str) -> str:
-        match = self.URL_REGEX.match(url)
-        if match is None:
-            return url
-        return f'https://linktr.ee/{match.group("id")}'
-
-    async def visit(self, url, context: Context, id: str):
-        res = await context.session.get(
-            f"https://linktr.ee/{id}",
+class Linktree(Service):
+    def __init__(self) -> None:
+        super().__init__(
+            name="Linktree",
+            regex=re.compile(HTTP_REGEX + r"linktr\.ee/(?P<id>\w+)", re.IGNORECASE),
         )
-        if res.status != 200:
-            return None
+
+    async def visit(self, context: Context, id: str):
+        url = f"https://linktr.ee/{id}"
+        res = await context.session.get(url)
+        res.raise_for_status()
         soup = bs4.BeautifulSoup(await res.text(), "html.parser")
         data_element = soup.find(attrs={"id": "__NEXT_DATA__"})
         assert data_element
         data: Root = json.loads(data_element.get_text())
         info = data["props"]["pageProps"]
         context.create_result(
-            "Linktree",
+            self,
+            id=id,
             url=url,
             description=info["description"],
             profile_picture=info["profilePictureUrl"],
         )
         links = info["links"]
         for link in links:
             if not link["url"]:
```

### Comparing `iwashi-2.2.2/src/iwashi/visitors/litlink.py` & `iwashi-3.0.0/src/iwashi/service/litlink.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,53 +4,56 @@
 import re
 from typing import Dict, List, TypedDict, Union
 
 import bs4
 from loguru import logger
 
 from iwashi.helper import HTTP_REGEX
-from iwashi.visitor import Context, SiteVisitor
+from iwashi.visitor import Context, Service
 
 
-class LitLink(SiteVisitor):
-    NAME = "LitLink"
-    URL_REGEX: re.Pattern = re.compile(
-        HTTP_REGEX + r"lit\.link/(?P<id>\w+)", re.IGNORECASE
-    )
-
-    async def normalize(self, context: Context, url: str) -> str:
-        match = self.URL_REGEX.match(url)
-        if match is None:
-            return url
-        return f'https://lit.link/{match.group("id")}'
-
-    async def visit(self, url, context: Context, id: str):
-        res = await context.session.get(
-            f"https://lit.link/{id}",
+class LitLink(Service):
+    def __init__(self) -> None:
+        super().__init__(
+            name="LitLink",
+            regex=re.compile(HTTP_REGEX + r"lit\.link/(?P<id>\w+)", re.IGNORECASE),
         )
+
+    async def visit(self, context: Context, id: str):
+        url = f"https://lit.link/{id}"
+        res = await context.session.get(url)
+        res.raise_for_status()
         soup = bs4.BeautifulSoup(await res.text(), "html.parser")
         data_element = soup.find(attrs={"id": "__NEXT_DATA__"})
         if data_element is None:
             logger.warning(f"[LitLink] Could not find data element for {url}")
             return
         data: Root = json.loads(data_element.get_text())
         profile = data["props"]["pageProps"]["profile"]
 
         context.create_result(
-            "LitLink",
+            self,
+            id=id,
             url=url,
             name=profile["name"],
             description=profile["profileText"],
             profile_picture=profile["pictureUrl"],
         )
 
         for link in profile["snsIconLinks"]:
             if "url" not in link:
                 continue
             context.enqueue_visit(link["url"])
+        for link in profile["profileLinks"]:
+            if "buttonLink" not in link:
+                continue
+            button_link = link["buttonLink"]
+            if button_link is None:
+                continue
+            context.enqueue_visit(button_link["url"])
 
 
 class SnsiconlinksItem(TypedDict):
     id: str
     type: str
     url: str
     userId: str
```

### Comparing `iwashi-2.2.2/src/iwashi/visitors/mirrativ.py` & `iwashi-3.0.0/src/iwashi/service/mirrativ.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,57 +2,55 @@
 
 import re
 from typing import Dict, List, TypedDict, Union
 
 import bs4
 
 from iwashi.helper import BASE_HEADERS, HTTP_REGEX
-from iwashi.visitor import Context, SiteVisitor
+from iwashi.visitor import Context, Service
 
 
-class Mirrativ(SiteVisitor):
-    NAME = "Mirrative"
-    URL_REGEX: re.Pattern = re.compile(
-        HTTP_REGEX + r"mirrativ.com/user/(?P<id>[\d]+)", re.IGNORECASE
-    )
-
-    async def normalize(self, context: Context, url: str) -> str:
-        match = self.URL_REGEX.match(url)
-        if match is None:
-            return url
-        return f'https://mirrativ.com/user/{match.group("id")}'
+class Mirrativ(Service):
+    def __init__(self):
+        super().__init__(
+            name="Mirrativ",
+            regex=re.compile(
+                HTTP_REGEX + r"mirrativ.com/user/(?P<id>[\d]+)", re.IGNORECASE
+            ),
+        )
 
     async def fetch_scrf_token(self, context: Context) -> str | None:
-        res = await context.session.get(
-            "https://www.mirrativ.com/",
-        )
+        res = await context.session.get("https://www.mirrativ.com/")
+        res.raise_for_status()
         soup = bs4.BeautifulSoup(await res.text(), "html.parser")
         element = soup.select_one('meta[name="csrf-token"]')
         if element is None:
             raise RuntimeError("Could not find csrf-token")
         return element.attrs.get("content")
 
-    async def visit(self, url, context: Context, id: str):
-        url = f"https://www.mirrativ.com/api/user/profile?user_id={id}"
+    async def visit(self, context: Context, id: str):
+        url = f"https://www.mirrativ.com/user/{id}"
 
         headers = BASE_HEADERS | {
             "accept": "application/json",
-            "x-csrf-token": self.fetch_scrf_token(context),
+            "x-csrf-token": await self.fetch_scrf_token(context),
         }
 
         res = await context.session.get(
             "https://www.mirrativ.com/api/user/profile",
             params={
                 "user_id": id,
             },
             headers=headers,
         )
+        res.raise_for_status()
         info: Root = await res.json()
         context.create_result(
-            "Mirrativ",
+            self,
+            id=id,
             url=url,
             name=info["name"],
             description=info["description"],
             profile_picture=info["profile_image_url"],
         )
 
         for link in info["links"]:
```

### Comparing `iwashi-2.2.2/src/iwashi/visitors/nicovideo.py` & `iwashi-3.0.0/src/iwashi/service/nicovideo.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,50 +2,54 @@
 import re
 from typing import List, TypedDict
 
 import bs4
 from loguru import logger
 
 from iwashi.helper import HTTP_REGEX
-from iwashi.visitor import Context, SiteVisitor
+from iwashi.visitor import Context, Service
 
 
-class Nicovideo(SiteVisitor):
-    NAME = "Nicovideo"
-    URL_REGEX: re.Pattern = re.compile(
-        HTTP_REGEX + r"(sp\.)?nicovideo\.jp/(?P<path>user|mylist)/(?P<id>\d+)",
-        re.IGNORECASE,
-    )
+class Nicovideo(Service):
+    def __init__(self) -> None:
+        super().__init__(
+            name="Nicovideo",
+            regex=re.compile(
+                HTTP_REGEX + r"(sp\.)?nicovideo\.jp/(?P<path>user|mylist)/(?P<id>\d+)",
+                re.IGNORECASE,
+            ),
+        )
 
-    async def normalize(self, context: Context, url: str) -> str:
-        match = self.URL_REGEX.match(url)
+    async def resolve_id(self, context: Context, url: str) -> str:
+        match = self.regex.match(url)
         if match is None:
             return url
         if match.group("path") == "mylist":
             res = await context.session.get(
                 f'https://www.nicovideo.jp/mylist/{match.group("id")}'
             )
-            return await self.normalize(context, str(res.url))
-        return f'nicovideo.jp/user/{match.group("id")}'
+            res.raise_for_status()
+            return await self.resolve_id(context, str(res.url))
+        return match.group("id")
 
-    async def visit(self, url, context: Context, path: str, id: str):
+    async def visit(self, context: Context, id: str):
         url = f"https://www.nicovideo.jp/user/{id}"
-        res = await context.session.get(
-            f"https://www.nicovideo.jp/user/{id}",
-        )
+        res = await context.session.get(f"https://www.nicovideo.jp/user/{id}")
+        res.raise_for_status()
         soup = bs4.BeautifulSoup(await res.text(), "html.parser")
         element = soup.select_one("#js-initial-userpage-data")
         if element is None:
             logger.warning(f"[Nicovideo] {id} not found")
             return None
 
         info: Root = json.loads(element.attrs["data-initial-data"])
         user = info["state"]["userDetails"]["userDetails"]["user"]
         context.create_result(
-            "Nicovideo",
+            self,
+            id=id,
             url=url,
             name=user["nickname"],
             description=user["description"],
             profile_picture=user["icons"]["large"],
         )
 
         for link in user["sns"]:
```

### Comparing `iwashi-2.2.2/src/iwashi/visitors/note.py` & `iwashi-3.0.0/src/iwashi/service/note.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 from __future__ import annotations
 
 import json
 import re
-from typing import TypedDict
+from typing import List, TypedDict
 
 import bs4
 
 from iwashi.helper import HTTP_REGEX
-from iwashi.visitor import Context, SiteVisitor
+from iwashi.visitor import Context, Service
 
 
-class Note(SiteVisitor):
-    NAME = "Note"
-    URL_REGEX: re.Pattern = re.compile(
-        HTTP_REGEX + r"note\.com/(?P<user>[^/]+)", re.IGNORECASE
-    )
-
-    async def normalize(self, context: Context, url: str) -> str:
-        match = self.URL_REGEX.match(url)
-        if match is None:
-            return url
-        return f"https://note.com/{match.group('user')}"
-
-    async def visit(self, url: str, context: Context, user: str):
-        res = await context.session.get(
-            url,
+class Note(Service):
+    def __init__(self):
+        super().__init__(
+            name="Note",
+            regex=re.compile(HTTP_REGEX + r"note\.com/(?P<id>[^/]+)", re.IGNORECASE),
         )
+
+    async def visit(self, context: Context, id: str):
+        url = f"https://note.com/{id}"
+        res = await context.session.get(url)
+        res.raise_for_status()
         soup = bs4.BeautifulSoup(await res.text(), "html.parser")
 
         data_element = soup.select_one("script[type='application/ld+json']")
         if data_element is None:
             return
-        data: Root = json.loads(data_element.text)
+        data_root: Root = json.loads(data_element.text)
+        if len(data_root) != 1:
+            raise Exception("Root element is not unique")
+        data = data_root[0]["mainEntity"]
 
         context.create_result(
-            "Note",
+            self,
+            id=id,
             url=url,
-            name=data["headline"],
+            name=data["name"],
             description=data["description"],
             profile_picture=data["image"]["url"],
         )
 
         links: set[str] = set()
         for element in soup.select(".m-creatorSocialLinks__item"):
             link = element.select_one("a")
@@ -49,30 +48,30 @@
             if "href" not in link.attrs:
                 continue
             links.add(link.attrs["href"])
         for link in links:
             context.enqueue_visit(link)
 
 
-Author = TypedDict("author", {"@type": "str", "name": "str", "url": "str"})
-Logo = TypedDict(
-    "logo", {"@type": "str", "url": "str", "width": "str", "height": "str"}
-)
-Publisher = TypedDict("publisher", {"@type": "str", "name": "str", "logo": "Logo"})
 Image = TypedDict(
-    "image", {"@type": "str", "url": "str", "width": "int", "height": "int"}
+    "Image", {"@type": "str", "url": "str", "width": "int", "height": "int"}
 )
-Root = TypedDict(
-    "Root",
+Mainentity = TypedDict(
+    "Mainentity",
     {
-        "@context": "str",
         "@type": "str",
-        "mainEntityOfPage": "str",
-        "headline": "str",
-        "datePublished": "str",
-        "dateModified": "str",
-        "author": "Author",
-        "publisher": "Publisher",
+        "name": "str",
+        "url": "str",
         "image": "Image",
         "description": "str",
     },
 )
+RootItem = TypedDict(
+    "RootItem",
+    {
+        "@context": "str",
+        "@type": "str",
+        "dateCreated": "str",
+        "mainEntity": "Mainentity",
+    },
+)
+Root = List[RootItem]
```

### Comparing `iwashi-2.2.2/src/iwashi/visitors/pixiv.py` & `iwashi-3.0.0/src/iwashi/service/pixiv.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,33 +2,30 @@
 import re
 from typing import Dict, List, Optional, TypeAlias, TypedDict
 
 import bs4
 from loguru import logger
 
 from iwashi.helper import HTTP_REGEX
-from iwashi.visitor import Context, SiteVisitor
+from iwashi.visitor import Context, Service
 
 
-class Pixiv(SiteVisitor):
-    NAME = "Pixiv"
-    URL_REGEX: re.Pattern = re.compile(
-        HTTP_REGEX + r"pixiv\.net/users/(?P<id>\d+)", re.IGNORECASE
-    )
-
-    async def normalize(self, context: Context, url: str) -> str:
-        match = self.URL_REGEX.match(url)
-        if match is None:
-            return url
-        return f'https://pixiv.net/users/{match.group("id")}'
-
-    async def visit(self, url, context: Context, id: str):
-        res = await context.session.get(
-            f"https://pixiv.net/users/{id}",
+class Pixiv(Service):
+    def __init__(self):
+        super().__init__(
+            name="Pixiv",
+            regex=re.compile(
+                HTTP_REGEX + r"pixiv\.net/users/(?P<id>\d+)", re.IGNORECASE
+            ),
         )
+
+    async def visit(self, context: Context, id: str):
+        url = f"https://www.pixiv.net/users/{id}"
+        res = await context.session.get(url)
+        res.raise_for_status()
         soup = bs4.BeautifulSoup(await res.text(), "html.parser")
         meta_element = soup.select_one(
             'meta[name="preload-data"][id="meta-preload-data"]'
         )
         if meta_element is None:
             logger.warning(f"[Pixiv] meta-preload-data not found: {id}")
             return
@@ -36,29 +33,31 @@
 
         if len(info["user"].values()) > 1:
             logger.warning(f"[Pixiv] User is must be unique: {id}")
             return
 
         for user in info["user"].values():
             context.create_result(
-                "Pixiv",
+                self,
+                id=id,
                 url=url,
                 name=user["name"],
                 description=user["comment"],
                 profile_picture=user["imageBig"],
             )
             if "webpage" in user and user["webpage"] is not None:
                 context.enqueue_visit(user["webpage"])
             if user["social"]:
                 for link in user["social"].values():
                     context.enqueue_visit(link["url"])
 
             resp = await context.session.get(
                 f"https://sketch.pixiv.net/api/pixiv/user/posts/latest?user_id={id}"
             )
+            res.raise_for_status()
             if resp.status == 200:
                 data = await resp.json()
                 context.enqueue_visit(data["data"]["user"]["url"])
 
 
 class Background(TypedDict):
     repeat: None
```

### Comparing `iwashi-2.2.2/src/iwashi/visitors/reddit.py` & `iwashi-3.0.0/src/iwashi/service/reddit.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,46 +3,43 @@
 import json
 import re
 from typing import List, TypedDict
 
 import bs4
 
 from iwashi.helper import HTTP_REGEX
-from iwashi.visitor import Context, SiteVisitor
+from iwashi.visitor import Context, Service
 
 
-class Reddit(SiteVisitor):
-    NAME = "Reddit"
-    URL_REGEX: re.Pattern = re.compile(
-        HTTP_REGEX + r"reddit\.com/user/(?P<id>[\w-]+)", re.IGNORECASE
-    )
-
-    async def normalize(self, context: Context, url: str) -> str:
-        match = self.URL_REGEX.match(url)
-        if match is None:
-            return url
-        return f'https://reddit.com/user/{match.group("id")}'
-
-    async def visit(self, url, context: Context, id: str):
-        res = await context.session.get(
-            f"https://www.reddit.com/user/{id}/about.json",
+class Reddit(Service):
+    def __init__(self):
+        super().__init__(
+            name="Reddit",
+            regex=re.compile(
+                HTTP_REGEX + r"reddit\.com/user/(?P<id>[\w-]+)", re.IGNORECASE
+            ),
         )
+
+    async def visit(self, context: Context, id: str):
+        url = f"https://www.reddit.com/user/{id}"
+        res = await context.session.get(f"https://www.reddit.com/user/{id}/about.json")
+        res.raise_for_status()
         info: Root = await res.json()
 
         context.create_result(
-            "Reddit",
+            self,
+            id=id,
             url=url,
             name=info["data"]["name"],
             description=info["data"]["subreddit"]["public_description"],
             profile_picture=info["data"]["icon_img"],
         )
 
-        res = await context.session.get(
-            f"https://www.reddit.com/user/{id}/",
-        )
+        res = await context.session.get(f"https://www.reddit.com/user/{id}/")
+        res.raise_for_status()
         soup = bs4.BeautifulSoup(await res.text(), "html.parser")
         # noun="social_link"
         for element in soup.select('[noun="social_link"]'):
             data: SocialLink = json.loads(
                 element.attrs["data-faceplate-tracking-context"]
             )
             context.enqueue_visit(data["social_link"]["url"])
```

### Comparing `iwashi-2.2.2/src/iwashi/visitors/soundcloud.py` & `iwashi-3.0.0/src/iwashi/service/soundcloud.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 import json
 import re
 from typing import List, TypedDict
 
 from loguru import logger
 
 from iwashi.helper import HTTP_REGEX
-from iwashi.visitor import Context, SiteVisitor
+from iwashi.visitor import Context, Service
 
 
-class Soundcloud(SiteVisitor):
-    NAME = "Soundcloud"
-    URL_REGEX: re.Pattern = re.compile(
-        HTTP_REGEX + r"soundcloud\.com/(?P<id>[-\w]+)", re.IGNORECASE
-    )
-
-    async def normalize(self, context: Context, url: str) -> str:
-        match = self.URL_REGEX.match(url)
-        if match is None:
-            return url
-        return f'https://soundcloud.com/{match.group("id")}'
+class Soundcloud(Service):
+    def __init__(self) -> None:
+        super().__init__(
+            name="Soundcloud",
+            regex=re.compile(
+                HTTP_REGEX + r"soundcloud\.com/(?P<id>[-\w]+)", re.IGNORECASE
+            ),
+        )
 
-    async def visit(self, url, context: Context, id: str):
+    async def visit(self, context: Context, id: str):
         url = f"https://soundcloud.com/{id}"
-        res = await context.session.get(
-            url,
-        )
+        res = await context.session.get(url)
+        res.raise_for_status()
         info_json = re.search(
             r"window\.__sc_hydration ?= ?(?P<info>.+);", await res.text()
         )
         if info_json is None:
             logger.warning(f"[Soundcloud] Could not find info for {url}")
             return
         info_list: Root = json.loads(info_json.group("info"))
@@ -36,24 +32,26 @@
             if info["hydratable"] == "user":
                 break
         else:
             logger.warning(f"[Soundcloud] Could not find user info for {url}")
             return
 
         context.create_result(
-            "Soundcloud",
+            self,
+            id=id,
             url=url,
             name=info["data"]["username"],
             description=info["data"]["description"],
             profile_picture=info["data"]["avatar_url"],
         )
 
         client_id_res = await context.session.get(
-            "https://a-v2.sndcdn.com/assets/0-bf97f26a.js",
+            "https://a-v2.sndcdn.com/assets/0-bf97f26a.js"
         )
+        client_id_res.raise_for_status()
         match = re.search(
             r"client_id: ?\"(?P<client_id>\w{32})\"", await client_id_res.text()
         )
         if match is None:
             logger.warning(f"[Soundcloud] Could not find client_id for {url}")
             return
         client_id = match.group("client_id")
@@ -82,14 +80,15 @@
         }
 
         profile_res = await context.session.get(
             f'https://api-v2.soundcloud.com/users/{info["data"]["urn"]}/web-profiles',
             params=params,
             headers=headers,
         )
+        profile_res.raise_for_status()
         profile: List[ProfileItem] = await profile_res.json()
         for item in profile:
             context.enqueue_visit(item["url"])
 
 
 class ProfileItem(TypedDict):
     url: str
```

### Comparing `iwashi-2.2.2/src/iwashi/visitors/spotify.py` & `iwashi-3.0.0/src/iwashi/service/spotify.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,76 +3,77 @@
 
 import re
 from typing import Dict, List, Literal, TypedDict
 
 import bs4
 
 from iwashi.helper import HTTP_REGEX, BASE_HEADERS
-from iwashi.visitor import Context, SiteVisitor
+from iwashi.visitor import Context, Service
 
 
-class Spotify(SiteVisitor):
-    NAME = "Spotify"
-    URL_REGEX: re.Pattern = re.compile(
-        HTTP_REGEX
-        + r"(open\.)?spotify\.com\/(intl-[\w]*\/)?artist\/(?P<artist_id>[0-9a-zA-Z]+)",
-        re.IGNORECASE,
-    )
+class Spotify(Service):
+    def __init__(self):
+        super().__init__(
+            name="Spotify",
+            regex=re.compile(
+                HTTP_REGEX
+                + r"(open\.)?spotify\.com\/(intl-[\w]*\/)?artist\/(?P<id>[0-9a-zA-Z]+)",
+                re.IGNORECASE,
+            ),
+        )
 
     async def extract_access_token(self, soup: bs4.BeautifulSoup) -> str:
         script = soup.select_one("script#session")
         if script is None:
             raise RuntimeError("Token not found")
         data = Session(**json.loads(script.text))
         return data["accessToken"]
 
-    async def normalize(self, context: Context, url: str) -> str:
-        match = self.URL_REGEX.match(url)
-        if match is None:
-            return url
-        return f"https://open.spotify.com/artist/{match.group('artist_id')}"
-
-    async def visit(self, url, context: Context, artist_id: str):
+    async def visit(self, context: Context, id: str):
+        url = f"https://open.spotify.com/artist/{id}"
         response = await context.session.get(url, headers=BASE_HEADERS)
+        response.raise_for_status()
         soup = bs4.BeautifulSoup(await response.text(), "html.parser")
         access_token = await self.extract_access_token(soup)
 
         headers = {
             "accept": "application/json",
             "authorization": f"Bearer {access_token}",
             "content-type": "application/json",
         }
         params = {
             "operationName": "queryArtistOverview",
             "variables": json.dumps(
                 {
-                    "uri": f"spotify:artist:{artist_id}",
+                    "uri": f"spotify:artist:{id}",
                     "locale": "intl-ja",
                     "includePrerelease": True,
                 }
             ),
             "extensions": '{"persistedQuery":{"version":1,"sha256Hash":"da986392124383827dc03cbb3d66c1de81225244b6e20f8d78f9f802cc43df6e"}}',
         }
         response = await context.session.get(
             "https://api-partner.spotify.com/pathfinder/v1/query",
             params=params,
             headers=headers | BASE_HEADERS,
         )
+        response.raise_for_status()
         data: ArtistResponse = await response.json()
         profile = data["data"]["artistUnion"]["profile"]
         avatar_image = data["data"]["artistUnion"]["visuals"]["avatarImage"]
         if len(avatar_image["sources"]) == 0:
             avatar_url = None
         else:
             avatar_url = sorted(
                 avatar_image["sources"], key=lambda x: x["width"] * x["height"]
             )[-1]["url"]
 
         context.create_result(
-            "Spotify",
+            self,
+            id=id,
             url=url,
             name=profile["name"],
             description=profile["biography"]["text"],
             profile_picture=avatar_url,
         )
 
         for link in profile["externalLinks"]["items"]:
```

### Comparing `iwashi-2.2.2/src/iwashi/visitors/tiktok.py` & `iwashi-3.0.0/src/iwashi/service/bandcamp.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,80 +1,60 @@
 from __future__ import annotations
 
 import json
 import re
 from typing import List, TypedDict
 
 import bs4
-from loguru import logger
 
-from iwashi.helper import HTTP_REGEX, normalize_url
-from iwashi.visitor import Context, SiteVisitor
+from iwashi.helper import HTTP_REGEX
+from iwashi.visitor import Context, Service
 
+DATA_REGEX = r"preloadLink\s?=\s(?P<json>{[^;]+)"
 
-class TikTok(SiteVisitor):
-    NAME = "TikTok"
-    URL_REGEX: re.Pattern = re.compile(
-        HTTP_REGEX + r"tiktok\.com/@(?P<id>[-\w]+)", re.IGNORECASE
-    )
-
-    async def normalize(self, context: Context, url: str) -> str:
-        match = self.URL_REGEX.match(url)
-        if match is None:
-            return url
-        return f'https://tiktok.com/@{match.group("id")}'
-
-    async def visit(self, url, context: Context, id: str):
-        url = f"https://tiktok.com/@{id}"
-        res = await context.session.get(
-            url,
+
+class Bandcamp(Service):
+    def __init__(self):
+        super().__init__(
+            name="Bandcamp",
+            regex=re.compile(
+                HTTP_REGEX + r"(?P<id>[\w-]+)?\.bandcamp\.com", re.IGNORECASE
+            ),
         )
-        soup = bs4.BeautifulSoup(await res.text(), "html.parser")
-        # icon: <meta property="og:image"
-        element = soup.select_one('meta[property="og:image"]')
-        profile_picture = None
-        if element is not None:
-            attr = element["content"]
-            if isinstance(attr, str):
-                profile_picture = normalize_url(attr)
-
-        # data: #Person
-        element = soup.select_one("script#Person")
-        if element is None:
-            logger.warning(f"[TikTok] Could not find data for {url}")
-            return
-        data: Root = json.loads(element.text)
 
+    async def visit(self, context: Context, id: str) -> None:
+        url = f"https://{id}.bandcamp.com"
+        res = await context.session.get(url)
+        res.raise_for_status()
+        soup = bs4.BeautifulSoup(await res.text(), "html.parser")
+        script = soup.select_one("script[data-band]")
+        if script is None:
+            raise Exception("No script found")
+
+        data: Root = json.loads(script.attrs["data-band"])
+        description_element = soup.select_one(".signed-out-artists-bio-text")
+        profile_picture_element = soup.select_one(".band-photo")
         context.create_result(
-            "TikTok",
+            self,
+            id=id,
             url=url,
             name=data["name"],
-            description=data["description"],
-            profile_picture=profile_picture,
+            description=description_element.text.strip()
+            if description_element
+            else None,
+            profile_picture=profile_picture_element.attrs["src"]
+            if profile_picture_element
+            else None,
         )
 
+        for site in data["sites"]:
+            context.enqueue_visit(site["url"])
+
+
+class Site(TypedDict):
+    url: str
+    title: str
+
 
-InteractionType = TypedDict("InteractionType", {"@type": "str"})
-InteractionStatisticItem = TypedDict(
-    "InteractionStatisticItem",
-    {
-        "@type": "str",
-        "interactionType": "InteractionType",
-        "userInteractionCount": "int",
-    },
-)
-Mainentityofpage = TypedDict("Mainentityofpage", {"@id": "str", "@type": "str"})
-Root = TypedDict(
-    "Root",
-    {
-        "@context": "str",
-        "@type": "str",
-        "name": "str",
-        "description": "str",
-        "alternateName": "str",
-        "url": "str",
-        "knowsLanguage": "str",
-        "nationality": "str",
-        "interactionStatistic": "List[InteractionStatisticItem]",
-        "mainEntityOfPage": "Mainentityofpage",
-    },
-)
+class Root(TypedDict):
+    sites: List[Site]
+    name: str
```

### Comparing `iwashi-2.2.2/src/iwashi/visitors/twitcasting.py` & `iwashi-3.0.0/src/iwashi/service/twitcasting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,55 @@
 import re
 
 import bs4
 from loguru import logger
 
 from iwashi.helper import HTTP_REGEX, normalize_url
-from iwashi.visitor import Context, SiteVisitor
+from iwashi.visitor import Context, Service
 
 
-class TwitCasting(SiteVisitor):
-    NAME = "TwitCasting"
-    URL_REGEX: re.Pattern = re.compile(
-        HTTP_REGEX + r"twitcasting\.tv/(?P<id>[-\w]+)", re.IGNORECASE
-    )
-
-    async def normalize(self, context: Context, url: str) -> str:
-        match = self.URL_REGEX.match(url)
-        if match is None:
-            return url
-        return f'https://twitcasting.tv/{match.group("id")}'
+class TwitCasting(Service):
+    def __init__(self) -> None:
+        super().__init__(
+            name="TwitCasting",
+            regex=re.compile(
+                HTTP_REGEX + r"twitcasting\.tv/(?P<id>[-\w]+)", re.IGNORECASE
+            ),
+        )
 
-    async def visit(self, url, context: Context, id: str):
+    async def visit(self, context: Context, id: str):
         url = f"https://twitcasting.tv/{id}"
-        res = await context.session.get(
-            url,
-        )
+        res = await context.session.get(url)
+        res.raise_for_status()
         soup = bs4.BeautifulSoup(await res.text(), "html.parser")
-        # name: .tw-user-nav-name
         element = soup.select_one(".tw-user-nav-name")
         if element is None:
             logger.warning(f"[TwitCasting] Could not find name for {url}")
             return
         name = element.text.strip()
-        # icon: .tw-user-nav-icon > img
         element = soup.select_one(".tw-user-nav-icon > img")
         profile_picture = None
         if element is not None:
             attr = element["src"]
             if isinstance(attr, str):
                 profile_picture = normalize_url(attr)
+        description: str | None = None
+        element = soup.select_one('meta[name="description"]')
+        if element is not None:
+            description = element.attrs.get("content")
 
         context.create_result(
-            "TwitCasting",
+            self,
+            id=id,
             url=url,
             name=name,
-            description=None,
+            description=description,
             profile_picture=profile_picture,
         )
 
-        links = set()
+        links = set()  # TODO
         for element in soup.select(".tw-follow-list-row-icon"):
             links.add(element["href"])
         for link in links:
             if link.startswith("/"):
                 continue
             context.enqueue_visit(link)
```

### Comparing `iwashi-2.2.2/src/iwashi/visitors/twitch.py` & `iwashi-3.0.0/src/iwashi/service/twitch.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,27 @@
 import re
 from typing import List, TypedDict
 
 from loguru import logger
 
 from iwashi.helper import HTTP_REGEX
-from iwashi.visitor import Context, SiteVisitor
+from iwashi.visitor import Context, Service
 
 
-class Twitch(SiteVisitor):
-    NAME = "Twitch"
-    URL_REGEX: re.Pattern = re.compile(
-        HTTP_REGEX + r"twitch\.tv/(?P<id>\w+)", re.IGNORECASE
-    )
-
-    async def normalize(self, context: Context, url: str) -> str:
-        match = self.URL_REGEX.match(url)
-        if match is None:
-            return url
-        return f'https://www.twitch.tv/{match.group("id")}'
+class Twitch(Service):
+    def __init__(self) -> None:
+        super().__init__(
+            name="Twitch",
+            regex=re.compile(HTTP_REGEX + r"twitch\.tv/(?P<id>\w+)", re.IGNORECASE),
+        )
 
-    async def visit(self, url, context: Context, id: str):
+    async def visit(self, context: Context, id: str):
         url = f"https://www.twitch.tv/{id}"
-
-        res = await context.session.get(
-            url,
-        )
+        res = await context.session.get(url)
+        res.raise_for_status()
         match = re.search(
             r'clientId ?= ?"(?P<token>kimne78kx3ncx6brgo4mv6wki5h1ko)"',
             await res.text(),
         )
         if match is None:
             logger.warning(f"[Twitch] Could not find token for {url}")
             return
@@ -48,22 +41,23 @@
                     },
                 }
             ],
             headers={
                 "Client-Id": token,
             },
         )
-
+        res.raise_for_status()
         info: Root = await res.json()
         user = info[0]["data"]["user"]
         if user is None:
             logger.warning(f"[Twitch] Could not find user for {url}")
             return
         context.create_result(
-            "Twitch",
+            self,
+            id=id,
             url=url,
             name=user["displayName"],
             description=user["description"],
             profile_picture=user["profileImageURL"],
         )
 
         for link in user["channel"]["socialMedias"]:
```

### Comparing `iwashi-2.2.2/src/iwashi/visitors/twitter.py` & `iwashi-3.0.0/src/iwashi/service/twitter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,64 @@
 import json
 import re
 from typing import List, TypedDict
 
 from loguru import logger
 
 from iwashi.helper import HTTP_REGEX
-from iwashi.visitor import Context, SiteVisitor
+from iwashi.visitor import Context, Service
 
 
-class Twitter(SiteVisitor):
-    NAME = "Twitter"
-    URL_REGEX: re.Pattern = re.compile(
-        HTTP_REGEX + r"(twitter|x)\.com/(#!/)?@?(?P<id>\w+)", re.IGNORECASE
-    )
-
+class Twitter(Service):
     def __init__(self) -> None:
+        super().__init__(
+            name="Twitter",
+            regex=re.compile(
+                HTTP_REGEX + r"(twitter|x)\.com/(#!/)?@?(?P<id>\w+)", re.IGNORECASE
+            ),
+        )
         self.headers = {
             "accept": "*/*",
             "accept-encoding": "gzip, deflate, br",
             "accept-language": "ja",
         }
         self.bearer_token: str | None = None
         self.guest_token: str | None = None
 
-    async def normalize(self, context: Context, url: str) -> str:
-        match = self.URL_REGEX.search(url)
-        if match is None:
-            return url
-        return f'https://twitter.com/{match.group("id")}'
-
     async def fetch_authorization(self, context: Context) -> str:
         if self.bearer_token:
             return self.bearer_token
         res = await context.session.get(
             "https://abs.twimg.com/responsive-web/client-web/main.28fc48ca.js"
         )
+        res.raise_for_status()
         match = re.search('(AAAAA.*?)"', await res.text())
         assert match
         bearer_token = "Bearer " + match.group(1)
         self.bearer_token = bearer_token
         return bearer_token
 
     async def fetch_guest_token(self, context: Context) -> str:
         if self.guest_token:
             return self.guest_token
         res = await context.session.post(
             "https://api.twitter.com/1.1/guest/activate.json",
             headers=self.headers,
         )
+        res.raise_for_status()
         data = await res.json()
         self.guest_token = data["guest_token"]
         return data["guest_token"]
 
     async def setup_headers(self, context: Context) -> None:
         self.headers["authorization"] = await self.fetch_authorization(context)
         self.headers["x-guest-token"] = await self.fetch_guest_token(context)
 
-    async def visit(self, url, context: Context, id: str):
+    async def visit(self, context: Context, id: str) -> None:
+        url = f"https://twitter.com/{id}"
         await self.setup_headers(context)
 
         res = await context.session.get(
             "https://api.twitter.com/graphql/rePnxwe9LZ51nQ7Sn_xN_A/UserByScreenName",
             params={
                 "variables": json.dumps(
                     {
@@ -77,26 +75,33 @@
                         "responsive_web_graphql_skip_user_profile_image_extensions_enabled": False,
                         "responsive_web_graphql_timeline_navigation_enabled": True,
                     }
                 ),
             },
             headers=self.headers,
         )
+        res.raise_for_status()
         info: Root = await res.json()
         if not info["data"]:
             logger.warning(f"[Twitter] Could not find data for {url}")
             return
         result = info["data"]["user"]["result"]
         if result["__typename"] == "UserUnavailable":
-            context.create_result("Twitter", url=url, name="<UserUnavailable>")
+            context.create_result(
+                self,
+                id=id,
+                url=url,
+                name="<UserUnavailable>",
+            )
             return
 
         data = result["legacy"]
         context.create_result(
-            "Twitter",
+            self,
+            id=id,
             url=url,
             name=data["name"],
             description=data["description"],
             profile_picture=data["profile_image_url_https"],
         )
 
         if "url" not in data["entities"]:
```

### Comparing `iwashi-2.2.2/src/iwashi/visitors/youtube/youtube.py` & `iwashi-3.0.0/src/iwashi/service/youtube/youtube.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,83 +1,94 @@
 import json
 import re
 from typing import Tuple
 from urllib import parse
 
 import bs4
 
-from iwashi.helper import BASE_HEADERS, HTTP_REGEX, normalize_url
-from iwashi.visitor import Context, SiteVisitor
+from iwashi.helper import BASE_HEADERS, HTTP_REGEX, traverse
+from iwashi.visitor import Context, Service
 
 from .types import thumbnails, ytinitialdata
 from .types.about import AboutRes
 
+VANITY_ID_REGEX = re.compile(r"youtube.com/@(?P<id>[\w-]+)")
 
-class Youtube(SiteVisitor):
-    NAME = "Youtube"
-    URL_REGEX: re.Pattern = re.compile(
-        HTTP_REGEX + r"((m|gaming)\.)?(youtube\.com|youtu\.be)", re.IGNORECASE
-    )
 
-    async def normalize(self, context: Context, url: str) -> str | None:
+class Youtube(Service):
+    def __init__(self):
+        super().__init__(
+            name="Youtube",
+            regex=re.compile(
+                HTTP_REGEX + r"((m|gaming)\.)?(youtube\.com|youtu\.be)",
+            ),
+        )
+
+    async def resolve_id(self, context: Context, url: str) -> str | None:
         uri = parse.urlparse(url)
         if uri.hostname == "youtu.be":
             return await self._channel_by_video(context, uri.path[1:])
         type = next(filter(None, uri.path.split("/")))
         if type.startswith("@"):
-            return f"https://www.youtube.com/{type}"
+            return self._id_from_vanity_url(url)
         if type == "playlist":
             return None
         if type == "watch":
             return await self._channel_by_video(
                 context, parse.parse_qs(uri.query)["v"][0]
             )
         if type in ("channel", "user", "c"):
             return await self._channel_by_url(context, url)
-        return url
+        return uri.path.split("/")[1]
 
     async def _channel_by_video(self, context: Context, video_id: str) -> str | None:
-        result = await self._channel_by_oembed(
-            context, f"https://www.youtube.com/watch?v={video_id}"
-        )
+        result = await self._channel_by_oembed(context, video_id)
         if result is not None:
             return result
         response = await context.session.get(
             f"https://www.youtube.com/watch?v={video_id}"
         )
-        if response.status == 404:
-            return None
+        response.raise_for_status()
         soup = bs4.BeautifulSoup(await response.text(), "html.parser")
         element = soup.select_one('span[itemprop="author"] > link[itemprop="url"]')
         if element is None:
             return None
-        return normalize_url(element.attrs["href"])
+        href = element.attrs.get("href")
+        if href is None:
+            return None
+        return self._id_from_vanity_url(href)
 
     async def _channel_by_oembed(self, context: Context, video_id: str) -> str | None:
         res = await context.session.get(
             "https://www.youtube.com/oembed",
             params={
                 "url": f"https://www.youtube.com/watch?v={video_id}",
                 "format": "json",
             },
         )
-        if res.status // 100 != 2:
-            return None
+        res.raise_for_status()
         data = await res.json()
-        return normalize_url(data["author_url"])
+        author_url = data.get("author_url")
+        if author_url is None:
+            return None
+        return self._id_from_vanity_url(author_url)
 
     async def _channel_by_url(self, context: Context, url: str) -> str | None:
         res = await context.session.get(url)
-        if res.status == 404:
-            return None
+        res.raise_for_status()
         soup = bs4.BeautifulSoup(await res.text(), "html.parser")
         data = self.extract_initial_data(soup)
-        return normalize_url(
-            data["metadata"]["channelMetadataRenderer"]["vanityChannelUrl"]
-        )
+        vanity_url = data["metadata"]["channelMetadataRenderer"]["vanityChannelUrl"]
+        return self._id_from_vanity_url(vanity_url)
+
+    def _id_from_vanity_url(self, url: str) -> str | None:
+        match = VANITY_ID_REGEX.search(url)
+        if match is None:
+            return None
+        return match.group("id")
 
     def parse_thumbnail(self, thumbnails: thumbnails) -> str:
         size = 0
         url: str | None = None
         for thumbnail in thumbnails["thumbnails"]:
             if thumbnail["width"] > size:
                 size = thumbnail["width"]
@@ -85,63 +96,93 @@
         if url is None:
             raise RuntimeError("Thumbnail not found")
         return url
 
     def parse_token(
         self, data: ytinitialdata
     ) -> Tuple[str | None, Tuple[str, str] | None]:
-        # TODO: 地獄
-        first_link = None
-        c4TabbedHeaderRenderer = data["header"]["c4TabbedHeaderRenderer"]
-        if "headerLinks" not in c4TabbedHeaderRenderer:
+        # FIXME: 地獄
+        first_link: str | None = None
+        # c4TabbedHeaderRenderer = data["header"]["c4TabbedHeaderRenderer"]
+        c4TabbedHeaderRenderer = (
+            traverse(data)
+            .map(lambda x: x.get("header"))
+            .map(lambda x: x.get("c4TabbedHeaderRenderer"))
+            .get()
+        )
+        if (
+            c4TabbedHeaderRenderer is None
+            or "headerLinks" not in c4TabbedHeaderRenderer
+        ):
             return (first_link, None)
-        channelHeaderLinksViewModel = c4TabbedHeaderRenderer["headerLinks"][
-            "channelHeaderLinksViewModel"
-        ]
-        if "firstLink" in channelHeaderLinksViewModel:
-            first_link = channelHeaderLinksViewModel["firstLink"]["commandRuns"][0][
-                "onTap"
-            ]["innertubeCommand"]["urlEndpoint"]["url"]
-        if "more" not in channelHeaderLinksViewModel:
+        first_link = (
+            traverse(c4TabbedHeaderRenderer)
+            .map(lambda x: x.get("headerLinks"))
+            .map(lambda x: x.get("channelHeaderLinksViewModel"))
+            .map(lambda x: x.get("firstLink"))
+            .map(lambda x: x.get("commandRuns"))
+            .map(lambda x: x[0])
+            .map(lambda x: x.get("onTap"))
+            .map(lambda x: x.get("innertubeCommand"))
+            .map(lambda x: x.get("urlEndpoint"))
+            .map(lambda x: x.get("url"))
+            .get()
+        )
+        endpoint = (
+            traverse(c4TabbedHeaderRenderer)
+            .map(lambda x: x.get("headerLinks"))
+            .map(lambda x: x.get("channelHeaderLinksViewModel"))
+            .map(lambda x: x.get("more"))
+            .map(lambda x: x.get("commandRuns"))
+            .map(lambda x: x[0])
+            .map(lambda x: x.get("onTap"))
+            .map(lambda x: x.get("innertubeCommand"))
+            .map(lambda x: x.get("showEngagementPanelEndpoint"))
+            .map(lambda x: x.get("engagementPanel"))
+            .map(lambda x: x.get("engagementPanelSectionListRenderer"))
+            .map(lambda x: x.get("content"))
+            .map(lambda x: x.get("sectionListRenderer"))
+            .map(lambda x: x.get("contents"))
+            .map(lambda x: x[0])
+            .map(lambda x: x.get("itemSectionRenderer"))
+            .map(lambda x: x.get("contents"))
+            .map(lambda x: x[0])
+            .map(lambda x: x.get("continuationItemRenderer"))
+            .map(lambda x: x.get("continuationEndpoint"))
+            .get()
+        )
+        if endpoint is None:
             return (first_link, None)
-        runs = channelHeaderLinksViewModel["more"]["commandRuns"]
-        command = runs[0]["onTap"]["innertubeCommand"]
-        if "showEngagementPanelEndpoint" not in command:
-            raise RuntimeError("token not found")
-        contents1 = command["showEngagementPanelEndpoint"]["engagementPanel"][
-            "engagementPanelSectionListRenderer"
-        ]["content"]["sectionListRenderer"]["contents"]
-        contents2 = contents1[0]["itemSectionRenderer"]["contents"]
-        endpoint = contents2[0]["continuationItemRenderer"]["continuationEndpoint"]
         api_url = endpoint["commandMetadata"]["webCommandMetadata"]["apiUrl"]
         token = endpoint["continuationCommand"]["token"]
         return (first_link, (api_url, token))
 
     def parse_redirect(self, url: str) -> str:
         uri = parse.urlparse(url)
         if uri.hostname != "www.youtube.com":
             return url
         if uri.path == "/redirect":
             return parse.parse_qs(uri.query)["q"][0]
         return url
 
-    async def visit(self, url: str, context: Context):
+    async def visit(self, context: Context, id: str):
+        url = f"https://www.youtube.com/@{id}"
         res = await context.session.get(url)
-        if res.status // 100 != 2:
-            raise RuntimeError(f"HTTP Error: {res.status}")
+        res.raise_for_status()
         soup = bs4.BeautifulSoup(await res.text(), "html.parser")
         data = self.extract_initial_data(soup)
         vanity_id = data["metadata"]["channelMetadataRenderer"]["vanityChannelUrl"]
         name = data["metadata"]["channelMetadataRenderer"]["title"]
         description = data["metadata"]["channelMetadataRenderer"]["description"]
         profile_picture = self.parse_thumbnail(
             data["metadata"]["channelMetadataRenderer"]["avatar"]
         )
         context.create_result(
-            site_name="YouTube",
+            self,
+            id=id,
             url=f"https://www.youtube.com/@{vanity_id.split('@')[1]}",
             name=name,
             description=description,
             profile_picture=profile_picture,
         )
 
         first_link, api = self.parse_token(data)
@@ -163,14 +204,15 @@
                             "clientVersion": "2.20231219.04.00",
                         }
                     },
                     "continuation": token,
                 }
             ),
         )
+        about_res.raise_for_status()
         about_data: AboutRes = await about_res.json()
         links = about_data["onResponseReceivedEndpoints"][0][
             "appendContinuationItemsAction"
         ]["continuationItems"][0]["aboutChannelRenderer"]["metadata"][
             "aboutChannelViewModel"
         ]["links"]
         for link in links:
```

### Comparing `iwashi-2.2.2/src/iwashi/visitors/youtube/types/about.py` & `iwashi-3.0.0/src/iwashi/service/youtube/types/about.py`

 * *Files identical despite different names*

### Comparing `iwashi-2.2.2/src/iwashi/visitors/youtube/types/ytinitialdata.py` & `iwashi-3.0.0/src/iwashi/service/youtube/types/ytinitialdata.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, NotRequired, TypedDict
+from typing import List, TypedDict
 
 
 class thumbnail(TypedDict):
     url: str
     width: int
     height: int
 
@@ -92,16 +92,16 @@
 
 class more(TypedDict):
     content: str
     commandRuns: List[_commandRuns]
 
 
 class channelHeaderLinksViewModel(TypedDict):
-    firstLink: NotRequired[firstLink]
-    more: NotRequired[more]
+    firstLink: firstLink
+    more: more
 
 
 class headerLinks(TypedDict):
     channelHeaderLinksViewModel: channelHeaderLinksViewModel
 
 
 class runs_item(TypedDict):
@@ -113,15 +113,15 @@
 
 
 class c4TabbedHeaderRenderer(TypedDict):
     channelId: str
     title: str
     avatar: thumbnails
     banner: thumbnails
-    headerLinks: NotRequired[headerLinks]
+    headerLinks: headerLinks
     trackingParams: str
     channelHandleText: runs
     style: str
 
 
 class header(TypedDict):
     c4TabbedHeaderRenderer: c4TabbedHeaderRenderer
```

### Comparing `iwashi-2.2.2/LICENSE` & `iwashi-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iwashi-2.2.2/pyproject.toml` & `iwashi-3.0.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "iwashi"
-version = "2.2.2"
+version = "3.0.0"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = ["aiohttp>=3.9.1", "bs4>=0.0.1", "loguru>=0.7.2", "click>=8.1.7"]
 readme = "README.md"
 requires-python = ">= 3.8"
@@ -19,11 +19,12 @@
     "ruff>=0.1.9",
     "typingdict>=0.1.3",
     "build>=1.0.3",
     "strinpy>=0.0.4",
     "astor>=0.8.1",
     "pytest-asyncio>=0.23.5",
     "pytest-cov>=4.1.0",
+    "pyright>=1.1.355",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
```

