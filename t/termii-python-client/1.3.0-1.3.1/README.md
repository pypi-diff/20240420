# Comparing `tmp/termii_python_client-1.3.0.tar.gz` & `tmp/termii_python_client-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termii_python_client-1.3.0.tar", last modified: Fri Apr 19 08:02:17 2024, max compression
+gzip compressed data, was "termii_python_client-1.3.1.tar", last modified: Sat Apr 20 14:14:06 2024, max compression
```

## Comparing `termii_python_client-1.3.0.tar` & `termii_python_client-1.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:17.911800 termii_python_client-1.3.0/
--rw-rw-rw-   0        0        0     1093 2024-04-18 09:23:17.000000 termii_python_client-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     5179 2024-04-19 08:02:17.896837 termii_python_client-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4565 2024-04-19 07:54:48.000000 termii_python_client-1.3.0/README.md
--rw-rw-rw-   0        0        0      725 2024-04-19 08:00:41.000000 termii_python_client-1.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-19 08:02:17.912795 termii_python_client-1.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:17.396175 termii_python_client-1.3.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:17.561732 termii_python_client-1.3.0/src/termii/
--rw-rw-rw-   0        0        0        0 2024-04-16 19:13:19.000000 termii_python_client-1.3.0/src/termii/__init__.py
--rw-rw-rw-   0        0        0    21752 2024-04-19 07:59:45.000000 termii_python_client-1.3.0/src/termii/termii.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:17.894845 termii_python_client-1.3.0/src/termii_python_client.egg-info/
--rw-rw-rw-   0        0        0     5179 2024-04-19 08:02:17.000000 termii_python_client-1.3.0/src/termii_python_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2024-04-19 08:02:17.000000 termii_python_client-1.3.0/src/termii_python_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 08:02:17.000000 termii_python_client-1.3.0/src/termii_python_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-19 08:02:17.000000 termii_python_client-1.3.0/src/termii_python_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-19 08:02:17.885866 termii_python_client-1.3.0/tests/
--rw-rw-rw-   0        0        0      932 2024-04-19 07:35:12.000000 termii_python_client-1.3.0/tests/test_contact.py
--rw-rw-rw-   0        0        0     1390 2024-04-19 07:35:19.000000 termii_python_client-1.3.0/tests/test_insights.py
--rw-rw-rw-   0        0        0     1698 2024-04-19 07:35:25.000000 termii_python_client-1.3.0/tests/test_messaging.py
--rw-rw-rw-   0        0        0     1203 2024-04-19 07:35:30.000000 termii_python_client-1.3.0/tests/test_number_api.py
--rw-rw-rw-   0        0        0     2233 2024-04-19 07:35:37.000000 termii_python_client-1.3.0/tests/test_phonebooks.py
--rw-rw-rw-   0        0        0      653 2024-04-19 07:35:43.000000 termii_python_client-1.3.0/tests/test_sender_id.py
--rw-rw-rw-   0        0        0     2196 2024-04-19 07:34:50.000000 termii_python_client-1.3.0/tests/test_token.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:14:06.848866 termii_python_client-1.3.1/
+-rw-rw-rw-   0        0        0     1093 2024-04-18 09:23:17.000000 termii_python_client-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0     5179 2024-04-20 14:14:06.834907 termii_python_client-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4565 2024-04-19 07:54:48.000000 termii_python_client-1.3.1/README.md
+-rw-rw-rw-   0        0        0      725 2024-04-20 14:13:48.000000 termii_python_client-1.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-20 14:14:06.848866 termii_python_client-1.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-20 14:14:06.727220 termii_python_client-1.3.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-20 14:14:06.744175 termii_python_client-1.3.1/src/termii/
+-rw-rw-rw-   0        0        0        0 2024-04-16 19:13:19.000000 termii_python_client-1.3.1/src/termii/__init__.py
+-rw-rw-rw-   0        0        0    21686 2024-04-20 13:57:25.000000 termii_python_client-1.3.1/src/termii/termii.py
+drwxrwxrwx   0        0        0        0 2024-04-20 14:14:06.833907 termii_python_client-1.3.1/src/termii_python_client.egg-info/
+-rw-rw-rw-   0        0        0     5179 2024-04-20 14:14:06.000000 termii_python_client-1.3.1/src/termii_python_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2024-04-20 14:14:06.000000 termii_python_client-1.3.1/src/termii_python_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 14:14:06.000000 termii_python_client-1.3.1/src/termii_python_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-20 14:14:06.000000 termii_python_client-1.3.1/src/termii_python_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 14:14:06.830915 termii_python_client-1.3.1/tests/
+-rw-rw-rw-   0        0        0      932 2024-04-19 07:35:12.000000 termii_python_client-1.3.1/tests/test_contact.py
+-rw-rw-rw-   0        0        0     1390 2024-04-19 07:35:19.000000 termii_python_client-1.3.1/tests/test_insights.py
+-rw-rw-rw-   0        0        0     1698 2024-04-19 07:35:25.000000 termii_python_client-1.3.1/tests/test_messaging.py
+-rw-rw-rw-   0        0        0     1203 2024-04-19 07:35:30.000000 termii_python_client-1.3.1/tests/test_number_api.py
+-rw-rw-rw-   0        0        0     2233 2024-04-19 07:35:37.000000 termii_python_client-1.3.1/tests/test_phonebooks.py
+-rw-rw-rw-   0        0        0      653 2024-04-19 07:35:43.000000 termii_python_client-1.3.1/tests/test_sender_id.py
+-rw-rw-rw-   0        0        0     2196 2024-04-19 07:34:50.000000 termii_python_client-1.3.1/tests/test_token.py
```

### Comparing `termii_python_client-1.3.0/LICENSE` & `termii_python_client-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `termii_python_client-1.3.0/PKG-INFO` & `termii_python_client-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termii-python-client
-Version: 1.3.0
+Version: 1.3.1
 Summary: Termii python package
 Author-email: "Gabriel Michael Ojomakpene [codewitgabi]" <codewitgabi222@gmail.com>, Joshua Joseph <joshuajosephizzyjosh@gmail.com>
 Project-URL: Homepage, https://github.com/codewitgabi/python-termii
 Project-URL: Issues, https://github.com/codewitgabi/python-termii/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `termii_python_client-1.3.0/README.md` & `termii_python_client-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `termii_python_client-1.3.0/pyproject.toml` & `termii_python_client-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "requests>=2.31.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "termii-python-client"
-version = "1.3.0"
+version = "1.3.1"
 authors = [ { name="Gabriel Michael Ojomakpene [codewitgabi]", email="codewitgabi222@gmail.com" }, { name="Joshua Joseph", email="joshuajosephizzyjosh@gmail.com" },
 ]
 description = "Termii python package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `termii_python_client-1.3.0/src/termii/termii.py` & `termii_python_client-1.3.1/src/termii/termii.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,14 @@
         """
         Get phonebooks using these APIs. Each phonebook can be identified by a unique ID, which makes it easier to edit or delete a phonebook.
         """
 
         response = requests.get(
             f"{self.__base_url}/phonebooks?api_key={self.api_key}")
 
