# Comparing `tmp/nakametpy-2024.3.0.tar.gz` & `tmp/nakametpy-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nakametpy-2024.3.0.tar", last modified: Wed Mar 20 13:38:47 2024, max compression
+gzip compressed data, was "nakametpy-2024.4.0.tar", last modified: Sat Apr 20 09:42:19 2024, max compression
```

## Comparing `nakametpy-2024.3.0.tar` & `nakametpy-2024.4.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-03-20 13:38:47.024079 nakametpy-2024.3.0/
--rw-rw-rw-   0        0        0     1555 2024-03-20 13:25:39.000000 nakametpy-2024.3.0/LICENSE
--rw-rw-rw-   0        0        0       58 2024-03-20 13:25:39.000000 nakametpy-2024.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3636 2024-03-20 13:38:47.023080 nakametpy-2024.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3200 2024-03-20 13:25:39.000000 nakametpy-2024.3.0/README.md
--rw-rw-rw-   0        0        0      540 2024-03-20 13:35:48.000000 nakametpy-2024.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       47 2024-03-20 13:25:40.000000 nakametpy-2024.3.0/requirements.txt
--rw-rw-rw-   0        0        0       81 2024-03-20 13:38:47.026109 nakametpy-2024.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1106 2024-03-20 13:35:53.000000 nakametpy-2024.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-20 13:38:46.969793 nakametpy-2024.3.0/src/
-drwxrwxrwx   0        0        0        0 2024-03-20 13:38:47.008580 nakametpy-2024.3.0/src/nakametpy/
--rw-rw-rw-   0        0        0      877 2024-03-20 13:25:40.000000 nakametpy-2024.3.0/src/nakametpy/__init__.py
--rw-rw-rw-   0        0        0     6507 2024-03-20 13:25:40.000000 nakametpy-2024.3.0/src/nakametpy/_error.py
--rw-rw-rw-   0        0        0      195 2024-03-20 13:34:56.000000 nakametpy-2024.3.0/src/nakametpy/_version.py
--rw-rw-rw-   0        0        0    68632 2024-03-20 13:25:40.000000 nakametpy-2024.3.0/src/nakametpy/cmaps.py
--rw-rw-rw-   0        0        0     2834 2024-03-20 13:25:40.000000 nakametpy-2024.3.0/src/nakametpy/constants.py
--rw-rw-rw-   0        0        0    12123 2024-03-20 13:25:40.000000 nakametpy-2024.3.0/src/nakametpy/grads.py
--rw-rw-rw-   0        0        0     1265 2024-03-20 13:25:40.000000 nakametpy-2024.3.0/src/nakametpy/jma.py
--rw-rw-rw-   0        0        0    67887 2024-03-20 13:25:40.000000 nakametpy-2024.3.0/src/nakametpy/kinematics.py
--rw-rw-rw-   0        0        0    26216 2024-03-20 13:25:40.000000 nakametpy-2024.3.0/src/nakametpy/thermo.py
--rw-rw-rw-   0        0        0     7786 2024-03-20 13:25:40.000000 nakametpy-2024.3.0/src/nakametpy/util.py
-drwxrwxrwx   0        0        0        0 2024-03-20 13:38:47.022080 nakametpy-2024.3.0/src/nakametpy.egg-info/
--rw-rw-rw-   0        0        0     3636 2024-03-20 13:38:46.000000 nakametpy-2024.3.0/src/nakametpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      508 2024-03-20 13:38:46.000000 nakametpy-2024.3.0/src/nakametpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-20 13:38:46.000000 nakametpy-2024.3.0/src/nakametpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-03-20 13:38:46.000000 nakametpy-2024.3.0/src/nakametpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-20 13:38:46.000000 nakametpy-2024.3.0/src/nakametpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 09:42:19.516022 nakametpy-2024.4.0/
+-rw-rw-rw-   0        0        0     1555 2024-03-20 13:25:39.000000 nakametpy-2024.4.0/LICENSE
+-rw-rw-rw-   0        0        0       58 2024-03-20 13:25:39.000000 nakametpy-2024.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3043 2024-04-20 09:42:19.516022 nakametpy-2024.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2526 2024-04-20 09:36:49.000000 nakametpy-2024.4.0/README.md
+-rw-rw-rw-   0        0        0      668 2024-04-20 09:40:40.000000 nakametpy-2024.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0      113 2024-04-20 09:36:49.000000 nakametpy-2024.4.0/requirements.txt
+-rw-rw-rw-   0        0        0       81 2024-04-20 09:42:19.518016 nakametpy-2024.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1106 2024-04-20 09:40:40.000000 nakametpy-2024.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 09:42:19.458177 nakametpy-2024.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-20 09:42:19.497073 nakametpy-2024.4.0/src/nakametpy/
+-rw-rw-rw-   0        0        0      877 2024-03-20 13:25:40.000000 nakametpy-2024.4.0/src/nakametpy/__init__.py
+-rw-rw-rw-   0        0        0     6872 2024-04-20 09:36:49.000000 nakametpy-2024.4.0/src/nakametpy/_error.py
+-rw-rw-rw-   0        0        0      195 2024-04-20 09:40:40.000000 nakametpy-2024.4.0/src/nakametpy/_version.py
+-rw-rw-rw-   0        0        0    68632 2024-03-20 13:25:40.000000 nakametpy-2024.4.0/src/nakametpy/cmaps.py
+-rw-rw-rw-   0        0        0     2834 2024-03-20 13:25:40.000000 nakametpy-2024.4.0/src/nakametpy/constants.py
+-rw-rw-rw-   0        0        0    12123 2024-03-20 13:25:40.000000 nakametpy-2024.4.0/src/nakametpy/grads.py
+-rw-rw-rw-   0        0        0     1265 2024-03-20 13:25:40.000000 nakametpy-2024.4.0/src/nakametpy/jma.py
+-rw-rw-rw-   0        0        0    67887 2024-03-20 13:25:40.000000 nakametpy-2024.4.0/src/nakametpy/kinematics.py
+-rw-rw-rw-   0        0        0    26216 2024-03-20 13:25:40.000000 nakametpy-2024.4.0/src/nakametpy/thermo.py
+-rw-rw-rw-   0        0        0     9905 2024-04-20 09:36:49.000000 nakametpy-2024.4.0/src/nakametpy/util.py
+drwxrwxrwx   0        0        0        0 2024-04-20 09:42:19.514029 nakametpy-2024.4.0/src/nakametpy.egg-info/
+-rw-rw-rw-   0        0        0     3043 2024-04-20 09:42:19.000000 nakametpy-2024.4.0/src/nakametpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      548 2024-04-20 09:42:19.000000 nakametpy-2024.4.0/src/nakametpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 09:42:19.000000 nakametpy-2024.4.0/src/nakametpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2024-04-20 09:42:19.000000 nakametpy-2024.4.0/src/nakametpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-20 09:42:19.000000 nakametpy-2024.4.0/src/nakametpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 09:42:19.511037 nakametpy-2024.4.0/tests/
+-rw-rw-rw-   0        0        0      316 2024-04-20 09:36:49.000000 nakametpy-2024.4.0/tests/test_thermo.py
+-rw-rw-rw-   0        0        0    18498 2024-04-20 09:36:49.000000 nakametpy-2024.4.0/tests/test_util.py
```

### Comparing `nakametpy-2024.3.0/LICENSE` & `nakametpy-2024.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.3.0/PKG-INFO` & `nakametpy-2024.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,88 +1,81 @@
 Metadata-Version: 2.1
 Name: nakametpy
