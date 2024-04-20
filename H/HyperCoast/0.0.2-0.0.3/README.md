# Comparing `tmp/hypercoast-0.0.2.tar.gz` & `tmp/hypercoast-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypercoast-0.0.2.tar", last modified: Fri Apr 19 02:49:14 2024, max compression
+gzip compressed data, was "hypercoast-0.0.3.tar", last modified: Sat Apr 20 15:28:00 2024, max compression
```

## Comparing `hypercoast-0.0.2.tar` & `hypercoast-0.0.3.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:49:14.861634 hypercoast-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:49:14.853634 hypercoast-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:49:14.857634 hypercoast-0.0.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:49:14.857634 hypercoast-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-19 02:49:01.000000 hypercoast-0.0.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:49:14.861634 hypercoast-0.0.2/HyperCoast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-19 02:49:14.000000 hypercoast-0.0.2/HyperCoast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-19 02:49:14.000000 hypercoast-0.0.2/HyperCoast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 02:49:14.000000 hypercoast-0.0.2/HyperCoast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-19 02:49:14.000000 hypercoast-0.0.2/HyperCoast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 02:49:14.000000 hypercoast-0.0.2/HyperCoast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 02:49:14.000000 hypercoast-0.0.2/HyperCoast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-19 02:49:01.000000 hypercoast-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-19 02:49:01.000000 hypercoast-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-19 02:49:14.861634 hypercoast-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-19 02:49:01.000000 hypercoast-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:49:14.861634 hypercoast-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 02:49:01.000000 hypercoast-0.0.2/docs/CNAME
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-19 02:49:01.000000 hypercoast-0.0.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 02:49:01.000000 hypercoast-0.0.2/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-19 02:49:01.000000 hypercoast-0.0.2/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:49:14.861634 hypercoast-0.0.2/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-19 02:49:01.000000 hypercoast-0.0.2/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 02:49:01.000000 hypercoast-0.0.2/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 02:49:01.000000 hypercoast-0.0.2/docs/hypercoast.md
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-19 02:49:01.000000 hypercoast-0.0.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-19 02:49:01.000000 hypercoast-0.0.2/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:49:14.861634 hypercoast-0.0.2/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 02:49:01.000000 hypercoast-0.0.2/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-19 02:49:01.000000 hypercoast-0.0.2/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:49:14.861634 hypercoast-0.0.2/hypercoast/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-19 02:49:01.000000 hypercoast-0.0.2/hypercoast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-19 02:49:01.000000 hypercoast-0.0.2/hypercoast/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-19 02:49:01.000000 hypercoast-0.0.2/hypercoast/hypercoast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-19 02:49:01.000000 hypercoast-0.0.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-19 02:49:01.000000 hypercoast-0.0.2/pyproject-codespell.precommit-toml
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-19 02:49:01.000000 hypercoast-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 02:49:01.000000 hypercoast-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-19 02:49:01.000000 hypercoast-0.0.2/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 02:49:14.861634 hypercoast-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:49:14.861634 hypercoast-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 02:49:01.000000 hypercoast-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-19 02:49:01.000000 hypercoast-0.0.2/tests/test_hypercoast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:00.765577 hypercoast-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:00.753577 hypercoast-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:00.757577 hypercoast-0.0.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:00.757577 hypercoast-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:00.765577 hypercoast-0.0.3/HyperCoast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-20 15:28:00.000000 hypercoast-0.0.3/HyperCoast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-20 15:28:00.000000 hypercoast-0.0.3/HyperCoast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 15:28:00.000000 hypercoast-0.0.3/HyperCoast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-20 15:28:00.000000 hypercoast-0.0.3/HyperCoast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-20 15:28:00.000000 hypercoast-0.0.3/HyperCoast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-20 15:28:00.000000 hypercoast-0.0.3/HyperCoast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-20 15:27:50.000000 hypercoast-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-20 15:27:50.000000 hypercoast-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-20 15:28:00.765577 hypercoast-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-20 15:27:50.000000 hypercoast-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:00.761577 hypercoast-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-20 15:27:50.000000 hypercoast-0.0.3/docs/CNAME
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-20 15:27:50.000000 hypercoast-0.0.3/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 15:27:50.000000 hypercoast-0.0.3/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-20 15:27:50.000000 hypercoast-0.0.3/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-20 15:27:50.000000 hypercoast-0.0.3/docs/emit.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:00.761577 hypercoast-0.0.3/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-20 15:27:50.000000 hypercoast-0.0.3/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-20 15:27:50.000000 hypercoast-0.0.3/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-20 15:27:50.000000 hypercoast-0.0.3/docs/hypercoast.md
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-20 15:27:50.000000 hypercoast-0.0.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-20 15:27:50.000000 hypercoast-0.0.3/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:00.761577 hypercoast-0.0.3/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-20 15:27:50.000000 hypercoast-0.0.3/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-20 15:27:50.000000 hypercoast-0.0.3/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:00.765577 hypercoast-0.0.3/hypercoast/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-20 15:27:50.000000 hypercoast-0.0.3/hypercoast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-20 15:27:50.000000 hypercoast-0.0.3/hypercoast/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37734 2024-04-20 15:27:50.000000 hypercoast-0.0.3/hypercoast/emit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-20 15:27:50.000000 hypercoast-0.0.3/hypercoast/hypercoast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-20 15:27:50.000000 hypercoast-0.0.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-20 15:27:50.000000 hypercoast-0.0.3/pyproject-codespell.precommit-toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-20 15:27:50.000000 hypercoast-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-20 15:27:50.000000 hypercoast-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-20 15:27:50.000000 hypercoast-0.0.3/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 15:28:00.765577 hypercoast-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:00.765577 hypercoast-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-20 15:27:50.000000 hypercoast-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-20 15:27:50.000000 hypercoast-0.0.3/tests/test_hypercoast.py
```

### Comparing `hypercoast-0.0.2/.github/workflows/docs-build.yml` & `hypercoast-0.0.3/.github/workflows/docs-build.yml`

 * *Files 7% similar despite different names*

```diff
@@ -31,22 +31,22 @@
                   pip install .
             - name: PKG-TEST
               run: |
                   python -m unittest discover tests/
             - name: Build docs
               run: |
                   mkdocs build
