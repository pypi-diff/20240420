# Comparing `tmp/featransform-0.9.15-py3-none-any.whl.zip` & `tmp/featransform-0.9.16-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -8,13 +8,13 @@
 -rw-rw-rw-  2.0 fat     3388 b- defN 24-Apr-07 17:39 featransform/feature_engineering/clustering.py
 -rw-rw-rw-  2.0 fat     4042 b- defN 24-Apr-07 17:39 featransform/feature_engineering/dimensionality.py
 -rw-rw-rw-  2.0 fat        2 b- defN 24-Apr-01 18:31 featransform/optimizer/__init__.py
 -rw-rw-rw-  2.0 fat    11425 b- defN 24-Apr-07 17:40 featransform/optimizer/evaluator.py
 -rw-rw-rw-  2.0 fat     5277 b- defN 24-Apr-07 17:40 featransform/optimizer/selector.py
 -rw-rw-rw-  2.0 fat        2 b- defN 24-Apr-01 18:31 featransform/processing/__init__.py
 -rw-rw-rw-  2.0 fat     3512 b- defN 24-Apr-01 20:48 featransform/processing/processor.py
--rw-rw-rw-  2.0 fat     1090 b- defN 24-Apr-07 17:54 featransform-0.9.15.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     7198 b- defN 24-Apr-07 17:54 featransform-0.9.15.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-07 17:54 featransform-0.9.15.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-07 17:54 featransform-0.9.15.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1617 b- defN 24-Apr-07 17:54 featransform-0.9.15.dist-info/RECORD
-18 files, 54729 bytes uncompressed, 15875 bytes compressed:  71.0%
+-rw-rw-rw-  2.0 fat     1090 b- defN 24-Apr-19 22:15 featransform-0.9.16.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     7196 b- defN 24-Apr-19 22:15 featransform-0.9.16.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-19 22:15 featransform-0.9.16.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-19 22:15 featransform-0.9.16.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1617 b- defN 24-Apr-19 22:15 featransform-0.9.16.dist-info/RECORD
+18 files, 54727 bytes uncompressed, 15875 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: featransform/processing/__init__.py
 Comment: 
 
 Filename: featransform/processing/processor.py
 Comment: 
 
-Filename: featransform-0.9.15.dist-info/LICENSE
+Filename: featransform-0.9.16.dist-info/LICENSE
 Comment: 
 
-Filename: featransform-0.9.15.dist-info/METADATA
+Filename: featransform-0.9.16.dist-info/METADATA
 Comment: 
 
-Filename: featransform-0.9.15.dist-info/WHEEL
+Filename: featransform-0.9.16.dist-info/WHEEL
 Comment: 
 
-Filename: featransform-0.9.15.dist-info/top_level.txt
+Filename: featransform-0.9.16.dist-info/top_level.txt
 Comment: 
 
-Filename: featransform-0.9.15.dist-info/RECORD
+Filename: featransform-0.9.16.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `featransform-0.9.15.dist-info/LICENSE` & `featransform-0.9.16.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `featransform-0.9.15.dist-info/METADATA` & `featransform-0.9.16.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featransform
-Version: 0.9.15
+Version: 0.9.16
 Summary: Featransform is an automated feature engineering framework for supervised machine learning
 Home-page: https://github.com/TsLu1s/Featransform
 Author: Luís Santos
 Author-email: luisf_ssantos@hotmail.com
 License: MIT
 Keywords: data science,machine learning,data processing,feature engineering,feature selection,feature construction,feature optimization,automated feature engineering,automated machine learning,predictive modeling
 Classifier: Intended Audience :: Education
@@ -123,16 +123,16 @@
                   configs = configs)
 
 ft.fit_engineering(X = train,              # X:pd.DataFrame, target:str="Target_Column"
                    target = "Target_Column_Name")
 
 ## Transform Data 
 
-train = atl.transform(X=train)
-test = atl.transform(X=test)
+train = ft.transform(X=train)
+test = ft.transform(X=test)
 
 # Export Featransform Metadata
 
 import pickle
 output = open("ft_eng.pkl", 'wb')
 pickle.dump(ft, output)
```

## Comparing `featransform-0.9.15.dist-info/RECORD` & `featransform-0.9.16.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -7,12 +7,12 @@
 featransform/feature_engineering/clustering.py,sha256=Ypkdh__1eMk1uIOungD3qM1ozHFsaZIBxEV8aRK_bYs,3388
 featransform/feature_engineering/dimensionality.py,sha256=ZQBSHppc43BmQJyS3duyHaFTiiSW057cQxnM87aamFM,4042
 featransform/optimizer/__init__.py,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
 featransform/optimizer/evaluator.py,sha256=lsj3pEexLig0XXmjJClsiUfu-n-4e2kflsyhA5W29dA,11425
 featransform/optimizer/selector.py,sha256=Zf8OccuTg1qe070letEn3GmJDawUzJLRIXCCSO5yOeI,5277
 featransform/processing/__init__.py,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
 featransform/processing/processor.py,sha256=_eVGVNOF3RiJEabRwrq3G1AxY0c21MAleYdtaw3xGT4,3512
-featransform-0.9.15.dist-info/LICENSE,sha256=VMXkEvDFBFiT1owkPDp8dUVbidhkemgBSzG9qsUhs54,1090
-featransform-0.9.15.dist-info/METADATA,sha256=R0WnqfKopde_CfdWxecpiFAz-bq5Dlrb01KrhFG-s_E,7198
-featransform-0.9.15.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-featransform-0.9.15.dist-info/top_level.txt,sha256=nGf-wp6SDVDIawemhMuwByTbpGahhv92kQ1dQbRdYwo,13
-featransform-0.9.15.dist-info/RECORD,,
+featransform-0.9.16.dist-info/LICENSE,sha256=VMXkEvDFBFiT1owkPDp8dUVbidhkemgBSzG9qsUhs54,1090
+featransform-0.9.16.dist-info/METADATA,sha256=6V63AuY2rYgsXfkXwwPvUZg0VNiz85PkYc7wa-fbiH4,7196
+featransform-0.9.16.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+featransform-0.9.16.dist-info/top_level.txt,sha256=nGf-wp6SDVDIawemhMuwByTbpGahhv92kQ1dQbRdYwo,13
+featransform-0.9.16.dist-info/RECORD,,
```

