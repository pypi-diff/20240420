# Comparing `tmp/xls_updater-0.1.9.tar.gz` & `tmp/xls_updater-0.2.0.tar.gz`

## Comparing `xls_updater-0.1.9.tar` & `xls_updater-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,35 @@
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 xls_updater-0.1.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 xls_updater-0.1.9/.pylintrc
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 xls_updater-0.1.9/CONTRIBUTING.md
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 xls_updater-0.1.9/Makefile
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 xls_updater-0.1.9/requirements-dev.txt
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 xls_updater-0.1.9/requirements-test.txt
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 xls_updater-0.1.9/xls_updater.spec
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 xls_updater-0.1.9/.github/actions/prepare-environment/action.yaml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 xls_updater-0.1.9/.github/workflows/black.yml
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 xls_updater-0.1.9/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 xls_updater-0.1.9/.github/workflows/isort.yml
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 xls_updater-0.1.9/.github/workflows/mypy.yml
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 xls_updater-0.1.9/.github/workflows/publish.yml
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 xls_updater-0.1.9/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 xls_updater-0.1.9/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 xls_updater-0.1.9/.github/workflows/validation.yaml
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 xls_updater-0.1.9/tests/test_app.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 xls_updater-0.1.9/tests/test_big.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 xls_updater-0.1.9/tests/test_cli.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 xls_updater-0.1.9/tests/test_samples.py
--rw-r--r--   0        0        0    30208 2020-02-02 00:00:00.000000 xls_updater-0.1.9/tests/samples/sample1.xls
--rw-r--r--   0        0        0    39424 2020-02-02 00:00:00.000000 xls_updater-0.1.9/tests/samples/sample2.xls
--rw-r--r--   0        0        0    16384 2020-02-02 00:00:00.000000 xls_updater-0.1.9/tests/samples/sample3.xls
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xls_updater-0.1.9/xls_updater/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 xls_updater-0.1.9/xls_updater/__main__.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 xls_updater-0.1.9/xls_updater/app.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 xls_updater-0.1.9/xls_updater/cli.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 xls_updater-0.1.9/.gitignore
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 xls_updater-0.1.9/README.md
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 xls_updater-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 xls_updater-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 xls_updater-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 xls_updater-0.2.0/.pylintrc
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 xls_updater-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 xls_updater-0.2.0/Makefile
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 xls_updater-0.2.0/requirements-dev.txt
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 xls_updater-0.2.0/requirements-test.txt
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 xls_updater-0.2.0/xls_updater.spec
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 xls_updater-0.2.0/.github/actions/prepare-environment/action.yaml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 xls_updater-0.2.0/.github/workflows/black.yml
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 xls_updater-0.2.0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 xls_updater-0.2.0/.github/workflows/isort.yml
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 xls_updater-0.2.0/.github/workflows/mypy.yml
+-rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 xls_updater-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 xls_updater-0.2.0/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 xls_updater-0.2.0/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 xls_updater-0.2.0/.github/workflows/validation.yaml
+-rw-r--r--   0        0        0  7668024 2020-02-02 00:00:00.000000 xls_updater-0.2.0/artifact/xls_updater
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 xls_updater-0.2.0/artifact/xls_updater.md5
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 xls_updater-0.2.0/artifact/xls_updater.sha256
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 xls_updater-0.2.0/tests/test_app.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 xls_updater-0.2.0/tests/test_big.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 xls_updater-0.2.0/tests/test_cli.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 xls_updater-0.2.0/tests/test_samples.py
+-rw-r--r--   0        0        0    30208 2020-02-02 00:00:00.000000 xls_updater-0.2.0/tests/samples/sample1.xls
+-rw-r--r--   0        0        0    39424 2020-02-02 00:00:00.000000 xls_updater-0.2.0/tests/samples/sample2.xls
+-rw-r--r--   0        0        0    16384 2020-02-02 00:00:00.000000 xls_updater-0.2.0/tests/samples/sample3.xls
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 xls_updater-0.2.0/xls_updater/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xls_updater-0.2.0/xls_updater/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 xls_updater-0.2.0/xls_updater/__main__.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 xls_updater-0.2.0/xls_updater/app.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 xls_updater-0.2.0/xls_updater/cli.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 xls_updater-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 xls_updater-0.2.0/README.md
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 xls_updater-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 xls_updater-0.2.0/PKG-INFO
```

### Comparing `xls_updater-0.1.9/.pre-commit-config.yaml` & `xls_updater-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.9/.pylintrc` & `xls_updater-0.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.9/CONTRIBUTING.md` & `xls_updater-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.9/Makefile` & `xls_updater-0.2.0/Makefile`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 	python3 -m black .
 	python3 -m isort .
 
 check-lint:
 	python3 -m pylint --reports=True xls_updater
 
 pytest:
-	python3 -m pytest -v
+	python3 -m pytest -v --durations=0
 
 coverage:
 	python3 -m coverage run --source=xls_updater --module pytest \
 	--verbose tests && coverage report --show-missing
 
 tests: | pytest coverage
```

