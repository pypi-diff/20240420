# Comparing `tmp/movoid_package-1.2.0.tar.gz` & `tmp/movoid_package-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_package-1.2.0.tar", last modified: Sun Mar 24 16:33:04 2024, max compression
+gzip compressed data, was "movoid_package-1.2.1.tar", last modified: Sat Apr 20 15:52:45 2024, max compression
```

## Comparing `movoid_package-1.2.0.tar` & `movoid_package-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-24 16:33:04.029638 movoid_package-1.2.0/
--rw-rw-rw-   0        0        0      212 2024-03-24 16:33:04.028636 movoid_package-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_package-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-24 16:33:04.015858 movoid_package-1.2.0/movoid_package/
--rw-rw-rw-   0        0        0      253 2024-03-04 17:02:37.000000 movoid_package-1.2.0/movoid_package/__init__.py
--rw-rw-rw-   0        0        0     2902 2024-03-04 15:17:35.000000 movoid_package-1.2.0/movoid_package/for_import.py
--rw-rw-rw-   0        0        0    13456 2024-03-24 16:32:46.000000 movoid_package-1.2.0/movoid_package/stub.py
-drwxrwxrwx   0        0        0        0 2024-03-24 16:33:04.027614 movoid_package-1.2.0/movoid_package.egg-info/
--rw-rw-rw-   0        0        0      212 2024-03-24 16:33:03.000000 movoid_package-1.2.0/movoid_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2024-03-24 16:33:04.000000 movoid_package-1.2.0/movoid_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-24 16:33:03.000000 movoid_package-1.2.0/movoid_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-03-24 16:33:03.000000 movoid_package-1.2.0/movoid_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-24 16:33:04.030640 movoid_package-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      461 2024-03-24 16:31:35.000000 movoid_package-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-24 16:33:04.026600 movoid_package-1.2.0/test/
--rw-rw-rw-   0        0        0     1617 2024-03-03 15:42:19.000000 movoid_package-1.2.0/test/__init__.py
--rw-rw-rw-   0        0        0      732 2024-03-04 16:41:42.000000 movoid_package-1.2.0/test/test1.py
--rw-rw-rw-   0        0        0      573 2024-03-04 16:52:19.000000 movoid_package-1.2.0/test/test1.pyi
--rw-rw-rw-   0        0        0      245 2024-03-04 16:29:14.000000 movoid_package-1.2.0/test/test2.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:52:45.345510 movoid_package-1.2.1/
+-rw-rw-rw-   0        0        0      212 2024-04-20 15:52:45.344513 movoid_package-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_package-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 15:52:45.328946 movoid_package-1.2.1/movoid_package/
+-rw-rw-rw-   0        0        0      253 2024-03-04 17:02:37.000000 movoid_package-1.2.1/movoid_package/__init__.py
+-rw-rw-rw-   0        0        0     2902 2024-03-04 15:17:35.000000 movoid_package-1.2.1/movoid_package/for_import.py
+-rw-rw-rw-   0        0        0    13774 2024-04-20 15:50:56.000000 movoid_package-1.2.1/movoid_package/stub.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:52:45.343516 movoid_package-1.2.1/movoid_package.egg-info/
+-rw-rw-rw-   0        0        0      212 2024-04-20 15:52:45.000000 movoid_package-1.2.1/movoid_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-04-20 15:52:45.000000 movoid_package-1.2.1/movoid_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 15:52:45.000000 movoid_package-1.2.1/movoid_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-20 15:52:45.000000 movoid_package-1.2.1/movoid_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 15:52:45.345510 movoid_package-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      461 2024-04-20 15:51:43.000000 movoid_package-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 15:52:45.342520 movoid_package-1.2.1/test/
+-rw-rw-rw-   0        0        0     1617 2024-03-03 15:42:19.000000 movoid_package-1.2.1/test/__init__.py
+-rw-rw-rw-   0        0        0      732 2024-03-04 16:41:42.000000 movoid_package-1.2.1/test/test1.py
+-rw-rw-rw-   0        0        0      573 2024-03-04 16:52:19.000000 movoid_package-1.2.1/test/test1.pyi
+-rw-rw-rw-   0        0        0      245 2024-03-04 16:29:14.000000 movoid_package-1.2.1/test/test2.py
+-rw-rw-rw-   0        0        0      396 2024-04-20 15:19:33.000000 movoid_package-1.2.1/test/test3.py
```

### Comparing `movoid_package-1.2.0/movoid_package/for_import.py` & `movoid_package-1.2.1/movoid_package/for_import.py`

 * *Files identical despite different names*

### Comparing `movoid_package-1.2.0/movoid_package/stub.py` & `movoid_package-1.2.1/movoid_package/stub.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,18 +113,23 @@
                 return element.__name__
             else:
                 module_name = module.__name__
                 if module_name not in self._imports:
                     self._imports.setdefault(module_name, module)
                 return '{0}.{1}'.format(module_name, element.__name__)
         elif inspect.getmodule(element) == inspect.getmodule(typing):
-            module_name = str(element).split('.')[0]
+            element_str = str(element)
+            module_name = element_str.split('.')[0]
             if module_name not in self._imports:
                 self._imports.setdefault(module_name, typing)
-            return str(element).replace('NoneType', 'None')
+            element_re = re.search(r'(.*?)\[(.*)\]', element_str)
+            if element_re is not None:
+                arg_list = [self._get_element_name_with_module(_) for _ in element.__args__]
+                element_str = f'{element_re.group(1)}[{", ".join(arg_list)}]'
+            return element_str.replace('NoneType', 'None')
 
     def _generate_class_stub(self, class_name: str, tar_class: type) -> str:
         parent_class = [self._get_element_name_with_module(_) for _ in tar_class.__bases__]
         if tar_class.__class__ != type:
             parent_class.append('metaclass=' + self._get_element_name_with_module(tar_class.__class__))
         pure_class_name = class_name.split('.')[-1]
         retext = 'class ' + pure_class_name + '(' + ', '.join(parent_class) + '):\n'
```

### Comparing `movoid_package-1.2.0/test/__init__.py` & `movoid_package-1.2.1/test/__init__.py`

 * *Files identical despite different names*

### Comparing `movoid_package-1.2.0/test/test1.py` & `movoid_package-1.2.1/test/test1.py`

 * *Files identical despite different names*

### Comparing `movoid_package-1.2.0/test/test1.pyi` & `movoid_package-1.2.1/test/test1.pyi`

 * *Files identical despite different names*

