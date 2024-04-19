# Comparing `tmp/smallneuron-1.0.1.tar.gz` & `tmp/smallneuron-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smallneuron-1.0.1.tar", last modified: Wed Apr 17 20:54:50 2024, max compression
+gzip compressed data, was "smallneuron-1.0.2.tar", last modified: Fri Apr 19 14:50:25 2024, max compression
```

## Comparing `smallneuron-1.0.1.tar` & `smallneuron-1.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-17 20:54:50.663550 smallneuron-1.0.1/
--rw-rw-r--   0 andres    (1000) andres    (1000)      441 2024-02-20 00:54:30.000000 smallneuron-1.0.1/.gitignore
--rw-rw-r--   0 andres    (1000) andres    (1000)     1074 2024-02-18 18:56:34.000000 smallneuron-1.0.1/LICENSE
--rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-04-17 20:54:50.663550 smallneuron-1.0.1/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      753 2024-04-14 21:53:34.000000 smallneuron-1.0.1/README.md
--rw-rw-r--   0 andres    (1000) andres    (1000)     3645 2024-04-14 20:50:42.000000 smallneuron-1.0.1/example.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      655 2024-04-17 20:53:10.000000 smallneuron-1.0.1/pyproject.toml
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2024-04-17 20:54:50.663550 smallneuron-1.0.1/setup.cfg
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-17 20:54:50.659550 smallneuron-1.0.1/src/
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-17 20:54:50.663550 smallneuron-1.0.1/src/smallneuron/
--rw-rw-r--   0 andres    (1000) andres    (1000)      242 2024-02-18 18:56:34.000000 smallneuron-1.0.1/src/smallneuron/__init__.py
--rwxrwxr-x   0 andres    (1000) andres    (1000)      231 2024-02-18 18:56:34.000000 smallneuron-1.0.1/src/smallneuron/build
--rw-rw-r--   0 andres    (1000) andres    (1000)    21308 2024-02-18 18:56:34.000000 smallneuron-1.0.1/src/smallneuron/gpio_h3.c
--rw-rw-r--   0 andres    (1000) andres    (1000)     7411 2024-02-18 18:56:34.000000 smallneuron-1.0.1/src/smallneuron/gpio_h3.h
--rwxrwxr-x   0 andres    (1000) andres    (1000)    26760 2024-02-18 18:56:34.000000 smallneuron-1.0.1/src/smallneuron/gpio_h3.so
--rw-rw-r--   0 andres    (1000) andres    (1000)     1388 2024-04-17 20:53:40.000000 smallneuron-1.0.1/src/smallneuron/logger.py
--rw-rw-r--   0 andres    (1000) andres    (1000)    13776 2024-04-14 22:54:22.000000 smallneuron-1.0.1/src/smallneuron/smallneuron.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1066 2024-04-14 22:54:22.000000 smallneuron-1.0.1/src/smallneuron/sndummy.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1472 2024-04-14 22:44:26.000000 smallneuron-1.0.1/src/smallneuron/sngpio.py
--rwxrwxr-x   0 andres    (1000) andres    (1000)     4087 2024-04-14 22:54:22.000000 smallneuron-1.0.1/src/smallneuron/snhttp.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     3011 2024-04-14 22:54:22.000000 smallneuron-1.0.1/src/smallneuron/sninput.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     2350 2024-04-14 22:54:22.000000 smallneuron-1.0.1/src/smallneuron/snmqtt.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     2555 2024-04-14 22:54:22.000000 smallneuron-1.0.1/src/smallneuron/snserial.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      985 2024-04-14 22:54:22.000000 smallneuron-1.0.1/src/smallneuron/sntimer.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-17 20:54:50.663550 smallneuron-1.0.1/src/smallneuron.egg-info/
--rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-04-17 20:54:50.000000 smallneuron-1.0.1/src/smallneuron.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      775 2024-04-17 20:54:50.000000 smallneuron-1.0.1/src/smallneuron.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-04-17 20:54:50.000000 smallneuron-1.0.1/src/smallneuron.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-04-17 20:54:50.000000 smallneuron-1.0.1/src/smallneuron.egg-info/top_level.txt
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-17 20:54:50.663550 smallneuron-1.0.1/src/smallneuron_pelainux.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1062 2024-02-18 18:56:34.000000 smallneuron-1.0.1/src/smallneuron_pelainux.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      496 2024-02-18 18:56:34.000000 smallneuron-1.0.1/src/smallneuron_pelainux.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-02-18 18:56:34.000000 smallneuron-1.0.1/src/smallneuron_pelainux.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-02-18 18:56:34.000000 smallneuron-1.0.1/src/smallneuron_pelainux.egg-info/top_level.txt
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-19 14:50:25.234319 smallneuron-1.0.2/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      441 2024-02-20 00:54:30.000000 smallneuron-1.0.2/.gitignore
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1074 2024-02-18 18:56:34.000000 smallneuron-1.0.2/LICENSE
+-rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-04-19 14:50:25.234319 smallneuron-1.0.2/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      753 2024-04-14 21:53:34.000000 smallneuron-1.0.2/README.md
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3645 2024-04-14 20:50:42.000000 smallneuron-1.0.2/example.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      655 2024-04-19 14:49:12.000000 smallneuron-1.0.2/pyproject.toml
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2024-04-19 14:50:25.234319 smallneuron-1.0.2/setup.cfg
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-19 14:50:25.230318 smallneuron-1.0.2/src/
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-19 14:50:25.234319 smallneuron-1.0.2/src/smallneuron/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      242 2024-02-18 18:56:34.000000 smallneuron-1.0.2/src/smallneuron/__init__.py
+-rwxrwxr-x   0 andres    (1000) andres    (1000)      231 2024-02-18 18:56:34.000000 smallneuron-1.0.2/src/smallneuron/build
+-rw-rw-r--   0 andres    (1000) andres    (1000)    21308 2024-02-18 18:56:34.000000 smallneuron-1.0.2/src/smallneuron/gpio_h3.c
+-rw-rw-r--   0 andres    (1000) andres    (1000)     7411 2024-02-18 18:56:34.000000 smallneuron-1.0.2/src/smallneuron/gpio_h3.h
+-rwxrwxr-x   0 andres    (1000) andres    (1000)    26760 2024-02-18 18:56:34.000000 smallneuron-1.0.2/src/smallneuron/gpio_h3.so
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1388 2024-04-17 20:53:40.000000 smallneuron-1.0.2/src/smallneuron/logger.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)    13900 2024-04-19 14:49:12.000000 smallneuron-1.0.2/src/smallneuron/smallneuron.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1066 2024-04-14 22:54:22.000000 smallneuron-1.0.2/src/smallneuron/sndummy.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1472 2024-04-14 22:44:26.000000 smallneuron-1.0.2/src/smallneuron/sngpio.py
+-rwxrwxr-x   0 andres    (1000) andres    (1000)     4087 2024-04-14 22:54:22.000000 smallneuron-1.0.2/src/smallneuron/snhttp.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3011 2024-04-14 22:54:22.000000 smallneuron-1.0.2/src/smallneuron/sninput.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     2350 2024-04-14 22:54:22.000000 smallneuron-1.0.2/src/smallneuron/snmqtt.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     2555 2024-04-14 22:54:22.000000 smallneuron-1.0.2/src/smallneuron/snserial.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      985 2024-04-14 22:54:22.000000 smallneuron-1.0.2/src/smallneuron/sntimer.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-19 14:50:25.234319 smallneuron-1.0.2/src/smallneuron.egg-info/
+-rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-04-19 14:50:25.000000 smallneuron-1.0.2/src/smallneuron.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      775 2024-04-19 14:50:25.000000 smallneuron-1.0.2/src/smallneuron.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-04-19 14:50:25.000000 smallneuron-1.0.2/src/smallneuron.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-04-19 14:50:25.000000 smallneuron-1.0.2/src/smallneuron.egg-info/top_level.txt
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-19 14:50:25.234319 smallneuron-1.0.2/src/smallneuron_pelainux.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1062 2024-02-18 18:56:34.000000 smallneuron-1.0.2/src/smallneuron_pelainux.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      496 2024-02-18 18:56:34.000000 smallneuron-1.0.2/src/smallneuron_pelainux.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-02-18 18:56:34.000000 smallneuron-1.0.2/src/smallneuron_pelainux.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-02-18 18:56:34.000000 smallneuron-1.0.2/src/smallneuron_pelainux.egg-info/top_level.txt
```

### Comparing `smallneuron-1.0.1/LICENSE` & `smallneuron-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smallneuron-1.0.1/PKG-INFO` & `smallneuron-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smallneuron
-Version: 1.0.1
+Version: 1.0.2
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smallneuron-1.0.1/README.md` & `smallneuron-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `smallneuron-1.0.1/example.py` & `smallneuron-1.0.2/example.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.0.1/pyproject.toml` & `smallneuron-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 
 [project]
 name = "smallneuron"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Andres Artigas", email="andres@artigas.cl" },
 ]
 description = "Small Neuron Workflow"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `smallneuron-1.0.1/src/smallneuron/gpio_h3.c` & `smallneuron-1.0.2/src/smallneuron/gpio_h3.c`

 * *Files identical despite different names*

### Comparing `smallneuron-1.0.1/src/smallneuron/gpio_h3.h` & `smallneuron-1.0.2/src/smallneuron/gpio_h3.h`

 * *Files identical despite different names*

### Comparing `smallneuron-1.0.1/src/smallneuron/gpio_h3.so` & `smallneuron-1.0.2/src/smallneuron/gpio_h3.so`

 * *Files identical despite different names*

### Comparing `smallneuron-1.0.1/src/smallneuron/logger.py` & `smallneuron-1.0.2/src/smallneuron/logger.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.0.1/src/smallneuron/smallneuron.py` & `smallneuron-1.0.2/src/smallneuron/smallneuron.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,46 +305,48 @@
                 self.thread=threading.Thread(target=SnWatcher._check, args=(self,[bridge,bridge_args,mode, period]))
                 log.debug("SnWatcher.run Thread to start")
                 self.thread.start()
                 log.debug("SnWatcher.run Thread to started")
             except Exception as e:
                 log.error(e)
                 log.error(traceback.format_exc())
