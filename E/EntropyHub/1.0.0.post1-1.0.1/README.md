# Comparing `tmp/EntropyHub-1.0.0.post1.tar.gz` & `tmp/EntropyHub-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EntropyHub-1.0.0.post1.tar", last modified: Mon Mar 25 21:02:04 2024, max compression
+gzip compressed data, was "EntropyHub-1.0.1.tar", last modified: Sat Apr 20 00:20:35 2024, max compression
```

## Comparing `EntropyHub-1.0.0.post1.tar` & `EntropyHub-1.0.1.tar`

### file list

```diff
@@ -1,62 +1,60 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 21:02:04.513825 EntropyHub-1.0.0.post1/
-drwxrwxrwx   0        0        0        0 2024-03-25 21:02:04.497683 EntropyHub-1.0.0.post1/EntropyHub/
--rw-rw-rw-   0        0        0     3945 2024-01-07 01:04:32.000000 EntropyHub-1.0.0.post1/EntropyHub/_ApEn.py
--rw-rw-rw-   0        0        0     3849 2024-01-01 21:19:20.000000 EntropyHub-1.0.0.post1/EntropyHub/_AttnEn.py
--rw-rw-rw-   0        0        0     3465 2024-01-01 21:19:27.000000 EntropyHub-1.0.0.post1/EntropyHub/_BubbEn.py
--rw-rw-rw-   0        0        0     4281 2024-01-01 21:19:48.000000 EntropyHub-1.0.0.post1/EntropyHub/_CoSiEn.py
--rw-rw-rw-   0        0        0     4310 2024-01-01 21:19:42.000000 EntropyHub-1.0.0.post1/EntropyHub/_CondEn.py
--rw-rw-rw-   0        0        0     7211 2024-02-14 16:53:36.000000 EntropyHub-1.0.0.post1/EntropyHub/_DispEn.py
--rw-rw-rw-   0        0        0     7753 2024-03-19 01:45:42.000000 EntropyHub-1.0.0.post1/EntropyHub/_DispEn2D.py
--rw-rw-rw-   0        0        0     4786 2024-01-01 21:20:51.000000 EntropyHub-1.0.0.post1/EntropyHub/_DistEn.py
--rw-rw-rw-   0        0        0     7342 2024-01-01 21:20:58.000000 EntropyHub-1.0.0.post1/EntropyHub/_DistEn2D.py
--rw-rw-rw-   0        0        0     4378 2023-12-26 22:21:02.000000 EntropyHub-1.0.0.post1/EntropyHub/_DivEn.py
--rw-rw-rw-   0        0        0     3624 2024-01-01 21:21:39.000000 EntropyHub-1.0.0.post1/EntropyHub/_EnofEn.py
--rw-rw-rw-   0        0        0     5292 2024-01-01 21:21:46.000000 EntropyHub-1.0.0.post1/EntropyHub/_EspEn2D.py
--rw-rw-rw-   0        0        0     4568 2024-03-19 20:34:45.000000 EntropyHub-1.0.0.post1/EntropyHub/_ExampleData.py
--rw-rw-rw-   0        0        0    10280 2024-03-16 23:40:09.000000 EntropyHub-1.0.0.post1/EntropyHub/_FuzzEn.py
--rw-rw-rw-   0        0        0    11944 2024-03-19 19:41:05.000000 EntropyHub-1.0.0.post1/EntropyHub/_FuzzEn2D.py
--rw-rw-rw-   0        0        0    25799 2024-01-14 00:56:35.000000 EntropyHub-1.0.0.post1/EntropyHub/_GenEn.py
--rw-rw-rw-   0        0        0     5623 2024-01-01 21:22:42.000000 EntropyHub-1.0.0.post1/EntropyHub/_GridEn.py
--rw-rw-rw-   0        0        0     4075 2024-01-01 21:23:44.000000 EntropyHub-1.0.0.post1/EntropyHub/_IncrEn.py
--rw-rw-rw-   0        0        0     3444 2024-02-12 23:37:22.000000 EntropyHub-1.0.0.post1/EntropyHub/_K2En.py
--rw-rw-rw-   0        0        0    11077 2024-03-21 13:57:35.000000 EntropyHub-1.0.0.post1/EntropyHub/_MSEn.py
--rw-rw-rw-   0        0        0     7072 2024-01-01 21:24:34.000000 EntropyHub-1.0.0.post1/EntropyHub/_MSEn2D.py
--rw-rw-rw-   0        0        0     5147 2024-03-22 17:12:37.000000 EntropyHub-1.0.0.post1/EntropyHub/_MSobject.py
--rw-rw-rw-   0        0        0    13201 2023-12-26 22:49:28.000000 EntropyHub-1.0.0.post1/EntropyHub/_PermEn.py
--rw-rw-rw-   0        0        0     7587 2023-12-26 22:56:37.000000 EntropyHub-1.0.0.post1/EntropyHub/_PermEn2D.py
--rw-rw-rw-   0        0        0     4730 2024-01-01 21:25:25.000000 EntropyHub-1.0.0.post1/EntropyHub/_PhasEn.py
--rw-rw-rw-   0        0        0     5738 2023-12-27 00:58:42.000000 EntropyHub-1.0.0.post1/EntropyHub/_RangEn.py
--rw-rw-rw-   0        0        0     6107 2024-01-01 21:26:08.000000 EntropyHub-1.0.0.post1/EntropyHub/_SampEn.py
--rw-rw-rw-   0        0        0     7404 2024-01-01 21:26:15.000000 EntropyHub-1.0.0.post1/EntropyHub/_SampEn2D.py
--rw-rw-rw-   0        0        0     4108 2024-01-01 21:26:42.000000 EntropyHub-1.0.0.post1/EntropyHub/_SlopEn.py
--rw-rw-rw-   0        0        0     4529 2024-01-01 21:26:58.000000 EntropyHub-1.0.0.post1/EntropyHub/_SpecEn.py
--rw-rw-rw-   0        0        0     6120 2024-01-01 21:27:06.000000 EntropyHub-1.0.0.post1/EntropyHub/_SyDyEn.py
--rw-rw-rw-   0        0        0     2280 2024-01-01 21:33:23.000000 EntropyHub-1.0.0.post1/EntropyHub/_TranEn.py
--rw-rw-rw-   0        0        0     5541 2024-01-07 00:27:23.000000 EntropyHub-1.0.0.post1/EntropyHub/_XApEn.py
--rw-rw-rw-   0        0        0     5821 2024-01-07 17:34:30.000000 EntropyHub-1.0.0.post1/EntropyHub/_XCondEn.py
--rw-rw-rw-   0        0        0     6378 2024-01-07 18:04:42.000000 EntropyHub-1.0.0.post1/EntropyHub/_XDistEn.py
--rw-rw-rw-   0        0        0    11966 2024-03-19 19:41:33.000000 EntropyHub-1.0.0.post1/EntropyHub/_XFuzzEn.py
--rw-rw-rw-   0        0        0     4880 2024-01-07 18:50:39.000000 EntropyHub-1.0.0.post1/EntropyHub/_XK2En.py
--rw-rw-rw-   0        0        0    10546 2024-03-21 13:57:59.000000 EntropyHub-1.0.0.post1/EntropyHub/_XMSEn.py
--rw-rw-rw-   0        0        0     4404 2024-01-07 19:40:06.000000 EntropyHub-1.0.0.post1/EntropyHub/_XPermEn.py
--rw-rw-rw-   0        0        0     6547 2024-01-06 22:50:26.000000 EntropyHub-1.0.0.post1/EntropyHub/_XSampEn.py
--rw-rw-rw-   0        0        0     5202 2024-03-11 12:29:50.000000 EntropyHub-1.0.0.post1/EntropyHub/_XSpecEn.py
--rw-rw-rw-   0        0        0    14062 2024-03-21 14:42:57.000000 EntropyHub-1.0.0.post1/EntropyHub/__init__.py
--rw-rw-rw-   0        0        0     9959 2024-03-22 20:38:15.000000 EntropyHub-1.0.0.post1/EntropyHub/_cMSEn.py
--rw-rw-rw-   0        0        0    11157 2024-03-22 20:37:30.000000 EntropyHub-1.0.0.post1/EntropyHub/_cXMSEn.py
--rw-rw-rw-   0        0        0     9154 2024-03-21 13:59:16.000000 EntropyHub-1.0.0.post1/EntropyHub/_hMSEn.py
--rw-rw-rw-   0        0        0    10791 2024-03-21 13:57:47.000000 EntropyHub-1.0.0.post1/EntropyHub/_hXMSEn.py
--rw-rw-rw-   0        0        0     8313 2024-03-21 13:58:39.000000 EntropyHub-1.0.0.post1/EntropyHub/_rMSEn.py
--rw-rw-rw-   0        0        0     9180 2024-03-21 13:57:41.000000 EntropyHub-1.0.0.post1/EntropyHub/_rXMSEn.py
-drwxrwxrwx   0        0        0        0 2024-03-25 21:02:04.513825 EntropyHub-1.0.0.post1/EntropyHub.egg-info/
--rw-rw-rw-   0        0        0     9892 2024-03-25 21:02:04.000000 EntropyHub-1.0.0.post1/EntropyHub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1288 2024-03-25 21:02:04.000000 EntropyHub-1.0.0.post1/EntropyHub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-25 21:02:04.000000 EntropyHub-1.0.0.post1/EntropyHub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-03-25 21:02:04.000000 EntropyHub-1.0.0.post1/EntropyHub.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-25 21:02:04.000000 EntropyHub-1.0.0.post1/EntropyHub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11357 2023-01-21 18:52:09.000000 EntropyHub-1.0.0.post1/LICENSE.txt
--rw-rw-rw-   0        0        0      206 2023-01-21 18:52:09.000000 EntropyHub-1.0.0.post1/MANIFEST.in
--rw-rw-rw-   0        0        0     9892 2024-03-25 21:02:04.513825 EntropyHub-1.0.0.post1/PKG-INFO
--rw-rw-rw-   0        0        0     7922 2024-03-25 21:00:39.000000 EntropyHub-1.0.0.post1/README.md
--rw-rw-rw-   0        0        0       85 2024-03-25 21:02:04.516002 EntropyHub-1.0.0.post1/setup.cfg
--rw-rw-rw-   0        0        0    11057 2024-03-25 21:01:58.000000 EntropyHub-1.0.0.post1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 00:20:35.925696 EntropyHub-1.0.1/
+drwxrwxrwx   0        0        0        0 2024-04-20 00:20:35.895594 EntropyHub-1.0.1/EntropyHub/
+-rw-rw-rw-   0        0        0     3945 2024-01-07 01:04:32.000000 EntropyHub-1.0.1/EntropyHub/_ApEn.py
+-rw-rw-rw-   0        0        0     3849 2024-01-01 21:19:20.000000 EntropyHub-1.0.1/EntropyHub/_AttnEn.py
+-rw-rw-rw-   0        0        0     3465 2024-01-01 21:19:27.000000 EntropyHub-1.0.1/EntropyHub/_BubbEn.py
+-rw-rw-rw-   0        0        0     4286 2024-04-11 12:49:48.000000 EntropyHub-1.0.1/EntropyHub/_CoSiEn.py
+-rw-rw-rw-   0        0        0     4310 2024-01-01 21:19:42.000000 EntropyHub-1.0.1/EntropyHub/_CondEn.py
+-rw-rw-rw-   0        0        0     7211 2024-02-14 16:53:36.000000 EntropyHub-1.0.1/EntropyHub/_DispEn.py
+-rw-rw-rw-   0        0        0     7753 2024-03-19 01:45:42.000000 EntropyHub-1.0.1/EntropyHub/_DispEn2D.py
+-rw-rw-rw-   0        0        0     4786 2024-01-01 21:20:51.000000 EntropyHub-1.0.1/EntropyHub/_DistEn.py
+-rw-rw-rw-   0        0        0     7342 2024-01-01 21:20:58.000000 EntropyHub-1.0.1/EntropyHub/_DistEn2D.py
+-rw-rw-rw-   0        0        0     4378 2023-12-26 22:21:02.000000 EntropyHub-1.0.1/EntropyHub/_DivEn.py
+-rw-rw-rw-   0        0        0     3624 2024-01-01 21:21:39.000000 EntropyHub-1.0.1/EntropyHub/_EnofEn.py
+-rw-rw-rw-   0        0        0     5292 2024-01-01 21:21:46.000000 EntropyHub-1.0.1/EntropyHub/_EspEn2D.py
+-rw-rw-rw-   0        0        0     4568 2024-03-19 20:34:45.000000 EntropyHub-1.0.1/EntropyHub/_ExampleData.py
+-rw-rw-rw-   0        0        0    10292 2024-04-10 09:26:28.000000 EntropyHub-1.0.1/EntropyHub/_FuzzEn.py
+-rw-rw-rw-   0        0        0    11944 2024-03-19 19:41:05.000000 EntropyHub-1.0.1/EntropyHub/_FuzzEn2D.py
+-rw-rw-rw-   0        0        0     5623 2024-01-01 21:22:42.000000 EntropyHub-1.0.1/EntropyHub/_GridEn.py
+-rw-rw-rw-   0        0        0     4075 2024-01-01 21:23:44.000000 EntropyHub-1.0.1/EntropyHub/_IncrEn.py
+-rw-rw-rw-   0        0        0     3444 2024-02-12 23:37:22.000000 EntropyHub-1.0.1/EntropyHub/_K2En.py
+-rw-rw-rw-   0        0        0    11077 2024-03-21 13:57:35.000000 EntropyHub-1.0.1/EntropyHub/_MSEn.py
+-rw-rw-rw-   0        0        0     7072 2024-01-01 21:24:34.000000 EntropyHub-1.0.1/EntropyHub/_MSEn2D.py
+-rw-rw-rw-   0        0        0     5100 2024-04-12 12:06:16.000000 EntropyHub-1.0.1/EntropyHub/_MSobject.py
+-rw-rw-rw-   0        0        0    13201 2023-12-26 22:49:28.000000 EntropyHub-1.0.1/EntropyHub/_PermEn.py
+-rw-rw-rw-   0        0        0     7587 2023-12-26 22:56:37.000000 EntropyHub-1.0.1/EntropyHub/_PermEn2D.py
+-rw-rw-rw-   0        0        0     4730 2024-01-01 21:25:25.000000 EntropyHub-1.0.1/EntropyHub/_PhasEn.py
+-rw-rw-rw-   0        0        0     5738 2023-12-27 00:58:42.000000 EntropyHub-1.0.1/EntropyHub/_RangEn.py
+-rw-rw-rw-   0        0        0     6107 2024-01-01 21:26:08.000000 EntropyHub-1.0.1/EntropyHub/_SampEn.py
+-rw-rw-rw-   0        0        0     7404 2024-01-01 21:26:15.000000 EntropyHub-1.0.1/EntropyHub/_SampEn2D.py
+-rw-rw-rw-   0        0        0     4108 2024-01-01 21:26:42.000000 EntropyHub-1.0.1/EntropyHub/_SlopEn.py
+-rw-rw-rw-   0        0        0     4529 2024-01-01 21:26:58.000000 EntropyHub-1.0.1/EntropyHub/_SpecEn.py
+-rw-rw-rw-   0        0        0     6120 2024-01-01 21:27:06.000000 EntropyHub-1.0.1/EntropyHub/_SyDyEn.py
+-rw-rw-rw-   0        0        0     5541 2024-01-07 00:27:23.000000 EntropyHub-1.0.1/EntropyHub/_XApEn.py
+-rw-rw-rw-   0        0        0     5821 2024-01-07 17:34:30.000000 EntropyHub-1.0.1/EntropyHub/_XCondEn.py
+-rw-rw-rw-   0        0        0     6378 2024-01-07 18:04:42.000000 EntropyHub-1.0.1/EntropyHub/_XDistEn.py
+-rw-rw-rw-   0        0        0    11966 2024-03-19 19:41:33.000000 EntropyHub-1.0.1/EntropyHub/_XFuzzEn.py
+-rw-rw-rw-   0        0        0     4880 2024-01-07 18:50:39.000000 EntropyHub-1.0.1/EntropyHub/_XK2En.py
+-rw-rw-rw-   0        0        0    10546 2024-03-21 13:57:59.000000 EntropyHub-1.0.1/EntropyHub/_XMSEn.py
+-rw-rw-rw-   0        0        0     4404 2024-01-07 19:40:06.000000 EntropyHub-1.0.1/EntropyHub/_XPermEn.py
+-rw-rw-rw-   0        0        0     6547 2024-01-06 22:50:26.000000 EntropyHub-1.0.1/EntropyHub/_XSampEn.py
+-rw-rw-rw-   0        0        0     5202 2024-03-11 12:29:50.000000 EntropyHub-1.0.1/EntropyHub/_XSpecEn.py
+-rw-rw-rw-   0        0        0    14927 2024-04-19 23:50:20.000000 EntropyHub-1.0.1/EntropyHub/__init__.py
+-rw-rw-rw-   0        0        0     9959 2024-03-22 20:38:15.000000 EntropyHub-1.0.1/EntropyHub/_cMSEn.py
+-rw-rw-rw-   0        0        0    11157 2024-03-22 20:37:30.000000 EntropyHub-1.0.1/EntropyHub/_cXMSEn.py
+-rw-rw-rw-   0        0        0     9154 2024-03-21 13:59:16.000000 EntropyHub-1.0.1/EntropyHub/_hMSEn.py
+-rw-rw-rw-   0        0        0    10791 2024-03-21 13:57:47.000000 EntropyHub-1.0.1/EntropyHub/_hXMSEn.py
+-rw-rw-rw-   0        0        0     8313 2024-03-21 13:58:39.000000 EntropyHub-1.0.1/EntropyHub/_rMSEn.py
+-rw-rw-rw-   0        0        0     9180 2024-03-21 13:57:41.000000 EntropyHub-1.0.1/EntropyHub/_rXMSEn.py
+drwxrwxrwx   0        0        0        0 2024-04-20 00:20:35.925696 EntropyHub-1.0.1/EntropyHub.egg-info/
+-rw-rw-rw-   0        0        0     9886 2024-04-20 00:20:35.000000 EntropyHub-1.0.1/EntropyHub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1245 2024-04-20 00:20:35.000000 EntropyHub-1.0.1/EntropyHub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 00:20:35.000000 EntropyHub-1.0.1/EntropyHub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-20 00:20:35.000000 EntropyHub-1.0.1/EntropyHub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 00:20:35.000000 EntropyHub-1.0.1/EntropyHub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11357 2023-01-21 18:52:09.000000 EntropyHub-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      206 2023-01-21 18:52:09.000000 EntropyHub-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     9886 2024-04-20 00:20:35.925696 EntropyHub-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7922 2024-03-25 21:00:39.000000 EntropyHub-1.0.1/README.md
+-rw-rw-rw-   0        0        0       85 2024-04-20 00:20:35.925696 EntropyHub-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0    11130 2024-04-20 00:18:33.000000 EntropyHub-1.0.1/setup.py
```

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_ApEn.py` & `EntropyHub-1.0.1/EntropyHub/_ApEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_AttnEn.py` & `EntropyHub-1.0.1/EntropyHub/_AttnEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_BubbEn.py` & `EntropyHub-1.0.1/EntropyHub/_BubbEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_CoSiEn.py` & `EntropyHub-1.0.1/EntropyHub/_CoSiEn.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     AngDis = np.arccos(np.triu(Num/Den,1))/np.pi    
     if np.max(np.imag(AngDis)) < 10**-6:
         Bm = np.sum(np.triu(np.round(AngDis,6) < r,1))/(Nx*(Nx-1)/2)    
     else:
         Bm = np.sum(np.triu(np.real(AngDis) < r,1))/(Nx*(Nx-1)/2)
         print('Warning: Complex values ignored')
     if Bm == 1 or Bm == 0:
-        CoSi = 0
+        CoSi = np.NaN
     else:
         CoSi = -(Bm*np.log(Bm)/np.log(Logx)) - ((1-Bm)*np.log(1-Bm)/np.log(Logx))
 
     return CoSi, Bm
 
 """
     Copyright 2024 Matthew W. Flood, EntropyHub
```

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_CondEn.py` & `EntropyHub-1.0.1/EntropyHub/_CondEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_DispEn.py` & `EntropyHub-1.0.1/EntropyHub/_DispEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_DispEn2D.py` & `EntropyHub-1.0.1/EntropyHub/_DispEn2D.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_DistEn.py` & `EntropyHub-1.0.1/EntropyHub/_DistEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_DistEn2D.py` & `EntropyHub-1.0.1/EntropyHub/_DistEn2D.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_DivEn.py` & `EntropyHub-1.0.1/EntropyHub/_DivEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_EnofEn.py` & `EntropyHub-1.0.1/EntropyHub/_EnofEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_EspEn2D.py` & `EntropyHub-1.0.1/EntropyHub/_EspEn2D.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_ExampleData.py` & `EntropyHub-1.0.1/EntropyHub/_ExampleData.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_FuzzEn.py` & `EntropyHub-1.0.1/EntropyHub/_FuzzEn.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     """   
 
     Sig = np.squeeze(Sig)
     N = Sig.shape[0]    
     assert N>10 and Sig.ndim == 1, "Sig:   must be a numpy vector"
     assert isinstance(m,int) and (m > 0), "m:     must be an integer > 0"
     assert isinstance(tau,int) and (tau > 0), "tau:   must be an integer > 0"
-    assert isinstance(r,(int,float)) or ((r[0] >= 0) and len(r) ==2), "r:     must be 2 element tuple of positive values"
+    assert isinstance(r,(int,float)) or ((r[0] >= 0) and len(r) ==2), "r:     must be a scalar or 2 element tuple of positive values"
     assert Fx.lower() in ['default','sigmoid','modsampen','gudermannian',
                           'bell', 'gaussian', 'constgaussian', 'triangular' ,
                           'trapezoidal1', 'trapezoidal2', 'z_shaped'] \
             and isinstance(Fx,str), """Fx:    must be one of the following strings -
             'default', 'sigmoid', 'modsampen', 'gudermannian', 'bell', 'z_shaped',
             'triangular', 'trapezoidal1','trapezoidal2','gaussian','constgaussian'"""
     assert isinstance(Logx,(int,float)) and (Logx>0), "Logx:     must be a positive value"
```

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_FuzzEn2D.py` & `EntropyHub-1.0.1/EntropyHub/_FuzzEn2D.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_GridEn.py` & `EntropyHub-1.0.1/EntropyHub/_GridEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_IncrEn.py` & `EntropyHub-1.0.1/EntropyHub/_IncrEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_K2En.py` & `EntropyHub-1.0.1/EntropyHub/_K2En.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_MSEn.py` & `EntropyHub-1.0.1/EntropyHub/_MSEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_MSEn2D.py` & `EntropyHub-1.0.1/EntropyHub/_MSEn2D.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_MSobject.py` & `EntropyHub-1.0.1/EntropyHub/_MSobject.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,54 +51,54 @@
         :``'GridEn'``:    - Grid Distribution Entropy	
         :``'EnofEn'``:    - Entropy of Entropy	
         :``'AttnEn'``:    - Attention Entropy
         [``'DivEn'``]:    - Diversity Entropy
         [``'RangEn'``]:   - Range Entropy
         
     
-    
     :Cross Entropies:    
         :``'XApEn'``:     - Cross-Approximate Entropy
         :``'XSampEn'``:   - Cross-Sample Entropy
         :``'XFuzzEn'``:   - Cross-Fuzzy Entropy
         :``'XK2En'``:     - Cross-Kolmogorov Entropy
         :``'XPermEn'``:   - Cross-Permutation Entropy
         :``'XCondEn'``:   - Cross-Conditional Entropy (corrected)
         :``'XDistEn'``:   - Cross-Distribution Entropy
         :``'XSpecEn'``:   - Cross-Spectral Entropy
         
-        
-    :Bidimensional Entropies:    
-        :``'SampEn2D'``:   - Bidimensional Sample Entropy
-        :``'FuzzEn2D'``:   - Bidimensional Fuzzy Entropy
-        :``'DispEn2D'``:   - Bidimensional Dispersion Entropy
-        :``'DistEn2D'``:   - Bidimensional Distribution Entropy
-        :``'PermEn2D'``:   - Bidimensional Permutation Entropy
-        :``'EspEn2D'``:    - Bidimensional Espinosa Entropy
+     
+    :Multivariate Entropies:          
+        :``'MvSampEn'``:   - Multivariate Sample Entropy
+        :``'MvFuzzEn'``:   - Multivariate Fuzzy Entropy
+        :``'MvDispEn'``:   - Multivariate Dispersion Entropy
+        :``'MvCoSiEn'``:   - Multivariate Cosine Similarity Entropy
+        :``'MvPermEn'``:   - Multivariate Permutation Entropy   
+
     
     :See also:
-        ``MSEn``, ``cMSEn``, ``rMSEn``, ``hMSEn``, ``XMSEn``, ``rXMSEn``, ``cXMSEn``, ``hXMSEn``
-    
+        ``MSEn``, ``cMSEn``, ``rMSEn``, ``hMSEn``, ``XMSEn``, ``rXMSEn``, ``cXMSEn``, ``hXMSEn``    
     """
         
     Chk = ['_ApEn',   '_SampEn', '_FuzzEn', '_K2En',   '_PermEn', '_CondEn', 
            '_DistEn', '_DispEn', '_SyDyEn', '_IncrEn', '_CoSiEn', '_PhasEn', 
            '_SpecEn', '_SlopEn', '_GridEn', '_BubbEn', '_EnofEn', '_AttnEn',
-           '_XApEn', '_XSampEn', '_XFuzzEn', '_XPermEn', '_XCondEn',
-           '_XDistEn','_XSpecEn', '_XK2En', '_SampEn2D', '_FuzzEn2D', 
-           '_DispEn2D', '_DistEn2D', '_PermEn2D', '_EspEn2D', '_DivEn', '_RangEn']
+           '_DivEn', '_RangEn', 
+           '_XApEn', '_XSampEn', '_XFuzzEn', '_XPermEn', 
+           '_XCondEn', '_XDistEn','_XSpecEn', '_XK2En', 
+           '_MvSampEn', '_MvFuzzEn', '_MvDispEn', '_MvPermEn','_MvCoSiEn']
     
     assert ('_'+EnType) in Chk, "EnType:      must be a valid entropy function name. \
     See help(EntropyHub.MSobject) for more info."
                 
     class MS_Entropy:
         def __init__(self, EnType, X):
             # _temp = __import__(('_'+EnType), globals(), locals(), [EnType], 0)
