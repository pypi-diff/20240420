# Comparing `tmp/robotframework_confluentkafkalibrary-2.2.0.post1.tar.gz` & `tmp/robotframework_confluentkafkalibrary-2.3.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_confluentkafkalibrary-2.2.0.post1.tar", last modified: Sat Apr 13 19:52:38 2024, max compression
+gzip compressed data, was "robotframework_confluentkafkalibrary-2.3.0.post1.tar", last modified: Sat Apr 20 20:50:58 2024, max compression
```

## Comparing `robotframework_confluentkafkalibrary-2.2.0.post1.tar` & `robotframework_confluentkafkalibrary-2.3.0.post1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:52:38.663756 robotframework_confluentkafkalibrary-2.2.0.post1/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-13 19:52:32.000000 robotframework_confluentkafkalibrary-2.2.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-13 19:52:38.663756 robotframework_confluentkafkalibrary-2.2.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-13 19:52:32.000000 robotframework_confluentkafkalibrary-2.2.0.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 19:52:38.663756 robotframework_confluentkafkalibrary-2.2.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-13 19:52:32.000000 robotframework_confluentkafkalibrary-2.2.0.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:52:38.659756 robotframework_confluentkafkalibrary-2.2.0.post1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:52:38.659756 robotframework_confluentkafkalibrary-2.2.0.post1/src/ConfluentKafkaLibrary/
--rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-04-13 19:52:32.000000 robotframework_confluentkafkalibrary-2.2.0.post1/src/ConfluentKafkaLibrary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-04-13 19:52:32.000000 robotframework_confluentkafkalibrary-2.2.0.post1/src/ConfluentKafkaLibrary/admin_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16088 2024-04-13 19:52:32.000000 robotframework_confluentkafkalibrary-2.2.0.post1/src/ConfluentKafkaLibrary/consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-13 19:52:32.000000 robotframework_confluentkafkalibrary-2.2.0.post1/src/ConfluentKafkaLibrary/producer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-13 19:52:32.000000 robotframework_confluentkafkalibrary-2.2.0.post1/src/ConfluentKafkaLibrary/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-13 19:52:32.000000 robotframework_confluentkafkalibrary-2.2.0.post1/src/ConfluentKafkaLibrary/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:52:38.663756 robotframework_confluentkafkalibrary-2.2.0.post1/src/robotframework_confluentkafkalibrary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-13 19:52:38.000000 robotframework_confluentkafkalibrary-2.2.0.post1/src/robotframework_confluentkafkalibrary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-13 19:52:38.000000 robotframework_confluentkafkalibrary-2.2.0.post1/src/robotframework_confluentkafkalibrary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 19:52:38.000000 robotframework_confluentkafkalibrary-2.2.0.post1/src/robotframework_confluentkafkalibrary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-13 19:52:38.000000 robotframework_confluentkafkalibrary-2.2.0.post1/src/robotframework_confluentkafkalibrary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-13 19:52:38.000000 robotframework_confluentkafkalibrary-2.2.0.post1/src/robotframework_confluentkafkalibrary.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:50:58.422298 robotframework_confluentkafkalibrary-2.3.0.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-20 20:50:52.000000 robotframework_confluentkafkalibrary-2.3.0.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-20 20:50:58.418298 robotframework_confluentkafkalibrary-2.3.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-20 20:50:52.000000 robotframework_confluentkafkalibrary-2.3.0.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 20:50:58.422298 robotframework_confluentkafkalibrary-2.3.0.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-20 20:50:52.000000 robotframework_confluentkafkalibrary-2.3.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:50:58.414298 robotframework_confluentkafkalibrary-2.3.0.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:50:58.418298 robotframework_confluentkafkalibrary-2.3.0.post1/src/ConfluentKafkaLibrary/
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-04-20 20:50:52.000000 robotframework_confluentkafkalibrary-2.3.0.post1/src/ConfluentKafkaLibrary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-04-20 20:50:52.000000 robotframework_confluentkafkalibrary-2.3.0.post1/src/ConfluentKafkaLibrary/admin_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16088 2024-04-20 20:50:52.000000 robotframework_confluentkafkalibrary-2.3.0.post1/src/ConfluentKafkaLibrary/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-20 20:50:52.000000 robotframework_confluentkafkalibrary-2.3.0.post1/src/ConfluentKafkaLibrary/producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-20 20:50:52.000000 robotframework_confluentkafkalibrary-2.3.0.post1/src/ConfluentKafkaLibrary/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-20 20:50:52.000000 robotframework_confluentkafkalibrary-2.3.0.post1/src/ConfluentKafkaLibrary/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:50:58.418298 robotframework_confluentkafkalibrary-2.3.0.post1/src/robotframework_confluentkafkalibrary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-20 20:50:58.000000 robotframework_confluentkafkalibrary-2.3.0.post1/src/robotframework_confluentkafkalibrary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-20 20:50:58.000000 robotframework_confluentkafkalibrary-2.3.0.post1/src/robotframework_confluentkafkalibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 20:50:58.000000 robotframework_confluentkafkalibrary-2.3.0.post1/src/robotframework_confluentkafkalibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-20 20:50:58.000000 robotframework_confluentkafkalibrary-2.3.0.post1/src/robotframework_confluentkafkalibrary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 20:50:58.000000 robotframework_confluentkafkalibrary-2.3.0.post1/src/robotframework_confluentkafkalibrary.egg-info/top_level.txt
```

### Comparing `robotframework_confluentkafkalibrary-2.2.0.post1/LICENSE` & `robotframework_confluentkafkalibrary-2.3.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_confluentkafkalibrary-2.2.0.post1/README.md` & `robotframework_confluentkafkalibrary-2.3.0.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 To install the library, run the following command:
 
 ```
 pip install robotframework-confluentkafkalibrary
 ```
 
 Extra packages:
