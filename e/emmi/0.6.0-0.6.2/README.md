# Comparing `tmp/emmi-0.6.0.tar.gz` & `tmp/emmi-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmi-0.6.0.tar", last modified: Tue Apr  9 13:19:44 2024, max compression
+gzip compressed data, was "emmi-0.6.2.tar", last modified: Sat Apr 20 14:06:32 2024, max compression
```

## Comparing `emmi-0.6.0.tar` & `emmi-0.6.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 13:19:44.149115 emmi-0.6.0/
--rw-r--r--   0 florin    (1000) florin    (1000)      138 2024-03-29 10:47:21.000000 emmi-0.6.0/.gitignore
--rw-r--r--   0 florin    (1000) florin    (1000)     3263 2023-06-06 15:18:43.000000 emmi-0.6.0/.gitlab-ci.yml
--rw-r--r--   0 florin    (1000) florin    (1000)    35147 2022-11-16 13:15:18.000000 emmi-0.6.0/LICENSE
--rw-r--r--   0 florin    (1000) florin    (1000)     2465 2024-04-09 13:19:44.149115 emmi-0.6.0/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)     1055 2024-03-29 10:47:21.000000 emmi-0.6.0/README.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 13:19:44.143115 emmi-0.6.0/doc/
--rw-r--r--   0 florin    (1000) florin    (1000)     9904 2024-03-29 10:47:21.000000 emmi-0.6.0/doc/eda.md
--rw-r--r--   0 florin    (1000) florin    (1000)     2260 2024-03-29 10:47:21.000000 emmi-0.6.0/doc/index.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 13:19:44.144115 emmi-0.6.0/examples/
--rw-r--r--   0 florin    (1000) florin    (1000)       33 2023-06-06 15:18:26.000000 emmi-0.6.0/examples/simple-ioc.json
--rwxr-xr-x   0 florin    (1000) florin    (1000)     1772 2023-06-06 15:18:26.000000 emmi-0.6.0/examples/simple-ioc.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1461 2024-03-29 10:47:21.000000 emmi-0.6.0/pyproject.toml
--rw-r--r--   0 florin    (1000) florin    (1000)      202 2024-04-09 13:19:44.149115 emmi-0.6.0/setup.cfg
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 13:19:44.142115 emmi-0.6.0/src/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 13:19:44.144115 emmi-0.6.0/src/emmi/
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2022-11-18 18:47:06.000000 emmi-0.6.0/src/emmi/__init__.py
--rw-r--r--   0 florin    (1000) florin    (1000)      411 2024-04-09 13:19:44.000000 emmi-0.6.0/src/emmi/_version.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 13:19:44.145115 emmi-0.6.0/src/emmi/api/
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2022-11-30 14:07:54.000000 emmi-0.6.0/src/emmi/api/__init__.py
--rw-r--r--   0 florin    (1000) florin    (1000)    32108 2024-04-09 09:56:30.000000 emmi-0.6.0/src/emmi/api/exports.py
--rw-r--r--   0 florin    (1000) florin    (1000)    10895 2024-04-09 13:17:03.000000 emmi-0.6.0/src/emmi/api/motor.py
--rw-r--r--   0 florin    (1000) florin    (1000)    16743 2024-04-09 09:56:30.000000 emmi-0.6.0/src/emmi/app.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 13:19:44.145115 emmi-0.6.0/src/emmi/ca/
--rwxr-xr-x   0 florin    (1000) florin    (1000)    12064 2024-03-29 10:47:21.000000 emmi-0.6.0/src/emmi/ca/histo.py
--rw-r--r--   0 florin    (1000) florin    (1000)    18872 2024-03-29 10:47:21.000000 emmi-0.6.0/src/emmi/ca/reader.py
--rw-r--r--   0 florin    (1000) florin    (1000)    17122 2024-04-09 13:16:51.000000 emmi-0.6.0/src/emmi/eda.py
--rw-r--r--   0 florin    (1000) florin    (1000)    60843 2024-04-09 09:56:30.000000 emmi-0.6.0/src/emmi/scpi.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 13:19:44.148115 emmi-0.6.0/src/emmi.egg-info/
--rw-r--r--   0 florin    (1000) florin    (1000)     2465 2024-04-09 13:19:44.000000 emmi-0.6.0/src/emmi.egg-info/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)      788 2024-04-09 13:19:44.000000 emmi-0.6.0/src/emmi.egg-info/SOURCES.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        1 2024-04-09 13:19:44.000000 emmi-0.6.0/src/emmi.egg-info/dependency_links.txt
--rw-r--r--   0 florin    (1000) florin    (1000)      155 2024-04-09 13:19:44.000000 emmi-0.6.0/src/emmi.egg-info/requires.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        5 2024-04-09 13:19:44.000000 emmi-0.6.0/src/emmi.egg-info/top_level.txt
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-09 13:19:44.148115 emmi-0.6.0/tests/
--rw-r--r--   0 florin    (1000) florin    (1000)     5431 2023-06-06 15:18:26.000000 emmi-0.6.0/tests/api_exports_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     5158 2023-06-06 15:18:26.000000 emmi-0.6.0/tests/app_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     2342 2023-06-06 15:18:26.000000 emmi-0.6.0/tests/eda_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1370 2024-03-29 10:47:21.000000 emmi-0.6.0/tests/huber_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1821 2024-04-09 13:18:05.000000 emmi-0.6.0/tests/motor_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1987 2024-03-29 10:47:21.000000 emmi-0.6.0/tests/pharos_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)      483 2024-03-29 10:47:21.000000 emmi-0.6.0/tests/pytest_dev.yaml
--rw-r--r--   0 florin    (1000) florin    (1000)     5053 2024-03-29 10:47:21.000000 emmi-0.6.0/tests/scpi_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)      263 2024-03-29 10:47:21.000000 emmi-0.6.0/tests/visa-sim-huber.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      640 2024-03-29 10:47:21.000000 emmi-0.6.0/tests/visa-sim-pharos.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      698 2024-03-29 10:47:21.000000 emmi-0.6.0/tests/visa-sim-sds2k.yml
--rw-r--r--   0 florin    (1000) florin    (1000)     1305 2024-03-29 10:47:21.000000 emmi-0.6.0/tests/visa-sim-sigen.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      507 2024-03-29 10:47:21.000000 emmi-0.6.0/tests/visa-sim.yml
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-20 14:06:32.852094 emmi-0.6.2/
+-rw-r--r--   0 florin    (1000) florin    (1000)      138 2024-03-29 10:47:21.000000 emmi-0.6.2/.gitignore
+-rw-r--r--   0 florin    (1000) florin    (1000)     3263 2023-06-06 15:18:43.000000 emmi-0.6.2/.gitlab-ci.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)    35147 2022-11-16 13:15:18.000000 emmi-0.6.2/LICENSE
+-rw-r--r--   0 florin    (1000) florin    (1000)     2465 2024-04-20 14:06:32.852094 emmi-0.6.2/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)     1055 2024-03-29 10:47:21.000000 emmi-0.6.2/README.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-20 14:06:32.848094 emmi-0.6.2/doc/
+-rw-r--r--   0 florin    (1000) florin    (1000)     9904 2024-03-29 10:47:21.000000 emmi-0.6.2/doc/eda.md
+-rw-r--r--   0 florin    (1000) florin    (1000)     2260 2024-03-29 10:47:21.000000 emmi-0.6.2/doc/index.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-20 14:06:32.848094 emmi-0.6.2/examples/
+-rw-r--r--   0 florin    (1000) florin    (1000)       33 2023-06-06 15:18:26.000000 emmi-0.6.2/examples/simple-ioc.json
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     1772 2023-06-06 15:18:26.000000 emmi-0.6.2/examples/simple-ioc.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1461 2024-03-29 10:47:21.000000 emmi-0.6.2/pyproject.toml
+-rw-r--r--   0 florin    (1000) florin    (1000)      202 2024-04-20 14:06:32.852094 emmi-0.6.2/setup.cfg
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-20 14:06:32.847094 emmi-0.6.2/src/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-20 14:06:32.848094 emmi-0.6.2/src/emmi/
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2022-11-18 18:47:06.000000 emmi-0.6.2/src/emmi/__init__.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      411 2024-04-20 14:06:32.000000 emmi-0.6.2/src/emmi/_version.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-20 14:06:32.849094 emmi-0.6.2/src/emmi/api/
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2022-11-30 14:07:54.000000 emmi-0.6.2/src/emmi/api/__init__.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    30656 2024-04-10 11:31:48.000000 emmi-0.6.2/src/emmi/api/exports.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    12030 2024-04-20 14:06:23.000000 emmi-0.6.2/src/emmi/api/motor.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    17029 2024-04-10 11:24:35.000000 emmi-0.6.2/src/emmi/app.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-20 14:06:32.850094 emmi-0.6.2/src/emmi/ca/
+-rwxr-xr-x   0 florin    (1000) florin    (1000)    12064 2024-03-29 10:47:21.000000 emmi-0.6.2/src/emmi/ca/histo.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    19232 2024-04-20 14:06:23.000000 emmi-0.6.2/src/emmi/ca/reader.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    17099 2024-04-10 12:02:44.000000 emmi-0.6.2/src/emmi/eda.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    60843 2024-04-09 09:56:30.000000 emmi-0.6.2/src/emmi/scpi.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-20 14:06:32.851094 emmi-0.6.2/src/emmi.egg-info/
+-rw-r--r--   0 florin    (1000) florin    (1000)     2465 2024-04-20 14:06:32.000000 emmi-0.6.2/src/emmi.egg-info/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)      788 2024-04-20 14:06:32.000000 emmi-0.6.2/src/emmi.egg-info/SOURCES.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        1 2024-04-20 14:06:32.000000 emmi-0.6.2/src/emmi.egg-info/dependency_links.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)      155 2024-04-20 14:06:32.000000 emmi-0.6.2/src/emmi.egg-info/requires.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        5 2024-04-20 14:06:32.000000 emmi-0.6.2/src/emmi.egg-info/top_level.txt
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-20 14:06:32.851094 emmi-0.6.2/tests/
+-rw-r--r--   0 florin    (1000) florin    (1000)     5431 2023-06-06 15:18:26.000000 emmi-0.6.2/tests/api_exports_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     5158 2023-06-06 15:18:26.000000 emmi-0.6.2/tests/app_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     2342 2023-06-06 15:18:26.000000 emmi-0.6.2/tests/eda_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1370 2024-03-29 10:47:21.000000 emmi-0.6.2/tests/huber_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1821 2024-04-09 13:18:05.000000 emmi-0.6.2/tests/motor_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1987 2024-03-29 10:47:21.000000 emmi-0.6.2/tests/pharos_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      483 2024-03-29 10:47:21.000000 emmi-0.6.2/tests/pytest_dev.yaml
+-rw-r--r--   0 florin    (1000) florin    (1000)     5053 2024-03-29 10:47:21.000000 emmi-0.6.2/tests/scpi_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      263 2024-03-29 10:47:21.000000 emmi-0.6.2/tests/visa-sim-huber.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      640 2024-03-29 10:47:21.000000 emmi-0.6.2/tests/visa-sim-pharos.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      698 2024-03-29 10:47:21.000000 emmi-0.6.2/tests/visa-sim-sds2k.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)     1305 2024-03-29 10:47:21.000000 emmi-0.6.2/tests/visa-sim-sigen.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      507 2024-03-29 10:47:21.000000 emmi-0.6.2/tests/visa-sim.yml
```

### Comparing `emmi-0.6.0/.gitlab-ci.yml` & `emmi-0.6.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `emmi-0.6.0/LICENSE` & `emmi-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `emmi-0.6.0/PKG-INFO` & `emmi-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emmi
-Version: 0.6.0
+Version: 0.6.2
 Summary: A Selection of Tools for EPICS Monday-Morning Integrations
 Author-email: Matthias Rössle <matthias.roessle@helmholtz-berlin.de>, Florin Boariu <florin.pt@rootshell.ro>
 Project-URL: Source Code, https://gitlab.com/codedump2/emmi/
 Project-URL: Bug Tracker, https://gitlab.com/codedump2/emmi/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `emmi-0.6.0/README.md` & `emmi-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `emmi-0.6.0/doc/eda.md` & `emmi-0.6.2/doc/eda.md`

 * *Files identical despite different names*

