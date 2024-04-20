# Comparing `tmp/mlops_api_gemstack-0.1.tar.gz` & `tmp/mlops_api_gemstack-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlops_api_gemstack-0.1.tar", last modified: Sat Apr 20 05:41:48 2024, max compression
+gzip compressed data, was "mlops_api_gemstack-0.2.tar", last modified: Sat Apr 20 18:57:50 2024, max compression
```

## Comparing `mlops_api_gemstack-0.1.tar` & `mlops_api_gemstack-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-20 05:41:48.864667 mlops_api_gemstack-0.1/
--rw-r--r--   0 ricardosun   (501) staff       (20)      342 2024-04-20 05:41:48.863705 mlops_api_gemstack-0.1/PKG-INFO
--rw-r--r--   0 ricardosun   (501) staff       (20)        0 2024-04-09 22:49:12.000000 mlops_api_gemstack-0.1/README.md
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-20 05:41:48.852946 mlops_api_gemstack-0.1/mlops_api_gemstack/
--rw-r--r--   0 ricardosun   (501) staff       (20)       18 2024-04-20 05:10:06.000000 mlops_api_gemstack-0.1/mlops_api_gemstack/__init__.py
--rw-r--r--   0 ricardosun   (501) staff       (20)    10803 2024-04-20 05:40:02.000000 mlops_api_gemstack-0.1/mlops_api_gemstack/api.py
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-20 05:41:48.862664 mlops_api_gemstack-0.1/mlops_api_gemstack.egg-info/
--rw-r--r--   0 ricardosun   (501) staff       (20)      342 2024-04-20 05:41:48.000000 mlops_api_gemstack-0.1/mlops_api_gemstack.egg-info/PKG-INFO
--rw-r--r--   0 ricardosun   (501) staff       (20)      329 2024-04-20 05:41:48.000000 mlops_api_gemstack-0.1/mlops_api_gemstack.egg-info/SOURCES.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)        1 2024-04-20 05:41:48.000000 mlops_api_gemstack-0.1/mlops_api_gemstack.egg-info/dependency_links.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       50 2024-04-20 05:41:48.000000 mlops_api_gemstack-0.1/mlops_api_gemstack.egg-info/entry_points.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       37 2024-04-20 05:41:48.000000 mlops_api_gemstack-0.1/mlops_api_gemstack.egg-info/requires.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       19 2024-04-20 05:41:48.000000 mlops_api_gemstack-0.1/mlops_api_gemstack.egg-info/top_level.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       38 2024-04-20 05:41:48.866302 mlops_api_gemstack-0.1/setup.cfg
--rw-r--r--   0 ricardosun   (501) staff       (20)      620 2024-04-20 04:30:02.000000 mlops_api_gemstack-0.1/setup.py
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-20 18:57:50.208727 mlops_api_gemstack-0.2/
+-rw-r--r--   0 ricardosun   (501) staff       (20)      342 2024-04-20 18:57:50.208054 mlops_api_gemstack-0.2/PKG-INFO
+-rw-r--r--   0 ricardosun   (501) staff       (20)        0 2024-04-09 22:49:12.000000 mlops_api_gemstack-0.2/README.md
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-20 18:57:50.193830 mlops_api_gemstack-0.2/mlops_api_gemstack/
+-rw-r--r--   0 ricardosun   (501) staff       (20)       18 2024-04-20 05:10:06.000000 mlops_api_gemstack-0.2/mlops_api_gemstack/__init__.py
+-rw-r--r--   0 ricardosun   (501) staff       (20)    10879 2024-04-20 18:55:15.000000 mlops_api_gemstack-0.2/mlops_api_gemstack/api.py
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-20 18:57:50.201419 mlops_api_gemstack-0.2/mlops_api_gemstack.egg-info/
+-rw-r--r--   0 ricardosun   (501) staff       (20)      342 2024-04-20 18:57:50.000000 mlops_api_gemstack-0.2/mlops_api_gemstack.egg-info/PKG-INFO
+-rw-r--r--   0 ricardosun   (501) staff       (20)      329 2024-04-20 18:57:50.000000 mlops_api_gemstack-0.2/mlops_api_gemstack.egg-info/SOURCES.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)        1 2024-04-20 18:57:50.000000 mlops_api_gemstack-0.2/mlops_api_gemstack.egg-info/dependency_links.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       50 2024-04-20 18:57:50.000000 mlops_api_gemstack-0.2/mlops_api_gemstack.egg-info/entry_points.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       37 2024-04-20 18:57:50.000000 mlops_api_gemstack-0.2/mlops_api_gemstack.egg-info/requires.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       19 2024-04-20 18:57:50.000000 mlops_api_gemstack-0.2/mlops_api_gemstack.egg-info/top_level.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       38 2024-04-20 18:57:50.208994 mlops_api_gemstack-0.2/setup.cfg
+-rw-r--r--   0 ricardosun   (501) staff       (20)      620 2024-04-20 18:57:44.000000 mlops_api_gemstack-0.2/setup.py
```

### Comparing `mlops_api_gemstack-0.1/mlops_api_gemstack/api.py` & `mlops_api_gemstack-0.2/mlops_api_gemstack/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
 @click.argument('file_path')
 @click.argument('source')
 def dataset_upload(file_path, source):
     try:
         with open(file_path, 'rb') as f:
             files = {'file': f}
             click.echo(f"Uploading {file_path}. Please wait and do not kill the process. This may take a while.")
-            response = requests.post(f"{base_url}/datasets/upload", files=files)
+            response = requests.post(f"{base_url}/datasets/upload", files=files, stream=True)
             if response.status_code == 200:
                 response_data = response.json()
                 click.echo(f"Message: {response_data['message']}. Dataset name: {response_data['filename']}")
                 response = requests.put(
                     f"{base_url}/datasets/{response_data['inserted_datasets_id']}", 
                     json={"Source": source}
                 )
@@ -243,26 +243,28 @@
 
     with open(topics_file) as f:
         topics = [line.strip() for line in f.readlines()]
 
     if not topics:
         print(f"No topics found in {topics_file}")
         exit(1)
+    
+    if not rosbag_file_name.endswith('.bag'):
+        rosbag_file_name += '.bag'
 
     topics = " ".join(topics)
 
     command = f"rosbag record {topics} -O {rosbag_file_name}"
     # command = "ping 127.0.0.1 -t"
 
     process = subprocess.Popen(command, shell=True)
 
     def stop_recording(sig, frame):
         print("Stopping rosbag recording")
         process.terminate()
-        process.wait()
         print("Recording stopped")
         # send rosbag file through api
         # Add to here
         if delete_rosbag:
             print("Removing rosbag file")
             subprocess.run(f"rm {rosbag_file_name}", shell=True)
         exit(0)
```

### Comparing `mlops_api_gemstack-0.1/setup.py` & `mlops_api_gemstack-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mlops_api_gemstack',
-    version='0.1',
+    version='0.2',
     description='An API package connect to a MLops server relating to the GEMstack project.',
     author='Haoming Sun',
     author_email='ricardosun990122@gmail.com',
     url='https://github.com/krishauser/GEMstack/tree/s2024_MLops/MLops/mlops_api_gemstack',
     packages=find_packages(),
     install_requires=[
         'requests',
```

