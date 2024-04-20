# Comparing `tmp/fotolab-0.9.0.tar.gz` & `tmp/fotolab-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fotolab-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fotolab-0.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fotolab-0.9.0.tar` & `fotolab-0.9.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      254 2024-01-15 16:49:11.109740 fotolab-0.9.0/.coveragerc
--rw-r--r--   0        0        0     3108 2023-12-27 09:44:17.383635 fotolab-0.9.0/.gitignore
--rw-r--r--   0        0        0     2818 2024-03-16 13:10:19.685329 fotolab-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       36 2024-02-29 15:57:08.436831 fotolab-0.9.0/.python-version
--rw-r--r--   0        0        0     2298 2024-03-17 07:09:23.192556 fotolab-0.9.0/CHANGELOG.md
--rw-r--r--   0        0        0     2899 2023-12-27 09:44:17.387635 fotolab-0.9.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    31956 2023-12-27 09:44:17.387635 fotolab-0.9.0/LICENSE.md
--rw-r--r--   0        0        0      565 2024-01-26 04:35:27.179138 fotolab-0.9.0/Pipfile
--rw-r--r--   0        0        0    63778 2024-03-14 15:53:17.651731 fotolab-0.9.0/Pipfile.lock
--rw-r--r--   0        0        0     5714 2024-03-12 14:49:29.463459 fotolab-0.9.0/README.md
--rw-r--r--   0        0        0      638 2024-01-02 16:40:12.610377 fotolab-0.9.0/docs/Makefile
--rw-r--r--   0        0        0      804 2024-01-02 16:40:12.610377 fotolab-0.9.0/docs/make.bat
-lrwxr-xr-x   0        0        0        0 2024-01-02 16:46:44.751562 fotolab-0.9.0/docs/source/CHANGELOG.md -> ../../CHANGELOG.md
-lrwxr-xr-x   0        0        0        0 2024-01-02 16:46:59.296873 fotolab-0.9.0/docs/source/CONTRIBUTING.md -> ../../CONTRIBUTING.md
-lrwxr-xr-x   0        0        0        0 2024-01-02 16:47:13.823329 fotolab-0.9.0/docs/source/LICENSE.md -> ../../LICENSE.md
-lrwxr-xr-x   0        0        0        0 2024-01-02 16:47:22.670019 fotolab-0.9.0/docs/source/README.md -> ../../README.md
--rw-r--r--   0        0        0    11658 2024-01-02 16:54:08.403595 fotolab-0.9.0/docs/source/_static/logo.jpg
--rw-r--r--   0        0        0     1523 2024-01-02 16:46:16.884655 fotolab-0.9.0/docs/source/conf.py
--rw-r--r--   0        0        0      172 2024-01-02 16:43:22.508047 fotolab-0.9.0/docs/source/index.rst
--rw-r--r--   0        0        0     1237 2024-03-17 07:09:34.652704 fotolab-0.9.0/fotolab/__init__.py
--rw-r--r--   0        0        0      833 2023-12-27 09:44:17.387635 fotolab-0.9.0/fotolab/__main__.py
--rw-r--r--   0        0        0     2142 2024-03-06 15:12:47.696706 fotolab-0.9.0/fotolab/auto.py
--rw-r--r--   0        0        0     3776 2024-03-01 20:30:00.532561 fotolab-0.9.0/fotolab/border.py
--rw-r--r--   0        0        0     4433 2024-03-15 14:55:53.440620 fotolab-0.9.0/fotolab/cli.py
--rw-r--r--   0        0        0     2350 2024-03-07 15:41:56.161154 fotolab-0.9.0/fotolab/contrast.py
--rw-r--r--   0        0        0     1400 2024-02-09 15:59:22.122310 fotolab-0.9.0/fotolab/env.py
--rw-r--r--   0        0        0     2505 2024-02-16 15:53:13.149377 fotolab-0.9.0/fotolab/resize.py
--rw-r--r--   0        0        0     2902 2024-03-07 15:42:07.245330 fotolab-0.9.0/fotolab/sharpen.py
--rw-r--r--   0        0        0     5031 2024-03-07 15:42:20.005541 fotolab-0.9.0/fotolab/watermark.py
--rw-r--r--   0        0        0     1073 2023-12-27 09:44:17.391635 fotolab-0.9.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-27 09:44:17.391635 fotolab-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0      940 2023-12-27 09:44:17.391635 fotolab-0.9.0/tests/conftest.py
--rw-r--r--   0        0        0      251 2024-01-10 16:35:46.973153 fotolab-0.9.0/tests/test_env.py
--rw-r--r--   0        0        0      239 2024-01-15 15:25:08.902134 fotolab-0.9.0/tests/test_help_flag.py
--rw-r--r--   0        0        0      216 2024-01-15 15:26:46.165639 fotolab-0.9.0/tests/test_quiet_flag.py
--rw-r--r--   0        0        0      658 2023-12-27 09:44:17.391635 fotolab-0.9.0/tox.ini
--rw-r--r--   0        0        0     6688 1970-01-01 00:00:00.000000 fotolab-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      254 2024-01-15 16:49:11.109740 fotolab-0.9.1/.coveragerc
+-rw-r--r--   0        0        0     3108 2023-12-27 09:44:17.383635 fotolab-0.9.1/.gitignore
+-rw-r--r--   0        0        0     2818 2024-03-16 13:10:19.685329 fotolab-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       36 2024-02-29 15:57:08.436831 fotolab-0.9.1/.python-version
+-rw-r--r--   0        0        0     2518 2024-03-23 17:50:09.932726 fotolab-0.9.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2899 2023-12-27 09:44:17.387635 fotolab-0.9.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    31956 2023-12-27 09:44:17.387635 fotolab-0.9.1/LICENSE.md
+-rw-r--r--   0        0        0      565 2024-01-26 04:35:27.179138 fotolab-0.9.1/Pipfile
+-rw-r--r--   0        0        0    64788 2024-03-22 15:51:53.430868 fotolab-0.9.1/Pipfile.lock
+-rw-r--r--   0        0        0     5714 2024-03-12 14:49:29.463459 fotolab-0.9.1/README.md
+-rw-r--r--   0        0        0      638 2024-01-02 16:40:12.610377 fotolab-0.9.1/docs/Makefile
+-rw-r--r--   0        0        0      804 2024-01-02 16:40:12.610377 fotolab-0.9.1/docs/make.bat
+lrwxr-xr-x   0        0        0        0 2024-01-02 16:46:44.751562 fotolab-0.9.1/docs/source/CHANGELOG.md -> ../../CHANGELOG.md
+lrwxr-xr-x   0        0        0        0 2024-01-02 16:46:59.296873 fotolab-0.9.1/docs/source/CONTRIBUTING.md -> ../../CONTRIBUTING.md
+lrwxr-xr-x   0        0        0        0 2024-01-02 16:47:13.823329 fotolab-0.9.1/docs/source/LICENSE.md -> ../../LICENSE.md
+lrwxr-xr-x   0        0        0        0 2024-01-02 16:47:22.670019 fotolab-0.9.1/docs/source/README.md -> ../../README.md
+-rw-r--r--   0        0        0    11658 2024-01-02 16:54:08.403595 fotolab-0.9.1/docs/source/_static/logo.jpg
+-rw-r--r--   0        0        0     1523 2024-01-02 16:46:16.884655 fotolab-0.9.1/docs/source/conf.py
+-rw-r--r--   0        0        0      172 2024-01-02 16:43:22.508047 fotolab-0.9.1/docs/source/index.rst
+-rw-r--r--   0        0        0     2015 2024-03-23 17:50:38.401354 fotolab-0.9.1/fotolab/__init__.py
+-rw-r--r--   0        0        0      833 2023-12-27 09:44:17.387635 fotolab-0.9.1/fotolab/__main__.py
+-rw-r--r--   0        0        0     2173 2024-03-22 16:30:35.020584 fotolab-0.9.1/fotolab/auto.py
+-rw-r--r--   0        0        0     3413 2024-03-23 17:31:54.231733 fotolab-0.9.1/fotolab/border.py
+-rw-r--r--   0        0        0     4433 2024-03-22 16:19:54.437661 fotolab-0.9.1/fotolab/cli.py
+-rw-r--r--   0        0        0     1969 2024-03-23 17:16:48.616109 fotolab-0.9.1/fotolab/contrast.py
+-rw-r--r--   0        0        0     1449 2024-03-19 16:18:43.365937 fotolab-0.9.1/fotolab/env.py
+-rw-r--r--   0        0        0     2128 2024-03-23 17:16:45.748077 fotolab-0.9.1/fotolab/resize.py
+-rw-r--r--   0        0        0     2535 2024-03-23 17:16:46.364084 fotolab-0.9.1/fotolab/sharpen.py
+-rw-r--r--   0        0        0     4648 2024-03-23 17:16:46.908090 fotolab-0.9.1/fotolab/watermark.py
+-rw-r--r--   0        0        0     1073 2023-12-27 09:44:17.391635 fotolab-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-27 09:44:17.391635 fotolab-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0      940 2023-12-27 09:44:17.391635 fotolab-0.9.1/tests/conftest.py
+-rw-r--r--   0        0        0      251 2024-01-10 16:35:46.973153 fotolab-0.9.1/tests/test_env.py
+-rw-r--r--   0        0        0      239 2024-01-15 15:25:08.902134 fotolab-0.9.1/tests/test_help_flag.py
+-rw-r--r--   0        0        0      216 2024-01-15 15:26:46.165639 fotolab-0.9.1/tests/test_quiet_flag.py
+-rw-r--r--   0        0        0      658 2023-12-27 09:44:17.391635 fotolab-0.9.1/tox.ini
+-rw-r--r--   0        0        0     6688 1970-01-01 00:00:00.000000 fotolab-0.9.1/PKG-INFO
```

### Comparing `fotolab-0.9.0/.gitignore` & `fotolab-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fotolab-0.9.0/.pre-commit-config.yaml` & `fotolab-0.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fotolab-0.9.0/CHANGELOG.md` & `fotolab-0.9.1/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,25 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [0-based versioning](https://0ver.org/).
 
 ## [Unreleased]
 
+## v0.9.1 (2024-03-24)
+
+### Changed
+
+- Implement open image using the default program
+- Refactor all subcommand to use `save_image` global helper function
+
+### Fixed
+
+- Fix newline in `sys.version` output in Python 3.8
+
 ## v0.9.0 (2024-03-17)
 
 ### Added
 
 - Add `-op` or `--open` flag to open the image using default program
 
 ### Changed
```

### Comparing `fotolab-0.9.0/CONTRIBUTING.md` & `fotolab-0.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fotolab-0.9.0/LICENSE.md` & `fotolab-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fotolab-0.9.0/Pipfile` & `fotolab-0.9.1/Pipfile`

 * *Files identical despite different names*

### Comparing `fotolab-0.9.0/Pipfile.lock` & `fotolab-0.9.1/Pipfile.lock`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9793006752432155%*

 * *Differences: {"'develop'": "{'coverage': {'hashes': "*

 * *              "['sha256:00838a35b882694afda09f85e469c96367daa3f3f2b097d846a7216993d37f4c', "*

 * *              "'sha256:0513b9508b93da4e1716744ef6ebc507aff016ba115ffe8ecff744d1322a7b63', "*

 * *              "'sha256:09c3255458533cb76ef55da8cc49ffab9e33f083739c8bd4f58e79fecfe288f7', "*

 * *              "'sha256:09ef9199ed6653989ebbcaacc9b62b514bb63ea2f90256e71fea3ed74bd8ff6f', "*

 * *              "'sha256:09fa497a8ab37784fbb20ab699c246053ac294d13fc7eb40ec007a5043ec91f8', "*

 * *           […]*

```diff
@@ -110,69 +110,69 @@
             "version": "==3.4.0"
         },
         "coverage": {
             "extras": [
                 "toml"
             ],
             "hashes": [
-                "sha256:0209a6369ccce576b43bb227dc8322d8ef9e323d089c6f3f26a597b09cb4d2aa",
-                "sha256:062b0a75d9261e2f9c6d071753f7eef0fc9caf3a2c82d36d76667ba7b6470003",
-                "sha256:0842571634f39016a6c03e9d4aba502be652a6e4455fadb73cd3a3a49173e38f",
-                "sha256:16bae383a9cc5abab9bb05c10a3e5a52e0a788325dc9ba8499e821885928968c",
-                "sha256:18c7320695c949de11a351742ee001849912fd57e62a706d83dfc1581897fa2e",
-                "sha256:18d90523ce7553dd0b7e23cbb28865db23cddfd683a38fb224115f7826de78d0",
-                "sha256:1bf25fbca0c8d121a3e92a2a0555c7e5bc981aee5c3fdaf4bb7809f410f696b9",
-                "sha256:276f6077a5c61447a48d133ed13e759c09e62aff0dc84274a68dc18660104d52",
-                "sha256:280459f0a03cecbe8800786cdc23067a8fc64c0bd51dc614008d9c36e1659d7e",
-                "sha256:28ca2098939eabab044ad68850aac8f8db6bf0b29bc7f2887d05889b17346454",
-                "sha256:2c854ce44e1ee31bda4e318af1dbcfc929026d12c5ed030095ad98197eeeaed0",
-                "sha256:35eb581efdacf7b7422af677b92170da4ef34500467381e805944a3201df2079",
-                "sha256:37389611ba54fd6d278fde86eb2c013c8e50232e38f5c68235d09d0a3f8aa352",
-                "sha256:3b253094dbe1b431d3a4ac2f053b6d7ede2664ac559705a704f621742e034f1f",
-                "sha256:3b2eccb883368f9e972e216c7b4c7c06cabda925b5f06dde0650281cb7666a30",
-                "sha256:451f433ad901b3bb00184d83fd83d135fb682d780b38af7944c9faeecb1e0bfe",
-                "sha256:489763b2d037b164846ebac0cbd368b8a4ca56385c4090807ff9fad817de4113",
-                "sha256:4af154d617c875b52651dd8dd17a31270c495082f3d55f6128e7629658d63765",
-                "sha256:506edb1dd49e13a2d4cac6a5173317b82a23c9d6e8df63efb4f0380de0fbccbc",
-                "sha256:6679060424faa9c11808598504c3ab472de4531c571ab2befa32f4971835788e",
-                "sha256:69b9f6f66c0af29642e73a520b6fed25ff9fd69a25975ebe6acb297234eda501",
-                "sha256:6c00cdc8fa4e50e1cc1f941a7f2e3e0f26cb2a1233c9696f26963ff58445bac7",
-                "sha256:6c0cdedd3500e0511eac1517bf560149764b7d8e65cb800d8bf1c63ebf39edd2",
-                "sha256:708a3369dcf055c00ddeeaa2b20f0dd1ce664eeabde6623e516c5228b753654f",
-                "sha256:718187eeb9849fc6cc23e0d9b092bc2348821c5e1a901c9f8975df0bc785bfd4",
-                "sha256:767b35c3a246bcb55b8044fd3a43b8cd553dd1f9f2c1eeb87a302b1f8daa0524",
-                "sha256:77fbfc5720cceac9c200054b9fab50cb2a7d79660609200ab83f5db96162d20c",
-                "sha256:7cbde573904625509a3f37b6fecea974e363460b556a627c60dc2f47e2fffa51",
-                "sha256:8249b1c7334be8f8c3abcaaa996e1e4927b0e5a23b65f5bf6cfe3180d8ca7840",
-                "sha256:8580b827d4746d47294c0e0b92854c85a92c2227927433998f0d3320ae8a71b6",
-                "sha256:8640f1fde5e1b8e3439fe482cdc2b0bb6c329f4bb161927c28d2e8879c6029ee",
-                "sha256:9a9babb9466fe1da12417a4aed923e90124a534736de6201794a3aea9d98484e",
-                "sha256:a78ed23b08e8ab524551f52953a8a05d61c3a760781762aac49f8de6eede8c45",
-                "sha256:abbbd8093c5229c72d4c2926afaee0e6e3140de69d5dcd918b2921f2f0c8baba",
-                "sha256:ae7f19afe0cce50039e2c782bff379c7e347cba335429678450b8fe81c4ef96d",
-                "sha256:b3ec74cfef2d985e145baae90d9b1b32f85e1741b04cd967aaf9cfa84c1334f3",
-                "sha256:b51bfc348925e92a9bd9b2e48dad13431b57011fd1038f08316e6bf1df107d10",
-                "sha256:b9a4a8dd3dcf4cbd3165737358e4d7dfbd9d59902ad11e3b15eebb6393b0446e",
-                "sha256:ba3a8aaed13770e970b3df46980cb068d1c24af1a1968b7818b69af8c4347efb",
-                "sha256:c0524de3ff096e15fcbfe8f056fdb4ea0bf497d584454f344d59fce069d3e6e9",
-                "sha256:c0a120238dd71c68484f02562f6d446d736adcc6ca0993712289b102705a9a3a",
-                "sha256:cbbe5e739d45a52f3200a771c6d2c7acf89eb2524890a4a3aa1a7fa0695d2a47",
-                "sha256:ce8c50520f57ec57aa21a63ea4f325c7b657386b3f02ccaedeccf9ebe27686e1",
-                "sha256:cf30900aa1ba595312ae41978b95e256e419d8a823af79ce670835409fc02ad3",
-                "sha256:d25b937a5d9ffa857d41be042b4238dd61db888533b53bc76dc082cb5a15e914",
-                "sha256:d6cdecaedea1ea9e033d8adf6a0ab11107b49571bbb9737175444cea6eb72328",
-                "sha256:dec9de46a33cf2dd87a5254af095a409ea3bf952d85ad339751e7de6d962cde6",
-                "sha256:ebe7c9e67a2d15fa97b77ea6571ce5e1e1f6b0db71d1d5e96f8d2bf134303c1d",
-                "sha256:ee866acc0861caebb4f2ab79f0b94dbfbdbfadc19f82e6e9c93930f74e11d7a0",
-                "sha256:f6a09b360d67e589236a44f0c39218a8efba2593b6abdccc300a8862cffc2f94",
-                "sha256:fcc66e222cf4c719fe7722a403888b1f5e1682d1679bd780e2b26c18bb648cdc",
-                "sha256:fd6545d97c98a192c5ac995d21c894b581f1fd14cf389be90724d21808b657e2"
+                "sha256:00838a35b882694afda09f85e469c96367daa3f3f2b097d846a7216993d37f4c",
+                "sha256:0513b9508b93da4e1716744ef6ebc507aff016ba115ffe8ecff744d1322a7b63",
+                "sha256:09c3255458533cb76ef55da8cc49ffab9e33f083739c8bd4f58e79fecfe288f7",
+                "sha256:09ef9199ed6653989ebbcaacc9b62b514bb63ea2f90256e71fea3ed74bd8ff6f",
+                "sha256:09fa497a8ab37784fbb20ab699c246053ac294d13fc7eb40ec007a5043ec91f8",
+                "sha256:0f9f50e7ef2a71e2fae92774c99170eb8304e3fdf9c8c3c7ae9bab3e7229c5cf",
+                "sha256:137eb07173141545e07403cca94ab625cc1cc6bc4c1e97b6e3846270e7e1fea0",
+                "sha256:1f384c3cc76aeedce208643697fb3e8437604b512255de6d18dae3f27655a384",
+                "sha256:201bef2eea65e0e9c56343115ba3814e896afe6d36ffd37bab783261db430f76",
+                "sha256:38dd60d7bf242c4ed5b38e094baf6401faa114fc09e9e6632374388a404f98e7",
+                "sha256:3b799445b9f7ee8bf299cfaed6f5b226c0037b74886a4e11515e569b36fe310d",
+                "sha256:3ea79bb50e805cd6ac058dfa3b5c8f6c040cb87fe83de10845857f5535d1db70",
+                "sha256:40209e141059b9370a2657c9b15607815359ab3ef9918f0196b6fccce8d3230f",
+                "sha256:41c9c5f3de16b903b610d09650e5e27adbfa7f500302718c9ffd1c12cf9d6818",
+                "sha256:54eb8d1bf7cacfbf2a3186019bcf01d11c666bd495ed18717162f7eb1e9dd00b",
+                "sha256:598825b51b81c808cb6f078dcb972f96af96b078faa47af7dfcdf282835baa8d",
+                "sha256:5fc1de20b2d4a061b3df27ab9b7c7111e9a710f10dc2b84d33a4ab25065994ec",
+                "sha256:623512f8ba53c422fcfb2ce68362c97945095b864cda94a92edbaf5994201083",
+                "sha256:690db6517f09336559dc0b5f55342df62370a48f5469fabf502db2c6d1cffcd2",
+                "sha256:69eb372f7e2ece89f14751fbcbe470295d73ed41ecd37ca36ed2eb47512a6ab9",
+                "sha256:73bfb9c09951125d06ee473bed216e2c3742f530fc5acc1383883125de76d9cd",
+                "sha256:742a76a12aa45b44d236815d282b03cfb1de3b4323f3e4ec933acfae08e54ade",
+                "sha256:7c95949560050d04d46b919301826525597f07b33beba6187d04fa64d47ac82e",
+                "sha256:8130a2aa2acb8788e0b56938786c33c7c98562697bf9f4c7d6e8e5e3a0501e4a",
+                "sha256:8a2b2b78c78293782fd3767d53e6474582f62443d0504b1554370bde86cc8227",
+                "sha256:8ce1415194b4a6bd0cdcc3a1dfbf58b63f910dcb7330fe15bdff542c56949f87",
+                "sha256:9ca28a302acb19b6af89e90f33ee3e1906961f94b54ea37de6737b7ca9d8827c",
+                "sha256:a4cdc86d54b5da0df6d3d3a2f0b710949286094c3a6700c21e9015932b81447e",
+                "sha256:aa5b1c1bfc28384f1f53b69a023d789f72b2e0ab1b3787aae16992a7ca21056c",
+                "sha256:aadacf9a2f407a4688d700e4ebab33a7e2e408f2ca04dbf4aef17585389eff3e",
+                "sha256:ae71e7ddb7a413dd60052e90528f2f65270aad4b509563af6d03d53e979feafd",
+                "sha256:b14706df8b2de49869ae03a5ccbc211f4041750cd4a66f698df89d44f4bd30ec",
+                "sha256:b1a93009cb80730c9bca5d6d4665494b725b6e8e157c1cb7f2db5b4b122ea562",
+                "sha256:b2991665420a803495e0b90a79233c1433d6ed77ef282e8e152a324bbbc5e0c8",
+                "sha256:b2c5edc4ac10a7ef6605a966c58929ec6c1bd0917fb8c15cb3363f65aa40e677",
+                "sha256:b4d33f418f46362995f1e9d4f3a35a1b6322cb959c31d88ae56b0298e1c22357",
+                "sha256:b91cbc4b195444e7e258ba27ac33769c41b94967919f10037e6355e998af255c",
+                "sha256:c74880fc64d4958159fbd537a091d2a585448a8f8508bf248d72112723974cbd",
+                "sha256:c901df83d097649e257e803be22592aedfd5182f07b3cc87d640bbb9afd50f49",
+                "sha256:cac99918c7bba15302a2d81f0312c08054a3359eaa1929c7e4b26ebe41e9b286",
+                "sha256:cc4f1358cb0c78edef3ed237ef2c86056206bb8d9140e73b6b89fbcfcbdd40e1",
+                "sha256:ccd341521be3d1b3daeb41960ae94a5e87abe2f46f17224ba5d6f2b8398016cf",
+                "sha256:ce4b94265ca988c3f8e479e741693d143026632672e3ff924f25fab50518dd51",
+                "sha256:cf271892d13e43bc2b51e6908ec9a6a5094a4df1d8af0bfc360088ee6c684409",
+                "sha256:d5ae728ff3b5401cc320d792866987e7e7e880e6ebd24433b70a33b643bb0384",
+                "sha256:d71eec7d83298f1af3326ce0ff1d0ea83c7cb98f72b577097f9083b20bdaf05e",
+                "sha256:d898fe162d26929b5960e4e138651f7427048e72c853607f2b200909794ed978",
+                "sha256:d89d7b2974cae412400e88f35d86af72208e1ede1a541954af5d944a8ba46c57",
+                "sha256:dfa8fe35a0bb90382837b238fff375de15f0dcdb9ae68ff85f7a63649c98527e",
+                "sha256:e0be5efd5127542ef31f165de269f77560d6cdef525fffa446de6f7e9186cfb2",
+                "sha256:fdfafb32984684eb03c2d83e1e51f64f0906b11e64482df3c5db936ce3839d48",
+                "sha256:ff7687ca3d7028d8a5f0ebae95a6e4827c5616b31a4ee1192bdfde697db110d4"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==7.4.3"
+            "version": "==7.4.4"
         },
         "distlib": {
             "hashes": [
                 "sha256:034db59a0b96f8ca18035f36290806a9a6e6bd9d1ff91e45a7f172eb17e51784",
                 "sha256:1530ea13e350031b6312d8580ddb6b27a104275a31106523b8f123787f494f64"
             ],
             "version": "==0.3.8"
@@ -264,20 +264,20 @@
                 "sha256:c4de0081837b211594f8e877a6b4fad7ca32bbfc1a9307fdd61c28bfe923f13e"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==2.5.35"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:198f568f3230878cb1b44fbd7975f87906c22336dba2e4a7f05278c281fbd792",
-                "sha256:f4bc4c0c070c490abf4ce96d715f68e95923320370efb66143df00199bb6c100"
+                "sha256:30962b96c0c223483ed6cc7280e7f0199feb01a0e40cfae4d4450fc6fab1f570",
+                "sha256:b78938b926ee8d5f020fc4772d487045805a55ddbad2ecf21c6d60938dc7fcd2"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.8'",
-            "version": "==7.0.2"
+            "version": "==7.1.0"
         },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
@@ -396,20 +396,20 @@
                 "sha256:8c85c2876142a764e5b7548e7d9a0e0ddb46f5185161049a79b7e974454223be"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==1.4.0"
         },
         "pre-commit": {
             "hashes": [
-                "sha256:ba637c2d7a670c10daedc059f5c49b5bd0aadbccfcd7ec15592cf9665117532c",
-                "sha256:c3ef34f463045c88658c5b99f38c1e297abdcc0ff13f98d3370055fbbfabc67e"
+                "sha256:5804465c675b659b0862f07907f96295d490822a450c4c40e747d0b1c6ebcb32",
+                "sha256:841dc9aef25daba9a0238cd27984041fa0467b4199fc4852e27950664919f660"
             ],
             "index": "pypi",
-            "markers": "python_version >= '3.9'",
-            "version": "==3.6.2"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.5.0"
         },
         "py": {
             "hashes": [
                 "sha256:51c75c4126074b472f746a24399ad32f6053d1b34b68d2fa41e558e6f4a98719",
                 "sha256:607c53218732647dff4acdfcd50cb62615cedf612e72d1724fb1a0cc6405b378"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
@@ -594,29 +594,29 @@
                 "sha256:e08e13ecdca7a0bd53798f356d5831434afa5b07b93f0abdf0797b7a06ffe197"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==20.25.1"
         },
         "zipp": {
             "hashes": [
-                "sha256:c1bb803ed69d2cce2373152797064f7e79bc43f0a3748eb494096a867e0ebf79",
-                "sha256:df8d042b02765029a09b157efd8e820451045890acc30f8e37dd2f94a060221f"
+                "sha256:206f5a15f2af3dbaee80769fb7dc6f249695e940acca08dfb2a4769fe61e538b",
+                "sha256:2884ed22e7d8961de1c9a05142eb69a247f120291bc0206a00a7642f09b5b715"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==3.18.0"
+            "version": "==3.18.1"
         }
     },
     "doc": {
         "alabaster": {
             "hashes": [
-                "sha256:75a8b99c28a5dad50dd7f8ccdd447a121ddb3892da9e53d1ca5cca3106d58d65",
-                "sha256:b46733c07dce03ae4e150330b975c75737fa60f0a7c591b6c8bf4928a28e2c92"
+                "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3",
+                "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
             ],
-            "markers": "python_version >= '3.9'",
-            "version": "==0.7.16"
+            "markers": "python_version >= '3.6'",
+            "version": "==0.7.13"
         },
         "babel": {
             "hashes": [
                 "sha256:6919867db036398ba21eb5c7a0f6b28ab8cbc3ae7a73a44ebe34ae74a4e7d363",
                 "sha256:efb1a25b7118e67ce3a259bed20545c29cb68be8ad2c784c83689981b7a57287"
             ],
             "markers": "python_version >= '3.7'",
@@ -746,14 +746,22 @@
             "hashes": [
                 "sha256:0d8d18d08f840c19d0ee7ca1fd82490fdc3729b7ac93f49870406ddde8ef8d8b",
                 "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.4.1"
         },
+        "importlib-metadata": {
+            "hashes": [
+                "sha256:30962b96c0c223483ed6cc7280e7f0199feb01a0e40cfae4d4450fc6fab1f570",
+                "sha256:b78938b926ee8d5f020fc4772d487045805a55ddbad2ecf21c6d60938dc7fcd2"
+            ],
+            "markers": "python_version < '3.10'",
+            "version": "==7.1.0"
+        },
         "jinja2": {
             "hashes": [
                 "sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa",
                 "sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.1.3"
@@ -869,14 +877,22 @@
             "hashes": [
                 "sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c",
                 "sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.17.2"
         },
+        "pytz": {
+            "hashes": [
+                "sha256:2a29735ea9c18baf14b448846bde5a48030ed267578472d8955cd0e7443a9812",
+                "sha256:328171f4e3623139da4983451950b28e95ac706e13f3f2630a879749e7a8b319"
+            ],
+            "markers": "python_version < '3.9'",
+            "version": "==2024.1"
+        },
         "pyyaml": {
             "hashes": [
                 "sha256:04ac92ad1925b2cff1db0cfebffb6ffc43457495c9b3c39d3fcae417d7125dc5",
                 "sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc",
                 "sha256:0d3304d8c0adc42be59c5f8a4d9e3d7379e6955ad754aa9d6ab7a398b59dd1df",
                 "sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741",
                 "sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206",
@@ -943,20 +959,20 @@
                 "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1",
                 "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"
             ],
             "version": "==2.2.0"
         },
         "sphinx": {
             "hashes": [
-                "sha256:1e09160a40b956dc623c910118fa636da93bd3ca0b9876a7b3df90f07d691560",
-                "sha256:9a5160e1ea90688d5963ba09a2dcd8bdd526620edbb65c328728f1b2228d5ab5"
+                "sha256:780f4d32f1d7d1126576e0e5ecc19dc32ab76cd24e950228dcf7b1f6d3d9e22f",
+                "sha256:d170a81825b2fcacb6dfd5a0d7f578a053e45d3f2b153fecc948c37344eb4cbe"
             ],
             "index": "pypi",
-            "markers": "python_version >= '3.9'",
-            "version": "==7.2.6"
+            "markers": "python_version >= '3.8'",
+            "version": "==7.1.2"
         },
         "sphinx-autodoc-typehints": {
             "hashes": [
                 "sha256:12c0e161f6fe191c2cdfd8fa3caea271f5387d9fbc67ebcd6f4f1f24ce880993",
                 "sha256:7f2cdac2e70fd9787926b6e9e541cd4ded1e838d2b46fda2a1bb0a75ec5b7f3a"
             ],
             "index": "pypi",
@@ -970,63 +986,71 @@
             ],
             "index": "pypi",
             "markers": "python_version >= '3.7'",
             "version": "==0.5.2"
         },
         "sphinxcontrib-applehelp": {
             "hashes": [
-                "sha256:c40a4f96f3776c4393d933412053962fac2b84f4c99a7982ba42e09576a70619",
-                "sha256:cb61eb0ec1b61f349e5cc36b2028e9e7ca765be05e49641c97241274753067b4"
+                "sha256:29d341f67fb0f6f586b23ad80e072c8e6ad0b48417db2bde114a4c9746feb228",
+                "sha256:828f867945bbe39817c210a1abfd1bc4895c8b73fcaade56d45357a348a07d7e"
             ],
-            "markers": "python_version >= '3.9'",
-            "version": "==1.0.8"
+            "markers": "python_version >= '3.8'",
+            "version": "==1.0.4"
         },
         "sphinxcontrib-devhelp": {
             "hashes": [
-                "sha256:6485d09629944511c893fa11355bda18b742b83a2b181f9a009f7e500595c90f",
-                "sha256:9893fd3f90506bc4b97bdb977ceb8fbd823989f4316b28c3841ec128544372d3"
+                "sha256:8165223f9a335cc1af7ffe1ed31d2871f325254c0423bc0c4c7cd1c1e4734a2e",
+                "sha256:ff7f1afa7b9642e7060379360a67e9c41e8f3121f2ce9164266f61b9f4b338e4"
             ],
-            "markers": "python_version >= '3.9'",
-            "version": "==1.0.6"
+            "markers": "python_version >= '3.5'",
+            "version": "==1.0.2"
         },
         "sphinxcontrib-htmlhelp": {
             "hashes": [
-                "sha256:0dc87637d5de53dd5eec3a6a01753b1ccf99494bd756aafecd74b4fa9e729015",
-                "sha256:393f04f112b4d2f53d93448d4bce35842f62b307ccdc549ec1585e950bc35e04"
+                "sha256:0cbdd302815330058422b98a113195c9249825d681e18f11e8b1f78a2f11efff",
+                "sha256:c38cb46dccf316c79de6e5515e1770414b797162b23cd3d06e67020e1d2a6903"
             ],
-            "markers": "python_version >= '3.9'",
-            "version": "==2.0.5"
+            "markers": "python_version >= '3.8'",
+            "version": "==2.0.1"
         },
         "sphinxcontrib-jsmath": {
             "hashes": [
                 "sha256:2ec2eaebfb78f3f2078e73666b1415417a116cc848b72e5172e596c871103178",
                 "sha256:a9925e4a4587247ed2191a22df5f6970656cb8ca2bd6284309578f2153e0c4b8"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.1"
         },
         "sphinxcontrib-qthelp": {
             "hashes": [
-                "sha256:053dedc38823a80a7209a80860b16b722e9e0209e32fea98c90e4e6624588ed6",
-                "sha256:e2ae3b5c492d58fcbd73281fbd27e34b8393ec34a073c792642cd8e529288182"
+                "sha256:4c33767ee058b70dba89a6fc5c1892c0d57a54be67ddd3e7875a18d14cba5a72",
+                "sha256:bd9fc24bcb748a8d51fd4ecaade681350aa63009a347a8c14e637895444dfab6"
             ],
-            "markers": "python_version >= '3.9'",
-            "version": "==1.0.7"
+            "markers": "python_version >= '3.5'",
+            "version": "==1.0.3"
         },
         "sphinxcontrib-serializinghtml": {
             "hashes": [
-                "sha256:326369b8df80a7d2d8d7f99aa5ac577f51ea51556ed974e7716cfd4fca3f6cb7",
-                "sha256:93f3f5dc458b91b192fe10c397e324f262cf163d79f3282c158e8436a2c4511f"
+                "sha256:352a9a00ae864471d3a7ead8d7d79f5fc0b57e8b3f95e9867eb9eb28999b92fd",
+                "sha256:aa5f6de5dfdf809ef505c4895e51ef5c9eac17d0f287933eb49ec495280b6952"
             ],
-            "markers": "python_version >= '3.9'",
-            "version": "==1.1.10"
+            "markers": "python_version >= '3.5'",
+            "version": "==1.1.5"
         },
         "urllib3": {
             "hashes": [
                 "sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d",
                 "sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==2.2.1"
+        },
+        "zipp": {
+            "hashes": [
+                "sha256:206f5a15f2af3dbaee80769fb7dc6f249695e940acca08dfb2a4769fe61e538b",
+                "sha256:2884ed22e7d8961de1c9a05142eb69a247f120291bc0206a00a7642f09b5b715"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==3.18.1"
         }
     }
 }
```

### Comparing `fotolab-0.9.0/README.md` & `fotolab-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `fotolab-0.9.0/docs/Makefile` & `fotolab-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fotolab-0.9.0/docs/make.bat` & `fotolab-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fotolab-0.9.0/docs/source/_static/logo.jpg` & `fotolab-0.9.1/docs/source/_static/logo.jpg`

 * *Files identical despite different names*

### Comparing `fotolab-0.9.0/docs/source/conf.py` & `fotolab-0.9.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fotolab-0.9.0/fotolab/__main__.py` & `fotolab-0.9.1/fotolab/__main__.py`

 * *Files identical despite different names*

### Comparing `fotolab-0.9.0/fotolab/auto.py` & `fotolab-0.9.1/fotolab/auto.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
         "font_size": 12,
         "font_color": "white",
         "outline_width": 2,
         "outline_color": "black",
     }
     combined_args = argparse.Namespace(**vars(args), **extra_args)
     combined_args.overwrite = True
+    combined_args.open = False
     log.debug(args)
     log.debug(combined_args)
 
     fotolab.resize.run(combined_args)
     fotolab.contrast.run(combined_args)
     fotolab.sharpen.run(combined_args)
     fotolab.watermark.run(combined_args)
```

### Comparing `fotolab-0.9.0/fotolab/border.py` & `fotolab-0.9.1/fotolab/border.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 
 """Border subcommand."""
 
 import argparse
 import logging
-from pathlib import Path
 
 from PIL import Image, ImageColor, ImageOps
 
+from fotolab import save_image
+
 log = logging.getLogger(__name__)
 
 
 def build_subparser(subparsers) -> None:
     """Build the subparser."""
     border_parser = subparsers.add_parser("border", help="add border to image")
 
@@ -106,16 +107,14 @@
         config (argparse.Namespace): Config from command line arguments
 
     Returns:
         None
     """
     log.debug(args)
 
-    image_file = Path(args.image_filename)
-
     original_image = Image.open(args.image_filename)
 
     if (
         args.width_left
         or args.width_top
         or args.width_right
         or args.width_bottom
@@ -131,17 +130,8 @@
 
     bordered_image = ImageOps.expand(
         original_image,
         border=border,
         fill=ImageColor.getrgb(args.color),
     )
 
-    if args.overwrite:
-        new_filename = image_file.with_name(image_file.name)
-    else:
-        new_filename = Path(
-            args.output_dir, image_file.with_name(f"border_{image_file.name}")
-        )
-        new_filename.parent.mkdir(parents=True, exist_ok=True)
-
-    log.info("creating image: %s", new_filename)
-    bordered_image.save(new_filename)
+    save_image(args, bordered_image)
```

### Comparing `fotolab-0.9.0/fotolab/cli.py` & `fotolab-0.9.1/fotolab/cli.py`

 * *Files identical despite different names*

### Comparing `fotolab-0.9.0/fotolab/contrast.py` & `fotolab-0.9.1/fotolab/contrast.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 
 """Contrast subcommand."""
 
 import argparse
 import logging
-from pathlib import Path
 
 from PIL import Image, ImageOps
 
+from fotolab import save_image
+
 log = logging.getLogger(__name__)
 
 
 def build_subparser(subparsers) -> None:
     """Build the subparser."""
     contrast_parser = subparsers.add_parser(
         "contrast", help="contrast an image"
@@ -62,23 +63,11 @@
         config (argparse.Namespace): Config from command line arguments
 
     Returns:
         None
     """
     log.debug(args)
 
-    image_file = Path(args.image_filename)
-
     original_image = Image.open(args.image_filename)
     contrast_image = ImageOps.autocontrast(original_image, cutoff=args.cutoff)
 
-    if args.overwrite:
-        new_filename = image_file.with_name(image_file.name)
-    else:
-        new_filename = Path(
-            args.output_dir,
-            image_file.with_name(f"contrast_{image_file.name}"),
-        )
-        new_filename.parent.mkdir(parents=True, exist_ok=True)
-
-    log.info("contrasting image: %s", new_filename)
-    contrast_image.save(new_filename)
+    save_image(args, contrast_image)
```

### Comparing `fotolab-0.9.0/fotolab/env.py` & `fotolab-0.9.1/fotolab/env.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,10 +41,12 @@
         config (argparse.Namespace): Config from command line arguments
 
     Returns:
         None
     """
     log.debug(args)
 
+    sys_version = sys.version.replace("\n", "")
+
     print(f"fotolab: {__version__}")
-    print(f"python: {sys.version}")
+    print(f"python: {sys_version}")
     print(f"platform: {platform.platform()}")
```

### Comparing `fotolab-0.9.0/fotolab/resize.py` & `fotolab-0.9.1/fotolab/resize.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 
 """Resize subcommand."""
 
 import argparse
 import logging
-from pathlib import Path
 
 from PIL import Image
 
+from fotolab import save_image
+
 log = logging.getLogger(__name__)
 
 
 def build_subparser(subparsers) -> None:
     """Build the subparser."""
     resize_parser = subparsers.add_parser("resize", help="resize an image")
 
@@ -59,32 +60,21 @@
     )
 
 
 def run(args: argparse.Namespace) -> None:
     """Run resize subcommand.
 
     Args:
-        config (argparse.Namespace): Config from command line arguments
+        args (argparse.Namespace): Config from command line arguments
 
     Returns:
         None
     """
     log.debug(args)
 
-    image_file = Path(args.image_filename)
     original_image = Image.open(args.image_filename)
     resized_image = original_image.copy()
     resized_image = resized_image.resize(
         (args.width, args.height), Image.Resampling.LANCZOS
     )
 
-    if args.overwrite:
-        new_filename = image_file.with_name(image_file.name)
-    else:
-        new_filename = Path(
-            args.output_dir,
-            image_file.with_name(f"resize_{image_file.name}"),
-        )
-        new_filename.parent.mkdir(parents=True, exist_ok=True)
-
-    log.info("resizing image: %s", new_filename)
-    resized_image.save(new_filename)
+    save_image(args, resized_image)
```

### Comparing `fotolab-0.9.0/fotolab/sharpen.py` & `fotolab-0.9.1/fotolab/sharpen.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 
 """Sharpen subcommand."""
 
 import argparse
 import logging
-from pathlib import Path
 
 from PIL import Image, ImageFilter
 
+from fotolab import save_image
+
 log = logging.getLogger(__name__)
 
 
 def build_subparser(subparsers) -> None:
     """Build the subparser."""
     sharpen_parser = subparsers.add_parser("sharpen", help="sharpen an image")
 
@@ -82,26 +83,14 @@
         config (argparse.Namespace): Config from command line arguments
 
     Returns:
         None
     """
     log.debug(args)
 
-    image_file = Path(args.image_filename)
-
     original_image = Image.open(args.image_filename)
     sharpen_image = original_image.filter(
         ImageFilter.UnsharpMask(
             args.radius, percent=args.percent, threshold=args.threshold
         )
     )
-
-    if args.overwrite:
-        new_filename = image_file.with_name(image_file.name)
-    else:
-        new_filename = Path(
-            args.output_dir, image_file.with_name(f"sharpen_{image_file.name}")
-        )
-        new_filename.parent.mkdir(parents=True, exist_ok=True)
-
-    log.info("sharpening image: %s", new_filename)
-    sharpen_image.save(new_filename)
+    save_image(args, sharpen_image)
```

### Comparing `fotolab-0.9.0/fotolab/watermark.py` & `fotolab-0.9.1/fotolab/watermark.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 
 """Watermark subcommand."""
 
 import argparse
 import logging
-from pathlib import Path
 
 from PIL import Image, ImageColor, ImageDraw, ImageFont
 
+from fotolab import save_image
+
 log = logging.getLogger(__name__)
 
 POSITIONS = ["top-left", "top-right", "bottom-left", "bottom-right"]
 
 
 def build_subparser(subparsers) -> None:
     """Build the subparser."""
@@ -115,16 +116,14 @@
         config (argparse.Namespace): Config from command line arguments
 
     Returns:
         None
     """
     log.debug(args)
 
-    image_file = Path(args.image_filename)
-
     original_image = Image.open(args.image_filename)
     watermarked_image = original_image.copy()
 
     draw = ImageDraw.Draw(watermarked_image)
 
     font = ImageFont.truetype("arial.ttf", args.font_size)
 
@@ -142,25 +141,15 @@
         args.text,
         font=font,
         fill=ImageColor.getrgb(args.font_color),
         stroke_width=args.outline_width,
         stroke_fill=ImageColor.getrgb(args.outline_color),
     )
 
-    if args.overwrite:
-        new_filename = image_file.with_name(image_file.name)
-    else:
-        new_filename = Path(
-            args.output_dir,
-            image_file.with_name(f"watermark_{image_file.name}"),
-        )
-        new_filename.parent.mkdir(parents=True, exist_ok=True)
-
-    log.info("watermarking image: %s", new_filename)
-    watermarked_image.save(new_filename)
+    save_image(args, watermarked_image)
 
 
 def calculate_position(image, text_width, text_height, position) -> tuple:
     """Calculate the boundary coordinates of the watermark text."""
     padding = 10
     if position == "top-left":
         position_x = 0 + padding
```

### Comparing `fotolab-0.9.0/pyproject.toml` & `fotolab-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fotolab-0.9.0/tests/conftest.py` & `fotolab-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fotolab-0.9.0/tox.ini` & `fotolab-0.9.1/tox.ini`

 * *Files identical despite different names*

### Comparing `fotolab-0.9.0/PKG-INFO` & `fotolab-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fotolab
-Version: 0.9.0
+Version: 0.9.1
 Summary: A console program that manipulate images.
 Keywords: photography,photo
 Author-email: Kian-Meng Ang <kianmeng@cpan.org>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

