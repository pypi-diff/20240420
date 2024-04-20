# Comparing `tmp/func_bk-1.0.1.tar.gz` & `tmp/func_bk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_bk-1.0.1.tar", last modified: Sun Apr 14 13:47:26 2024, max compression
+gzip compressed data, was "func_bk-1.0.2.tar", last modified: Sat Apr 20 12:52:51 2024, max compression
```

## Comparing `func_bk-1.0.1.tar` & `func_bk-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 13:47:26.474747 func_bk-1.0.1/
--rw-rw-rw-   0        0        0     1783 2024-04-14 13:47:26.474747 func_bk-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1566 2024-04-14 13:45:24.000000 func_bk-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 13:47:26.468747 func_bk-1.0.1/func_bk/
--rw-rw-rw-   0        0        0     2874 2024-04-13 17:49:52.000000 func_bk-1.0.1/func_bk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 13:47:26.473747 func_bk-1.0.1/func_bk.egg-info/
--rw-rw-rw-   0        0        0     1783 2024-04-14 13:47:26.000000 func_bk-1.0.1/func_bk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-14 13:47:26.000000 func_bk-1.0.1/func_bk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 13:47:26.000000 func_bk-1.0.1/func_bk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-14 13:47:26.000000 func_bk-1.0.1/func_bk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2024-04-14 13:47:26.000000 func_bk-1.0.1/func_bk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       44 2024-04-14 13:47:26.475749 func_bk-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      492 2024-04-14 13:46:14.000000 func_bk-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 12:52:51.640498 func_bk-1.0.2/
+-rw-rw-rw-   0        0        0     1783 2024-04-20 12:52:51.639499 func_bk-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1566 2024-04-20 12:50:24.000000 func_bk-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 12:52:51.634498 func_bk-1.0.2/func_bk/
+-rw-rw-rw-   0        0        0     2876 2024-04-20 12:50:17.000000 func_bk-1.0.2/func_bk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 12:52:51.639499 func_bk-1.0.2/func_bk.egg-info/
+-rw-rw-rw-   0        0        0     1783 2024-04-20 12:52:51.000000 func_bk-1.0.2/func_bk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-20 12:52:51.000000 func_bk-1.0.2/func_bk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 12:52:51.000000 func_bk-1.0.2/func_bk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-14 13:47:26.000000 func_bk-1.0.2/func_bk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2024-04-20 12:52:51.000000 func_bk-1.0.2/func_bk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       44 2024-04-20 12:52:51.640498 func_bk-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      492 2024-04-14 13:46:14.000000 func_bk-1.0.2/setup.py
```

### Comparing `func_bk-1.0.1/PKG-INFO` & `func_bk-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func_bk
-Version: 1.0.1
+Version: 1.0.2
 Summary: add function for normal python and add class(for inheritance) for django
 Author-email: lilo.pio147@mail.ru
 Description-Content-Type: text/markdown
 
 add function 
 
 sejango - 3 arguments form(django),key(in form cleaned data),var(return if key is not find)
```

### Comparing `func_bk-1.0.1/README.md` & `func_bk-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `func_bk-1.0.1/func_bk/__init__.py` & `func_bk-1.0.2/func_bk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 		return var
 	else :
 		return form.cleaned_data.get(key,0)
 	
 
 
 class LBASE(ListView):
-	context_paginator_name = "page"
+	context_paginator_name="page_obj"
 	page_n=0
 
 	def get_paginate_by(self, queryset) -> int | None:
 		if len(queryset) >= self.page_n:
 			return len(queryset) // self.page_n
 		else:
 			return super().get_paginate_by(queryset)
```

### Comparing `func_bk-1.0.1/func_bk.egg-info/PKG-INFO` & `func_bk-1.0.2/func_bk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func_bk
-Version: 1.0.1
+Version: 1.0.2
 Summary: add function for normal python and add class(for inheritance) for django
 Author-email: lilo.pio147@mail.ru
 Description-Content-Type: text/markdown
 
 add function 
 
 sejango - 3 arguments form(django),key(in form cleaned data),var(return if key is not find)
```