### Comparing `xls_updater-0.1.9/requirements-dev.txt` & `xls_updater-0.2.0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.9/requirements-test.txt` & `xls_updater-0.2.0/requirements-test.txt`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.9/xls_updater.spec` & `xls_updater-0.2.0/xls_updater.spec`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.9/.github/workflows/coverage.yml` & `xls_updater-0.2.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.9/.github/workflows/publish.yml` & `xls_updater-0.2.0/.github/workflows/publish.yml`

 * *Files 11% similar despite different names*

```diff
@@ -51,32 +51,37 @@
 
       - name: Bump Version
         id: bump_version
         env:
           BUMP_TYPE: ${{ github.event.inputs.bump_type }}
         run: |
           echo "Bumping type: ${{ env.BUMP_TYPE }}"
-          new_version=$(python -m semvergit -t ${{ env.BUMP_TYPE }} -v)
+          new_version=$(python -m semvergit -v -t ${{ env.BUMP_TYPE }} -f xls_updater/__about__.py)
           echo "new_version=$new_version" >> $GITHUB_OUTPUT
 
+      - name: Download Binary Artifact
+        uses: actions/download-artifact@v4
+        with:
+          name: xls_updater
+          path: artifact
+
       - name: Create Github Release
         if: ${{ github.event.inputs.release == 'true' }}
         id: create_release
         uses: softprops/action-gh-release@v2
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-          ARTIFACT_ID: ${{ needs.bundle.outputs.artifact-id }}
         with:
           tag_name: ${{ steps.bump_version.outputs.new_version }}
           release_name: ${{ steps.bump_version.outputs.new_version }}
           body: New Release ${{ steps.bump_version.outputs.new_version }}
           files: |
-            dist/xls_updater
-            dist/xls_updater.md5
-            dist/xls_updater.sha256
+            artifact/xls_updater
+            artifact/xls_updater.md5
+            artifact/xls_updater.sha256
 
       - name: Build Package
         if: ${{ github.event.inputs.publish == 'true' }}
         run: |
           python -m build
 
       - name: Publish To PyPI
@@ -86,16 +91,14 @@
           TWINE_USERNAME: ${{ secrets.PYPI_API_USER }}
         run: |
           python -m twine upload dist/*
 
   bundle:
     name: Bundle
     runs-on: ubuntu-latest
-    outputs:
-      artifact-id: ${{ steps.artifact-upload-step.outputs.artifact-id }}
 
     steps:
       - name: Checkout
         uses: actions/checkout@v4
         with:
           ref: ${{ github.ref }}
           fetch-depth: 0
@@ -104,28 +107,27 @@
         run: |
           python -m pip install --upgrade pip
           python -m pip install '.[bin]'
 
       - name: Create binary bundle
         run: |
           pyinstaller xls_updater.spec
+          chmod +x dist/xls_updater
 
       - name: Bundle info
         run: |
           md5sum dist/xls_updater | cut -d ' ' -f1 > dist/xls_updater.md5
           sha256sum dist/xls_updater | cut -d ' ' -f1 > dist/xls_updater.sha256
           echo "Bundle Info"
           echo "============"
           echo "Size: $(du -sh dist/xls_updater | cut -f1)"
           echo "MD5: $(cat dist/xls_updater.md5)"
           echo "SHA256: $(cat dist/xls_updater.sha256)"
 
       - name: Upload Artifact
         uses: actions/upload-artifact@v4
-        id: artifact-upload-step
         with:
           name: xls_updater
-          path: dist/xls_updater
-
-      - name: Output artifact ID
-        run: |
-          echo "Artifact ID is ${{ steps.artifact-upload-step.outputs.artifact-id }}"
+          path: |
+            dist/xls_updater
+            dist/xls_updater.md5
+            dist/xls_updater.sha256
```

