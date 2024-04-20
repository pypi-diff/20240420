# Comparing `tmp/nyckel-0.4.2.tar.gz` & `tmp/nyckel-0.4.3.tar.gz`

## Comparing `nyckel-0.4.2.tar` & `nyckel-0.4.3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 nyckel-0.4.2/mkdocs.yml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nyckel-0.4.2/requirements.txt
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 nyckel-0.4.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nyckel-0.4.2/.github/workflows/docs.yml
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nyckel-0.4.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nyckel-0.4.2/.vscode/extensions.json
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 nyckel-0.4.2/.vscode/settings.json
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nyckel-0.4.2/docs/copy_function.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nyckel-0.4.2/docs/credentials.md
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 nyckel-0.4.2/docs/data_classes.md
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nyckel-0.4.2/docs/delete_label.md
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nyckel-0.4.2/docs/delete_samples.md
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nyckel-0.4.2/docs/image_classification.md
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nyckel-0.4.2/docs/image_tags.md
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 nyckel-0.4.2/docs/index.md
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nyckel-0.4.2/docs/merge_labels.md
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 nyckel-0.4.2/docs/multimodal_classification.md
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nyckel-0.4.2/docs/quickstart.md
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nyckel-0.4.2/docs/requirements.txt
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nyckel-0.4.2/docs/tabular_classification.md
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nyckel-0.4.2/docs/text_classification.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 nyckel-0.4.2/docs/text_tags.md
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 nyckel-0.4.2/docs/assets/favicon.ico
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 nyckel-0.4.2/docs/assets/nyckel-logo.png
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nyckel-0.4.2/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/__init__.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/auth.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/config.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/data_classes.py
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/image_processing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/py.typed
--rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/request_utils.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/functions/__init__.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/functions/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/functions/classification/__init__.py
--rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/functions/classification/classification.py
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/functions/classification/factory.py
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/functions/classification/function_handler.py
--rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/functions/classification/image_classification.py
--rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/functions/classification/label_handler.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/functions/classification/sample_handler.py
--rw-r--r--   0        0        0    14966 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/functions/classification/tabular_classification.py
--rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/functions/classification/text_classification.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/functions/tags/__init__.py
--rw-r--r--   0        0        0    10186 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/functions/tags/image_tags.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/functions/tags/tags.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/functions/tags/tags_function_factory.py
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/functions/tags/tags_function_handler.py
--rw-r--r--   0        0        0     6726 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/functions/tags/tags_sample_handler.py
--rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 nyckel-0.4.2/src/nyckel/functions/tags/text_tags.py
--rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 nyckel-0.4.2/tests/conftest.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nyckel-0.4.2/tests/test_duplicates_handling.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 nyckel-0.4.2/tests/test_field_handler.py
--rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 nyckel-0.4.2/tests/test_image_classification_function.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 nyckel-0.4.2/tests/test_image_decoder.py
--rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 nyckel-0.4.2/tests/test_image_tags_function.py
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 nyckel-0.4.2/tests/test_label_handler.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 nyckel-0.4.2/tests/test_sample_handler.py
--rw-r--r--   0        0        0     5436 2020-02-02 00:00:00.000000 nyckel-0.4.2/tests/test_tabular_classification_function.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 nyckel-0.4.2/tests/test_text_classification_function.py
--rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 nyckel-0.4.2/tests/test_text_tags_function.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 nyckel-0.4.2/tests/test_white_background.py
--rw-r--r--   0        0        0   107239 2020-02-02 00:00:00.000000 nyckel-0.4.2/tests/fixtures/flower.jpg
--rw-r--r--   0        0        0    26189 2020-02-02 00:00:00.000000 nyckel-0.4.2/tests/fixtures/mixed-alpha-background.png
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 nyckel-0.4.2/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.4.2/LICENSE
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 nyckel-0.4.2/README.md
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nyckel-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 nyckel-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 nyckel-0.4.3/mkdocs.yml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nyckel-0.4.3/requirements.txt
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 nyckel-0.4.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nyckel-0.4.3/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nyckel-0.4.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nyckel-0.4.3/.vscode/extensions.json
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 nyckel-0.4.3/.vscode/settings.json
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/copy_function.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/credentials.md
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/data_classes.md
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/delete_label.md
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/delete_samples.md
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/image_classification.md
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/image_tags.md
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/index.md
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/merge_labels.md
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/multimodal_classification.md
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/quickstart.md
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/requirements.txt
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/tabular_classification.md
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/text_classification.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/text_tags.md
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/assets/favicon.ico
+-rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/assets/nyckel-logo.png
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/__init__.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/auth.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/config.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/data_classes.py
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/image_processing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/py.typed
+-rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/request_utils.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/__init__.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/classification/__init__.py
+-rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/classification/classification.py
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/classification/factory.py
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/classification/function_handler.py
+-rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/classification/image_classification.py
+-rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/classification/label_handler.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/classification/sample_handler.py
+-rw-r--r--   0        0        0    14966 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/classification/tabular_classification.py
+-rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/classification/text_classification.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/tags/__init__.py
+-rw-r--r--   0        0        0    10186 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/tags/image_tags.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/tags/tags.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/tags/tags_function_factory.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/tags/tags_function_handler.py
+-rw-r--r--   0        0        0     6726 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/tags/tags_sample_handler.py
+-rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/tags/text_tags.py
+-rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/conftest.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/test_duplicates_handling.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/test_field_handler.py
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/test_image_classification_function.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/test_image_decoder.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/test_image_tags_function.py
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/test_label_handler.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/test_sample_handler.py
+-rw-r--r--   0        0        0     5667 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/test_tabular_classification_function.py
+-rw-r--r--   0        0        0     8886 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/test_tags_shared.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/test_text_classification_function.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/test_white_background.py
+-rw-r--r--   0        0        0   107239 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/fixtures/flower.jpg
+-rw-r--r--   0        0        0    26189 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/fixtures/mixed-alpha-background.png
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 nyckel-0.4.3/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.4.3/LICENSE
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 nyckel-0.4.3/README.md
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nyckel-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 nyckel-0.4.3/PKG-INFO
```

### Comparing `nyckel-0.4.2/mkdocs.yml` & `nyckel-0.4.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/.github/workflows/build.yml` & `nyckel-0.4.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/.github/workflows/docs.yml` & `nyckel-0.4.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/.github/workflows/test.yml` & `nyckel-0.4.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/.vscode/settings.json` & `nyckel-0.4.3/.vscode/settings.json`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         "**/__pycache__": true,
         "**/.pytest_cache": true,
         "**/.ropeproject": true,
         "**/.idea": true,
     },
     "cSpell.words": [
         "chunkify",
+        "getfixturevalue",
         "getpixel",
         "Gruezi",
         "Hola",
         "Multimodal",
         "ncols",
         "nyckel",
         "pytest",
```

