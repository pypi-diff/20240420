# Comparing `tmp/polyaxon-sdk-2.1.7.tar.gz` & `tmp/polyaxon_sdk-2.1.8-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyaxon-sdk-2.1.7.tar", last modified: Mon Apr 15 15:15:34 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

