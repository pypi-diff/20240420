# Comparing `tmp/liba-0.1.9.tar.gz` & `tmp/liba-0.1.9.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liba-0.1.9.tar", last modified: Sun Mar 31 02:07:02 2024, max compression
+gzip compressed data, was "liba-0.1.9.post1.tar", last modified: Sun Mar 31 04:05:35 2024, max compression
```

## Comparing `liba-0.1.9.tar` & `liba-0.1.9.post1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 02:07:02.784593 liba-0.1.9/
--rw-rw-rw-   0        0        0    16727 2024-03-18 13:04:44.000000 liba-0.1.9/LICENSE.txt
--rw-rw-rw-   0        0        0       61 2024-03-28 13:34:12.000000 liba-0.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0     5291 2024-03-31 02:07:02.784593 liba-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     4500 2024-03-28 13:34:12.000000 liba-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-03-31 02:07:02.643005 liba-0.1.9/include/
-drwxrwxrwx   0        0        0        0 2024-03-31 02:07:02.711810 liba-0.1.9/include/a/
--rw-rw-rw-   0        0        0    42638 2024-03-31 00:23:36.000000 liba-0.1.9/include/a/a.h
--rw-rw-rw-   0        0        0     9807 2024-03-28 13:34:12.000000 liba-0.1.9/include/a/avl.h
--rw-rw-rw-   0        0        0    11048 2024-03-28 13:34:12.000000 liba-0.1.9/include/a/buf.h
--rw-rw-rw-   0        0        0    31885 2024-03-18 13:04:44.000000 liba-0.1.9/include/a/complex.h
--rw-rw-rw-   0        0        0     1487 2024-03-18 13:04:44.000000 liba-0.1.9/include/a/crc.h
--rw-rw-rw-   0        0        0     3984 2024-03-28 13:34:12.000000 liba-0.1.9/include/a/fuzzy.h
--rw-rw-rw-   0        0        0     3171 2024-03-30 14:06:42.000000 liba-0.1.9/include/a/hpf.h
--rw-rw-rw-   0        0        0    13295 2024-03-28 13:34:12.000000 liba-0.1.9/include/a/list.h
--rw-rw-rw-   0        0        0     2989 2024-03-30 14:06:42.000000 liba-0.1.9/include/a/lpf.h
--rw-rw-rw-   0        0        0    10506 2024-03-18 13:04:44.000000 liba-0.1.9/include/a/math.h
--rw-rw-rw-   0        0        0     9317 2024-03-18 13:04:44.000000 liba-0.1.9/include/a/mf.h
--rw-rw-rw-   0        0        0   111612 2024-03-18 13:04:44.000000 liba-0.1.9/include/a/notefreqs.h
--rw-rw-rw-   0        0        0     2291 2024-03-18 13:04:44.000000 liba-0.1.9/include/a/operator.h
--rw-rw-rw-   0        0        0     4081 2024-03-28 13:34:12.000000 liba-0.1.9/include/a/pid.h
--rw-rw-rw-   0        0        0     6670 2024-03-28 13:34:12.000000 liba-0.1.9/include/a/pid_fuzzy.h
--rw-rw-rw-   0        0        0     3748 2024-03-28 13:34:12.000000 liba-0.1.9/include/a/pid_neuro.h
--rw-rw-rw-   0        0        0     1948 2024-03-18 13:04:44.000000 liba-0.1.9/include/a/poly.h
--rw-rw-rw-   0        0        0     9622 2024-03-30 14:06:42.000000 liba-0.1.9/include/a/que.h
--rw-rw-rw-   0        0        0    10091 2024-03-28 13:34:12.000000 liba-0.1.9/include/a/rbt.h
--rw-rw-rw-   0        0        0     5228 2024-03-18 13:04:44.000000 liba-0.1.9/include/a/slist.h
--rw-rw-rw-   0        0        0     8624 2024-03-28 13:34:12.000000 liba-0.1.9/include/a/str.h
--rw-rw-rw-   0        0        0     2969 2024-03-28 13:34:12.000000 liba-0.1.9/include/a/tf.h
--rw-rw-rw-   0        0        0     7440 2024-03-28 13:34:12.000000 liba-0.1.9/include/a/trajbell.h
--rw-rw-rw-   0        0        0     4853 2024-03-28 13:34:12.000000 liba-0.1.9/include/a/trajpoly3.h
--rw-rw-rw-   0        0        0     5768 2024-03-28 13:34:12.000000 liba-0.1.9/include/a/trajpoly5.h
--rw-rw-rw-   0        0        0     7895 2024-03-28 13:34:12.000000 liba-0.1.9/include/a/trajpoly7.h
--rw-rw-rw-   0        0        0     4904 2024-03-28 13:34:12.000000 liba-0.1.9/include/a/trajtrap.h
--rw-rw-rw-   0        0        0     1603 2024-03-18 13:04:44.000000 liba-0.1.9/include/a/utf.h
--rw-rw-rw-   0        0        0    12780 2024-03-28 13:34:12.000000 liba-0.1.9/include/a/vec.h
--rw-rw-rw-   0        0        0     6914 2024-03-30 14:06:42.000000 liba-0.1.9/include/a/version.h
--rw-rw-rw-   0        0        0       92 2024-03-18 13:04:44.000000 liba-0.1.9/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-03-31 02:07:02.657818 liba-0.1.9/python/
-drwxrwxrwx   0        0        0        0 2024-03-31 02:07:02.718844 liba-0.1.9/python/liba.egg-info/
--rw-rw-rw-   0        0        0     5291 2024-03-31 02:07:02.000000 liba-0.1.9/python/liba.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1513 2024-03-31 02:07:02.000000 liba-0.1.9/python/liba.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 02:07:02.000000 liba-0.1.9/python/liba.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-03-31 02:07:02.000000 liba-0.1.9/python/liba.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-31 02:07:02.723892 liba-0.1.9/python/src/
-drwxrwxrwx   0        0        0        0 2024-03-31 02:07:02.746527 liba-0.1.9/python/src/a/
--rw-rw-rw-   0        0        0     1307 2024-03-28 13:34:12.000000 liba-0.1.9/python/src/a/__init__.pxd
--rw-rw-rw-   0        0        0     1022 2024-03-18 13:04:44.000000 liba-0.1.9/python/src/a/crc.pxd
--rw-rw-rw-   0        0        0      499 2024-03-28 13:34:12.000000 liba-0.1.9/python/src/a/fuzzy.pxd
--rw-rw-rw-   0        0        0      311 2024-03-18 13:04:44.000000 liba-0.1.9/python/src/a/hpf.pxd
--rw-rw-rw-   0        0        0      289 2024-03-18 13:04:44.000000 liba-0.1.9/python/src/a/lpf.pxd
--rw-rw-rw-   0        0        0      193 2024-03-18 13:04:44.000000 liba-0.1.9/python/src/a/math.pxd
--rw-rw-rw-   0        0        0     1305 2024-03-18 13:04:44.000000 liba-0.1.9/python/src/a/mf.pxd
--rw-rw-rw-   0        0        0      614 2024-03-28 13:34:12.000000 liba-0.1.9/python/src/a/pid.pxd
--rw-rw-rw-   0        0        0     1332 2024-03-28 13:34:12.000000 liba-0.1.9/python/src/a/pid_fuzzy.pxd
--rw-rw-rw-   0        0        0      604 2024-03-18 13:04:44.000000 liba-0.1.9/python/src/a/pid_neuro.pxd
--rw-rw-rw-   0        0        0      232 2024-03-18 13:04:44.000000 liba-0.1.9/python/src/a/poly.pxd
--rw-rw-rw-   0        0        0      499 2024-03-18 13:04:44.000000 liba-0.1.9/python/src/a/tf.pxd
--rw-rw-rw-   0        0        0      750 2024-03-28 13:31:42.000000 liba-0.1.9/python/src/a/trajbell.pxd
--rw-rw-rw-   0        0        0      461 2024-03-30 23:58:00.000000 liba-0.1.9/python/src/a/trajpoly3.pxd
--rw-rw-rw-   0        0        0      485 2024-03-30 23:58:02.000000 liba-0.1.9/python/src/a/trajpoly5.pxd
--rw-rw-rw-   0        0        0      600 2024-03-30 23:58:05.000000 liba-0.1.9/python/src/a/trajpoly7.pxd
--rw-rw-rw-   0        0        0      642 2024-03-28 13:31:42.000000 liba-0.1.9/python/src/a/trajtrap.pxd
--rw-rw-rw-   0        0        0     1245 2024-03-30 23:58:11.000000 liba-0.1.9/python/src/a/version.pxd
--rw-rw-rw-   0        0        0  2099989 2024-03-31 02:07:02.000000 liba-0.1.9/python/src/a.c
--rw-rw-rw-   0        0        0    40552 2024-03-31 00:06:16.000000 liba-0.1.9/python/src/a.pyx
--rw-rw-rw-   0        0        0      664 2024-03-31 02:07:02.786599 liba-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     5073 2024-03-28 13:31:47.000000 liba-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-31 02:07:02.783622 liba-0.1.9/src/
--rw-rw-rw-   0        0        0     2761 2024-03-18 13:04:44.000000 liba-0.1.9/src/a.c
--rw-rw-rw-   0        0        0    23944 2024-03-28 13:34:12.000000 liba-0.1.9/src/avl.c
--rw-rw-rw-   0        0        0     4167 2024-03-28 13:34:12.000000 liba-0.1.9/src/buf.c
--rw-rw-rw-   0        0        0    25134 2024-03-18 13:04:44.000000 liba-0.1.9/src/complex.c
--rw-rw-rw-   0        0        0     4875 2024-03-28 13:31:47.000000 liba-0.1.9/src/crc.c
--rw-rw-rw-   0        0        0      328 2024-03-28 13:34:12.000000 liba-0.1.9/src/fuzzy.c
--rw-rw-rw-   0        0        0     6113 2024-03-28 13:34:12.000000 liba-0.1.9/src/math.c
--rw-rw-rw-   0        0        0     4500 2024-03-18 13:04:44.000000 liba-0.1.9/src/mf.c
--rw-rw-rw-   0        0        0     2127 2024-03-28 13:34:12.000000 liba-0.1.9/src/pid.c
--rw-rw-rw-   0        0        0     6574 2024-03-28 13:34:12.000000 liba-0.1.9/src/pid_fuzzy.c
--rw-rw-rw-   0        0        0     1819 2024-03-28 13:34:12.000000 liba-0.1.9/src/pid_neuro.c
--rw-rw-rw-   0        0        0      561 2024-03-28 13:59:44.000000 liba-0.1.9/src/poly.c
--rw-rw-rw-   0        0        0     7685 2024-03-31 00:23:36.000000 liba-0.1.9/src/que.c
--rw-rw-rw-   0        0        0    22692 2024-03-28 13:34:12.000000 liba-0.1.9/src/rbt.c
--rw-rw-rw-   0        0        0     5713 2024-03-28 13:34:12.000000 liba-0.1.9/src/str.c
--rw-rw-rw-   0        0        0     1269 2024-03-18 13:04:44.000000 liba-0.1.9/src/tf.c
--rw-rw-rw-   0        0        0     8585 2024-03-28 13:34:12.000000 liba-0.1.9/src/trajbell.c
--rw-rw-rw-   0        0        0     1811 2024-03-28 13:31:42.000000 liba-0.1.9/src/trajpoly3.c
--rw-rw-rw-   0        0        0     2466 2024-03-28 13:31:42.000000 liba-0.1.9/src/trajpoly5.c
--rw-rw-rw-   0        0        0     3713 2024-03-28 13:31:42.000000 liba-0.1.9/src/trajpoly7.c
--rw-rw-rw-   0        0        0     3816 2024-03-28 13:34:12.000000 liba-0.1.9/src/trajtrap.c
--rw-rw-rw-   0        0        0     2872 2024-03-18 13:04:44.000000 liba-0.1.9/src/utf.c
--rw-rw-rw-   0        0        0     6064 2024-03-28 13:59:44.000000 liba-0.1.9/src/vec.c
--rw-rw-rw-   0        0        0     5535 2024-03-28 13:34:12.000000 liba-0.1.9/src/version.c
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-31 04:05:35.820005 liba-0.1.9.post1/
+-rwxrwxrwx   0 root         (0) root         (0)    16727 2024-03-18 13:04:44.000000 liba-0.1.9.post1/LICENSE.txt
+-rwxrwxrwx   0 root         (0) root         (0)       61 2024-03-28 13:34:12.000000 liba-0.1.9.post1/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     5056 2024-03-31 04:05:35.820005 liba-0.1.9.post1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     4500 2024-03-28 13:34:12.000000 liba-0.1.9.post1/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-31 04:05:35.659261 liba-0.1.9.post1/include/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-31 04:05:35.736288 liba-0.1.9.post1/include/a/
+-rwxrwxrwx   0 root         (0) root         (0)    42638 2024-03-31 04:02:52.000000 liba-0.1.9.post1/include/a/a.h
+-rwxrwxrwx   0 root         (0) root         (0)     9807 2024-03-28 13:34:12.000000 liba-0.1.9.post1/include/a/avl.h
+-rwxrwxrwx   0 root         (0) root         (0)    11048 2024-03-28 13:34:12.000000 liba-0.1.9.post1/include/a/buf.h
+-rwxrwxrwx   0 root         (0) root         (0)    31885 2024-03-18 13:04:44.000000 liba-0.1.9.post1/include/a/complex.h
+-rwxrwxrwx   0 root         (0) root         (0)     1487 2024-03-18 13:04:44.000000 liba-0.1.9.post1/include/a/crc.h
+-rwxrwxrwx   0 root         (0) root         (0)     3984 2024-03-28 13:34:12.000000 liba-0.1.9.post1/include/a/fuzzy.h
+-rwxrwxrwx   0 root         (0) root         (0)     3171 2024-03-30 14:06:42.000000 liba-0.1.9.post1/include/a/hpf.h
+-rwxrwxrwx   0 root         (0) root         (0)    13295 2024-03-28 13:34:12.000000 liba-0.1.9.post1/include/a/list.h
+-rwxrwxrwx   0 root         (0) root         (0)     2989 2024-03-30 14:06:42.000000 liba-0.1.9.post1/include/a/lpf.h
+-rwxrwxrwx   0 root         (0) root         (0)    10506 2024-03-18 13:04:44.000000 liba-0.1.9.post1/include/a/math.h
+-rwxrwxrwx   0 root         (0) root         (0)     9317 2024-03-18 13:04:44.000000 liba-0.1.9.post1/include/a/mf.h
+-rwxrwxrwx   0 root         (0) root         (0)   111612 2024-03-18 13:04:44.000000 liba-0.1.9.post1/include/a/notefreqs.h
+-rwxrwxrwx   0 root         (0) root         (0)     2291 2024-03-18 13:04:44.000000 liba-0.1.9.post1/include/a/operator.h
+-rwxrwxrwx   0 root         (0) root         (0)     4081 2024-03-28 13:34:12.000000 liba-0.1.9.post1/include/a/pid.h
+-rwxrwxrwx   0 root         (0) root         (0)     6670 2024-03-28 13:34:12.000000 liba-0.1.9.post1/include/a/pid_fuzzy.h
+-rwxrwxrwx   0 root         (0) root         (0)     3748 2024-03-28 13:34:12.000000 liba-0.1.9.post1/include/a/pid_neuro.h
+-rwxrwxrwx   0 root         (0) root         (0)     1948 2024-03-18 13:04:44.000000 liba-0.1.9.post1/include/a/poly.h
+-rwxrwxrwx   0 root         (0) root         (0)     9622 2024-03-30 14:06:42.000000 liba-0.1.9.post1/include/a/que.h
+-rwxrwxrwx   0 root         (0) root         (0)    10091 2024-03-28 13:34:12.000000 liba-0.1.9.post1/include/a/rbt.h
+-rwxrwxrwx   0 root         (0) root         (0)     5228 2024-03-18 13:04:44.000000 liba-0.1.9.post1/include/a/slist.h
+-rwxrwxrwx   0 root         (0) root         (0)     8624 2024-03-28 13:34:12.000000 liba-0.1.9.post1/include/a/str.h
+-rwxrwxrwx   0 root         (0) root         (0)     2969 2024-03-28 13:34:12.000000 liba-0.1.9.post1/include/a/tf.h
+-rwxrwxrwx   0 root         (0) root         (0)     7440 2024-03-28 13:34:12.000000 liba-0.1.9.post1/include/a/trajbell.h
+-rwxrwxrwx   0 root         (0) root         (0)     4853 2024-03-28 13:34:12.000000 liba-0.1.9.post1/include/a/trajpoly3.h
+-rwxrwxrwx   0 root         (0) root         (0)     5768 2024-03-28 13:34:12.000000 liba-0.1.9.post1/include/a/trajpoly5.h
+-rwxrwxrwx   0 root         (0) root         (0)     7895 2024-03-28 13:34:12.000000 liba-0.1.9.post1/include/a/trajpoly7.h
+-rwxrwxrwx   0 root         (0) root         (0)     4904 2024-03-28 13:34:12.000000 liba-0.1.9.post1/include/a/trajtrap.h
+-rwxrwxrwx   0 root         (0) root         (0)     1603 2024-03-18 13:04:44.000000 liba-0.1.9.post1/include/a/utf.h
+-rwxrwxrwx   0 root         (0) root         (0)    12780 2024-03-28 13:34:12.000000 liba-0.1.9.post1/include/a/vec.h
+-rwxrwxrwx   0 root         (0) root         (0)     6914 2024-03-30 14:06:42.000000 liba-0.1.9.post1/include/a/version.h
+-rwxrwxrwx   0 root         (0) root         (0)       92 2024-03-18 13:04:44.000000 liba-0.1.9.post1/pyproject.toml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-31 04:05:35.661740 liba-0.1.9.post1/python/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-31 04:05:35.745915 liba-0.1.9.post1/python/liba.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     5056 2024-03-31 04:05:35.000000 liba-0.1.9.post1/python/liba.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1498 2024-03-31 04:05:35.000000 liba-0.1.9.post1/python/liba.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-03-31 04:05:35.000000 liba-0.1.9.post1/python/liba.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        6 2024-03-31 04:05:35.000000 liba-0.1.9.post1/python/liba.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-31 04:05:35.748398 liba-0.1.9.post1/python/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-31 04:05:35.780486 liba-0.1.9.post1/python/src/a/
+-rwxrwxrwx   0 root         (0) root         (0)     1307 2024-03-28 13:34:12.000000 liba-0.1.9.post1/python/src/a/__init__.pxd
+-rwxrwxrwx   0 root         (0) root         (0)     1022 2024-03-18 13:04:44.000000 liba-0.1.9.post1/python/src/a/crc.pxd
+-rwxrwxrwx   0 root         (0) root         (0)      499 2024-03-28 13:34:12.000000 liba-0.1.9.post1/python/src/a/fuzzy.pxd
+-rwxrwxrwx   0 root         (0) root         (0)      311 2024-03-18 13:04:44.000000 liba-0.1.9.post1/python/src/a/hpf.pxd
+-rwxrwxrwx   0 root         (0) root         (0)      289 2024-03-18 13:04:44.000000 liba-0.1.9.post1/python/src/a/lpf.pxd
+-rwxrwxrwx   0 root         (0) root         (0)      193 2024-03-18 13:04:44.000000 liba-0.1.9.post1/python/src/a/math.pxd
+-rwxrwxrwx   0 root         (0) root         (0)     1305 2024-03-18 13:04:44.000000 liba-0.1.9.post1/python/src/a/mf.pxd
+-rwxrwxrwx   0 root         (0) root         (0)      614 2024-03-28 13:34:12.000000 liba-0.1.9.post1/python/src/a/pid.pxd
+-rwxrwxrwx   0 root         (0) root         (0)     1332 2024-03-28 13:34:12.000000 liba-0.1.9.post1/python/src/a/pid_fuzzy.pxd
+-rwxrwxrwx   0 root         (0) root         (0)      604 2024-03-18 13:04:44.000000 liba-0.1.9.post1/python/src/a/pid_neuro.pxd
+-rwxrwxrwx   0 root         (0) root         (0)      232 2024-03-18 13:04:44.000000 liba-0.1.9.post1/python/src/a/poly.pxd
+-rwxrwxrwx   0 root         (0) root         (0)      499 2024-03-18 13:04:44.000000 liba-0.1.9.post1/python/src/a/tf.pxd
+-rwxrwxrwx   0 root         (0) root         (0)      750 2024-03-28 13:31:42.000000 liba-0.1.9.post1/python/src/a/trajbell.pxd
+-rwxrwxrwx   0 root         (0) root         (0)      461 2024-03-31 04:02:52.000000 liba-0.1.9.post1/python/src/a/trajpoly3.pxd
+-rwxrwxrwx   0 root         (0) root         (0)      485 2024-03-31 04:02:52.000000 liba-0.1.9.post1/python/src/a/trajpoly5.pxd
+-rwxrwxrwx   0 root         (0) root         (0)      600 2024-03-31 04:02:52.000000 liba-0.1.9.post1/python/src/a/trajpoly7.pxd
+-rwxrwxrwx   0 root         (0) root         (0)      642 2024-03-28 13:31:42.000000 liba-0.1.9.post1/python/src/a/trajtrap.pxd
+-rwxrwxrwx   0 root         (0) root         (0)     1245 2024-03-31 04:02:52.000000 liba-0.1.9.post1/python/src/a/version.pxd
+-rwxrwxrwx   0 root         (0) root         (0)  2100208 2024-03-31 04:05:16.000000 liba-0.1.9.post1/python/src/a.c
+-rwxrwxrwx   0 root         (0) root         (0)    40552 2024-03-31 04:02:52.000000 liba-0.1.9.post1/python/src/a.pyx
+-rwxrwxrwx   0 root         (0) root         (0)      635 2024-03-31 04:05:35.821566 liba-0.1.9.post1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     5074 2024-03-31 04:02:52.000000 liba-0.1.9.post1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-31 04:05:35.814354 liba-0.1.9.post1/src/
+-rwxrwxrwx   0 root         (0) root         (0)     2761 2024-03-18 13:04:44.000000 liba-0.1.9.post1/src/a.c
+-rwxrwxrwx   0 root         (0) root         (0)    23944 2024-03-28 13:34:12.000000 liba-0.1.9.post1/src/avl.c
+-rwxrwxrwx   0 root         (0) root         (0)     4167 2024-03-28 13:34:12.000000 liba-0.1.9.post1/src/buf.c
+-rwxrwxrwx   0 root         (0) root         (0)    25134 2024-03-18 13:04:44.000000 liba-0.1.9.post1/src/complex.c
+-rwxrwxrwx   0 root         (0) root         (0)     4875 2024-03-28 13:31:47.000000 liba-0.1.9.post1/src/crc.c
+-rwxrwxrwx   0 root         (0) root         (0)      328 2024-03-28 13:34:12.000000 liba-0.1.9.post1/src/fuzzy.c
+-rwxrwxrwx   0 root         (0) root         (0)     6113 2024-03-28 13:34:12.000000 liba-0.1.9.post1/src/math.c
+-rwxrwxrwx   0 root         (0) root         (0)     4500 2024-03-18 13:04:44.000000 liba-0.1.9.post1/src/mf.c
+-rwxrwxrwx   0 root         (0) root         (0)     2127 2024-03-28 13:34:12.000000 liba-0.1.9.post1/src/pid.c
+-rwxrwxrwx   0 root         (0) root         (0)     6574 2024-03-28 13:34:12.000000 liba-0.1.9.post1/src/pid_fuzzy.c
+-rwxrwxrwx   0 root         (0) root         (0)     1819 2024-03-28 13:34:12.000000 liba-0.1.9.post1/src/pid_neuro.c
+-rwxrwxrwx   0 root         (0) root         (0)      561 2024-03-28 13:59:44.000000 liba-0.1.9.post1/src/poly.c
+-rwxrwxrwx   0 root         (0) root         (0)     7685 2024-03-31 04:02:52.000000 liba-0.1.9.post1/src/que.c
+-rwxrwxrwx   0 root         (0) root         (0)    22692 2024-03-28 13:34:12.000000 liba-0.1.9.post1/src/rbt.c
+-rwxrwxrwx   0 root         (0) root         (0)     5713 2024-03-28 13:34:12.000000 liba-0.1.9.post1/src/str.c
+-rwxrwxrwx   0 root         (0) root         (0)     1269 2024-03-18 13:04:44.000000 liba-0.1.9.post1/src/tf.c
+-rwxrwxrwx   0 root         (0) root         (0)     8585 2024-03-28 13:34:12.000000 liba-0.1.9.post1/src/trajbell.c
+-rwxrwxrwx   0 root         (0) root         (0)     1811 2024-03-28 13:31:42.000000 liba-0.1.9.post1/src/trajpoly3.c
+-rwxrwxrwx   0 root         (0) root         (0)     2466 2024-03-28 13:31:42.000000 liba-0.1.9.post1/src/trajpoly5.c
+-rwxrwxrwx   0 root         (0) root         (0)     3713 2024-03-28 13:31:42.000000 liba-0.1.9.post1/src/trajpoly7.c
+-rwxrwxrwx   0 root         (0) root         (0)     3816 2024-03-28 13:34:12.000000 liba-0.1.9.post1/src/trajtrap.c
+-rwxrwxrwx   0 root         (0) root         (0)     2872 2024-03-18 13:04:44.000000 liba-0.1.9.post1/src/utf.c
+-rwxrwxrwx   0 root         (0) root         (0)     6064 2024-03-28 13:59:44.000000 liba-0.1.9.post1/src/vec.c
+-rwxrwxrwx   0 root         (0) root         (0)     5535 2024-03-28 13:34:12.000000 liba-0.1.9.post1/src/version.c
```

### Comparing `liba-0.1.9/LICENSE.txt` & `liba-0.1.9.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/PKG-INFO` & `liba-0.1.9.post1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,241 +1,241 @@
-Metadata-Version: 2.1
-Name: liba
-Version: 0.1.9
-Summary: An algorithm library based on C/C++ language
-Home-page: https://github.com/tqfx/liba.git
-Author: tqfx
-Author-email: tqfx@tqfx.org
-License: MPL-2.0
-Keywords: algorithms
-Platform: CPython
-Classifier: Programming Language :: C
-Classifier: Programming Language :: C++
-Classifier: Programming Language :: Cython
-Classifier: Programming Language :: Python
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# An algorithm library {#mainpage}
-
-[![docs](https://github.com/tqfx/liba/actions/workflows/docs.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/docs.yml)
-[![conan](https://github.com/tqfx/liba/actions/workflows/conan.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/conan.yml)
-[![xmake](https://github.com/tqfx/liba/actions/workflows/xmake.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/xmake.yml)
-[![meson](https://github.com/tqfx/liba/actions/workflows/meson.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/meson.yml)
-[![msvc](https://github.com/tqfx/liba/actions/workflows/msvc.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/msvc.yml)
-[![linux](https://github.com/tqfx/liba/actions/workflows/linux.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/linux.yml)
-[![macos](https://github.com/tqfx/liba/actions/workflows/macos.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/macos.yml)
-[![mingw](https://github.com/tqfx/liba/actions/workflows/mingw.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/mingw.yml)
-[![msys2](https://github.com/tqfx/liba/actions/workflows/msys2.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/msys2.yml)
-[![freebsd](https://github.com/tqfx/liba/actions/workflows/freebsd.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/freebsd.yml)
-
-## documentation
-
-- [C/C++](https://tqfx.org/liba/)
-- [Lua](https://tqfx.org/liba/lua/)
-- [Java](https://tqfx.org/liba/java/)
-- [Rust](https://tqfx.org/liba/rust/liba/)
-
-## required tools
-
-- C/C++ compiler: [tcc](https://bellard.org/tcc) or [gnu](https://gcc.gnu.org) or [llvm](https://clang.llvm.org) or [msvc](https://visualstudio.microsoft.com/visual-cpp-build-tools) etc
-
-## optional tools
-
-- [lua](https://www.lua.org)
-- [java](https://www.oracle.com/java)
-- [rust](https://www.rust-lang.org)
-- [emsdk](https://emscripten.org)
-- [xmake](https://xmake.io)
-- [cmake](https://cmake.org)
-- [conan](https://conan.io)
-- [vcpkg](https://vcpkg.io)
-- [meson](https://mesonbuild.com)
-- [python](https://www.python.org)
-- [quickjs](https://github.com/bellard/quickjs)
-
-## build
-
-### xmake
-
-```bash
-xmake f
-xmake
-xmake i
-```
-
-### cmake
-
-```bash
-cmake -S . -B build
-cmake --build build
-cmake --install build
-```
-
-### meson
-
-```bash
-meson setup builddir
-meson install -C builddir
-```
-
-### vcpkg
-
-```bash
-cmake -S . -B build -DLIBA_VCPKG=1
-```
-
-```bash
-cp -r build/vcpkg/* $VCPKG_INSTALLATION_ROOT
-```
-
-```pwsh
-cp -r -Force build/vcpkg/* $ENV:VCPKG_INSTALLATION_ROOT
-```
-
-### conan
-
-```bash
-conan create .
-```
-
-### cargo
-
-```bash
-cargo build --release
-```
-
-### cython
-
-```bash
-python setup.py build_ext --inplace
-```
-
-## usage
-
-### C/C++
-
-#### xmake.lua
-
-```lua
-add_requires("alib") -- static
-add_requires("liba") -- shared
-```
-
-#### CMakeLists.txt
-
-```cmake
-find_package(liba CONFIG REQUIRED)
-target_link_libraries(<TARGET> PRIVATE alib) # static
-target_link_libraries(<TARGET> PRIVATE liba) # shared
-```
-
-#### conanfile.txt
-
-```txt
-[requires]
-liba/[~0.1]
-```
-
-### Lua
-
-```bash
-luarocks install liba # release
-```
-
-```bash
-luarocks install liba --dev # latest
-```
-
-#### main.lua
-
-```lua
-local liba = require("liba")
-print("version", liba.VERSION)
-```
-
-### Java
-
-#### Main.java
-
-```java
-public class Main {
-    public static void main(String[] args) {
-        System.out.println("version " + liba.VERSION);
-    }
-}
-```
-
-### Rust
-
-#### Cargo.toml
-
-```bash
-cargo add liba # release
-```
-
-```bash
-cargo add --git https://github.com/tqfx/liba.git # latest
-```
-
-#### main.rs
-
-```rs
-use liba;
-fn main() {
-    println!(
-        "version {}.{}.{}+{}",
-        liba::version::major(),
-        liba::version::minor(),
-        liba::version::patch(),
-        liba::version::tweak()
-    );
-}
-```
-
-### Python
-
-```bash
-pip install liba # release
-```
-
-```bash
-pip install git+https://github.com/tqfx/liba.git # latest
-```
-
-#### main.py
-
-```py
-import liba
-print("version", liba.VERSION)
-```
-
-### JavaScript
-
-```bash
-npm i @tqfx/liba
-```
-
-#### index.js
-
-```js
-import liba from "@tqfx/liba";
-console.log("version", liba.VERSION);
-```
-
-### QuickJS
-
-#### main.js
-
-```js
-import * as liba from "liba.so";
-console.log("version", liba.VERSION);
-```
-
-## Copyright {#copyright}
-
-Copyright (C) 2020-present tqfx, All rights reserved.
-
-This Source Code Form is subject to the terms of the Mozilla Public
-License, v. 2.0. If a copy of the MPL was not distributed with this
-file, You can obtain one at <https://mozilla.org/MPL/2.0/>.
+Metadata-Version: 2.1
+Name: liba
+Version: 0.1.9.post1
+Summary: An algorithm library based on C/C++ language
+Home-page: https://github.com/tqfx/liba.git
+Author: tqfx
+Author-email: tqfx@tqfx.org
+License: MPL-2.0
+Keywords: algorithms
+Platform: CPython
+Classifier: Programming Language :: C
+Classifier: Programming Language :: C++
+Classifier: Programming Language :: Cython
+Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# An algorithm library {#mainpage}
+
+[![docs](https://github.com/tqfx/liba/actions/workflows/docs.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/docs.yml)
+[![conan](https://github.com/tqfx/liba/actions/workflows/conan.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/conan.yml)
+[![xmake](https://github.com/tqfx/liba/actions/workflows/xmake.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/xmake.yml)
+[![meson](https://github.com/tqfx/liba/actions/workflows/meson.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/meson.yml)
+[![msvc](https://github.com/tqfx/liba/actions/workflows/msvc.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/msvc.yml)
+[![linux](https://github.com/tqfx/liba/actions/workflows/linux.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/linux.yml)
+[![macos](https://github.com/tqfx/liba/actions/workflows/macos.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/macos.yml)
+[![mingw](https://github.com/tqfx/liba/actions/workflows/mingw.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/mingw.yml)
+[![msys2](https://github.com/tqfx/liba/actions/workflows/msys2.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/msys2.yml)
+[![freebsd](https://github.com/tqfx/liba/actions/workflows/freebsd.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/freebsd.yml)
+
+## documentation
+
+- [C/C++](https://tqfx.org/liba/)
+- [Lua](https://tqfx.org/liba/lua/)
+- [Java](https://tqfx.org/liba/java/)
+- [Rust](https://tqfx.org/liba/rust/liba/)
+
+## required tools
+
+- C/C++ compiler: [tcc](https://bellard.org/tcc) or [gnu](https://gcc.gnu.org) or [llvm](https://clang.llvm.org) or [msvc](https://visualstudio.microsoft.com/visual-cpp-build-tools) etc
+
+## optional tools
+
+- [lua](https://www.lua.org)
+- [java](https://www.oracle.com/java)
+- [rust](https://www.rust-lang.org)
+- [emsdk](https://emscripten.org)
+- [xmake](https://xmake.io)
+- [cmake](https://cmake.org)
+- [conan](https://conan.io)
+- [vcpkg](https://vcpkg.io)
+- [meson](https://mesonbuild.com)
+- [python](https://www.python.org)
+- [quickjs](https://github.com/bellard/quickjs)
+
+## build
+
+### xmake
+
+```bash
+xmake f
+xmake
+xmake i
+```
+
+### cmake
+
+```bash
+cmake -S . -B build
+cmake --build build
+cmake --install build
+```
+
+### meson
+
+```bash
+meson setup builddir
+meson install -C builddir
+```
+
+### vcpkg
+
+```bash
+cmake -S . -B build -DLIBA_VCPKG=1
+```
+
+```bash
+cp -r build/vcpkg/* $VCPKG_INSTALLATION_ROOT
+```
+
+```pwsh
+cp -r -Force build/vcpkg/* $ENV:VCPKG_INSTALLATION_ROOT
+```
+
+### conan
+
+```bash
+conan create .
+```
+
+### cargo
+
+```bash
+cargo build --release
+```
+
+### cython
+
+```bash
+python setup.py build_ext --inplace
+```
+
+## usage
+
+### C/C++
+
+#### xmake.lua
+
+```lua
+add_requires("alib") -- static
+add_requires("liba") -- shared
+```
+
+#### CMakeLists.txt
+
+```cmake
+find_package(liba CONFIG REQUIRED)
+target_link_libraries(<TARGET> PRIVATE alib) # static
+target_link_libraries(<TARGET> PRIVATE liba) # shared
+```
+
+#### conanfile.txt
+
+```txt
+[requires]
+liba/[~0.1]
+```
+
+### Lua
+
+```bash
+luarocks install liba # release
+```
+
+```bash
+luarocks install liba --dev # latest
+```
+
+#### main.lua
+
+```lua
+local liba = require("liba")
+print("version", liba.VERSION)
+```
+
+### Java
+
+#### Main.java
+
+```java
+public class Main {
+    public static void main(String[] args) {
+        System.out.println("version " + liba.VERSION);
+    }
+}
+```
+
+### Rust
+
+#### Cargo.toml
+
+```bash
+cargo add liba # release
+```
+
+```bash
+cargo add --git https://github.com/tqfx/liba.git # latest
+```
+
+#### main.rs
+
+```rs
+use liba;
+fn main() {
+    println!(
+        "version {}.{}.{}+{}",
+        liba::version::major(),
+        liba::version::minor(),
+        liba::version::patch(),
+        liba::version::tweak()
+    );
+}
+```
+
+### Python
+
+```bash
+pip install liba # release
+```
+
+```bash
+pip install git+https://github.com/tqfx/liba.git # latest
+```
+
+#### main.py
+
+```py
+import liba
+print("version", liba.VERSION)
+```
+
+### JavaScript
+
+```bash
+npm i @tqfx/liba
+```
+
+#### index.js
+
+```js
+import liba from "@tqfx/liba";
+console.log("version", liba.VERSION);
+```
+
+### QuickJS
+
+#### main.js
+
+```js
+import * as liba from "liba.so";
+console.log("version", liba.VERSION);
+```
+
+## Copyright {#copyright}
+
+Copyright (C) 2020-present tqfx, All rights reserved.
+
+This Source Code Form is subject to the terms of the Mozilla Public
+License, v. 2.0. If a copy of the MPL was not distributed with this
+file, You can obtain one at <https://mozilla.org/MPL/2.0/>.
```

### Comparing `liba-0.1.9/README.md` & `liba-0.1.9.post1/README.md`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/a.h` & `liba-0.1.9.post1/include/a/a.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/avl.h` & `liba-0.1.9.post1/include/a/avl.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/buf.h` & `liba-0.1.9.post1/include/a/buf.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/complex.h` & `liba-0.1.9.post1/include/a/complex.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/crc.h` & `liba-0.1.9.post1/include/a/crc.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/fuzzy.h` & `liba-0.1.9.post1/include/a/fuzzy.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/hpf.h` & `liba-0.1.9.post1/include/a/hpf.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/list.h` & `liba-0.1.9.post1/include/a/list.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/lpf.h` & `liba-0.1.9.post1/include/a/lpf.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/math.h` & `liba-0.1.9.post1/include/a/math.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/mf.h` & `liba-0.1.9.post1/include/a/mf.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/notefreqs.h` & `liba-0.1.9.post1/include/a/notefreqs.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/operator.h` & `liba-0.1.9.post1/include/a/operator.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/pid.h` & `liba-0.1.9.post1/include/a/pid.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/pid_fuzzy.h` & `liba-0.1.9.post1/include/a/pid_fuzzy.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/pid_neuro.h` & `liba-0.1.9.post1/include/a/pid_neuro.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/poly.h` & `liba-0.1.9.post1/include/a/poly.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/que.h` & `liba-0.1.9.post1/include/a/que.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/rbt.h` & `liba-0.1.9.post1/include/a/rbt.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/slist.h` & `liba-0.1.9.post1/include/a/slist.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/str.h` & `liba-0.1.9.post1/include/a/str.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/tf.h` & `liba-0.1.9.post1/include/a/tf.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/trajbell.h` & `liba-0.1.9.post1/include/a/trajbell.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/trajpoly3.h` & `liba-0.1.9.post1/include/a/trajpoly3.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/trajpoly5.h` & `liba-0.1.9.post1/include/a/trajpoly5.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/trajpoly7.h` & `liba-0.1.9.post1/include/a/trajpoly7.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/trajtrap.h` & `liba-0.1.9.post1/include/a/trajtrap.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/utf.h` & `liba-0.1.9.post1/include/a/utf.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/vec.h` & `liba-0.1.9.post1/include/a/vec.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/include/a/version.h` & `liba-0.1.9.post1/include/a/version.h`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/python/liba.egg-info/PKG-INFO` & `liba-0.1.9.post1/python/liba.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,241 +1,241 @@
-Metadata-Version: 2.1
-Name: liba
-Version: 0.1.9
-Summary: An algorithm library based on C/C++ language
-Home-page: https://github.com/tqfx/liba.git
-Author: tqfx
-Author-email: tqfx@tqfx.org
-License: MPL-2.0
-Keywords: algorithms
-Platform: CPython
-Classifier: Programming Language :: C
-Classifier: Programming Language :: C++
-Classifier: Programming Language :: Cython
-Classifier: Programming Language :: Python
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# An algorithm library {#mainpage}
-
-[![docs](https://github.com/tqfx/liba/actions/workflows/docs.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/docs.yml)
-[![conan](https://github.com/tqfx/liba/actions/workflows/conan.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/conan.yml)
-[![xmake](https://github.com/tqfx/liba/actions/workflows/xmake.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/xmake.yml)
-[![meson](https://github.com/tqfx/liba/actions/workflows/meson.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/meson.yml)
-[![msvc](https://github.com/tqfx/liba/actions/workflows/msvc.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/msvc.yml)
-[![linux](https://github.com/tqfx/liba/actions/workflows/linux.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/linux.yml)
-[![macos](https://github.com/tqfx/liba/actions/workflows/macos.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/macos.yml)
-[![mingw](https://github.com/tqfx/liba/actions/workflows/mingw.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/mingw.yml)
-[![msys2](https://github.com/tqfx/liba/actions/workflows/msys2.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/msys2.yml)
-[![freebsd](https://github.com/tqfx/liba/actions/workflows/freebsd.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/freebsd.yml)
-
-## documentation
-
-- [C/C++](https://tqfx.org/liba/)
-- [Lua](https://tqfx.org/liba/lua/)
-- [Java](https://tqfx.org/liba/java/)
-- [Rust](https://tqfx.org/liba/rust/liba/)
-
-## required tools
-
-- C/C++ compiler: [tcc](https://bellard.org/tcc) or [gnu](https://gcc.gnu.org) or [llvm](https://clang.llvm.org) or [msvc](https://visualstudio.microsoft.com/visual-cpp-build-tools) etc
-
-## optional tools
-
-- [lua](https://www.lua.org)
-- [java](https://www.oracle.com/java)
-- [rust](https://www.rust-lang.org)
-- [emsdk](https://emscripten.org)
-- [xmake](https://xmake.io)
-- [cmake](https://cmake.org)
-- [conan](https://conan.io)
-- [vcpkg](https://vcpkg.io)
-- [meson](https://mesonbuild.com)
-- [python](https://www.python.org)
-- [quickjs](https://github.com/bellard/quickjs)
-
-## build
-
-### xmake
-
-```bash
-xmake f
-xmake
-xmake i
-```
-
-### cmake
-
-```bash
-cmake -S . -B build
-cmake --build build
-cmake --install build
-```
-
-### meson
-
-```bash
-meson setup builddir
-meson install -C builddir
-```
-
-### vcpkg
-
-```bash
-cmake -S . -B build -DLIBA_VCPKG=1
-```
-
-```bash
-cp -r build/vcpkg/* $VCPKG_INSTALLATION_ROOT
-```
-
-```pwsh
-cp -r -Force build/vcpkg/* $ENV:VCPKG_INSTALLATION_ROOT
-```
-
-### conan
-
-```bash
-conan create .
-```
-
-### cargo
-
-```bash
-cargo build --release
-```
-
-### cython
-
-```bash
-python setup.py build_ext --inplace
-```
-
-## usage
-
-### C/C++
-
-#### xmake.lua
-
-```lua
-add_requires("alib") -- static
-add_requires("liba") -- shared
-```
-
-#### CMakeLists.txt
-
-```cmake
-find_package(liba CONFIG REQUIRED)
-target_link_libraries(<TARGET> PRIVATE alib) # static
-target_link_libraries(<TARGET> PRIVATE liba) # shared
-```
-
-#### conanfile.txt
-
-```txt
-[requires]
-liba/[~0.1]
-```
-
-### Lua
-
-```bash
-luarocks install liba # release
-```
-
-```bash
-luarocks install liba --dev # latest
-```
-
-#### main.lua
-
-```lua
-local liba = require("liba")
-print("version", liba.VERSION)
-```
-
-### Java
-
-#### Main.java
-
-```java
-public class Main {
-    public static void main(String[] args) {
-        System.out.println("version " + liba.VERSION);
-    }
-}
-```
-
-### Rust
-
-#### Cargo.toml
-
-```bash
-cargo add liba # release
-```
-
-```bash
-cargo add --git https://github.com/tqfx/liba.git # latest
-```
-
-#### main.rs
-
-```rs
-use liba;
-fn main() {
-    println!(
-        "version {}.{}.{}+{}",
-        liba::version::major(),
-        liba::version::minor(),
-        liba::version::patch(),
-        liba::version::tweak()
-    );
-}
-```
-
-### Python
-
-```bash
-pip install liba # release
-```
-
-```bash
-pip install git+https://github.com/tqfx/liba.git # latest
-```
-
-#### main.py
-
-```py
-import liba
-print("version", liba.VERSION)
-```
-
-### JavaScript
-
-```bash
-npm i @tqfx/liba
-```
-
-#### index.js
-
-```js
-import liba from "@tqfx/liba";
-console.log("version", liba.VERSION);
-```
-
-### QuickJS
-
-#### main.js
-
-```js
-import * as liba from "liba.so";
-console.log("version", liba.VERSION);
-```
-
-## Copyright {#copyright}
-
-Copyright (C) 2020-present tqfx, All rights reserved.
-
-This Source Code Form is subject to the terms of the Mozilla Public
-License, v. 2.0. If a copy of the MPL was not distributed with this
-file, You can obtain one at <https://mozilla.org/MPL/2.0/>.
+Metadata-Version: 2.1
+Name: liba
+Version: 0.1.9.post1
+Summary: An algorithm library based on C/C++ language
+Home-page: https://github.com/tqfx/liba.git
+Author: tqfx
+Author-email: tqfx@tqfx.org
+License: MPL-2.0
+Keywords: algorithms
+Platform: CPython
+Classifier: Programming Language :: C
+Classifier: Programming Language :: C++
+Classifier: Programming Language :: Cython
+Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# An algorithm library {#mainpage}
+
+[![docs](https://github.com/tqfx/liba/actions/workflows/docs.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/docs.yml)
+[![conan](https://github.com/tqfx/liba/actions/workflows/conan.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/conan.yml)
+[![xmake](https://github.com/tqfx/liba/actions/workflows/xmake.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/xmake.yml)
+[![meson](https://github.com/tqfx/liba/actions/workflows/meson.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/meson.yml)
+[![msvc](https://github.com/tqfx/liba/actions/workflows/msvc.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/msvc.yml)
+[![linux](https://github.com/tqfx/liba/actions/workflows/linux.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/linux.yml)
+[![macos](https://github.com/tqfx/liba/actions/workflows/macos.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/macos.yml)
+[![mingw](https://github.com/tqfx/liba/actions/workflows/mingw.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/mingw.yml)
+[![msys2](https://github.com/tqfx/liba/actions/workflows/msys2.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/msys2.yml)
+[![freebsd](https://github.com/tqfx/liba/actions/workflows/freebsd.yml/badge.svg)](https://github.com/tqfx/liba/actions/workflows/freebsd.yml)
+
+## documentation
+
+- [C/C++](https://tqfx.org/liba/)
+- [Lua](https://tqfx.org/liba/lua/)
+- [Java](https://tqfx.org/liba/java/)
+- [Rust](https://tqfx.org/liba/rust/liba/)
+
+## required tools
+
+- C/C++ compiler: [tcc](https://bellard.org/tcc) or [gnu](https://gcc.gnu.org) or [llvm](https://clang.llvm.org) or [msvc](https://visualstudio.microsoft.com/visual-cpp-build-tools) etc
+
+## optional tools
+
+- [lua](https://www.lua.org)
+- [java](https://www.oracle.com/java)
+- [rust](https://www.rust-lang.org)
+- [emsdk](https://emscripten.org)
+- [xmake](https://xmake.io)
+- [cmake](https://cmake.org)
+- [conan](https://conan.io)
+- [vcpkg](https://vcpkg.io)
+- [meson](https://mesonbuild.com)
+- [python](https://www.python.org)
+- [quickjs](https://github.com/bellard/quickjs)
+
+## build
+
+### xmake
+
+```bash
+xmake f
+xmake
+xmake i
+```
+
+### cmake
+
+```bash
+cmake -S . -B build
+cmake --build build
+cmake --install build
+```
+
+### meson
+
+```bash
+meson setup builddir
+meson install -C builddir
+```
+
+### vcpkg
+
+```bash
+cmake -S . -B build -DLIBA_VCPKG=1
+```
+
+```bash
+cp -r build/vcpkg/* $VCPKG_INSTALLATION_ROOT
+```
+
+```pwsh
+cp -r -Force build/vcpkg/* $ENV:VCPKG_INSTALLATION_ROOT
+```
+
+### conan
+
+```bash
+conan create .
+```
+
+### cargo
+
+```bash
+cargo build --release
+```
+
+### cython
+
+```bash
+python setup.py build_ext --inplace
+```
+
+## usage
+
+### C/C++
+
+#### xmake.lua
+
+```lua
+add_requires("alib") -- static
+add_requires("liba") -- shared
+```
+
+#### CMakeLists.txt
+
+```cmake
+find_package(liba CONFIG REQUIRED)
+target_link_libraries(<TARGET> PRIVATE alib) # static
+target_link_libraries(<TARGET> PRIVATE liba) # shared
+```
+
+#### conanfile.txt
+
+```txt
+[requires]
+liba/[~0.1]
+```
+
+### Lua
+
+```bash
+luarocks install liba # release
+```
+
+```bash
+luarocks install liba --dev # latest
+```
+
+#### main.lua
+
+```lua
+local liba = require("liba")
+print("version", liba.VERSION)
+```
+
+### Java
+
+#### Main.java
+
+```java
+public class Main {
+    public static void main(String[] args) {
+        System.out.println("version " + liba.VERSION);
+    }
+}
+```
+
+### Rust
+
+#### Cargo.toml
+
+```bash
+cargo add liba # release
+```
+
+```bash
+cargo add --git https://github.com/tqfx/liba.git # latest
+```
+
+#### main.rs
+
+```rs
+use liba;
+fn main() {
+    println!(
+        "version {}.{}.{}+{}",
+        liba::version::major(),
+        liba::version::minor(),
+        liba::version::patch(),
+        liba::version::tweak()
+    );
+}
+```
+
+### Python
+
+```bash
+pip install liba # release
+```
+
+```bash
+pip install git+https://github.com/tqfx/liba.git # latest
+```
+
+#### main.py
+
+```py
+import liba
+print("version", liba.VERSION)
+```
+
+### JavaScript
+
+```bash
+npm i @tqfx/liba
+```
+
+#### index.js
+
+```js
+import liba from "@tqfx/liba";
+console.log("version", liba.VERSION);
+```
+
+### QuickJS
+
+#### main.js
+
+```js
+import * as liba from "liba.so";
+console.log("version", liba.VERSION);
+```
+
+## Copyright {#copyright}
+
+Copyright (C) 2020-present tqfx, All rights reserved.
+
+This Source Code Form is subject to the terms of the Mozilla Public
+License, v. 2.0. If a copy of the MPL was not distributed with this
+file, You can obtain one at <https://mozilla.org/MPL/2.0/>.
```

### Comparing `liba-0.1.9/python/liba.egg-info/SOURCES.txt` & `liba-0.1.9.post1/python/liba.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 include/a/trajpoly3.h
 include/a/trajpoly5.h
 include/a/trajpoly7.h
 include/a/trajtrap.h
 include/a/utf.h
 include/a/vec.h
 include/a/version.h
-python/src/a.c
 python/liba.egg-info/PKG-INFO
 python/liba.egg-info/SOURCES.txt
 python/liba.egg-info/dependency_links.txt
 python/liba.egg-info/top_level.txt
 python/src/a.c
 python/src/a.pyx
 python/src/a/__init__.pxd
```

### Comparing `liba-0.1.9/python/src/a/__init__.pxd` & `liba-0.1.9.post1/python/src/a/__init__.pxd`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/python/src/a/crc.pxd` & `liba-0.1.9.post1/python/src/a/crc.pxd`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/python/src/a/mf.pxd` & `liba-0.1.9.post1/python/src/a/mf.pxd`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/python/src/a/pid.pxd` & `liba-0.1.9.post1/python/src/a/pid.pxd`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/python/src/a/pid_fuzzy.pxd` & `liba-0.1.9.post1/python/src/a/pid_fuzzy.pxd`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/python/src/a/pid_neuro.pxd` & `liba-0.1.9.post1/python/src/a/pid_neuro.pxd`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/python/src/a/trajbell.pxd` & `liba-0.1.9.post1/python/src/a/trajbell.pxd`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/python/src/a/trajpoly7.pxd` & `liba-0.1.9.post1/python/src/a/trajpoly7.pxd`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/python/src/a/trajtrap.pxd` & `liba-0.1.9.post1/python/src/a/trajtrap.pxd`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/python/src/a/version.pxd` & `liba-0.1.9.post1/python/src/a/version.pxd`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/python/src/a.c` & `liba-0.1.9.post1/python/src/a.c`

 * *Files 0% similar despite different names*

```diff
@@ -2,72 +2,72 @@
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "A_HAVE_H",
-                "\"..\\..\\build\\a.setup.h\""
+                "\"../../build/a.setup.h\""
             ],
             [
                 "A_EXPORTS",
                 null
             ]
         ],
         "depends": [
-            "include\\a\\a.h",
-            "include\\a\\crc.h",
-            "include\\a\\fuzzy.h",
-            "include\\a\\hpf.h",
-            "include\\a\\lpf.h",
-            "include\\a\\math.h",
-            "include\\a\\mf.h",
-            "include\\a\\pid.h",
-            "include\\a\\pid_fuzzy.h",
-            "include\\a\\pid_neuro.h",
-            "include\\a\\poly.h",
-            "include\\a\\tf.h",
-            "include\\a\\trajbell.h",
-            "include\\a\\trajpoly3.h",
-            "include\\a\\trajpoly5.h",
-            "include\\a\\trajpoly7.h",
-            "include\\a\\trajtrap.h",
-            "include\\a\\version.h"
+            "include/a/a.h",
+            "include/a/crc.h",
+            "include/a/fuzzy.h",
+            "include/a/hpf.h",
+            "include/a/lpf.h",
+            "include/a/math.h",
+            "include/a/mf.h",
+            "include/a/pid.h",
+            "include/a/pid_fuzzy.h",
+            "include/a/pid_neuro.h",
+            "include/a/poly.h",
+            "include/a/tf.h",
+            "include/a/trajbell.h",
+            "include/a/trajpoly3.h",
+            "include/a/trajpoly5.h",
+            "include/a/trajpoly7.h",
+            "include/a/trajtrap.h",
+            "include/a/version.h"
         ],
         "include_dirs": [
             "include"
         ],
         "language": "c",
         "name": "liba",
         "sources": [
             "python/src/a.pyx",
-            "src\\a.c",
-            "src\\avl.c",
-            "src\\buf.c",
-            "src\\complex.c",
-            "src\\crc.c",
-            "src\\fuzzy.c",
-            "src\\math.c",
-            "src\\mf.c",
-            "src\\pid.c",
-            "src\\pid_fuzzy.c",
-            "src\\pid_neuro.c",
-            "src\\poly.c",
-            "src\\que.c",
-            "src\\rbt.c",
-            "src\\str.c",
-            "src\\tf.c",
-            "src\\trajbell.c",
-            "src\\trajpoly3.c",
-            "src\\trajpoly5.c",
-            "src\\trajpoly7.c",
-            "src\\trajtrap.c",
-            "src\\utf.c",
-            "src\\vec.c",
-            "src\\version.c"
+            "src/a.c",
+            "src/avl.c",
+            "src/buf.c",
+            "src/complex.c",
+            "src/crc.c",
+            "src/fuzzy.c",
+            "src/math.c",
+            "src/mf.c",
+            "src/pid.c",
+            "src/pid_fuzzy.c",
+            "src/pid_neuro.c",
+            "src/poly.c",
+            "src/que.c",
+            "src/rbt.c",
+            "src/str.c",
+            "src/tf.c",
+            "src/trajbell.c",
+            "src/trajpoly3.c",
+            "src/trajpoly5.c",
+            "src/trajpoly7.c",
+            "src/trajtrap.c",
+            "src/utf.c",
+            "src/vec.c",
+            "src/version.c"
         ]
     },
     "module_name": "liba"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
@@ -1585,21 +1585,21 @@
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
-  "python\\\\src\\\\a.pyx",
+  "python/src/a.pyx",
   "<stringsource>",
-  "contextvars.pxd",
-  "array.pxd",
-  "type.pxd",
-  "bool.pxd",
-  "complex.pxd",
+  "venv/lib/python3.11/site-packages/Cython/Includes/cpython/contextvars.pxd",
+  "venv/lib/python3.11/site-packages/Cython/Includes/cpython/array.pxd",
+  "venv/lib/python3.11/site-packages/Cython/Includes/cpython/type.pxd",
+  "venv/lib/python3.11/site-packages/Cython/Includes/cpython/bool.pxd",
+  "venv/lib/python3.11/site-packages/Cython/Includes/cpython/complex.pxd",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
@@ -3159,15 +3159,15 @@
 static const char __pyx_k_version_parse[] = "version.parse";
 static const char __pyx_k_pid_fuzzy_kpid[] = "pid_fuzzy.kpid";
 static const char __pyx_k_pid_fuzzy_rule[] = "pid_fuzzy.rule";
 static const char __pyx_k_pid_fuzzy_zero[] = "pid_fuzzy.zero";
 static const char __pyx_k_pid_neuro_kpid[] = "pid_neuro.kpid";
 static const char __pyx_k_pid_neuro_wpid[] = "pid_neuro.wpid";
 static const char __pyx_k_pid_neuro_zero[] = "pid_neuro.zero";
-static const char __pyx_k_python_src_a_pyx[] = "python\\src\\a.pyx";
+static const char __pyx_k_python_src_a_pyx[] = "python/src/a.pyx";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_pid_fuzzy_set_block[] = "pid_fuzzy.set_block";
 /* #### Code section: decls ### */
 static int __pyx_pf_7cpython_5array_5array___getbuffer__(arrayobject *__pyx_v_self, Py_buffer *__pyx_v_info, CYTHON_UNUSED int __pyx_v_flags); /* proto */
 static void __pyx_pf_7cpython_5array_5array_2__releasebuffer__(CYTHON_UNUSED arrayobject *__pyx_v_self, Py_buffer *__pyx_v_info); /* proto */
 static PyObject *__pyx_pf_4liba_hash_bkdr(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_str, a_u32 __pyx_v_val); /* proto */
```

### Comparing `liba-0.1.9/python/src/a.pyx` & `liba-0.1.9.post1/python/src/a.pyx`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/setup.py` & `liba-0.1.9.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             continue
         text += "#define %s 1\n" % (name)
     return text
 
 
 def configure(config):
     with open("setup.cfg", "r") as f:
-        version = findall(r"version = (.+)", f.read())[0]
+        version = findall(r"version = (\S+)", f.read())[0]
     major, minor, patch = findall(r"(\d+).(\d+).(\d+)", version)[0]
     order = {"little": 1234, "big": 4321}.get(byteorder)
     vsize = ctypes.sizeof(ctypes.c_void_p(0))
     text = """/* autogenerated by setup.py */
 #define A_VERSION "{}"
 #define A_VERSION_MAJOR {}
 #define A_VERSION_MINOR {}
```

### Comparing `liba-0.1.9/src/a.c` & `liba-0.1.9.post1/src/a.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/src/avl.c` & `liba-0.1.9.post1/src/avl.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/src/buf.c` & `liba-0.1.9.post1/src/buf.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/src/complex.c` & `liba-0.1.9.post1/src/complex.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/src/crc.c` & `liba-0.1.9.post1/src/crc.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/src/math.c` & `liba-0.1.9.post1/src/math.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/src/mf.c` & `liba-0.1.9.post1/src/mf.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/src/pid.c` & `liba-0.1.9.post1/src/pid.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/src/pid_fuzzy.c` & `liba-0.1.9.post1/src/pid_fuzzy.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/src/pid_neuro.c` & `liba-0.1.9.post1/src/pid_neuro.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/src/poly.c` & `liba-0.1.9.post1/src/poly.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/src/que.c` & `liba-0.1.9.post1/src/que.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/src/rbt.c` & `liba-0.1.9.post1/src/rbt.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/src/str.c` & `liba-0.1.9.post1/src/str.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/src/tf.c` & `liba-0.1.9.post1/src/tf.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/src/trajbell.c` & `liba-0.1.9.post1/src/trajbell.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/src/trajpoly3.c` & `liba-0.1.9.post1/src/trajpoly3.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/src/trajpoly5.c` & `liba-0.1.9.post1/src/trajpoly5.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/src/trajpoly7.c` & `liba-0.1.9.post1/src/trajpoly7.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/src/trajtrap.c` & `liba-0.1.9.post1/src/trajtrap.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/src/utf.c` & `liba-0.1.9.post1/src/utf.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/src/vec.c` & `liba-0.1.9.post1/src/vec.c`

 * *Files identical despite different names*

### Comparing `liba-0.1.9/src/version.c` & `liba-0.1.9.post1/src/version.c`

 * *Files identical despite different names*