-* [avro] = ['fastavro >= 1.3.2', 'avro-python3 >= 1.10.1']
+* [avro] = ['fastavro >= 1.3.2', 'avro >= 1.11.1']
+* [legacyavro] = ['fastavro >= 1.3.2', 'avro-python3 >= 1.10.1']
 * [json] = ['jsonschema >= 3.2.0']
 * [protobuf] = ['protobuf >= 4.22.0']
 
 To install all dependencies use `[all]` extension like:
 
 ```
 pip install robotframework-confluentkafkalibrary[all]
```

### Comparing `robotframework_confluentkafkalibrary-2.2.0.post1/setup.py` & `robotframework_confluentkafkalibrary-2.3.0.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 filename=join(dirname(__file__), 'src', 'ConfluentKafkaLibrary', 'version.py')
 exec(compile(open(filename).read(),filename, 'exec'))
 
 DESCRIPTION = """
 Confluent Kafka wrapped in Robot Framework.
 """[1:-1]
 
-AVRO_REQUIRES = ['fastavro >= 1.3.2', 'avro-python3 >= 1.10.1']
+AVRO_REQUIRES = ['fastavro >= 1.3.2', 'avro >= 1.11.1']
+LEGACYAVRO_REQUIRES = ['fastavro >= 1.3.2', 'avro-python3 >= 1.10.1']
 JSON_REQUIRES = ['jsonschema >= 3.2.0']
 PROTO_REQUIRES = ['protobuf >= 4.22.0']
-ALL = AVRO_REQUIRES + JSON_REQUIRES + PROTO_REQUIRES
+ALL = AVRO_REQUIRES + LEGACYAVRO_REQUIRES + JSON_REQUIRES + PROTO_REQUIRES
 setup(name         = 'robotframework-confluentkafkalibrary',
       version      = VERSION,
       description  = 'Confluent Kafka library for Robot Framework',
       long_description = DESCRIPTION,
       author       = 'Robert Karasek',
       author_email = '<robo.karasek@gmail.com>',
       url          = 'https://github.com/robooo/robotframework-ConfluentKafkaLibrary',
@@ -28,19 +29,20 @@
           "License :: OSI Approved :: Apache Software License",
           "Operating System :: OS Independent",
           "Programming Language :: Python",
           "Topic :: Software Development :: Testing"
       ],
       install_requires = [
           'robotframework >= 3.2.1',
-          'confluent-kafka == 2.2.0',
+          'confluent-kafka == 2.3.0',
           'requests >= 2.25.1',
       ],
       extras_require={
           'all': ALL,
           'avro': AVRO_REQUIRES,
+          'legacyavro': LEGACYAVRO_REQUIRES,
           'json': JSON_REQUIRES,
           'protobuf': PROTO_REQUIRES,
       },
       package_dir  = {'' : 'src'},
       packages     = ['ConfluentKafkaLibrary'],
       )
