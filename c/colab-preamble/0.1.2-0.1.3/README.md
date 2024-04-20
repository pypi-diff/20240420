# Comparing `tmp/colab-preamble-0.1.2.tar.gz` & `tmp/colab-preamble-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colab-preamble-0.1.2.tar", last modified: Tue Jan  9 04:17:39 2024, max compression
+gzip compressed data, was "colab-preamble-0.1.3.tar", last modified: Sat Apr 20 00:17:31 2024, max compression
```

## Comparing `colab-preamble-0.1.2.tar` & `colab-preamble-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 kota      (1000) kota      (1000)        0 2024-01-09 04:17:39.396224 colab-preamble-0.1.2/
--rw-rw-r--   0 kota      (1000) kota      (1000)     1066 2024-01-09 04:08:20.000000 colab-preamble-0.1.2/LICENSE
--rw-rw-r--   0 kota      (1000) kota      (1000)     1172 2024-01-09 04:17:39.396224 colab-preamble-0.1.2/PKG-INFO
--rw-rw-r--   0 kota      (1000) kota      (1000)      853 2024-01-09 04:16:43.000000 colab-preamble-0.1.2/README.md
-drwxrwxr-x   0 kota      (1000) kota      (1000)        0 2024-01-09 04:17:39.396224 colab-preamble-0.1.2/colab_preamble.egg-info/
--rw-rw-r--   0 kota      (1000) kota      (1000)     1172 2024-01-09 04:17:39.000000 colab-preamble-0.1.2/colab_preamble.egg-info/PKG-INFO
--rw-rw-r--   0 kota      (1000) kota      (1000)      233 2024-01-09 04:17:39.000000 colab-preamble-0.1.2/colab_preamble.egg-info/SOURCES.txt
--rw-rw-r--   0 kota      (1000) kota      (1000)        1 2024-01-09 04:17:39.000000 colab-preamble-0.1.2/colab_preamble.egg-info/dependency_links.txt
--rw-rw-r--   0 kota      (1000) kota      (1000)       36 2024-01-09 04:17:39.000000 colab-preamble-0.1.2/colab_preamble.egg-info/requires.txt
--rw-rw-r--   0 kota      (1000) kota      (1000)       15 2024-01-09 04:17:39.000000 colab-preamble-0.1.2/colab_preamble.egg-info/top_level.txt
--rw-rw-r--   0 kota      (1000) kota      (1000)      742 2024-01-09 04:01:29.000000 colab-preamble-0.1.2/colab_preamble.py
--rw-rw-r--   0 kota      (1000) kota      (1000)       38 2024-01-09 04:17:39.396224 colab-preamble-0.1.2/setup.cfg
--rw-rw-r--   0 kota      (1000) kota      (1000)      607 2024-01-09 04:17:22.000000 colab-preamble-0.1.2/setup.py
+drwxr-xr-x   0 km255052   (501) staff       (20)        0 2024-04-20 00:17:31.001753 colab-preamble-0.1.3/
+-rw-r--r--   0 km255052   (501) staff       (20)     1066 2024-04-20 00:14:13.000000 colab-preamble-0.1.3/LICENSE
+-rw-r--r--   0 km255052   (501) staff       (20)     1418 2024-04-20 00:17:31.001189 colab-preamble-0.1.3/PKG-INFO
+-rw-r--r--   0 km255052   (501) staff       (20)     1136 2024-04-20 00:14:13.000000 colab-preamble-0.1.3/README.md
+drwxr-xr-x   0 km255052   (501) staff       (20)        0 2024-04-20 00:17:31.000173 colab-preamble-0.1.3/colab_preamble.egg-info/
+-rw-r--r--   0 km255052   (501) staff       (20)     1418 2024-04-20 00:17:30.000000 colab-preamble-0.1.3/colab_preamble.egg-info/PKG-INFO
+-rw-r--r--   0 km255052   (501) staff       (20)      233 2024-04-20 00:17:30.000000 colab-preamble-0.1.3/colab_preamble.egg-info/SOURCES.txt
+-rw-r--r--   0 km255052   (501) staff       (20)        1 2024-04-20 00:17:30.000000 colab-preamble-0.1.3/colab_preamble.egg-info/dependency_links.txt
+-rw-r--r--   0 km255052   (501) staff       (20)       36 2024-04-20 00:17:30.000000 colab-preamble-0.1.3/colab_preamble.egg-info/requires.txt
+-rw-r--r--   0 km255052   (501) staff       (20)       15 2024-04-20 00:17:30.000000 colab-preamble-0.1.3/colab_preamble.egg-info/top_level.txt
+-rw-r--r--   0 km255052   (501) staff       (20)      753 2024-04-20 00:15:32.000000 colab-preamble-0.1.3/colab_preamble.py
+-rw-r--r--   0 km255052   (501) staff       (20)       38 2024-04-20 00:17:31.001912 colab-preamble-0.1.3/setup.cfg
+-rw-r--r--   0 km255052   (501) staff       (20)      607 2024-04-20 00:16:55.000000 colab-preamble-0.1.3/setup.py
```

### Comparing `colab-preamble-0.1.2/LICENSE` & `colab-preamble-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `colab-preamble-0.1.2/PKG-INFO` & `colab-preamble-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 Metadata-Version: 2.1
 Name: colab-preamble
-Version: 0.1.2
+Version: 0.1.3
 Summary: Prepare google colabpratory by one line of command
 Home-page: https://github.com/kota7/colab-preamble
 Author: Kota Mori
 Author-email: kmori05@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# COLAB PREAMPLE
+# COLAB PREAMBLE
 Prepare google colaboratory by one line of command
 
+[![](https://badge.fury.io/py/colab-preamble.svg)](https://badge.fury.io/py/colab-preamble)
+
+
 ## Installation
 
 ```python
 # from pypi
 $ pip install colab-preamble
 
 # alternatively, from github
 $ git clone https://github.com/kota7/colab-preamble --depth 1