-            # - name: Deploy to Netlify
-            #   uses: nwtgck/actions-netlify@v2.0
-            #   with:
-            #       publish-dir: "./site"
-            #       production-branch: main
+            - name: Deploy to Netlify
+              uses: nwtgck/actions-netlify@v2.0
+              with:
+                  publish-dir: "./site"
+                  production-branch: main
 
-            #       github-token: ${{ secrets.GITHUB_TOKEN }}
-            #       deploy-message: "Deploy from GitHub Actions"
-            #       enable-pull-request-comment: true
-            #       enable-commit-comment: false
-            #       overwrites-pull-request-comment: true
-            #   env:
-            #       NETLIFY_AUTH_TOKEN: ${{ secrets.NETLIFY_AUTH_TOKEN }}
-            #       NETLIFY_SITE_ID: ${{ secrets.NETLIFY_SITE_ID }}
-            #   timeout-minutes: 10
+                  github-token: ${{ secrets.GITHUB_TOKEN }}
+                  deploy-message: "Deploy from GitHub Actions"
+                  enable-pull-request-comment: true
+                  enable-commit-comment: false
+                  overwrites-pull-request-comment: true
+              env:
+                  NETLIFY_AUTH_TOKEN: ${{ secrets.NETLIFY_AUTH_TOKEN }}
+                  NETLIFY_SITE_ID: ${{ secrets.NETLIFY_SITE_ID }}
+              timeout-minutes: 10
```

### Comparing `hypercoast-0.0.2/.github/workflows/docs.yml` & `hypercoast-0.0.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.0.2/.github/workflows/installation.yml` & `hypercoast-0.0.3/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.0.2/.github/workflows/macos.yml` & `hypercoast-0.0.3/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.0.2/.github/workflows/pypi.yml` & `hypercoast-0.0.3/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.0.2/.github/workflows/ubuntu.yml` & `hypercoast-0.0.3/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.0.2/.github/workflows/windows.yml` & `hypercoast-0.0.3/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.0.2/.gitignore` & `hypercoast-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `hypercoast-0.0.2/.pre-commit-config.yaml` & `hypercoast-0.0.3/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 
     - repo: https://github.com/psf/black
       rev: 24.4.0
       hooks:
           - id: black-jupyter
             language_version: python3.11
 
-    - repo: https://github.com/codespell-project/codespell
-      rev: v2.2.6
-      hooks:
-          - id: codespell
-            args: [--toml, pyproject-codespell.precommit-toml]
+    # - repo: https://github.com/codespell-project/codespell
+    #   rev: v2.2.6
+    #   hooks:
+    #       - id: codespell
+    #         args: [--toml, pyproject-codespell.precommit-toml]
 
     - repo: https://github.com/kynan/nbstripout
       rev: 0.7.1
       hooks:
           - id: nbstripout
```

