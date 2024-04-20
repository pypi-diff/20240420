# Comparing `tmp/qdataclass-1.0.0.tar.gz` & `tmp/qdataclass-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdataclass-1.0.0.tar", last modified: Mon Oct 16 14:00:51 2023, max compression
+gzip compressed data, was "qdataclass-1.0.2.tar", last modified: Sat Apr 20 09:07:05 2024, max compression
```

## Comparing `qdataclass-1.0.0.tar` & `qdataclass-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-10-16 14:00:51.930225 qdataclass-1.0.0/
--rw-rw-rw-   0        0        0     1070 2023-10-16 13:48:08.000000 qdataclass-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      257 2023-10-16 14:00:51.929223 qdataclass-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-10-16 13:48:08.000000 qdataclass-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-10-16 14:00:51.919420 qdataclass-1.0.0/qdataclass/
--rw-rw-rw-   0        0        0      290 2023-10-16 13:59:02.000000 qdataclass-1.0.0/qdataclass/__init__.py
--rw-rw-rw-   0        0        0     1345 2023-10-16 13:48:15.000000 qdataclass-1.0.0/qdataclass/qdataclass.py
-drwxrwxrwx   0        0        0        0 2023-10-16 14:00:51.928223 qdataclass-1.0.0/qdataclass.egg-info/
--rw-rw-rw-   0        0        0      257 2023-10-16 14:00:51.000000 qdataclass-1.0.0/qdataclass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-10-16 14:00:51.000000 qdataclass-1.0.0/qdataclass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-16 14:00:51.000000 qdataclass-1.0.0/qdataclass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-10-16 14:00:51.000000 qdataclass-1.0.0/qdataclass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-16 14:00:51.930225 qdataclass-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      308 2023-10-16 14:00:42.000000 qdataclass-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 09:07:05.461144 qdataclass-1.0.2/
+-rw-rw-rw-   0        0        0     1070 2023-10-16 13:48:08.000000 qdataclass-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-20 09:07:05.460140 qdataclass-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      115 2023-10-16 14:09:31.000000 qdataclass-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 09:07:05.430112 qdataclass-1.0.2/qdataclass/
+-rw-rw-rw-   0        0        0      290 2024-04-14 13:41:16.000000 qdataclass-1.0.2/qdataclass/__init__.py
+-rw-rw-rw-   0        0        0     1404 2024-04-20 08:46:41.000000 qdataclass-1.0.2/qdataclass/qdataclass.py
+drwxrwxrwx   0        0        0        0 2024-04-20 09:07:05.457137 qdataclass-1.0.2/qdataclass.egg-info/
+-rw-rw-rw-   0        0        0      257 2024-04-20 09:07:05.000000 qdataclass-1.0.2/qdataclass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-04-20 09:07:05.000000 qdataclass-1.0.2/qdataclass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 09:07:05.000000 qdataclass-1.0.2/qdataclass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-20 09:07:05.000000 qdataclass-1.0.2/qdataclass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 09:07:05.461144 qdataclass-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      308 2024-04-20 09:06:57.000000 qdataclass-1.0.2/setup.py
```

### Comparing `qdataclass-1.0.0/LICENSE` & `qdataclass-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qdataclass-1.0.0/qdataclass/qdataclass.py` & `qdataclass-1.0.2/qdataclass/qdataclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 def _process_cls(cls: type):
     if "staticMetaObject" not in cls.__dict__:
         raise Exception("Class must be a QObject")
     ann = cls.__annotations__
     for prop_name, prop_type in ann.items():
+        if hasattr(cls, prop_name):
+            continue
         if prop_type in {Property, Signal}:
             continue
         getter, setter = _getter_setter(prop_name)
         signal = Signal(prop_type)
         setattr(cls, prop_name+"Changed", signal)
         setattr(cls, prop_name, Property(
             prop_type, getter, setter, notify=signal))
```

