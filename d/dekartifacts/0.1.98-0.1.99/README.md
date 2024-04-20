# Comparing `tmp/dekartifacts-0.1.98.tar.gz` & `tmp/dekartifacts-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dekartifacts-0.1.98.tar", last modified: Wed Feb 28 14:49:30 2024, max compression
+gzip compressed data, was "dekartifacts-0.1.99.tar", last modified: Thu Feb 29 08:20:14 2024, max compression
```

## Comparing `dekartifacts-0.1.98.tar` & `dekartifacts-0.1.99.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2024-02-28 14:49:28.705762 dekartifacts-0.1.98/README.md
--rw-r--r--   0        0        0        0 2024-02-28 14:49:28.705762 dekartifacts-0.1.98/dekartifacts/allinone/__init__.py
--rw-r--r--   0        0        0     1443 2024-02-28 14:49:28.705762 dekartifacts-0.1.98/dekartifacts/allinone/base/__init__.py
--rw-r--r--   0        0        0     1233 2024-02-28 14:49:28.705762 dekartifacts-0.1.98/dekartifacts/allinone/docker.py
--rw-r--r--   0        0        0     2432 2024-02-28 14:49:28.705762 dekartifacts-0.1.98/dekartifacts/allinone/helm.py
--rw-r--r--   0        0        0     1743 2024-02-28 14:49:28.705762 dekartifacts-0.1.98/dekartifacts/allinone/staticfiles.py
--rw-r--r--   0        0        0        0 2024-02-28 14:49:28.705762 dekartifacts-0.1.98/dekartifacts/artifacts/__init__.py
--rw-r--r--   0        0        0     3063 2024-02-28 14:49:28.705762 dekartifacts-0.1.98/dekartifacts/artifacts/base/__init__.py
--rw-r--r--   0        0        0    10399 2024-02-28 14:49:28.705762 dekartifacts-0.1.98/dekartifacts/artifacts/docker.py
--rw-r--r--   0        0        0     9111 2024-02-28 14:49:28.705762 dekartifacts-0.1.98/dekartifacts/artifacts/helm.py
--rw-r--r--   0        0        0     1166 2024-02-28 14:49:28.705762 dekartifacts-0.1.98/dekartifacts/artifacts/staticfiles.py
--rw-r--r--   0        0        0      118 2024-02-28 14:49:28.705762 dekartifacts-0.1.98/dekartifacts/click/__entry__.py
--rw-r--r--   0        0        0       54 2024-02-28 14:49:28.709762 dekartifacts-0.1.98/dekartifacts/click/__init__.py
--rw-r--r--   0        0        0     1746 2024-02-28 14:49:28.709762 dekartifacts-0.1.98/dekartifacts/click/image.py
--rw-r--r--   0        0        0        0 2024-02-28 14:49:28.709762 dekartifacts-0.1.98/dekartifacts/tools/__init__.py
--rw-r--r--   0        0        0     1391 2024-02-28 14:49:28.709762 dekartifacts-0.1.98/dekartifacts/tools/helm.py
--rw-r--r--   0        0        0      465 2024-02-28 14:49:30.245783 dekartifacts-0.1.98/pyproject.toml
--rw-r--r--   0        0        0      210 1970-01-01 00:00:00.000000 dekartifacts-0.1.98/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-29 08:20:12.400828 dekartifacts-0.1.99/README.md
+-rw-r--r--   0        0        0        0 2024-02-29 08:20:12.400828 dekartifacts-0.1.99/dekartifacts/allinone/__init__.py
+-rw-r--r--   0        0        0     1443 2024-02-29 08:20:12.400828 dekartifacts-0.1.99/dekartifacts/allinone/base/__init__.py
+-rw-r--r--   0        0        0     1233 2024-02-29 08:20:12.400828 dekartifacts-0.1.99/dekartifacts/allinone/docker.py
+-rw-r--r--   0        0        0     2432 2024-02-29 08:20:12.400828 dekartifacts-0.1.99/dekartifacts/allinone/helm.py
+-rw-r--r--   0        0        0     1743 2024-02-29 08:20:12.400828 dekartifacts-0.1.99/dekartifacts/allinone/staticfiles.py
+-rw-r--r--   0        0        0        0 2024-02-29 08:20:12.400828 dekartifacts-0.1.99/dekartifacts/artifacts/__init__.py
+-rw-r--r--   0        0        0     3063 2024-02-29 08:20:12.404828 dekartifacts-0.1.99/dekartifacts/artifacts/base/__init__.py
+-rw-r--r--   0        0        0    10634 2024-02-29 08:20:12.404828 dekartifacts-0.1.99/dekartifacts/artifacts/docker.py
+-rw-r--r--   0        0        0     9139 2024-02-29 08:20:12.404828 dekartifacts-0.1.99/dekartifacts/artifacts/helm.py
+-rw-r--r--   0        0        0     1166 2024-02-29 08:20:12.404828 dekartifacts-0.1.99/dekartifacts/artifacts/staticfiles.py
+-rw-r--r--   0        0        0      118 2024-02-29 08:20:12.404828 dekartifacts-0.1.99/dekartifacts/click/__entry__.py
+-rw-r--r--   0        0        0       54 2024-02-29 08:20:12.404828 dekartifacts-0.1.99/dekartifacts/click/__init__.py
+-rw-r--r--   0        0        0     1746 2024-02-29 08:20:12.404828 dekartifacts-0.1.99/dekartifacts/click/image.py
+-rw-r--r--   0        0        0        0 2024-02-29 08:20:12.404828 dekartifacts-0.1.99/dekartifacts/tools/__init__.py
+-rw-r--r--   0        0        0     1391 2024-02-29 08:20:12.404828 dekartifacts-0.1.99/dekartifacts/tools/helm.py
+-rw-r--r--   0        0        0      465 2024-02-29 08:20:14.388862 dekartifacts-0.1.99/pyproject.toml
+-rw-r--r--   0        0        0      210 1970-01-01 00:00:00.000000 dekartifacts-0.1.99/PKG-INFO
```

### Comparing `dekartifacts-0.1.98/dekartifacts/allinone/base/__init__.py` & `dekartifacts-0.1.99/dekartifacts/allinone/base/__init__.py`

 * *Files identical despite different names*

### Comparing `dekartifacts-0.1.98/dekartifacts/allinone/docker.py` & `dekartifacts-0.1.99/dekartifacts/allinone/docker.py`

 * *Files identical despite different names*

### Comparing `dekartifacts-0.1.98/dekartifacts/allinone/helm.py` & `dekartifacts-0.1.99/dekartifacts/allinone/helm.py`

 * *Files identical despite different names*

### Comparing `dekartifacts-0.1.98/dekartifacts/allinone/staticfiles.py` & `dekartifacts-0.1.99/dekartifacts/allinone/staticfiles.py`

 * *Files identical despite different names*

### Comparing `dekartifacts-0.1.98/dekartifacts/artifacts/base/__init__.py` & `dekartifacts-0.1.99/dekartifacts/artifacts/base/__init__.py`

 * *Files identical despite different names*

### Comparing `dekartifacts-0.1.98/dekartifacts/artifacts/docker.py` & `dekartifacts-0.1.99/dekartifacts/artifacts/docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,22 @@
     typed = 'docker'
     cli_list = ['docker', 'nerdctl', 'podman']
 
     image_tag_max_length = 128
     registry_standard = 'docker.io'
 
     @classmethod
