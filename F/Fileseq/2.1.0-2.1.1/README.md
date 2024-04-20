# Comparing `tmp/Fileseq-2.1.0.tar.gz` & `tmp/fileseq-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fileseq-2.1.0.tar", last modified: Tue Mar 26 19:46:59 2024, max compression
+gzip compressed data, was "fileseq-2.1.1.tar", last modified: Sat Apr 20 00:50:39 2024, max compression
```

## Comparing `Fileseq-2.1.0.tar` & `fileseq-2.1.1.tar`

### file list

```diff
@@ -1,253 +1,252 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:59.632875 Fileseq-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-26 19:46:51.000000 Fileseq-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-26 19:46:51.000000 Fileseq-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-03-26 19:46:59.632875 Fileseq-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-03-26 19:46:51.000000 Fileseq-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 19:46:59.632875 Fileseq-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-03-26 19:46:51.000000 Fileseq-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:59.596875 Fileseq-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:59.632875 Fileseq-2.1.0/src/Fileseq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-03-26 19:46:59.000000 Fileseq-2.1.0/src/Fileseq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-03-26 19:46:59.000000 Fileseq-2.1.0/src/Fileseq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 19:46:59.000000 Fileseq-2.1.0/src/Fileseq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-26 19:46:59.000000 Fileseq-2.1.0/src/Fileseq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-26 19:46:59.000000 Fileseq-2.1.0/src/Fileseq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:59.600875 Fileseq-2.1.0/src/fileseq/
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-03-26 19:46:51.000000 Fileseq-2.1.0/src/fileseq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-26 19:46:59.000000 Fileseq-2.1.0/src/fileseq/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-03-26 19:46:51.000000 Fileseq-2.1.0/src/fileseq/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-26 19:46:51.000000 Fileseq-2.1.0/src/fileseq/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    53781 2024-03-26 19:46:51.000000 Fileseq-2.1.0/src/fileseq/filesequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    48249 2024-03-26 19:46:51.000000 Fileseq-2.1.0/src/fileseq/frameset.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/src/fileseq/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13103 2024-03-26 19:46:51.000000 Fileseq-2.1.0/src/fileseq/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:59.600875 Fileseq-2.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:59.600875 Fileseq-2.1.0/test/broken_seq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/broken_seq/broke.0000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/broken_seq/broke.0001.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/broken_seq/broke.0002.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/broken_seq/broke.0004.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/broken_seq/broke.0006.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/broken_seq/broke.0007.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/broken_seq/broke.0008.exr
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:59.604875 Fileseq-2.1.0/test/complex_ext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/complex_ext/1.a.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/complex_ext/2.a.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/complex_ext/3.a.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/complex_ext/file.5.a.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/complex_ext/file.6.a.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/complex_ext/file.7.a.ext
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:59.604875 Fileseq-2.1.0/test/mixed/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed/seq.-0001.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed/seq.-001.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed/seq.-1.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed/seq.00.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed/seq.0000.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed/seq.00000.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed/seq.00001.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed/seq.00002.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed/seq.00003.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed/seq.00004.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed/seq.00005.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed/seq.0001.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed/seq.0002.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed/seq.0003.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed/seq.0004.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed/seq.0005.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed/seq.01.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed/seq.02.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed/seq.03.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed/seq.04.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed/seq.05.ext
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:59.596875 Fileseq-2.1.0/test/mixed_case/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:59.608875 Fileseq-2.1.0/test/mixed_case/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed_case/sub/file_FOO_004.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed_case/sub/file_FOO_005.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed_case/sub/file_FOO_006.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed_case/sub/file_foo_001.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed_case/sub/file_foo_002.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/mixed_case/sub/file_foo_003.ext
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:59.608875 Fileseq-2.1.0/test/multi_range/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/multi_range/file_0003.0001.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/multi_range/file_0004.0001.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/multi_range/file_0005.0001.exr
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/pytest.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)      308 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:59.612875 Fileseq-2.1.0/test/seq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/0001.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/0002.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/0003.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/bar1000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/bar1001.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/bar1002.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/bar1004.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/bar1005.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/bar1006.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/baz_left.0001.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/baz_left.0002.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/baz_left.0003.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/baz_right.0001.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/baz_right.0002.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/baz_right.0003.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/big.0999.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/big.1000.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/big.1001.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/big.1002.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/big.1003.ext
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/foo.0001.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/foo.0001.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/foo.0002.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/foo.0002.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/foo.0003.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/foo.0003.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/foo.0004.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/foo.0004.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/foo.0005.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/foo.0005.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/foo.debug.0001.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/foo.debug.0002.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/foo.debug.0003.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/foo.debug.0004.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/foo.debug.0005.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/foo_0001.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seq/foo_0001_extra.exr
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:59.616875 Fileseq-2.1.0/test/seqhidden/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/.bar1000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/.bar1001.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/.bar1002.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/.bar1004.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/.bar1005.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/.bar1006.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/.foo.0001.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/.foo.0001.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/.foo.0002.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/.foo.0002.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/.foo.0003.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/.foo.0003.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/.foo.0004.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/.foo.0004.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/.foo.0005.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/.foo.0005.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/.hidden
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/bar1000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/bar1001.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/bar1002.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/bar1004.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/bar1005.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/bar1006.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/foo.0001.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/foo.0001.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/foo.0002.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/foo.0002.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/foo.0003.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/foo.0003.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/foo.0004.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/foo.0004.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/foo.0005.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqhidden/foo.0005.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:59.616875 Fileseq-2.1.0/test/seqneg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqneg/bar.-001.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqneg/bar.0000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqneg/bar.0001.exr
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:59.596875 Fileseq-2.1.0/test/seqsubdirs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:59.620875 Fileseq-2.1.0/test/seqsubdirs/sub1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqsubdirs/sub1/0001.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqsubdirs/sub1/0002.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqsubdirs/sub1/0003.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqsubdirs/sub1/bar1000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqsubdirs/sub1/bar1001.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqsubdirs/sub1/bar1002.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqsubdirs/sub1/bar1004.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqsubdirs/sub1/bar1005.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqsubdirs/sub1/bar1006.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqsubdirs/sub1/foo.0001.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqsubdirs/sub1/foo.0001.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqsubdirs/sub1/foo.0002.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqsubdirs/sub1/foo.0002.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqsubdirs/sub1/foo.0003.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqsubdirs/sub1/foo.0003.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqsubdirs/sub1/foo.0004.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqsubdirs/sub1/foo.0004.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqsubdirs/sub1/foo.0005.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqsubdirs/sub1/foo.0005.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqsubdirs/sub1/foo.debug.0001.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqsubdirs/sub1/foo.debug.0002.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqsubdirs/sub1/foo.debug.0003.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqsubdirs/sub1/foo.debug.0004.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqsubdirs/sub1/foo.debug.0005.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/seqsubdirs/sub1/foo_0001.exr
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:59.624875 Fileseq-2.1.0/test/step_seq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/step_seq/step1.0001.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/step_seq/step1.0005.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/step_seq/step1.0009.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/step_seq/step1.0013.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/step_seq/step1.0014.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/step_seq/step1.0015.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/step_seq/step1.0016.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/step_seq/step1.0017.exr
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:59.632875 Fileseq-2.1.0/test/subframe_seq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/bar.0001.0000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/baz.0001.0000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/baz.0001.2500.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/baz.0001.5000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/baz.0001.7500.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/baz.0002.0000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/baz.0003.0000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/baz.0003.2500.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/baz.0003.5000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/baz.0003.7500.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/baz.0004.0000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/baz_left.1001.0000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/baz_left.1001.2500.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/baz_left.1001.5000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/baz_left.1001.7500.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/baz_left.1002.0000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/baz_right.1001.0000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/baz_right.1001.2500.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/baz_right.1001.5000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/baz_right.1001.7500.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/baz_right.1002.0000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foo.0001.0000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foo.0001.0000.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foo.0001.2500.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foo.0001.2500.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foo.0001.5000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foo.0001.5000.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foo.0001.7500.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foo.0001.7500.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foo.0002.0000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foo.0002.0000.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foo.0002.2500.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foo.0002.2500.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foo.0002.5000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foo.0002.5000.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foo.0002.7500.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foo.0002.7500.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foo.0003.0000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foo.0003.0000.jpg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foz.1001.0000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foz.1001.2500.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foz.1001.5000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foz.1001.7500.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foz.1002.0000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foz.1002.2500.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foz.1002.5000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foz.1002.7500.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foz.1003.0000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foz.debug.1001.0000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foz.debug.1001.2500.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foz.debug.1001.5000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foz.debug.1001.7500.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/foz.debug.1002.0000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/guz.0001.00.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/guz.0001.25.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/guz.0001.50.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/guz.0001.75.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seq/guz.0002.00.exr
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:59.632875 Fileseq-2.1.0/test/subframe_seqneg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seqneg/bar.-000.5000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seqneg/bar.0000.0000.exr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/subframe_seqneg/bar.0000.5000.exr
--rwxr-xr-x   0 runner    (1001) docker     (127)    57636 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/test_fuzz.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    86583 2024-03-26 19:46:51.000000 Fileseq-2.1.0/test/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:39.434176 fileseq-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-20 00:50:31.000000 fileseq-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-20 00:50:31.000000 fileseq-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-20 00:50:39.434176 fileseq-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-04-20 00:50:31.000000 fileseq-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 00:50:39.434176 fileseq-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-20 00:50:31.000000 fileseq-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:39.398176 fileseq-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:39.434176 fileseq-2.1.1/src/Fileseq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-20 00:50:39.000000 fileseq-2.1.1/src/Fileseq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-04-20 00:50:39.000000 fileseq-2.1.1/src/Fileseq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 00:50:39.000000 fileseq-2.1.1/src/Fileseq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 00:50:39.000000 fileseq-2.1.1/src/Fileseq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:39.402176 fileseq-2.1.1/src/fileseq/
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-20 00:50:31.000000 fileseq-2.1.1/src/fileseq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 00:50:39.000000 fileseq-2.1.1/src/fileseq/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-04-20 00:50:31.000000 fileseq-2.1.1/src/fileseq/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-20 00:50:31.000000 fileseq-2.1.1/src/fileseq/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55100 2024-04-20 00:50:31.000000 fileseq-2.1.1/src/fileseq/filesequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49657 2024-04-20 00:50:31.000000 fileseq-2.1.1/src/fileseq/frameset.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/src/fileseq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-04-20 00:50:31.000000 fileseq-2.1.1/src/fileseq/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:39.402176 fileseq-2.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:39.406175 fileseq-2.1.1/test/broken_seq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/broken_seq/broke.0000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/broken_seq/broke.0001.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/broken_seq/broke.0002.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/broken_seq/broke.0004.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/broken_seq/broke.0006.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/broken_seq/broke.0007.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/broken_seq/broke.0008.exr
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:39.406175 fileseq-2.1.1/test/complex_ext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/complex_ext/1.a.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/complex_ext/2.a.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/complex_ext/3.a.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/complex_ext/file.5.a.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/complex_ext/file.6.a.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/complex_ext/file.7.a.ext
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:39.410176 fileseq-2.1.1/test/mixed/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed/seq.-0001.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed/seq.-001.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed/seq.-1.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed/seq.00.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed/seq.0000.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed/seq.00000.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed/seq.00001.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed/seq.00002.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed/seq.00003.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed/seq.00004.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed/seq.00005.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed/seq.0001.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed/seq.0002.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed/seq.0003.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed/seq.0004.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed/seq.0005.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed/seq.01.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed/seq.02.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed/seq.03.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed/seq.04.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed/seq.05.ext
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:39.398176 fileseq-2.1.1/test/mixed_case/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:39.410176 fileseq-2.1.1/test/mixed_case/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed_case/sub/file_FOO_004.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed_case/sub/file_FOO_005.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed_case/sub/file_FOO_006.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed_case/sub/file_foo_001.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed_case/sub/file_foo_002.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/mixed_case/sub/file_foo_003.ext
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:39.410176 fileseq-2.1.1/test/multi_range/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/multi_range/file_0003.0001.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/multi_range/file_0004.0001.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/multi_range/file_0005.0001.exr
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/pytest.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)      308 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:39.414176 fileseq-2.1.1/test/seq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/0001.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/0002.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/0003.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/bar1000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/bar1001.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/bar1002.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/bar1004.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/bar1005.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/bar1006.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/baz_left.0001.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/baz_left.0002.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/baz_left.0003.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/baz_right.0001.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/baz_right.0002.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/baz_right.0003.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/big.0999.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/big.1000.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/big.1001.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/big.1002.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/big.1003.ext
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/foo.0001.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/foo.0001.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/foo.0002.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/foo.0002.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/foo.0003.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/foo.0003.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/foo.0004.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/foo.0004.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/foo.0005.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/foo.0005.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/foo.debug.0001.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/foo.debug.0002.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/foo.debug.0003.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/foo.debug.0004.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/foo.debug.0005.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/foo_0001.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seq/foo_0001_extra.exr
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:39.418176 fileseq-2.1.1/test/seqhidden/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/.bar1000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/.bar1001.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/.bar1002.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/.bar1004.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/.bar1005.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/.bar1006.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/.foo.0001.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/.foo.0001.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/.foo.0002.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/.foo.0002.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/.foo.0003.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/.foo.0003.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/.foo.0004.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/.foo.0004.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/.foo.0005.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/.foo.0005.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/.hidden
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/bar1000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/bar1001.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/bar1002.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/bar1004.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/bar1005.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/bar1006.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/foo.0001.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/foo.0001.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/foo.0002.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/foo.0002.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/foo.0003.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/foo.0003.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/foo.0004.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/foo.0004.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/foo.0005.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqhidden/foo.0005.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:39.418176 fileseq-2.1.1/test/seqneg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqneg/bar.-001.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqneg/bar.0000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqneg/bar.0001.exr
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:39.398176 fileseq-2.1.1/test/seqsubdirs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:39.422176 fileseq-2.1.1/test/seqsubdirs/sub1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqsubdirs/sub1/0001.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqsubdirs/sub1/0002.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqsubdirs/sub1/0003.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqsubdirs/sub1/bar1000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqsubdirs/sub1/bar1001.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqsubdirs/sub1/bar1002.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqsubdirs/sub1/bar1004.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqsubdirs/sub1/bar1005.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqsubdirs/sub1/bar1006.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqsubdirs/sub1/foo.0001.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqsubdirs/sub1/foo.0001.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqsubdirs/sub1/foo.0002.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqsubdirs/sub1/foo.0002.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqsubdirs/sub1/foo.0003.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqsubdirs/sub1/foo.0003.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqsubdirs/sub1/foo.0004.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqsubdirs/sub1/foo.0004.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqsubdirs/sub1/foo.0005.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqsubdirs/sub1/foo.0005.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqsubdirs/sub1/foo.debug.0001.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqsubdirs/sub1/foo.debug.0002.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqsubdirs/sub1/foo.debug.0003.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqsubdirs/sub1/foo.debug.0004.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqsubdirs/sub1/foo.debug.0005.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/seqsubdirs/sub1/foo_0001.exr
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:39.426175 fileseq-2.1.1/test/step_seq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/step_seq/step1.0001.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/step_seq/step1.0005.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/step_seq/step1.0009.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/step_seq/step1.0013.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/step_seq/step1.0014.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/step_seq/step1.0015.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/step_seq/step1.0016.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/step_seq/step1.0017.exr
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:39.434176 fileseq-2.1.1/test/subframe_seq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/bar.0001.0000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/baz.0001.0000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/baz.0001.2500.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/baz.0001.5000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/baz.0001.7500.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/baz.0002.0000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/baz.0003.0000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/baz.0003.2500.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/baz.0003.5000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/baz.0003.7500.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/baz.0004.0000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/baz_left.1001.0000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/baz_left.1001.2500.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/baz_left.1001.5000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/baz_left.1001.7500.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/baz_left.1002.0000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/baz_right.1001.0000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/baz_right.1001.2500.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/baz_right.1001.5000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/baz_right.1001.7500.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/baz_right.1002.0000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foo.0001.0000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foo.0001.0000.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foo.0001.2500.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foo.0001.2500.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foo.0001.5000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foo.0001.5000.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foo.0001.7500.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foo.0001.7500.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foo.0002.0000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foo.0002.0000.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foo.0002.2500.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foo.0002.2500.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foo.0002.5000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foo.0002.5000.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foo.0002.7500.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foo.0002.7500.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foo.0003.0000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foo.0003.0000.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foz.1001.0000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foz.1001.2500.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foz.1001.5000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foz.1001.7500.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foz.1002.0000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foz.1002.2500.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foz.1002.5000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foz.1002.7500.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foz.1003.0000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foz.debug.1001.0000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foz.debug.1001.2500.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foz.debug.1001.5000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foz.debug.1001.7500.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/foz.debug.1002.0000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/guz.0001.00.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/guz.0001.25.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/guz.0001.50.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/guz.0001.75.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seq/guz.0002.00.exr
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:39.434176 fileseq-2.1.1/test/subframe_seqneg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seqneg/bar.-000.5000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seqneg/bar.0000.0000.exr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/subframe_seqneg/bar.0000.5000.exr
+-rwxr-xr-x   0 runner    (1001) docker     (127)    57636 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/test_fuzz.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    86583 2024-04-20 00:50:31.000000 fileseq-2.1.1/test/test_unit.py
```

### Comparing `Fileseq-2.1.0/LICENSE` & `fileseq-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Fileseq-2.1.0/PKG-INFO` & `fileseq-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fileseq
-Version: 2.1.0
+Version: 2.1.1
 Summary: A Python library for parsing frame ranges and file sequences commonly used in VFX and Animation applications.
 Home-page: https://github.com/justinfx/fileseq
 Author: Matt Chambers
 Author-email: yougotrooted@gmail.com
 Maintainer: Justin Israel
 Maintainer-email: justinisrael@gmail.com
 License: MIT