### Comparing `emmi-0.6.0/doc/index.md` & `emmi-0.6.2/doc/index.md`

 * *Files identical despite different names*

### Comparing `emmi-0.6.0/examples/simple-ioc.py` & `emmi-0.6.2/examples/simple-ioc.py`

 * *Files identical despite different names*

### Comparing `emmi-0.6.0/pyproject.toml` & `emmi-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `emmi-0.6.0/src/emmi/api/exports.py` & `emmi-0.6.2/src/emmi/api/exports.py`

 * *Files 8% similar despite different names*

```diff
@@ -341,15 +341,16 @@
         '''
         
         if not set(kw).issubset(set(self.argnames)):
             raise TypeError("Unknown arguments: %r" % set(kw).difference(self.argnames))
         
         k = ConnectorKinds[kw.get('kind')]
 
-        suffix = kw.get('suffix') or kw.get('name')
+        _s = kw.get('suffix')
+        suffix = _s if _s is not None else kw.get('name')
 
         pv_create_args = k.get('create', {})
         pv_create_args.update(kw.get('create', {}))
         RecordType = k["in"]
         self.pv = RecordType(suffix, **(pv_create_args))
 
         if hasattr(kw.get('access', None), "__call__"):
@@ -416,15 +417,16 @@
         '''
 
         if not set(kw).issubset(set(self.argnames)):
             raise TypeError("Unknown arguments: %r" % set(kw).difference(self.argnames))
         
         k = ConnectorKinds[kw.get('kind')]
 
-        suffix = kw.get('suffix') or kw.get('name')
+        _s = kw.get('suffix')        
+        suffix = _s if _s is not None else kw.get('name')
         
         if hasattr(kw['access'], "__call__"):
             access = kw['access']
         else:
             access = partial(setattr, *(kw['access']))
 
         if  k['from-epics'] is None:
@@ -507,60 +509,33 @@
 
         #print ("Intermediate 1.2: %r" % (kw['access'],))
         
         ad = {}
         ad.update(kw.get('actor', {}))
         ad.setdefault("kind", kw['kind'])
 
-        #if 'access' in ad:
-        #    # Subconnector has its own 'access' information -- we need to use that.
-        #    if isinstance(ad['access'], str):
-        #        # If it's a plain string, we intepret that to be a (sub-)property
-        #        # relative to the base class already specified in kw['access'].
-        #        # If kw['access'] doesn't have anything, we're out of luck anyway,
-        #        # because we don't have access to a base class here.
-        #        ad['access'] = FindAccess(kw['access'], ad['access'])
-        #    elif hasattr(ad['access'], "__len__") \
-        #         and len(ad['access']) == 2 \
-        #         and isinstance(str, ad['access'][1]):
-        #        # ...may be a tuple (obj, "attribute")?
-        #        ad['access'] = FindAccess(*(ad['access']))
-        #    else:
-        #        raise RuntimeError("Unsupported sub-access type %r for property connector")
-        #else:
-        #    # Regular
-        #    ad['access'] = kw['access']
         ad['access'] = self.descend_access(kw['access'], ad.get('access', None))
             
+
+        _s = kw.get('suffix')
         
         ad.setdefault("validator", kw.get('validator', None))
-        ad.setdefault("suffix", (kw.get('suffix') or kw.get('name'))+"VAL")
+        ad.setdefault("suffix", (_s if _s is not None else kw.get('name'))+"VAL")
         self.val = ActorConnector(ioc_dispatcher, **ad)
 
         sd = {}
         sd.update(kw.get('signal', {}))
         sd.setdefault("kind", kw['kind'])
 
-        #if 'access' in sd:
-        #    if isinstance(sd['access'], str):
-        #        sd['access'] = FindAccess(kw['access'], sd['access'])
-        #    elif hasattr(sd['access'], "__len__") \
-        #         and len(sd['access']) == 2 \
-        #         and isinstance(str, sd['access'][1]):
-        #        # ...may be a tuple (obj, "attribute")?
-        #        sd['access'] = FindAccess(*(sd['access']))
-        #    else:
-        #        raise RuntimeError("Unsupported sub-access type %r for property connector")                
-        #else:
         sd['access'] = self.descend_access(kw['access'], sd.get('access', None))
                 
         #print ("Intermediate 1.7: %r" % (sd['access'],))
         
         sd.setdefault("validator", kw.get('validator', None))
-        sd.setdefault("suffix", (kw.get('suffix') or kw.get('name'))+"RBV")
+        sd.setdefault("suffix", (_s if _s is not None else kw.get('name'))+"RBV")
         self.rbv = SignalConnector(ioc_dispatcher, **sd)
 
         logger.info ("Registering property: %s" % (kw.get('suffix') or kw.get('name')))
 
 
     def descend_access(self, top_access, sub_access):
         '''
```

