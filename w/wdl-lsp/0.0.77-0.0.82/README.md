# Comparing `tmp/wdl-lsp-0.0.77.tar.gz` & `tmp/wdl_lsp-0.0.82-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wdl-lsp-0.0.77.tar", last modified: Thu Sep  2 16:23:44 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

