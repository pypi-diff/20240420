# Comparing `tmp/whoisit-2.7.3.tar.gz` & `tmp/whoisit-2.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whoisit-2.7.3.tar", last modified: Wed Sep  6 06:56:26 2023, max compression
+gzip compressed data, was "whoisit-2.7.4.tar", last modified: Sat Apr 20 06:10:52 2024, max compression
```

## Comparing `whoisit-2.7.3.tar` & `whoisit-2.7.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-09-06 06:56:26.280486 whoisit-2.7.3/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1528 2021-06-06 06:10:53.000000 whoisit-2.7.3/LICENSE
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2021-06-10 06:05:53.000000 whoisit-2.7.3/MANIFEST.in
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    21653 2023-09-06 06:56:26.280486 whoisit-2.7.3/PKG-INFO
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    20802 2022-07-08 03:09:28.000000 whoisit-2.7.3/README.md
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       43 2022-12-06 10:28:45.000000 whoisit-2.7.3/requirements.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       79 2023-09-06 06:56:26.280486 whoisit-2.7.3/setup.cfg
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1359 2023-09-06 06:56:01.000000 whoisit-2.7.3/setup.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-09-06 06:56:26.280486 whoisit-2.7.3/tests/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2021-06-06 06:14:06.000000 whoisit-2.7.3/tests/__init__.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    11786 2022-12-06 10:28:45.000000 whoisit-2.7.3/tests/test_bootstrap.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    21934 2022-12-06 10:28:45.000000 whoisit-2.7.3/tests/test_parser.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     5150 2021-11-18 03:52:35.000000 whoisit-2.7.3/tests/test_query.py
--rw-r--r--   0 meeb      (1000) meeb      (1000)     2070 2023-06-03 08:56:21.000000 whoisit-2.7.3/tests/test_ssl.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-09-06 06:56:26.280486 whoisit-2.7.3/whoisit/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     2359 2023-06-03 08:55:13.000000 whoisit-2.7.3/whoisit/__init__.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    17741 2023-06-03 08:55:54.000000 whoisit-2.7.3/whoisit/bootstrap.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      937 2022-12-06 10:28:45.000000 whoisit-2.7.3/whoisit/errors.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      522 2021-06-08 06:47:34.000000 whoisit-2.7.3/whoisit/logger.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1171 2023-09-06 06:55:37.000000 whoisit-2.7.3/whoisit/overrides.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    15838 2022-12-06 10:28:45.000000 whoisit-2.7.3/whoisit/parser.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     8965 2023-06-03 07:58:57.000000 whoisit-2.7.3/whoisit/query.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     3940 2023-07-10 18:02:01.000000 whoisit-2.7.3/whoisit/utils.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       19 2023-09-06 06:55:55.000000 whoisit-2.7.3/whoisit/version.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-09-06 06:56:26.280486 whoisit-2.7.3/whoisit.egg-info/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    21653 2023-09-06 06:56:26.000000 whoisit-2.7.3/whoisit.egg-info/PKG-INFO
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      489 2023-09-06 06:56:26.000000 whoisit-2.7.3/whoisit.egg-info/SOURCES.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)        1 2023-09-06 06:56:26.000000 whoisit-2.7.3/whoisit.egg-info/dependency_links.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       43 2023-09-06 06:56:26.000000 whoisit-2.7.3/whoisit.egg-info/requires.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2023-09-06 06:56:26.000000 whoisit-2.7.3/whoisit.egg-info/top_level.txt
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-04-20 06:10:52.156591 whoisit-2.7.4/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1528 2021-06-06 06:10:53.000000 whoisit-2.7.4/LICENSE
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2021-06-10 06:05:53.000000 whoisit-2.7.4/MANIFEST.in
+-rw-r--r--   0 meeb      (1000) meeb      (1000)    21721 2024-04-20 06:10:52.156591 whoisit-2.7.4/PKG-INFO
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    20802 2022-07-08 03:09:28.000000 whoisit-2.7.4/README.md
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       43 2022-12-06 10:28:45.000000 whoisit-2.7.4/requirements.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       79 2024-04-20 06:10:52.156591 whoisit-2.7.4/setup.cfg
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1359 2024-04-20 06:08:12.000000 whoisit-2.7.4/setup.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-04-20 06:10:52.152591 whoisit-2.7.4/tests/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2021-06-06 06:14:06.000000 whoisit-2.7.4/tests/__init__.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    11786 2022-12-06 10:28:45.000000 whoisit-2.7.4/tests/test_bootstrap.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    21934 2022-12-06 10:28:45.000000 whoisit-2.7.4/tests/test_parser.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     5150 2021-11-18 03:52:35.000000 whoisit-2.7.4/tests/test_query.py
+-rw-r--r--   0 meeb      (1000) meeb      (1000)     2070 2023-06-03 08:56:21.000000 whoisit-2.7.4/tests/test_ssl.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-04-20 06:10:52.156591 whoisit-2.7.4/whoisit/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     3009 2024-04-20 06:05:08.000000 whoisit-2.7.4/whoisit/__init__.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    17741 2023-06-03 08:55:54.000000 whoisit-2.7.4/whoisit/bootstrap.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      937 2022-12-06 10:28:45.000000 whoisit-2.7.4/whoisit/errors.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      522 2021-06-08 06:47:34.000000 whoisit-2.7.4/whoisit/logger.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1897 2024-03-23 08:51:07.000000 whoisit-2.7.4/whoisit/overrides.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    16104 2024-04-20 06:03:35.000000 whoisit-2.7.4/whoisit/parser.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     8965 2023-06-03 07:58:57.000000 whoisit-2.7.4/whoisit/query.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     3940 2023-07-10 18:02:01.000000 whoisit-2.7.4/whoisit/utils.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       18 2024-04-20 06:08:20.000000 whoisit-2.7.4/whoisit/version.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-04-20 06:10:52.156591 whoisit-2.7.4/whoisit.egg-info/
+-rw-r--r--   0 meeb      (1000) meeb      (1000)    21721 2024-04-20 06:10:52.000000 whoisit-2.7.4/whoisit.egg-info/PKG-INFO
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      489 2024-04-20 06:10:52.000000 whoisit-2.7.4/whoisit.egg-info/SOURCES.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)        1 2024-04-20 06:10:52.000000 whoisit-2.7.4/whoisit.egg-info/dependency_links.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       43 2024-04-20 06:10:52.000000 whoisit-2.7.4/whoisit.egg-info/requires.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2024-04-20 06:10:52.000000 whoisit-2.7.4/whoisit.egg-info/top_level.txt
```

### Comparing `whoisit-2.7.3/LICENSE` & `whoisit-2.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.3/PKG-INFO` & `whoisit-2.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: whoisit
-Version: 2.7.3
+Version: 2.7.4
 Summary: A Python client to RDAP WHOIS-like services for internet resources.
 Home-page: https://github.com/meeb/whoisit
 Author: https://github.com/meeb
 Author-email: meeb@meeb.org
 License: BSD
 Keywords: whoisit,whois,rdap,ip,network,cidr,prefix,domain,asn,autnum,tld,entity,handle,arin,afrinic,apnic,ripe,lacnic
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: python-dateutil
+Requires-Dist: typing-extensions
 
 # whoisit
 
 A Python client to RDAP WHOIS-like services for internet resources (IPs, ASNs, domains,
 etc.). `whoisit` is a simple library that makes requests to the "new" RDAP (Registration
 Data Access Protocol) query services for internet resource information. These services
 started to appear in 2017 and have become more widespread since 2020.