### Comparing `nyckel-0.4.2/docs/copy_function.md` & `nyckel-0.4.3/docs/copy_function.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/docs/delete_label.md` & `nyckel-0.4.3/docs/delete_label.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/docs/delete_samples.md` & `nyckel-0.4.3/docs/delete_samples.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/docs/index.md` & `nyckel-0.4.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/docs/merge_labels.md` & `nyckel-0.4.3/docs/merge_labels.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/docs/multimodal_classification.md` & `nyckel-0.4.3/docs/multimodal_classification.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/docs/quickstart.md` & `nyckel-0.4.3/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/docs/assets/favicon.ico` & `nyckel-0.4.3/docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/docs/assets/nyckel-logo.png` & `nyckel-0.4.3/docs/assets/nyckel-logo.png`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/src/nyckel/__init__.py` & `nyckel-0.4.3/src/nyckel/__init__.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/src/nyckel/auth.py` & `nyckel-0.4.3/src/nyckel/auth.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/src/nyckel/image_processing.py` & `nyckel-0.4.3/src/nyckel/image_processing.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/src/nyckel/request_utils.py` & `nyckel-0.4.3/src/nyckel/request_utils.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/src/nyckel/functions/utils.py` & `nyckel-0.4.3/src/nyckel/functions/utils.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/src/nyckel/functions/classification/classification.py` & `nyckel-0.4.3/src/nyckel/functions/classification/classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/src/nyckel/functions/classification/factory.py` & `nyckel-0.4.3/src/nyckel/functions/classification/factory.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/src/nyckel/functions/classification/function_handler.py` & `nyckel-0.4.3/src/nyckel/functions/classification/function_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/src/nyckel/functions/classification/image_classification.py` & `nyckel-0.4.3/src/nyckel/functions/classification/image_classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/src/nyckel/functions/classification/label_handler.py` & `nyckel-0.4.3/src/nyckel/functions/classification/label_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/src/nyckel/functions/classification/sample_handler.py` & `nyckel-0.4.3/src/nyckel/functions/classification/sample_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/src/nyckel/functions/classification/tabular_classification.py` & `nyckel-0.4.3/src/nyckel/functions/classification/tabular_classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/src/nyckel/functions/classification/text_classification.py` & `nyckel-0.4.3/src/nyckel/functions/classification/text_classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/src/nyckel/functions/tags/image_tags.py` & `nyckel-0.4.3/src/nyckel/functions/tags/image_tags.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/src/nyckel/functions/tags/tags.py` & `nyckel-0.4.3/src/nyckel/functions/tags/tags.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/src/nyckel/functions/tags/tags_function_factory.py` & `nyckel-0.4.3/src/nyckel/functions/tags/tags_function_factory.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/src/nyckel/functions/tags/tags_function_handler.py` & `nyckel-0.4.3/src/nyckel/functions/tags/tags_function_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/src/nyckel/functions/tags/tags_sample_handler.py` & `nyckel-0.4.3/src/nyckel/functions/tags/tags_sample_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/src/nyckel/functions/tags/text_tags.py` & `nyckel-0.4.3/src/nyckel/functions/tags/text_tags.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/tests/conftest.py` & `nyckel-0.4.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/tests/test_duplicates_handling.py` & `nyckel-0.4.3/tests/test_duplicates_handling.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/tests/test_field_handler.py` & `nyckel-0.4.3/tests/test_field_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/tests/test_image_classification_function.py` & `nyckel-0.4.3/tests/test_image_classification_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/tests/test_image_decoder.py` & `nyckel-0.4.3/tests/test_image_decoder.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/tests/test_label_handler.py` & `nyckel-0.4.3/tests/test_label_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/tests/test_sample_handler.py` & `nyckel-0.4.3/tests/test_sample_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/tests/test_tabular_classification_function.py` & `nyckel-0.4.3/tests/test_tabular_classification_function.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,21 +30,24 @@
     func.create_samples(
         [
             TabularClassificationSample(
                 data={"firstname": "Adam", "lastname": "Art", "mugshot": local_image_file},
                 annotation=ClassificationAnnotation(label_name="happy"),
             ),
             TabularClassificationSample(
-                data={"firstname": "Bo", "lastname": "Busy"}, annotation=ClassificationAnnotation(label_name="happy")
+                data={"firstname": "Bo", "lastname": "Busy", "mugshot": local_image_file},
+                annotation=ClassificationAnnotation(label_name="happy"),
             ),
             TabularClassificationSample(
-                data={"firstname": "Carl", "lastname": "Carrot"}, annotation=ClassificationAnnotation(label_name="sad")
+                data={"firstname": "Carl", "lastname": "Carrot", "mugshot": local_image_file},
+                annotation=ClassificationAnnotation(label_name="sad"),
             ),
             TabularClassificationSample(
-                data={"firstname": "Dick", "lastname": "Denali"}, annotation=ClassificationAnnotation(label_name="sad")
+                data={"firstname": "Dick", "lastname": "Denali", "mugshot": local_image_file},
+                annotation=ClassificationAnnotation(label_name="sad"),
             ),
         ]
     )
 
     fields = func.list_fields()
     assert len(fields) == 3
     assert set([field.name for field in fields]) == set(["firstname", "lastname", "mugshot"])
