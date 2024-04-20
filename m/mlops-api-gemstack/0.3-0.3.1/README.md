# Comparing `tmp/mlops_api_gemstack-0.3.tar.gz` & `tmp/mlops_api_gemstack-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlops_api_gemstack-0.3.tar", last modified: Sat Apr 20 19:52:35 2024, max compression
+gzip compressed data, was "mlops_api_gemstack-0.3.1.tar", last modified: Sat Apr 20 20:05:40 2024, max compression
```

## Comparing `mlops_api_gemstack-0.3.tar` & `mlops_api_gemstack-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-20 19:52:35.649591 mlops_api_gemstack-0.3/
--rw-r--r--   0 ricardosun   (501) staff       (20)      342 2024-04-20 19:52:35.649030 mlops_api_gemstack-0.3/PKG-INFO
--rw-r--r--   0 ricardosun   (501) staff       (20)        0 2024-04-09 22:49:12.000000 mlops_api_gemstack-0.3/README.md
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-20 19:52:35.622162 mlops_api_gemstack-0.3/mlops_api_gemstack/
--rw-r--r--   0 ricardosun   (501) staff       (20)       18 2024-04-20 05:10:06.000000 mlops_api_gemstack-0.3/mlops_api_gemstack/__init__.py
--rw-r--r--   0 ricardosun   (501) staff       (20)    10904 2024-04-20 19:52:01.000000 mlops_api_gemstack-0.3/mlops_api_gemstack/api.py
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-20 19:52:35.644734 mlops_api_gemstack-0.3/mlops_api_gemstack.egg-info/
--rw-r--r--   0 ricardosun   (501) staff       (20)      342 2024-04-20 19:52:35.000000 mlops_api_gemstack-0.3/mlops_api_gemstack.egg-info/PKG-INFO
--rw-r--r--   0 ricardosun   (501) staff       (20)      329 2024-04-20 19:52:35.000000 mlops_api_gemstack-0.3/mlops_api_gemstack.egg-info/SOURCES.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)        1 2024-04-20 19:52:35.000000 mlops_api_gemstack-0.3/mlops_api_gemstack.egg-info/dependency_links.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       50 2024-04-20 19:52:35.000000 mlops_api_gemstack-0.3/mlops_api_gemstack.egg-info/entry_points.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       37 2024-04-20 19:52:35.000000 mlops_api_gemstack-0.3/mlops_api_gemstack.egg-info/requires.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       19 2024-04-20 19:52:35.000000 mlops_api_gemstack-0.3/mlops_api_gemstack.egg-info/top_level.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       38 2024-04-20 19:52:35.649941 mlops_api_gemstack-0.3/setup.cfg
--rw-r--r--   0 ricardosun   (501) staff       (20)      620 2024-04-20 19:52:30.000000 mlops_api_gemstack-0.3/setup.py
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-20 20:05:40.461067 mlops_api_gemstack-0.3.1/
+-rw-r--r--   0 ricardosun   (501) staff       (20)      344 2024-04-20 20:05:40.460350 mlops_api_gemstack-0.3.1/PKG-INFO
+-rw-r--r--   0 ricardosun   (501) staff       (20)        0 2024-04-09 22:49:12.000000 mlops_api_gemstack-0.3.1/README.md
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-20 20:05:40.449594 mlops_api_gemstack-0.3.1/mlops_api_gemstack/
+-rw-r--r--   0 ricardosun   (501) staff       (20)       18 2024-04-20 05:10:06.000000 mlops_api_gemstack-0.3.1/mlops_api_gemstack/__init__.py
+-rw-r--r--   0 ricardosun   (501) staff       (20)    11785 2024-04-20 20:04:41.000000 mlops_api_gemstack-0.3.1/mlops_api_gemstack/api.py
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-20 20:05:40.458541 mlops_api_gemstack-0.3.1/mlops_api_gemstack.egg-info/
+-rw-r--r--   0 ricardosun   (501) staff       (20)      344 2024-04-20 20:05:40.000000 mlops_api_gemstack-0.3.1/mlops_api_gemstack.egg-info/PKG-INFO
+-rw-r--r--   0 ricardosun   (501) staff       (20)      329 2024-04-20 20:05:40.000000 mlops_api_gemstack-0.3.1/mlops_api_gemstack.egg-info/SOURCES.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)        1 2024-04-20 20:05:40.000000 mlops_api_gemstack-0.3.1/mlops_api_gemstack.egg-info/dependency_links.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       50 2024-04-20 20:05:40.000000 mlops_api_gemstack-0.3.1/mlops_api_gemstack.egg-info/entry_points.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       37 2024-04-20 20:05:40.000000 mlops_api_gemstack-0.3.1/mlops_api_gemstack.egg-info/requires.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       19 2024-04-20 20:05:40.000000 mlops_api_gemstack-0.3.1/mlops_api_gemstack.egg-info/top_level.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       38 2024-04-20 20:05:40.461419 mlops_api_gemstack-0.3.1/setup.cfg
+-rw-r--r--   0 ricardosun   (501) staff       (20)      622 2024-04-20 20:01:30.000000 mlops_api_gemstack-0.3.1/setup.py
```

### Comparing `mlops_api_gemstack-0.3/mlops_api_gemstack/api.py` & `mlops_api_gemstack-0.3.1/mlops_api_gemstack/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,14 +231,35 @@
     except FileNotFoundError:
         click.echo(f"File not found: {file_path}")
     except PermissionError:
         click.echo(f"Permission denied: {file_path}")
     except Exception as e:
         click.echo(f"An error occurred: {e}")
 
