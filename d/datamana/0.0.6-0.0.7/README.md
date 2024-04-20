# Comparing `tmp/datamana-0.0.6.tar.gz` & `tmp/datamana-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamana-0.0.6.tar", last modified: Mon Apr 15 12:57:32 2024, max compression
+gzip compressed data, was "datamana-0.0.7.tar", last modified: Sat Apr 20 01:30:25 2024, max compression
```

## Comparing `datamana-0.0.6.tar` & `datamana-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:57:32.838795 datamana-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-15 12:57:19.000000 datamana-0.0.6/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-15 12:57:19.000000 datamana-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-15 12:57:32.838795 datamana-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:57:19.000000 datamana-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:57:32.834795 datamana-0.0.6/csrc/
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-15 12:57:19.000000 datamana-0.0.6/csrc/mqueue.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-15 12:57:19.000000 datamana-0.0.6/csrc/python.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-15 12:57:19.000000 datamana-0.0.6/csrc/semaphore.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:57:32.834795 datamana-0.0.6/datamana/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:57:19.000000 datamana-0.0.6/datamana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:57:19.000000 datamana-0.0.6/datamana/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-15 12:57:19.000000 datamana-0.0.6/datamana/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:57:32.834795 datamana-0.0.6/datamana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-15 12:57:32.000000 datamana-0.0.6/datamana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-15 12:57:32.000000 datamana-0.0.6/datamana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 12:57:32.000000 datamana-0.0.6/datamana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 12:57:32.000000 datamana-0.0.6/datamana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 12:57:32.000000 datamana-0.0.6/datamana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-15 12:57:19.000000 datamana-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 12:57:32.838795 datamana-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-04-15 12:57:19.000000 datamana-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:30:25.805787 datamana-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-20 01:30:17.000000 datamana-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-20 01:30:17.000000 datamana-0.0.7/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-20 01:30:17.000000 datamana-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-20 01:30:17.000000 datamana-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-20 01:30:25.805787 datamana-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:30:17.000000 datamana-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:30:25.805787 datamana-0.0.7/csrc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-20 01:30:17.000000 datamana-0.0.7/csrc/mqueue.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-20 01:30:17.000000 datamana-0.0.7/csrc/python.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-20 01:30:17.000000 datamana-0.0.7/csrc/semaphore.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:30:25.805787 datamana-0.0.7/datamana/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:30:17.000000 datamana-0.0.7/datamana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:30:17.000000 datamana-0.0.7/datamana/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-20 01:30:17.000000 datamana-0.0.7/datamana/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:30:25.805787 datamana-0.0.7/datamana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-20 01:30:25.000000 datamana-0.0.7/datamana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-20 01:30:25.000000 datamana-0.0.7/datamana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 01:30:25.000000 datamana-0.0.7/datamana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-20 01:30:25.000000 datamana-0.0.7/datamana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 01:30:25.000000 datamana-0.0.7/datamana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-20 01:30:17.000000 datamana-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 01:30:25.809787 datamana-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-20 01:30:17.000000 datamana-0.0.7/setup.py
```

### Comparing `datamana-0.0.6/CMakeLists.txt` & `datamana-0.0.7/CMakeLists.txt`

 * *Files 18% similar despite different names*

```diff
@@ -13,11 +13,11 @@
   COMMAND "${Python_EXECUTABLE}" -m nanobind --cmake_dir
   OUTPUT_STRIP_TRAILING_WHITESPACE OUTPUT_VARIABLE NB_DIR)
 list(APPEND CMAKE_PREFIX_PATH "${NB_DIR}")
 find_package(nanobind CONFIG REQUIRED)
 
 nanobind_add_module(
   core STABLE_ABI
-  csrc/semaphore.hpp csrc/mqueue.hpp csrc/fcntl.hpp
+  csrc/semaphore.hpp csrc/mqueue.hpp
   csrc/python.cpp
 )
 target_link_libraries(core PRIVATE rt)
