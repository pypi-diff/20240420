# Comparing `tmp/wei_office_simptool-0.0.3.tar.gz` & `tmp/wei_office_simptool-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wei_office_simptool-0.0.3.tar", last modified: Fri Apr 19 08:34:04 2024, max compression
+gzip compressed data, was "wei_office_simptool-0.0.4.tar", last modified: Fri Apr 19 08:57:43 2024, max compression
```

## Comparing `wei_office_simptool-0.0.3.tar` & `wei_office_simptool-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 08:34:04.402133 wei_office_simptool-0.0.3/
--rw-rw-rw-   0        0        0     4854 2024-04-19 08:34:04.400127 wei_office_simptool-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4092 2024-04-19 08:30:50.000000 wei_office_simptool-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-19 08:34:04.402133 wei_office_simptool-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2648 2024-04-19 08:32:20.000000 wei_office_simptool-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:34:04.380078 wei_office_simptool-0.0.3/tests/
--rw-rw-rw-   0        0        0     1359 2024-04-19 06:49:12.000000 wei_office_simptool-0.0.3/tests/__init__.py
--rw-rw-rw-   0        0        0     2101 2024-04-19 06:49:12.000000 wei_office_simptool-0.0.3/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:34:04.383078 wei_office_simptool-0.0.3/wei_office_simptool/
--rw-rw-rw-   0        0        0     1667 2024-04-19 06:49:12.000000 wei_office_simptool-0.0.3/wei_office_simptool/__init__.py
--rw-rw-rw-   0        0        0    14275 2024-04-19 08:31:03.000000 wei_office_simptool-0.0.3/wei_office_simptool/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:34:04.396078 wei_office_simptool-0.0.3/wei_office_simptool.egg-info/
--rw-rw-rw-   0        0        0     4854 2024-04-19 08:34:04.000000 wei_office_simptool-0.0.3/wei_office_simptool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2024-04-19 08:34:04.000000 wei_office_simptool-0.0.3/wei_office_simptool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 08:34:04.000000 wei_office_simptool-0.0.3/wei_office_simptool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-19 08:34:04.000000 wei_office_simptool-0.0.3/wei_office_simptool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-19 08:34:04.000000 wei_office_simptool-0.0.3/wei_office_simptool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 08:57:43.133954 wei_office_simptool-0.0.4/
+-rw-rw-rw-   0        0        0     4854 2024-04-19 08:57:43.130941 wei_office_simptool-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4092 2024-04-19 08:30:50.000000 wei_office_simptool-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-19 08:57:43.133954 wei_office_simptool-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2648 2024-04-19 08:56:17.000000 wei_office_simptool-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:57:43.112941 wei_office_simptool-0.0.4/tests/
+-rw-rw-rw-   0        0        0     1359 2024-04-19 06:49:12.000000 wei_office_simptool-0.0.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     2101 2024-04-19 06:49:12.000000 wei_office_simptool-0.0.4/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:57:43.116949 wei_office_simptool-0.0.4/wei_office_simptool/
+-rw-rw-rw-   0        0        0     1669 2024-04-19 08:47:36.000000 wei_office_simptool-0.0.4/wei_office_simptool/__init__.py
+-rw-rw-rw-   0        0        0    14302 2024-04-19 08:55:33.000000 wei_office_simptool-0.0.4/wei_office_simptool/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:57:43.128939 wei_office_simptool-0.0.4/wei_office_simptool.egg-info/
+-rw-rw-rw-   0        0        0     4854 2024-04-19 08:57:43.000000 wei_office_simptool-0.0.4/wei_office_simptool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2024-04-19 08:57:43.000000 wei_office_simptool-0.0.4/wei_office_simptool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 08:57:43.000000 wei_office_simptool-0.0.4/wei_office_simptool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-19 08:57:43.000000 wei_office_simptool-0.0.4/wei_office_simptool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-19 08:57:43.000000 wei_office_simptool-0.0.4/wei_office_simptool.egg-info/top_level.txt
```

### Comparing `wei_office_simptool-0.0.3/PKG-INFO` & `wei_office_simptool-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wei_office_simptool
-Version: 0.0.3
+Version: 0.0.4
 Summary: 一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换等常见功能,实现1到3行代码完成相关处理的快捷操作。
 Home-page: https://github.com/phoenixlucky/wei_office_simptool
 Author: Ethan Wilkins
 Author-email: thisluckyboy@126.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wei_office_simptool-0.0.3/README.md` & `wei_office_simptool-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `wei_office_simptool-0.0.3/setup.py` & `wei_office_simptool-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 @email:thisluckyboy@126.com
 """
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name='wei_office_simptool',
-    version='0.0.3',
+    version='0.0.4',
     author="Ethan Wilkins",  # 作者
     author_email="thisluckyboy@126.com",  # 作者联系方式，可写自己的邮箱地址
     description="一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换等常见功能,实现1到3行代码完成相关处理的快捷操作。",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/phoenixlucky/wei_office_simptool",  # 自己项目地址，比如github的项目地址
     packages=find_packages(),
```

### Comparing `wei_office_simptool-0.0.3/tests/__init__.py` & `wei_office_simptool-0.0.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `wei_office_simptool-0.0.3/tests/test_utils.py` & `wei_office_simptool-0.0.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wei_office_simptool-0.0.3/wei_office_simptool/__init__.py` & `wei_office_simptool-0.0.4/wei_office_simptool/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,14 @@
 # 导入需要公开的模块或变量
 from .utils import *
 
 # 定义__all__变量
 __all__ = ['utils']
 
 # 执行初始化代码
-print("Initializing package...")
+# print("Initializing package...")
 
 # 定义包级别的变量和函数
 #package_variable = 123
 
 #def package_function():
 #    print("This is a package-level function.")
```

### Comparing `wei_office_simptool-0.0.3/wei_office_simptool/utils.py` & `wei_office_simptool-0.0.4/wei_office_simptool/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,16 +194,16 @@
             self.connection.commit()
             print("Query executed successfully")
         except mysql.connector.Error as err:
             print(f"Error: {err}")
         finally:
             cursor.close()
 
-    def fetch_query(self, query, params=None):
-        cursor = self.connection.cursor()
+    def fetch_query(self, query, params=None,dictionary=False):
+        cursor = self.connection.cursor(dictionary)
         try:
             if params:
                 cursor.execute(query, params)
             else:
                 cursor.execute(query)
             result = cursor.fetchall()
             return result
```

### Comparing `wei_office_simptool-0.0.3/wei_office_simptool.egg-info/PKG-INFO` & `wei_office_simptool-0.0.4/wei_office_simptool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wei_office_simptool
-Version: 0.0.3
+Version: 0.0.4
 Summary: 一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换等常见功能,实现1到3行代码完成相关处理的快捷操作。
 Home-page: https://github.com/phoenixlucky/wei_office_simptool
 Author: Ethan Wilkins
 Author-email: thisluckyboy@126.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