@@ -15,15 +15,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: typing-extensions
 
 # <img src="docs/_static/fileseq_large.png" width="30%" height="30%" title="Fileseq" alt="Fileseq">
 
 [![Documentation Status](https://readthedocs.org/projects/fileseq/badge/?version=latest)](http://fileseq.readthedocs.io/en/latest/) [![Build status](https://github.com/justinfx/fileseq/actions/workflows/ci.yml/badge.svg)](https://github.com/justinfx/fileseq/actions/workflows/ci.yml)
 
 A Python library for parsing frame ranges and file sequences commonly 
 used in VFX and Animation applications.
```

### Comparing `Fileseq-2.1.0/README.md` & `fileseq-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `Fileseq-2.1.0/setup.py` & `fileseq-2.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,10 +48,8 @@
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
           'Programming Language :: Python :: 3',
       ],
 
       keywords='vfx visual effects file sequence frames image',
-
-      install_requires=['typing-extensions'],
       )
```

### Comparing `Fileseq-2.1.0/src/Fileseq.egg-info/PKG-INFO` & `fileseq-2.1.1/src/Fileseq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fileseq
-Version: 2.1.0
+Version: 2.1.1
 Summary: A Python library for parsing frame ranges and file sequences commonly used in VFX and Animation applications.
 Home-page: https://github.com/justinfx/fileseq
 Author: Matt Chambers
 Author-email: yougotrooted@gmail.com
 Maintainer: Justin Israel
 Maintainer-email: justinisrael@gmail.com
 License: MIT
@@ -15,15 +15,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: typing-extensions
 
 # <img src="docs/_static/fileseq_large.png" width="30%" height="30%" title="Fileseq" alt="Fileseq">
 
 [![Documentation Status](https://readthedocs.org/projects/fileseq/badge/?version=latest)](http://fileseq.readthedocs.io/en/latest/) [![Build status](https://github.com/justinfx/fileseq/actions/workflows/ci.yml/badge.svg)](https://github.com/justinfx/fileseq/actions/workflows/ci.yml)
 
 A Python library for parsing frame ranges and file sequences commonly 
 used in VFX and Animation applications.
```

### Comparing `Fileseq-2.1.0/src/Fileseq.egg-info/SOURCES.txt` & `fileseq-2.1.1/src/Fileseq.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 src/Fileseq.egg-info/PKG-INFO
 src/Fileseq.egg-info/SOURCES.txt
 src/Fileseq.egg-info/dependency_links.txt
-src/Fileseq.egg-info/requires.txt
 src/Fileseq.egg-info/top_level.txt
 src/fileseq/__init__.py
 src/fileseq/__version__.py
 src/fileseq/constants.py
 src/fileseq/exceptions.py
 src/fileseq/filesequence.py
 src/fileseq/frameset.py
```

### Comparing `Fileseq-2.1.0/src/fileseq/__init__.py` & `fileseq-2.1.1/src/fileseq/__init__.py`

 * *Files identical despite different names*

### Comparing `Fileseq-2.1.0/src/fileseq/constants.py` & `fileseq-2.1.1/src/fileseq/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """
 constants - General constants of use to fileseq operations.
 """
 
 import re
+import typing
 
 # The max frame count of a FrameSet before a MaxSizeException
 # exception is raised
 MAX_FRAME_SIZE = 10000000
 
 
 class _PadStyle(object):
     def __init__(self, name: str):
         self.__name = name
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return hash(str(self))
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return '<PAD_STYLE: {}>'.format(self.__name)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.__name
 
-    def __eq__(self, other):
+    def __eq__(self, other: typing.Any) -> bool:
         if not isinstance(other, _PadStyle):
             return False
         return str(self) == str(other)
 
 
 PAD_STYLE_HASH1 = _PadStyle("HASH1")
 PAD_STYLE_HASH4 = _PadStyle("HASH4")
```

### Comparing `Fileseq-2.1.0/src/fileseq/filesequence.py` & `fileseq-2.1.1/src/fileseq/filesequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 filesequence - A parsing object representing sequential files for fileseq.
 """
 from __future__ import annotations
 
+import collections.abc
 import dataclasses
 import decimal
 import fnmatch
 import functools
 import operator
 import os
 import re
 import sys
 import typing
 from glob import iglob
-from typing_extensions import Self
 
 from . import constants, utils
 from .constants import (
     PAD_STYLE_DEFAULT, PAD_MAP, REVERSE_PAD_MAP,
     DISK_RE, DISK_SUB_RE, SPLIT_RE, SPLIT_SUB_RE,
     PRINTF_SYNTAX_PADDING_RE, HOUDINI_SYNTAX_PADDING_RE,
     UDIM_PADDING_PATTERNS)
@@ -144,29 +144,29 @@
         # Round subframes to match sequence
         if self._frameSet is not None and self._frameSet.hasSubFrames():
             self._frameSet = FrameSet([
                 utils.quantize(frame, self._decimal_places)
                 for frame in self._frameSet
             ])
 
-    def copy(self) -> Self:
+    def copy(self) -> FileSequence:
         """
         Create a deep copy of this sequence
 
         Returns:
             :class:`.FileSequence`:
         """
         fs = self.__class__.__new__(self.__class__)
         fs.__dict__ = self.__dict__.copy()
         fs._frameSet = None
         if self._frameSet is not None:
             fs._frameSet = self._frameSet.copy()
         return fs
 
-    def format(self, template="{basename}{range}{padding}{extension}") -> str:
+    def format(self, template: str = "{basename}{range}{padding}{extension}") -> str:
         """Return the file sequence as a formatted string according to
         the given template.
 
         Utilizes the python string format syntax.  Available keys include:
             * basename - the basename of the sequence.
             * range - the range of the sequence
             * padding - the detecting amount of padding.
@@ -192,29 +192,29 @@
             `fileseq.constants.MAX_FRAME_SIZE``
         """
         try:
             return self._format(template)
         except UnicodeEncodeError:
             return self._format(str(template))
 
-    def _format(self, template):
+    def _format(self, template: str) -> str:
         # Potentially expensive if inverted range is large
         # and user never asked for it in template
         inverted = (self.invertedFrameRange() or "") if "{inverted}" in template else ""
 
         return template.format(
             basename=self.basename(),
             extension=self.extension(), start=self.start(),
             end=self.end(), length=len(self),
             padding=self.padding(),
             range=self.frameRange() or "",
             inverted=inverted,
             dirname=self.dirname())
 
-    def split(self) -> list[Self]:
+    def split(self) -> list[FileSequence]:
         """
         Split the :class:`FileSequence` into contiguous pieces and return them
         as a list of :class:`FileSequence` instances.
 
         Returns:
             list[:class:`FileSequence`]:
         """
@@ -229,15 +229,15 @@
         Return the directory name of the sequence.
 
         Returns:
             str:
         """
         return self._dir
 
-    def setDirname(self, dirname: str):
+    def setDirname(self, dirname: str) -> None:
         """
         Set a new directory name for the sequence.
 
         Args:
             dirname (str): the new directory name
         """
         # Make sure the dirname always ends in
@@ -254,15 +254,15 @@
         Return the basename of the sequence.
 
         Returns:
             str: sequence basename
         """
         return self._base
 
-    def setBasename(self, base: str):
+    def setBasename(self, base: str) -> None:
         """
         Set a new basename for the sequence.
 
         Args:
             base (str): the new base name
         """
         self._base = utils.asString(base)
@@ -273,15 +273,15 @@
         See fileseq.constants.PAD_STYLE_HASH1 and fileseq.constants.PAD_STYLE_HASH4
 
         Returns:
             (`PAD_STYLE_DEFAULT` or `PAD_STYLE_HASH1` or `PAD_STYLE_HASH4`): padding style
         """
         return self._pad_style
 
-    def setPadStyle(self, pad_style: constants._PadStyle, set_zfill: bool = False):
+    def setPadStyle(self, pad_style: constants._PadStyle, set_zfill: bool = False) -> None:
         """
         Set new padding style for the sequence.
         See fileseq.constants.PAD_STYLE_HASH1 and fileseq.constants.PAD_STYLE_HASH4
 
         The default behavior converts only the padding characters representation per the new style,
         the same zfill/decimalPlaces value. If ``set_zfill=True``, convert the zfill/decimalPlaces
         values to match the meaning of the padding characters per the new style.
@@ -318,15 +318,15 @@
         Return the padding characters in the sequence.
 
         Returns:
             str: sequence padding
         """
         return self._pad
 
-    def setPadding(self, padding: str):
+    def setPadding(self, padding: str) -> None:
         """
         Set new padding characters for the sequence.
         i.e. "#" or "@@@" or '%04d', or an empty string to disable range formatting.
 
         Args:
             padding (str): sequence padding to set
 
@@ -351,15 +351,15 @@
         Return the padding characters in the sequence.
 
         Returns:
             str: sequence padding
         """
         return self._frame_pad
 
-    def setFramePadding(self, padding: str):
+    def setFramePadding(self, padding: str) -> None:
         """
         Set new padding characters for the frames of the sequence.
         i.e. "#" or "@@@" or '%04d', or an empty string to disable range formatting.
 
         Args:
             padding (str): sequence padding to set
 
@@ -385,15 +385,15 @@
         Return the padding characters for subframes in the sequence.
 
         Returns:
             str: sequence padding
         """
         return self._subframe_pad
 
-    def setSubframePadding(self, padding: str):
+    def setSubframePadding(self, padding: str) -> None:
         """
         Set new padding characters for the subframes in the sequence.
         i.e. "#" or "@@@", or an empty string to disable range
         formatting.
 
         Args:
             padding (str): sequence padding to set
@@ -412,25 +412,25 @@
         decimal_places = self.getPaddingNum(subframe_pad, pad_style=pad_style)
 
         # Set all fields atomically after parsing valid padding characters
         self._subframe_pad = subframe_pad
         self._pad = pad
         self._decimal_places = decimal_places
 
-    def frameSet(self) -> FrameSet | None:
+    def frameSet(self) -> FrameSet|None:
         """
         Return the :class:`.FrameSet` of the sequence if specified,
         otherwise None.
 
         Returns:
             :class:`.FrameSet` or None:
         """
         return self._frameSet
 
-    def setFrameSet(self, frameSet: FrameSet | None):
+    def setFrameSet(self, frameSet: FrameSet|None) -> None:
         """
         Set a new :class:`.FrameSet` for the sequence.
 
         Args:
             frameSet (:class:`.FrameSet`): the new :class:`.FrameSet` object
         """
         if frameSet is not None and frameSet.hasSubFrames():
@@ -449,29 +449,29 @@
         Return the file extension of the sequence, including leading period.
 
         Returns:
             str:
         """
         return self._ext
 
-    def setExtension(self, ext: str):
+    def setExtension(self, ext: str) -> None:
         """
         Set a new file extension for the sequence.
 
         Note:
             A leading period will be added if none is provided.
 
         Args:
             ext (str): the new file extension
         """
         if ext and ext[0] != ".":
             ext = "." + ext
         self._ext = utils.asString(ext)
 
-    def setExtention(self, ext: str):
+    def setExtention(self, ext: str) -> None:
         """
         Deprecated: use :meth:`setExtension`.
 
         Args:
             ext (str):
         """
         import warnings
@@ -487,15 +487,15 @@
         Returns:
             str:
         """
         if not self._frameSet:
             return ''
         return self._frameSet.frameRange(self._zfill, self._decimal_places)
 
-    def setFrameRange(self, frange):
+    def setFrameRange(self, frange: typing.Any) -> None:
         """
         Set a new frame range for the sequence.
 
         Args:
             frange (str): a properly formatted frame range, as per :class:`.FrameSet`
         """
         self._frameSet = FrameSet(frange)
@@ -607,15 +607,15 @@
 
         Args:
             idx (int): the desired index
 
         Returns:
             str:
         """
-        return self.__getitem__(idx)
+        return self.__getitem__(idx)  # type: ignore
 
     def batches(self, batch_size: int, paths: bool = False) -> typing.Iterable[str | FileSequence]:
         """
         Returns a generator that yields groups of file paths, up to ``batch_size``.
         Convenience method for ``fileseq.utils.batchIterable(self, batch_size)``
         If ``paths=False``, each batch is a new ``FileSequence`` subrange.
         If ``paths=True``, each batch is an islice generator object of each file
@@ -635,29 +635,29 @@
             # They just want batches of the individual file paths
             return utils.batchIterable(self, batch_size)
 
         # generate batches of index ranges for the current sequence
         frame_gen = utils.batchFrames(0, len(self) - 1, batch_size)
         return (self[f.start:f.stop + 1] for f in frame_gen)
 
-    def __setstate__(self, state):
+    def __setstate__(self, state: typing.Any) -> None:
         """
         Allows for de-serialization from a pickled :class:`FileSequence`.
 
         Args:
             state (dict): Pickle dictionary produced by default pickle implementation
         """
         for name, value in state.items():
             self.__dict__[name] = value
         self.__dict__.setdefault('_pad_style', PAD_STYLE_DEFAULT)
         self.__dict__.setdefault('_frame_pad', self._pad)
         self.__dict__.setdefault('_subframe_pad', '')
         self.__dict__.setdefault('_decimal_places', 0)
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         """
         Convert sequence object into a state dict that is suitable for
         further serialization, such as to JSON
 
         Returns:
             dict: state of the current sequence object
         """
@@ -665,15 +665,15 @@
         state['_pad_style'] = str(self._pad_style)
         state['_frameSet'] = None
         if self._frameSet is not None:
             state['_frameSet'] = self._frameSet.__getstate__()
         return state
 
     @classmethod
-    def from_dict(cls, state: dict) -> FileSequence:
+    def from_dict(cls, state: dict[str, typing.Any]) -> FileSequence:
         """
         Constructor to create a new sequence object from a state
         that was previously returned by :meth:`FileSequence.to_dict`
 
         Args:
             state (dict): state returned from :meth:`FileSequence.to_dict`
 
@@ -688,32 +688,32 @@
             raise ValueError("bad pad style constant value %r" % padStyle)
         state['_pad_style'] = padStyle
         state['_frameSet'] = frameSet
         fs = cls.__new__(cls)
         fs.__setstate__(state)
         return fs
 
-    def __iter__(self):
+    def __iter__(self) -> collections.abc.Generator[str, None, None]:
         """
         Allow iteration over the path or paths this :class:`FileSequence`
         represents.
 
         Yields:
-            :class:`FileSequence`:
+            str: path
         """
         # If there is no frame range, or there is no padding
         # characters, then we only want to represent a single path
         if not self._frameSet or not self._zfill:
             yield utils.asString(self)
             return
 
         for f in self._frameSet:
             yield self.frame(f)
 
-    def __getitem__(self, idx):
+    def __getitem__(self, idx: typing.Any) -> str|FileSequence:
         """
         Allows indexing and slicing into the underlying :class:`.FrameSet`
 
         When indexing, a string filepath is returns for the frame.
 
         When slicing, a new :class:`FileSequence` is returned.
         Slicing outside the range of the sequence results in an
@@ -740,66 +740,73 @@
         if fset.is_null:
             raise IndexError("slice is out of range and returns no frames")
 
         fs = self.copy()
         fs.setFrameSet(fset)
         return fs
 
-    def __len__(self):
+    def __len__(self) -> int:
         """
         The length (number of files) represented by this :class:`FileSequence`.
 
         Returns:
             int:
         """
         if not self._frameSet or not self._zfill:
             return 1
         return len(self._frameSet)
 
-    def __str__(self):
+    def __str__(self) -> str:
         """
         String representation of this :class:`FileSequence`.
 
+        Note:
+            A FileSequence that does not define a frame range will omit
+            the padding character component when string formatted, even
+            if the padding character is set.
+            For more control over the exact string format, use the
+            :obj:`FileSequence.format()` method.
+
         Returns:
             str:
         """
         cmpts = self.__components()
         cmpts.frameSet = utils.asString(cmpts.frameSet or "")
         return "".join(dataclasses.astuple(cmpts))
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         try:
             return "<%s: %r>" % (self.__class__.__name__, self.__str__())
         except TypeError:
             return super(self.__class__, self).__repr__()
 
-    def __eq__(self, other):
+    def __eq__(self, other: typing.Any) -> bool:
         if not isinstance(other, FileSequence):
             return str(self) == str(other)
 
         a = self.__components()
         b = other.__components()
 
-        a.pad = self.getPaddingNum(a.pad)
-        b.pad = other.getPaddingNum(b.pad)
+        a.pad = self.getPaddingNum(str(a.pad))
+        b.pad = other.getPaddingNum(str(b.pad))
 
         return a == b
 
-    def __ne__(self, other):
+    def __ne__(self, other: typing.Any) -> bool:
         return not self.__eq__(other)
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         # TODO: Technically we should be returning None,
         # as this class is mutable and cannot reliably be hashed.
         # Python2 allows it without this definition.
         # Python3 fails with TypeError: unhashable.
         # For now, preserving the hashing behaviour in py3.
         return id(self)
 
-    def __components(self):
+    def __components(self) -> _Components:
         return self._Components(
             self._dir,
             self._base,
             self._frameSet or "",
             self._pad if self._frameSet else "",
             self._ext,
         )
@@ -853,15 +860,15 @@
             dirname, basename, ext = using.dirname(), using.basename(), using.extension()
             head: int = len(dirname + basename)
             tail: int = -len(ext)
             frames: set[str] = set()
 
             path: str
             for path in filter(None, map(utils.asString, paths)):
-                frame = path[head:tail]  # type: ignore
+                frame = path[head:tail]
                 try:
                     int(frame)
                 except ValueError:
                     if not allow_subframes:
                         continue
                     try:
                         decimal.Decimal(frame)
@@ -881,44 +888,45 @@
                     key = (dirname, basename, ext, len(subframe))
                 else:
                     key = (dirname, basename, ext, 0)
                 seqs.setdefault(key, set())
                 if frame:
                     seqs[key].add(frame)
 
-        def start_new_seq():
+        def start_new_seq() -> FileSequence:
             seq = cls.__new__(cls)
             seq._dir = dirname or ''
             seq._base = basename or ''
             seq._ext = ext or ''
             return seq
 
-        def finish_new_seq(seq):
+        def finish_new_seq(seq: FileSequence) -> None:
             if seq._subframe_pad:
                 seq._pad = '.'.join([seq._frame_pad, seq._subframe_pad])
             else:
                 seq._pad = seq._frame_pad
 
-            seq.__init__(utils.asString(seq), pad_style=pad_style, allow_subframes=allow_subframes)
+            seq.__init__(utils.asString(seq), pad_style=pad_style,  # type: ignore[misc]
+                         allow_subframes=allow_subframes)
 
-        def get_frame_width(frame_str):
+        def get_frame_width(frame_str: str) -> int:
             frame_num, _, _ = frame_str.partition(".")
             return len(frame_num)
 
-        def get_frame_minwidth(frame_str):
+        def get_frame_minwidth(frame_str: str) -> int:
             # find the smallest padding width for a frame string
             frame_num, _, _ = frame_str.partition(".")
             size = len(frame_num)
             num = int(frame_num)
             num_size = len(str(num))
             if size == num_size:
                 return 1
             return size
 
-        def frames_to_seq(frames, pad_length, decimal_places):
+        def frames_to_seq(frames: typing.Iterable[str], pad_length: int, decimal_places: int) -> FileSequence:
             seq = start_new_seq()
             seq._frameSet = FrameSet(sorted(decimal.Decimal(f) for f in frames))
             seq._frame_pad = cls.getPaddingChars(pad_length, pad_style=pad_style)
             if decimal_places:
                 seq._subframe_pad = cls.getPaddingChars(decimal_places, pad_style=pad_style)
             else:
                 seq._subframe_pad = ''
@@ -940,19 +948,19 @@
             # If we have multiple frames, then we need to check them for different
             # padding and possibly yield more than one sequence.
 
             # sort the frame list by their string padding width
             sorted_frames = sorted(((get_frame_width(f), f) for f in frames), key=operator.itemgetter(0))
 
             current_frames: list[str] = []
-            current_width = None
+            current_width = -1
 
             for width, frame in sorted_frames:
                 # initialize on first item
-                if current_width is None:
+                if current_width < 0:
                     current_width = width
 
                 if width != current_width and get_frame_minwidth(frame) > current_width:
                     # We have a new padding length.
                     # Commit the current sequence, and then start a new one.
                     yield frames_to_seq(current_frames, current_width, decimal_places)
 
@@ -1221,16 +1229,19 @@
 
         if pad:
             patt = r'\A'
             if dirname:
                 patt = r'.*[/\\]'
             patt += re.escape(basename) + '(.*)' + re.escape(ext) + r'\Z'
 
-            def get_frame(f):
-                return re.match(patt, f, re.I).group(1)
+            def get_frame(f: str) -> str:
+                m = re.match(patt, f, re.I)
+                if not m:
+                    raise ValueError(f'no frame match: str={f}, pattern={patt}')
+                return m.group(1)
 
             if strictPadding:
                 globbed = pad_filter_ctx(
                     globbed,
                     seq.zfill(),
                     decimal_places=seq.decimalPlaces(),
                     get_frame=get_frame
@@ -1300,22 +1311,27 @@
         """
         filename = filename.replace('.', r'\.')
         filename = filename.replace('*', '.*')
         filename = filename.replace('?', '.')
         return filename
 
     class _FilterByPaddingNum(object):
-        def __init__(self):
+        def __init__(self) -> None:
             # Tracks whether a padded frame has been yielded:
             #       padded: file.0001.ext
             #   not padded: file.1001.ext
             self.has_padded_frames = False
             self.has_padded_subframes = False
 
-        def __call__(self, iterable, zfill, decimal_places=0, get_frame=None):
+        def __call__(self,
+                     iterable: typing.Iterable[str],
+                     zfill: int|None,
+                     decimal_places: typing.Optional[int] = 0,
+                     get_frame: typing.Optional[typing.Callable[[str], str]] = None
+                     ) -> collections.abc.Generator[str, None, None]:
             """
             Yield only path elements from iterable which have a frame padding that
             matches the given target padding numbers. If zfill is None only the
             subframe length is matched against decimal places. If provided get_frame
             should be a callable taking one argument that will extract the frame
             number from a filename.
 
@@ -1335,18 +1351,20 @@
 
             self.has_padded_frames = False
             self.has_padded_subframes = False
 
             has_padded_frame = False
             has_padded_subframe = False
 
-            def check_padded(frame):
-                return frame and (frame[0] == '0' or frame[:2] == '-0')
+            def check_padded(frame: str) -> bool:
+                if frame and (frame[0] == '0' or frame[:2] == '-0'):
+                    return True
+                return False
 
-            def set_has_padded():
+            def set_has_padded() -> None:
                 if has_padded_frame:
                     self.has_padded_frames = True
                 if has_padded_subframe:
                     self.has_padded_subframes = True
 
             for item in iterable:
                 # Add a filter for paths that don't match the frame
@@ -1400,15 +1418,15 @@
                     set_has_padded()
                     # A frame that does not lead with '0' can match
                     # a padding width >= to the target padding number
                     yield item
                     continue
 
     @classmethod
-    def _filterByPaddingNum(cls, *args, **kwargs):
+    def _filterByPaddingNum(cls, *args, **kwargs) -> typing.Generator[str]:  # type: ignore
         ctx = cls._FilterByPaddingNum()
         return ctx(*args, **kwargs)
 
     @classmethod
     def getPaddingChars(cls, num: int, pad_style: constants._PadStyle = PAD_STYLE_DEFAULT) -> str:
         """
         Given a particular amount of padding, return the proper padding characters.
```

### Comparing `Fileseq-2.1.0/src/fileseq/frameset.py` & `fileseq-2.1.1/src/fileseq/frameset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """
 frameset - A set-like object representing a frame range for fileseq.
 """
 from __future__ import annotations
 
 import decimal
 import numbers
+import re
 import typing
 from collections.abc import Set, Sized, Iterable
+from typing import Union
 
 from . import constants  # constants.MAX_FRAME_SIZE updated during tests
 from .constants import PAD_MAP, FRANGE_RE, PAD_RE
 from .exceptions import MaxSizeException, ParseException
 from .utils import (asString, xfrange, unique, pad, quantize,
                     normalizeFrame, normalizeFrames, batchIterable)
 
 
-class FrameSet(Set):
+class FrameSet(Set):  # type:ignore[type-arg]
     """
     A ``FrameSet`` is an immutable representation of the ordered, unique
     set of frames in a given frame range.
 
     The frame range can be expressed in the following ways:
         - 1-5
         - 1-5,10-20
@@ -82,15 +84,15 @@
     PAD_RE = PAD_RE
 
     __slots__ = ('_frange', '_items', '_order')
 
     _items: frozenset[int]
     _order: tuple[int, ...]
 
-    def __new__(cls, *args, **kwargs):
+    def __new__(cls, *args: typing.Any, **kwargs: typing.Any) -> FrameSet:
         """
         Initialize the :class:`FrameSet` object.
 
         Args:
             frange (str or :class:`FrameSet`): the frame range as a string (ie "1-100x5")
 
         Raises:
@@ -98,19 +100,19 @@
                 (or a portion of it) could not be parsed.
             :class:`fileseq.exceptions.MaxSizeException`: if the range exceeds
                 ``fileseq.constants.MAX_FRAME_SIZE``
         """
         self = super(cls, FrameSet).__new__(cls)
         return self
 
-    def __init__(self, frange):
+    def __init__(self, frange: typing.Any) -> None:
         """Initialize the :class:`FrameSet` object.
         """
 
-        def catch_parse_err(fn, *a, **kw):
+        def catch_parse_err(fn, *a, **kw):  # type: ignore
             try:
                 return fn(*a, **kw)
             except (TypeError, ValueError) as e:
                 raise ParseException('FrameSet args parsing error: {}'.format(e)) from e
 
         # if the user provides anything but a string, short-circuit the build
         if not isinstance(frange, (str,)):
@@ -118,35 +120,35 @@
             if set(dir(frange)).issuperset(self.__slots__):
                 for attr in self.__slots__:
                     setattr(self, attr, getattr(frange, attr))
                 return
             # if it's inherently disordered, sort and build
             elif isinstance(frange, Set):
                 self._maxSizeCheck(frange)
-                self._items = frozenset(catch_parse_err(normalizeFrames, frange))
+                self._items = frozenset(catch_parse_err(normalizeFrames, frange))  # type: ignore
                 self._order = tuple(sorted(self._items))
-                self._frange = catch_parse_err(
+                self._frange = catch_parse_err(  # type: ignore
                     self.framesToFrameRange, self._order, sort=False, compress=False)
                 return
             # if it's ordered, find unique and build
             elif isinstance(frange, Sized) and isinstance(frange, Iterable):
                 self._maxSizeCheck(frange)
-                items = set()
-                order = unique(items, catch_parse_err(normalizeFrames, frange))
+                items: typing.Set[int] = set()
+                order = unique(items, catch_parse_err(normalizeFrames, frange))  # type: ignore
                 self._order = tuple(order)
                 self._items = frozenset(items)
-                self._frange = catch_parse_err(
+                self._frange = catch_parse_err(  # type: ignore
                     self.framesToFrameRange, self._order, sort=False, compress=False)
                 return
             # if it's an individual number build directly
             elif isinstance(frange, (int, float, decimal.Decimal)):
                 frame = normalizeFrame(frange)
-                self._order = (frame,)
-                self._items = frozenset([frame])
-                self._frange = catch_parse_err(
+                self._order = (frame,)  # type: ignore
+                self._items = frozenset([frame])  # type: ignore
+                self._frange = catch_parse_err(  # type: ignore
                     self.framesToFrameRange, self._order, sort=False, compress=False)
             # in all other cases, cast to a string
             else:
                 try:
                     frange = asString(frange)
                 except Exception as err:
                     msg = 'Could not parse "{0}": cast to string raised: {1}'
@@ -163,76 +165,76 @@
         if not self._frange:
             self._items = frozenset()
             self._order = tuple()
             return
 
         # build the mutable stores, then cast to immutable for storage
         items = set()
-        order = []
+        order_f: typing.List[int] = []
 
         maxSize = constants.MAX_FRAME_SIZE
 
-        frange_parts = []
-        frange_types = []
+        frange_parts: typing.List[typing.Any] = []
+        frange_types: typing.List[typing.Any] = []
         for part in self._frange.split(","):
             # this is to deal with leading / trailing commas
             if not part:
                 continue
             # parse the partial range
             start, end, modifier, chunk = self._parse_frange_part(part)
             frange_parts.append((start, end, modifier, chunk))
             frange_types.extend(map(type, (start, end, chunk)))
 
         # Determine best type for numbers in range. Note that
         # _parse_frange_part will always return decimal.Decimal for subframes
         FrameType = int
         if decimal.Decimal in frange_types:
-            FrameType = decimal.Decimal
+            FrameType = decimal.Decimal  # type: ignore
 
         for start, end, modifier, chunk in frange_parts:
             # handle batched frames (1-100x5)
             if modifier == 'x':
                 frames = xfrange(start, end, chunk, maxSize=maxSize)
-                frames = [FrameType(f) for f in frames if f not in items]
-                self._maxSizeCheck(len(frames) + len(items))
-                order.extend(frames)
+                frames = [FrameType(f) for f in frames if f not in items]  # type: ignore
+                self._maxSizeCheck(len(frames) + len(items))  # type: ignore
+                order_f.extend(frames)
                 items.update(frames)
             # handle staggered frames (1-100:5)
             elif modifier == ':':
                 if '.' in str(chunk):
                     raise ValueError("Unable to stagger subframes")
                 for stagger in range(chunk, 0, -1):
                     frames = xfrange(start, end, stagger, maxSize=maxSize)
-                    frames = [f for f in frames if f not in items]
-                    self._maxSizeCheck(len(frames) + len(items))
-                    order.extend(frames)
+                    frames = [f for f in frames if f not in items]  # type: ignore
+                    self._maxSizeCheck(len(frames) + len(items))  # type: ignore
+                    order_f.extend(frames)
                     items.update(frames)
             # handle filled frames (1-100y5)
             elif modifier == 'y':
                 if '.' in str(chunk):
                     raise ValueError("Unable to fill subframes")
                 not_good = frozenset(xfrange(start, end, chunk, maxSize=maxSize))
                 frames = xfrange(start, end, 1, maxSize=maxSize)
                 frames = (f for f in frames if f not in not_good)
-                frames = [f for f in frames if f not in items]
-                self._maxSizeCheck(len(frames) + len(items))
-                order.extend(frames)
+                frames = [f for f in frames if f not in items]  # type: ignore
+                self._maxSizeCheck(len(frames) + len(items))  # type: ignore
+                order_f.extend(frames)
                 items.update(frames)
             # handle full ranges and single frames
             else:
                 frames = xfrange(start, end, 1 if start < end else -1, maxSize=maxSize)
-                frames = [FrameType(f) for f in frames if f not in items]
-                self._maxSizeCheck(len(frames) + len(items))
-                order.extend(frames)
+                frames = [FrameType(f) for f in frames if f not in items]  # type: ignore
+                self._maxSizeCheck(len(frames) + len(items))  # type: ignore
+                order_f.extend(frames)
                 items.update(frames)
 
         # lock the results into immutable internals
         # this allows for hashing and fast equality checking
         self._items = frozenset(items)
-        self._order = tuple(order)
+        self._order = tuple(order_f)
 
     @property
     def is_null(self) -> bool:
         """
         Read-only access to determine if the :class:`FrameSet` is the null or
         empty :class:`FrameSet`.
 
@@ -245,15 +247,15 @@
     def frange(self) -> str:
         """
         Read-only access to the frame range used to create this :class:`FrameSet`.
 
         Returns:
             str:
         """
-        return self._frange
+        return self._frange or ''
 
     @property
     def items(self) -> frozenset[int]:
         """
         Read-only access to the unique frames that form this :class:`FrameSet`.
 
         Returns:
@@ -301,25 +303,25 @@
         # match range() exception
         if not isinstance(step, int):
             raise TypeError("integer step argument expected, got {}."
                             .format(type(step)))
         elif step == 0:
             raise ValueError("step argument must not be zero")
         elif step == 1:
-            start, end = normalizeFrames([start, end])
+            start, end = normalizeFrames([start, end])  # type:ignore[assignment]
             range_str = "{0}-{1}".format(start, end)
         else:
-            start, end = normalizeFrames([start, end])
-            step = normalizeFrame(step)
+            start, end = normalizeFrames([start, end])  # type:ignore[assignment]
+            step = normalizeFrame(step)  # type: ignore
             range_str = "{0}-{1}x{2}".format(start, end, step)
 
         return FrameSet(range_str)
 
     @classmethod
-    def _cast_to_frameset(cls, other):
+    def _cast_to_frameset(cls, other: typing.Any) -> FrameSet:
         """
         Private method to simplify comparison operations.
 
         Args:
             other (:class:`FrameSet` or set or frozenset or iterable): item to be compared
 
         Returns:
@@ -511,15 +513,15 @@
 
         Returns:
             :class:`FrameSet`:
         """
         return FrameSet(FrameSet.framesToFrameRange(
             self.items, sort=True, compress=False))
 
-    def batches(self, batch_size: int, frames: bool = False) -> typing.Iterator:
+    def batches(self, batch_size: int, frames: bool = False) -> typing.Iterator[typing.Any]:
         """
         Returns a generator that yields sub-batches of frames, up to ``batch_size``.
         If ``frames=False``, each batch is a new ``FrameSet`` subrange.
         If ``frames=True``, each batch is an islice generator object of the sub-range.
 
         Args:
             batch_size (int): max frame values in each batch
@@ -527,148 +529,148 @@
 
         Returns:
             generator: yields batches of islice or FrameSet sub-ranges
         """
         batch_it = batchIterable(self, batch_size)
         if frames:
             # They just want batches of the frame values
-            return batch_it
+            return batch_it  # type: ignore
 
         # return batches of FrameSet instance
         return (self.from_iterable(b) for b in batch_it)
 
-    def __getstate__(self):
+    def __getstate__(self) -> tuple[str]:
         """
         Allows for serialization to a pickled :class:`FrameSet`.
 
         Returns:
-            tuple: (frame range string, )
+            tuple: (frame range string,
         """
         # we have to special-case the empty FrameSet, because of a quirk in
         # Python where __setstate__ will not be called if the return value of
         # bool(__getstate__) == False.  A tuple with ('',) will return True.
         return (self.frange,)
 
-    def __setstate__(self, state):
+    def __setstate__(self, state: typing.Any) -> None:
         """
         Allows for de-serialization from a pickled :class:`FrameSet`.
 
         Args:
             state (tuple or str or dict): A string/dict can be used for
                 backwards compatibility
 
         Raises:
             ValueError: if state is not an appropriate type
         """
         if isinstance(state, tuple):
             # this is to allow unpickling of "3rd generation" FrameSets,
             # which are immutable and may be empty.
-            self.__init__(state[0])
+            self.__init__(state[0])  # type: ignore[misc]
         elif isinstance(state, str):
             # this is to allow unpickling of "2nd generation" FrameSets,
             # which were mutable and could not be empty.
-            self.__init__(state)
+            self.__init__(state)  # type: ignore[misc]
         elif isinstance(state, dict):
             # this is to allow unpickling of "1st generation" FrameSets,
             # when the full __dict__ was stored
             if '__frange' in state and '__set' in state and '__list' in state:
                 self._frange = state['__frange']
                 self._items = frozenset(state['__set'])
                 self._order = tuple(state['__list'])
             else:
                 for k in self.__slots__:
                     setattr(self, k, state[k])
         else:
             msg = "Unrecognized state data from which to deserialize FrameSet"
             raise ValueError(msg)
 
-    def __getitem__(self, index):
+    def __getitem__(self, index: int) -> int:
         """
         Allows indexing into the ordered frames of this :class:`FrameSet`.
 
         Args:
             index (int): the index to retrieve
 
         Returns:
             int:
 
         Raises:
             :class:`IndexError`: if index is out of bounds
         """
         return self.order[index]
 
-    def __len__(self):
+    def __len__(self) -> int:
         """
         Returns the length of the ordered frames of this :class:`FrameSet`.
 
         Returns:
             int:
         """
         return len(self.order)
 
-    def __str__(self):
+    def __str__(self) -> str:
         """
         Returns the frame range string of this :class:`FrameSet`.
 
         Returns:
             str:
         """
         return self.frange
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         """
         Returns a long-form representation of this :class:`FrameSet`.
 
         Returns:
             str:
         """
         return '{0}("{1}")'.format(self.__class__.__name__, self.frange)
 
-    def __iter__(self):
+    def __iter__(self):  # type: ignore
         """
         Allows for iteration over the ordered frames of this :class:`FrameSet`.
 
         Returns:
             generator:
         """
         return (i for i in self.order)
 
-    def __reversed__(self):
+    def __reversed__(self):  # type: ignore
         """
         Allows for reversed iteration over the ordered frames of this
         :class:`FrameSet`.
 
         Returns:
             generator:
         """
         return (i for i in reversed(self.order))
 
-    def __contains__(self, item):
+    def __contains__(self, item: typing.Any) -> bool:
         """
         Check if item is a member of this :class:`FrameSet`.
 
         Args:
             item (int): the frame number to check for
 
         Returns:
             bool:
         """
         return item in self.items
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         """
         Builds the hash of this :class:`FrameSet` for equality checking and to
         allow use as a dictionary key.
 
         Returns:
             int:
         """
         return hash(self.frange) | hash(self.items) | hash(self.order)
 
-    def __lt__(self, other):
+    def __lt__(self, other: typing.Any) -> typing.Any:
         """
         Check if self < other via a comparison of the contents. If other is not
         a :class:`FrameSet`, but is a set, frozenset, or is iterable, it will be
         cast to a :class:`FrameSet`.
 
         Note:
 
@@ -690,15 +692,15 @@
         """
         other = self._cast_to_frameset(other)
         if other is NotImplemented:
             return NotImplemented
         return self.items < other.items or (
                 self.items == other.items and self.order < other.order)
 
-    def __le__(self, other):
+    def __le__(self, other: typing.Any) -> typing.Any:
         """
         Check if `self` <= `other` via a comparison of the contents.
         If `other` is not a :class:`FrameSet`, but is a set, frozenset, or
         is iterable, it will be cast to a :class:`FrameSet`.
 
         Args:
             other (:class:`FrameSet`): Also accepts an object that can be cast to a :class:`FrameSet`
@@ -708,15 +710,15 @@
             :class:`NotImplemented`: if `other` fails to convert to a :class:`FrameSet`
         """
         other = self._cast_to_frameset(other)
         if other is NotImplemented:
             return NotImplemented
         return self.items <= other.items
 
-    def __eq__(self, other):
+    def __eq__(self, other: typing.Any) -> typing.Any:
         """
         Check if `self` == `other` via a comparison of the hash of
         their contents.
         If `other` is not a :class:`FrameSet`, but is a set, frozenset, or
         is iterable, it will be cast to a :class:`FrameSet`.
 
         Args:
@@ -730,15 +732,15 @@
             if not hasattr(other, '__iter__'):
                 return NotImplemented
             other = self.from_iterable(other)
         this = hash(self.items) | hash(self.order)
         that = hash(other.items) | hash(other.order)
         return this == that
 
-    def __ne__(self, other):
+    def __ne__(self, other: typing.Any) -> typing.Any:
         """
         Check if `self` != `other` via a comparison of the hash of
         their contents.
         If `other` is not a :class:`FrameSet`, but is a set, frozenset, or
         is iterable, it will be cast to a :class:`FrameSet`.
 
         Args:
@@ -749,15 +751,15 @@
             :class:`NotImplemented`: if `other` fails to convert to a :class:`FrameSet`
         """
         is_equals = self == other
         if is_equals != NotImplemented:
             return not is_equals
         return is_equals
 
-    def __ge__(self, other):
+    def __ge__(self, other: typing.Any) -> typing.Any:
         """
         Check if `self` >= `other` via a comparison of the contents.
         If `other` is not a :class:`FrameSet`, but is a set, frozenset, or
         is iterable, it will be cast to a :class:`FrameSet`.
 
         Args:
             other (:class:`FrameSet`): Also accepts an object that can be cast to a :class:`FrameSet`
@@ -767,15 +769,15 @@
             :class:`NotImplemented`: if `other` fails to convert to a :class:`FrameSet`
         """
         other = self._cast_to_frameset(other)
         if other is NotImplemented:
             return NotImplemented
         return self.items >= other.items
 
-    def __gt__(self, other):
+    def __gt__(self, other: typing.Any) -> typing.Any:
         """
         Check if `self` > `other` via a comparison of the contents.
         If `other` is not a :class:`FrameSet`, but is a set, frozenset, or
         is iterable, it will be cast to a :class:`FrameSet`.
 
         Note:
            A :class:`FrameSet` is greater than `other` if the set of its
@@ -797,15 +799,15 @@
         """
         other = self._cast_to_frameset(other)
         if other is NotImplemented:
             return NotImplemented
         return self.items > other.items or (
                 self.items == other.items and self.order > other.order)
 
-    def __and__(self, other):
+    def __and__(self, other: typing.Any) -> typing.Any:
         """
         Overloads the ``&`` operator.
         Returns a new :class:`FrameSet` that holds only the
         frames `self` and `other` have in common.
 
         Note:
 
@@ -822,15 +824,15 @@
         other = self._cast_to_frameset(other)
         if other is NotImplemented:
             return NotImplemented
         return self.from_iterable(self.items & other.items, sort=True)
 
     __rand__ = __and__
 
-    def __sub__(self, other):
+    def __sub__(self, other: typing.Any) -> typing.Any:
         """
         Overloads the ``-`` operator.
         Returns a new :class:`FrameSet` that holds only the
         frames of `self` that are not in `other.`
 
         Note:
 
@@ -844,15 +846,15 @@
             :class:`NotImplemented`: if `other` fails to convert to a :class:`FrameSet`
         """
         other = self._cast_to_frameset(other)
         if other is NotImplemented:
             return NotImplemented
         return self.from_iterable(self.items - other.items, sort=True)
 
-    def __rsub__(self, other):
+    def __rsub__(self, other: typing.Any) -> typing.Any:
         """
         Overloads the ``-`` operator.
         Returns a new :class:`FrameSet` that holds only the
         frames of `other` that are not in `self.`
 
         Note:
 
@@ -866,15 +868,15 @@
             :class:`NotImplemented`: if `other` fails to convert to a :class:`FrameSet`
         """
         other = self._cast_to_frameset(other)
         if other is NotImplemented:
             return NotImplemented
         return self.from_iterable(other.items - self.items, sort=True)
 
-    def __or__(self, other):
+    def __or__(self, other: typing.Any) -> typing.Any:
         """
         Overloads the ``|`` operator.
         Returns a new :class:`FrameSet` that holds all the
         frames in `self,` `other,` or both.
 
         Note:
 
@@ -891,15 +893,15 @@
         other = self._cast_to_frameset(other)
         if other is NotImplemented:
             return NotImplemented
         return self.from_iterable(self.items | other.items, sort=True)
 
     __ror__ = __or__
 
-    def __xor__(self, other):
+    def __xor__(self, other: typing.Any) -> typing.Any:
         """
         Overloads the ``^`` operator.
         Returns a new :class:`FrameSet` that holds all the
         frames in `self` or `other` but not both.
 
         Note:
             The order of operations is irrelevant:
@@ -915,15 +917,15 @@
         other = self._cast_to_frameset(other)
         if other is NotImplemented:
             return NotImplemented
         return self.from_iterable(self.items ^ other.items, sort=True)
 
     __rxor__ = __xor__
 
-    def isdisjoint(self, other) -> bool | NotImplemented:  # type: ignore
+    def isdisjoint(self, other: typing.Any) -> bool | NotImplemented:  # type: ignore
         """
         Check if the contents of :class:self has no common intersection with the
         contents of :class:other.
 
         Args:
             other (:class:`FrameSet`):
 
@@ -932,91 +934,91 @@
             :class:`NotImplemented`: if `other` fails to convert to a :class:`FrameSet`
         """
         other = self._cast_to_frameset(other)
         if other is NotImplemented:
             return NotImplemented
         return self.items.isdisjoint(other.items)
 
-    def issubset(self, other) -> bool | NotImplemented:  # type: ignore
+    def issubset(self, other: typing.Any) -> bool | NotImplemented:  # type: ignore
         """
         Check if the contents of `self` is a subset of the contents of
         `other.`
 
         Args:
             other (:class:`FrameSet`):
 
         Returns:
             bool:
             :class:`NotImplemented`: if `other` fails to convert to a :class:`FrameSet`
         """
         other = self._cast_to_frameset(other)
         if other is NotImplemented:
             return NotImplemented
-        return self.items <= other.items
+        return self.items <= other.items  # type: ignore
 
-    def issuperset(self, other) -> bool | NotImplemented:  # type: ignore
+    def issuperset(self, other: typing.Any) -> bool | NotImplemented:  # type: ignore
         """
         Check if the contents of `self` is a superset of the contents of
         `other.`
 
         Args:
             other (:class:`FrameSet`):
 
         Returns:
             bool:
             :class:`NotImplemented`: if `other` fails to convert to a :class:`FrameSet`
         """
         other = self._cast_to_frameset(other)
         if other is NotImplemented:
             return NotImplemented
-        return self.items >= other.items
+        return self.items >= other.items  # type: ignore
 
-    def union(self, *other) -> FrameSet:
+    def union(self, *other: typing.Any) -> FrameSet:
         """
         Returns a new :class:`FrameSet` with the elements of `self` and
         of `other`.
 
         Args:
             other (:class:`FrameSet`): or objects that can cast to :class:`FrameSet`
 
         Returns:
             :class:`FrameSet`:
         """
         from_frozenset = self.items.union(*(set(o) for o in other))
         return self.from_iterable(from_frozenset, sort=True)
 
-    def intersection(self, *other) -> FrameSet:
+    def intersection(self, *other: typing.Any) -> FrameSet:
         """
         Returns a new :class:`FrameSet` with the elements common to `self` and
         `other`.
 
         Args:
             other (:class:`FrameSet`): or objects that can cast to :class:`FrameSet`
 
         Returns:
             :class:`FrameSet`:
         """
         from_frozenset = self.items.intersection(*(set(o) for o in other))
         return self.from_iterable(from_frozenset, sort=True)
 
-    def difference(self, *other) -> FrameSet:
+    def difference(self, *other: typing.Any) -> FrameSet:
         """
         Returns a new :class:`FrameSet` with elements in `self` but not in
         `other`.
 
         Args:
             other (:class:`FrameSet`): or objects that can cast to :class:`FrameSet`
 
         Returns:
             :class:`FrameSet`:
         """
         from_frozenset = self.items.difference(*(set(o) for o in other))
         return self.from_iterable(from_frozenset, sort=True)
 
-    def symmetric_difference(self, other) -> FrameSet:
+    def symmetric_difference(self, other: typing.Any) -> FrameSet:
         """
         Returns a new :class:`FrameSet` that contains all the elements in either
         `self` or `other`, but not both.
 
         Args:
             other (:class:`FrameSet`):
 
@@ -1039,15 +1041,15 @@
         fs = self.__class__.__new__(self.__class__)
         fs._frange = self._frange
         fs._items = self._items
         fs._order = self._order
         return fs
 
     @classmethod
-    def _maxSizeCheck(cls, obj: int | float | decimal.Decimal | Sized):
+    def _maxSizeCheck(cls, obj: int | float | decimal.Decimal | Sized) -> None:
         """
         Raise a MaxSizeException if ``obj`` exceeds MAX_FRAME_SIZE
 
         Args:
             obj (numbers.Number or collection):
 
         Raises:
@@ -1110,15 +1112,15 @@
             zfill (int):
             decimal_places (int or None):
 
         Returns:
             str:
         """
 
-        def _do_pad(match):
+        def _do_pad(match: typing.Any) -> str:
             """
             Substitutes padded for unpadded frames.
             """
             result = list(match.groups())
 
             neg, start = result[:2]
             result[:2] = [pad(neg + start, zfill, decimal_places)]
@@ -1152,27 +1154,27 @@
             msg = 'Could not parse "{0}": did not match {1}'
             raise ParseException(msg.format(frange, cls.FRANGE_RE.pattern))
         start, end, modifier, chunk = match.groups()
         start = normalizeFrame(start)
         end = normalizeFrame(end) if end is not None else start
         chunk = normalizeFrame(chunk) if chunk is not None else 1
 
-        if end > start and chunk is not None and chunk < 0:
+        if end > start and chunk is not None and chunk < 0:  # type: ignore[operator]
             msg = 'Could not parse "{0}: chunk can not be negative'
             raise ParseException(msg.format(frange))
 
         # a zero chunk is just plain illogical
         if chunk == 0:
             msg = 'Could not parse "{0}": chunk cannot be 0'
             raise ParseException(msg.format(frange))
 
-        return start, end, modifier, abs(chunk)
+        return start, end, modifier, abs(chunk)  # type: ignore
 
     @staticmethod
-    def _build_frange_part(start: object, stop: object, stride: int | decimal.Decimal | None, zfill: int = 0) -> str:
+    def _build_frange_part(start: object, stop: object, stride: int|float|decimal.Decimal|None, zfill: int = 0) -> str:
         """
         Private method: builds a proper and padded frame range string.
 
         Args:
             start (int): first frame
             stop (int or None): last frame
             stride (int or None): increment
@@ -1198,15 +1200,15 @@
             start: decimal.Decimal,
             stop: decimal.Decimal,
             count: int,
             stride: decimal.Decimal | None,
             min_stride: decimal.Decimal,
             max_stride: decimal.Decimal,
             zfill: int = 0
-    ):
+        ) -> str:
         """
         Private method: builds a proper and padded subframe range string from
         decimal values.
 
         Args:
             start (decimal.Decimal): first frame
             stop (decimal.Decimal): last frame
@@ -1239,19 +1241,22 @@
         # Adjust end frame if required so correct number of steps is
         # calculated when recreating FrameSet from frange string
         while abs(stop - start) / stride + 1 < count:
             exponent = int(stop.as_tuple().exponent)
             delta = decimal.Decimal(1).scaleb(exponent)
             stop += delta.copy_sign(stop)
 
-        start, stop = normalizeFrames([start, stop])
+        start, stop = normalizeFrames([start, stop])  # type:ignore[assignment]
         return FrameSet._build_frange_part(start, stop, stride, zfill=zfill)
 
     @staticmethod
-    def framesToFrameRanges(frames: typing.Iterable, zfill: int = 0) -> typing.Iterator[str]:
+    def framesToFrameRanges(
+            frames: typing.Iterable[typing.Any],
+            zfill: int = 0
+        ) -> typing.Iterator[str]:
         """
         Converts a sequence of frames to a series of padded
         frame range strings.
 
         Args:
             frames (collections.Iterable): sequence of frames to process
             zfill (int): width for zero padding
@@ -1366,15 +1371,20 @@
                 stride = curr_strides.pop() if len(curr_strides) == 1 else None
                 yield _build_decimal(curr_start, curr_frame, curr_count,
                                      stride, curr_min_stride, curr_max_stride, zfill)
             else:
                 yield _build(curr_start, curr_frame, curr_stride, zfill)
 
     @staticmethod
-    def framesToFrameRange(frames: typing.Iterable, sort: bool = True, zfill: int = 0, compress: bool = False) -> str:
+    def framesToFrameRange(
+            frames: typing.Iterable[typing.Any],
+            sort: bool = True,
+            zfill: int = 0,
+            compress: bool = False
+        ) -> str:
         """
         Converts an iterator of frames into a
         frame range string.
 
         Args:
             frames (collections.Iterable): sequence of frames to process
             sort (bool): sort the sequence before processing
```

### Comparing `Fileseq-2.1.0/src/fileseq/utils.py` & `fileseq-2.1.1/src/fileseq/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 """
 utils - General tools of use to fileseq operations.
 """
+from __future__ import annotations
 
+import collections.abc
 import decimal
 import os
 import typing
 
 import sys
 from itertools import chain, count, islice
 
 from . import exceptions
 
 
 FILESYSTEM_ENCODING = sys.getfilesystemencoding() or 'utf-8'
 
 
-def quantize(number, decimal_places, rounding=decimal.ROUND_HALF_EVEN):
+def quantize(
+        number: decimal.Decimal,
+        decimal_places: int,
+        rounding: str = decimal.ROUND_HALF_EVEN
+        ) -> decimal.Decimal:
     """
     Round a decimal value to given number of decimal places
 
     Args:
         number (decimal.Decimal): Decimal number to round
         decimal_places (int): Number of decimal places in return value
         rounding (str): decimal.Decimal rounding mode. See rounding argument of
@@ -31,15 +37,15 @@
     quantize_exponent = decimal.Decimal(1).scaleb(-decimal_places)
     nq = number.quantize(quantize_exponent, rounding=rounding)
     if nq.is_zero():
         return nq.copy_abs()
     return nq
 
 
-def lenRange(start, stop, step=1):
+def lenRange(start: int, stop: int, step: int = 1) -> int:
     """
     Get the length of values for a given range, exclusive of the stop
 
     Args:
         start (int):
         stop (int):
         step (int):
@@ -63,49 +69,49 @@
 
     Provides the features of an islice, with the added support
     for checking the length of the range.
     """
 
     __slots__ = ['_len', '_islice', '_start', '_stop', '_step']
 
-    def __init__(self, start, stop=None, step=1):
+    def __init__(self, start: int, stop: typing.Optional[int] = None, step: int = 1):
         if stop is None:
             start, stop = 0, start
 
         self._len = lenRange(start, stop, step)
         self._islice = islice(count(start, step), self._len)
         self._start = start
         self._stop = stop
         self._step = step
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         if self._step == 1:
             return 'range({}, {})'.format(self._start, self._stop)
         else:
             return 'range({}, {}, {})'.format(self._start, self._stop, self._step)
 
-    def __len__(self):
+    def __len__(self) -> int:
         return self._len
 
-    def __next__(self):
+    def __next__(self) -> int:
         return next(self._islice)
 
-    def __iter__(self):
+    def __iter__(self) -> typing.Iterable[typing.Any]:
         return self._islice.__iter__()
 
     @property
-    def start(self):
+    def start(self) -> int:
         return self._start
 
     @property
-    def stop(self):
+    def stop(self) -> int:
         return self._stop
 
     @property
-    def step(self):
+    def step(self) -> int:
         return self._step
 
 
 # Issue #44
 # On Windows platform, it is possible for xrange to get an
 # OverflowError if a value passed to xrange exceeds the size of a C long.
 # Switch to an alternate implementation.
@@ -113,50 +119,51 @@
     xrange = range = xrange2
 else:
     xrange = range
 
 
 class _islice(object):
 
-    def __init__(self, gen, start, stop, step=1):
+    def __init__(self, gen: typing.Iterable[typing.Any], start: int, stop: int, step: int = 1):
         self._gen = gen
         self._start = start
         self._stop = stop
         self._step = step
 
-    def __len__(self):
+    def __len__(self) -> int:
         return lenRange(self._start, self._stop, self._step)
 
-    def __next__(self):
-        return next(self._gen)
+    def __next__(self) -> typing.Any:
+        # noinspection PyTypeChecker
+        return next(self._gen)  # type:ignore
 
-    def __iter__(self):
+    def __iter__(self) -> typing.Iterable[typing.Any]:
         return self._gen.__iter__()
 
     @property
-    def start(self):
+    def start(self) -> int:
         return self._start
 
     @property
-    def stop(self):
+    def stop(self) -> int:
         return self._stop
 
     @property
-    def step(self):
+    def step(self) -> int:
         return self._step
 
 
 class _xfrange(_islice):
 
-    def __len__(self):
+    def __len__(self) -> int:
         stop = self._stop + (1 if self._start <= self._stop else -1)
         return lenRange(self._start, stop, self._step)
 
 
-def xfrange(start, stop, step=1, maxSize=-1):
+def xfrange(start: int, stop: int, step: int = 1, maxSize: int = -1) -> typing.Generator[typing.Any, None, None]:
     """
     Returns a generator that yields the frames from start to stop, inclusive.
     In other words it adds or subtracts a frame, as necessary, to return the
     stop value as well, if the stepped range would touch that value.
 
     Args:
         start (int):
@@ -169,15 +176,15 @@
 
     Raises:
         :class:`fileseq.exceptions.MaxSizeException`: if size is exceeded
     """
     if not step:
         raise ValueError('xfrange() step argument must not be zero')
 
-    start, stop, step = normalizeFrames([start, stop, step])
+    start, stop, step = normalizeFrames([start, stop, step])  # type:ignore[assignment]
 
     if start <= stop:
         step = abs(step)
     else:
         step = -abs(step)
 
     if isinstance(start, int):
@@ -189,22 +196,22 @@
         raise exceptions.MaxSizeException(
             "Size %d > %s (MAX_FRAME_SIZE)" % (size, maxSize))
 
     # because an xrange is an odd object all its own, we wrap it in a
     # generator expression to get a proper Generator
     if isinstance(start, int):
         offset = step // abs(step)
-        gen = (f for f in range(start, stop + offset, step))
+        gen = (f for f in range(start, stop + offset, step))  # type:ignore
     else:
         gen = (start + i * step for i in range(size))
 
-    return _xfrange(gen, start, stop, step)
+    return _xfrange(gen, start, stop, step)  # type:ignore
 
 
-def batchFrames(start, stop, batch_size):
+def batchFrames(start: int, stop: int, batch_size: int) -> typing.Iterable[typing.Any]:
     """
     Returns a generator that yields batches of frames from start to stop, inclusive.
     Each batch value is a ``range`` generator object, also providing start, stop, and
     step properties.
     The last batch frame length may be smaller if the batches cannot be divided evenly.
 
     start value is allowed to be greater than stop value, to generate decreasing frame
@@ -225,15 +232,15 @@
         if start <= stop:
             sub_stop = min(i - 1 + batch_size, stop)
         else:
             sub_stop = max(i + 1 - batch_size, stop)
         yield xfrange(i, sub_stop)
 
 
-def batchIterable(it, batch_size):
+def batchIterable(it: typing.Iterable[typing.Any], batch_size: int) -> typing.Iterable[typing.Any]:
     """
     Returns a generator that yields batches of items returned by the given iterable.
     The last batch frame length may be smaller if the batches cannot be divided evenly.
 
     Args:
         it (iterable): An iterable from which to yield batches of values
         batch_size (int): max size of each batch
@@ -244,28 +251,28 @@
     if batch_size <= 0:
         return
 
     # Try to get the length. If it is a generator with no
     # known length, then we have to use a less efficient
     # method that builds results by exhausting the generator
     try:
-        length = len(it)
+        length = len(it)  # type:ignore
     except TypeError:
         for b in _batchGenerator(it, batch_size):
             yield b
         return
 
     # We can use the known length to yield slices
-    for start in xrange(0, length, batch_size):
+    for start in xrange(0, length, batch_size):  # type:ignore
         stop = start + batch_size
         gen = islice(it, start, stop)
         yield _islice(gen, start, stop)
 
 
-def _batchGenerator(gen, batch_size):
+def _batchGenerator(gen: typing.Iterable[typing.Any], batch_size: int) -> typing.Generator[typing.Any, None, None]:
     """
     A batching generator function that handles a generator
     type, where the length isn't known.
 
     Args:
         gen: generator object
         batch_size (int): max size of each batch
@@ -279,15 +286,15 @@
         if len(batch) == batch_size:
             yield batch
             batch = []
     if batch:
         yield batch
 
 
-def normalizeFrame(frame):
+def normalizeFrame(frame: int | float | decimal.Decimal | str) -> int | float | decimal.Decimal | None:
     """
     Convert a frame number to the most appropriate type - the most compact type
     that doesn't affect precision, for example numbers that convert exactly
     to integer values will be converted to int
 
     Args:
         frame (int, float, decimal.Decimal, str): frame number to normalize
@@ -312,20 +319,20 @@
     else:
         try:
             return int(frame)
         except ValueError:
             try:
                 frame = decimal.Decimal(frame)
             except decimal.DecimalException:
-                return frame
+                return frame  # type:ignore[return-value]
             else:
                 return normalizeFrame(frame)
 
 
-def normalizeFrames(frames: typing.Iterable[typing.Any]) -> list:
+def normalizeFrames(frames: typing.Iterable[typing.Any]) -> list[int | float | decimal.Decimal]:
     """
     Convert a sequence of frame numbers to the most appropriate type for the
     overall sequence, where all members of the result are of the same type.
 
     Args:
         frames (iterable of int, float, decimal.Decimal, or str):
             frame numbers to normalize
@@ -360,15 +367,18 @@
             -frame.as_tuple().exponent for frame in frames
         )
         frames = [quantize(frame, maximum_decimal_places) for frame in frames]
 
     return frames
 
 
-def unique(seen, *iterables):
+def unique(
+        seen: typing.Set[typing.Any],
+        *iterables: typing.Iterable[typing.Any]
+    ) -> typing.Generator[typing.Any, None, None]:
     """
     Get the unique items in iterables while preserving order.  Note that this
     mutates the seen set provided only when the returned generator is used.
 
     Args:
         seen (set): either an empty set, or the set of things already seen
         *iterables: one or more iterable lists to chain together
@@ -378,15 +388,15 @@
     """
     _add = seen.add
     # return a generator of the unique items and the set of the seen items
     # the seen set will mutate when the generator is iterated over
     return (i for i in chain(*iterables) if i not in seen and not _add(i))
 
 
-def pad(number, width=0, decimal_places=None):
+def pad(number: typing.Any, width: typing.Optional[int] = 0, decimal_places: typing.Optional[int] = None) -> str:
     """
     Return the zero-padded string of a given number.
 
     Args:
         number (str, int, float, or decimal.Decimal): the number to pad
         width (int): width for zero padding the integral component
         decimal_places (int): number of decimal places to use in frame range
@@ -400,15 +410,15 @@
     # See _DeriveClipTimeString for formatting of templateAssetPath
     # https://github.com/PixarAnimationStudios/USD/blob/release/pxr/usd/usd/clipSetDefinition.cpp
     if decimal_places == 0:
         try:
             number = round(number) or 0
         except TypeError:
             pass
-        return str(number).partition(".")[0].zfill(width)
+        return str(number).partition(".")[0].zfill(width)  # type:ignore[arg-type]
 
     # USD ultimately uses vsnprintf to format floats for templateAssetPath:
     # _DeriveClipTimeString -> TfStringPrintf -> ArchVStringPrintf -> ArchVsnprintf -> vsnprintf
     # Since glibc 2.17 the printf family of functions rounds floats using the
     # current IEEE rounding mode, by default bankers' rounding (FE_TONEAREST).
     # See https://sourceware.org/bugzilla/show_bug.cgi?id=5044 and man(3) fegetround
     # Also https://www.exploringbinary.com/inconsistent-rounding-of-printed-floating-point-numbers/
@@ -420,15 +430,15 @@
     number = str(number)
 
     parts = number.split(".", 1)
     parts[0] = parts[0].zfill(width)
     return ".".join(parts)
 
 
-def _getPathSep(path):
+def _getPathSep(path: str) -> str:
     """
     Abstracts returning the appropriate path separator
     for the given path string.
 
     This implementation always returns ``os.sep``
 
     Abstracted to make test mocking easier.
@@ -441,33 +451,33 @@
     """
     return os.sep
 
 
 _STR_TYPES = frozenset((str, bytes))
 
 
-def asString(obj):
+def asString(obj: object) -> str:
     """
-    Ensure an object is either explicitly str or unicode
+    Ensure an object is explicitly str type
     and not some derived type that can change semantics.
 
-    If the object is unicode, return unicode.
+    If the object is str, return str.
     Otherwise, return the string conversion of the object.
 
     Args:
-        obj: Object to return as str or unicode
+        obj: Object to return as str
 
     Returns:
-        str or unicode:
+        str:
     """
     typ = type(obj)
     # explicit type check as faster path
     if typ in _STR_TYPES:
         if typ is bytes:
-            obj = os.fsdecode(obj)
-        return obj
+            obj = os.fsdecode(obj)  # type: ignore
+        return obj  # type: ignore
     # derived type check
     elif isinstance(obj, bytes):
         obj = obj.decode(FILESYSTEM_ENCODING)
     else:
         obj = str(obj)
     return str(obj)
```

### Comparing `Fileseq-2.1.0/test/test_fuzz.py` & `fileseq-2.1.1/test/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `Fileseq-2.1.0/test/test_unit.py` & `fileseq-2.1.1/test/test_unit.py`

 * *Files identical despite different names*