-            _temp = __import__(('EntropyHub._'+EnType), fromlist=[EnType])
-            #_temp = __import__('_'+EnType)
+            
+            #_temp = __import__(('EntropyHub._'+EnType), fromlist=[EnType])
+            _temp = __import__('_'+EnType)
             
             self.Func = getattr(_temp,EnType) 
             self.Kwargs = X
     
     Mobj = MS_Entropy(EnType, kwargs)   
     return Mobj
```

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_PermEn.py` & `EntropyHub-1.0.1/EntropyHub/_PermEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_PermEn2D.py` & `EntropyHub-1.0.1/EntropyHub/_PermEn2D.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_PhasEn.py` & `EntropyHub-1.0.1/EntropyHub/_PhasEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_RangEn.py` & `EntropyHub-1.0.1/EntropyHub/_RangEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_SampEn.py` & `EntropyHub-1.0.1/EntropyHub/_SampEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_SampEn2D.py` & `EntropyHub-1.0.1/EntropyHub/_SampEn2D.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_SlopEn.py` & `EntropyHub-1.0.1/EntropyHub/_SlopEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_SpecEn.py` & `EntropyHub-1.0.1/EntropyHub/_SpecEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_SyDyEn.py` & `EntropyHub-1.0.1/EntropyHub/_SyDyEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_XApEn.py` & `EntropyHub-1.0.1/EntropyHub/_XApEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_XCondEn.py` & `EntropyHub-1.0.1/EntropyHub/_XCondEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_XDistEn.py` & `EntropyHub-1.0.1/EntropyHub/_XDistEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_XFuzzEn.py` & `EntropyHub-1.0.1/EntropyHub/_XFuzzEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_XK2En.py` & `EntropyHub-1.0.1/EntropyHub/_XK2En.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_XMSEn.py` & `EntropyHub-1.0.1/EntropyHub/_XMSEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_XPermEn.py` & `EntropyHub-1.0.1/EntropyHub/_XPermEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_XSampEn.py` & `EntropyHub-1.0.1/EntropyHub/_XSampEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_XSpecEn.py` & `EntropyHub-1.0.1/EntropyHub/_XSpecEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/__init__.py` & `EntropyHub-1.0.1/EntropyHub/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,28 +36,39 @@
 from EntropyHub._FuzzEn2D import FuzzEn2D
 from EntropyHub._DistEn2D import DistEn2D
 from EntropyHub._DispEn2D import DispEn2D
 from EntropyHub._EspEn2D import EspEn2D
 from EntropyHub._PermEn2D import PermEn2D
 
 
+from EntropyHub._MvSampEn import MvSampEn
+from EntropyHub._MvFuzzEn import MvFuzzEn
+from EntropyHub._MvCoSiEn import MvCoSiEn
+from EntropyHub._MvDispEn import MvDispEn
+from EntropyHub._MvPermEn import MvPermEn
+
+
 from EntropyHub._ExampleData import ExampleData
+from EntropyHub._WindowData import WindowData
 from EntropyHub._MSobject import MSobject
 
 
 from EntropyHub._MSEn import MSEn
 from EntropyHub._cMSEn import cMSEn
 from EntropyHub._rMSEn import rMSEn
 from EntropyHub._hMSEn import hMSEn
 
 from EntropyHub._XMSEn import XMSEn
 from EntropyHub._cXMSEn import cXMSEn
 from EntropyHub._rXMSEn import rXMSEn
 from EntropyHub._hXMSEn import hXMSEn
 
+from EntropyHub._MvMSEn import MvMSEn
+from EntropyHub._cMvMSEn import cMvMSEn
+
 # from EntropyHub._MSEn2D import MSEn2D
 
 
 def greet():
     print("""
     
     	 ___  _   _  _____  _____  ____  ____  _     _          
@@ -141,14 +152,23 @@
         _____________________________________________________|___________________
         Bidimensional Sample Entropy                         |	SampEn2D
         Bidimensional Fuzzy Entropy                          |	FuzzEn2D
         Bidimensional Distribution Entropy                   |	DistEn2D
         Bidimensional Dispersion Entropy                     |	DispEn2D
         Bidimensional Permutation Entropy                    |	PermEn2D
         Bidimensional Espinosa Entropy                       |	EspEn2D
+        
+        _________________________________________________________________________
+        Multivariate Entropies                               |	Function Name
+        _____________________________________________________|___________________
+        Multivariate Sample Entropy                          |	MvSampEn
+        Multivariate Fuzzy Entropy                           |	MvFuzzEn
+        Multivariate Cosine Similarity Entropy               |	MvCoSiEn
+        Multivariate Dispersion Entropy                      |	MvDispEn
+        Multivariate Permutation Entropy                     |	MvPermEn
         	
         _________________________________________________________________________
         Multiscale Entropy Functions                          | Function Name
         ______________________________________________________|__________________ 
         Multiscale Entropy Object                             |   MSobject
                                                               |
         Multiscale Entropy                                    |   MSEn
@@ -196,22 +216,30 @@
         Multiscale Cross-Approximate Entropy                  |	
         Multiscale Cross-Fuzzy Entropy                        |	MSobject
         Multiscale Cross-Permutation Entropy                  |	    +
         Multiscale Cross-Distribution Entropy                 |	XMSEn / cXMSEn
         Multiscale Cross-Kolmogorov Entropy                   |   rXMSEn / hXMSEn
         Multiscale Cross-Conditional Entropy                  |	
         
-
+        _________________________________________________________________________
+        Multivariate Multiscale Entropies                     |	Function Name
+        ______________________________________________________|__________________
+        Multivariate Multiscale Sample Entropy                |	
+        Multivariate Multiscale Fuzzy Entropy                 |	MSobject
+        Multivariate Multiscale Dispersion Entropy            |	    +
+        Multivariate Multiscale Permutation Entropy           |	MvMSEn / cMvMSEn
+        Multivariate Multiscale Cosine Similarity Entropy     |	
+        
         
         
         This package is open for use by all in accordance with the terms of the 
         attached License agreement. Any scientific outputs obtained using 
         EntropyHub are required to include the following citation:
         
-          Matthew W. Flood and Bernd Grimm, 
+          Matthew W. Flood, 
           "EntropyHub: An open-source toolkit for entropic time series analysis",
           2021, https://github.com/MattWillFlood/EntropyHub
         
           © Copyright 2024 Matthew W. Flood, EntropyHub
         
           Licensed under the Apache License, Version 2.0 (the "License");
           you may not use this file except in compliance with the License.
@@ -241,25 +269,8 @@
         # Multiscale Bidimensional-Entropies                    |	Function Name
         # ______________________________________________________|__________________
         # Multiscale Bidimensional Sample Entropy               |	
         # Multiscale Bidimensional Fuzzy Entropy                |	
         # Multiscale Bidimensional Distribution Entropy         |	MSobject
         # Multiscale Bidimensional Dispersion Entropy           |	    +
         # Multiscale Bidimensional Permutation Entropy          |	 MSEn2D
-        # Multiscale Bidimensional Espinosa Entropy             |	
-        
-        
-        
-        
-# __all__ =  ["ApEn", "SampEn", "FuzzEn", "K2En", "PermEn", "CondEn", "DivEn",
-#             "DistEn", "DispEn", "SyDyEn", "IncrEn", "CoSiEn", "PhasEn", 
-#             "SpecEn", "SlopEn", "GridEn", "BubbEn", "EnofEn", "AttnEn", "RangEn",
-           
-#             "XApEn",   "XSampEn", "XFuzzEn", "XPermEn", 
-#             "XDistEn", "XSpecEn", "XK2En", "XCondEn",
-                      
-#             "SampEn2D",  "DistEn2D", "FuzzEn2D", "DispEn2D",
-                                
-#             "MSobject", "ExampleData",
-            
-#             "MSEn", "cMSEn", "rMSEn", "hMSEn",
-#             "XMSEn",  "cXMSEn",  "rXMSEn",  "hXMSEn"] 
+        # Multiscale Bidimensional Espinosa Entropy             |
```

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_cMSEn.py` & `EntropyHub-1.0.1/EntropyHub/_cMSEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_cXMSEn.py` & `EntropyHub-1.0.1/EntropyHub/_cXMSEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_hMSEn.py` & `EntropyHub-1.0.1/EntropyHub/_hMSEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_hXMSEn.py` & `EntropyHub-1.0.1/EntropyHub/_hXMSEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_rMSEn.py` & `EntropyHub-1.0.1/EntropyHub/_rMSEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub/_rXMSEn.py` & `EntropyHub-1.0.1/EntropyHub/_rXMSEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/EntropyHub.egg-info/PKG-INFO` & `EntropyHub-1.0.1/EntropyHub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EntropyHub
-Version: 1.0.0.post1
+Version: 1.0.1
 Summary: An open-source toolkit for entropic time series analysis.
 Home-page: https://www.EntropyHub.xyz
 Author: Matthew W. Flood
 Author-email: info@entropyhub.xyz, help@entropyhub.xyz
 License: Apache 2.0
 Project-URL: Contact, https://www.entropyhub.xyz/#contact
 Project-URL: Examples, https://www.entropyhub.xyz/python/pyexamples.html