### Comparing `emmi-0.6.0/src/emmi/api/motor.py` & `emmi-0.6.2/src/emmi/api/motor.py`

 * *Files 17% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     FIXME: need to add support for supplementary actions / properties / signals
     (e.g. extend by additional "BUSY" states, or read/write specific properties
     like limits, force probe thresholds etc).
     '''    
 
     def __init__(self, motor_prefix, motor_engine, ioc_dispatcher,
-                 poll_period=0.1, separator="_", style="simple"):
+                 poll_period=0.1, separator="_"):
         '''
         Initializes the IOC variables. Parameters:
         
           - `motor_prefix`: a string to prepend to the motor variables.
         
           - `motor_engine`: the `MotorEngine` object we'll be talking to.
         
@@ -119,15 +119,15 @@
         # VAL/RBV
         self.con_pos = PropertyConnector(ioc_dispatcher,
                                          suffix=motor_prefix+separator,
                                          access=(motor_engine, "position"),
                                          signal={ 'pollPeriod': poll_period },
                                          kind="analog")
 
-        # STATEVAL/RBV
+        # STATE (motor engine)
         self.con_state = SignalConnector(ioc_dispatcher,
                                          suffix=motor_prefix+separator+"STATE",
                                          access=(motor_engine, "state"),
                                          pollPeriod=poll_period,
                                          kind="strings",
                                          validator={ 'values': [
                                              'INIT', 'IDLE', 'STAGING', 'BUSY',
@@ -146,47 +146,14 @@
         self.prefix_separator = separator
 
         # for use with .addBusy()
         self.additional_actions = {}
 
         self.ioc_dispatcher = ioc_dispatcher
 
-        if style == "spec":
-
-            # lots of variables expected by spec but which we don't really serve
-            self.con_constants = [
-                SignalConnector(ioc_dispatcher,
-                                suffix=motor_prefix+separator+suffix,
-                                access=lambda: value,
-                                kind=kind,
-                                pollPeriod=10.0)
-                for suffix,kind,value in [ ("ACCL", "analog", 0),
-                                           ("BDST", "analog", 0),
-                                           ("BVAL", "analog", 0),
-                                           ("VBAS", "analog", 0),
-                                           ("ERES", "analog", 0),
-                                           ("MRES", "analog", 0),
-                                           ("UEIP", "analog", 1),
-                                           ("VELO", "analog", 0)]]
-            #("EGU",  "text", "mm")] ]
-
-            # DMOV - set to 0 when motor begins moving
-            self.con_dmov = SignalConnector(ioc_dispatcher,
-                                            suffix=motor_prefix+separator+"DMOV",
-                                            access=lambda: int(self.engine.state == "IDLE"),
-                                            kind="integer",
-                                            pollPeriod=self.pollPeriod)
-
-            
-            self.con_status = SignalConnector(ioc_dispatcher,
-                                              suffix=motor_prefix+separator+"STATUS",
-                                              access=lambda: 0x02 if self.engine.state == "BUSY" else 0x00,
-                                              kind="integer",
-                                              pollPeriod=self.pollPeriod)
-
 
     def addBusy(self, action_suffix, go, **go_params):
         '''
         Adds an additional motor work trigger with the specified suffix.
         
         Some motors support additional actions in their BUSY phase (e.g.
         relative move, homing action etc). This supports a simple extension
@@ -257,7 +224,76 @@
         self.engine.state = "STOP"
         self.con_stop.pv.set(0)
         
         while self.engine.state != "IDLE":
             await asyncio.sleep(self.pollPeriod)
             
         self.con_val.set(self.engine.position)
+
+
+class DMOVMixin:
+    ''' Implements the DMOV motor suffix (returns 1 while motor is not IDLE).
+    '''
+    def __init__(self):
+        
+        # DMOV - set to 0 when motor begins moving
+        self.con_dmov = SignalConnector(self.ioc_dispatcher,
+                                        suffix=self.motor_prefix+self.prefix_separator+"DMOV",
+                                        access=lambda: int(self.engine.state == "IDLE"),
+                                        kind="integer",
+                                        pollPeriod=self.pollPeriod)
+
+
+class MSTAMixin:
+    ''' Implements a SPEC-like STATUS motor suffix (returns 0x02 bit set while moving).
+
+    EPICS (motor record) actually defines the following bits:
+      1. DIRECTION: last raw direction; (0:Negative, 1:Positive)
+      2. DONE: motion is complete.
+      3. PLUS_LS: plus limit switch has been hit.
+      4. HOMELS: state of the home limit switch.
+      5. Unused
+      6. POSITION: closed-loop position control is enabled.
+      7. SLIP_STALL: Slip/Stall detected (eg. fatal following error)
+      8. HOME: if at home position.
+      9. PRESENT: encoder is present.
+     10. PROBLEM: driver stopped polling, or hardware problem
+     11. MOVING: non-zero velocity present.
+     12. GAIN_SUPPORT: motor supports closed-loop position control.
+     13. COMM_ERR: Controller communication error.
+     14. MINUS_LS: minus limit switch has been hit.
+     15. HOMED: the motor has been homed.
+    '''
+
+    def __init__(self):
+        
+        suffix=self.motor_prefix+self.separator+"MSTA"
+        
+        status_lambda = lambda: 0x02 if self.engine.state == "BUSY" else 0x00
+        
+        self.con_status = SignalConnector(self.ioc_dispatcher,
+                                          suffix=suffix,
+                                          access=status_lambda,
+                                          kind="integer",
+                                          pollPeriod=self.pollPeriod)
+
+class SpecMixin:
+    ''' Adds a number of nonsensical fields to keep Spec happy '''
+
+    def __init__(self):
+        
+        # lots of variables expected by spec but which we don't really serve
+        self.con_constants = [
+            SignalConnector(self.ioc_dispatcher,
+                            suffix=self.motor_prefix+self.separator_suffix+s,
+                            access=lambda: value,
+                            kind=kind,
+                            pollPeriod=10.0)
+            for s,kind,value in [ ("ACCL", "analog", 0),
+                                  ("BDST", "analog", 0),
+                                  ("BVAL", "analog", 0),
+                                  ("VBAS", "analog", 0),
+                                  ("ERES", "analog", 0),
+                                  ("MRES", "analog", 0),
+                                  ("UEIP", "analog", 1),
+                                  ("VELO", "analog", 0)]]
+        #("EGU",  "text", "mm")] ]
```

### Comparing `emmi-0.6.0/src/emmi/app.py` & `emmi-0.6.2/src/emmi/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 #!/usr/bin/python3
 
 import asyncio, time, logging
 import logging
+logger = logging.getLogger(__name__)
 
 from os import environ
 
 from emmi.api.exports import ExportObjectFromDict
 
+from softioc import softioc, builder, asyncio_dispatcher
+
 '''
 Base modules for easier development of EPICS
 '''
 
 def cfgFromFlat(flatCfg, prefix='', splitChar='_'):
     '''
     Returns a (possibly nested) configuration dictionary from a flat
@@ -282,14 +285,19 @@
             to be loaded in additio to `cfg`, and which may not yet be available
             at the point at which your `IocApplication` is being defined.
         '''
         
         self.conf = cfg or dict({})
 
         if prefix is not None:
+            # pythonSoftIOC will add a ':' by its own. Meanwhile, we're trying
+            # to use prefix _exactly_ as specified (for later compatibility with
+            # caproto, for instance).
+            if prefix[-1] == ':':
+                prefix = prefix[:-1:]            
             self.conf.setdefault('epics', {}).setdefault('prefix', prefix)
 
         if setupIoc:
             self.setupIoc()
                  
 
     def addNestedConfig(self, cfg):
@@ -328,19 +336,16 @@
             self.conf.setdefault('epics', {})['prefix'] = prefix
 
         # Set some defaults if they're not specified in cfg.epics
         self.conf.setdefault('epics', {}).setdefault('heartbeat', heartbeat)
         self.conf.setdefault('epics', {}).setdefault('killSwitch', killSwitch)
 
         self.epicsPrefix = self.conf['epics']['prefix']
-        logging.info("Using EPICS device prefix: %s" % self.epicsPrefix)
+        logger.debug("Using EPICS device prefix: %s" % self.epicsPrefix)
         
-        # the epics part
-        from softioc import softioc, builder, asyncio_dispatcher
-
         self.softioc = softioc
         self.iocBuilder = builder
         self.iocDispatch = asyncio_dispatcher.AsyncioDispatcher()
         self.iocBuilder.SetDeviceName(self.epicsPrefix)
 
         # the device property part
         self.pv = {}
```

### Comparing `emmi-0.6.0/src/emmi/ca/histo.py` & `emmi-0.6.2/src/emmi/ca/histo.py`

 * *Files identical despite different names*

### Comparing `emmi-0.6.0/src/emmi/ca/reader.py` & `emmi-0.6.2/src/emmi/ca/reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import asyncio, time, logging
 
 from caproto.sync import client as ca_client
 from caproto.asyncio.client import Context
 from caproto import CaprotoTimeoutError
 import numpy as np
 
+import copy
+
 from xarray import DataArray
 
 class PvRetry(RuntimeError):
     '''
     Raised by GuidedPvReader when the PVs are not yet ready / guide does
     not yet signal readiness for signal readout.
     '''
@@ -37,17 +39,15 @@
         Args:
         
             pv: A single PV, or a list of PVs, to read out. If not
               specified here, it can be specified later.
         
             guides: A dicitonary of guide variable(s) and their respective
               value to use. The `pv` values will be acquired on the first occasion
-              when *all* of the guides' values have changed *to* the value specified    ctx = Context()
-
-
+              when *all* of the guides' values have changed *to* the value specified
               in the dictionary. If the dictionary value is a callable, it will be
               called with the current (i.e. new) guide values as its sole
               parameters and the `pv` value will be obtained the first time the
               return value changes to `True`.
 
             prefix: If specified, it will be prepended to all of the
               PVs' and guides' EPICS names.
@@ -116,23 +116,21 @@
             # If we have an array and it ends on _SIGNAL, we also try to
             # load _OFFSET and _DELTA for intrinsic scaling information
             o_name = pvName.replace("_SIGNAL", "_OFFSET")
             d_name = pvName.replace("_SIGNAL", "_DELTA")
 
             if o_name in others:
                 offs = self.extract_data(others.get(o_name, 0))
-                del others[o_name]
-                #print("Removed:", o_name)
+                #del others[o_name]
             else:
                 offs = 0
 
             if d_name in others:
                 dlta = self.extract_data(others.get(d_name, 1))
-                del others[d_name]
-                #print("Removed:", d_name)
+                #del others[d_name]
             else:
                 dlta = 1
                 
             axis = offs+np.array(range(len(response.data)))*dlta
                 
             return DataArray(data=response.data, dims=["x"], coords=[axis])
 
@@ -205,14 +203,15 @@
         super().__init__(*args, **kwargs)
         self.ctx = ctx
 
         self.data_pvs = None        
         self.guide_pvs = None
         self.subscribe = subscribe
         self.incoming_hooks = []
+        self.incoming_lock = asyncio.Lock()
 
 
     def subscribe_incoming(self, proc):
         ''' Registers a hook for processing incoming data.
         The hook will receive a dictionary with full PV
         name(s) as keys, and data as values.
         '''
@@ -271,15 +270,15 @@
         # Also important to note: keeping this accurate for _all_ guides
         # at once is difficult when more than one guide is involved (values
         # will change with a slight delay). Hence the policy: once a guide
         # is considered triggered, it _stays_ triggered for as long as
         # its value doesn't chance, or data isn't read.
         self.guide_trigger = {k:False for k in self.guides.keys()}
 
-        self._incoming_data = {k:None for k in self.pv}
+        self._incoming_data = {f'{self.prefix}{k}':None for k in self.pv}
 
 
     async def wait_for_guides(self, PVs, timeout=-1):
         ''' Waits for the internal list of PVs '''
         guides = await asyncio.gather(*[v.read() for v in PVs ])
         for (k,v),data in zip(self.guides.items(),guides):
             self._guide_changed(None,data,pv_name=k)
@@ -332,21 +331,30 @@
     def _get_incoming(self):
         ''' Returns the currently incoming data (from subscriptions)
         and clears everything for the next run.
         '''
         
         for k in self.guide_trigger:
             self.guide_trigger[k] = False
-            
-        data = { k:self.extract_data(v, k, others=self._incoming_data) \
-                 for k,v in self._incoming_data.items() if v is not None}
+
+        # need to work on a copy here because _incoming_data might change
+        # while we're waiting for new incoming data.
+        tmp = self._incoming_data
+        #tmp.update(self._incoming_data)
+        #print(f'tmp: {len(tmp)}, {[k for k in tmp.keys()]}')
+
+        try:
+            data = { k:self.extract_data(v, k, others=tmp) \
+                     for k,v in tmp.items() if v is not None }
+            return data            
+        except RuntimeError as e:
+            raise
+            #print(f'tmp now: {len(tmp)}, {[k for k in tmp.keys()]}')
 
         # FIXME: should we clear incoming data, too?...
-        
-        return data
 
     
     async def wait_for_incoming(self):
         ''' Waits for incoming data -- this is similar to .value(),
         only this uses the subscription mechanism.
         '''
         await self.wait_for_guides(self.guide_pvs)
@@ -469,15 +477,15 @@
 
         if self.subscribe:
             for d in self.data_pvs:
                 logging.info(f'Subscribing to data: {d.name}')
                 self.data_subscriptions[d.name] = d.subscribe()
                 self.data_subscriptions[d.name].add_callback(self._data_changed)
 
-        self._incoming_data = {k:None for k in self.pv_names}
+        self._incoming_data = {f'{self.prefix}{k}':None for k in self.pv_names}
         
 
     def _data_changed(self, sub=None, response=None, name=None):
         ''' Called when new data arrives. '''
 
         pv_name = sub.pv.name if sub is not None else name   
         #logger.debug(f'New data for {pv_name}: {response}')
```

### Comparing `emmi-0.6.0/src/emmi/eda.py` & `emmi-0.6.2/src/emmi/eda.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,18 +202,18 @@
         return "IDLE"
 
 
     # BUSY state: trigger busy action, stay here while action not done
     def state_enter_STAGING(self, state):
         
         if self.__scheduled_stop: # STOP trumps everything
-            logger.info(f'STAGING: {self.__scheduled_go[0]} requested, but also have a stop request pending')            
+            logger.debug(f'STAGING: {self.__scheduled_go[0]} requested, but also have a stop request pending')
             return "STOP"
         
-        logger.info(f'STAGING: {self.__scheduled_go[0]}')
+        logger.debug(f'STAGING: {self.__scheduled_go[0]}')
         self.__scheduled_go[1]()
         return state
 
     def state_STAGING(self, state):
         if self.__scheduled_go[2]() == True:
             return "BUSY"
 
@@ -224,26 +224,26 @@
             return "STOP"
         
         if self.__scheduled_stop is not None:
             return "STOP"
         
         if self.__scheduled_go[2]() == False:
             return "STOP"
-    
+
 
     # IDLE state: stay here until there is work scheduled.
     def state_IDLE(self, state):
         
         if len(self.errors) > 0:
             logger.debug(f'Have {len(self.errors)}, STOP-ing motor')
             return "STOP"
         
         if self.__scheduled_go is not None:
             self.__business = self.__scheduled_go[0] or "(default)"
-            logger.info(f'Going BUSY, business {self.__business}')
+            logger.debug(f'Going BUSY, business {self.__business}')
             return 'STAGING'
 
 
     def state_ERROR(self, state):
         '''
         The only way we can leave ERROR is by clearing/going to IDLE
         '''
@@ -266,15 +266,15 @@
         s_proc_name = state if not state.startswith("BUSY.") else state[:4]
         s_proc = getattr(self, f'state_{s_proc_name}')
 
         #print(f"State run: {self.__old_state} {state}")
 
         # If we just entered the current state, maybe there's a dedicated state_enter_{...}
         if state != self.__old_state:
-            logger.info ("State: %s -> %s" % (self.__old_state, state))
+            logger.debug ("State: %s -> %s" % (self.__old_state, state))
             try:
                 s_proc = getattr(self, f'state_enter_{state}')
             except AttributeError:
                 pass
 
         new_state = s_proc(state)
             
@@ -291,15 +291,15 @@
         Async function to run the Motor Engine
         '''
         if self.__state == "FAIL":
             raise RuntimeError("Attempted to start a motor engine in a failed state")
 
         while (self.__state not in [ "FAIL" ]) or (not stop_on_fail):
             try:
-                self.state_proc(self.__state)
+                self.state_proc()
                 await asyncio.sleep(period)
             except Exception as e:
                 logger.error(f'Motor engine failed: {str(e)}')
                 self.__state == "FAIL"
 
         logger.error("Motor engine in FAIL state")
 
@@ -521,13 +521,13 @@
 
     async def run(self, period=0.1):
         while self.__do_run:
             tstart = time.time()
             current_state = self.__state
             new_state = self.state_workers[current_state]()
             if new_state != current_state:
-                logger.info("State: %r -> %r" % (current_state, new_state))
+                logger.debug("State: %r -> %r" % (current_state, new_state))
                 self.__state = new_state
                 self.state_entries[new_state]()
             tdiff = time.time()-tstart
             await asyncio.sleep(tdiff)
```

### Comparing `emmi-0.6.0/src/emmi/scpi.py` & `emmi-0.6.2/src/emmi/scpi.py`

 * *Files identical despite different names*

### Comparing `emmi-0.6.0/src/emmi.egg-info/PKG-INFO` & `emmi-0.6.2/src/emmi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emmi
-Version: 0.6.0
+Version: 0.6.2
 Summary: A Selection of Tools for EPICS Monday-Morning Integrations
 Author-email: Matthias Rössle <matthias.roessle@helmholtz-berlin.de>, Florin Boariu <florin.pt@rootshell.ro>
 Project-URL: Source Code, https://gitlab.com/codedump2/emmi/
 Project-URL: Bug Tracker, https://gitlab.com/codedump2/emmi/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `emmi-0.6.0/src/emmi.egg-info/SOURCES.txt` & `emmi-0.6.2/src/emmi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emmi-0.6.0/tests/api_exports_test.py` & `emmi-0.6.2/tests/api_exports_test.py`

 * *Files identical despite different names*

### Comparing `emmi-0.6.0/tests/app_test.py` & `emmi-0.6.2/tests/app_test.py`

 * *Files identical despite different names*

### Comparing `emmi-0.6.0/tests/eda_test.py` & `emmi-0.6.2/tests/eda_test.py`

 * *Files identical despite different names*

### Comparing `emmi-0.6.0/tests/huber_test.py` & `emmi-0.6.2/tests/huber_test.py`

 * *Files identical despite different names*

### Comparing `emmi-0.6.0/tests/motor_test.py` & `emmi-0.6.2/tests/motor_test.py`

 * *Files identical despite different names*

### Comparing `emmi-0.6.0/tests/pharos_test.py` & `emmi-0.6.2/tests/pharos_test.py`

 * *Files identical despite different names*

### Comparing `emmi-0.6.0/tests/scpi_test.py` & `emmi-0.6.2/tests/scpi_test.py`

 * *Files identical despite different names*

### Comparing `emmi-0.6.0/tests/visa-sim-pharos.yml` & `emmi-0.6.2/tests/visa-sim-pharos.yml`

 * *Files identical despite different names*

### Comparing `emmi-0.6.0/tests/visa-sim-sds2k.yml` & `emmi-0.6.2/tests/visa-sim-sds2k.yml`

 * *Files identical despite different names*

### Comparing `emmi-0.6.0/tests/visa-sim-sigen.yml` & `emmi-0.6.2/tests/visa-sim-sigen.yml`

 * *Files identical despite different names*