```

### Comparing `datamana-0.0.6/LICENSE` & `datamana-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `datamana-0.0.6/PKG-INFO` & `datamana-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamana
-Version: 0.0.6
+Version: 0.0.7
 Summary: Dataset Manager
 Author-email: Jiau Zhang <jiauzhang@163.com>
 Project-URL: Homepage, https://github.com/jiauzhang/datamana
 Keywords: Deep Learning,Dataset Manager,Artificial Intelligence
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datamana-0.0.6/csrc/mqueue.hpp` & `datamana-0.0.7/csrc/mqueue.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 namespace nb = nanobind;
 
 struct MQueue {
     mqd_t mqd;
 
     MQueue() : mqd((mqd_t)-1) {}
 
-    int py_mq_open(const char *name, int oflag, unsigned int mode, struct mq_attr *attr) {
-        mqd = mq_open(name, oflag, (mode_t)mode, attr);
+    int py_mq_open(const char *name, int oflag, unsigned int mode) {
+        mqd = mq_open(name, oflag, (mode_t)mode, nullptr);
         if (mqd == (mqd_t)-1) {
-            return -1;
+            return errno;
         } else {
             return 0;
         }
     }
     int py_mq_unlink(const char *name) {
         return mq_unlink(name);
     }
```

### Comparing `datamana-0.0.6/csrc/semaphore.hpp` & `datamana-0.0.7/csrc/semaphore.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     Semaphore() : sem((sem_t *)0) {}
 
     int py_sem_open(const char *name, int oflag, unsigned int mode, unsigned int value) {
         sem = sem_open(name, oflag, (mode_t)mode, value);
         if (sem == (sem_t *)SEM_FAILED) {
             sem = 0;
-            return -1;
+            return errno;
         } else {
             return 0;
         }
     }
     int py_sem_unlink(const char *name) {
         return sem_unlink(name);
     }
```

### Comparing `datamana-0.0.6/datamana/torch.py` & `datamana-0.0.7/datamana/torch.py`

 * *Files identical despite different names*

### Comparing `datamana-0.0.6/datamana.egg-info/PKG-INFO` & `datamana-0.0.7/datamana.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamana
-Version: 0.0.6
+Version: 0.0.7
 Summary: Dataset Manager
 Author-email: Jiau Zhang <jiauzhang@163.com>
 Project-URL: Homepage, https://github.com/jiauzhang/datamana
 Keywords: Deep Learning,Dataset Manager,Artificial Intelligence
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datamana-0.0.6/pyproject.toml` & `datamana-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = [
-    "build >= 1.2",
-    "setuptools >= 67",
+    "build",
+    "setuptools >= 42",
     "wheel",
     "ninja",
     "cmake >= 3.15",
     "nanobind >= 1.9.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datamana"
-version = "0.0.6"
+version = "0.0.7"
 description = "Dataset Manager"
 readme = "README.md"
 authors = [
     {name = "Jiau Zhang", email = "jiauzhang@163.com"},
 ]
 classifiers = [
     'Intended Audience :: Developers',
```

### Comparing `datamana-0.0.6/setup.py` & `datamana-0.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     "win-arm64": "ARM64",
 }
 
 # A CMakeExtension needs a sourcedir instead of a file list.
 # The name must be the _single_ output extension from the CMake build.
 # If you need multiple extensions, see scikit-build.
 class CMakeExtension(Extension):
-    def __init__(self, name: str, sourcedir: str, sources) -> None:
+    def __init__(self, name: str, sourcedir: str = "") -> None:
+        super().__init__(name, sources=[])
         self.sourcedir = os.fspath(Path(sourcedir).resolve())
-        super().__init__(name, sources=sources)
 
 
 class CMakeBuild(build_ext):
     def build_extension(self, ext: CMakeExtension) -> None:
         # Must be in this form due to bug in .resolve() only fixed in Python 3.10+
         ext_fullpath = Path.cwd() / self.get_ext_fullpath(ext.name)
         extdir = ext_fullpath.parent.resolve()
@@ -114,13 +114,10 @@
             ["cmake", ext.sourcedir, *cmake_args], cwd=build_temp, check=True
         )
         subprocess.run(
             ["cmake", "--build", ".", *build_args], cwd=build_temp, check=True
         )
 
 setup(
-    ext_modules=[CMakeExtension("datamana.core", sourcedir=".", sources=[
-        'CMakeLists.txt',
-        'csrc/semaphore.hpp', 'csrc/mqueue.hpp', 'csrc/python.cpp', ' csrc/fcntl.hpp',
-    ])],
+    ext_modules=[CMakeExtension("datamana.core", sourcedir=".")],
     cmdclass={"build_ext": CMakeBuild},
 )
```