-Version: 2024.3.0
+Version: 2024.4.0
 Summary: Meteorological modules for calculation and colormap.
 Home-page: https://github.com/muchojp/NakaMetPy
 Author: muchojp
 Author-email: contact.muchiwo@gmail.com
 License: BSD 3-clause
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.17.0
+Requires-Dist: numpy<=1.21.1; python_version < "3.11"
+Requires-Dist: numpy>=1.21.2; python_version >= "3.11"
 Requires-Dist: matplotlib>=3.3.0
 Requires-Dist: nose>=1.3.0
 
 # NakaMetPy
 
 [![PyPI version][pypi-image]][pypi-link]
 [![Anaconda version][anaconda-v-image]][anaconda-v-link]
-[![pytest](https://github.com/muchojp/NakaMetPy/actions/workflows/ci.yml/badge.svg)](https://github.com/muchojp/NakaMetPy/actions/workflows/ci.yml)
-<!-- [![Travis][travis-image]][travis-link] -->
+[![pytest][github-actions-image]][github-actions-link]
 
 [pypi-image]: https://badge.fury.io/py/nakametpy.svg
 [pypi-link]: https://pypi.org/project/nakametpy
 [anaconda-v-image]: https://anaconda.org/muchiwo/nakametpy/badges/version.svg
 [anaconda-v-link]: https://anaconda.org/muchiwo/nakametpy
-<!-- [travis-image]: https://travis-ci.org/muchojp/NakaMetPy.svg?branch=main
-[travis-link]: https://travis-ci.org/github/muchojp/NakaMetPy -->
 [github-actions-image]: https://github.com/muchojp/NakaMetPy/actions/workflows/ci.yml/badge.svg
 [github-actions-link]: https://github.com/muchojp/NakaMetPy/actions/workflows/ci.yml
 
 ## 概要
 このモジュールはMetPyの関数をNumPyで動作するように書き換えた関数のほか、
 観測データを扱う上で便利な関数が含まれています。
 気象データをNumPyでベクトル(配列)として扱うことを想定しています。
 
 そのため変数単位はMetPyとは異なり自分で気をつけて関数に与えなければなりません。
 また、関数の鉛直層数および時間のサイズは適当に与えています。利用される際にデータに合わせて引数を関数に渡してください。
 さらに、WRFの計算結果を入力する場合は`wrfon`のオプションを1にする必要があります。
-(`wrfon`オプションは使い勝手が悪いため、今後廃止される予定です。現在はそのための方策を考えているところです。)
+なお`wrfon`オプションは使い勝手が悪いため、今後廃止を検討中です。
 
-NakaMetPyは少なくとも2023年1月あたりまでは開発が継続される予定です。
-皆さんのContributionもお待ちしています。
+皆さまのContributionもお待ちしています。
 
 ## Abstract
 `nakametpy` is a rewrited package of `MetPy` based on `NumPy`.
 I appreciate your contribution.
 
 ## Documentation
 ドキュメンテーションは[こちら](https://muchojp.github.io/NakaMetPy/ "Docs")のページにあります。
 Documentation is [HERE](https://muchojp.github.io/NakaMetPy/).
 
 ## How to Install
 ### via Anaconda
 
 ```
-conda install -c muchiwo nakametpy
+conda install muchiwo::nakametpy
 ```
 
 ### via PyPI
 
 ```
-pip install nakametpy
+pip3 install nakametpy
 ```
 
 ## Licence
 `BSD-3-Clause`
 
 ## Citation
 ```
-Nakamura, Y. (2021). NakaMety (Version xxxx.x.x) [Software]. Fukuoka, Japan. https://github.com/muchojp/NakaMetPy
+Nakamura, Y. (2024). NakaMety (Version xxxx.x.x) [Software]. Chiba, Japan. https://github.com/muchojp/NakaMetPy
 ```
 Note: The version number xxxx.x.x should be set to the version of NakaMetPy that you are using.
 
 ## Update plans
-Next(`2022.4.0b0` or `2022.5.0` later): 
- - Refine reading GrADS binary function
+Next(`2024.x.0` or later):
+ - テストケースの追加
 
 To Do: 
  - `wrfon`オプションの廃止
  - MetPyの関数の移植 \[Further addition of MetPy function\]
  - NCLに実装されている関数の移植 \[adding the NCL's function\]
  - 方位角平均を取る関数の作成 \[Add function of Azimuthal Mean\]
 
- - ~GPU(cupy)対応 \[GPU(cupy) compatible\]~
- -> 軽い負荷の作業では GPU を利用するとかえって CPU only より遅くなることが多いため、ひとまず保留する。
-
-
```

### Comparing `nakametpy-2024.3.0/README.md` & `nakametpy-2024.4.0/src/nakametpy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,81 @@
+Metadata-Version: 2.1
+Name: nakametpy
+Version: 2024.4.0
+Summary: Meteorological modules for calculation and colormap.
+Home-page: https://github.com/muchojp/NakaMetPy
+Author: muchojp
+Author-email: contact.muchiwo@gmail.com
+License: BSD 3-clause
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy<=1.21.1; python_version < "3.11"
+Requires-Dist: numpy>=1.21.2; python_version >= "3.11"
+Requires-Dist: matplotlib>=3.3.0
+Requires-Dist: nose>=1.3.0
+
 # NakaMetPy
 
 [![PyPI version][pypi-image]][pypi-link]
 [![Anaconda version][anaconda-v-image]][anaconda-v-link]
-[![pytest](https://github.com/muchojp/NakaMetPy/actions/workflows/ci.yml/badge.svg)](https://github.com/muchojp/NakaMetPy/actions/workflows/ci.yml)
-<!-- [![Travis][travis-image]][travis-link] -->
+[![pytest][github-actions-image]][github-actions-link]
 
 [pypi-image]: https://badge.fury.io/py/nakametpy.svg
 [pypi-link]: https://pypi.org/project/nakametpy
 [anaconda-v-image]: https://anaconda.org/muchiwo/nakametpy/badges/version.svg
 [anaconda-v-link]: https://anaconda.org/muchiwo/nakametpy
-<!-- [travis-image]: https://travis-ci.org/muchojp/NakaMetPy.svg?branch=main
-[travis-link]: https://travis-ci.org/github/muchojp/NakaMetPy -->
 [github-actions-image]: https://github.com/muchojp/NakaMetPy/actions/workflows/ci.yml/badge.svg
 [github-actions-link]: https://github.com/muchojp/NakaMetPy/actions/workflows/ci.yml
 
 ## 概要
 このモジュールはMetPyの関数をNumPyで動作するように書き換えた関数のほか、
 観測データを扱う上で便利な関数が含まれています。
 気象データをNumPyでベクトル(配列)として扱うことを想定しています。
 
 そのため変数単位はMetPyとは異なり自分で気をつけて関数に与えなければなりません。
 また、関数の鉛直層数および時間のサイズは適当に与えています。利用される際にデータに合わせて引数を関数に渡してください。
 さらに、WRFの計算結果を入力する場合は`wrfon`のオプションを1にする必要があります。
-(`wrfon`オプションは使い勝手が悪いため、今後廃止される予定です。現在はそのための方策を考えているところです。)
+なお`wrfon`オプションは使い勝手が悪いため、今後廃止を検討中です。
 
-NakaMetPyは少なくとも2023年1月あたりまでは開発が継続される予定です。
-皆さんのContributionもお待ちしています。
+皆さまのContributionもお待ちしています。
 
 ## Abstract
 `nakametpy` is a rewrited package of `MetPy` based on `NumPy`.
 I appreciate your contribution.
 
 ## Documentation
 ドキュメンテーションは[こちら](https://muchojp.github.io/NakaMetPy/ "Docs")のページにあります。
 Documentation is [HERE](https://muchojp.github.io/NakaMetPy/).
 
 ## How to Install
 ### via Anaconda
 
 ```
-conda install -c muchiwo nakametpy
+conda install muchiwo::nakametpy
 ```
 
 ### via PyPI
 
 ```
-pip install nakametpy
+pip3 install nakametpy
 ```
 
 ## Licence
 `BSD-3-Clause`
 
 ## Citation
 ```
-Nakamura, Y. (2021). NakaMety (Version xxxx.x.x) [Software]. Fukuoka, Japan. https://github.com/muchojp/NakaMetPy
+Nakamura, Y. (2024). NakaMety (Version xxxx.x.x) [Software]. Chiba, Japan. https://github.com/muchojp/NakaMetPy
 ```
 Note: The version number xxxx.x.x should be set to the version of NakaMetPy that you are using.
 
 ## Update plans
-Next(`2022.4.0b0` or `2022.5.0` later): 
- - Refine reading GrADS binary function
+Next(`2024.x.0` or later):
+ - テストケースの追加
 
 To Do: 
  - `wrfon`オプションの廃止
  - MetPyの関数の移植 \[Further addition of MetPy function\]
  - NCLに実装されている関数の移植 \[adding the NCL's function\]
  - 方位角平均を取る関数の作成 \[Add function of Azimuthal Mean\]
 
- - ~GPU(cupy)対応 \[GPU(cupy) compatible\]~
- -> 軽い負荷の作業では GPU を利用するとかえって CPU only より遅くなることが多いため、ひとまず保留する。
-
-
```

### Comparing `nakametpy-2024.3.0/pyproject.toml` & `nakametpy-2024.4.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 [tool.poetry]
 name = "NakaMetPy"
-version = "2024.3.0"
+version = "2024.4.0"
 description = "Meteorological Tools for Calculation and Colormap."
 authors = ["muchojp <contact.muchiwo@mail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/muchojp/NakaMetPy"
 repository = "https://github.com/muchojp/NakaMetPy"
 documentation = "https://muchojp.github.io/NakaMetPy/"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-numpy = "^1.17.0"
-matplotlib = "^3.3.0"
-nose = "^1.3.0"
+python = ">=3.7"
+# numpy = ">=1.17.0"
+numpy = [
+  {version = ">=1.17.0,<=1.21.1", python = ">=3.6,<3.11"},
+  {version = ">=1.21.1", python = ">=3.11"}
+]
+matplotlib = ">=3.3.0"
+nose = ">=1.3.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^3.4"
+pytest = ">=6.2.5"
```

### Comparing `nakametpy-2024.3.0/setup.py` & `nakametpy-2024.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     # 'sample_lib_cli=sample_lib_cli.call:main',
 ]
 
 
 setup(
     name='nakametpy',
     python_requires='>=3.7.0',
-    version='2024.3.0',
+    version='2024.4.0',
     description='Meteorological modules for calculation and colormap.',
     # packages=packages,
     packages=find_packages('src'),
     # install_requires=install_requires,
     package_dir={"": "src"}, 
     install_requires=_requires_from_file('requirements.txt'),
     url = 'https://github.com/muchojp/NakaMetPy',
```

### Comparing `nakametpy-2024.3.0/src/nakametpy/__init__.py` & `nakametpy-2024.4.0/src/nakametpy/__init__.py`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.3.0/src/nakametpy/_error.py` & `nakametpy-2024.4.0/src/nakametpy/_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,8 +102,15 @@
         )
 
 class NotMatchTarContentNameError(MyException3):
     def __str__(self):
         return (
             f"tar ファイル {self.kargs[0]} に {self.kargs[1]} という名前のファイルはありません。名前は正しいですか?\n"+\
             f"{self.kargs[1]} was not found in tar file {self.kargs[0]} . Is the name correct?"
+        )
+
+class NotSupportedExtentionError(MyException3):
+    def __str__(self):
+        return (
+            f"この関数は拡張子{self.kargs[0]}をサポートしていません。サポートしている拡張子は{self.kargs[1]}です。\n"+\
+            f"Extention {self.kargs[0]} is not supported. Extention {self.kargs[1]} is/are suppoerted."
         )
```

### Comparing `nakametpy-2024.3.0/src/nakametpy/cmaps.py` & `nakametpy-2024.4.0/src/nakametpy/cmaps.py`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.3.0/src/nakametpy/constants.py` & `nakametpy-2024.4.0/src/nakametpy/constants.py`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.3.0/src/nakametpy/grads.py` & `nakametpy-2024.4.0/src/nakametpy/grads.py`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.3.0/src/nakametpy/jma.py` & `nakametpy-2024.4.0/src/nakametpy/jma.py`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.3.0/src/nakametpy/kinematics.py` & `nakametpy-2024.4.0/src/nakametpy/kinematics.py`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.3.0/src/nakametpy/thermo.py` & `nakametpy-2024.4.0/src/nakametpy/thermo.py`

 * *Files identical despite different names*

### Comparing `nakametpy-2024.3.0/src/nakametpy/util.py` & `nakametpy-2024.4.0/src/nakametpy/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,27 @@
-# Copyright (c) 2021, NakaMetPy Develoers.
+# Copyright (c) 2021-2024, NakaMetPy Develoers.
 # Distributed under the terms of the BSD 3-Clause License.
 # SPDX-License-Identifier: BSD-3-Clause
 # 
 # Function load_jmara_grib2 is based on Qiita article
 # URL: https://qiita.com/vpcf/items/b680f504cfe8b6a64222
 #
 
 import struct
 import tarfile
+import gzip
 import numpy as np
 from itertools import repeat
-from ._error import NotHaveSetArgError, NotMatchTarContentNameError
+from ._error import NotHaveSetArgError, NotMatchTarContentNameError, NotSupportedExtentionError
 import glob
+import logging
 
+logging.basicConfig(level=logging.INFO, format='%(levelname)s: %(message)s')
+# logging.basicConfig(level=logging.DEBUG, format='%(levelname)s: %(message)s')
+# logging.disable(logging.CRITICAL)
 
 def _set_table(section5):
   max_level = struct.unpack_from('>H', section5, 15)[0]
   table = (
     -10, # define representative of level 0　(Missing Value)
     *struct.unpack_from('>'+str(max_level)+'H', section5, 18)
   )
@@ -29,14 +34,41 @@
       pwr = 0
       yield level
     else:
       length = (0xFF - hi_level)**pwr * (raw - (hi_level + 1))
       pwr += 1
       yield from repeat(level, length)
 
+def _get_binary(file, tar_flag=False, tar_contentname=None):
+  _ext1 = file.split(sep=".")[-1]
+  logging.debug(f"_ext = {_ext1}")
+  if tar_flag:
+    _found_flag = False
+    if tar_contentname == None:
+      raise NotHaveSetArgError("tar_flag", "tar_contentname")
+    if _ext1.lower() == "tar":
+      with tarfile.open(file, mode="r") as tar:
+        for tarinfo in tar.getmembers():
+          logging.debug(f"tarinfo.name = {tarinfo.name}")
+          if tarinfo.name == tar_contentname:
+            binary = b''.join(tar.extractfile(tarinfo).readlines())
+            _found_flag = True
+            break
+    if _found_flag == False:
+      raise NotMatchTarContentNameError(file, tar_contentname)
+  elif (_ext1.lower() == "gz") or (_ext1.lower() == "gzip"):
+    with gzip.open(file, mode="rb") as gz:
+      binary = gz.read()
+  elif _ext1.lower() == "bin":
+    with open(file, 'rb') as f:
+      binary = f.read()
+  else:
+    raise NotSupportedExtentionError(_ext1, "bin, tar, gz, gzip")
+  return binary
+
 def load_jmara_grib2(file, tar_flag=False, tar_contentname=None):
   r'''気象庁解析雨量やレーダー雨量を返す関数
 
   欠損値は負の値として表現される
 
   Parameters
   --------
@@ -54,51 +86,43 @@
     Units(単位) [mm/h]
 
   Note
   -----
   ``jma_rain_lat`` , ``jma_rain_lon`` はそれぞれ返り値に対応する
   `np.ndarray` 型の緯度経度である。
   '''
-  if tar_flag:
-    _found_flag = False
-    if tar_contentname == None:
-      raise NotHaveSetArgError("tar_flag", "tar_contentname")
-    with tarfile.open(file, mode="r") as tar:
-      for tarinfo in tar.getmembers():
-        if tarinfo.name == tar_contentname:
-          binary = b''.join(tar.extractfile(tarinfo).readlines())
-          _found_flag = True
-          break
-    if _found_flag == False:
-      raise NotMatchTarContentNameError(file, tar_contentname)
-  else:
-    with open(file, 'rb') as f:
-      binary = f.read()
+  binary = _get_binary(file=file, tar_flag=tar_flag, tar_contentname=tar_contentname)
   
+  # The Sector 0, 1, 3, 4, 6 are fixed.
   len_ = {'sec0':16, 'sec1':21, 'sec3':72, 'sec4':82, 'sec6':6}
+  end1 = len_['sec0'] + len_['sec1'] - 1
+  # +31 is octet of grid numbers align latitude line.
+  nlon = struct.unpack_from('>I', binary, end1+31)[0]
+  nlat = struct.unpack_from('>I', binary, end1+35)[0]
+  logging.debug(f"nlon = {nlon}")
+  logging.debug(f"nlat = {nlat}")
   
   end4 = len_['sec0'] + len_['sec1'] + len_['sec3'] + len_['sec4'] - 1
+  # +1 is octet
   len_['sec5'] = struct.unpack_from('>I', binary, end4+1)[0]
   section5 = binary[end4:(end4+len_['sec5']+1)]
   power = section5[17]
-  # print(power)
+  logging.debug(f"power = {power}")
   
   end6 = end4 + len_['sec5'] + len_['sec6']
+  # +1 is octet
   len_['sec7'] = struct.unpack_from('>I', binary, end6+1)[0]
   section7 = binary[end6:(end6+len_['sec7']+1)]
   
   highest_level = struct.unpack_from('>H', section5, 13)[0]
   level_table = _set_table(section5)
   decoded = np.fromiter(
     _decode_runlength(section7[6:], highest_level), dtype=np.int16
   )
-  if "Gll2p5km_Phhlv_ANAL_grib2.bin" in tar_contentname:
-      decoded=decoded.reshape((1120, 1024))
-  else:
-      decoded=decoded.reshape((3360, 2560))
+  decoded=decoded.reshape((nlat, nlon))
   
   # convert level to representative
   return np.ma.masked_less((level_table[decoded]/(10**power))[::-1, :], 0)
 
 def get_jmara_lat():
   r'''解析雨量の緯度を返す関数
 
@@ -133,14 +157,35 @@
 
   Returns
   -------
   lon: `numpy.ndarray`
   '''
   return np.linspace(118, 150, 1024, endpoint=False) + 1/80 / 2
 
+def get_grib2_latlon(file, tar_flag=False, tar_contentname=None):
+  binary = _get_binary(file=file, tar_flag=tar_flag, tar_contentname=tar_contentname)
+  
+  # The Sector 0, 1, 3, 4, 6 are fixed.
+  len_ = {'sec0':16, 'sec1':21, 'sec3':72, 'sec4':82, 'sec6':6}
+  end1 = len_['sec0'] + len_['sec1'] - 1
+  # +31 is octet of grid numbers align latitude line.
+  nlon = struct.unpack_from('>I', binary, end1+31)[0]
+  nlat = struct.unpack_from('>I', binary, end1+35)[0]
+  slat = struct.unpack_from('>I', binary, end1+47)[0]
+  slon = struct.unpack_from('>I', binary, end1+51)[0]
+  elat = struct.unpack_from('>I', binary, end1+56)[0]
+  elon = struct.unpack_from('>I', binary, end1+60)[0]
+  logging.debug(f"nlon = {nlon}")
+  logging.debug(f"nlat = {nlat}")
+  logging.debug(f"slat = {slat}")
+  logging.debug(f"slon = {slon}")
+  logging.debug(f"elat = {elat}")
+  logging.debug(f"elon = {elon}")
+  return (np.linspace(slat, elat, nlat)[::-1]/1E6, np.linspace(slon, elon, nlon)/1E6)
+
 def get_gsmap_lat():
   r'''GSMaPの緯度を返す関数
 
   Returns
   -------
   lat: `numpy.ndarray`
   '''
@@ -279,16 +324,16 @@
   Parameters
   --------
   file: `str`
     file path 
     ファイルのPATH
   '''
   with tarfile.open(file, mode="r") as tar:
-      for tarinfo in tar.getmembers():
-          print(tarinfo.name)
+    for tarinfo in tar.getmembers():
+      print(tarinfo.name)
 
 def concat_array(*arr, sort=True):
   r"""
   Return concatenated array in numpy.ndarray.
 
   Parameters
   ----------
@@ -303,22 +348,26 @@
       >>> levs = concat_array(np.arange(0.5, 2., 0.5), np.arange(2., 5.1, 1.))
       >>> print(levs)
       [0.5  1.   1.5  2.   2.5  3.   3.5  4.   4.5  5. ]
 
   """
   _list = []
   for _irr in arr:
-      _list.extend(list(np.array(_irr)))
+    _list.extend(list(np.array(_irr)))
   if sort:
-      _list = sorted(list(set(_list)))
+    _list = sorted(list(set(_list)))
   return np.array(_list)
 
 def myglob(path, reverse=False):
     r"""
     Return sorted glob results.
     Parameters
     ----------
     path: `str`
     
     reverse: `bool`
+
+    Returns
+    -------
+    result_list: `list`
     """
     return sorted(glob.glob(path), reverse=reverse)
```

### Comparing `nakametpy-2024.3.0/src/nakametpy.egg-info/PKG-INFO` & `nakametpy-2024.4.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,88 +1,65 @@
-Metadata-Version: 2.1
-Name: nakametpy
-Version: 2024.3.0
-Summary: Meteorological modules for calculation and colormap.
-Home-page: https://github.com/muchojp/NakaMetPy
-Author: muchojp
-Author-email: contact.muchiwo@gmail.com
-License: BSD 3-clause
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy>=1.17.0
-Requires-Dist: matplotlib>=3.3.0
-Requires-Dist: nose>=1.3.0
-
 # NakaMetPy
 
 [![PyPI version][pypi-image]][pypi-link]
 [![Anaconda version][anaconda-v-image]][anaconda-v-link]
-[![pytest](https://github.com/muchojp/NakaMetPy/actions/workflows/ci.yml/badge.svg)](https://github.com/muchojp/NakaMetPy/actions/workflows/ci.yml)
-<!-- [![Travis][travis-image]][travis-link] -->
+[![pytest][github-actions-image]][github-actions-link]
 
 [pypi-image]: https://badge.fury.io/py/nakametpy.svg
 [pypi-link]: https://pypi.org/project/nakametpy
 [anaconda-v-image]: https://anaconda.org/muchiwo/nakametpy/badges/version.svg
 [anaconda-v-link]: https://anaconda.org/muchiwo/nakametpy
-<!-- [travis-image]: https://travis-ci.org/muchojp/NakaMetPy.svg?branch=main
-[travis-link]: https://travis-ci.org/github/muchojp/NakaMetPy -->
 [github-actions-image]: https://github.com/muchojp/NakaMetPy/actions/workflows/ci.yml/badge.svg
 [github-actions-link]: https://github.com/muchojp/NakaMetPy/actions/workflows/ci.yml
 
 ## 概要
 このモジュールはMetPyの関数をNumPyで動作するように書き換えた関数のほか、
 観測データを扱う上で便利な関数が含まれています。
 気象データをNumPyでベクトル(配列)として扱うことを想定しています。
 
 そのため変数単位はMetPyとは異なり自分で気をつけて関数に与えなければなりません。
 また、関数の鉛直層数および時間のサイズは適当に与えています。利用される際にデータに合わせて引数を関数に渡してください。
 さらに、WRFの計算結果を入力する場合は`wrfon`のオプションを1にする必要があります。
-(`wrfon`オプションは使い勝手が悪いため、今後廃止される予定です。現在はそのための方策を考えているところです。)
+なお`wrfon`オプションは使い勝手が悪いため、今後廃止を検討中です。
 
-NakaMetPyは少なくとも2023年1月あたりまでは開発が継続される予定です。
-皆さんのContributionもお待ちしています。
+皆さまのContributionもお待ちしています。
 
 ## Abstract
 `nakametpy` is a rewrited package of `MetPy` based on `NumPy`.
 I appreciate your contribution.
 
 ## Documentation
 ドキュメンテーションは[こちら](https://muchojp.github.io/NakaMetPy/ "Docs")のページにあります。
 Documentation is [HERE](https://muchojp.github.io/NakaMetPy/).
 
 ## How to Install
 ### via Anaconda
 
 ```
-conda install -c muchiwo nakametpy
+conda install muchiwo::nakametpy
 ```
 
 ### via PyPI
 
 ```
-pip install nakametpy
+pip3 install nakametpy
 ```
 
 ## Licence
 `BSD-3-Clause`
 
 ## Citation
 ```
-Nakamura, Y. (2021). NakaMety (Version xxxx.x.x) [Software]. Fukuoka, Japan. https://github.com/muchojp/NakaMetPy
+Nakamura, Y. (2024). NakaMety (Version xxxx.x.x) [Software]. Chiba, Japan. https://github.com/muchojp/NakaMetPy
 ```
 Note: The version number xxxx.x.x should be set to the version of NakaMetPy that you are using.
 
 ## Update plans
-Next(`2022.4.0b0` or `2022.5.0` later): 
- - Refine reading GrADS binary function
+Next(`2024.x.0` or later):
+ - テストケースの追加
 
 To Do: 
  - `wrfon`オプションの廃止
  - MetPyの関数の移植 \[Further addition of MetPy function\]
  - NCLに実装されている関数の移植 \[adding the NCL's function\]
  - 方位角平均を取る関数の作成 \[Add function of Azimuthal Mean\]
 
- - ~GPU(cupy)対応 \[GPU(cupy) compatible\]~
- -> 軽い負荷の作業では GPU を利用するとかえって CPU only より遅くなることが多いため、ひとまず保留する。
-
-
```