-$ pip install -U ./colab-preample
+$ pip install -U ./colab-preamble
 ```
 
+## Example
+
+Example colab notebook is here: [colab-preamble-example.ipynb](https://colab.research.google.com/drive/1CD_tZTP5eDRYe0u8ZchuLlEYHjCDJOYw?usp=sharing)
 
 ## Usage
 
 ```python
 import colab_preamble
 
-colab_preample_run(google_cloud_project="<project-id>", mount_drive=True)
+colab_preamble_run(google_cloud_project="<project-id>", mount_drive=True)
 # If no need to access google cloud services, no need to provide set google_cloud_project=None
 # If no need to mount google drive, set mount_drive=False
 ```
 
 ## Effect
 
 When `google_cloud_project` is given,
 
 - Set the default project ID
     - Run `gcloud config set ...`
-    - Set `GOOGLE_CLOUD_PROJECT` env variable
+    - Set `GOOGLE_CLOUD_PROJECT` environment variable
 - Open the authentication prompt
 - Introduce bigquery magic command `bq`
 
 
 When `mount_drive` is true,
 
-- Google drive is mounted at '/content/drive'
-
-
+- Open the prompt and mount the google drive at '/content/drive'
```

### Comparing `colab-preamble-0.1.2/README.md` & `colab-preamble-0.1.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,45 @@
-# COLAB PREAMPLE
+# COLAB PREAMBLE
 Prepare google colaboratory by one line of command
 
