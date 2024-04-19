# Comparing `tmp/cf2tf-0.7.0a0.tar.gz` & `tmp/cf2tf-0.7.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf2tf-0.7.0a0.tar", max compression
+gzip compressed data, was "cf2tf-0.7.1a0.tar", max compression
```

## Comparing `cf2tf-0.7.0a0.tar` & `cf2tf-0.7.1a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/LICENSE.txt
--rw-r--r--   0        0        0     7485 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/README.md
--rw-r--r--   0        0        0     1089 2024-04-19 21:26:04.618107 cf2tf-0.7.0a0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/__init__.py
--rw-r--r--   0        0        0     1451 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/app.py
--rw-r--r--   0        0        0       46 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/cloudformation/__init__.py
--rw-r--r--   0        0        0     2621 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/cloudformation/_template.py
--rw-r--r--   0        0        0        0 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/conversion/__init__.py
--rw-r--r--   0        0        0    32491 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/conversion/expressions.py
--rw-r--r--   0        0        0     2026 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/conversion/overrides.py
--rw-r--r--   0        0        0    21718 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/convert.py
--rw-r--r--   0        0        0     2673 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/save.py
--rw-r--r--   0        0        0        0 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/terraform/__init__.py
--rw-r--r--   0        0        0      368 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/terraform/_configuration.py
--rw-r--r--   0        0        0     2199 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/terraform/blocks.py
--rw-r--r--   0        0        0     3995 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/terraform/code.py
--rw-r--r--   0        0        0     4674 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/terraform/doc_file.py
--rw-r--r--   0        0        0      304 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/terraform/hcl2/__init__.py
--rw-r--r--   0        0        0     2971 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/terraform/hcl2/_block.py
--rw-r--r--   0        0        0     1815 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/terraform/hcl2/complex.py
--rw-r--r--   0        0        0      868 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/terraform/hcl2/custom.py
--rw-r--r--   0        0        0     2673 2024-04-19 21:25:54.606101 cf2tf-0.7.0a0/src/cf2tf/terraform/hcl2/primitive.py
--rw-r--r--   0        0        0     8533 1970-01-01 00:00:00.000000 cf2tf-0.7.0a0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-19 22:16:37.205552 cf2tf-0.7.1a0/LICENSE.txt
+-rw-r--r--   0        0        0     7485 2024-04-19 22:16:37.205552 cf2tf-0.7.1a0/README.md
+-rw-r--r--   0        0        0     1089 2024-04-19 22:16:48.533600 cf2tf-0.7.1a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-19 22:16:37.209552 cf2tf-0.7.1a0/src/cf2tf/__init__.py
+-rw-r--r--   0        0        0     1451 2024-04-19 22:16:37.209552 cf2tf-0.7.1a0/src/cf2tf/app.py
+-rw-r--r--   0        0        0       46 2024-04-19 22:16:37.209552 cf2tf-0.7.1a0/src/cf2tf/cloudformation/__init__.py
+-rw-r--r--   0        0        0     2621 2024-04-19 22:16:37.209552 cf2tf-0.7.1a0/src/cf2tf/cloudformation/_template.py
+-rw-r--r--   0        0        0        0 2024-04-19 22:16:37.209552 cf2tf-0.7.1a0/src/cf2tf/conversion/__init__.py
+-rw-r--r--   0        0        0    32457 2024-04-19 22:16:37.209552 cf2tf-0.7.1a0/src/cf2tf/conversion/expressions.py
+-rw-r--r--   0        0        0     2026 2024-04-19 22:16:37.209552 cf2tf-0.7.1a0/src/cf2tf/conversion/overrides.py
+-rw-r--r--   0        0        0    21718 2024-04-19 22:16:37.209552 cf2tf-0.7.1a0/src/cf2tf/convert.py
+-rw-r--r--   0        0        0     2673 2024-04-19 22:16:37.209552 cf2tf-0.7.1a0/src/cf2tf/save.py
+-rw-r--r--   0        0        0        0 2024-04-19 22:16:37.209552 cf2tf-0.7.1a0/src/cf2tf/terraform/__init__.py
+-rw-r--r--   0        0        0      368 2024-04-19 22:16:37.209552 cf2tf-0.7.1a0/src/cf2tf/terraform/_configuration.py
+-rw-r--r--   0        0        0     2199 2024-04-19 22:16:37.209552 cf2tf-0.7.1a0/src/cf2tf/terraform/blocks.py
+-rw-r--r--   0        0        0     3995 2024-04-19 22:16:37.209552 cf2tf-0.7.1a0/src/cf2tf/terraform/code.py
+-rw-r--r--   0        0        0     4674 2024-04-19 22:16:37.209552 cf2tf-0.7.1a0/src/cf2tf/terraform/doc_file.py
+-rw-r--r--   0        0        0      304 2024-04-19 22:16:37.209552 cf2tf-0.7.1a0/src/cf2tf/terraform/hcl2/__init__.py
+-rw-r--r--   0        0        0     2971 2024-04-19 22:16:37.209552 cf2tf-0.7.1a0/src/cf2tf/terraform/hcl2/_block.py
+-rw-r--r--   0        0        0     1815 2024-04-19 22:16:37.209552 cf2tf-0.7.1a0/src/cf2tf/terraform/hcl2/complex.py
+-rw-r--r--   0        0        0      868 2024-04-19 22:16:37.209552 cf2tf-0.7.1a0/src/cf2tf/terraform/hcl2/custom.py
+-rw-r--r--   0        0        0     2673 2024-04-19 22:16:37.209552 cf2tf-0.7.1a0/src/cf2tf/terraform/hcl2/primitive.py
+-rw-r--r--   0        0        0     8533 1970-01-01 00:00:00.000000 cf2tf-0.7.1a0/PKG-INFO
```

### Comparing `cf2tf-0.7.0a0/LICENSE.txt` & `cf2tf-0.7.1a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.0a0/README.md` & `cf2tf-0.7.1a0/README.md`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.0a0/pyproject.toml` & `cf2tf-0.7.1a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cf2tf"
-version = "0.7.0a0"
+version = "0.7.1a0"
 description = "Convert Cloudformation Templates to Terraform."
 readme = "README.md"
 authors = ["Levi Blaney <shadycuz@gmail.com>"]
 repository = "https://github.com/DontShaveTheYak/cf2tf"
 keywords = ["cloudformation", "terraform", "cf2tf", "convert", "cloud", "conversion"]
 license = "GPL-3.0-only"
```

