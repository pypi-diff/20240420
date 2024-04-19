# Comparing `tmp/grpcio-observability-1.63.0rc1.tar.gz` & `tmp/grpcio_observability-1.63.0rc2-cp39-cp39-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpcio-observability-1.63.0rc1.tar", last modified: Fri Apr 12 06:57:05 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

