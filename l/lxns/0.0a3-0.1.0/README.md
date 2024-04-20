# Comparing `tmp/lxns-0.0a3.tar.gz` & `tmp/lxns-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lxns-0.0a3.tar", last modified: Sun Apr 14 15:28:21 2024, max compression
+gzip compressed data, was "lxns-0.1.0.tar", last modified: Sat Apr 20 15:38:00 2024, max compression
```

## Comparing `lxns-0.0a3.tar` & `lxns-0.1.0.tar`

### file list

```diff
@@ -1,37 +1,40 @@
--rw-r--r--   0        0        0      156 2024-04-14 15:10:09.000000 lxns-0.0a3/.clang-format
--rw-r--r--   0        0        0      717 2024-04-14 15:10:09.000000 lxns-0.0a3/.github/workflows/ci.yaml
--rw-r--r--   0        0        0      140 2024-04-14 15:10:09.000000 lxns-0.0a3/.gitignore
--rw-r--r--   0        0        0      250 2024-04-14 15:10:09.000000 lxns-0.0a3/.readthedocs.yaml
--rw-r--r--   0        0        0      614 2024-04-14 15:10:09.000000 lxns-0.0a3/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2024-04-14 15:10:09.000000 lxns-0.0a3/LICENSES/MIT.txt
--rw-r--r--   0        0        0    16727 2024-04-14 15:10:09.000000 lxns-0.0a3/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0     1214 2024-04-14 15:10:09.000000 lxns-0.0a3/README.md
--rw-r--r--   0        0        0      333 2024-04-14 15:10:09.000000 lxns-0.0a3/docs/conf.py
--rw-r--r--   0        0        0      384 2024-04-14 15:10:09.000000 lxns-0.0a3/docs/index.rst
--rw-r--r--   0        0        0      595 2024-04-14 15:10:09.000000 lxns-0.0a3/docs/mount.rst
--rw-r--r--   0        0        0     2712 2024-04-14 15:10:09.000000 lxns-0.0a3/docs/namespace.rst
--rw-r--r--   0        0        0       92 2024-04-14 15:10:09.000000 lxns-0.0a3/docs/requirements.txt
--rw-r--r--   0        0        0     2191 2024-04-14 15:10:09.000000 lxns-0.0a3/docs/tips_and_tricks.rst
--rw-r--r--   0        0        0     1900 2024-04-14 15:10:09.000000 lxns-0.0a3/examples/add_bind_mount.py
--rw-r--r--   0        0        0     1033 2024-04-14 15:10:09.000000 lxns-0.0a3/examples/join_all_pid_namespaces.py
--rw-r--r--   0        0        0      572 2024-04-14 15:10:09.000000 lxns-0.0a3/examples/process_executor.py
--rw-r--r--   0        0        0      757 2024-04-14 15:10:09.000000 lxns-0.0a3/examples/process_executor_asyncio.py
--rw-r--r--   0        0        0      239 2024-04-14 15:10:09.000000 lxns-0.0a3/meson.build
--rw-r--r--   0        0        0      611 2024-04-14 15:10:09.000000 lxns-0.0a3/meson.options
--rw-r--r--   0        0        0     1215 2024-04-14 15:10:09.000000 lxns-0.0a3/pyproject.toml
--rw-r--r--   0        0        0      110 2024-04-14 15:10:09.000000 lxns-0.0a3/setup.cfg
--rw-r--r--   0        0        0      110 2024-04-14 15:10:09.000000 lxns-0.0a3/src/lxns/__init__.py
--rw-r--r--   0        0        0     1516 2024-04-14 15:10:09.000000 lxns-0.0a3/src/lxns/meson.build
--rw-r--r--   0        0        0     1958 2024-04-14 15:10:09.000000 lxns-0.0a3/src/lxns/mount.py
--rw-r--r--   0        0        0     7789 2024-04-14 15:10:09.000000 lxns-0.0a3/src/lxns/namespaces.py
--rw-r--r--   0        0        0     8753 2024-04-14 15:10:09.000000 lxns-0.0a3/src/lxns/os.c
--rw-r--r--   0        0        0     1556 2024-04-14 15:10:09.000000 lxns-0.0a3/src/lxns/os.py
--rw-r--r--   0        0        0       90 2024-04-14 15:10:09.000000 lxns-0.0a3/src/meson.build
--rw-r--r--   0        0        0       75 2024-04-14 15:10:09.000000 lxns-0.0a3/test/__init__.py
--rw-r--r--   0        0        0      493 2024-04-14 15:10:09.000000 lxns-0.0a3/test/check_typing.py
--rw-r--r--   0        0        0     1101 2024-04-14 15:10:09.000000 lxns-0.0a3/test/test_mount.py
--rw-r--r--   0        0        0     1921 2024-04-14 15:10:09.000000 lxns-0.0a3/test/test_namespaces.py
--rw-r--r--   0        0        0     5958 2024-04-14 15:10:09.000000 lxns-0.0a3/test/test_os.py
--rw-r--r--   0        0        0     4214 2024-04-14 15:10:09.000000 lxns-0.0a3/tools/build_in_container.py
--rw-r--r--   0        0        0     2513 2024-04-14 15:10:09.000000 lxns-0.0a3/tools/run_linters.py
--rw-r--r--   0        0        0     2259 2024-04-14 15:28:21.913429 lxns-0.0a3/PKG-INFO
+-rw-r--r--   0        0        0      156 2024-04-20 15:21:18.000000 lxns-0.1.0/.clang-format
+-rw-r--r--   0        0        0     1261 2024-04-20 15:21:18.000000 lxns-0.1.0/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0      865 2024-04-20 15:21:18.000000 lxns-0.1.0/.github/workflows/pypi_test.yaml
+-rw-r--r--   0        0        0      140 2024-04-20 15:21:18.000000 lxns-0.1.0/.gitignore
+-rw-r--r--   0        0        0      250 2024-04-20 15:21:18.000000 lxns-0.1.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      614 2024-04-20 15:21:18.000000 lxns-0.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2024-04-20 15:21:18.000000 lxns-0.1.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0    16727 2024-04-20 15:21:18.000000 lxns-0.1.0/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0     1556 2024-04-20 15:21:18.000000 lxns-0.1.0/README.md
+-rw-r--r--   0        0        0      333 2024-04-20 15:21:18.000000 lxns-0.1.0/docs/conf.py
+-rw-r--r--   0        0        0      384 2024-04-20 15:21:18.000000 lxns-0.1.0/docs/index.rst
+-rw-r--r--   0        0        0      595 2024-04-20 15:21:18.000000 lxns-0.1.0/docs/mount.rst
+-rw-r--r--   0        0        0     2712 2024-04-20 15:21:18.000000 lxns-0.1.0/docs/namespace.rst
+-rw-r--r--   0        0        0       92 2024-04-20 15:21:18.000000 lxns-0.1.0/docs/requirements.txt
+-rw-r--r--   0        0        0     2191 2024-04-20 15:21:18.000000 lxns-0.1.0/docs/tips_and_tricks.rst
+-rw-r--r--   0        0        0     1900 2024-04-20 15:21:18.000000 lxns-0.1.0/examples/add_bind_mount.py
+-rw-r--r--   0        0        0     1033 2024-04-20 15:21:18.000000 lxns-0.1.0/examples/join_all_pid_namespaces.py
+-rw-r--r--   0        0        0      572 2024-04-20 15:21:18.000000 lxns-0.1.0/examples/process_executor.py
+-rw-r--r--   0        0        0      757 2024-04-20 15:21:18.000000 lxns-0.1.0/examples/process_executor_asyncio.py
+-rw-r--r--   0        0        0      234 2024-04-20 15:21:18.000000 lxns-0.1.0/meson.build
+-rw-r--r--   0        0        0      611 2024-04-20 15:21:18.000000 lxns-0.1.0/meson.options
+-rw-r--r--   0        0        0     1210 2024-04-20 15:21:18.000000 lxns-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      110 2024-04-20 15:21:18.000000 lxns-0.1.0/setup.cfg
+-rw-r--r--   0        0        0      110 2024-04-20 15:21:18.000000 lxns-0.1.0/src/lxns/__init__.py
+-rw-r--r--   0        0        0     1532 2024-04-20 15:21:18.000000 lxns-0.1.0/src/lxns/meson.build
+-rw-r--r--   0        0        0     1958 2024-04-20 15:21:18.000000 lxns-0.1.0/src/lxns/mount.py
+-rw-r--r--   0        0        0     7789 2024-04-20 15:21:18.000000 lxns-0.1.0/src/lxns/namespaces.py
+-rw-r--r--   0        0        0     8753 2024-04-20 15:21:18.000000 lxns-0.1.0/src/lxns/os.c
+-rw-r--r--   0        0        0     1556 2024-04-20 15:21:18.000000 lxns-0.1.0/src/lxns/os.py
+-rw-r--r--   0        0        0       75 2024-04-20 15:21:18.000000 lxns-0.1.0/src/lxns/py.typed
+-rw-r--r--   0        0        0       90 2024-04-20 15:21:18.000000 lxns-0.1.0/src/meson.build
+-rw-r--r--   0        0        0       75 2024-04-20 15:21:18.000000 lxns-0.1.0/test/__init__.py
+-rw-r--r--   0        0        0      493 2024-04-20 15:21:18.000000 lxns-0.1.0/test/check_typing.py
+-rw-r--r--   0        0        0     1101 2024-04-20 15:21:18.000000 lxns-0.1.0/test/test_mount.py
+-rw-r--r--   0        0        0     1921 2024-04-20 15:21:18.000000 lxns-0.1.0/test/test_namespaces.py
+-rw-r--r--   0        0        0     5958 2024-04-20 15:21:18.000000 lxns-0.1.0/test/test_os.py
+-rw-r--r--   0        0        0      715 2024-04-20 15:21:18.000000 lxns-0.1.0/tools/audit_wheel_wrapper.py
+-rw-r--r--   0        0        0     4209 2024-04-20 15:21:18.000000 lxns-0.1.0/tools/build_in_container.py
+-rw-r--r--   0        0        0     2513 2024-04-20 15:21:18.000000 lxns-0.1.0/tools/run_linters.py
+-rw-r--r--   0        0        0     2601 2024-04-20 15:38:00.394309 lxns-0.1.0/PKG-INFO
```

### Comparing `lxns-0.0a3/CHANGELOG.md` & `lxns-0.1.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `lxns-0.0a3/LICENSES/MIT.txt` & `lxns-0.1.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `lxns-0.0a3/LICENSES/MPL-2.0.txt` & `lxns-0.1.0/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `lxns-0.0a3/README.md` & `lxns-0.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 <!--
 SPDX-License-Identifier: MPL-2.0
 SPDX-FileCopyrightText: 2023 igo95862
 -->
 
 [![Documentation Status](https://readthedocs.org/projects/python-lxns/badge/?version=latest)](https://python-lxns.readthedocs.io/en/latest/?badge=latest)
+![PyPI - Version](https://img.shields.io/pypi/v/lxns)
 
 # Python-lxns
 
 ## Python library to control Linux kernel namespaces
 
 Implemented using C extension module.
 
@@ -21,16 +22,26 @@
     * Automatic file descriptor resource control using `with`.
     * Getting and setting the max number of namespaces.
 * Mount utilities using new file descriptor based API.
     * Create bind mounts.
 
 ## [Documentation](https://python-lxns.readthedocs.io/en/latest/)
 
+Also see [`examples/`](examples/) folder for code examples.
+
 ## Requirements
 
+* Python version 3.7 or higher
+
+### [PyPI wheels](https://pypi.org/project/lxns/)
+
+PyPI wheels are completely statically linked and do not depend on any library.
+
+Available architectures: `x86_64`, `i686`, `aarch64`, `armv7l`
+
 ### Compiling source package
 
 * Meson build system
 * Python headers
 * C compiler
 * Linux kernel headers
```

