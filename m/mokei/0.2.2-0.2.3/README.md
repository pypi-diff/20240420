# Comparing `tmp/mokei-0.2.2.tar.gz` & `tmp/mokei-0.2.3.tar.gz`

## Comparing `mokei-0.2.2.tar` & `mokei-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 mokei-0.2.2/src/mokei/__init__.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 mokei-0.2.2/src/mokei/client.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 mokei-0.2.2/src/mokei/config.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 mokei-0.2.2/src/mokei/datatypes.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mokei-0.2.2/src/mokei/exceptions.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 mokei-0.2.2/src/mokei/logging.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 mokei-0.2.2/src/mokei/middlewares.py
--rw-r--r--   0        0        0     9965 2020-02-02 00:00:00.000000 mokei-0.2.2/src/mokei/mokei.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mokei-0.2.2/src/mokei/request.py
--rw-r--r--   0        0        0     7995 2020-02-02 00:00:00.000000 mokei-0.2.2/src/mokei/websocket.py
--rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 mokei-0.2.2/src/mokei/wsclient.py
--rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 mokei-0.2.2/src/mokei/js/mokei.js
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mokei-0.2.2/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 mokei-0.2.2/LICENSE
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 mokei-0.2.2/README.md
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 mokei-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 mokei-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 mokei-0.2.3/src/mokei/__init__.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 mokei-0.2.3/src/mokei/client.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 mokei-0.2.3/src/mokei/config.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 mokei-0.2.3/src/mokei/datatypes.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mokei-0.2.3/src/mokei/exceptions.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 mokei-0.2.3/src/mokei/logging.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 mokei-0.2.3/src/mokei/middlewares.py
+-rw-r--r--   0        0        0     9965 2020-02-02 00:00:00.000000 mokei-0.2.3/src/mokei/mokei.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mokei-0.2.3/src/mokei/request.py
+-rw-r--r--   0        0        0     7995 2020-02-02 00:00:00.000000 mokei-0.2.3/src/mokei/websocket.py
+-rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 mokei-0.2.3/src/mokei/wsclient.py
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 mokei-0.2.3/src/mokei/js/mokei.js
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mokei-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 mokei-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 mokei-0.2.3/README.md
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 mokei-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 mokei-0.2.3/PKG-INFO
```

### Comparing `mokei-0.2.2/src/mokei/client.py` & `mokei-0.2.3/src/mokei/client.py`

 * *Files identical despite different names*

### Comparing `mokei-0.2.2/src/mokei/config.py` & `mokei-0.2.3/src/mokei/config.py`

 * *Files identical despite different names*

### Comparing `mokei-0.2.2/src/mokei/logging.py` & `mokei-0.2.3/src/mokei/logging.py`

 * *Files identical despite different names*

### Comparing `mokei-0.2.2/src/mokei/mokei.py` & `mokei-0.2.3/src/mokei/mokei.py`

 * *Files identical despite different names*

### Comparing `mokei-0.2.2/src/mokei/websocket.py` & `mokei-0.2.3/src/mokei/websocket.py`

 * *Files identical despite different names*

### Comparing `mokei-0.2.2/src/mokei/wsclient.py` & `mokei-0.2.3/src/mokei/wsclient.py`

 * *Files identical despite different names*

### Comparing `mokei-0.2.2/src/mokei/js/mokei.js` & `mokei-0.2.3/src/mokei/js/mokei.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,9 @@
 /**
+ * Version 0.2.3
  * Websocket handler class for use with Python Mokei backend.
  *
  * Preferred usage is to instantiate from mokeiWebsocketExchange to avoid duplicates.
  *
  * const ws = mokeiWebsocketExchange.getWebsocket('wss://some.url.com/ws');
  * ws.on('eventName', (data) => console.log(data));  // register callback for event
  * ws.ontext((text) => console.log(text));  // register callback for text
@@ -20,14 +21,15 @@
 export class MokeiWebSocket {
     /**
      * Websocket handler class for use with Python Mokei backend.
      * @param url - starts with ws:// or wss://
      */
     constructor(url) {
         this.url = url;
+        this._connectCalled = false;
         this._onconnect = [];
         this._ondisconnect = [];
         this._ontext = [];
         this._onbinary = [];
         this._onevent = {};
         this.connected = false;
         this._messages = [];
@@ -102,31 +104,40 @@
 
     connect() {
         /**
          * Must be called once to create and connect the websocket.
          * Event callbacks may be registered before or after connect() is called,
          * but some events may be missed if registering after calling connect()
          */
-        if (this._ws !== null) {
-            return;
+        if (!this._connectCalled) {
+            this._connectCalled = true;
+            this._connect();
         }
+    }
+
+    _connect() {
+        /**
+         * Internal method to handle actually creating and connecting to the websocket
+         * This is called only once by this.connect (and not called on subsequent calls to this.connect)
+         * This is also called again when a disconnect occurs, after a given back-off
+         */
         this._ws = new WebSocket(this.url);
         this._ws.onopen = () => {
             this.connected = true;
             this._backoff = this.defaultBackoff;
             this._sendAll();
             this._onconnect.forEach(handler => handler());
         }
         this._ws.onmessage = ((event) => this._handleMessage(event.data));
         this._ws.onclose = () => {
             if (this.connected) {
                 this._ondisconnect.forEach(handler => handler());
             }
             this.connected = false;
-            setTimeout(this.connect.bind(this), this._backoff);
+            setTimeout(this._connect.bind(this), this._backoff);
             this._backoff = Math.min(this._backoff * 2 + Math.random() * 1000, this.maxBackoff);
         }
     }
 }
 
 class MokeiSocketExchange {
     constructor() {
```

### Comparing `mokei-0.2.2/LICENSE` & `mokei-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mokei-0.2.2/README.md` & `mokei-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `mokei-0.2.2/pyproject.toml` & `mokei-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mokei"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="deuxglaces", email="dev@deuxglaces.com" },
 ]
 description = "A simple asynchronous Python web framework built on aiohttp."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `mokei-0.2.2/PKG-INFO` & `mokei-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mokei
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple asynchronous Python web framework built on aiohttp.
 Project-URL: Homepage, https://github.com/deuxglaces/mokei
 Project-URL: Issues, https://github.com/deuxglaces/mokei/issues
 Author-email: deuxglaces <dev@deuxglaces.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

