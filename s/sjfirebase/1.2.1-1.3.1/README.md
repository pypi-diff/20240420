# Comparing `tmp/sjfirebase-1.2.1.tar.gz` & `tmp/sjfirebase-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sjfirebase-1.2.1.tar", max compression
+gzip compressed data, was "sjfirebase-1.3.1.tar", max compression
```

## Comparing `sjfirebase-1.2.1.tar` & `sjfirebase-1.3.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1089 2023-12-10 23:15:47.231398 sjfirebase-1.2.1/LICENSE
--rw-r--r--   0        0        0      384 2024-02-01 01:50:14.727719 sjfirebase-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     5387 2024-01-25 16:02:53.110728 sjfirebase-1.2.1/README.md
--rw-r--r--   0        0        0       85 2023-12-11 00:34:34.249257 sjfirebase-1.2.1/sjfirebase/__init__.py
--rw-r--r--   0        0        0      140 2023-12-27 22:36:50.204966 sjfirebase-1.2.1/sjfirebase/jclass/__init__.py
--rw-r--r--   0        0        0      377 2023-12-27 12:48:03.927374 sjfirebase-1.2.1/sjfirebase/jclass/action.py
--rw-r--r--   0        0        0      398 2023-12-27 12:37:21.088744 sjfirebase-1.2.1/sjfirebase/jclass/auth.py
--rw-r--r--   0        0        0      431 2023-12-27 12:37:21.181438 sjfirebase-1.2.1/sjfirebase/jclass/database.py
--rw-r--r--   0        0        0      350 2023-12-27 06:46:54.841910 sjfirebase-1.2.1/sjfirebase/jclass/firestore.py
--rw-r--r--   0        0        0      686 2024-01-06 06:33:41.814286 sjfirebase-1.2.1/sjfirebase/jclass/storage.py
--rw-r--r--   0        0        0      465 2024-02-01 01:49:57.086573 sjfirebase-1.2.1/sjfirebase/jclass/user.py
--rw-r--r--   0        0        0      117 2024-02-01 01:49:57.042408 sjfirebase-1.2.1/sjfirebase/jinterface/__init__.py
--rw-r--r--   0        0        0      865 2024-01-24 13:11:08.894167 sjfirebase-1.2.1/sjfirebase/jinterface/auth.py
--rw-r--r--   0        0        0     3497 2024-01-25 16:16:16.740098 sjfirebase-1.2.1/sjfirebase/jinterface/database.py
--rw-r--r--   0        0        0      849 2024-01-25 16:33:29.730195 sjfirebase-1.2.1/sjfirebase/jinterface/firestore.py
--rw-r--r--   0        0        0     1295 2024-01-25 16:43:59.689649 sjfirebase-1.2.1/sjfirebase/jinterface/storage.py
--rw-r--r--   0        0        0     1681 2024-01-24 12:22:33.677340 sjfirebase-1.2.1/sjfirebase/jinterface/task.py
--rw-r--r--   0        0        0        0 2023-12-10 23:39:37.131493 sjfirebase-1.2.1/sjfirebase/tools/__init__.py
--rw-r--r--   0        0        0     5671 1970-01-01 00:00:00.000000 sjfirebase-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-06 21:25:57.942339 sjfirebase-1.3.1/LICENSE
+-rw-r--r--   0        0        0     5256 2024-04-20 16:46:58.658368 sjfirebase-1.3.1/README.md
+-rw-r--r--   0        0        0      368 2024-04-20 21:21:43.395769 sjfirebase-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0       84 2024-03-06 21:25:57.942339 sjfirebase-1.3.1/sjfirebase/__init__.py
+-rw-r--r--   0        0        0      139 2024-04-20 16:46:57.466327 sjfirebase-1.3.1/sjfirebase/jclass/__init__.py
+-rw-r--r--   0        0        0      368 2024-03-06 21:25:57.942339 sjfirebase-1.3.1/sjfirebase/jclass/action.py
+-rw-r--r--   0        0        0      421 2024-03-06 21:25:57.942339 sjfirebase-1.3.1/sjfirebase/jclass/database.py
+-rw-r--r--   0        0        0      388 2024-03-06 21:25:57.942339 sjfirebase-1.3.1/sjfirebase/jclass/emailauth.py
+-rw-r--r--   0        0        0      341 2024-03-06 21:25:57.942339 sjfirebase-1.3.1/sjfirebase/jclass/firestore.py
+-rw-r--r--   0        0        0     1030 2024-04-20 17:56:31.465194 sjfirebase-1.3.1/sjfirebase/jclass/phoneauth.py
+-rw-r--r--   0        0        0      248 2024-04-20 16:46:58.266354 sjfirebase-1.3.1/sjfirebase/jclass/storage.py
+-rw-r--r--   0        0        0      455 2024-03-06 21:25:57.942339 sjfirebase-1.3.1/sjfirebase/jclass/user.py
+-rw-r--r--   0        0        0      112 2024-03-06 21:25:57.942339 sjfirebase-1.3.1/sjfirebase/jinterface/__init__.py
+-rw-r--r--   0        0        0      836 2024-03-06 21:25:57.942339 sjfirebase-1.3.1/sjfirebase/jinterface/auth.py
+-rw-r--r--   0        0        0     3410 2024-03-06 21:25:57.942339 sjfirebase-1.3.1/sjfirebase/jinterface/database.py
+-rw-r--r--   0        0        0      822 2024-03-06 21:25:57.942339 sjfirebase-1.3.1/sjfirebase/jinterface/firestore.py
+-rw-r--r--   0        0        0     1255 2024-03-06 21:25:57.942339 sjfirebase-1.3.1/sjfirebase/jinterface/storage.py
+-rw-r--r--   0        0        0     1622 2024-03-06 21:25:57.942339 sjfirebase-1.3.1/sjfirebase/jinterface/task.py
+-rw-r--r--   0        0        0        0 2024-03-06 21:25:57.942339 sjfirebase-1.3.1/sjfirebase/tools/__init__.py
+-rw-r--r--   0        0        0     5828 1970-01-01 00:00:00.000000 sjfirebase-1.3.1/PKG-INFO
```

### Comparing `sjfirebase-1.2.1/README.md` & `sjfirebase-1.3.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,138 +1,154 @@
-# sj-firebase-python
- Implement Firebase Java SDK in Python
-
-*[Firebase](https://firebase.google.com/)*
-> Make your app the
-> best it can be
-> 
-> Firebase is an app development platform that helps you build and grow apps and games users love. 
-> Backed by Google and trusted by millions of businesses around the world.
-
-## Usage
-### Buildozer Android project
-```properties
-android.gradle_dependencies = io.github.simplejnius:sjfirebase:0.3.0
-requirements = https://github.com/SimpleJnius/sj-firebase-python/archive/refs/heads/master.zip
-```
-The current version of [python-for-android](https://github.com/kivy/python-for-android) 
-lacks support for incorporating bom dependencies, modifying the classpath, and copying the `google-service.json`. 
-To address this limitation, a fork of python-for-android has been developed to include these functionalities. 
-To implement these changes in your `buildozer.spec` file, 
-make adjustments to the specified section using the provided values below:
-```properties
-android.api = 34
-android.enable_androidx = True
-android.gradle_dependencies = io.github.simplejnius:sjfirebase:1.0.0,
-    com.google.firebase:firebase-auth,com.google.firebase:firebase-database,
-    com.google.firebase:firebase-firestore,com.google.firebase:firebase-storage,
-    com.google.firebase:firebase-analytics
-p4a.fork = SimpleJnius
-p4a.branch = firebase
-```
-**Important Note:** Upon creating an Android project within your [Firebase Console](https://firebase.google.com), 
-ensure to transfer the `google-service.json` file to the same location as your `main.py` file.
-#### Python(Buildozer) installation
-```shell
-# pip
-pip install sjfirebase
-
-# buildozer.spec
-requirements = sjfirebase
-```
-### Python API
-#### ActionCodeSettings
-```python
-class sjfirebase.jclass.action.ActionCodeSettings
-```
-Structure that contains the required continue/state URL with optional Android and iOS bundle identifiers. 
-The stateUrl used to initialize this class is the link/deep link/fallback url used while constructing the 
-Firebase dynamic link.
-
-**methods**
-- `newBuilder`
-##### Visit [ActionCodeSettings Documentation](https://firebase.google.com/docs/reference/android/com/google/firebase/auth/ActionCodeSettings) for more API
-
-#### SJFirebaseAuthEmai
-```python
-class sjfirebase.jclass.auth.SJFirebaseAuthEmai
-```
-The entry point of the Firebase Authentication SDK.
-First, obtain an instance of this class by calling `get_instance`
-
-**methods**
-- check_user_signed_in
-- get_instance
-##### Visit [FirebaseAuth Documentation](https://firebase.google.com/docs/reference/android/com/google/firebase/auth/FirebaseAuth) for more API
-
-#### SJFirebaseDatabase
-```python
-class sjfirebase.jclass.database.SJFirebaseDatabase
-```
-The entry point for accessing a Firebase Database. 
-You can get an instance by calling getInstance. 
-To access a location in the database and read or write data, use `get_ref`
-
-**methods**
-- get_db
-- get_ref
-##### Visit [FirebaseDatabase Documentation](https://firebase.google.com/docs/reference/android/com/google/firebase/database/FirebaseDatabase) for more API
-
-#### SJFirebaseFirestore
-```python
-class sjfirebase.jclass.firestore.SJFirebaseFirestore
-```
-
-**methods**
-- get_db
-##### Visit [FirebaseFirestore Documentation](https://firebase.google.com/docs/reference/android/com/google/firebase/firestore/FirebaseFirestore) for more API
-
-#### SJFirebaseUser
-```python
-class sjfirebase.jclass.user.SJFirebaseUser
-```
-Represents a user's profile information in your Firebase project's user database. 
-It also contains helper methods to change or retrieve profile information, 
-as well as to manage that user's authentication state.
-
-**methods**
-- get_current_user
-- profile_change_request_builder
-##### Visit [FirebaseUser Documentation](https://firebase.google.com/docs/reference/android/com/google/firebase/auth/FirebaseUser) for more API
-
-#### SJFirebaseStorage
-```python
-class sjfirebase.jclass.user.SJFirebaseStorage
-```
-FirebaseStorage is a service that supports uploading and downloading large objects
-to Google Cloud Storage. Pass a custom instance of FirebaseApp to get_instance which
-will initialize it with a storage location (bucket) specified via setStorageBucket.
-
-Otherwise, if you call getReference without a FirebaseApp, the FirebaseStorage instance
-will initialize with the default FirebaseApp obtainable from get_instance. The storage
-location in this case will come the JSON configuration file downloaded from the web
-
-**methods**
-- get_instance
-##### Visit [FirebaseStorage Documentation](https://firebase.google.com/docs/reference/android/com/google/firebase/storage/FirebaseStorage) for more API
-
-#### OnCompleteListener
-```python
-class sjfirebase.jinterface.google
-
-OnCompleteListener
-```
-Listener called when a Task completes.
-
-**methods**
-- onComplete
-##### Visit [OnCompleteListener Documentation](https://developers.google.com/android/reference/com/google/android/gms/tasks/OnCompleteListener) for more API
-
-#### ValueEventListener
-```python
-class sjfirebase.jinterface.firebase.ValueEventListener
-```
-
-**methods**
-- onDataChange
-- onCancelled
-##### Visit [ValueEventListener Documentation](https://firebase.google.com/docs/reference/android/com/google/firebase/database/ValueEventListener) for more API
+Metadata-Version: 2.1
+Name: sjfirebase
+Version: 1.3.1
+Summary: Implement Firebase Java SDK in python
+Author: Kenechukwu Akubue
+Author-email: kengoon19@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: pyjnius (>=1.6.1,<2.0.0)
+Description-Content-Type: text/markdown
+
+# sj-firebase-python
+ Implement Firebase Java SDK in Python
+
+*[Firebase](https://firebase.google.com/)*
+> Make your app the
+> best it can be
+> 
+> Firebase is an app development platform that helps you build and grow apps and games users love. 
+> Backed by Google and trusted by millions of businesses around the world.
+
+## Usage
+### Buildozer Android project
+```properties
+android.gradle_dependencies = io.github.simplejnius:sjfirebase:0.3.0
+requirements = https://github.com/SimpleJnius/sj-firebase-python/archive/refs/heads/master.zip
+```
+The current version of [python-for-android](https://github.com/kivy/python-for-android) 
+lacks support for incorporating bom dependencies, modifying the classpath, and copying the `google-service.json`. 
+To address this limitation, a fork of python-for-android has been developed to include these functionalities. 
+To implement these changes in your `buildozer.spec` file, 
+make adjustments to the specified section using the provided values below:
+```properties
+android.api = 34
+android.enable_androidx = True
+android.gradle_dependencies = io.github.simplejnius:sjfirebase:1.0.0,
+    com.google.firebase:firebase-auth,com.google.firebase:firebase-database,
+    com.google.firebase:firebase-firestore,com.google.firebase:firebase-storage,
+    com.google.firebase:firebase-analytics
+p4a.fork = SimpleJnius
+p4a.branch = firebase
+```
+**Important Note:** Upon creating an Android project within your [Firebase Console](https://firebase.google.com), 
+ensure to transfer the `google-service.json` file to the same location as your `main.py` file.
+#### Python(Buildozer) installation
+```shell
+# pip
+pip install sjfirebase
+
+# buildozer.spec
+requirements = sjfirebase
+```
+### Python API
+#### ActionCodeSettings
+```python
+class sjfirebase.jclass.action.ActionCodeSettings
+```
+Structure that contains the required continue/state URL with optional Android and iOS bundle identifiers. 
+The stateUrl used to initialize this class is the link/deep link/fallback url used while constructing the 
+Firebase dynamic link.
+
+**methods**
+- `newBuilder`
+##### Visit [ActionCodeSettings Documentation](https://firebase.google.com/docs/reference/android/com/google/firebase/auth/ActionCodeSettings) for more API
+
+#### SJFirebaseAuthEmai
+```python
+class sjfirebase.jclass.emailauth.SJFirebaseAuthEmail
+```
+The entry point of the Firebase Authentication SDK.
+First, obtain an instance of this class by calling `get_instance`
+
+**methods**
+- check_user_signed_in
+- get_instance
+##### Visit [FirebaseAuth Documentation](https://firebase.google.com/docs/reference/android/com/google/firebase/auth/FirebaseAuth) for more API
+
+#### SJFirebaseDatabase
+```python
+class sjfirebase.jclass.database.SJFirebaseDatabase
+```
+The entry point for accessing a Firebase Database. 
+You can get an instance by calling getInstance. 
+To access a location in the database and read or write data, use `get_ref`
+
+**methods**
+- get_db
+- get_ref
+##### Visit [FirebaseDatabase Documentation](https://firebase.google.com/docs/reference/android/com/google/firebase/database/FirebaseDatabase) for more API
+
+#### SJFirebaseFirestore
+```python
+class sjfirebase.jclass.firestore.SJFirebaseFirestore
+```
+
+**methods**
+- get_db
+##### Visit [FirebaseFirestore Documentation](https://firebase.google.com/docs/reference/android/com/google/firebase/firestore/FirebaseFirestore) for more API
+
+#### SJFirebaseUser
+```python
+class sjfirebase.jclass.user.SJFirebaseUser
+```
+Represents a user's profile information in your Firebase project's user database. 
+It also contains helper methods to change or retrieve profile information, 
+as well as to manage that user's authentication state.
+
+**methods**
+- get_current_user
+- profile_change_request_builder
+##### Visit [FirebaseUser Documentation](https://firebase.google.com/docs/reference/android/com/google/firebase/auth/FirebaseUser) for more API
+
+#### SJFirebaseStorage
+```python
+class sjfirebase.jclass.user.SJFirebaseStorage
+```
+FirebaseStorage is a service that supports uploading and downloading large objects
+to Google Cloud Storage. Pass a custom instance of FirebaseApp to get_instance which
+will initialize it with a storage location (bucket) specified via setStorageBucket.
+
+Otherwise, if you call getReference without a FirebaseApp, the FirebaseStorage instance
+will initialize with the default FirebaseApp obtainable from get_instance. The storage
+location in this case will come the JSON configuration file downloaded from the web
+
+**methods**
+- get_instance
+##### Visit [FirebaseStorage Documentation](https://firebase.google.com/docs/reference/android/com/google/firebase/storage/FirebaseStorage) for more API
+
+#### OnCompleteListener
+```python
+class sjfirebase.jinterface.google
+
+OnCompleteListener
+```
+Listener called when a Task completes.
+
+**methods**
+- onComplete
+##### Visit [OnCompleteListener Documentation](https://developers.google.com/android/reference/com/google/android/gms/tasks/OnCompleteListener) for more API
+
+#### ValueEventListener
+```python
+class sjfirebase.jinterface.firebase.ValueEventListener
+```
+
+**methods**
+- onDataChange
+- onCancelled
+##### Visit [ValueEventListener Documentation](https://firebase.google.com/docs/reference/android/com/google/firebase/database/ValueEventListener) for more API
```

### Comparing `sjfirebase-1.2.1/sjfirebase/jinterface/database.py` & `sjfirebase-1.3.1/sjfirebase/jinterface/database.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-from jnius import PythonJavaClass, java_method
-
-__all__ = ("ValueEventListener", "ChildEventListener")
-
-
-class ValueEventListener(PythonJavaClass):
-    __javainterfaces__ = ["com/google/firebase/database/ValueEventListener"]
-    __javacontext__ = "app"
-
-    def __init__(self, on_data_change, on_cancelled):
-        super().__init__()
-        self.on_data_change = on_data_change
-        self.on_cancelled = on_cancelled
-
-    @java_method('(Lcom/google/firebase/database/DataSnapshot;)V')
-    def onDataChange(self, snapshot):
-        self.on_data_change(snapshot)
-
-    @java_method('(Lcom/google/firebase/database/DatabaseError;)V')
-    def onCancelled(self, error):
-        self.on_cancelled(error)
-
-
-class CompletionListener(PythonJavaClass):
-    __javainterfaces__ = ["com/google/firebase/database/DatabaseReference$CompletionListener"]
-    __javacontext__ = "app"
-
-    def __init__(self, on_complete):
-        super().__init__()
-        self.on_complete = on_complete
-
-    @java_method('(Lcom/google/firebase/database/DatabaseError;'
-                 'Lcom/google/firebase/database/DatabaseReference)V')
-    def onComplete(self, error, ref):
-        self.on_complete(error, ref)
-
-
-class ChildEventListener(PythonJavaClass):
-    __javainterfaces__ = ["com/google/firebase/database/ChildEventListener"]
-    __javacontext__ = "app"
-
-    def __init__(self, **kwargs):
-        self.on_cancelled = kwargs.get("on_cancelled", lambda _: None)
-        self.on_child_added = kwargs.get("on_child_added", lambda *_: None)
-        self.on_child_moved = kwargs.get("on_child_moved", lambda *_: None)
-        self.on_child_changed = kwargs.get("on_child_changed", lambda *_: None)
-        self.on_child_removed = kwargs.get("on_child_removed", lambda _: None)
-
-    @java_method('(Lcom/google/firebase/database/DatabaseError;)V')
-    def onCancelled(self, error):
-        self.on_cancelled(error)
-
-    @java_method("(Lcom/google/firebase/database/DataSnapshot;Ljava/lang/String;)V")
-    def onChildAdded(self, snapshot, previous_child_name):
-        self.on_child_added(snapshot, previous_child_name)
-
-    @java_method("(Lcom/google/firebase/database/DataSnapshot;Ljava/lang/String;)V")
-    def onChildChanged(self, snapshot, previous_child_name):
-        self.on_child_changed(snapshot, previous_child_name)
-
-    @java_method("(Lcom/google/firebase/database/DataSnapshot;Ljava/lang/String;)V")
-    def onChildMoved(self, snapshot, previous_child_name):
-        self.on_child_moved(snapshot, previous_child_name)
-
-    @java_method("(Lcom/google/firebase/database/DataSnapshot;)V")
-    def onChildRemoved(self, snapshot):
-        self.on_child_removed(snapshot)
-
-
-class TransactionHandler(PythonJavaClass):
-    __javainterfaces__ = ["com/google/firebase/database/Transaction$Handler"]
-    __javacontext__ = "app"
-
-    def __init__(self, do_transaction, on_complete):
-        super().__init__()
-        self.do_transaction = do_transaction
-        self.on_complete = on_complete
-
-    @java_method("(Lcom/google/firebase/database/MutableData;)"
-                 "Lcom/google/firebase/database/Transaction$Result")
-    def doTransaction(self, current_data):
-        self.do_transaction(current_data)
-
-    @java_method('(Lcom/google/firebase/database/DatabaseError;'
-                 'Lcom/google/firebase/database/DataSnapshot)V')
-    def onComplete(self, error, current_data):
-        self.on_complete(error, current_data)
+from jnius import PythonJavaClass, java_method
+
+__all__ = ("ValueEventListener", "ChildEventListener")
+
+
+class ValueEventListener(PythonJavaClass):
+    __javainterfaces__ = ["com/google/firebase/database/ValueEventListener"]
+    __javacontext__ = "app"
+
+    def __init__(self, on_data_change, on_cancelled):
+        super().__init__()
+        self.on_data_change = on_data_change
+        self.on_cancelled = on_cancelled
+
+    @java_method('(Lcom/google/firebase/database/DataSnapshot;)V')
+    def onDataChange(self, snapshot):
+        self.on_data_change(snapshot)
+
+    @java_method('(Lcom/google/firebase/database/DatabaseError;)V')
+    def onCancelled(self, error):
+        self.on_cancelled(error)
+
+
+class CompletionListener(PythonJavaClass):
+    __javainterfaces__ = ["com/google/firebase/database/DatabaseReference$CompletionListener"]
+    __javacontext__ = "app"
+
+    def __init__(self, on_complete):
+        super().__init__()
+        self.on_complete = on_complete
+
+    @java_method('(Lcom/google/firebase/database/DatabaseError;'
+                 'Lcom/google/firebase/database/DatabaseReference)V')
+    def onComplete(self, error, ref):
+        self.on_complete(error, ref)
+
+
+class ChildEventListener(PythonJavaClass):
+    __javainterfaces__ = ["com/google/firebase/database/ChildEventListener"]
+    __javacontext__ = "app"
+
+    def __init__(self, **kwargs):
+        self.on_cancelled = kwargs.get("on_cancelled", lambda _: None)
+        self.on_child_added = kwargs.get("on_child_added", lambda *_: None)
+        self.on_child_moved = kwargs.get("on_child_moved", lambda *_: None)
+        self.on_child_changed = kwargs.get("on_child_changed", lambda *_: None)
+        self.on_child_removed = kwargs.get("on_child_removed", lambda _: None)
+
+    @java_method('(Lcom/google/firebase/database/DatabaseError;)V')
+    def onCancelled(self, error):
+        self.on_cancelled(error)
+
+    @java_method("(Lcom/google/firebase/database/DataSnapshot;Ljava/lang/String;)V")
+    def onChildAdded(self, snapshot, previous_child_name):
+        self.on_child_added(snapshot, previous_child_name)
+
+    @java_method("(Lcom/google/firebase/database/DataSnapshot;Ljava/lang/String;)V")
+    def onChildChanged(self, snapshot, previous_child_name):
+        self.on_child_changed(snapshot, previous_child_name)
+
+    @java_method("(Lcom/google/firebase/database/DataSnapshot;Ljava/lang/String;)V")
+    def onChildMoved(self, snapshot, previous_child_name):
+        self.on_child_moved(snapshot, previous_child_name)
+
+    @java_method("(Lcom/google/firebase/database/DataSnapshot;)V")
+    def onChildRemoved(self, snapshot):
+        self.on_child_removed(snapshot)
+
+
+class TransactionHandler(PythonJavaClass):
+    __javainterfaces__ = ["com/google/firebase/database/Transaction$Handler"]
+    __javacontext__ = "app"
+
+    def __init__(self, do_transaction, on_complete):
+        super().__init__()
+        self.do_transaction = do_transaction
+        self.on_complete = on_complete
+
+    @java_method("(Lcom/google/firebase/database/MutableData;)"
+                 "Lcom/google/firebase/database/Transaction$Result")
+    def doTransaction(self, current_data):
+        self.do_transaction(current_data)
+
+    @java_method('(Lcom/google/firebase/database/DatabaseError;'
+                 'Lcom/google/firebase/database/DataSnapshot)V')
+    def onComplete(self, error, current_data):
+        self.on_complete(error, current_data)
```

### Comparing `sjfirebase-1.2.1/sjfirebase/jinterface/firestore.py` & `sjfirebase-1.3.1/sjfirebase/jinterface/firestore.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from jnius import PythonJavaClass, java_method
-
-__all__ = ("EventListener", "OnProgressListener")
-
-
-class EventListener(PythonJavaClass):
-    __javainterfaces__ = ["com/google/firebase/firestore/EventListener"]
-    __javacontext__ = "app"
-
-    def __init__(self, on_event):
-        self.on_event = on_event
-
-    @java_method("(Ljava/lang/Object;com/google/firebase/firestore/FirebaseFirestoreException;)V")
-    def onEvent(self, value, error):
-        self.on_event(value, error)
-
-
-class OnProgressListener(PythonJavaClass):
-    __javainterfaces__ = ["com/google/firebase/firestore/OnProgressListener"]
-    __javacontext__ = "app"
-
-    def __init__(self, on_progress):
-        self.on_progress = on_progress
-
-    @java_method("(Ljava/lang/Object;)V")
-    def onProgress(self, snapshot):
-        self.on_progress(snapshot)
+from jnius import PythonJavaClass, java_method
+
+__all__ = ("EventListener", "OnProgressListener")
+
+
+class EventListener(PythonJavaClass):
+    __javainterfaces__ = ["com/google/firebase/firestore/EventListener"]
+    __javacontext__ = "app"
+
+    def __init__(self, on_event):
+        self.on_event = on_event
+
+    @java_method("(Ljava/lang/Object;com/google/firebase/firestore/FirebaseFirestoreException;)V")
+    def onEvent(self, value, error):
+        self.on_event(value, error)
+
+
+class OnProgressListener(PythonJavaClass):
+    __javainterfaces__ = ["com/google/firebase/firestore/OnProgressListener"]
+    __javacontext__ = "app"
+
+    def __init__(self, on_progress):
+        self.on_progress = on_progress
+
+    @java_method("(Ljava/lang/Object;)V")
+    def onProgress(self, snapshot):
+        self.on_progress(snapshot)
```

### Comparing `sjfirebase-1.2.1/sjfirebase/jinterface/task.py` & `sjfirebase-1.3.1/sjfirebase/jinterface/task.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from jnius import PythonJavaClass, java_method
-
-__all__ = ("OnCompleteListener", "OnCanceledListener", "OnFailureListener", "OnSuccessListener")
-
-
-class OnCompleteListener(PythonJavaClass):
-    __javainterfaces__ = ["com/google/android/gms/tasks/OnCompleteListener"]
-    __javacontext__ = "app"
-
-    def __init__(self, callback):
-        super().__init__()
-        self.callback = callback
-
-    @java_method('(Lcom/google/android/gms/tasks/Task;)V')
-    def onComplete(self, task):
-        self.callback(task)
-
-
-class OnCanceledListener(PythonJavaClass):
-    __javainterfaces__ = ["com/google/android/gms/tasks/OnCanceledListener"]
-    __javacontext__ = "app"
-
-    def __init__(self, callback):
-        super().__init__()
-        self.callback = callback
-
-    @java_method('()V')
-    def onCanceled(self):
-        self.callback()
-
-
-class OnFailureListener(PythonJavaClass):
-    __javainterfaces__ = ["com/google/android/gms/tasks/OnFailureListener"]
-    __javacontext__ = "app"
-
-    def __init__(self, callback):
-        super().__init__()
-        self.callback = callback
-
-    @java_method('(Ljava.lang.Exception;)V')
-    def onFailure(self, e):
-        self.callback(e)
-
-
-class OnSuccessListener(PythonJavaClass):
-    __javainterfaces__ = ["com/google/android/gms/tasks/OnSuccessListener"]
-    __javacontext__ = "app"
-
-    def __init__(self, callback, args=False):
-        super().__init__()
-        self._args = args
-        self.callback = callback
-
-    @java_method('(Ljava/lang/Object;)V')
-    def onSuccess(self, obj):
-        if self._args:
-            self.callback(obj)
-        else:
-            self.callback()
+from jnius import PythonJavaClass, java_method
+
+__all__ = ("OnCompleteListener", "OnCanceledListener", "OnFailureListener", "OnSuccessListener")
+
+
+class OnCompleteListener(PythonJavaClass):
+    __javainterfaces__ = ["com/google/android/gms/tasks/OnCompleteListener"]
+    __javacontext__ = "app"
+
+    def __init__(self, callback):
+        super().__init__()
+        self.callback = callback
+
+    @java_method('(Lcom/google/android/gms/tasks/Task;)V')
+    def onComplete(self, task):
+        self.callback(task)
+
+
+class OnCanceledListener(PythonJavaClass):
+    __javainterfaces__ = ["com/google/android/gms/tasks/OnCanceledListener"]
+    __javacontext__ = "app"
+
+    def __init__(self, callback):
+        super().__init__()
+        self.callback = callback
+
+    @java_method('()V')
+    def onCanceled(self):
+        self.callback()
+
+
+class OnFailureListener(PythonJavaClass):
+    __javainterfaces__ = ["com/google/android/gms/tasks/OnFailureListener"]
+    __javacontext__ = "app"
+
+    def __init__(self, callback):
+        super().__init__()
+        self.callback = callback
+
+    @java_method('(Ljava.lang.Exception;)V')
+    def onFailure(self, e):
+        self.callback(e)
+
+
+class OnSuccessListener(PythonJavaClass):
+    __javainterfaces__ = ["com/google/android/gms/tasks/OnSuccessListener"]
+    __javacontext__ = "app"
+
+    def __init__(self, callback, args=False):
+        super().__init__()
+        self._args = args
+        self.callback = callback
+
+    @java_method('(Ljava/lang/Object;)V')
+    def onSuccess(self, obj):
+        if self._args:
+            self.callback(obj)
+        else:
+            self.callback()
```

### Comparing `sjfirebase-1.2.1/PKG-INFO` & `sjfirebase-1.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: sjfirebase
-Version: 1.2.1
-Summary: Implement Firebase Java SDK in pytho
-Author: Kenechukwu Akubue
-Author-email: kengoon19@gmail.com
-Requires-Python: >=3.11,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pyjnius (>=1.6.1,<2.0.0)
-Description-Content-Type: text/markdown
-
 # sj-firebase-python
  Implement Firebase Java SDK in Python
 
 *[Firebase](https://firebase.google.com/)*
 > Make your app the
 > best it can be
 > 
@@ -63,15 +50,15 @@
 
 **methods**
 - `newBuilder`
 ##### Visit [ActionCodeSettings Documentation](https://firebase.google.com/docs/reference/android/com/google/firebase/auth/ActionCodeSettings) for more API
 
 #### SJFirebaseAuthEmai
 ```python
-class sjfirebase.jclass.auth.SJFirebaseAuthEmai
+class sjfirebase.jclass.emailauth.SJFirebaseAuthEmail
 ```
 The entry point of the Firebase Authentication SDK.
 First, obtain an instance of this class by calling `get_instance`
 
 **methods**
 - check_user_signed_in
 - get_instance
@@ -144,8 +131,8 @@
 ```python
 class sjfirebase.jinterface.firebase.ValueEventListener
 ```
 
 **methods**
 - onDataChange
 - onCancelled
-##### Visit [ValueEventListener Documentation](https://firebase.google.com/docs/reference/android/com/google/firebase/database/ValueEventListener) for more API
+##### Visit [ValueEventListener Documentation](https://firebase.google.com/docs/reference/android/com/google/firebase/database/ValueEventListener) for more API
```

