# Comparing `tmp/wuff-1.1.3.tar.gz` & `tmp/wuff-1.1.4-cp312-cp312-manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wuff-1.1.3.tar", last modified: Wed Mar 13 13:18:22 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