### Comparing `xls_updater-0.1.9/.github/workflows/pytest.yml` & `xls_updater-0.2.0/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.9/.github/workflows/validation.yaml` & `xls_updater-0.2.0/.github/workflows/validation.yaml`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.9/tests/test_app.py` & `xls_updater-0.2.0/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.9/tests/test_big.py` & `xls_updater-0.2.0/tests/test_big.py`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.9/tests/test_cli.py` & `xls_updater-0.2.0/tests/test_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,17 +12,25 @@
 
 @fixture(name="convert_xls_to_xlsx")
 def mock_convert_xls_to_xlsx(mocker: MockerFixture) -> MagicMock:
     """Mock convert_xls_to_xlsx."""
     return mocker.patch("xls_updater.cli.convert_xls_to_xlsx")
 
 
-def test_cli(convert_xls_to_xlsx: MagicMock) -> None:
+def test_cli_convert(convert_xls_to_xlsx: MagicMock) -> None:
     """Test app."""
     runner = CliRunner()
     with runner.isolated_filesystem():
         # create mock file
         Path("sample.xls").touch()
         result = runner.invoke(cli, ["sample.xls"])
         assert result.exit_code == 0, result.output
         convert_xls_to_xlsx.assert_called_once_with(Path("sample.xls"))
         Path("sample.xls").unlink()
+
+
+def test_cli_version() -> None:
+    """Test app."""
+    runner = CliRunner()
+    result = runner.invoke(cli, ["--version"])
+    assert result.exit_code == 0, result.output
+    assert "version" in result.output
```

### Comparing `xls_updater-0.1.9/tests/test_samples.py` & `xls_updater-0.2.0/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.9/tests/samples/sample1.xls` & `xls_updater-0.2.0/tests/samples/sample1.xls`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.9/tests/samples/sample2.xls` & `xls_updater-0.2.0/tests/samples/sample2.xls`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.9/tests/samples/sample3.xls` & `xls_updater-0.2.0/tests/samples/sample3.xls`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.9/xls_updater/app.py` & `xls_updater-0.2.0/xls_updater/app.py`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.9/.gitignore` & `xls_updater-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.9/README.md` & `xls_updater-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.9/pyproject.toml` & `xls_updater-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 [project]
 name = "xls-updater"
 description = "Convert legacy xls data to newer xlsx format."
 readme = "README.md"
 requires-python = ">=3.10"
-dynamic = ["version"]
 keywords = [
     "converter",
     "xls",
     "xlsx",
     "excel",
     "spreadsheet",
     "fileformat",
@@ -21,14 +20,15 @@
     "Natural Language :: English",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Office/Business :: Financial :: Spreadsheet",
     "Topic :: File Formats",
 ]
+dynamic = ["version"]
 dependencies = [
     "click==8.1.7",
     "openpyxl==3.1.2",
     "xlrd==2.0.1",
     "tqdm==4.66.2"
 ]
 [project.optional-dependencies]
@@ -61,30 +61,19 @@
 xls-updater = "xls_updater.cli:cli"
 
 [project.urls]
 homepage = "https://github.com/Tranquility2/xls_updater"
 repository = "https://github.com/Tranquility2/xls_updater"
 
 [build-system]
-requires = [
-    "hatchling",
-    "versioningit",
-]
+requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.version]
-source = "versioningit"
-
-[tool.versioningit.vcs]
-default-tag = "0.0.0"
-match = ["v*", ]
-method = "git"
-
-[tool.versioningit.tag2version]
-rmprefix = "v"
+path = "xls_updater/__about__.py"
 
 [tool.pip-tools]
 quiet = true
 rebuild = true
 strip-extras = true
 no-header = true
 annotation-style = "line"
@@ -96,32 +85,28 @@
 [tool.isort]
 multi_line_output = 3
 line_length = 120
 include_trailing_comma = true
 
 [tool.black]
 line-length = 120
-target_version = ["py311"]
 include = '\.pyi?$'
 exclude = '''
 (
   /(
-      \.eggs         # exclude a few common directories in the
-    | \.git          # root of the project
-    | \.hg
+      \.eggs
+    | \.git
     | \.mypy_cache
     | \.tox
     | \.venv
     | _build
-    | buck-out
     | build
     | dist
   )/
-  | foo.py           # also separately exclude a file named foo.py in
-                     # the root of the project
+  | version.py
 )
 '''
 
 [tool.pylint.main]
 fail-under = 10.0
 
 [tool.pylint.format]
```

### Comparing `xls_updater-0.1.9/PKG-INFO` & `xls_updater-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: xls-updater
-Version: 0.1.9
+Version: 0.2.0
 Summary: Convert legacy xls data to newer xlsx format.
 Project-URL: homepage, https://github.com/Tranquility2/xls_updater
 Project-URL: repository, https://github.com/Tranquility2/xls_updater
 Author-email: Roy Moore <roy@moore.co.il>
 Keywords: converter,excel,fileformat,spreadsheet,xls,xlsx
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