### Comparing `lxns-0.0a3/docs/mount.rst` & `lxns-0.1.0/docs/mount.rst`

 * *Files identical despite different names*

### Comparing `lxns-0.0a3/docs/namespace.rst` & `lxns-0.1.0/docs/namespace.rst`

 * *Files identical despite different names*

### Comparing `lxns-0.0a3/docs/tips_and_tricks.rst` & `lxns-0.1.0/docs/tips_and_tricks.rst`

 * *Files identical despite different names*

### Comparing `lxns-0.0a3/examples/add_bind_mount.py` & `lxns-0.1.0/examples/add_bind_mount.py`

 * *Files identical despite different names*

### Comparing `lxns-0.0a3/examples/join_all_pid_namespaces.py` & `lxns-0.1.0/examples/join_all_pid_namespaces.py`

 * *Files identical despite different names*

### Comparing `lxns-0.0a3/examples/process_executor.py` & `lxns-0.1.0/examples/process_executor.py`

 * *Files identical despite different names*

### Comparing `lxns-0.0a3/examples/process_executor_asyncio.py` & `lxns-0.1.0/examples/process_executor_asyncio.py`

 * *Files identical despite different names*

### Comparing `lxns-0.0a3/meson.options` & `lxns-0.1.0/meson.options`

 * *Files identical despite different names*