+def upload_bag(rosbag_file_name, source):
+    with open(rosbag_file_name, 'rb') as f:
+        files = {'file': f}
+        response = requests.post(f"{base_url}/datasets/uploadBag", files=files)
+        if response.status_code == 200:
+            response_data = response.json()
+            click.echo(f"Message: {response_data['message']}.")
+
+            for inserted in response_data['inserted_objects']:
+                response = requests.put(
+                    f"{base_url}/datasets/{inserted[1]}", 
+                    json={"Source": source}
+                )
+                if response.status_code == 200:
+                    click.echo("Dataset updated successfully")
+                    
+        elif response.status_code == 400:
+            click.echo(f"Error: {response.json()['error']}")
+        else:
+            click.echo(f"Failed to upload the file. Status code: {response.status_code}")
+
 @cli.command()
 @click.argument('topics_file', type=click.Path(exists=True))
 @click.argument('rosbag_file_name')
 @click.argument('source')
 @click.option('--delete_rosbag', is_flag=True, help='Keep the rosbag file after recording')
 def record_rosbag(topics_file, rosbag_file_name, source, delete_rosbag):
 
@@ -258,17 +279,18 @@
 
     process = subprocess.Popen(command, shell=True)
 
     def stop_recording(sig, frame):
         print("Stopping rosbag recording")
         process.terminate()
         print("Recording stopped")
+
         # send rosbag file through api
-        dataset_uploadBag(rosbag_file_name, source)
-        # Add to here
+        upload_bag(rosbag_file_name, source)
+
         if delete_rosbag:
             print("Removing rosbag file")
             subprocess.run(f"rm {rosbag_file_name}", shell=True)
         exit(0)
 
     signal.signal(signal.SIGINT, stop_recording)
```

### Comparing `mlops_api_gemstack-0.3/setup.py` & `mlops_api_gemstack-0.3.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mlops_api_gemstack',
-    version='0.3',
+    version='0.3.1',
     description='An API package connect to a MLops server relating to the GEMstack project.',
     author='Haoming Sun',
     author_email='ricardosun990122@gmail.com',
     url='https://github.com/krishauser/GEMstack/tree/s2024_MLops/MLops/mlops_api_gemstack',
     packages=find_packages(),
     install_requires=[
         'requests',
```

