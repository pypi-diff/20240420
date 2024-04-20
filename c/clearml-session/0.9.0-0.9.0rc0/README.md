# Comparing `tmp/clearml_session-0.9.0-py3-none-any.whl.zip` & `tmp/clearml_session-0.9.0rc0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 41801 bytes, number of entries: 12
--rw-r--r--  2.0 unx        0 b- defN 23-Sep-15 11:16 clearml_session/__init__.py
--rw-r--r--  2.0 unx    55382 b- defN 23-Sep-15 11:16 clearml_session/__main__.py
--rw-r--r--  2.0 unx    39840 b- defN 23-Sep-15 11:16 clearml_session/interactive_session_task.py
--rw-r--r--  2.0 unx     4781 b- defN 23-Sep-15 11:16 clearml_session/single_thread_proxy.py
--rw-r--r--  2.0 unx    15948 b- defN 23-Sep-15 11:16 clearml_session/tcp_proxy.py
--rw-r--r--  2.0 unx       22 b- defN 23-Sep-15 11:16 clearml_session/version.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Sep-15 11:16 clearml_session-0.9.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    18809 b- defN 23-Sep-15 11:16 clearml_session-0.9.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Sep-15 11:16 clearml_session-0.9.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 23-Sep-15 11:16 clearml_session-0.9.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 23-Sep-15 11:16 clearml_session-0.9.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1060 b- defN 23-Sep-15 11:16 clearml_session-0.9.0.dist-info/RECORD
-12 files, 147374 bytes uncompressed, 39995 bytes compressed:  72.9%
+Zip file size: 41840 bytes, number of entries: 12
+-rw-r--r--  2.0 unx        0 b- defN 23-Sep-13 11:35 clearml_session/__init__.py
+-rw-r--r--  2.0 unx    55364 b- defN 23-Sep-13 11:35 clearml_session/__main__.py
+-rw-r--r--  2.0 unx    39840 b- defN 23-Sep-13 11:35 clearml_session/interactive_session_task.py
+-rw-r--r--  2.0 unx     4781 b- defN 23-Sep-13 11:35 clearml_session/single_thread_proxy.py
+-rw-r--r--  2.0 unx    15948 b- defN 23-Sep-13 11:35 clearml_session/tcp_proxy.py
+-rw-r--r--  2.0 unx       25 b- defN 23-Sep-13 11:35 clearml_session/version.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Sep-13 11:36 clearml_session-0.9.0rc0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    18812 b- defN 23-Sep-13 11:36 clearml_session-0.9.0rc0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Sep-13 11:36 clearml_session-0.9.0rc0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 23-Sep-13 11:36 clearml_session-0.9.0rc0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-Sep-13 11:36 clearml_session-0.9.0rc0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1078 b- defN 23-Sep-13 11:36 clearml_session-0.9.0rc0.dist-info/RECORD
+12 files, 147380 bytes uncompressed, 39998 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: clearml_session/tcp_proxy.py
 Comment: 
 
 Filename: clearml_session/version.py
 Comment: 
 
-Filename: clearml_session-0.9.0.dist-info/LICENSE
+Filename: clearml_session-0.9.0rc0.dist-info/LICENSE
 Comment: 
 
-Filename: clearml_session-0.9.0.dist-info/METADATA
+Filename: clearml_session-0.9.0rc0.dist-info/METADATA
 Comment: 
 
-Filename: clearml_session-0.9.0.dist-info/WHEEL
+Filename: clearml_session-0.9.0rc0.dist-info/WHEEL
 Comment: 
 
-Filename: clearml_session-0.9.0.dist-info/entry_points.txt
+Filename: clearml_session-0.9.0rc0.dist-info/entry_points.txt
 Comment: 
 
-Filename: clearml_session-0.9.0.dist-info/top_level.txt
+Filename: clearml_session-0.9.0rc0.dist-info/top_level.txt
 Comment: 
 
-Filename: clearml_session-0.9.0.dist-info/RECORD
+Filename: clearml_session-0.9.0rc0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## clearml_session/__main__.py

```diff
@@ -751,16 +751,15 @@
                     raise ValueError('Incorrect password')
                 except pexpect.TIMEOUT:
                     pass
     except Exception:
         child.terminate(force=True)
         child = None
     print('\n')
-    if child:
-        child.logfile = None
+    child.logfile = None
     return child, ssh_password
 
 
 def monitor_ssh_tunnel(state, task):
     def interactive_ssh(p):
         import struct, fcntl, termios, signal, sys  # noqa
```