### Comparing `lxns-0.0a3/pyproject.toml` & `lxns-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-License-Identifier: MPL-2.0
 # SPDX-FileCopyrightText: 2023 igo95862
 [project]
 name = "lxns"
-version = "0.0.alpha3"
+version = "0.1.0"
 description = "Python library to interact with Linux kernel namespaces."
 readme = "README.md"
 license = {text = "MPL-2.0"}
 authors = [
     {name = "igo95862"}
 ]
 requires-python = ">= 3.7"
```

### Comparing `lxns-0.0a3/src/lxns/meson.build` & `lxns-0.1.0/src/lxns/meson.build`

 * *Files 2% similar despite different names*

```diff
@@ -52,13 +52,14 @@
 )
 
 lxns_python_files = [
     '__init__.py',
     'os.py',
     'namespaces.py',
     'mount.py',
+    'py.typed',
 ]
 
 python.install_sources(
     lxns_python_files,
     subdir : 'lxns',
 )
```

### Comparing `lxns-0.0a3/src/lxns/mount.py` & `lxns-0.1.0/src/lxns/mount.py`

 * *Files identical despite different names*

### Comparing `lxns-0.0a3/src/lxns/namespaces.py` & `lxns-0.1.0/src/lxns/namespaces.py`

 * *Files identical despite different names*

### Comparing `lxns-0.0a3/src/lxns/os.c` & `lxns-0.1.0/src/lxns/os.c`

 * *Files identical despite different names*

### Comparing `lxns-0.0a3/src/lxns/os.py` & `lxns-0.1.0/src/lxns/os.py`

 * *Files identical despite different names*

### Comparing `lxns-0.0a3/test/test_mount.py` & `lxns-0.1.0/test/test_mount.py`

 * *Files identical despite different names*

### Comparing `lxns-0.0a3/test/test_namespaces.py` & `lxns-0.1.0/test/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `lxns-0.0a3/test/test_os.py` & `lxns-0.1.0/test/test_os.py`

 * *Files identical despite different names*

