# Comparing `tmp/fluidimage-0.4.5.tar.gz` & `tmp/fluidimage-0.4.6-cp39-cp39-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluidimage-0.4.5.tar", last modified: Wed Apr 17 13:04:59 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

