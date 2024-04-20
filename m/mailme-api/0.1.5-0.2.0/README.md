# Comparing `tmp/mailme_api-0.1.5.tar.gz` & `tmp/mailme-api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mailme_api-0.1.5.tar", last modified: Tue Sep  5 14:23:08 2017, max compression
+gzip compressed data, was "dist/mailme-api-0.2.0.tar", last modified: Sat Apr 20 16:45:12 2024, max compression
```

## Comparing `mailme_api-0.1.5.tar` & `mailme-api-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-09-05 14:23:08.000000 mailme_api-0.1.5/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-09-05 14:23:08.000000 mailme_api-0.1.5/src/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-09-05 14:23:08.000000 mailme_api-0.1.5/src/mailme/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-09-05 14:23:08.000000 mailme_api-0.1.5/src/mailme/scripts/
--rw-r--r--   0 travis    (2000) travis    (2000)     1235 2017-09-05 14:22:23.000000 mailme_api-0.1.5/src/mailme/scripts/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2012 2017-09-05 14:22:23.000000 mailme_api-0.1.5/src/mailme/scripts/sender.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1240 2017-09-05 14:22:23.000000 mailme_api-0.1.5/src/mailme/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2474 2017-09-05 14:22:23.000000 mailme_api-0.1.5/src/mailme/base.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-09-05 14:23:08.000000 mailme_api-0.1.5/src/mailme_api.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)      955 2017-09-05 14:23:08.000000 mailme_api-0.1.5/src/mailme_api.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)      346 2017-09-05 14:23:08.000000 mailme_api-0.1.5/src/mailme_api.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2017-09-05 14:23:08.000000 mailme_api-0.1.5/src/mailme_api.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2017-09-05 14:23:08.000000 mailme_api-0.1.5/src/mailme_api.egg-info/not-zip-safe
--rw-r--r--   0 travis    (2000) travis    (2000)        7 2017-09-05 14:23:08.000000 mailme_api-0.1.5/src/mailme_api.egg-info/requires.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        7 2017-09-05 14:23:08.000000 mailme_api-0.1.5/src/mailme_api.egg-info/top_level.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       67 2017-09-05 14:23:08.000000 mailme_api-0.1.5/setup.cfg
--rw-r--r--   0 travis    (2000) travis    (2000)     2532 2017-09-05 14:22:23.000000 mailme_api-0.1.5/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)      955 2017-09-05 14:23:08.000000 mailme_api-0.1.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 16:45:12.000000 mailme-api-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     2655 2024-04-20 16:45:07.000000 mailme-api-0.2.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1214 2024-04-20 16:45:07.000000 mailme-api-0.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-20 16:45:12.000000 mailme-api-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2735 2024-04-20 16:45:12.000000 mailme-api-0.2.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 16:45:12.000000 mailme-api-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 16:45:12.000000 mailme-api-0.2.0/src/mailme_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 16:45:12.000000 mailme-api-0.2.0/src/mailme_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      356 2024-04-20 16:45:12.000000 mailme-api-0.2.0/src/mailme_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-20 16:45:12.000000 mailme-api-0.2.0/src/mailme_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2735 2024-04-20 16:45:12.000000 mailme-api-0.2.0/src/mailme_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-20 16:45:12.000000 mailme-api-0.2.0/src/mailme_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 16:45:09.000000 mailme-api-0.2.0/src/mailme_api.egg-info/not-zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 16:45:12.000000 mailme-api-0.2.0/src/mailme/
+-rw-r--r--   0 root         (0) root         (0)     2467 2024-04-20 16:45:07.000000 mailme-api-0.2.0/src/mailme/base.py
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-04-20 16:45:07.000000 mailme-api-0.2.0/src/mailme/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 16:45:12.000000 mailme-api-0.2.0/src/mailme/scripts/
+-rw-r--r--   0 root         (0) root         (0)     1836 2024-04-20 16:45:07.000000 mailme-api-0.2.0/src/mailme/scripts/sender.py
+-rw-r--r--   0 root         (0) root         (0)     1012 2024-04-20 16:45:07.000000 mailme-api-0.2.0/src/mailme/scripts/__init__.py
```

### Comparing `mailme_api-0.1.5/src/mailme/scripts/__init__.py` & `mailme-api-0.2.0/src/mailme/scripts/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Mailme API
-# Copyright (c) 2008-2017 Hive Solutions Lda.
+# Copyright (c) 2008-2020 Hive Solutions Lda.
 #
 # This file is part of Hive Mailme API.
 #
 # Hive Mailme API is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -15,24 +15,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # Apache License for more details.
 #
 # You should have received a copy of the Apache License along with
 # Hive Mailme API. If not, see <http://www.apache.org/licenses/>.
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2017 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import sender
```

### Comparing `mailme_api-0.1.5/src/mailme/scripts/sender.py` & `mailme-api-0.2.0/src/mailme/scripts/sender.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Mailme API
-# Copyright (c) 2008-2017 Hive Solutions Lda.
+# Copyright (c) 2008-2020 Hive Solutions Lda.
 #
 # This file is part of Hive Mailme API.
 #
 # Hive Mailme API is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,49 +18,47 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Mailme API. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2017 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import pprint
 
 import appier
 import mailme
 
+
 def send(*args, **kwargs):
     api = mailme.API()
     return api.send(kwargs)
 