@@ -575,9 +577,7 @@
 $ python3 some-script-that-uses-whoisit.py
 ```
 
 
 # Contributing
 
 All properly formatted and sensible pull requests, issues and comments are welcome.
-
-
```

### Comparing `whoisit-2.7.3/README.md` & `whoisit-2.7.4/README.md`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.3/setup.py` & `whoisit-2.7.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 
-version = '2.7.3'
+version = '2.7.4'
 
 
 with open('README.md', 'rt') as f:
     long_description = f.read()
 
 
 with open('requirements.txt', 'rt') as f:
```

### Comparing `whoisit-2.7.3/tests/test_bootstrap.py` & `whoisit-2.7.4/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.3/tests/test_parser.py` & `whoisit-2.7.4/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.3/tests/test_query.py` & `whoisit-2.7.4/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.3/tests/test_ssl.py` & `whoisit-2.7.4/tests/test_ssl.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.3/whoisit/__init__.py` & `whoisit-2.7.4/whoisit/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,16 +40,32 @@
 
 def domain(domain_name, raw=False, allow_insecure_ssl=False, session=None):
     session = get_session(session, allow_insecure_ssl=allow_insecure_ssl)
     method, url, exact_match = build_query(
         query_type='domain', query_value=domain_name)
     q = Query(session, method, url)
     response = q.request()
