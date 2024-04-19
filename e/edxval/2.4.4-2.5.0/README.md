# Comparing `tmp/edxval-2.4.4.tar.gz` & `tmp/edxval-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edxval-2.4.4.tar", last modified: Thu Oct  5 17:15:16 2023, max compression
+gzip compressed data, was "edxval-2.5.0.tar", last modified: Fri Apr 19 23:54:02 2024, max compression
```

## Comparing `edxval-2.4.4.tar` & `edxval-2.5.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 17:15:16.721067 edxval-2.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35135 2023-10-05 17:15:11.000000 edxval-2.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-10-05 17:15:11.000000 edxval-2.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      641 2023-10-05 17:15:16.721067 edxval-2.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2023-10-05 17:15:11.000000 edxval-2.4.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 17:15:16.717067 edxval-2.4.4/edxval/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    46499 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 17:15:16.717067 edxval-2.4.4/edxval/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/config/waffle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 17:15:16.717067 edxval-2.4.4/edxval/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    10732 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/migrations/0001_squashed_0016_add_transcript_credentials_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/migrations/0002_add_error_description_field.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/migrations/0003_delete_transcriptcredentials.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22828 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     8154 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 17:15:16.721067 edxval-2.4.4/edxval/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10706 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/tests/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)   131722 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/tests/test_transcript_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    43750 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/transcript_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     8793 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15506 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2023-10-05 17:15:11.000000 edxval-2.4.4/edxval/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 17:15:16.717067 edxval-2.4.4/edxval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2023-10-05 17:15:16.000000 edxval-2.4.4/edxval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      956 2023-10-05 17:15:16.000000 edxval-2.4.4/edxval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 17:15:16.000000 edxval-2.4.4/edxval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-10-05 17:15:16.000000 edxval-2.4.4/edxval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-05 17:15:16.000000 edxval-2.4.4/edxval.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 17:15:16.721067 edxval-2.4.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2023-10-05 17:15:11.000000 edxval-2.4.4/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-10-05 17:15:11.000000 edxval-2.4.4/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (127)      789 2023-10-05 17:15:16.721067 edxval-2.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2023-10-05 17:15:11.000000 edxval-2.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:54:02.717501 edxval-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35135 2024-04-19 23:53:58.000000 edxval-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-19 23:53:58.000000 edxval-2.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-19 23:54:02.717501 edxval-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-19 23:53:58.000000 edxval-2.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:54:02.713501 edxval-2.5.0/edxval/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46499 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:54:02.713501 edxval-2.5.0/edxval/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/config/waffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:54:02.713501 edxval-2.5.0/edxval/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/migrations/0001_squashed_0016_add_transcript_credentials_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/migrations/0002_add_error_description_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/migrations/0003_delete_transcriptcredentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22828 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:54:02.713501 edxval-2.5.0/edxval/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/tests/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131722 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/tests/test_transcript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43750 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/transcript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8793 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15474 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-19 23:53:58.000000 edxval-2.5.0/edxval/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:54:02.717501 edxval-2.5.0/edxval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-19 23:54:02.000000 edxval-2.5.0/edxval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-19 23:54:02.000000 edxval-2.5.0/edxval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 23:54:02.000000 edxval-2.5.0/edxval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-19 23:54:02.000000 edxval-2.5.0/edxval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 23:54:02.000000 edxval-2.5.0/edxval.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:54:02.713501 edxval-2.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-19 23:53:58.000000 edxval-2.5.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-19 23:53:58.000000 edxval-2.5.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-19 23:54:02.717501 edxval-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-19 23:53:58.000000 edxval-2.5.0/setup.py
```

### Comparing `edxval-2.4.4/LICENSE` & `edxval-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edxval-2.4.4/README.rst` & `edxval-2.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `edxval-2.4.4/edxval/admin.py` & `edxval-2.5.0/edxval/admin.py`

 * *Files identical despite different names*

### Comparing `edxval-2.4.4/edxval/api.py` & `edxval-2.5.0/edxval/api.py`

 * *Files identical despite different names*

### Comparing `edxval-2.4.4/edxval/config/waffle.py` & `edxval-2.5.0/edxval/config/waffle.py`

 * *Files identical despite different names*

### Comparing `edxval-2.4.4/edxval/exceptions.py` & `edxval-2.5.0/edxval/exceptions.py`

 * *Files identical despite different names*

### Comparing `edxval-2.4.4/edxval/migrations/0001_squashed_0016_add_transcript_credentials_model.py` & `edxval-2.5.0/edxval/migrations/0001_squashed_0016_add_transcript_credentials_model.py`

 * *Files identical despite different names*

### Comparing `edxval-2.4.4/edxval/models.py` & `edxval-2.5.0/edxval/models.py`

 * *Files identical despite different names*

### Comparing `edxval-2.4.4/edxval/serializers.py` & `edxval-2.5.0/edxval/serializers.py`

 * *Files identical despite different names*

### Comparing `edxval-2.4.4/edxval/tests/__init__.py` & `edxval-2.5.0/edxval/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `edxval-2.4.4/edxval/tests/constants.py` & `edxval-2.5.0/edxval/tests/constants.py`

 * *Files identical despite different names*

### Comparing `edxval-2.4.4/edxval/tests/test_admin.py` & `edxval-2.5.0/edxval/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `edxval-2.4.4/edxval/tests/test_api.py` & `edxval-2.5.0/edxval/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `edxval-2.4.4/edxval/tests/test_models.py` & `edxval-2.5.0/edxval/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edxval-2.4.4/edxval/tests/test_serializers.py` & `edxval-2.5.0/edxval/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `edxval-2.4.4/edxval/tests/test_transcript_utils.py` & `edxval-2.5.0/edxval/tests/test_transcript_utils.py`

 * *Files identical despite different names*

### Comparing `edxval-2.4.4/edxval/tests/test_utils.py` & `edxval-2.5.0/edxval/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edxval-2.4.4/edxval/tests/test_views.py` & `edxval-2.5.0/edxval/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `edxval-2.4.4/edxval/transcript_utils.py` & `edxval-2.5.0/edxval/transcript_utils.py`

 * *Files identical despite different names*

### Comparing `edxval-2.4.4/edxval/urls.py` & `edxval-2.5.0/edxval/urls.py`

 * *Files identical despite different names*

### Comparing `edxval-2.4.4/edxval/utils.py` & `edxval-2.5.0/edxval/utils.py`

 * *Files identical despite different names*

### Comparing `edxval-2.4.4/edxval/views.py` & `edxval-2.5.0/edxval/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,15 +279,15 @@
 
         course_id = request.data['course_id']
         edx_video_id = request.data['edx_video_id']
         generated_images = request.data['generated_images']
 
         try:
             validate_generated_images(generated_images, LIST_MAX_ITEMS)
-        except Exception as e:  # pylint: disable=broad-except
+        except Exception as e:
             return Response(
                 status=status.HTTP_400_BAD_REQUEST,
                 data={'message': str(e)}
             )
 
         try:
             course_video = CourseVideo.objects.select_related('video_image').get(
```

### Comparing `edxval-2.4.4/edxval/wsgi.py` & `edxval-2.5.0/edxval/wsgi.py`

 * *Files identical despite different names*

### Comparing `edxval-2.4.4/edxval.egg-info/SOURCES.txt` & `edxval-2.5.0/edxval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edxval-2.4.4/setup.cfg` & `edxval-2.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `edxval-2.4.4/setup.py` & `edxval-2.5.0/setup.py`

 * *Files identical despite different names*