### Comparing `hypercoast-0.0.2/HyperCoast.egg-info/PKG-INFO` & `hypercoast-0.0.3/HyperCoast.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: HyperCoast
-Version: 0.0.2
-Summary: A Python package for processing hyperspetral data in coastal regions
+Version: 0.0.3
+Summary: A Python package for processing hyperspectral data in coastal regions
 Author-email: Qiusheng Wu <giswqs@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/opengeos/HyperCoast
 Keywords: HyperCoast
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -13,29 +13,36 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: geopandas
+Requires-Dist: hvplot
 Requires-Dist: leafmap
+Requires-Dist: localtileserver
+Requires-Dist: netcdf4
 Requires-Dist: numpy
+Requires-Dist: xarray
 Provides-Extra: all
 Requires-Dist: HyperCoast[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # HyperCoast
 
 [![image](https://img.shields.io/pypi/v/HyperCoast.svg)](https://pypi.python.org/pypi/HyperCoast)
-[![image](https://img.shields.io/conda/vn/conda-forge/HyperCoast.svg)](https://anaconda.org/conda-forge/HyperCoast)
+[![image](https://static.pepy.tech/badge/hypercoast)](https://pepy.tech/project/hypercoast)
+[![image](https://img.shields.io/conda/vn/conda-forge/hypercoast.svg)](https://anaconda.org/conda-forge/hypercoast)
+[![Conda Recipe](https://img.shields.io/badge/recipe-hypercoast-green.svg)](https://github.com/conda-forge/hypercoast-feedstock)
+[![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/hypercoast.svg)](https://anaconda.org/conda-forge/hypercoast)
 
-**A Python package for processing hyperspetral data in coastal regions**
+**A Python package for visualizing and analyzing hyperspectral data in coastal regions**
 
 -   Free software: MIT License
--   Documentation: https://hypercoast.org
+-   Documentation: <https://hypercoast.org>
 
 ## Features
 
--  Visualize hyperspectral data
--  Analyze hypersepctral data
-
+-   Visualize hyperspectral data
+-   Analyze hyperspectral data
```

### Comparing `hypercoast-0.0.2/HyperCoast.egg-info/SOURCES.txt` & `hypercoast-0.0.3/HyperCoast.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -25,19 +25,21 @@
 HyperCoast.egg-info/entry_points.txt
 HyperCoast.egg-info/requires.txt
 HyperCoast.egg-info/top_level.txt
 docs/CNAME
 docs/changelog.md
 docs/common.md
 docs/contributing.md
+docs/emit.md
 docs/faq.md
 docs/hypercoast.md
 docs/index.md
 docs/installation.md
 docs/usage.md
 docs/examples/intro.ipynb
 docs/overrides/main.html
 hypercoast/__init__.py
 hypercoast/common.py
+hypercoast/emit.py
 hypercoast/hypercoast.py
 tests/__init__.py
 tests/test_hypercoast.py
```

### Comparing `hypercoast-0.0.2/LICENSE` & `hypercoast-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hypercoast-0.0.2/PKG-INFO` & `hypercoast-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: HyperCoast
-Version: 0.0.2
-Summary: A Python package for processing hyperspetral data in coastal regions
+Version: 0.0.3
+Summary: A Python package for processing hyperspectral data in coastal regions
 Author-email: Qiusheng Wu <giswqs@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/opengeos/HyperCoast
 Keywords: HyperCoast
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -13,29 +13,36 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: geopandas
+Requires-Dist: hvplot
 Requires-Dist: leafmap
+Requires-Dist: localtileserver
+Requires-Dist: netcdf4
 Requires-Dist: numpy
+Requires-Dist: xarray
 Provides-Extra: all
 Requires-Dist: HyperCoast[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # HyperCoast
 
 [![image](https://img.shields.io/pypi/v/HyperCoast.svg)](https://pypi.python.org/pypi/HyperCoast)
-[![image](https://img.shields.io/conda/vn/conda-forge/HyperCoast.svg)](https://anaconda.org/conda-forge/HyperCoast)
+[![image](https://static.pepy.tech/badge/hypercoast)](https://pepy.tech/project/hypercoast)
+[![image](https://img.shields.io/conda/vn/conda-forge/hypercoast.svg)](https://anaconda.org/conda-forge/hypercoast)
+[![Conda Recipe](https://img.shields.io/badge/recipe-hypercoast-green.svg)](https://github.com/conda-forge/hypercoast-feedstock)
+[![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/hypercoast.svg)](https://anaconda.org/conda-forge/hypercoast)
 
-**A Python package for processing hyperspetral data in coastal regions**
+**A Python package for visualizing and analyzing hyperspectral data in coastal regions**
 
 -   Free software: MIT License
--   Documentation: https://hypercoast.org
+-   Documentation: <https://hypercoast.org>
 
 ## Features
 
--  Visualize hyperspectral data
--  Analyze hypersepctral data
-
+-   Visualize hyperspectral data
+-   Analyze hyperspectral data
```

### Comparing `hypercoast-0.0.2/docs/contributing.md` & `hypercoast-0.0.3/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `hypercoast-0.0.2/mkdocs.yml` & `hypercoast-0.0.3/mkdocs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 site_name: HyperCoast
-site_description: A Python package for processing hyperspetral data in coastal regions
+site_description: A Python package for processing hyperspectral data in coastal regions
 site_author: giswqs
 site_url: https://hypercoast.org
 repo_url: https://github.com/opengeos/HyperCoast
 
-copyright: "Copyright &copy; 2024 - 2024 Qiusheng Wu"
+copyright: "Copyright &copy; 2024 - 2024 Bingqing Liu & Qiusheng Wu"
 
 theme:
     palette:
         - scheme: default
           #   primary: blue
           #   accent: indigo
           toggle:
@@ -78,9 +78,10 @@
     - Contributing: contributing.md
     - FAQ: faq.md
     - Changelog: changelog.md
     - Report Issues: https://github.com/opengeos/HyperCoast/issues
     - Examples:
           - examples/intro.ipynb
     - API Reference:
-          - hypercoast module: hypercoast.md
           - common module: common.md
+          - emit module: emit.md
+          - hypercoast module: hypercoast.md
```

### Comparing `hypercoast-0.0.2/pyproject.toml` & `hypercoast-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "HyperCoast"
-version = "0.0.2"
+version = "0.0.3"
 dynamic = [
     "dependencies",
 ]
-description = "A Python package for processing hyperspetral data in coastal regions"
+description = "A Python package for processing hyperspectral data in coastal regions"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
     "HyperCoast",
 ]
 license = {text = "MIT License"}
 authors = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.2"
+current_version = "0.0.3"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