### Comparing `cf2tf-0.7.0a0/src/cf2tf/app.py` & `cf2tf-0.7.1a0/src/cf2tf/app.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.0a0/src/cf2tf/cloudformation/_template.py` & `cf2tf-0.7.1a0/src/cf2tf/cloudformation/_template.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.0a0/src/cf2tf/conversion/expressions.py` & `cf2tf-0.7.1a0/src/cf2tf/conversion/expressions.py`

 * *Files 1% similar despite different names*

```diff
@@ -536,19 +536,19 @@
 
     data = [
         data for data in template.post_proccess_blocks if isinstance(data, hcl2.Data)
     ]
 
     if not data:
         az_data = hcl2.Data(
-            "available", "availability_zones", {"state": StringType("available")}
+            "available", "aws_availability_zones", {"state": StringType("available")}
         )
         template.post_proccess_blocks.insert(0, az_data)
 
-    return LiteralType("data.aws_availability_zones.available.names")
+    return az_data.ref("names")
 
 
 # todo Handle functions that are not applicable to terraform.
 def import_value(template: "TemplateConverter", name: Any):
     if not isinstance(name, str):
         raise TypeError(
             f"The import value type was expected to be string not {type(name)}"
```

### Comparing `cf2tf-0.7.0a0/src/cf2tf/conversion/overrides.py` & `cf2tf-0.7.1a0/src/cf2tf/conversion/overrides.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.0a0/src/cf2tf/convert.py` & `cf2tf-0.7.1a0/src/cf2tf/convert.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.0a0/src/cf2tf/save.py` & `cf2tf-0.7.1a0/src/cf2tf/save.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.0a0/src/cf2tf/terraform/blocks.py` & `cf2tf-0.7.1a0/src/cf2tf/terraform/blocks.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.0a0/src/cf2tf/terraform/code.py` & `cf2tf-0.7.1a0/src/cf2tf/terraform/code.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.0a0/src/cf2tf/terraform/doc_file.py` & `cf2tf-0.7.1a0/src/cf2tf/terraform/doc_file.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.0a0/src/cf2tf/terraform/hcl2/_block.py` & `cf2tf-0.7.1a0/src/cf2tf/terraform/hcl2/_block.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.0a0/src/cf2tf/terraform/hcl2/complex.py` & `cf2tf-0.7.1a0/src/cf2tf/terraform/hcl2/complex.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.0a0/src/cf2tf/terraform/hcl2/custom.py` & `cf2tf-0.7.1a0/src/cf2tf/terraform/hcl2/custom.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.0a0/src/cf2tf/terraform/hcl2/primitive.py` & `cf2tf-0.7.1a0/src/cf2tf/terraform/hcl2/primitive.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.7.0a0/PKG-INFO` & `cf2tf-0.7.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf2tf
-Version: 0.7.0a0
+Version: 0.7.1a0
 Summary: Convert Cloudformation Templates to Terraform.
 Home-page: https://github.com/DontShaveTheYak/cf2tf
 License: GPL-3.0-only
 Keywords: cloudformation,terraform,cf2tf,convert,cloud,conversion
 Author: Levi Blaney
 Author-email: shadycuz@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cf2tf Version: 0.7.0a0 Summary: Convert
+Metadata-Version: 2.1 Name: cf2tf Version: 0.7.1a0 Summary: Convert
 Cloudformation Templates to Terraform. Home-page: https://github.com/
 DontShaveTheYak/cf2tf License: GPL-3.0-only Keywords:
 cloudformation,terraform,cf2tf,convert,cloud,conversion Author: Levi Blaney
 Author-email: shadycuz@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