-                self.em.putEvent("panic", str(e))
-                exit(1)
-                
+               
             log.debug("SnWatcher.run done")
             return True
         log.debug("SnWatcher.run fail")
         return False
 
     def _check(self, args):
         log.debug("SnWatcher._check loop start",args)
-        [bridge,args,mode, period] = args
-        while not self.stop:
-            resp=bridge.check(**args)
+        try:
+            [bridge,args,mode, period] = args
+            while not self.stop:
+                resp=bridge.check(**args)
 
-            # Si la respuesta no es un dict
-            # creamos uno con la respuesta como data
-            if type(resp) != dict:
-                data=resp
-                resp={"data":data}
+                # Si la respuesta no es un dict
+                # creamos uno con la respuesta como data
+                if type(resp) != dict:
+                    data=resp
+                    resp={"data":data}
 
-            if self.event_pattern == None or re.search(self.event_pattern, resp["data"]) != None:
-                self.em.putEvent(self.event, dict(self.event_args,**resp))
-                log.info("SnWatcher trigger", self.event_args)
-                if mode=="match":
-                    log.debug("SnWatcher._check loop exit, match")
-                    return
+                if self.event_pattern == None or re.search(self.event_pattern, resp["data"]) != None:
+                    self.em.putEvent(self.event, dict(self.event_args,**resp))
+                    log.info("SnWatcher trigger", self.event_args)
+                    if mode=="match":
+                        log.debug("SnWatcher._check loop exit, match")
+                        return
 
