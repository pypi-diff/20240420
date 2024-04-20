# Comparing `tmp/mixport-0.1.2.tar.gz` & `tmp/mixport-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixport-0.1.2.tar", last modified: Mon Jan 29 01:47:23 2024, max compression
+gzip compressed data, was "mixport-0.1.3.tar", last modified: Sat Apr 20 02:04:05 2024, max compression
```

## Comparing `mixport-0.1.2.tar` & `mixport-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 01:47:23.054364 mixport-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-01-29 01:47:15.000000 mixport-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-01-29 01:47:23.054364 mixport-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-01-29 01:47:15.000000 mixport-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 01:47:23.050364 mixport-0.1.2/mixport/
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-01-29 01:47:15.000000 mixport-0.1.2/mixport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-29 01:47:15.000000 mixport-0.1.2/mixport/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-01-29 01:47:15.000000 mixport-0.1.2/mixport/transcode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 01:47:23.054364 mixport-0.1.2/mixport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-01-29 01:47:23.000000 mixport-0.1.2/mixport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-01-29 01:47:23.000000 mixport-0.1.2/mixport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 01:47:23.000000 mixport-0.1.2/mixport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-29 01:47:23.000000 mixport-0.1.2/mixport.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-29 01:47:23.000000 mixport-0.1.2/mixport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-29 01:47:23.000000 mixport-0.1.2/mixport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-01-29 01:47:15.000000 mixport-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 01:47:23.054364 mixport-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:04:05.212705 mixport-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-20 02:04:00.000000 mixport-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-20 02:04:05.212705 mixport-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-20 02:04:00.000000 mixport-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:04:05.212705 mixport-0.1.3/mixport/
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-20 02:04:00.000000 mixport-0.1.3/mixport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-20 02:04:00.000000 mixport-0.1.3/mixport/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-20 02:04:00.000000 mixport-0.1.3/mixport/transcode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:04:05.212705 mixport-0.1.3/mixport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-20 02:04:05.000000 mixport-0.1.3/mixport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-20 02:04:05.000000 mixport-0.1.3/mixport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 02:04:05.000000 mixport-0.1.3/mixport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-20 02:04:05.000000 mixport-0.1.3/mixport.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-20 02:04:05.000000 mixport-0.1.3/mixport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-20 02:04:05.000000 mixport-0.1.3/mixport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-20 02:04:00.000000 mixport-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 02:04:05.212705 mixport-0.1.3/setup.cfg
```

### Comparing `mixport-0.1.2/LICENSE` & `mixport-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mixport-0.1.2/PKG-INFO` & `mixport-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixport
-Version: 0.1.2
+Version: 0.1.3
 Summary: CLI tool for transcoding Mixxx recordings
 License: MIT License
         
         Copyright (c) 2023 fwcd
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `mixport-0.1.2/README.md` & `mixport-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mixport-0.1.2/mixport/__init__.py` & `mixport-0.1.3/mixport/__init__.py`

 * *Files identical despite different names*

### Comparing `mixport-0.1.2/mixport/transcode.py` & `mixport-0.1.3/mixport/transcode.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,13 +30,14 @@
     duration = get_duration(in_audio_path)
     print(f'Duration: {duration}')
 
     builder = ffmpeg.input(str(in_audio_path))
 
     if trim_duration:
         builder = builder.filter('atrim', duration=trim_duration)
+        duration = trim_duration
     if fade_in:
         builder = builder.filter('afade', type='in', duration=fade_in)
     if fade_out:
         builder = builder.filter('afade', type='out', duration=fade_out, start_time=duration - fade_out)
 
     builder.output(str(out_audio_path)).run(overwrite_output=True)
```

### Comparing `mixport-0.1.2/mixport.egg-info/PKG-INFO` & `mixport-0.1.3/mixport.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixport
-Version: 0.1.2
+Version: 0.1.3
 Summary: CLI tool for transcoding Mixxx recordings
 License: MIT License
         
         Copyright (c) 2023 fwcd
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `mixport-0.1.2/pyproject.toml` & `mixport-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mixport"
-version = "0.1.2"
+version = "0.1.3"
 description = "CLI tool for transcoding Mixxx recordings"
 readme = "README.md"
 requires-python = ">=3.9"
 license = { file = "LICENSE" }
 classifiers = ["Topic :: Utilities", "Topic :: Multimedia :: Sound/Audio :: Conversion"]
 keywords = ["mixxx", "ffmpeg"]
 dependencies = [
```