+
 if __name__ == "__main__":
-    receivers = appier.conf("RECEIVERS", [], cast = list)
+    receivers = appier.conf("RECEIVERS", [], cast=list)
     subject = appier.conf("SUBJECT", None)
     title = appier.conf("TITLE", None)
     contents = appier.conf("CONTENTS", None)
     copyright = appier.conf("COPYRIGHT", None)
 
     kwargs = dict()
-    if receivers: kwargs["receivers"] = receivers
-    if subject: kwargs["subject"] = subject
-    if title: kwargs["title"] = title
-    if contents: kwargs["contents"] = contents
-    if copyright: kwargs["copyright"] = copyright
+    if receivers:
+        kwargs["receivers"] = receivers
+    if subject:
+        kwargs["subject"] = subject
+    if title:
+        kwargs["title"] = title
+    if contents:
+        kwargs["contents"] = contents
+    if copyright:
+        kwargs["copyright"] = copyright
 
     result = send(**kwargs)
     pprint.pprint(result)
 else:
     __path__ = []
```

### Comparing `mailme_api-0.1.5/src/mailme/base.py` & `mailme-api-0.2.0/src/mailme/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Mailme API
-# Copyright (c) 2008-2017 Hive Solutions Lda.
+# Copyright (c) 2008-2020 Hive Solutions Lda.
 #
 # This file is part of Hive Mailme API.
 #
 # Hive Mailme API is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,64 +18,74 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Mailme API. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2017 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import appier
 
 BASE_URL = "https://mailme.bemisc.com/api/"
-""" The default base url to be used when no other
-base url value is provided to the constructor """
+""" The default base URL to be used when no other
+base URL value is provided to the constructor """
+
 
 class API(appier.API):
     """
     Implementation of the Mailme API specification
     for a simplified python client usage.
     """
 
     def __init__(self, *args, **kwargs):
         appier.API.__init__(self, *args, **kwargs)
         self.base_url = appier.conf("MAILME_BASE_URL", BASE_URL)
         self.key = appier.conf("MAILME_KEY", None)
-        self.base_url = kwargs.get("base_url", BASE_URL)
+        self.base_url = kwargs.get("base_url", self.base_url)
+        self.key = appier.conf("key", self.key)
 
     def build(
         self,
         method,
         url,
-        data = None,
-        data_j = None,
-        data_m = None,
-        headers = None,
-        params = None,
-        mime = None,
-        kwargs = None
+        data=None,
+        data_j=None,
+        data_m=None,
+        headers=None,
+        params=None,
+        mime=None,
+        kwargs=None,
     ):
         auth = kwargs.pop("auth", True)
-        if auth and self.key: headers["X-Secret-Key"] = self.key
+        if auth and self.key:
+            headers["X-Secret-Key"] = self.key
 
     def ping(self):
         url = self.base_url + "ping"
-        contents = self.get(url, auth = False)
+        contents = self.get(url, auth=False)
         return contents
 
     def send(self, payload):
         url = self.base_url + "send"
-        contents = self.post(url, data_j = payload)
+        contents = self.post(url, data_j=payload)
         return contents
+
+
+class Attachment(dict):
+    pass
+
+
+class AttachmentPayload(dict):
+    pass
+
+
+class Message(dict):
+    pass
+
+
+class MessagePayload(dict):
+    pass
```

### Comparing `mailme_api-0.1.5/setup.py` & `mailme-api-0.2.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Mailme API
-# Copyright (c) 2008-2017 Hive Solutions Lda.
+# Copyright (c) 2008-2020 Hive Solutions Lda.
 #
 # This file is part of Hive Mailme API.
 #
 # Hive Mailme API is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,62 +18,55 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Mailme API. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2017 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import os
 import setuptools
 
 setuptools.setup(
-    name = "mailme_api",
-    version = "0.1.5",
-    author = "Hive Solutions Lda.",
-    author_email = "development@hive.pt",
-    description = "Mailme API Client",
-    license = "Apache License, Version 2.0",
-    keywords = "mailme api",
-    url = "http://mailme-api.hive.pt",
-    zip_safe = False,
-    packages = [
-        "mailme",
-        "mailme.scripts"
-    ],
-    package_dir = {
-        "" : os.path.normpath("src")
-    },
-    install_requires = [
-        "appier"
-    ],
-    classifiers = [
+    name="mailme-api",
+    version="0.2.0",
+    author="Hive Solutions Lda.",
+    author_email="development@hive.pt",
+    description="Mailme API Client",
+    license="Apache License, Version 2.0",
+    keywords="mailme api",
+    url="http://mailme-api.hive.pt",
+    zip_safe=False,
+    packages=["mailme", "mailme.scripts"],
+    package_dir={"": os.path.normpath("src")},
+    install_requires=["appier"],
+    classifiers=[
         "Development Status :: 3 - Alpha",
         "Topic :: Utilities",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.6",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.0",
         "Programming Language :: Python :: 3.1",
         "Programming Language :: Python :: 3.2",
         "Programming Language :: Python :: 3.3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6"
-    ]
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+    ],
+    long_description=open(os.path.join(os.path.dirname(__file__), "README.md"), "rb")
+    .read()
+    .decode("utf-8"),
+    long_description_content_type="text/markdown",
 )
```

