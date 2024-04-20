# Comparing `tmp/fastapi-easyauth-0.0.3.tar.gz` & `tmp/fastapi-easyauth-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-easyauth-0.0.3.tar", last modified: Fri Apr 12 17:11:10 2024, max compression
+gzip compressed data, was "fastapi-easyauth-0.1.0.tar", last modified: Sat Apr 20 18:24:31 2024, max compression
```

## Comparing `fastapi-easyauth-0.0.3.tar` & `fastapi-easyauth-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 dmitrijtrejgo   (501) staff       (20)        0 2024-04-12 17:11:10.005113 fastapi-easyauth-0.0.3/
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     3145 2024-04-12 17:11:10.005182 fastapi-easyauth-0.0.3/PKG-INFO
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     2565 2024-04-12 17:07:46.000000 fastapi-easyauth-0.0.3/README.md
-drwxr-xr-x   0 dmitrijtrejgo   (501) staff       (20)        0 2024-04-12 17:11:10.004281 fastapi-easyauth-0.0.3/fastapi_easyauth/
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)       73 2024-04-12 17:07:32.000000 fastapi-easyauth-0.0.3/fastapi_easyauth/__init__.py
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     1305 2024-04-12 17:07:32.000000 fastapi-easyauth-0.0.3/fastapi_easyauth/easyauth.py
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)      233 2024-04-12 17:07:32.000000 fastapi-easyauth-0.0.3/fastapi_easyauth/exp.py
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     3287 2024-04-12 17:07:32.000000 fastapi-easyauth-0.0.3/fastapi_easyauth/jwt.py
-drwxr-xr-x   0 dmitrijtrejgo   (501) staff       (20)        0 2024-04-12 17:11:10.005012 fastapi-easyauth-0.0.3/fastapi_easyauth.egg-info/
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     3145 2024-04-12 17:11:09.000000 fastapi-easyauth-0.0.3/fastapi_easyauth.egg-info/PKG-INFO
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)      333 2024-04-12 17:11:09.000000 fastapi-easyauth-0.0.3/fastapi_easyauth.egg-info/SOURCES.txt
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)        1 2024-04-12 17:11:09.000000 fastapi-easyauth-0.0.3/fastapi_easyauth.egg-info/dependency_links.txt
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)       29 2024-04-12 17:11:09.000000 fastapi-easyauth-0.0.3/fastapi_easyauth.egg-info/requires.txt
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)       17 2024-04-12 17:11:09.000000 fastapi-easyauth-0.0.3/fastapi_easyauth.egg-info/top_level.txt
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)       38 2024-04-12 17:11:10.005387 fastapi-easyauth-0.0.3/setup.cfg
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)      885 2024-04-12 17:10:44.000000 fastapi-easyauth-0.0.3/setup.py
+drwxr-xr-x   0 dmitrijtrejgo   (501) staff       (20)        0 2024-04-20 18:24:31.693894 fastapi-easyauth-0.1.0/
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     4136 2024-04-20 18:24:31.693962 fastapi-easyauth-0.1.0/PKG-INFO
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     3556 2024-04-20 17:33:30.000000 fastapi-easyauth-0.1.0/README.md
+drwxr-xr-x   0 dmitrijtrejgo   (501) staff       (20)        0 2024-04-20 18:24:31.693099 fastapi-easyauth-0.1.0/fastapi_easyauth/
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)      111 2024-04-20 16:51:52.000000 fastapi-easyauth-0.1.0/fastapi_easyauth/__init__.py
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     3999 2024-04-20 16:44:35.000000 fastapi-easyauth-0.1.0/fastapi_easyauth/easyauth.py
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)      296 2024-04-20 11:39:28.000000 fastapi-easyauth-0.1.0/fastapi_easyauth/exp.py
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     5489 2024-04-20 16:44:52.000000 fastapi-easyauth-0.1.0/fastapi_easyauth/jwt.py
+drwxr-xr-x   0 dmitrijtrejgo   (501) staff       (20)        0 2024-04-20 18:24:31.693775 fastapi-easyauth-0.1.0/fastapi_easyauth.egg-info/
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     4136 2024-04-20 18:24:31.000000 fastapi-easyauth-0.1.0/fastapi_easyauth.egg-info/PKG-INFO
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)      333 2024-04-20 18:24:31.000000 fastapi-easyauth-0.1.0/fastapi_easyauth.egg-info/SOURCES.txt
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)        1 2024-04-20 18:24:31.000000 fastapi-easyauth-0.1.0/fastapi_easyauth.egg-info/dependency_links.txt
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)       29 2024-04-20 18:24:31.000000 fastapi-easyauth-0.1.0/fastapi_easyauth.egg-info/requires.txt
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)       17 2024-04-20 18:24:31.000000 fastapi-easyauth-0.1.0/fastapi_easyauth.egg-info/top_level.txt
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)       38 2024-04-20 18:24:31.694157 fastapi-easyauth-0.1.0/setup.cfg
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)      885 2024-04-20 17:35:45.000000 fastapi-easyauth-0.1.0/setup.py
```

### Comparing `fastapi-easyauth-0.0.3/setup.py` & `fastapi-easyauth-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 
 setup(
   name='fastapi-easyauth',
-  version='0.0.3',
+  version='0.1.0',
   author='duckduck',
   author_email='dimondtp@gmail.com',
   description='A library for quickly creating authentication using JWT and Cookies',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Trejgus/fastapi-easyauth',
   packages=find_packages(),
```

