# Comparing `tmp/mlops_api_gemstack-0.2.1.tar.gz` & `tmp/mlops_api_gemstack-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlops_api_gemstack-0.2.1.tar", last modified: Sat Apr 20 19:13:57 2024, max compression
+gzip compressed data, was "mlops_api_gemstack-0.3.tar", last modified: Sat Apr 20 19:52:35 2024, max compression
```

## Comparing `mlops_api_gemstack-0.2.1.tar` & `mlops_api_gemstack-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-20 19:13:57.096831 mlops_api_gemstack-0.2.1/
--rw-r--r--   0 ricardosun   (501) staff       (20)      344 2024-04-20 19:13:57.096268 mlops_api_gemstack-0.2.1/PKG-INFO
--rw-r--r--   0 ricardosun   (501) staff       (20)        0 2024-04-09 22:49:12.000000 mlops_api_gemstack-0.2.1/README.md
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-20 19:13:57.090391 mlops_api_gemstack-0.2.1/mlops_api_gemstack/
--rw-r--r--   0 ricardosun   (501) staff       (20)       18 2024-04-20 05:10:06.000000 mlops_api_gemstack-0.2.1/mlops_api_gemstack/__init__.py
--rw-r--r--   0 ricardosun   (501) staff       (20)    10854 2024-04-20 19:13:16.000000 mlops_api_gemstack-0.2.1/mlops_api_gemstack/api.py
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-20 19:13:57.095137 mlops_api_gemstack-0.2.1/mlops_api_gemstack.egg-info/
--rw-r--r--   0 ricardosun   (501) staff       (20)      344 2024-04-20 19:13:56.000000 mlops_api_gemstack-0.2.1/mlops_api_gemstack.egg-info/PKG-INFO
--rw-r--r--   0 ricardosun   (501) staff       (20)      329 2024-04-20 19:13:56.000000 mlops_api_gemstack-0.2.1/mlops_api_gemstack.egg-info/SOURCES.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)        1 2024-04-20 19:13:56.000000 mlops_api_gemstack-0.2.1/mlops_api_gemstack.egg-info/dependency_links.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       50 2024-04-20 19:13:56.000000 mlops_api_gemstack-0.2.1/mlops_api_gemstack.egg-info/entry_points.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       37 2024-04-20 19:13:56.000000 mlops_api_gemstack-0.2.1/mlops_api_gemstack.egg-info/requires.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       19 2024-04-20 19:13:56.000000 mlops_api_gemstack-0.2.1/mlops_api_gemstack.egg-info/top_level.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       38 2024-04-20 19:13:57.097056 mlops_api_gemstack-0.2.1/setup.cfg
--rw-r--r--   0 ricardosun   (501) staff       (20)      622 2024-04-20 19:13:47.000000 mlops_api_gemstack-0.2.1/setup.py
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-20 19:52:35.649591 mlops_api_gemstack-0.3/
+-rw-r--r--   0 ricardosun   (501) staff       (20)      342 2024-04-20 19:52:35.649030 mlops_api_gemstack-0.3/PKG-INFO
+-rw-r--r--   0 ricardosun   (501) staff       (20)        0 2024-04-09 22:49:12.000000 mlops_api_gemstack-0.3/README.md
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-20 19:52:35.622162 mlops_api_gemstack-0.3/mlops_api_gemstack/
+-rw-r--r--   0 ricardosun   (501) staff       (20)       18 2024-04-20 05:10:06.000000 mlops_api_gemstack-0.3/mlops_api_gemstack/__init__.py
+-rw-r--r--   0 ricardosun   (501) staff       (20)    10904 2024-04-20 19:52:01.000000 mlops_api_gemstack-0.3/mlops_api_gemstack/api.py
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-20 19:52:35.644734 mlops_api_gemstack-0.3/mlops_api_gemstack.egg-info/
+-rw-r--r--   0 ricardosun   (501) staff       (20)      342 2024-04-20 19:52:35.000000 mlops_api_gemstack-0.3/mlops_api_gemstack.egg-info/PKG-INFO
+-rw-r--r--   0 ricardosun   (501) staff       (20)      329 2024-04-20 19:52:35.000000 mlops_api_gemstack-0.3/mlops_api_gemstack.egg-info/SOURCES.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)        1 2024-04-20 19:52:35.000000 mlops_api_gemstack-0.3/mlops_api_gemstack.egg-info/dependency_links.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       50 2024-04-20 19:52:35.000000 mlops_api_gemstack-0.3/mlops_api_gemstack.egg-info/entry_points.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       37 2024-04-20 19:52:35.000000 mlops_api_gemstack-0.3/mlops_api_gemstack.egg-info/requires.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       19 2024-04-20 19:52:35.000000 mlops_api_gemstack-0.3/mlops_api_gemstack.egg-info/top_level.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       38 2024-04-20 19:52:35.649941 mlops_api_gemstack-0.3/setup.cfg
+-rw-r--r--   0 ricardosun   (501) staff       (20)      620 2024-04-20 19:52:30.000000 mlops_api_gemstack-0.3/setup.py
```

### Comparing `mlops_api_gemstack-0.2.1/mlops_api_gemstack/api.py` & `mlops_api_gemstack-0.3/mlops_api_gemstack/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -234,39 +234,40 @@
         click.echo(f"Permission denied: {file_path}")
     except Exception as e:
         click.echo(f"An error occurred: {e}")
 
 @cli.command()
 @click.argument('topics_file', type=click.Path(exists=True))
 @click.argument('rosbag_file_name')
+@click.argument('source')
 @click.option('--delete_rosbag', is_flag=True, help='Keep the rosbag file after recording')
-def record_rosbag(topics_file, rosbag_file_name, delete_rosbag):
+def record_rosbag(topics_file, rosbag_file_name, source, delete_rosbag):
 
     with open(topics_file) as f:
         topics = [line.strip() for line in f.readlines()]
 
     if not topics:
         print(f"No topics found in {topics_file}")
         exit(1)
     
     if not rosbag_file_name.endswith('.bag'):
         rosbag_file_name += '.bag'
 
     topics = " ".join(topics)
 
     command = f"rosbag record {topics} -O {rosbag_file_name}"
-    # command = "ping 127.0.0.1 -t"
 
     process = subprocess.Popen(command, shell=True)
 
     def stop_recording(sig, frame):
         print("Stopping rosbag recording")
         process.terminate()
         print("Recording stopped")
         # send rosbag file through api
+        dataset_uploadBag(rosbag_file_name, source)
         # Add to here
         if delete_rosbag:
             print("Removing rosbag file")
             subprocess.run(f"rm {rosbag_file_name}", shell=True)
         exit(0)
 
     signal.signal(signal.SIGINT, stop_recording)
```

### Comparing `mlops_api_gemstack-0.2.1/setup.py` & `mlops_api_gemstack-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mlops_api_gemstack',
-    version='0.2.1',
+    version='0.3',
     description='An API package connect to a MLops server relating to the GEMstack project.',
     author='Haoming Sun',
     author_email='ricardosun990122@gmail.com',
     url='https://github.com/krishauser/GEMstack/tree/s2024_MLops/MLops/mlops_api_gemstack',
     packages=find_packages(),
     install_requires=[
         'requests',
```

