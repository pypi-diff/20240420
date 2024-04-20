# Comparing `tmp/pytoy-0.0.3.tar.gz` & `tmp/pytoy-0.0.4.tar.gz`

## Comparing `pytoy-0.0.3.tar` & `pytoy-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,18 @@
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pytoy-0.0.3/mkdocs.yml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pytoy-0.0.3/requirements.txt
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 pytoy-0.0.3/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 pytoy-0.0.3/.github/workflows/python.yml
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 pytoy-0.0.3/.github/workflows/template-rename.yml
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pytoy-0.0.3/.github/workflows/template-sync.yml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pytoy-0.0.3/docs/index.md
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pytoy-0.0.3/src/pytoy/__init__.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 pytoy-0.0.3/src/pytoy/cli.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 pytoy-0.0.3/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pytoy-0.0.3/LICENSE
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pytoy-0.0.3/README.md
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pytoy-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 pytoy-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pytoy-0.0.4/mkdocs.yml
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 pytoy-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pytoy-0.0.4/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 pytoy-0.0.4/.github/workflows/python.yml
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 pytoy-0.0.4/.github/workflows/template-rename.yml
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pytoy-0.0.4/.github/workflows/template-sync.yml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pytoy-0.0.4/docs/index.md
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 pytoy-0.0.4/scripts/gen_ref_pages.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pytoy-0.0.4/src/pytoy/__init__.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 pytoy-0.0.4/src/pytoy/cli.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 pytoy-0.0.4/src/pytoy/cli_file.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pytoy-0.0.4/src/pytoy/common.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 pytoy-0.0.4/src/pytoy/nginx.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 pytoy-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pytoy-0.0.4/LICENSE
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pytoy-0.0.4/README.md
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pytoy-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 pytoy-0.0.4/PKG-INFO
```

### Comparing `pytoy-0.0.3/.github/workflows/python.yml` & `pytoy-0.0.4/.github/workflows/python.yml`

 * *Files 14% similar despite different names*

```diff
@@ -55,32 +55,74 @@
         with:
           python-version-file: 'pyproject.toml'
 
       - name: Display python version
         run: python3 --version
 
       - name: Install dependencies
-        run: python3 -m pip install --upgrade build
+        run: python3 -m pip install --upgrade -r requirements.txt
 
       - name: Build
         run: python3 -m build
 
-      - name: Upload artifacts
+      - name: Build docs
+        run: mkdocs build -s
+
+      - name: Upload package artifacts
         uses: actions/upload-artifact@v4
         with:
           name: package
           path: dist
 
-  pypi-publish:
-      name: Upload release to PyPI
-      runs-on: ubuntu-latest
-      needs: [package]
-      permissions:
-        id-token: write
-      steps:
-      - name: Download artifacts
-        uses: actions/download-artifact@v4
+      - name: Upload docs artifacts
+        uses: actions/upload-artifact@v4
         with:
-          name: package
-          path: dist
-      - name: Publish package distributions to PyPI
-        uses: pypa/gh-action-pypi-publish@release/v1
+          name: docs
+          path: site
+
+  pypi-publish:
+    name: Upload release to PyPI
+    runs-on: ubuntu-latest
+    needs: [package]
+    permissions:
+      id-token: write
+    steps:
+    - name: Download artifacts
+      uses: actions/download-artifact@v4
+      with:
+        name: package
+        path: dist
+    - name: Publish package distributions to PyPI
+      uses: pypa/gh-action-pypi-publish@release/v1
+  
+  pages-publish:
+    name: Upload release to PyPI
+    runs-on: ubuntu-latest
+    needs: [package]
+    environment:
+      name: github-pages
+      url: ${{ steps.deployment.outputs.page_url }}
+    permissions:
+      contents: read
+      pages: write
+      id-token: write
+    concurrency:
+      group: "pages"
+      cancel-in-progress: false
+    steps:
+
+    - name: Download artifacts
+      uses: actions/download-artifact@v4
+      with:
+        name: docs
+        path: site
+
+    - name: Setup Pages
+      uses: actions/configure-pages@v5
+
+    - name: Upload artifact
+      uses: actions/upload-pages-artifact@v3
+      with:
+        path: 'site'
+    - name: Deploy to GitHub Pages
+      id: deployment
+      uses: actions/deploy-pages@v4
```

### Comparing `pytoy-0.0.3/.github/workflows/template-rename.yml` & `pytoy-0.0.4/.github/workflows/template-rename.yml`

 * *Files identical despite different names*

### Comparing `pytoy-0.0.3/.github/workflows/template-sync.yml` & `pytoy-0.0.4/.github/workflows/template-sync.yml`

 * *Files identical despite different names*

### Comparing `pytoy-0.0.3/.gitignore` & `pytoy-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pytoy-0.0.3/LICENSE` & `pytoy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytoy-0.0.3/pyproject.toml` & `pytoy-0.0.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pytoy"
-version = "0.0.3"
+version = "0.0.4"
 authors = [{ name = "WitonAI" }]
 description = "PyToy package"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = ["fire"]
 classifiers = [
   "Programming Language :: Python :: 3",
```

