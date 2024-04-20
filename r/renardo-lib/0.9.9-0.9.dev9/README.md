# Comparing `tmp/renardo_lib-0.9.9.tar.gz` & `tmp/renardo_lib-0.9.dev9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renardo_lib-0.9.9.tar", last modified: Sat Apr 20 17:39:00 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

