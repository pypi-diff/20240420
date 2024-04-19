# Comparing `tmp/di_registry-0.5.0.tar.gz` & `tmp/di_registry-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/di_registry-0.5.0.tar", last modified: Tue Nov  7 00:04:49 2023, max compression
+gzip compressed data, was "dist/di_registry-0.5.1.tar", last modified: Fri Apr 19 22:22:11 2024, max compression
```

## Comparing `di_registry-0.5.0.tar` & `di_registry-0.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-07 00:04:49.000000 di_registry-0.5.0/
--rw-r--r--   0 root         (0) root         (0)      504 2023-11-07 00:04:49.000000 di_registry-0.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-11-07 00:04:44.000000 di_registry-0.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-07 00:04:49.000000 di_registry-0.5.0/di_registry/
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-11-07 00:04:44.000000 di_registry-0.5.0/di_registry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-11-07 00:04:44.000000 di_registry-0.5.0/di_registry/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    18465 2023-11-07 00:04:44.000000 di_registry-0.5.0/di_registry/abc.py
--rw-rw-rw-   0 root         (0) root         (0)    15970 2023-11-07 00:04:44.000000 di_registry-0.5.0/di_registry/registry.py
--rw-rw-rw-   0 root         (0) root         (0)      929 2023-11-07 00:04:44.000000 di_registry-0.5.0/di_registry/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-07 00:04:49.000000 di_registry-0.5.0/di_registry.egg-info/
--rw-r--r--   0 root         (0) root         (0)      504 2023-11-07 00:04:49.000000 di_registry-0.5.0/di_registry.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      306 2023-11-07 00:04:49.000000 di_registry-0.5.0/di_registry.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-07 00:04:49.000000 di_registry-0.5.0/di_registry.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-11-07 00:04:49.000000 di_registry-0.5.0/di_registry.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-11-07 00:04:49.000000 di_registry-0.5.0/di_registry.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-07 00:04:49.000000 di_registry-0.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1869 2023-11-07 00:04:44.000000 di_registry-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 22:22:11.000000 di_registry-0.5.1/
+-rw-r--r--   0 root         (0) root         (0)      504 2024-04-19 22:22:11.000000 di_registry-0.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-04-19 22:22:06.000000 di_registry-0.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 22:22:11.000000 di_registry-0.5.1/di_registry/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-19 22:22:06.000000 di_registry-0.5.1/di_registry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-19 22:22:06.000000 di_registry-0.5.1/di_registry/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18671 2024-04-19 22:22:06.000000 di_registry-0.5.1/di_registry/abc.py
+-rw-rw-rw-   0 root         (0) root         (0)    15970 2024-04-19 22:22:06.000000 di_registry-0.5.1/di_registry/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)      929 2024-04-19 22:22:06.000000 di_registry-0.5.1/di_registry/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 22:22:11.000000 di_registry-0.5.1/di_registry.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      504 2024-04-19 22:22:11.000000 di_registry-0.5.1/di_registry.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      306 2024-04-19 22:22:11.000000 di_registry-0.5.1/di_registry.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 22:22:11.000000 di_registry-0.5.1/di_registry.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-19 22:22:11.000000 di_registry-0.5.1/di_registry.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-19 22:22:11.000000 di_registry-0.5.1/di_registry.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-19 22:22:11.000000 di_registry-0.5.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1869 2024-04-19 22:22:06.000000 di_registry-0.5.1/setup.py
```

### Comparing `di_registry-0.5.0/di_registry/abc.py` & `di_registry-0.5.1/di_registry/abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,17 +237,20 @@
 
         :param kwargs: value updates
         """
         for name, params in self.yaml_parameters.items():
             # if value is defined and instance has this attribute, update the instance value
             if (params.kwarg_alias or name) in kwargs and hasattr(self, name):
                 val = kwargs[params.kwarg_alias or name]
+                # dont try to typecast None because an error will be thrown
                 if val is not None and params.typecast is not None:
-                    # dont try to typecast None because an error will be thrown
-                    val = params.typecast(val)
+                    try:
+                        val = params.typecast(val)
+                    except TypeError as e:
+                        raise TypeError(f'unable to cast {params.kwarg_alias or name} value {val} using typecast {params.typecast}: {e}')
                 setattr(self, name, val)
         # pass through kwargs to sub-instances
         for sub_config in self.sub_configurations:
             instance: YAMLConfig = getattr(self, sub_config, None)
             if instance is None:
                 continue
             instance.apply_parameters(**kwargs)
```

### Comparing `di_registry-0.5.0/di_registry/registry.py` & `di_registry-0.5.1/di_registry/registry.py`

 * *Files identical despite different names*

### Comparing `di_registry-0.5.0/di_registry/test.py` & `di_registry-0.5.1/di_registry/test.py`

 * *Files identical despite different names*

### Comparing `di_registry-0.5.0/setup.py` & `di_registry-0.5.1/setup.py`

 * *Files identical despite different names*