+[![](https://badge.fury.io/py/colab-preamble.svg)](https://badge.fury.io/py/colab-preamble)
+
+
 ## Installation
 
 ```python
 # from pypi
 $ pip install colab-preamble
 
 # alternatively, from github
 $ git clone https://github.com/kota7/colab-preamble --depth 1
-$ pip install -U ./colab-preample
+$ pip install -U ./colab-preamble
 ```
 
+## Example
+
+Example colab notebook is here: [colab-preamble-example.ipynb](https://colab.research.google.com/drive/1CD_tZTP5eDRYe0u8ZchuLlEYHjCDJOYw?usp=sharing)
 
 ## Usage
 
 ```python
 import colab_preamble
 
-colab_preample_run(google_cloud_project="<project-id>", mount_drive=True)
+colab_preamble_run(google_cloud_project="<project-id>", mount_drive=True)
 # If no need to access google cloud services, no need to provide set google_cloud_project=None
 # If no need to mount google drive, set mount_drive=False
 ```
 
 ## Effect
 
 When `google_cloud_project` is given,
 
 - Set the default project ID
     - Run `gcloud config set ...`
-    - Set `GOOGLE_CLOUD_PROJECT` env variable
+    - Set `GOOGLE_CLOUD_PROJECT` environment variable
 - Open the authentication prompt
 - Introduce bigquery magic command `bq`
 
 
 When `mount_drive` is true,
 
-- Google drive is mounted at '/content/drive'
+- Open the prompt and mount the google drive at '/content/drive'
```

### Comparing `colab-preamble-0.1.2/colab_preamble.egg-info/PKG-INFO` & `colab-preamble-0.1.3/colab_preamble.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 Metadata-Version: 2.1
 Name: colab-preamble
-Version: 0.1.2
+Version: 0.1.3
 Summary: Prepare google colabpratory by one line of command
 Home-page: https://github.com/kota7/colab-preamble
 Author: Kota Mori
 Author-email: kmori05@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# COLAB PREAMPLE
+# COLAB PREAMBLE
 Prepare google colaboratory by one line of command
 
+[![](https://badge.fury.io/py/colab-preamble.svg)](https://badge.fury.io/py/colab-preamble)
+
+
 ## Installation
 
 ```python
 # from pypi
 $ pip install colab-preamble
 
 # alternatively, from github
 $ git clone https://github.com/kota7/colab-preamble --depth 1
-$ pip install -U ./colab-preample
+$ pip install -U ./colab-preamble
 ```
 
+## Example
+
+Example colab notebook is here: [colab-preamble-example.ipynb](https://colab.research.google.com/drive/1CD_tZTP5eDRYe0u8ZchuLlEYHjCDJOYw?usp=sharing)
 
 ## Usage
 
 ```python
 import colab_preamble
 
-colab_preample_run(google_cloud_project="<project-id>", mount_drive=True)
+colab_preamble_run(google_cloud_project="<project-id>", mount_drive=True)
 # If no need to access google cloud services, no need to provide set google_cloud_project=None
 # If no need to mount google drive, set mount_drive=False
 ```
 
 ## Effect
 
 When `google_cloud_project` is given,
 
 - Set the default project ID
     - Run `gcloud config set ...`
-    - Set `GOOGLE_CLOUD_PROJECT` env variable
+    - Set `GOOGLE_CLOUD_PROJECT` environment variable
 - Open the authentication prompt
 - Introduce bigquery magic command `bq`
 
 
 When `mount_drive` is true,
 
-- Google drive is mounted at '/content/drive'
-
-
+- Open the prompt and mount the google drive at '/content/drive'
```

### Comparing `colab-preamble-0.1.2/colab_preamble.py` & `colab-preamble-0.1.3/colab_preamble.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 def run(google_cloud_project: str=None, mount_drive: bool=True):
     if mount_drive:
         print("Mounting google drive...", file=sys.stderr)
         drive.mount('/content/drive')        
 
     if google_cloud_project is not None:
         print(f"Setting default google cloud project as {google_cloud_project}...", file=sys.stderr)
-        subprocess.run(["gcloud", "config", "set", google_cloud_project])
+        subprocess.run(["gcloud", "config", "set", "project", google_cloud_project])
         os.environ["GOOGLE_CLOUD_PROJECT"] = google_cloud_project
         print(f"Authenticating user...", file=sys.stderr)
         auth.authenticate_user()
 
         print("To use bigquery magic, try:\n\n%load_ext bq\n%bq SELECT 1")
```

### Comparing `colab-preamble-0.1.2/setup.py` & `colab-preamble-0.1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 readmefile = os.path.join(os.path.dirname(__file__), "README.md")
 with open(readmefile) as f:
     readme = f.read()
 
 setup(
     name='colab-preamble',
-    version="0.1.2",
+    version="0.1.3",
     description='Prepare google colabpratory by one line of command',
     author='Kota Mori', 
     author_email='kmori05@gmail.com',
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://github.com/kota7/colab-preamble',
```

