# Comparing `tmp/pandas-wizard-1.0.0.dev0.tar.gz` & `tmp/pandas_wizard-1.0.1.dev0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-wizard-1.0.0.dev0.tar", last modified: Fri Apr 19 15:52:53 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

