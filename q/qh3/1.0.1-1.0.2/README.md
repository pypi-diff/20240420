# Comparing `tmp/qh3-1.0.1.tar.gz` & `tmp/qh3-1.0.2-pp37-pypy37_pp73-musllinux_1_1_armv7l.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

