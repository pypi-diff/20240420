# Comparing `tmp/mlrun_pipelines_kfp_v2_experiment-0.1.0-py3-none-any.whl.zip` & `tmp/mlrun_pipelines_kfp_v2_experiment-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11977 bytes, number of entries: 11
+Zip file size: 11975 bytes, number of entries: 11
 -rw-r--r--  2.0 unx      871 b- defN 24-Apr-17 22:01 mlrun_pipelines/helpers.py
 -rw-r--r--  2.0 unx     3216 b- defN 24-Apr-18 14:15 mlrun_pipelines/mixins.py
 -rw-r--r--  2.0 unx     3207 b- defN 24-Apr-17 22:18 mlrun_pipelines/models.py
 -rw-r--r--  2.0 unx     9499 b- defN 24-Apr-17 22:01 mlrun_pipelines/mounts.py
 -rw-r--r--  2.0 unx    11415 b- defN 24-Apr-17 22:01 mlrun_pipelines/ops.py
 -rw-r--r--  2.0 unx      571 b- defN 24-Apr-17 22:01 mlrun_pipelines/patcher.py
 -rw-r--r--  2.0 unx      829 b- defN 24-Apr-17 22:16 mlrun_pipelines/utils.py
--rw-r--r--  2.0 unx      357 b- defN 24-Apr-18 22:59 mlrun_pipelines_kfp_v2_experiment-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 22:59 mlrun_pipelines_kfp_v2_experiment-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 24-Apr-18 22:59 mlrun_pipelines_kfp_v2_experiment-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      971 b- defN 24-Apr-18 22:59 mlrun_pipelines_kfp_v2_experiment-0.1.0.dist-info/RECORD
-11 files, 31044 bytes uncompressed, 10309 bytes compressed:  66.8%
+-rw-r--r--  2.0 unx      359 b- defN 24-Apr-20 13:13 mlrun_pipelines_kfp_v2_experiment-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-20 13:13 mlrun_pipelines_kfp_v2_experiment-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-20 13:13 mlrun_pipelines_kfp_v2_experiment-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      971 b- defN 24-Apr-20 13:13 mlrun_pipelines_kfp_v2_experiment-0.1.1.dist-info/RECORD
+11 files, 31046 bytes uncompressed, 10307 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: mlrun_pipelines/patcher.py
 Comment: 
 
 Filename: mlrun_pipelines/utils.py
 Comment: 
 
-Filename: mlrun_pipelines_kfp_v2_experiment-0.1.0.dist-info/METADATA
+Filename: mlrun_pipelines_kfp_v2_experiment-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: mlrun_pipelines_kfp_v2_experiment-0.1.0.dist-info/WHEEL
+Filename: mlrun_pipelines_kfp_v2_experiment-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: mlrun_pipelines_kfp_v2_experiment-0.1.0.dist-info/top_level.txt
+Filename: mlrun_pipelines_kfp_v2_experiment-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: mlrun_pipelines_kfp_v2_experiment-0.1.0.dist-info/RECORD
+Filename: mlrun_pipelines_kfp_v2_experiment-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `mlrun_pipelines_kfp_v2_experiment-0.1.0.dist-info/RECORD` & `mlrun_pipelines_kfp_v2_experiment-0.1.1.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 mlrun_pipelines/helpers.py,sha256=DQujoI5DseRtC82WxDIFWIOhkVJSvNlRdlxnja-izus,871
 mlrun_pipelines/mixins.py,sha256=Sy5_z4t-t4UP9yCBSDBwXPxeS0VTdwBXG242Bon8jFU,3216
 mlrun_pipelines/models.py,sha256=3-zBM2wpJilvFCgAypXDBbn0EFul6pqMRtDoxlOGtzo,3207
 mlrun_pipelines/mounts.py,sha256=kAdS5jr87T1cZciRFS85VUCsHyflbvBM8X1Ufw32Xio,9499
 mlrun_pipelines/ops.py,sha256=-8wLiSMGg_fKINn_yWLCrtCKIZXw0hsZ1Rjk_NPBTyI,11415
 mlrun_pipelines/patcher.py,sha256=sOBwPJ0KuM6LMolYEwR4tPiJhlgFsla5_0gIdyxONlw,571
 mlrun_pipelines/utils.py,sha256=fAPSIvo5aIT7ixyZV_ncRnKSQf2M5hGCqbgv4Gzs9zA,829
-mlrun_pipelines_kfp_v2_experiment-0.1.0.dist-info/METADATA,sha256=2cjBm919aH7aIwGV05lYc8ZuX6omVyZV7tVGBxJtufc,357
-mlrun_pipelines_kfp_v2_experiment-0.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-mlrun_pipelines_kfp_v2_experiment-0.1.0.dist-info/top_level.txt,sha256=nLog7d6Z7sH90lLPiJHgM1Q2hqwiKlkc8MtKtltFJvE,16
-mlrun_pipelines_kfp_v2_experiment-0.1.0.dist-info/RECORD,,
+mlrun_pipelines_kfp_v2_experiment-0.1.1.dist-info/METADATA,sha256=GvyNESrd9RiSowUXI7iBjj5x3JYvZcNkHkvlCEl2-as,359
+mlrun_pipelines_kfp_v2_experiment-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+mlrun_pipelines_kfp_v2_experiment-0.1.1.dist-info/top_level.txt,sha256=nLog7d6Z7sH90lLPiJHgM1Q2hqwiKlkc8MtKtltFJvE,16
+mlrun_pipelines_kfp_v2_experiment-0.1.1.dist-info/RECORD,,
```