```

### Comparing `EntropyHub-1.0.0.post1/EntropyHub.egg-info/SOURCES.txt` & `EntropyHub-1.0.1/EntropyHub.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 EntropyHub/_DistEn2D.py
 EntropyHub/_DivEn.py
 EntropyHub/_EnofEn.py
 EntropyHub/_EspEn2D.py
 EntropyHub/_ExampleData.py
 EntropyHub/_FuzzEn.py
 EntropyHub/_FuzzEn2D.py
-EntropyHub/_GenEn.py
 EntropyHub/_GridEn.py
 EntropyHub/_IncrEn.py
 EntropyHub/_K2En.py
 EntropyHub/_MSEn.py
 EntropyHub/_MSEn2D.py
 EntropyHub/_MSobject.py
 EntropyHub/_PermEn.py
@@ -30,15 +29,14 @@
 EntropyHub/_PhasEn.py
 EntropyHub/_RangEn.py
 EntropyHub/_SampEn.py
 EntropyHub/_SampEn2D.py
 EntropyHub/_SlopEn.py
 EntropyHub/_SpecEn.py
 EntropyHub/_SyDyEn.py
-EntropyHub/_TranEn.py
 EntropyHub/_XApEn.py
 EntropyHub/_XCondEn.py
 EntropyHub/_XDistEn.py
 EntropyHub/_XFuzzEn.py
 EntropyHub/_XK2En.py
 EntropyHub/_XMSEn.py
 EntropyHub/_XPermEn.py
