# Comparing `tmp/polyaxon-2.1.7.post1.tar.gz` & `tmp/polyaxon-2.1.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyaxon-2.1.7.post1.tar", last modified: Thu Apr 18 09:41:26 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