@@ -56,15 +59,18 @@
         print("-> No trained model yet. Sleeping 1 sec...")
         time.sleep(1)
 
     prediction = func.invoke([{"firstname": "Eric", "lastname": "Ebony", "mugshot": local_image_file}])[0]
     assert isinstance(prediction, ClassificationPrediction)
 
     predictions = func.invoke(
-        [{"firstname": "Eric", "lastname": "Ebony"}, {"firstname": "Frank", "lastname": "Froggy"}]
+        [
+            {"firstname": "Eric", "lastname": "Ebony", "mugshot": local_image_file},
+            {"firstname": "Frank", "lastname": "Froggy", "mugshot": local_image_file},
+        ]
     )
     assert isinstance(predictions[0], ClassificationPrediction)
 
 
 def test_field_creation(tabular_classification_function: TabularClassificationFunction) -> None:
     func: TabularClassificationFunction = tabular_classification_function
     func.create_fields([TabularFunctionField(name="firstname", type="Text")])
```

### Comparing `nyckel-0.4.2/tests/test_text_classification_function.py` & `nyckel-0.4.3/tests/test_text_classification_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/tests/test_white_background.py` & `nyckel-0.4.3/tests/test_white_background.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/tests/fixtures/flower.jpg` & `nyckel-0.4.3/tests/fixtures/flower.jpg`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/tests/fixtures/mixed-alpha-background.png` & `nyckel-0.4.3/tests/fixtures/mixed-alpha-background.png`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/.gitignore` & `nyckel-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/LICENSE` & `nyckel-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/README.md` & `nyckel-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.2/pyproject.toml` & `nyckel-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/nyckel"]
 
 [project]
 name = "nyckel"
-version = "0.4.2"
+version = "0.4.3"
 authors = [{ name = "Oscar Beijbom", email = "oscar@nyckel.com" }]
 description = "Python package for the Nyckel API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `nyckel-0.4.2/PKG-INFO` & `nyckel-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nyckel
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python package for the Nyckel API
 Project-URL: Homepage, https://github.com/NyckelAI/python-sdk
 Author-email: Oscar Beijbom <oscar@nyckel.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