-        print(response.json())
         return response.json()
 
     def create_phonebook(self, phonebook_name: str, description: Optional[str] = None) -> Response:
         """
         Create a phonebook
 
         Arguments:
@@ -229,16 +228,14 @@
     def get_contact(self, phonebook_id: str):
         """
         Get all available contacts
         """
 
         response = requests.get(
             f"{self.__base_url}/phonebooks/{phonebook_id}/contacts?api_key={self.api_key}")
-
-        print(response.json())
         return response.json()
 
     def add_contact(self, phonebook_id: str, phone_number: str, country_code: Optional[int] = None, email_address: Optional[str] = None, first_name: Optional[str] = None, last_name: Optional[str] = None, company: Optional[str] = None) -> Response:
         """
         Adds a single contact to a phonebook
 
         Arguments:
```

### Comparing `termii_python_client-1.3.0/src/termii_python_client.egg-info/PKG-INFO` & `termii_python_client-1.3.1/src/termii_python_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termii-python-client
-Version: 1.3.0
+Version: 1.3.1
 Summary: Termii python package
 Author-email: "Gabriel Michael Ojomakpene [codewitgabi]" <codewitgabi222@gmail.com>, Joshua Joseph <joshuajosephizzyjosh@gmail.com>
 Project-URL: Homepage, https://github.com/codewitgabi/python-termii
 Project-URL: Issues, https://github.com/codewitgabi/python-termii/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `termii_python_client-1.3.0/tests/test_contact.py` & `termii_python_client-1.3.1/tests/test_contact.py`

 * *Files identical despite different names*

### Comparing `termii_python_client-1.3.0/tests/test_insights.py` & `termii_python_client-1.3.1/tests/test_insights.py`

 * *Files identical despite different names*

### Comparing `termii_python_client-1.3.0/tests/test_messaging.py` & `termii_python_client-1.3.1/tests/test_messaging.py`

 * *Files identical despite different names*

### Comparing `termii_python_client-1.3.0/tests/test_number_api.py` & `termii_python_client-1.3.1/tests/test_number_api.py`

 * *Files identical despite different names*

### Comparing `termii_python_client-1.3.0/tests/test_phonebooks.py` & `termii_python_client-1.3.1/tests/test_phonebooks.py`

 * *Files identical despite different names*

### Comparing `termii_python_client-1.3.0/tests/test_sender_id.py` & `termii_python_client-1.3.1/tests/test_sender_id.py`

 * *Files identical despite different names*

### Comparing `termii_python_client-1.3.0/tests/test_token.py` & `termii_python_client-1.3.1/tests/test_token.py`

 * *Files identical despite different names*