-    return response if raw else parse(_bootstrap, 'domain', domain_name, response)
-
+    if raw:
+        return response
+    # Attempt to follow the 'related' or 'registration' links if the TLD has
+    # an upstream RDAP endpoint that may have more information
+    relresponse = None
+    for link in response.get('links', []):
+        rel = link.get('rel', '')
+        if rel in ('related', 'registration'):
+            relhref = link.get('href', '')
+            if relhref:
+                print(f'MAKING SUBREQUEST TO {relhref}')
+                relq = Query(session, method, relhref)
+                relresponse = relq.request()
+                break
+    if relresponse:
+        return parse(_bootstrap, 'domain', domain_name, relresponse)
+    else:
+        return parse(_bootstrap, 'domain', domain_name, response)
 
 def ip(ip_address_or_network, rir=None, raw=False, allow_insecure_ssl=False, session=None):
     session = get_session(session, allow_insecure_ssl=allow_insecure_ssl)
     method, url, exact_match = build_query(
         query_type='ip', query_value=ip_address_or_network, rir=rir)
     q = Query(session, method, url)
     response = q.request()
```

### Comparing `whoisit-2.7.3/whoisit/bootstrap.py` & `whoisit-2.7.4/whoisit/bootstrap.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.3/whoisit/errors.py` & `whoisit-2.7.4/whoisit/errors.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.3/whoisit/logger.py` & `whoisit-2.7.4/whoisit/logger.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.3/whoisit/overrides.py` & `whoisit-2.7.4/whoisit/overrides.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,10 +25,22 @@
         'gov.gl': ['https://rdap.centralnic.com/gov.gl/'],
         'net.gl': ['https://rdap.centralnic.com/net.gl/'],
         'org.gl': ['https://rdap.centralnic.com/org.gl/'],
 
         # 2023-09-05 - .nl has an RDAP endpoint it's just not listed
         'nl': ['https://rdap.sidn.nl/'],
 
+        # 2023-12-13 - the Identity Digital RDAP server appears to support these ccTLDs
+        'ac': ['https://rdap.identitydigital.services/'],
+        'ag': ['https://rdap.identitydigital.services/'],
+        'bz': ['https://rdap.identitydigital.services/'],
+        'io': ['https://rdap.identitydigital.services/'],
+        'lc': ['https://rdap.identitydigital.services/'],
+        'me': ['https://rdap.identitydigital.services/'],
+        'mn': ['https://rdap.identitydigital.services/'],
+        'pr': ['https://rdap.identitydigital.services/'],
+        'sc': ['https://rdap.identitydigital.services/'],
+        'sh': ['https://rdap.identitydigital.services/'],
+        'vc': ['https://rdap.identitydigital.services/'],
     }
 
 }
```

### Comparing `whoisit-2.7.3/whoisit/parser.py` & `whoisit-2.7.4/whoisit/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,14 +242,22 @@
         self.extract_asn_range()
         return self.parsed
 
     def extract_asn_range(self):
         self.parsed['asn_range'] = None
         start_asn_range = self.raw_data.get('startAutnum', 0)
         end_asn_range = self.raw_data.get('endAutnum', 0)
+        try:
+            start_asn_range = int(start_asn_range)
+        except (ValueError, TypeError):
+            start_asn_range = 0
+        try:
+            end_asn_range = int(end_asn_range)
+        except (ValueError, TypeError):
+            end_asn_range = 0
         if start_asn_range > 0 and end_asn_range > 0:
             self.parsed['asn_range'] = [start_asn_range, end_asn_range]
 
 
 class ParseDomain(Parser):
     """
         Additional data extractors for domain objects.
```

### Comparing `whoisit-2.7.3/whoisit/query.py` & `whoisit-2.7.4/whoisit/query.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.3/whoisit/utils.py` & `whoisit-2.7.4/whoisit/utils.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.3/whoisit.egg-info/PKG-INFO` & `whoisit-2.7.4/whoisit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: whoisit
-Version: 2.7.3
+Version: 2.7.4
 Summary: A Python client to RDAP WHOIS-like services for internet resources.
 Home-page: https://github.com/meeb/whoisit
 Author: https://github.com/meeb
 Author-email: meeb@meeb.org
 License: BSD
 Keywords: whoisit,whois,rdap,ip,network,cidr,prefix,domain,asn,autnum,tld,entity,handle,arin,afrinic,apnic,ripe,lacnic
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: python-dateutil
+Requires-Dist: typing-extensions
 
 # whoisit
 
 A Python client to RDAP WHOIS-like services for internet resources (IPs, ASNs, domains,
 etc.). `whoisit` is a simple library that makes requests to the "new" RDAP (Registration
 Data Access Protocol) query services for internet resource information. These services
 started to appear in 2017 and have become more widespread since 2020.
@@ -575,9 +577,7 @@
 $ python3 some-script-that-uses-whoisit.py
 ```
 
 
 # Contributing
 
 All properly formatted and sensible pull requests, issues and comments are welcome.
-
-
```

