# Comparing `tmp/easy_ec2-0.1.8.tar.gz` & `tmp/easy_ec2-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_ec2-0.1.8.tar", max compression
+gzip compressed data, was "easy_ec2-0.1.9.tar", max compression
```

## Comparing `easy_ec2-0.1.8.tar` & `easy_ec2-0.1.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    11357 2024-04-19 13:05:24.656920 easy_ec2-0.1.8/LICENSE
--rw-r--r--   0        0        0     8877 2024-04-20 18:50:36.614165 easy_ec2-0.1.8/README.md
--rw-r--r--   0        0        0     1948 2024-04-20 13:17:57.832599 easy_ec2-0.1.8/easy_ec2/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 13:05:24.657397 easy_ec2-0.1.8/easy_ec2/cloudwatch/__init__.py
--rw-r--r--   0        0        0      781 2024-04-19 13:17:42.144309 easy_ec2-0.1.8/easy_ec2/cloudwatch/cloudwatch.py
--rw-r--r--   0        0        0     1470 2024-04-19 13:17:40.250005 easy_ec2-0.1.8/easy_ec2/cloudwatch/create.py
--rw-r--r--   0        0        0     1459 2024-04-19 13:17:38.990774 easy_ec2-0.1.8/easy_ec2/cloudwatch/delete.py
--rw-r--r--   0        0        0      876 2024-04-19 13:17:37.559820 easy_ec2-0.1.8/easy_ec2/cloudwatch/list.py
--rw-r--r--   0        0        0     6936 2024-04-19 13:16:15.196284 easy_ec2-0.1.8/easy_ec2/compound.py
--rw-r--r--   0        0        0      987 2024-04-19 13:16:17.105092 easy_ec2-0.1.8/easy_ec2/ec2/__init__.py
--rw-r--r--   0        0        0     3684 2024-04-19 13:17:36.177806 easy_ec2-0.1.8/easy_ec2/ec2/config_parser.py
--rw-r--r--   0        0        0     3611 2024-04-19 13:17:34.123795 easy_ec2-0.1.8/easy_ec2/ec2/connect.py
--rw-r--r--   0        0        0     1703 2024-04-19 13:17:32.645477 easy_ec2-0.1.8/easy_ec2/ec2/create.py
--rw-r--r--   0        0        0     2655 2024-04-19 13:17:31.239555 easy_ec2-0.1.8/easy_ec2/ec2/ec2.py
--rw-r--r--   0        0        0     2623 2024-04-19 13:05:24.658975 easy_ec2-0.1.8/easy_ec2/ec2/ec2_connections_management.py
--rw-r--r--   0        0        0      399 2024-04-19 13:17:29.694441 easy_ec2-0.1.8/easy_ec2/ec2/ec2_instance_management.py
--rw-r--r--   0        0        0     1909 2024-04-19 13:17:28.199703 easy_ec2-0.1.8/easy_ec2/ec2/list.py
--rw-r--r--   0        0        0     1475 2024-04-19 13:17:26.723662 easy_ec2-0.1.8/easy_ec2/ec2/logs.py
--rw-r--r--   0        0        0     2089 2024-04-19 13:05:24.659413 easy_ec2-0.1.8/easy_ec2/ec2/script.py
--rw-r--r--   0        0        0     2959 2024-04-19 13:16:19.283981 easy_ec2-0.1.8/easy_ec2/ec2/ssh.py
--rw-r--r--   0        0        0      830 2024-04-19 13:17:24.924812 easy_ec2-0.1.8/easy_ec2/ec2/start.py
--rw-r--r--   0        0        0      824 2024-04-19 13:17:23.557083 easy_ec2-0.1.8/easy_ec2/ec2/stop.py
--rw-r--r--   0        0        0        0 2024-04-19 13:05:24.659773 easy_ec2-0.1.8/easy_ec2/ec2/stop_all.py
--rw-r--r--   0        0        0      994 2024-04-19 13:17:21.918359 easy_ec2-0.1.8/easy_ec2/ec2/terminate.py
--rw-r--r--   0        0        0      670 2024-04-19 13:17:04.850898 easy_ec2-0.1.8/easy_ec2/main.py
--rw-r--r--   0        0        0        0 2024-04-19 13:05:24.660133 easy_ec2-0.1.8/easy_ec2/profile/__init__.py
--rw-r--r--   0        0        0     1294 2024-04-19 13:17:20.493493 easy_ec2-0.1.8/easy_ec2/profile/active.py
--rw-r--r--   0        0        0     3945 2024-04-19 13:17:18.932083 easy_ec2-0.1.8/easy_ec2/profile/ownership.py
--rw-r--r--   0        0        0     1293 2024-04-19 13:17:17.542942 easy_ec2-0.1.8/easy_ec2/profile/profile.py
--rw-r--r--   0        0        0     1475 2024-04-19 13:17:14.848523 easy_ec2-0.1.8/easy_ec2/profile/validation.py
--rw-r--r--   0        0        0     2828 2024-04-19 13:17:46.175306 easy_ec2-0.1.8/easy_ec2/router.py
--rw-r--r--   0        0        0      859 2024-04-19 13:17:44.197673 easy_ec2-0.1.8/easy_ec2/setup_session.py
--rw-r--r--   0        0        0        0 2024-04-19 13:05:24.660852 easy_ec2-0.1.8/easy_ec2/utilities/__init__.py
--rw-r--r--   0        0        0     1882 2024-04-19 13:17:12.219315 easy_ec2-0.1.8/easy_ec2/utilities/aws_profile_parser.py
--rw-r--r--   0        0        0     2471 2024-04-19 13:05:24.661084 easy_ec2-0.1.8/easy_ec2/utilities/decorators.py
--rw-r--r--   0        0        0     1259 2024-04-19 13:05:24.661193 easy_ec2-0.1.8/easy_ec2/utilities/logger_maker.py
--rw-r--r--   0        0        0     1048 2024-04-19 13:15:09.137657 easy_ec2-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    10088 1970-01-01 00:00:00.000000 easy_ec2-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-20 21:06:56.354748 easy_ec2-0.1.9/LICENSE
+-rw-r--r--   0        0        0     8877 2024-04-20 21:06:56.354748 easy_ec2-0.1.9/README.md
+-rw-r--r--   0        0        0     1948 2024-04-20 21:06:56.354748 easy_ec2-0.1.9/easy_ec2/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 21:06:56.354748 easy_ec2-0.1.9/easy_ec2/cloudwatch/__init__.py
+-rw-r--r--   0        0        0      781 2024-04-20 21:06:56.354748 easy_ec2-0.1.9/easy_ec2/cloudwatch/cloudwatch.py
+-rw-r--r--   0        0        0     1470 2024-04-20 21:06:56.354748 easy_ec2-0.1.9/easy_ec2/cloudwatch/create.py
+-rw-r--r--   0        0        0     1459 2024-04-20 21:06:56.354748 easy_ec2-0.1.9/easy_ec2/cloudwatch/delete.py
+-rw-r--r--   0        0        0      876 2024-04-20 21:06:56.354748 easy_ec2-0.1.9/easy_ec2/cloudwatch/list.py
+-rw-r--r--   0        0        0     6936 2024-04-20 21:06:56.354748 easy_ec2-0.1.9/easy_ec2/compound.py
+-rw-r--r--   0        0        0      987 2024-04-20 21:06:56.354748 easy_ec2-0.1.9/easy_ec2/ec2/__init__.py
+-rw-r--r--   0        0        0     3684 2024-04-20 21:06:56.354748 easy_ec2-0.1.9/easy_ec2/ec2/config_parser.py
+-rw-r--r--   0        0        0     3611 2024-04-20 21:06:56.354748 easy_ec2-0.1.9/easy_ec2/ec2/connect.py
+-rw-r--r--   0        0        0     1703 2024-04-20 21:06:56.354748 easy_ec2-0.1.9/easy_ec2/ec2/create.py
+-rw-r--r--   0        0        0     2655 2024-04-20 21:06:56.354748 easy_ec2-0.1.9/easy_ec2/ec2/ec2.py
+-rw-r--r--   0        0        0     2623 2024-04-20 21:06:56.354748 easy_ec2-0.1.9/easy_ec2/ec2/ec2_connections_management.py
+-rw-r--r--   0        0        0      399 2024-04-20 21:06:56.354748 easy_ec2-0.1.9/easy_ec2/ec2/ec2_instance_management.py
+-rw-r--r--   0        0        0     1909 2024-04-20 21:06:56.354748 easy_ec2-0.1.9/easy_ec2/ec2/list.py
+-rw-r--r--   0        0        0     1475 2024-04-20 21:06:56.354748 easy_ec2-0.1.9/easy_ec2/ec2/logs.py
+-rw-r--r--   0        0        0     2089 2024-04-20 21:06:56.354748 easy_ec2-0.1.9/easy_ec2/ec2/script.py
+-rw-r--r--   0        0        0     2959 2024-04-20 21:06:56.354748 easy_ec2-0.1.9/easy_ec2/ec2/ssh.py
+-rw-r--r--   0        0        0      830 2024-04-20 21:06:56.354748 easy_ec2-0.1.9/easy_ec2/ec2/start.py
+-rw-r--r--   0        0        0      824 2024-04-20 21:06:56.358748 easy_ec2-0.1.9/easy_ec2/ec2/stop.py
+-rw-r--r--   0        0        0        0 2024-04-20 21:06:56.358748 easy_ec2-0.1.9/easy_ec2/ec2/stop_all.py
+-rw-r--r--   0        0        0      994 2024-04-20 21:06:56.358748 easy_ec2-0.1.9/easy_ec2/ec2/terminate.py
+-rw-r--r--   0        0        0      670 2024-04-20 21:06:56.358748 easy_ec2-0.1.9/easy_ec2/main.py
+-rw-r--r--   0        0        0        0 2024-04-20 21:06:56.358748 easy_ec2-0.1.9/easy_ec2/profile/__init__.py
+-rw-r--r--   0        0        0     1294 2024-04-20 21:06:56.358748 easy_ec2-0.1.9/easy_ec2/profile/active.py
+-rw-r--r--   0        0        0     3945 2024-04-20 21:06:56.358748 easy_ec2-0.1.9/easy_ec2/profile/ownership.py
+-rw-r--r--   0        0        0     1293 2024-04-20 21:06:56.358748 easy_ec2-0.1.9/easy_ec2/profile/profile.py
+-rw-r--r--   0        0        0     1475 2024-04-20 21:06:56.358748 easy_ec2-0.1.9/easy_ec2/profile/validation.py
+-rw-r--r--   0        0        0     2828 2024-04-20 21:06:56.358748 easy_ec2-0.1.9/easy_ec2/router.py
+-rw-r--r--   0        0        0      859 2024-04-20 21:06:56.358748 easy_ec2-0.1.9/easy_ec2/setup_session.py
+-rw-r--r--   0        0        0        0 2024-04-20 21:06:56.358748 easy_ec2-0.1.9/easy_ec2/utilities/__init__.py
+-rw-r--r--   0        0        0     1882 2024-04-20 21:06:56.358748 easy_ec2-0.1.9/easy_ec2/utilities/aws_profile_parser.py
+-rw-r--r--   0        0        0     2471 2024-04-20 21:06:56.358748 easy_ec2-0.1.9/easy_ec2/utilities/decorators.py
+-rw-r--r--   0        0        0     1259 2024-04-20 21:06:56.358748 easy_ec2-0.1.9/easy_ec2/utilities/logger_maker.py
+-rw-r--r--   0        0        0     1048 2024-04-20 21:06:56.358748 easy_ec2-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    10088 1970-01-01 00:00:00.000000 easy_ec2-0.1.9/PKG-INFO
```

### Comparing `easy_ec2-0.1.8/LICENSE` & `easy_ec2-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/README.md` & `easy_ec2-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/__init__.py` & `easy_ec2-0.1.9/easy_ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/cloudwatch/cloudwatch.py` & `easy_ec2-0.1.9/easy_ec2/cloudwatch/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/cloudwatch/create.py` & `easy_ec2-0.1.9/easy_ec2/cloudwatch/create.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/cloudwatch/delete.py` & `easy_ec2-0.1.9/easy_ec2/cloudwatch/delete.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/cloudwatch/list.py` & `easy_ec2-0.1.9/easy_ec2/cloudwatch/list.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/compound.py` & `easy_ec2-0.1.9/easy_ec2/compound.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/ec2/__init__.py` & `easy_ec2-0.1.9/easy_ec2/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/ec2/config_parser.py` & `easy_ec2-0.1.9/easy_ec2/ec2/config_parser.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/ec2/connect.py` & `easy_ec2-0.1.9/easy_ec2/ec2/connect.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/ec2/create.py` & `easy_ec2-0.1.9/easy_ec2/ec2/create.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/ec2/ec2.py` & `easy_ec2-0.1.9/easy_ec2/ec2/ec2.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/ec2/ec2_connections_management.py` & `easy_ec2-0.1.9/easy_ec2/ec2/ec2_connections_management.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/ec2/list.py` & `easy_ec2-0.1.9/easy_ec2/ec2/list.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/ec2/logs.py` & `easy_ec2-0.1.9/easy_ec2/ec2/logs.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/ec2/script.py` & `easy_ec2-0.1.9/easy_ec2/ec2/script.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/ec2/ssh.py` & `easy_ec2-0.1.9/easy_ec2/ec2/ssh.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/ec2/start.py` & `easy_ec2-0.1.9/easy_ec2/ec2/start.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/ec2/stop.py` & `easy_ec2-0.1.9/easy_ec2/ec2/stop.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/ec2/terminate.py` & `easy_ec2-0.1.9/easy_ec2/ec2/terminate.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/main.py` & `easy_ec2-0.1.9/easy_ec2/main.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/profile/active.py` & `easy_ec2-0.1.9/easy_ec2/profile/active.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/profile/ownership.py` & `easy_ec2-0.1.9/easy_ec2/profile/ownership.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/profile/profile.py` & `easy_ec2-0.1.9/easy_ec2/profile/profile.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/profile/validation.py` & `easy_ec2-0.1.9/easy_ec2/profile/validation.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/router.py` & `easy_ec2-0.1.9/easy_ec2/router.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/setup_session.py` & `easy_ec2-0.1.9/easy_ec2/setup_session.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/utilities/aws_profile_parser.py` & `easy_ec2-0.1.9/easy_ec2/utilities/aws_profile_parser.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/utilities/decorators.py` & `easy_ec2-0.1.9/easy_ec2/utilities/decorators.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/easy_ec2/utilities/logger_maker.py` & `easy_ec2-0.1.9/easy_ec2/utilities/logger_maker.py`

 * *Files identical despite different names*

### Comparing `easy_ec2-0.1.8/pyproject.toml` & `easy_ec2-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easy_ec2"
-version = "0.1.8"
+version = "0.1.9"
 description = "`easy_ec2` simplifies remote `ec2` usage in vscode by adding a command line interface (CLI) and abridged Python API that allows you to easily create, manage, and tear-down AWS resources using `boto3` and `awscli` in a simple, easy to use, and easy to refactor `.yaml` configuration file."
 authors = ["Jeremy Watt <jermwatt@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/jermwatt/easy_ec2"
 packages = [{include = "easy_ec2"}]
```

### Comparing `easy_ec2-0.1.8/PKG-INFO` & `easy_ec2-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_ec2
-Version: 0.1.8
+Version: 0.1.9
 Summary: `easy_ec2` simplifies remote `ec2` usage in vscode by adding a command line interface (CLI) and abridged Python API that allows you to easily create, manage, and tear-down AWS resources using `boto3` and `awscli` in a simple, easy to use, and easy to refactor `.yaml` configuration file.
 Home-page: https://github.com/jermwatt/easy_ec2
 Author: Jeremy Watt
 Author-email: jermwatt@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

