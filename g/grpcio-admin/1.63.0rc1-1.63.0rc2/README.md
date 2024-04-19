# Comparing `tmp/grpcio-admin-1.63.0rc1.tar.gz` & `tmp/grpcio_admin-1.63.0rc2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpcio-admin-1.63.0rc1.tar", last modified: Fri Apr 12 06:40:51 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