```

### Comparing `EntropyHub-1.0.0.post1/LICENSE.txt` & `EntropyHub-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/PKG-INFO` & `EntropyHub-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EntropyHub
-Version: 1.0.0.post1
+Version: 1.0.1
 Summary: An open-source toolkit for entropic time series analysis.
 Home-page: https://www.EntropyHub.xyz
 Author: Matthew W. Flood
 Author-email: info@entropyhub.xyz, help@entropyhub.xyz
 License: Apache 2.0
 Project-URL: Contact, https://www.entropyhub.xyz/#contact
 Project-URL: Examples, https://www.entropyhub.xyz/python/pyexamples.html
```

### Comparing `EntropyHub-1.0.0.post1/README.md` & `EntropyHub-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.0.post1/setup.py` & `EntropyHub-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,23 +137,23 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
 For Terms of Use see https://github.com/MattWillFlood/EntropyHub
 """
 
-from setuptools import setup #find_packages
+from setuptools import setup, find_packages
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_desc = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='EntropyHub',  # Required
-    version='1.0.0.post1',  # Required
+    version='1.0.1',  # Required
     description='An open-source toolkit for entropic time series analysis.',  # Optional
     long_description=long_desc,  # Optional
     long_description_content_type='text/markdown',  # Optional (see note above)
 
     url='https://www.EntropyHub.xyz',  # Optional
     author='Matthew W. Flood',  # Optional
     author_email='info@entropyhub.xyz, help@entropyhub.xyz',  # Optional
@@ -181,16 +181,16 @@
     keywords=('entropy, nonlinear, time series, statistics, physics, mathematics, signal processing,'
                 'statistical physics, entropic, toolkit, research, multiscale, regularity, periodic,'
                 'sample entropy, approximate entropy, fuzzy entropy, permutation entropy, uncertainty,'
                 'dispersion entropy, kolmogorov, conditional entropy, composite, refined,'
                 'randomness, random, signal analysis, nonlinearity, julia, matlab, open-source,'
                 'refined-composite, hierarchical entropy, information theory, shannon entropy, complexity'),  # Optional
 
-    
-    packages = ['EntropyHub'], #find_packages(include ='EntropyHub*'),  # Required
+    packages = find_packages("EntropyHub", exclude=["__pycache__",".spyproject"]),
+    #packages = ['EntropyHub'], #find_packages(include ='EntropyHub*'),  # Required
     python_requires='>=3.6, <4',
     install_requires=['numpy', 'matplotlib', 'scipy', 'EMD-signal', 'requests'],  #'itertools', 'copy', #wheel?  Optional
 
 
     project_urls={  # Optional
         'Contact': 'https://www.entropyhub.xyz/#contact',
         'Examples': 'https://www.entropyhub.xyz/python/pyexamples.html',
```