+    def login_all_env(cls, prepare=True):
+        da = cls()
+        for registry in da.list_env_registries():
+            da.login(**da.get_env_kwargs(registry))
+            if prepare:
+                cls.prepare()
+
+    @classmethod
     def login(cls, registry='', username='', password=''):
         print(F"Login to {registry} {username[0]}***{username[-1]}")
         ret, _, err = shell_with_input(f'{cls.cli} login {registry} -u {username} --password-stdin', password)
         if ret:
             for mark in [b'net/http: TLS handshake timeout']:
                 if mark in err:
                     shell_wrapper('sleep 1')
```

### Comparing `dekartifacts-0.1.98/dekartifacts/artifacts/helm.py` & `dekartifacts-0.1.99/dekartifacts/artifacts/helm.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,16 @@
         ah = ArtifactHelm()
         artifacts = {}
         for registry in ah.list_env_registries():
             kwargs = ah.get_env_kwargs(registry)
             cls = get_artifact_helm_by_url(kwargs['registry'])
             artifact = artifacts[cls] = cls()
             artifact.login(**kwargs)
-            cls.prepare()
+            if prepare:
+                cls.prepare()
         return artifacts
 
 
 class HelmCommonArtifact(ArtifactHelm):
     @classmethod
     def recognize(cls, url):  # https://localhost/path-before-index--yaml::chart-name:version
         return True
```

### Comparing `dekartifacts-0.1.98/dekartifacts/artifacts/staticfiles.py` & `dekartifacts-0.1.99/dekartifacts/artifacts/staticfiles.py`

 * *Files identical despite different names*

### Comparing `dekartifacts-0.1.98/dekartifacts/click/image.py` & `dekartifacts-0.1.99/dekartifacts/click/image.py`

 * *Files identical despite different names*

### Comparing `dekartifacts-0.1.98/dekartifacts/tools/helm.py` & `dekartifacts-0.1.99/dekartifacts/tools/helm.py`

 * *Files identical despite different names*

