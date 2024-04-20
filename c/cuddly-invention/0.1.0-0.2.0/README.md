# Comparing `tmp/cuddly_invention-0.1.0.tar.gz` & `tmp/cuddly_invention-0.2.0.tar.gz`

## Comparing `cuddly_invention-0.1.0.tar` & `cuddly_invention-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 cuddly_invention-0.1.0/.github/release.yml
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 cuddly_invention-0.1.0/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 cuddly_invention-0.1.0/src/cuddly_invention/__about__.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 cuddly_invention-0.1.0/src/cuddly_invention/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cuddly_invention-0.1.0/src/cuddly_invention/__main__.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 cuddly_invention-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 cuddly_invention-0.1.0/.gitignore
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 cuddly_invention-0.1.0/LICENSE
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 cuddly_invention-0.1.0/README.md
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 cuddly_invention-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 cuddly_invention-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 cuddly_invention-0.2.0/.github/release.yml
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 cuddly_invention-0.2.0/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 cuddly_invention-0.2.0/src/cuddly_invention/__about__.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 cuddly_invention-0.2.0/src/cuddly_invention/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cuddly_invention-0.2.0/src/cuddly_invention/__main__.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 cuddly_invention-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 cuddly_invention-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 cuddly_invention-0.2.0/LICENSE
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 cuddly_invention-0.2.0/README.md
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 cuddly_invention-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 cuddly_invention-0.2.0/PKG-INFO
```

### Comparing `cuddly_invention-0.1.0/.github/workflows/publish-to-test-pypi.yml` & `cuddly_invention-0.2.0/.github/workflows/publish-to-test-pypi.yml`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 jobs:
   build:
     name: Build distribution 📦
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v4
+      with:
+        fetch-depth: 0
     - name: Set up Python
       uses: actions/setup-python@v5
       with:
         python-version: "3.x"
     - name: Install pypa/build
       run: >-
         python3 -m
@@ -53,14 +55,18 @@
     name: >-
       Sign the Python 🐍 distribution 📦 with Sigstore
       and upload them to GitHub Release
     needs:
     - publish-to-pypi
     runs-on: ubuntu-latest
 
+    environment:
+      name: github
+      url: https://github.com/MtkN1/cuddly-invention/releases
+
     permissions:
       contents: write  # IMPORTANT: mandatory for making GitHub Releases
       id-token: write  # IMPORTANT: mandatory for sigstore
 
     steps:
     - name: Download all the dists
       uses: actions/download-artifact@v4
@@ -78,18 +84,18 @@
         GITHUB_TOKEN: ${{ github.token }}
       run: >-
         gh release create
         '${{ github.ref_name }}'
         dist/**
         --repo '${{ github.repository }}'
         --generate-notes
-        --draft
 
   publish-to-testpypi:
     name: Publish Python 🐍 distribution 📦 to TestPyPI
+    if: github.ref == format('refs/heads/{0}', github.event.repository.default_branch)  # only publish to TestPyPI on default branch pushes
     needs:
     - build
     runs-on: ubuntu-latest
 
     environment:
       name: testpypi
       url: https://test.pypi.org/p/cuddly-invention
```

### Comparing `cuddly_invention-0.1.0/.gitignore` & `cuddly_invention-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cuddly_invention-0.1.0/LICENSE` & `cuddly_invention-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cuddly_invention-0.1.0/README.md` & `cuddly_invention-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cuddly_invention-0.1.0/pyproject.toml` & `cuddly_invention-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -30,18 +30,23 @@
 Documentation = "https://github.com/unknown/cuddly-invention#readme"
 Issues = "https://github.com/unknown/cuddly-invention/issues"
 Source = "https://github.com/unknown/cuddly-invention"
 
 [tool.hatch.version]
 source = "vcs"
 
+[tool.hatch.version.raw-options]
+version_scheme = "python-simplified-semver"
+local_scheme = "no-local-version"
+
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
+  "setuptools_scm",
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
```

### Comparing `cuddly_invention-0.1.0/PKG-INFO` & `cuddly_invention-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cuddly-invention
-Version: 0.1.0
+Version: 0.2.0
 Project-URL: Documentation, https://github.com/unknown/cuddly-invention#readme
 Project-URL: Issues, https://github.com/unknown/cuddly-invention/issues
 Project-URL: Source, https://github.com/unknown/cuddly-invention
 Author-email: MtkN1 <51289448+MtkN1@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