```

### Comparing `robotframework_confluentkafkalibrary-2.2.0.post1/src/ConfluentKafkaLibrary/__init__.py` & `robotframework_confluentkafkalibrary-2.3.0.post1/src/ConfluentKafkaLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework_confluentkafkalibrary-2.2.0.post1/src/ConfluentKafkaLibrary/admin_client.py` & `robotframework_confluentkafkalibrary-2.3.0.post1/src/ConfluentKafkaLibrary/admin_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import uuid
 from confluent_kafka.admin import AdminClient
-from confluent_kafka import KafkaException
+from confluent_kafka import KafkaException, TopicCollection
 
 
 class KafkaAdminClient():
 
     def __init__(self):
         self.admin_clients = {}
 
@@ -166,14 +166,52 @@
                     config_results[config.name] = f.exception()
             except KafkaException as e:
                 return f"Failed to describe config {config.name}: {e}"
             except (TypeError, ValueError ) as e:
                 return f"Invalid input: {e}"
         return config_results
 
+    def describe_topics(self, group_id, topics, **kwargs):
+        """Describe topics.
+        - ``topics``  (list(str) or str): List of topic names or only topic name to describe.
+        """
+        if isinstance(topics, list):
+            topics = TopicCollection(topics)
+        else:
+            topics = TopicCollection([topics])
+
+        topics = self.admin_clients[group_id].describe_topics(topics, **kwargs)
+        topics_results={}
+        for topic, f in topics.items():
+            try:
+                if f.exception() is None:
+                    topics_results[topic] = f.result()
+                else:
+                    topics_results[topic] = f.exception()
+            except KafkaException as e:
+                return f"Failed to describe topic {topic.name}: {e}"
+            except (TypeError, ValueError ) as e:
+                return f"Invalid input: {e}"
+        return topics_results
+
+    def describe_cluster(self, group_id, **kwargs):
+        """Describe cluster.
+        """
+        cluster = self.admin_clients[group_id].describe_cluster(**kwargs)
+        try:
+            if cluster.exception() is None:
+                cluster = cluster.result()
+            else:
+                cluster = cluster.exception()
+        except KafkaException as e:
+            return f"Failed to describe cluster: {e}"
+        except (TypeError, ValueError ) as e:
+            return f"Invalid input: {e}"
+        return cluster
+
     def alter_configs(self, group_id, resources, **kwargs):
         """Update configuration properties for the specified resources.
         - ``resources``  (list(ConfigResource) or ConfigResource): Resources to update configuration of.
         """
         fs = None
         if isinstance(resources, list):
             fs = self.admin_clients[group_id].alter_configs(resources, **kwargs)
```

### Comparing `robotframework_confluentkafkalibrary-2.2.0.post1/src/ConfluentKafkaLibrary/consumer.py` & `robotframework_confluentkafkalibrary-2.3.0.post1/src/ConfluentKafkaLibrary/consumer.py`

 * *Files identical despite different names*

### Comparing `robotframework_confluentkafkalibrary-2.2.0.post1/src/ConfluentKafkaLibrary/producer.py` & `robotframework_confluentkafkalibrary-2.3.0.post1/src/ConfluentKafkaLibrary/producer.py`

 * *Files identical despite different names*

### Comparing `robotframework_confluentkafkalibrary-2.2.0.post1/src/ConfluentKafkaLibrary/serialization.py` & `robotframework_confluentkafkalibrary-2.3.0.post1/src/ConfluentKafkaLibrary/serialization.py`

 * *Files identical despite different names*

### Comparing `robotframework_confluentkafkalibrary-2.2.0.post1/src/robotframework_confluentkafkalibrary.egg-info/SOURCES.txt` & `robotframework_confluentkafkalibrary-2.3.0.post1/src/robotframework_confluentkafkalibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