-            if mode=="noloop" :
-                log.debug("SnWatcher._check loop exit, noloop")
-                return
-                
-            # default mode is loop 
-            sleep(period)
-        log.debug("SnWatcher._check loop exit, stop")
+                if mode=="noloop" :
+                    log.debug("SnWatcher._check loop exit, noloop")
+                    return
+                    
+                # default mode is loop 
+                sleep(period)
+            log.debug("SnWatcher._check loop exit, stop")
+        except Exception as e:
+            log.error(e)
+            log.error(traceback.format_exc())
 
     def stop(self):
         self.stop=True
         self.thread.join()
         self.thread=None
```

### Comparing `smallneuron-1.0.1/src/smallneuron/sndummy.py` & `smallneuron-1.0.2/src/smallneuron/sndummy.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.0.1/src/smallneuron/sngpio.py` & `smallneuron-1.0.2/src/smallneuron/sngpio.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.0.1/src/smallneuron/snhttp.py` & `smallneuron-1.0.2/src/smallneuron/snhttp.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.0.1/src/smallneuron/sninput.py` & `smallneuron-1.0.2/src/smallneuron/sninput.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.0.1/src/smallneuron/snmqtt.py` & `smallneuron-1.0.2/src/smallneuron/snmqtt.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.0.1/src/smallneuron/snserial.py` & `smallneuron-1.0.2/src/smallneuron/snserial.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.0.1/src/smallneuron/sntimer.py` & `smallneuron-1.0.2/src/smallneuron/sntimer.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.0.1/src/smallneuron.egg-info/PKG-INFO` & `smallneuron-1.0.2/src/smallneuron.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smallneuron
-Version: 1.0.1
+Version: 1.0.2
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smallneuron-1.0.1/src/smallneuron.egg-info/SOURCES.txt` & `smallneuron-1.0.2/src/smallneuron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smallneuron-1.0.1/src/smallneuron_pelainux.egg-info/PKG-INFO` & `smallneuron-1.0.2/src/smallneuron_pelainux.egg-info/PKG-INFO`

 * *Files identical despite different names*

