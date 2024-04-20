# Comparing `tmp/pyaogmaneo-2.5.1.tar.gz` & `tmp/pyaogmaneo-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaogmaneo-2.5.1.tar", last modified: Mon Apr 15 00:01:39 2024, max compression
+gzip compressed data, was "pyaogmaneo-2.5.2.tar", last modified: Fri Apr 19 23:21:39 2024, max compression
```

## Comparing `pyaogmaneo-2.5.1.tar` & `pyaogmaneo-2.5.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:01:39.066031 pyaogmaneo-2.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:01:39.066031 pyaogmaneo-2.5.1/CMake/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/CMake/FindAOgmaNeo.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-15 00:01:39.066031 pyaogmaneo-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:01:39.066031 pyaogmaneo-2.5.1/pyaogmaneo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-15 00:01:39.000000 pyaogmaneo-2.5.1/pyaogmaneo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-15 00:01:39.000000 pyaogmaneo-2.5.1/pyaogmaneo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 00:01:39.000000 pyaogmaneo-2.5.1/pyaogmaneo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 00:01:38.000000 pyaogmaneo-2.5.1/pyaogmaneo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 00:01:39.000000 pyaogmaneo-2.5.1/pyaogmaneo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 00:01:39.066031 pyaogmaneo-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:01:39.062031 pyaogmaneo-2.5.1/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:01:39.066031 pyaogmaneo-2.5.1/source/pyaogmaneo/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/source/pyaogmaneo/py_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/source/pyaogmaneo/py_helpers.h
--rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/source/pyaogmaneo/py_hierarchy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/source/pyaogmaneo/py_hierarchy.h
--rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/source/pyaogmaneo/py_image_encoder.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/source/pyaogmaneo/py_image_encoder.h
--rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/source/pyaogmaneo/py_module.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:21:39.365796 pyaogmaneo-2.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:21:39.361796 pyaogmaneo-2.5.2/CMake/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-19 23:21:31.000000 pyaogmaneo-2.5.2/CMake/FindAOgmaNeo.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-19 23:21:31.000000 pyaogmaneo-2.5.2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-04-19 23:21:31.000000 pyaogmaneo-2.5.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-19 23:21:31.000000 pyaogmaneo-2.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-19 23:21:39.365796 pyaogmaneo-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-19 23:21:31.000000 pyaogmaneo-2.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:21:39.361796 pyaogmaneo-2.5.2/pyaogmaneo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-19 23:21:39.000000 pyaogmaneo-2.5.2/pyaogmaneo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-19 23:21:39.000000 pyaogmaneo-2.5.2/pyaogmaneo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 23:21:39.000000 pyaogmaneo-2.5.2/pyaogmaneo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 23:21:39.000000 pyaogmaneo-2.5.2/pyaogmaneo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 23:21:39.000000 pyaogmaneo-2.5.2/pyaogmaneo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-19 23:21:31.000000 pyaogmaneo-2.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 23:21:39.365796 pyaogmaneo-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-19 23:21:31.000000 pyaogmaneo-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:21:39.361796 pyaogmaneo-2.5.2/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:21:39.361796 pyaogmaneo-2.5.2/source/pyaogmaneo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-19 23:21:31.000000 pyaogmaneo-2.5.2/source/pyaogmaneo/py_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-19 23:21:31.000000 pyaogmaneo-2.5.2/source/pyaogmaneo/py_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12736 2024-04-19 23:21:31.000000 pyaogmaneo-2.5.2/source/pyaogmaneo/py_hierarchy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-04-19 23:21:31.000000 pyaogmaneo-2.5.2/source/pyaogmaneo/py_hierarchy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-04-19 23:21:31.000000 pyaogmaneo-2.5.2/source/pyaogmaneo/py_image_encoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-19 23:21:31.000000 pyaogmaneo-2.5.2/source/pyaogmaneo/py_image_encoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-04-19 23:21:31.000000 pyaogmaneo-2.5.2/source/pyaogmaneo/py_module.cpp
```

### Comparing `pyaogmaneo-2.5.1/CMake/FindAOgmaNeo.cmake` & `pyaogmaneo-2.5.2/CMake/FindAOgmaNeo.cmake`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.5.1/CMakeLists.txt` & `pyaogmaneo-2.5.2/CMakeLists.txt`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     find_package(AOgmaNeo)
 else()
     message(STATUS "Not using system installation of AOgmaNeo, will download from repository")
 
     FetchContent_Declare(
         AOgmaNeo
         GIT_REPOSITORY https://github.com/ogmacorp/AOgmaNeo.git
-        GIT_TAG efd239a88ff5e75acb4b4b0d4509526bdde50cae
+        GIT_TAG b9337629ae38f14a8d2b16fe0538acd0d008cd08
     )
 
     FetchContent_MakeAvailable(AOgmaNeo)
 endif()
 
 FetchContent_Declare(
     pybind11
```

### Comparing `pyaogmaneo-2.5.1/LICENSE.md` & `pyaogmaneo-2.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.5.1/PKG-INFO` & `pyaogmaneo-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.5.1
+Version: 2.5.2
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.5.1/README.md` & `pyaogmaneo-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.5.1/pyaogmaneo.egg-info/PKG-INFO` & `pyaogmaneo-2.5.2/pyaogmaneo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.5.1
+Version: 2.5.2
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.5.1/setup.py` & `pyaogmaneo-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             os.makedirs(self.build_temp)
 
         subprocess.check_call([ 'cmake', ext.sourcedir ] + cmake_args, cwd=self.build_temp, env=env)
         subprocess.check_call([ 'cmake', '--build', '.' ] + build_args, cwd=self.build_temp)
 
 setup(
     name="pyaogmaneo",
-    version="2.5.1",
+    version="2.5.2",
     description="Python bindings for the AOgmaNeo library",
     long_description='https://github.com/ogmacorp/PyAOgmaNeo',
     author='Ogma Intelligent Systems Corp',
     author_email='info@ogmacorp.com',
     url='https://ogmacorp.com/',
     license='Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License',
     classifiers=[
```

### Comparing `pyaogmaneo-2.5.1/source/pyaogmaneo/py_helpers.cpp` & `pyaogmaneo-2.5.2/source/pyaogmaneo/py_helpers.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.5.1/source/pyaogmaneo/py_helpers.h` & `pyaogmaneo-2.5.2/source/pyaogmaneo/py_helpers.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.5.1/source/pyaogmaneo/py_hierarchy.cpp` & `pyaogmaneo-2.5.2/source/pyaogmaneo/py_hierarchy.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,14 @@
         throw std::runtime_error("error: value_num_dendrites_per_cell < 2 is not allowed!");
 
     if (up_radius < 0)
         throw std::runtime_error("error: up_radius < 0 is not allowed!");
 
     if (down_radius < 0)
         throw std::runtime_error("error: down_radius < 0 is not allowed!");
-
-    if (history_capacity < 2)
-        throw std::runtime_error("error: history_capacity < 2 is not allowed!");
 }
 
 void Layer_Desc::check_in_range() const {
     if (std::get<0>(hidden_size) < 1)
         throw std::runtime_error("error: hidden_size[0] < 1 is not allowed!");
 
     if (std::get<1>(hidden_size) < 1)
@@ -114,16 +111,15 @@
 
         c_io_descs[i] = aon::Hierarchy::IO_Desc(
             aon::Int3(std::get<0>(io_descs[i].size), std::get<1>(io_descs[i].size), std::get<2>(io_descs[i].size)),
             static_cast<aon::IO_Type>(io_descs[i].type),
             io_descs[i].num_dendrites_per_cell,
             io_descs[i].value_num_dendrites_per_cell,
             io_descs[i].up_radius,
-            io_descs[i].down_radius,
-            io_descs[i].history_capacity
+            io_descs[i].down_radius
         );
     }
     
     aon::Array<aon::Hierarchy::Layer_Desc> c_layer_descs(layer_descs.size());
 
     for (int l = 0; l < layer_descs.size(); l++) {
         layer_descs[l].check_in_range();
```

### Comparing `pyaogmaneo-2.5.1/source/pyaogmaneo/py_hierarchy.h` & `pyaogmaneo-2.5.2/source/pyaogmaneo/py_hierarchy.h`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 #include "py_helpers.h"
 #include <aogmaneo/hierarchy.h>
 
 namespace py = pybind11;
 
 namespace pyaon {
-const int hierarchy_magic = 7229311;
+const int hierarchy_magic = 8221313;
 
 enum IO_Type {
     none = 0,
     prediction = 1,
     action = 2
 };
 
@@ -28,33 +28,29 @@
 
     int num_dendrites_per_cell;
     int value_num_dendrites_per_cell;
 
     int up_radius;
     int down_radius;
 
-    int history_capacity;
-
     IO_Desc(
         const std::tuple<int, int, int> &size,
         IO_Type type,
         int num_dendrites_per_cell,
         int value_num_dendrites_per_cell,
         int up_radius,
-        int down_radius,
-        int history_capacity
+        int down_radius
     )
     :
     size(size),
     type(type),
     num_dendrites_per_cell(num_dendrites_per_cell),
     value_num_dendrites_per_cell(value_num_dendrites_per_cell),
     up_radius(up_radius),
-    down_radius(down_radius),
-    history_capacity(history_capacity)
+    down_radius(down_radius)
     {}
 
     void check_in_range() const;
 };
 
 struct Layer_Desc {
     std::tuple<int, int, int> hidden_size;
@@ -88,19 +84,14 @@
 };
 
 struct Params {
     std::vector<aon::Hierarchy::Layer_Params> layers;
     std::vector<aon::Hierarchy::IO_Params> ios;
 
     bool anticipation;
-
-    Params()
-    :
-    anticipation(true)
-    {}
 };
 
 class Hierarchy {
 private:
     aon::Hierarchy h;
 
     aon::Array<aon::Int_Buffer> c_input_cis_backing;
@@ -281,22 +272,13 @@
 
         if (h.get_io_type(i) == aon::action)
             return h.get_actor(i).get_visible_layer_desc(0).radius;
         
         return h.get_decoder(l, i).get_visible_layer_desc(0).radius;
     }
 
-    int get_actor_history_capacity(
-        int i
-    ) const {
-        if (i < 0 || i >= h.get_num_io() || h.get_io_type(i) != aon::action)
-            throw std::runtime_error("error: " + std::to_string(i) + " is not a valid input index!");
-
-        return h.get_actor(i).get_history_capacity();
-    }
-
     void merge(
         const std::vector<Hierarchy*> &hierarchies,
         Merge_Mode mode
     );
 };
 }
```

### Comparing `pyaogmaneo-2.5.1/source/pyaogmaneo/py_image_encoder.cpp` & `pyaogmaneo-2.5.2/source/pyaogmaneo/py_image_encoder.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.5.1/source/pyaogmaneo/py_image_encoder.h` & `pyaogmaneo-2.5.2/source/pyaogmaneo/py_image_encoder.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.5.1/source/pyaogmaneo/py_module.cpp` & `pyaogmaneo-2.5.2/source/pyaogmaneo/py_module.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -32,32 +32,29 @@
     py::class_<pyaon::IO_Desc>(m, "IODesc")
         .def(py::init<
                 std::tuple<int, int, int>,
                 pyaon::IO_Type,
                 int,
                 int,
                 int,
-                int,
                 int
             >(),
             py::arg("size") = std::tuple<int, int, int>({ 4, 4, 16 }),
             py::arg("io_type") = pyaon::prediction,
             py::arg("num_dendrites_per_cell") = 4,
             py::arg("value_num_dendrites_per_cell") = 8,
             py::arg("up_radius") = 2,
-            py::arg("down_radius") = 2,
-            py::arg("history_capacity") = 256
+            py::arg("down_radius") = 2
         )
         .def_readwrite("size", &pyaon::IO_Desc::size)
         .def_readwrite("io_type", &pyaon::IO_Desc::type)
         .def_readwrite("num_dendrites_per_cell", &pyaon::IO_Desc::num_dendrites_per_cell)
         .def_readwrite("value_num_dendrites_per_cell", &pyaon::IO_Desc::value_num_dendrites_per_cell)
         .def_readwrite("up_radius", &pyaon::IO_Desc::up_radius)
         .def_readwrite("down_radius", &pyaon::IO_Desc::down_radius)
-        .def_readwrite("history_capacity", &pyaon::IO_Desc::history_capacity)
         .def("__copy__", 
             [](const pyaon::IO_Desc &other) {
                 return other;
             }
         )
         .def("__deepcopy__", 
             [](const pyaon::IO_Desc &other) {
@@ -112,20 +109,18 @@
         .def_readwrite("leak", &aon::Decoder::Params::leak);
 
     py::class_<aon::Actor::Params>(m, "ActorParams")
         .def(py::init<>())
         .def_readwrite("vlr", &aon::Actor::Params::vlr)
         .def_readwrite("plr", &aon::Actor::Params::plr)
         .def_readwrite("leak", &aon::Actor::Params::leak)
-        .def_readwrite("policy_rate", &aon::Actor::Params::policy_rate)
-        .def_readwrite("value_rate", &aon::Actor::Params::value_rate)
-        .def_readwrite("clip_coef", &aon::Actor::Params::clip_coef)
         .def_readwrite("discount", &aon::Actor::Params::discount)
-        .def_readwrite("min_steps", &aon::Actor::Params::min_steps)
-        .def_readwrite("history_iters", &aon::Actor::Params::history_iters);
+        .def_readwrite("policy_clip", &aon::Actor::Params::policy_clip)
+        .def_readwrite("value_clip", &aon::Actor::Params::value_clip)
+        .def_readwrite("trace_decay", &aon::Actor::Params::trace_decay);
 
     py::class_<aon::Hierarchy::Layer_Params>(m, "LayerParams")
         .def(py::init<>())
         .def_readwrite("encoder", &aon::Hierarchy::Layer_Params::encoder)
         .def_readwrite("decoder", &aon::Hierarchy::Layer_Params::decoder);
 
     py::class_<aon::Hierarchy::IO_Params>(m, "IOParams")
@@ -180,15 +175,14 @@
         .def("get_ticks", &pyaon::Hierarchy::get_ticks)
         .def("get_ticks_per_update", &pyaon::Hierarchy::get_ticks_per_update)
         .def("get_num_io", &pyaon::Hierarchy::get_num_io)
         .def("get_io_size", &pyaon::Hierarchy::get_io_size)
         .def("get_io_type", &pyaon::Hierarchy::get_io_type)
         .def("get_up_radius", &pyaon::Hierarchy::get_up_radius)
         .def("get_down_radius", &pyaon::Hierarchy::get_down_radius)
-        .def("get_actor_history_capacity", &pyaon::Hierarchy::get_actor_history_capacity)
         .def("merge", &pyaon::Hierarchy::merge)
         .def("__copy__", 
             [](const pyaon::Hierarchy &other) {
                 return other;
             }
         )
         .def("__deepcopy__",
```

