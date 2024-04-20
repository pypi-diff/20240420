# Comparing `tmp/remote_email_filtering-0.2.3.tar.gz` & `tmp/remote_email_filtering-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remote_email_filtering-0.2.3.tar", max compression
+gzip compressed data, was "remote_email_filtering-0.2.4.tar", max compression
```

## Comparing `remote_email_filtering-0.2.3.tar` & `remote_email_filtering-0.2.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2024-01-07 09:17:16.134292 remote_email_filtering-0.2.3/COPYING
--rw-r--r--   0        0        0      124 2024-01-07 09:17:16.134292 remote_email_filtering-0.2.3/README.rst
--rw-r--r--   0        0        0     1213 2024-04-12 01:06:26.782605 remote_email_filtering-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      132 2024-04-12 01:06:13.559214 remote_email_filtering-0.2.3/src/remote_email_filtering/__init__.py
--rw-r--r--   0        0        0     2470 2024-01-07 09:17:16.137292 remote_email_filtering-0.2.3/src/remote_email_filtering/action.py
--rw-r--r--   0        0        0      295 2024-01-07 09:17:16.137292 remote_email_filtering-0.2.3/src/remote_email_filtering/auth.py
--rw-r--r--   0        0        0     2235 2024-01-07 09:17:16.137292 remote_email_filtering-0.2.3/src/remote_email_filtering/main.py
--rw-r--r--   0        0        0     3027 2024-01-07 09:17:16.137292 remote_email_filtering-0.2.3/src/remote_email_filtering/message.py
--rw-r--r--   0        0        0     9915 2024-04-12 00:50:48.119309 remote_email_filtering-0.2.3/src/remote_email_filtering/remote.py
--rw-r--r--   0        0        0     1305 2024-01-16 10:29:23.216073 remote_email_filtering-0.2.3/src/remote_email_filtering/types.py
--rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 remote_email_filtering-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-01-07 09:17:16.134292 remote_email_filtering-0.2.4/COPYING
+-rw-r--r--   0        0        0      124 2024-01-07 09:17:16.134292 remote_email_filtering-0.2.4/README.rst
+-rw-r--r--   0        0        0     1213 2024-04-20 21:09:00.443089 remote_email_filtering-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      132 2024-04-20 21:09:09.860363 remote_email_filtering-0.2.4/src/remote_email_filtering/__init__.py
+-rw-r--r--   0        0        0     2470 2024-01-07 09:17:16.137292 remote_email_filtering-0.2.4/src/remote_email_filtering/action.py
+-rw-r--r--   0        0        0      295 2024-01-07 09:17:16.137292 remote_email_filtering-0.2.4/src/remote_email_filtering/auth.py
+-rw-r--r--   0        0        0     2235 2024-01-07 09:17:16.137292 remote_email_filtering-0.2.4/src/remote_email_filtering/main.py
+-rw-r--r--   0        0        0     3262 2024-04-20 21:01:31.200408 remote_email_filtering-0.2.4/src/remote_email_filtering/message.py
+-rw-r--r--   0        0        0     9915 2024-04-12 00:50:48.119309 remote_email_filtering-0.2.4/src/remote_email_filtering/remote.py
+-rw-r--r--   0        0        0     1305 2024-01-16 10:29:23.216073 remote_email_filtering-0.2.4/src/remote_email_filtering/types.py
+-rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 remote_email_filtering-0.2.4/PKG-INFO
```

### Comparing `remote_email_filtering-0.2.3/COPYING` & `remote_email_filtering-0.2.4/COPYING`

 * *Files identical despite different names*

### Comparing `remote_email_filtering-0.2.3/pyproject.toml` & `remote_email_filtering-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "remote-email-filtering"
-version = "0.2.3"
+version = "0.2.4"
 description = "Email client library for automation"
 authors = ["Gaurav Juvekar <gauravjuvekar@gmail.com>"]
 license = "MIT"
 readme = 'README.rst'
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Environment :: No Input/Output (Daemon)",
```

### Comparing `remote_email_filtering-0.2.3/src/remote_email_filtering/action.py` & `remote_email_filtering-0.2.4/src/remote_email_filtering/action.py`

 * *Files identical despite different names*

### Comparing `remote_email_filtering-0.2.3/src/remote_email_filtering/main.py` & `remote_email_filtering-0.2.4/src/remote_email_filtering/main.py`

 * *Files identical despite different names*

### Comparing `remote_email_filtering-0.2.3/src/remote_email_filtering/message.py` & `remote_email_filtering-0.2.4/src/remote_email_filtering/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,20 +74,26 @@
     @property
     def Time(self):
         return self.envelope['date']
 
     @property
     def SaneSubject(self):
         ascii_header = self.Subject.decode('ascii', errors='ignore')
-        encoded, charset = email.header.decode_header(ascii_header)[0]
-        if charset is not None:
-            ret = encoded.decode(charset, errors='replace')
-        else:
-            ret = encoded
-        return ret
+
+        def fragment_to_str(maybe_encoded, charset):
+            if isinstance(maybe_encoded, str):
+                return maybe_encoded
+            else:
+                if charset is None:
+                    charset = 'ascii'
+                return maybe_encoded.decode(charset, errors='replace')
+
+        return ''.join((fragment_to_str(e, c)
+                        for (e, c) in
+                            email.header.decode_header(ascii_header)))
 
     @property
     def BodyText(self):
         body = self.body.get_body(preferencelist=('plain',))
         if not body:
             return None
         text = body.get_content()
```

### Comparing `remote_email_filtering-0.2.3/src/remote_email_filtering/remote.py` & `remote_email_filtering-0.2.4/src/remote_email_filtering/remote.py`

 * *Files identical despite different names*

### Comparing `remote_email_filtering-0.2.3/src/remote_email_filtering/types.py` & `remote_email_filtering-0.2.4/src/remote_email_filtering/types.py`

 * *Files identical despite different names*

### Comparing `remote_email_filtering-0.2.3/PKG-INFO` & `remote_email_filtering-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remote-email-filtering
-Version: 0.2.3
+Version: 0.2.4
 Summary: Email client library for automation
 Home-page: https://github.com/gauravjuvekar/remote-email-filtering
 License: MIT
 Author: Gaurav Juvekar
 Author-email: gauravjuvekar@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