### Comparing `lxns-0.0a3/tools/build_in_container.py` & `lxns-0.1.0/tools/build_in_container.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 CFLAGS: tuple[str, ...] = (
     "-fno-omit-frame-pointer",
     # "-mno-omit-leaf-frame-pointer",
     "-pipe",
 )
 
-ARCH = "x86_64"
+ARCH: list[str] = []
 
 PROJECT_ROOT_PATH = Path(__file__).parent.parent
 BUILD_DIR = Path("/root/lxns")
 
 
 def run_command(*args: str) -> None:
     print(*args)
@@ -57,24 +57,23 @@
         )
     except CalledProcessError:
         print("Failed command: ", args)
         raise SystemError(1)
 
 
 def pull_latest_image() -> None:
-    run_command("podman", "pull", "--arch", ARCH, "docker.io/alpine:latest")
+    run_command("podman", "pull", *ARCH, "docker.io/alpine:latest")
 
 
 def start_container() -> None:
     run_command(
         "podman",
         "run",
         "--detach",
-        "--arch",
-        ARCH,
+        *ARCH,
         "--rm",
         "--name",
         "lxns-build",
         "--init",
         "docker.io/alpine:latest",
         "sleep",
         "1d",
@@ -153,16 +152,16 @@
     ("retag_wheel", retag_wheel),
     ("copy_dist", copy_dist),
 )
 
 
 def main(initial_stage: str, arch: str | None) -> None:
     if arch is not None:
-        global ARCH
-        ARCH = arch
+        ARCH.append("--arch")
+        ARCH.append(arch)
 
     skipping_stages = True
     for stage_name, stage_function in STAGES:
         if initial_stage == stage_name:
             skipping_stages = False
 
         if skipping_stages:
```

### Comparing `lxns-0.0a3/tools/run_linters.py` & `lxns-0.1.0/tools/run_linters.py`

 * *Files identical despite different names*

### Comparing `lxns-0.0a3/PKG-INFO` & `lxns-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lxns
-Version: 0.0a3
+Version: 0.1.0
 Summary: Python library to interact with Linux kernel namespaces.
 Keywords: linux namespace namespaces mount sandbox containers
 Author: igo95862
 License: MPL-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -23,14 +23,15 @@
 
 <!--
 SPDX-License-Identifier: MPL-2.0
 SPDX-FileCopyrightText: 2023 igo95862
 -->
 
 [![Documentation Status](https://readthedocs.org/projects/python-lxns/badge/?version=latest)](https://python-lxns.readthedocs.io/en/latest/?badge=latest)
+![PyPI - Version](https://img.shields.io/pypi/v/lxns)
 
 # Python-lxns
 
 ## Python library to control Linux kernel namespaces
 
 Implemented using C extension module.
 
@@ -44,16 +45,26 @@
     * Automatic file descriptor resource control using `with`.
     * Getting and setting the max number of namespaces.
 * Mount utilities using new file descriptor based API.
     * Create bind mounts.
 
 ## [Documentation](https://python-lxns.readthedocs.io/en/latest/)
 
+Also see [`examples/`](examples/) folder for code examples.
+
 ## Requirements
 
+* Python version 3.7 or higher
+
+### [PyPI wheels](https://pypi.org/project/lxns/)
+
+PyPI wheels are completely statically linked and do not depend on any library.
+
+Available architectures: `x86_64`, `i686`, `aarch64`, `armv7l`
+
 ### Compiling source package
 
 * Meson build system
 * Python headers
 * C compiler
 * Linux kernel headers
```