## clearml_session/version.py

```diff
@@ -1 +1 @@
-__version__ = '0.9.0'
+__version__ = '0.9.0rc0'
```

## Comparing `clearml_session-0.9.0.dist-info/LICENSE` & `clearml_session-0.9.0rc0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `clearml_session-0.9.0.dist-info/METADATA` & `clearml_session-0.9.0rc0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clearml-session
-Version: 0.9.0
+Version: 0.9.0rc0
 Summary: clearml-session - CLI for launching JupyterLab / VSCode on a remote machine
 Home-page: https://github.com/allegroai/clearml-session
 Author: Allegroai
 Author-email: clearml@allegro.ai
 License: Apache License 2.0
 Keywords: clearml mlops devops trains development machine deep learning version control machine-learning machinelearning deeplearning deep-learning experiment-manager jupyter vscode
 Platform: UNKNOWN
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clearml-session Version: 0.9.0 Summary: clearml-
+Metadata-Version: 2.1 Name: clearml-session Version: 0.9.0rc0 Summary: clearml-
 session - CLI for launching JupyterLab / VSCode on a remote machine Home-page:
 https://github.com/allegroai/clearml-session Author: Allegroai Author-email:
 clearml@allegro.ai License: Apache License 2.0 Keywords: clearml mlops devops
 trains development machine deep learning version control machine-learning
 machinelearning deeplearning deep-learning experiment-manager jupyter vscode
 Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
```

## Comparing `clearml_session-0.9.0.dist-info/RECORD` & `clearml_session-0.9.0rc0.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 clearml_session/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-clearml_session/__main__.py,sha256=PjO4ezhusxQoIsM7YUxpTrjuStOfJgB-q1xf_VJ39XQ,55382
+clearml_session/__main__.py,sha256=4YD3Wz8yy6l4K28kvKNkoXZpl648aToDs2E_9mkQv3E,55364
 clearml_session/interactive_session_task.py,sha256=TVchq2wSXFLAlQjmn5VGce4yfminb3wko-NTXkihC2U,39840
 clearml_session/single_thread_proxy.py,sha256=mOTRC0rca62C0EqhRkeXYEWbmDYwxBlE5_j_bMEb0nc,4781
 clearml_session/tcp_proxy.py,sha256=Oz6DNlbHtNRfhtSn3OYt_zNiasWZ_whHCk9KHIJr-2g,15948
-clearml_session/version.py,sha256=_DlwPNmTZTKflLiAF8YIqSr2ao66CTjj4bQtA6hz0jM,22
-clearml_session-0.9.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-clearml_session-0.9.0.dist-info/METADATA,sha256=_bmUNGvT42P_5_76fmMmWlW9S9ffmVVKPxOQhjPu0I4,18809
-clearml_session-0.9.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-clearml_session-0.9.0.dist-info/entry_points.txt,sha256=-KMe29157dlUO8Vd4z5kYkLHS2nInJZj52SHA0E9SsU,67
-clearml_session-0.9.0.dist-info/top_level.txt,sha256=Gt2u68qTEiXZqnHSKJR6CRlY799su4rlKW7Y3tM2RzY,16
-clearml_session-0.9.0.dist-info/RECORD,,
+clearml_session/version.py,sha256=P-esNjF-g0Lgd7aqiC3B822IXtdRR2ocOQN5Yur5Y1s,25
+clearml_session-0.9.0rc0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+clearml_session-0.9.0rc0.dist-info/METADATA,sha256=i4HTFTzW4le1yew2KYLoXGUuBRNWeqOiVDHw9vGKhyU,18812
+clearml_session-0.9.0rc0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+clearml_session-0.9.0rc0.dist-info/entry_points.txt,sha256=-KMe29157dlUO8Vd4z5kYkLHS2nInJZj52SHA0E9SsU,67
+clearml_session-0.9.0rc0.dist-info/top_level.txt,sha256=Gt2u68qTEiXZqnHSKJR6CRlY799su4rlKW7Y3tM2RzY,16
+clearml_session-0.9.0rc0.dist-info/RECORD,,
```

