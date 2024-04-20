# Comparing `tmp/deksecrets-0.1.4.tar.gz` & `tmp/deksecrets-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deksecrets-0.1.4.tar", last modified: Thu Feb 29 20:08:00 2024, max compression
+gzip compressed data, was "deksecrets-0.1.5.tar", last modified: Fri Mar  1 18:14:45 2024, max compression
```

## Comparing `deksecrets-0.1.4.tar` & `deksecrets-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-02-29 20:07:58.496745 deksecrets-0.1.4/README.md
--rw-r--r--   0        0        0      201 2024-02-29 20:07:58.496745 deksecrets-0.1.4/deksecrets/click/__entry__.py
--rw-r--r--   0        0        0       54 2024-02-29 20:07:58.496745 deksecrets-0.1.4/deksecrets/click/__init__.py
--rw-r--r--   0        0        0      891 2024-02-29 20:07:58.496745 deksecrets-0.1.4/deksecrets/click/infisical.py
--rw-r--r--   0        0        0      705 2024-02-29 20:07:58.496745 deksecrets-0.1.4/deksecrets/click/k8s.py
--rw-r--r--   0        0        0        0 2024-02-29 20:07:58.496745 deksecrets-0.1.4/deksecrets/tools/__init__.py
--rw-r--r--   0        0        0      573 2024-02-29 20:07:58.496745 deksecrets-0.1.4/deksecrets/tools/infisical.py
--rw-r--r--   0        0        0      487 2024-02-29 20:08:00.464935 deksecrets-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      246 1970-01-01 00:00:00.000000 deksecrets-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-01 18:14:43.578531 deksecrets-0.1.5/README.md
+-rw-r--r--   0        0        0      201 2024-03-01 18:14:43.578531 deksecrets-0.1.5/deksecrets/click/__entry__.py
+-rw-r--r--   0        0        0       54 2024-03-01 18:14:43.578531 deksecrets-0.1.5/deksecrets/click/__init__.py
+-rw-r--r--   0        0        0     1254 2024-03-01 18:14:43.578531 deksecrets-0.1.5/deksecrets/click/infisical.py
+-rw-r--r--   0        0        0      705 2024-03-01 18:14:43.578531 deksecrets-0.1.5/deksecrets/click/k8s.py
+-rw-r--r--   0        0        0        0 2024-03-01 18:14:43.578531 deksecrets-0.1.5/deksecrets/tools/__init__.py
+-rw-r--r--   0        0        0      573 2024-03-01 18:14:43.578531 deksecrets-0.1.5/deksecrets/tools/infisical.py
+-rw-r--r--   0        0        0      487 2024-03-01 18:14:45.126561 deksecrets-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      246 1970-01-01 00:00:00.000000 deksecrets-0.1.5/PKG-INFO
```

### Comparing `deksecrets-0.1.4/deksecrets/click/infisical.py` & `deksecrets-0.1.5/deksecrets/click/infisical.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,25 @@
 from dektools.file import write_file
 from ..tools.infisical import fetch_secrets
 
 app = typer.Typer(add_completion=False)
 
 
 @app.command()
-def env(site_url, client_id, project, environment, path=None, out=None, client_secret=None, fmt=None):
+def fetch(site_url, client_id, project, environment, path=None, out=None, client_secret=None, fmt=None):
+    _fetch(site_url, client_id, client_secret, project, environment, path, out, fmt)
+
+
+@app.command()
+def fetch_shortcut(url, out=None, fmt=None):
+    site_url, client_id, client_secret, project, environment, path = url.split('@')
+    _fetch(site_url, client_id, client_secret, project, environment, path, out, fmt)
+
+
+def _fetch(site_url, client_id, client_secret, project, environment, path, out, fmt):
     if not client_secret:
         client_secret = getpass('Please input ClientSecret:')
     data = fetch_secrets(site_url, client_id, client_secret, project, environment, path)
     fmt = fmt or 'env'
     if fmt == 'env':
         s = "\n".join(f'{k}="{v}"' for k, v in data.items())
     elif fmt == 'json':
@@ -21,12 +31,7 @@
     else:
         raise TypeError(f'Please provide a correct format: {fmt}')
     if out:
         write_file(out, s=s)
     else:
         out = write_file(f'.{fmt}', s=s, t=True)
         sys.stdout.write(out)
-
-
-@app.callback()
-def callback():
-    pass
```

### Comparing `deksecrets-0.1.4/deksecrets/click/k8s.py` & `deksecrets-0.1.5/deksecrets/click/k8s.py`

 * *Files identical despite different names*

### Comparing `deksecrets-0.1.4/deksecrets/tools/infisical.py` & `deksecrets-0.1.5/deksecrets/tools/infisical.py`

 * *Files identical despite different names*

