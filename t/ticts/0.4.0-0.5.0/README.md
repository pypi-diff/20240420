# Comparing `tmp/ticts-0.4.0.tar.gz` & `tmp/ticts-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ticts-0.4.0.tar", last modified: Tue Jun 28 14:22:39 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `ticts-0.4.0.tar` & `ticts-0.5.0.tar`

### file list

```diff
@@ -1,58 +1,43 @@
-drwxr-xr-x   0 gjeusel    (501) staff       (20)        0 2022-06-28 14:22:39.229325 ticts-0.4.0/
--rw-r--r--   0 gjeusel    (501) staff       (20)      209 2022-05-30 11:20:34.000000 ticts-0.4.0/.coveragerc
--rw-r--r--   0 gjeusel    (501) staff       (20)      109 2022-05-30 11:20:34.000000 ticts-0.4.0/.isort.cfg
--rw-r--r--   0 gjeusel    (501) staff       (20)     1642 2022-05-30 11:20:34.000000 ticts-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 gjeusel    (501) staff       (20)     1521 2022-05-30 11:20:34.000000 ticts-0.4.0/.travis.yml
--rw-r--r--   0 gjeusel    (501) staff       (20)      156 2022-06-28 14:22:38.000000 ticts-0.4.0/AUTHORS
--rw-r--r--   0 gjeusel    (501) staff       (20)     3673 2022-06-28 14:22:38.000000 ticts-0.4.0/ChangeLog
--rw-r--r--   0 gjeusel    (501) staff       (20)     1067 2022-05-30 11:20:34.000000 ticts-0.4.0/LICENSE
--rw-r--r--   0 gjeusel    (501) staff       (20)     2545 2022-06-28 14:22:39.229493 ticts-0.4.0/PKG-INFO
--rw-r--r--   0 gjeusel    (501) staff       (20)     1961 2022-05-30 11:20:34.000000 ticts-0.4.0/README.rst
-drwxr-xr-x   0 gjeusel    (501) staff       (20)        0 2022-06-28 14:22:39.224482 ticts-0.4.0/docs/
--rw-r--r--   0 gjeusel    (501) staff       (20)   119475 2022-05-30 11:20:34.000000 ticts-0.4.0/docs/Tutorial.ipynb
-drwxr-xr-x   0 gjeusel    (501) staff       (20)        0 2022-06-28 14:22:39.219222 ticts-0.4.0/docs/_static/
-drwxr-xr-x   0 gjeusel    (501) staff       (20)        0 2022-06-28 14:22:39.224635 ticts-0.4.0/docs/_static/css/
--rw-r--r--   0 gjeusel    (501) staff       (20)     2164 2022-05-30 11:20:34.000000 ticts-0.4.0/docs/_static/css/custom_theme.css
-drwxr-xr-x   0 gjeusel    (501) staff       (20)        0 2022-06-28 14:22:39.225068 ticts-0.4.0/docs/_static/img/
--rw-r--r--   0 gjeusel    (501) staff       (20)    42639 2022-05-30 11:20:34.000000 ticts-0.4.0/docs/_static/img/example.png
--rw-r--r--   0 gjeusel    (501) staff       (20)     2003 2022-05-30 11:20:34.000000 ticts-0.4.0/docs/_static/img/logo.svg
--rw-r--r--   0 gjeusel    (501) staff       (20)       44 2022-05-30 11:20:34.000000 ticts-0.4.0/docs/authors.rst
--rw-r--r--   0 gjeusel    (501) staff       (20)       26 2022-05-30 11:20:34.000000 ticts-0.4.0/docs/changelog.rst
--rwxr-xr-x   0 gjeusel    (501) staff       (20)     2907 2022-05-30 11:20:34.000000 ticts-0.4.0/docs/conf.py
--rw-r--r--   0 gjeusel    (501) staff       (20)     1561 2022-05-30 11:20:34.000000 ticts-0.4.0/docs/index.rst
--rw-r--r--   0 gjeusel    (501) staff       (20)      505 2022-05-30 11:20:34.000000 ticts-0.4.0/docs/ipython_init.py
-drwxr-xr-x   0 gjeusel    (501) staff       (20)        0 2022-06-28 14:22:39.225244 ticts-0.4.0/docs/notes/
--rw-r--r--   0 gjeusel    (501) staff       (20)     1675 2022-05-30 11:20:34.000000 ticts-0.4.0/docs/notes/quickstart.rst
--rw-r--r--   0 gjeusel    (501) staff       (20)       80 2022-05-30 11:20:34.000000 ticts-0.4.0/docs/requirements.txt
-drwxr-xr-x   0 gjeusel    (501) staff       (20)        0 2022-06-28 14:22:39.225440 ticts-0.4.0/docs/src/
--rw-r--r--   0 gjeusel    (501) staff       (20)       70 2022-05-30 11:20:34.000000 ticts-0.4.0/docs/src/timeseries.rst
--rw-r--r--   0 gjeusel    (501) staff       (20)      433 2022-05-30 11:20:34.000000 ticts-0.4.0/postBuild
--rw-r--r--   0 gjeusel    (501) staff       (20)      134 2022-05-30 11:20:34.000000 ticts-0.4.0/requirements-dev.txt
--rw-r--r--   0 gjeusel    (501) staff       (20)       32 2022-05-30 11:20:34.000000 ticts-0.4.0/requirements.txt
--rw-r--r--   0 gjeusel    (501) staff       (20)     1097 2022-06-28 14:22:39.230116 ticts-0.4.0/setup.cfg
--rw-r--r--   0 gjeusel    (501) staff       (20)      199 2022-05-30 11:20:34.000000 ticts-0.4.0/setup.py
-drwxr-xr-x   0 gjeusel    (501) staff       (20)        0 2022-06-28 14:22:39.226627 ticts-0.4.0/tests/
--rw-r--r--   0 gjeusel    (501) staff       (20)        0 2022-05-30 11:20:34.000000 ticts-0.4.0/tests/__init__.py
--rwxr-xr-x   0 gjeusel    (501) staff       (20)     1206 2022-05-30 11:20:34.000000 ticts-0.4.0/tests/conftest.py
--rw-r--r--   0 gjeusel    (501) staff       (20)     1247 2022-05-30 11:20:34.000000 ticts-0.4.0/tests/test_io.py
--rw-r--r--   0 gjeusel    (501) staff       (20)      111 2022-05-30 11:20:34.000000 ticts-0.4.0/tests/test_iplot.py
--rw-r--r--   0 gjeusel    (501) staff       (20)     9600 2022-05-30 11:20:34.000000 ticts-0.4.0/tests/test_operation.py
--rw-r--r--   0 gjeusel    (501) staff       (20)     4561 2022-05-30 11:20:34.000000 ticts-0.4.0/tests/test_pandas_mixin.py
--rw-r--r--   0 gjeusel    (501) staff       (20)    20202 2022-05-30 11:20:34.000000 ticts-0.4.0/tests/test_timeseries.py
-drwxr-xr-x   0 gjeusel    (501) staff       (20)        0 2022-06-28 14:22:39.228102 ticts-0.4.0/ticts/
--rw-r--r--   0 gjeusel    (501) staff       (20)     1032 2022-05-30 11:20:34.000000 ticts-0.4.0/ticts/__init__.py
--rw-r--r--   0 gjeusel    (501) staff       (20)     1640 2022-05-30 11:20:34.000000 ticts-0.4.0/ticts/io.py
--rw-r--r--   0 gjeusel    (501) staff       (20)     1338 2022-05-30 11:20:34.000000 ticts-0.4.0/ticts/iplot.py
--rw-r--r--   0 gjeusel    (501) staff       (20)     4834 2022-05-30 11:20:34.000000 ticts-0.4.0/ticts/operation.py
--rw-r--r--   0 gjeusel    (501) staff       (20)     2103 2022-05-30 11:20:34.000000 ticts-0.4.0/ticts/pandas_mixin.py
--rw-r--r--   0 gjeusel    (501) staff       (20)      328 2022-05-30 11:20:34.000000 ticts-0.4.0/ticts/testing.py
--rw-r--r--   0 gjeusel    (501) staff       (20)    12922 2022-06-28 14:15:55.000000 ticts-0.4.0/ticts/timeseries.py
--rw-r--r--   0 gjeusel    (501) staff       (20)      655 2022-05-30 11:20:34.000000 ticts-0.4.0/ticts/utils.py
-drwxr-xr-x   0 gjeusel    (501) staff       (20)        0 2022-06-28 14:22:39.229203 ticts-0.4.0/ticts.egg-info/
--rw-r--r--   0 gjeusel    (501) staff       (20)     2545 2022-06-28 14:22:38.000000 ticts-0.4.0/ticts.egg-info/PKG-INFO
--rw-r--r--   0 gjeusel    (501) staff       (20)      911 2022-06-28 14:22:39.000000 ticts-0.4.0/ticts.egg-info/SOURCES.txt
--rw-r--r--   0 gjeusel    (501) staff       (20)        1 2022-06-28 14:22:38.000000 ticts-0.4.0/ticts.egg-info/dependency_links.txt
--rw-r--r--   0 gjeusel    (501) staff       (20)        1 2022-06-28 14:15:13.000000 ticts-0.4.0/ticts.egg-info/not-zip-safe
--rw-r--r--   0 gjeusel    (501) staff       (20)       47 2022-06-28 14:22:39.000000 ticts-0.4.0/ticts.egg-info/pbr.json
--rw-r--r--   0 gjeusel    (501) staff       (20)       32 2022-06-28 14:22:38.000000 ticts-0.4.0/ticts.egg-info/requires.txt
--rw-r--r--   0 gjeusel    (501) staff       (20)        6 2022-06-28 14:22:38.000000 ticts-0.4.0/ticts.egg-info/top_level.txt
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 ticts-0.5.0/.cruft.json
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ticts-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 ticts-0.5.0/Makefile
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 ticts-0.5.0/mkdocs.yml
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 ticts-0.5.0/.binder/postBuild
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 ticts-0.5.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ticts-0.5.0/.github/dependabot.yml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 ticts-0.5.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 ticts-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 ticts-0.5.0/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 ticts-0.5.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 ticts-0.5.0/.github/workflows/smokeshow.yml
+-rw-r--r--   0        0        0   133393 2020-02-02 00:00:00.000000 ticts-0.5.0/docs/Tutorial.ipynb
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ticts-0.5.0/docs/abbreviations.md
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 ticts-0.5.0/docs/changelog.md
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 ticts-0.5.0/docs/index.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ticts-0.5.0/docs/reference.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 ticts-0.5.0/docs/css/custom.css
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 ticts-0.5.0/docs/css/termynal.css
+-rw-r--r--   0        0        0    42639 2020-02-02 00:00:00.000000 ticts-0.5.0/docs/img/example.png
+-rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 ticts-0.5.0/docs/img/favicon.ico
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 ticts-0.5.0/docs/img/logo.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ticts-0.5.0/docs/js/custom.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ticts-0.5.0/tests/__init__.py
+-rwxr-xr-x   0        0        0     1202 2020-02-02 00:00:00.000000 ticts-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 ticts-0.5.0/tests/test_io.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 ticts-0.5.0/tests/test_iplot.py
+-rw-r--r--   0        0        0     9837 2020-02-02 00:00:00.000000 ticts-0.5.0/tests/test_operation.py
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 ticts-0.5.0/tests/test_pandas_mixin.py
+-rw-r--r--   0        0        0    19863 2020-02-02 00:00:00.000000 ticts-0.5.0/tests/test_timeseries.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 ticts-0.5.0/ticts/__init__.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 ticts-0.5.0/ticts/io.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 ticts-0.5.0/ticts/iplot.py
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 ticts-0.5.0/ticts/operation.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 ticts-0.5.0/ticts/pandas_mixin.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 ticts-0.5.0/ticts/testing.py
+-rw-r--r--   0        0        0    12780 2020-02-02 00:00:00.000000 ticts-0.5.0/ticts/timeseries.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ticts-0.5.0/ticts/utils.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 ticts-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 ticts-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 ticts-0.5.0/README.md
+-rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 ticts-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4250 2020-02-02 00:00:00.000000 ticts-0.5.0/PKG-INFO
```

### Comparing `ticts-0.4.0/LICENSE` & `ticts-0.5.0/LICENSE`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-
 MIT License
 
-Copyright (c) 2019, gjeusel
+Copyright (c) 2024 gjeusel
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+The above copyright notice and this permission notice (including the next paragraph) shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
+
```

### Comparing `ticts-0.4.0/docs/Tutorial.ipynb` & `ticts-0.5.0/docs/Tutorial.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8565064594937128%*

 * *Differences: {"'cells'": "{2: {'execution_count': 1, 'outputs': {0: {'data': {'text/html': ['    <style>\\n', "*

 * *            "'        .bk-notebook-logo {\\n', '            display: block;\\n', '            "*

 * *            "width: 20px;\\n', '            height: 20px;\\n', '            background-image: "*

 * *            "url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABQAAAAUCAYAAACNiR0NAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAALEgAACxIB0t1+/AAAABx0RVh0U29mdHdhcmUAQWRvYmUgRmlyZXdvcmtzIENTNui8sowAAAOkSURBVDiNjZRtaJVlGMd/1/08zzln5z […]*

```diff
@@ -25,136 +25,149 @@
                 "- ensure timezone localization.\n",
                 "\n",
                 "Let's see the potential !"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "\n",
-                            "    <div class=\"bk-root\">\n",
-                            "        <a href=\"https://bokeh.pydata.org\" target=\"_blank\" class=\"bk-logo bk-logo-small bk-logo-notebook\"></a>\n",
-                            "        <span id=\"4187\">Loading BokehJS ...</span>\n",
-                            "    </div>"
+                            "    <style>\n",
+                            "        .bk-notebook-logo {\n",
+                            "            display: block;\n",
+                            "            width: 20px;\n",
+                            "            height: 20px;\n",
+                            "            background-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABQAAAAUCAYAAACNiR0NAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAALEgAACxIB0t1+/AAAABx0RVh0U29mdHdhcmUAQWRvYmUgRmlyZXdvcmtzIENTNui8sowAAAOkSURBVDiNjZRtaJVlGMd/1/08zzln5zjP1LWcU9N0NkN8m2CYjpgQYQXqSs0I84OLIC0hkEKoPtiH3gmKoiJDU7QpLgoLjLIQCpEsNJ1vqUOdO7ppbuec5+V+rj4ctwzd8IIbbi6u+8f1539dt3A78eXC7QizUF7gyV1fD1Yqg4JWz84yffhm0qkFqBogB9rM8tZdtwVsPUhWhGcFJngGeWrPzHm5oaMmkfEg1usvLFyc8jLRqDOMru7AyC8saQr7GG7f5fvDeH7Ej8CM66nIF+8yngt6HWaKh7k49Soy9nXurCi1o3qUbS3zWfrYeQDTB/Qj6kX6Ybhw4B+bOYoLKCC9H3Nu/leUTZ1JdRWkkn2ldcCamzrcf47KKXdAJllSlxAOkRgyHsGC/zRday5Qld9DyoM4/q/rUoy/CXh3jzOu3bHUVZeU+DEn8FInkPBFlu3+nW3Nw0mk6vCDiWg8CeJaxEwuHS3+z5RgY+YBR6V1Z1nxSOfoaPa4LASWxxdNp+VWTk7+4vzaou8v8PN+xo+KY2xsw6une2frhw05CTYOmQvsEhjhWjn0bmXPjpE1+kplmmkP3suftwTubK9Vq22qKmrBhpY4jvd5afdRA3wGjFAgcnTK2s4hY0/GPNIb0nErGMCRxWOOX64Z8RAC4oCXdklmEvcL8o0BfkNK4lUg9HTl+oPlQxdNo3Mg4Nv175e/1LDGzZen30MEjRUtmXSfiTVu1kK8W4txyV6BMKlbgk3lMwYCiusNy9fVfvvwMxv8Ynl6vxoByANLTWplvuj/nF9m2+PDtt1eiHPBr1oIfhCChQMBw6Aw0UulqTKZdfVvfG7VcfIqLG9bcldL/+pdWTLxLUy8Qq38heUIjh4XlzZxzQm19lLFlr8vdQ97rjZVOLf8nclzckbcD4wxXMidpX30sFd37Fv/GtwwhzhxGVAprjbg0gCAEeIgwCZyTV2Z1REEW8O4py0wsjeloKoMr6iCY6dP92H6Vw/oTyICIthibxjm/DfN9lVz8IqtqKYLUXfoKVMVQVVJOElGjrnnUt9T9wbgp8AyYKaGlqingHZU/uG2NTZSVqwHQTWkx9hxjkpWDaCg6Ckj5qebgBVbT3V3NNXMSiWSDdGV3hrtzla7J+duwPOToIg42ChPQOQjspnSlp1V+Gjdged7+8UN5CRAV7a5EdFNwCjEaBR27b3W890TE7g24NAP/mMDXRWrGoFPQI9ls/MWO2dWFAar/xcOIImbbpA3zgAAAABJRU5ErkJggg==);\n",
+                            "        }\n",
+                            "    </style>\n",
+                            "    <div>\n",
+                            "        <a href=\"https://bokeh.org\" target=\"_blank\" class=\"bk-notebook-logo\"></a>\n",
+                            "        <span id=\"f289b1ce-44e4-4f31-9076-bda2262f9dba\">Loading BokehJS ...</span>\n",
+                            "    </div>\n"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/javascript": [
-                            "\n",
+                            "'use strict';\n",
                             "(function(root) {\n",
                             "  function now() {\n",
                             "    return new Date();\n",
                             "  }\n",
                             "\n",
-                            "  var force = true;\n",
+                            "  const force = true;\n",
                             "\n",
                             "  if (typeof root._bokeh_onload_callbacks === \"undefined\" || force === true) {\n",
                             "    root._bokeh_onload_callbacks = [];\n",
                             "    root._bokeh_is_loading = undefined;\n",
                             "  }\n",
                             "\n",
-                            "  var JS_MIME_TYPE = 'application/javascript';\n",
-                            "  var HTML_MIME_TYPE = 'text/html';\n",
-                            "  var EXEC_MIME_TYPE = 'application/vnd.bokehjs_exec.v0+json';\n",
-                            "  var CLASS_NAME = 'output_bokeh rendered_html';\n",
+                            "const JS_MIME_TYPE = 'application/javascript';\n",
+                            "  const HTML_MIME_TYPE = 'text/html';\n",
+                            "  const EXEC_MIME_TYPE = 'application/vnd.bokehjs_exec.v0+json';\n",
+                            "  const CLASS_NAME = 'output_bokeh rendered_html';\n",
                             "\n",
                             "  /**\n",
                             "   * Render data to the DOM node\n",
                             "   */\n",
                             "  function render(props, node) {\n",
-                            "    var script = document.createElement(\"script\");\n",
+                            "    const script = document.createElement(\"script\");\n",
                             "    node.appendChild(script);\n",
                             "  }\n",
                             "\n",
                             "  /**\n",
                             "   * Handle when an output is cleared or removed\n",
                             "   */\n",
                             "  function handleClearOutput(event, handle) {\n",
-                            "    var cell = handle.cell;\n",
+                            "    function drop(id) {\n",
+                            "      const view = Bokeh.index.get_by_id(id)\n",
+                            "      if (view != null) {\n",
+                            "        view.model.document.clear()\n",
+                            "        Bokeh.index.delete(view)\n",
+                            "      }\n",
+                            "    }\n",
+                            "\n",
+                            "    const cell = handle.cell;\n",
+                            "\n",
+                            "    const id = cell.output_area._bokeh_element_id;\n",
+                            "    const server_id = cell.output_area._bokeh_server_id;\n",
                             "\n",
-                            "    var id = cell.output_area._bokeh_element_id;\n",
-                            "    var server_id = cell.output_area._bokeh_server_id;\n",
                             "    // Clean up Bokeh references\n",
-                            "    if (id != null && id in Bokeh.index) {\n",
-                            "      Bokeh.index[id].model.document.clear();\n",
-                            "      delete Bokeh.index[id];\n",
+                            "    if (id != null) {\n",
+                            "      drop(id)\n",
                             "    }\n",
                             "\n",
                             "    if (server_id !== undefined) {\n",
                             "      // Clean up Bokeh references\n",
-                            "      var cmd = \"from bokeh.io.state import curstate; print(curstate().uuid_to_server['\" + server_id + \"'].get_sessions()[0].document.roots[0]._id)\";\n",
-                            "      cell.notebook.kernel.execute(cmd, {\n",
+                            "      const cmd_clean = \"from bokeh.io.state import curstate; print(curstate().uuid_to_server['\" + server_id + \"'].get_sessions()[0].document.roots[0]._id)\";\n",
+                            "      cell.notebook.kernel.execute(cmd_clean, {\n",
                             "        iopub: {\n",
                             "          output: function(msg) {\n",
-                            "            var id = msg.content.text.trim();\n",
-                            "            if (id in Bokeh.index) {\n",
-                            "              Bokeh.index[id].model.document.clear();\n",
-                            "              delete Bokeh.index[id];\n",
-                            "            }\n",
+                            "            const id = msg.content.text.trim()\n",
+                            "            drop(id)\n",
                             "          }\n",
                             "        }\n",
                             "      });\n",
                             "      // Destroy server and session\n",
-                            "      var cmd = \"import bokeh.io.notebook as ion; ion.destroy_server('\" + server_id + \"')\";\n",
-                            "      cell.notebook.kernel.execute(cmd);\n",
+                            "      const cmd_destroy = \"import bokeh.io.notebook as ion; ion.destroy_server('\" + server_id + \"')\";\n",
+                            "      cell.notebook.kernel.execute(cmd_destroy);\n",
                             "    }\n",
                             "  }\n",
                             "\n",
                             "  /**\n",
                             "   * Handle when a new output is added\n",
                             "   */\n",
                             "  function handleAddOutput(event, handle) {\n",
-                            "    var output_area = handle.output_area;\n",
-                            "    var output = handle.output;\n",
+                            "    const output_area = handle.output_area;\n",
+                            "    const output = handle.output;\n",
                             "\n",
                             "    // limit handleAddOutput to display_data with EXEC_MIME_TYPE content only\n",
-                            "    if ((output.output_type != \"display_data\") || (!output.data.hasOwnProperty(EXEC_MIME_TYPE))) {\n",
+                            "    if ((output.output_type != \"display_data\") || (!Object.prototype.hasOwnProperty.call(output.data, EXEC_MIME_TYPE))) {\n",
                             "      return\n",
                             "    }\n",
                             "\n",
-                            "    var toinsert = output_area.element.find(\".\" + CLASS_NAME.split(' ')[0]);\n",
+                            "    const toinsert = output_area.element.find(\".\" + CLASS_NAME.split(' ')[0]);\n",
                             "\n",
                             "    if (output.metadata[EXEC_MIME_TYPE][\"id\"] !== undefined) {\n",
                             "      toinsert[toinsert.length - 1].firstChild.textContent = output.data[JS_MIME_TYPE];\n",
                             "      // store reference to embed id on output_area\n",
                             "      output_area._bokeh_element_id = output.metadata[EXEC_MIME_TYPE][\"id\"];\n",
                             "    }\n",
                             "    if (output.metadata[EXEC_MIME_TYPE][\"server_id\"] !== undefined) {\n",
-                            "      var bk_div = document.createElement(\"div\");\n",
+                            "      const bk_div = document.createElement(\"div\");\n",
                             "      bk_div.innerHTML = output.data[HTML_MIME_TYPE];\n",
-                            "      var script_attrs = bk_div.children[0].attributes;\n",
-                            "      for (var i = 0; i < script_attrs.length; i++) {\n",
+                            "      const script_attrs = bk_div.children[0].attributes;\n",
+                            "      for (let i = 0; i < script_attrs.length; i++) {\n",
                             "        toinsert[toinsert.length - 1].firstChild.setAttribute(script_attrs[i].name, script_attrs[i].value);\n",
+                            "        toinsert[toinsert.length - 1].firstChild.textContent = bk_div.children[0].textContent\n",
                             "      }\n",
                             "      // store reference to server id on output_area\n",
                             "      output_area._bokeh_server_id = output.metadata[EXEC_MIME_TYPE][\"server_id\"];\n",
                             "    }\n",
                             "  }\n",
                             "\n",
                             "  function register_renderer(events, OutputArea) {\n",
                             "\n",
                             "    function append_mime(data, metadata, element) {\n",
                             "      // create a DOM node to render to\n",
-                            "      var toinsert = this.create_output_subarea(\n",
+                            "      const toinsert = this.create_output_subarea(\n",
                             "        metadata,\n",
                             "        CLASS_NAME,\n",
                             "        EXEC_MIME_TYPE\n",
                             "      );\n",
                             "      this.keyboard_manager.register_events(toinsert);\n",
                             "      // Render to node\n",
-                            "      var props = {data: data, metadata: metadata[EXEC_MIME_TYPE]};\n",
+                            "      const props = {data: data, metadata: metadata[EXEC_MIME_TYPE]};\n",
                             "      render(props, toinsert[toinsert.length - 1]);\n",
                             "      element.append(toinsert);\n",
                             "      return toinsert\n",
                             "    }\n",
                             "\n",
                             "    /* Handle when an output is cleared or removed */\n",
                             "    events.on('clear_output.CodeCell', handleClearOutput);\n",
@@ -172,29 +185,27 @@
                             "      /* Index of renderer in `output_area.display_order` */\n",
                             "      index: 0\n",
                             "    });\n",
                             "  }\n",
                             "\n",
                             "  // register the mime type if in Jupyter Notebook environment and previously unregistered\n",
                             "  if (root.Jupyter !== undefined) {\n",
-                            "    var events = require('base/js/events');\n",
-                            "    var OutputArea = require('notebook/js/outputarea').OutputArea;\n",
+                            "    const events = require('base/js/events');\n",
+                            "    const OutputArea = require('notebook/js/outputarea').OutputArea;\n",
                             "\n",
                             "    if (OutputArea.prototype.mime_types().indexOf(EXEC_MIME_TYPE) == -1) {\n",
                             "      register_renderer(events, OutputArea);\n",
                             "    }\n",
                             "  }\n",
-                            "\n",
-                            "  \n",
                             "  if (typeof (root._bokeh_timeout) === \"undefined\" || force === true) {\n",
                             "    root._bokeh_timeout = Date.now() + 5000;\n",
                             "    root._bokeh_failed_load = false;\n",
                             "  }\n",
                             "\n",
-                            "  var NB_LOAD_WARNING = {'data': {'text/html':\n",
+                            "  const NB_LOAD_WARNING = {'data': {'text/html':\n",
                             "     \"<div style='background-color: #fdd'>\\n\"+\n",
                             "     \"<p>\\n\"+\n",
                             "     \"BokehJS does not appear to have successfully loaded. If loading BokehJS from CDN, this \\n\"+\n",
                             "     \"may be due to a slow or bad network connection. Possible fixes:\\n\"+\n",
                             "     \"</p>\\n\"+\n",
                             "     \"<ul>\\n\"+\n",
                             "     \"<li>re-rerun `output_notebook()` to attempt to load from CDN again, or</li>\\n\"+\n",
@@ -202,29 +213,53 @@
                             "     \"</ul>\\n\"+\n",
                             "     \"<code>\\n\"+\n",
                             "     \"from bokeh.resources import INLINE\\n\"+\n",
                             "     \"output_notebook(resources=INLINE)\\n\"+\n",
                             "     \"</code>\\n\"+\n",
                             "     \"</div>\"}};\n",
                             "\n",
-                            "  function display_loaded() {\n",
-                            "    var el = document.getElementById(\"4187\");\n",
+                            "  function display_loaded(error = null) {\n",
+                            "    const el = document.getElementById(\"f289b1ce-44e4-4f31-9076-bda2262f9dba\");\n",
                             "    if (el != null) {\n",
-                            "      el.textContent = \"BokehJS is loading...\";\n",
-                            "    }\n",
-                            "    if (root.Bokeh !== undefined) {\n",
-                            "      if (el != null) {\n",
-                            "        el.textContent = \"BokehJS \" + root.Bokeh.version + \" successfully loaded.\";\n",
+                            "      const html = (() => {\n",
+                            "        if (typeof root.Bokeh === \"undefined\") {\n",
+                            "          if (error == null) {\n",
+                            "            return \"BokehJS is loading ...\";\n",
+                            "          } else {\n",
+                            "            return \"BokehJS failed to load.\";\n",
+                            "          }\n",
+                            "        } else {\n",
+                            "          const prefix = `BokehJS ${root.Bokeh.version}`;\n",
+                            "          if (error == null) {\n",
+                            "            return `${prefix} successfully loaded.`;\n",
+                            "          } else {\n",
+                            "            return `${prefix} <b>encountered errors</b> while loading and may not function as expected.`;\n",
+                            "          }\n",
+                            "        }\n",
+                            "      })();\n",
+                            "      el.innerHTML = html;\n",
+                            "\n",
+                            "      if (error != null) {\n",
+                            "        const wrapper = document.createElement(\"div\");\n",
+                            "        wrapper.style.overflow = \"auto\";\n",
+                            "        wrapper.style.height = \"5em\";\n",
+                            "        wrapper.style.resize = \"vertical\";\n",
+                            "        const content = document.createElement(\"div\");\n",
+                            "        content.style.fontFamily = \"monospace\";\n",
+                            "        content.style.whiteSpace = \"pre-wrap\";\n",
+                            "        content.style.backgroundColor = \"rgb(255, 221, 221)\";\n",
+                            "        content.textContent = error.stack ?? error.toString();\n",
+                            "        wrapper.append(content);\n",
+                            "        el.append(wrapper);\n",
                             "      }\n",
                             "    } else if (Date.now() < root._bokeh_timeout) {\n",
-                            "      setTimeout(display_loaded, 100)\n",
+                            "      setTimeout(() => display_loaded(error), 100);\n",
                             "    }\n",
                             "  }\n",
                             "\n",
-                            "\n",
                             "  function run_callbacks() {\n",
                             "    try {\n",
                             "      root._bokeh_onload_callbacks.forEach(function(callback) {\n",
                             "        if (callback != null)\n",
                             "          callback();\n",
                             "      });\n",
                             "    } finally {\n",
@@ -253,97 +288,91 @@
                             "      root._bokeh_is_loading--;\n",
                             "      if (root._bokeh_is_loading === 0) {\n",
                             "        console.debug(\"Bokeh: all BokehJS libraries/stylesheets loaded\");\n",
                             "        run_callbacks()\n",
                             "      }\n",
                             "    }\n",
                             "\n",
-                            "    function on_error() {\n",
+                            "    function on_error(url) {\n",
                             "      console.error(\"failed to load \" + url);\n",
                             "    }\n",
                             "\n",
-                            "    for (var i = 0; i < css_urls.length; i++) {\n",
-                            "      var url = css_urls[i];\n",
+                            "    for (let i = 0; i < css_urls.length; i++) {\n",
+                            "      const url = css_urls[i];\n",
                             "      const element = document.createElement(\"link\");\n",
                             "      element.onload = on_load;\n",
-                            "      element.onerror = on_error;\n",
+                            "      element.onerror = on_error.bind(null, url);\n",
                             "      element.rel = \"stylesheet\";\n",
                             "      element.type = \"text/css\";\n",
                             "      element.href = url;\n",
                             "      console.debug(\"Bokeh: injecting link tag for BokehJS stylesheet: \", url);\n",
                             "      document.body.appendChild(element);\n",
                             "    }\n",
                             "\n",
-                            "    for (var i = 0; i < js_urls.length; i++) {\n",
-                            "      var url = js_urls[i];\n",
-                            "      var element = document.createElement('script');\n",
+                            "    for (let i = 0; i < js_urls.length; i++) {\n",
+                            "      const url = js_urls[i];\n",
+                            "      const element = document.createElement('script');\n",
                             "      element.onload = on_load;\n",
-                            "      element.onerror = on_error;\n",
+                            "      element.onerror = on_error.bind(null, url);\n",
                             "      element.async = false;\n",
                             "      element.src = url;\n",
                             "      console.debug(\"Bokeh: injecting script tag for BokehJS library: \", url);\n",
                             "      document.head.appendChild(element);\n",
                             "    }\n",
-                            "  };var element = document.getElementById(\"4187\");\n",
-                            "  if (element == null) {\n",
-                            "    console.error(\"Bokeh: ERROR: autoload.js configured with elementid '4187' but no matching script tag was found. \")\n",
-                            "    return false;\n",
-                            "  }\n",
+                            "  };\n",
                             "\n",
                             "  function inject_raw_css(css) {\n",
                             "    const element = document.createElement(\"style\");\n",
                             "    element.appendChild(document.createTextNode(css));\n",
                             "    document.body.appendChild(element);\n",
                             "  }\n",
                             "\n",
-                            "  var js_urls = [\"https://cdn.pydata.org/bokeh/release/bokeh-1.3.1.min.js\", \"https://cdn.pydata.org/bokeh/release/bokeh-widgets-1.3.1.min.js\", \"https://cdn.pydata.org/bokeh/release/bokeh-tables-1.3.1.min.js\", \"https://cdn.pydata.org/bokeh/release/bokeh-gl-1.3.1.min.js\"];\n",
-                            "  var css_urls = [];\n",
+                            "  const js_urls = [\"https://cdn.bokeh.org/bokeh/release/bokeh-3.4.1.min.js\", \"https://cdn.bokeh.org/bokeh/release/bokeh-gl-3.4.1.min.js\", \"https://cdn.bokeh.org/bokeh/release/bokeh-widgets-3.4.1.min.js\", \"https://cdn.bokeh.org/bokeh/release/bokeh-tables-3.4.1.min.js\", \"https://cdn.bokeh.org/bokeh/release/bokeh-mathjax-3.4.1.min.js\"];\n",
+                            "  const css_urls = [];\n",
                             "\n",
-                            "  var inline_js = [\n",
-                            "    function(Bokeh) {\n",
+                            "  const inline_js = [    function(Bokeh) {\n",
                             "      Bokeh.set_log_level(\"info\");\n",
                             "    },\n",
-                            "    \n",
-                            "    function(Bokeh) {\n",
-                            "      \n",
-                            "    },\n",
-                            "    function(Bokeh) {} // ensure no trailing comma for IE\n",
+                            "function(Bokeh) {\n",
+                            "    }\n",
                             "  ];\n",
                             "\n",
                             "  function run_inline_js() {\n",
-                            "    \n",
-                            "    if ((root.Bokeh !== undefined) || (force === true)) {\n",
-                            "      for (var i = 0; i < inline_js.length; i++) {\n",
-                            "        inline_js[i].call(root, root.Bokeh);\n",
+                            "    if (root.Bokeh !== undefined || force === true) {\n",
+                            "      try {\n",
+                            "            for (let i = 0; i < inline_js.length; i++) {\n",
+                            "      inline_js[i].call(root, root.Bokeh);\n",
+                            "    }\n",
+                            "\n",
+                            "      } catch (error) {display_loaded(error);throw error;\n",
                             "      }if (force === true) {\n",
                             "        display_loaded();\n",
                             "      }} else if (Date.now() < root._bokeh_timeout) {\n",
                             "      setTimeout(run_inline_js, 100);\n",
                             "    } else if (!root._bokeh_failed_load) {\n",
                             "      console.log(\"Bokeh: BokehJS failed to load within specified timeout.\");\n",
                             "      root._bokeh_failed_load = true;\n",
                             "    } else if (force !== true) {\n",
-                            "      var cell = $(document.getElementById(\"4187\")).parents('.cell').data().cell;\n",
+                            "      const cell = $(document.getElementById(\"f289b1ce-44e4-4f31-9076-bda2262f9dba\")).parents('.cell').data().cell;\n",
                             "      cell.output_area.append_execute_result(NB_LOAD_WARNING)\n",
                             "    }\n",
-                            "\n",
                             "  }\n",
                             "\n",
                             "  if (root._bokeh_is_loading === 0) {\n",
                             "    console.debug(\"Bokeh: BokehJS loaded, going straight to plotting\");\n",
                             "    run_inline_js();\n",
                             "  } else {\n",
                             "    load_libs(css_urls, js_urls, function() {\n",
                             "      console.debug(\"Bokeh: BokehJS plotting callback run at\", now());\n",
                             "      run_inline_js();\n",
                             "    });\n",
                             "  }\n",
                             "}(window));"
                         ],
-                        "application/vnd.bokehjs_load.v0+json": "\n(function(root) {\n  function now() {\n    return new Date();\n  }\n\n  var force = true;\n\n  if (typeof root._bokeh_onload_callbacks === \"undefined\" || force === true) {\n    root._bokeh_onload_callbacks = [];\n    root._bokeh_is_loading = undefined;\n  }\n\n  \n\n  \n  if (typeof (root._bokeh_timeout) === \"undefined\" || force === true) {\n    root._bokeh_timeout = Date.now() + 5000;\n    root._bokeh_failed_load = false;\n  }\n\n  var NB_LOAD_WARNING = {'data': {'text/html':\n     \"<div style='background-color: #fdd'>\\n\"+\n     \"<p>\\n\"+\n     \"BokehJS does not appear to have successfully loaded. If loading BokehJS from CDN, this \\n\"+\n     \"may be due to a slow or bad network connection. Possible fixes:\\n\"+\n     \"</p>\\n\"+\n     \"<ul>\\n\"+\n     \"<li>re-rerun `output_notebook()` to attempt to load from CDN again, or</li>\\n\"+\n     \"<li>use INLINE resources instead, as so:</li>\\n\"+\n     \"</ul>\\n\"+\n     \"<code>\\n\"+\n     \"from bokeh.resources import INLINE\\n\"+\n     \"output_notebook(resources=INLINE)\\n\"+\n     \"</code>\\n\"+\n     \"</div>\"}};\n\n  function display_loaded() {\n    var el = document.getElementById(\"4187\");\n    if (el != null) {\n      el.textContent = \"BokehJS is loading...\";\n    }\n    if (root.Bokeh !== undefined) {\n      if (el != null) {\n        el.textContent = \"BokehJS \" + root.Bokeh.version + \" successfully loaded.\";\n      }\n    } else if (Date.now() < root._bokeh_timeout) {\n      setTimeout(display_loaded, 100)\n    }\n  }\n\n\n  function run_callbacks() {\n    try {\n      root._bokeh_onload_callbacks.forEach(function(callback) {\n        if (callback != null)\n          callback();\n      });\n    } finally {\n      delete root._bokeh_onload_callbacks\n    }\n    console.debug(\"Bokeh: all callbacks have finished\");\n  }\n\n  function load_libs(css_urls, js_urls, callback) {\n    if (css_urls == null) css_urls = [];\n    if (js_urls == null) js_urls = [];\n\n    root._bokeh_onload_callbacks.push(callback);\n    if (root._bokeh_is_loading > 0) {\n      console.debug(\"Bokeh: BokehJS is being loaded, scheduling callback at\", now());\n      return null;\n    }\n    if (js_urls == null || js_urls.length === 0) {\n      run_callbacks();\n      return null;\n    }\n    console.debug(\"Bokeh: BokehJS not loaded, scheduling load and callback at\", now());\n    root._bokeh_is_loading = css_urls.length + js_urls.length;\n\n    function on_load() {\n      root._bokeh_is_loading--;\n      if (root._bokeh_is_loading === 0) {\n        console.debug(\"Bokeh: all BokehJS libraries/stylesheets loaded\");\n        run_callbacks()\n      }\n    }\n\n    function on_error() {\n      console.error(\"failed to load \" + url);\n    }\n\n    for (var i = 0; i < css_urls.length; i++) {\n      var url = css_urls[i];\n      const element = document.createElement(\"link\");\n      element.onload = on_load;\n      element.onerror = on_error;\n      element.rel = \"stylesheet\";\n      element.type = \"text/css\";\n      element.href = url;\n      console.debug(\"Bokeh: injecting link tag for BokehJS stylesheet: \", url);\n      document.body.appendChild(element);\n    }\n\n    for (var i = 0; i < js_urls.length; i++) {\n      var url = js_urls[i];\n      var element = document.createElement('script');\n      element.onload = on_load;\n      element.onerror = on_error;\n      element.async = false;\n      element.src = url;\n      console.debug(\"Bokeh: injecting script tag for BokehJS library: \", url);\n      document.head.appendChild(element);\n    }\n  };var element = document.getElementById(\"4187\");\n  if (element == null) {\n    console.error(\"Bokeh: ERROR: autoload.js configured with elementid '4187' but no matching script tag was found. \")\n    return false;\n  }\n\n  function inject_raw_css(css) {\n    const element = document.createElement(\"style\");\n    element.appendChild(document.createTextNode(css));\n    document.body.appendChild(element);\n  }\n\n  var js_urls = [\"https://cdn.pydata.org/bokeh/release/bokeh-1.3.1.min.js\", \"https://cdn.pydata.org/bokeh/release/bokeh-widgets-1.3.1.min.js\", \"https://cdn.pydata.org/bokeh/release/bokeh-tables-1.3.1.min.js\", \"https://cdn.pydata.org/bokeh/release/bokeh-gl-1.3.1.min.js\"];\n  var css_urls = [];\n\n  var inline_js = [\n    function(Bokeh) {\n      Bokeh.set_log_level(\"info\");\n    },\n    \n    function(Bokeh) {\n      \n    },\n    function(Bokeh) {} // ensure no trailing comma for IE\n  ];\n\n  function run_inline_js() {\n    \n    if ((root.Bokeh !== undefined) || (force === true)) {\n      for (var i = 0; i < inline_js.length; i++) {\n        inline_js[i].call(root, root.Bokeh);\n      }if (force === true) {\n        display_loaded();\n      }} else if (Date.now() < root._bokeh_timeout) {\n      setTimeout(run_inline_js, 100);\n    } else if (!root._bokeh_failed_load) {\n      console.log(\"Bokeh: BokehJS failed to load within specified timeout.\");\n      root._bokeh_failed_load = true;\n    } else if (force !== true) {\n      var cell = $(document.getElementById(\"4187\")).parents('.cell').data().cell;\n      cell.output_area.append_execute_result(NB_LOAD_WARNING)\n    }\n\n  }\n\n  if (root._bokeh_is_loading === 0) {\n    console.debug(\"Bokeh: BokehJS loaded, going straight to plotting\");\n    run_inline_js();\n  } else {\n    load_libs(css_urls, js_urls, function() {\n      console.debug(\"Bokeh: BokehJS plotting callback run at\", now());\n      run_inline_js();\n    });\n  }\n}(window));"
+                        "application/vnd.bokehjs_load.v0+json": "'use strict';\n(function(root) {\n  function now() {\n    return new Date();\n  }\n\n  const force = true;\n\n  if (typeof root._bokeh_onload_callbacks === \"undefined\" || force === true) {\n    root._bokeh_onload_callbacks = [];\n    root._bokeh_is_loading = undefined;\n  }\n\n\n  if (typeof (root._bokeh_timeout) === \"undefined\" || force === true) {\n    root._bokeh_timeout = Date.now() + 5000;\n    root._bokeh_failed_load = false;\n  }\n\n  const NB_LOAD_WARNING = {'data': {'text/html':\n     \"<div style='background-color: #fdd'>\\n\"+\n     \"<p>\\n\"+\n     \"BokehJS does not appear to have successfully loaded. If loading BokehJS from CDN, this \\n\"+\n     \"may be due to a slow or bad network connection. Possible fixes:\\n\"+\n     \"</p>\\n\"+\n     \"<ul>\\n\"+\n     \"<li>re-rerun `output_notebook()` to attempt to load from CDN again, or</li>\\n\"+\n     \"<li>use INLINE resources instead, as so:</li>\\n\"+\n     \"</ul>\\n\"+\n     \"<code>\\n\"+\n     \"from bokeh.resources import INLINE\\n\"+\n     \"output_notebook(resources=INLINE)\\n\"+\n     \"</code>\\n\"+\n     \"</div>\"}};\n\n  function display_loaded(error = null) {\n    const el = document.getElementById(\"f289b1ce-44e4-4f31-9076-bda2262f9dba\");\n    if (el != null) {\n      const html = (() => {\n        if (typeof root.Bokeh === \"undefined\") {\n          if (error == null) {\n            return \"BokehJS is loading ...\";\n          } else {\n            return \"BokehJS failed to load.\";\n          }\n        } else {\n          const prefix = `BokehJS ${root.Bokeh.version}`;\n          if (error == null) {\n            return `${prefix} successfully loaded.`;\n          } else {\n            return `${prefix} <b>encountered errors</b> while loading and may not function as expected.`;\n          }\n        }\n      })();\n      el.innerHTML = html;\n\n      if (error != null) {\n        const wrapper = document.createElement(\"div\");\n        wrapper.style.overflow = \"auto\";\n        wrapper.style.height = \"5em\";\n        wrapper.style.resize = \"vertical\";\n        const content = document.createElement(\"div\");\n        content.style.fontFamily = \"monospace\";\n        content.style.whiteSpace = \"pre-wrap\";\n        content.style.backgroundColor = \"rgb(255, 221, 221)\";\n        content.textContent = error.stack ?? error.toString();\n        wrapper.append(content);\n        el.append(wrapper);\n      }\n    } else if (Date.now() < root._bokeh_timeout) {\n      setTimeout(() => display_loaded(error), 100);\n    }\n  }\n\n  function run_callbacks() {\n    try {\n      root._bokeh_onload_callbacks.forEach(function(callback) {\n        if (callback != null)\n          callback();\n      });\n    } finally {\n      delete root._bokeh_onload_callbacks\n    }\n    console.debug(\"Bokeh: all callbacks have finished\");\n  }\n\n  function load_libs(css_urls, js_urls, callback) {\n    if (css_urls == null) css_urls = [];\n    if (js_urls == null) js_urls = [];\n\n    root._bokeh_onload_callbacks.push(callback);\n    if (root._bokeh_is_loading > 0) {\n      console.debug(\"Bokeh: BokehJS is being loaded, scheduling callback at\", now());\n      return null;\n    }\n    if (js_urls == null || js_urls.length === 0) {\n      run_callbacks();\n      return null;\n    }\n    console.debug(\"Bokeh: BokehJS not loaded, scheduling load and callback at\", now());\n    root._bokeh_is_loading = css_urls.length + js_urls.length;\n\n    function on_load() {\n      root._bokeh_is_loading--;\n      if (root._bokeh_is_loading === 0) {\n        console.debug(\"Bokeh: all BokehJS libraries/stylesheets loaded\");\n        run_callbacks()\n      }\n    }\n\n    function on_error(url) {\n      console.error(\"failed to load \" + url);\n    }\n\n    for (let i = 0; i < css_urls.length; i++) {\n      const url = css_urls[i];\n      const element = document.createElement(\"link\");\n      element.onload = on_load;\n      element.onerror = on_error.bind(null, url);\n      element.rel = \"stylesheet\";\n      element.type = \"text/css\";\n      element.href = url;\n      console.debug(\"Bokeh: injecting link tag for BokehJS stylesheet: \", url);\n      document.body.appendChild(element);\n    }\n\n    for (let i = 0; i < js_urls.length; i++) {\n      const url = js_urls[i];\n      const element = document.createElement('script');\n      element.onload = on_load;\n      element.onerror = on_error.bind(null, url);\n      element.async = false;\n      element.src = url;\n      console.debug(\"Bokeh: injecting script tag for BokehJS library: \", url);\n      document.head.appendChild(element);\n    }\n  };\n\n  function inject_raw_css(css) {\n    const element = document.createElement(\"style\");\n    element.appendChild(document.createTextNode(css));\n    document.body.appendChild(element);\n  }\n\n  const js_urls = [\"https://cdn.bokeh.org/bokeh/release/bokeh-3.4.1.min.js\", \"https://cdn.bokeh.org/bokeh/release/bokeh-gl-3.4.1.min.js\", \"https://cdn.bokeh.org/bokeh/release/bokeh-widgets-3.4.1.min.js\", \"https://cdn.bokeh.org/bokeh/release/bokeh-tables-3.4.1.min.js\", \"https://cdn.bokeh.org/bokeh/release/bokeh-mathjax-3.4.1.min.js\"];\n  const css_urls = [];\n\n  const inline_js = [    function(Bokeh) {\n      Bokeh.set_log_level(\"info\");\n    },\nfunction(Bokeh) {\n    }\n  ];\n\n  function run_inline_js() {\n    if (root.Bokeh !== undefined || force === true) {\n      try {\n            for (let i = 0; i < inline_js.length; i++) {\n      inline_js[i].call(root, root.Bokeh);\n    }\n\n      } catch (error) {display_loaded(error);throw error;\n      }if (force === true) {\n        display_loaded();\n      }} else if (Date.now() < root._bokeh_timeout) {\n      setTimeout(run_inline_js, 100);\n    } else if (!root._bokeh_failed_load) {\n      console.log(\"Bokeh: BokehJS failed to load within specified timeout.\");\n      root._bokeh_failed_load = true;\n    } else if (force !== true) {\n      const cell = $(document.getElementById(\"f289b1ce-44e4-4f31-9076-bda2262f9dba\")).parents('.cell').data().cell;\n      cell.output_area.append_execute_result(NB_LOAD_WARNING)\n    }\n  }\n\n  if (root._bokeh_is_loading === 0) {\n    console.debug(\"Bokeh: BokehJS loaded, going straight to plotting\");\n    run_inline_js();\n  } else {\n    load_libs(css_urls, js_urls, function() {\n      console.debug(\"Bokeh: BokehJS plotting callback run at\", now());\n      run_inline_js();\n    });\n  }\n}(window));"
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "from ticts import TimeSeries\n",
@@ -361,151 +390,154 @@
             "source": [
                 "## Overview\n",
                 "-----"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 27,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
                 "dct = {\n",
                 "  '2019-01-01': 10,\n",
                 "  '2019-01-01 00:10:00': 20,\n",
                 "  '2019-01-01 00:15:00': 10,\n",
                 "}\n",
                 "ts = TimeSeries(dct)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "<TimeSeries>\n",
-                        "2019-01-01T00:00:00+00:00: 10,\n",
-                        "2019-01-01T00:10:00+00:00: 20,\n",
-                        "2019-01-01T00:15:00+00:00: 10,\n"
-                    ]
+                    "data": {
+                        "text/html": [
+                            "<pre style=\"white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace\"><span style=\"font-weight: bold\">&lt;</span><span style=\"color: #ff00ff; text-decoration-color: #ff00ff; font-weight: bold\">TimeSeries</span><span style=\"font-weight: bold\">&gt;</span>\n",
+                            "<span style=\"color: #800080; text-decoration-color: #800080\">2019</span>-<span style=\"color: #800080; text-decoration-color: #800080\">01</span>-01T<span style=\"color: #00ff00; text-decoration-color: #00ff00; font-weight: bold\">00:00:00</span>+<span style=\"color: #00ff00; text-decoration-color: #00ff00; font-weight: bold\">00:00</span>: <span style=\"color: #800080; text-decoration-color: #800080\">10</span>,\n",
+                            "<span style=\"color: #800080; text-decoration-color: #800080\">2019</span>-<span style=\"color: #800080; text-decoration-color: #800080\">01</span>-01T<span style=\"color: #00ff00; text-decoration-color: #00ff00; font-weight: bold\">00:10:00</span>+<span style=\"color: #00ff00; text-decoration-color: #00ff00; font-weight: bold\">00:00</span>: <span style=\"color: #800080; text-decoration-color: #800080\">20</span>,\n",
+                            "<span style=\"color: #800080; text-decoration-color: #800080\">2019</span>-<span style=\"color: #800080; text-decoration-color: #800080\">01</span>-01T<span style=\"color: #00ff00; text-decoration-color: #00ff00; font-weight: bold\">00:15:00</span>+<span style=\"color: #00ff00; text-decoration-color: #00ff00; font-weight: bold\">00:00</span>: <span style=\"color: #800080; text-decoration-color: #800080\">10</span>,\n",
+                            "</pre>\n"
+                        ],
+                        "text/plain": [
+                            "\u001b[1m<\u001b[0m\u001b[1;95mTimeSeries\u001b[0m\u001b[1m>\u001b[0m\n",
+                            "\u001b[35m2019\u001b[0m-\u001b[35m01\u001b[0m-01T\u001b[1;92m00:00:00\u001b[0m+\u001b[1;92m00:00\u001b[0m: \u001b[35m10\u001b[0m,\n",
+                            "\u001b[35m2019\u001b[0m-\u001b[35m01\u001b[0m-01T\u001b[1;92m00:10:00\u001b[0m+\u001b[1;92m00:00\u001b[0m: \u001b[35m20\u001b[0m,\n",
+                            "\u001b[35m2019\u001b[0m-\u001b[35m01\u001b[0m-01T\u001b[1;92m00:15:00\u001b[0m+\u001b[1;92m00:00\u001b[0m: \u001b[35m10\u001b[0m,\n"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
                 }
             ],
             "source": [
                 "# Let's see it:\n",
                 "print(ts)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "\n",
-                            "\n",
-                            "\n",
-                            "\n",
-                            "\n",
-                            "\n",
-                            "  <div class=\"bk-root\" id=\"6d6ba3f3-17f9-4014-b289-2880b1c95389\" data-root-id=\"4188\"></div>\n"
+                            "  <div id=\"a7a692fc-231b-4f31-99dd-a2ce200de572\" data-root-id=\"p1001\" style=\"display: contents;\"></div>\n"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/javascript": [
                             "(function(root) {\n",
                             "  function embed_document(root) {\n",
-                            "    \n",
-                            "  var docs_json = {\"29e3fb21-5984-4de9-b335-d36c8a606364\":{\"roots\":{\"references\":[{\"attributes\":{\"below\":[{\"id\":\"4199\",\"type\":\"DatetimeAxis\"}],\"center\":[{\"id\":\"4203\",\"type\":\"Grid\"},{\"id\":\"4208\",\"type\":\"Grid\"}],\"left\":[{\"id\":\"4204\",\"type\":\"LinearAxis\"}],\"plot_height\":220,\"plot_width\":400,\"renderers\":[{\"id\":\"4225\",\"type\":\"GlyphRenderer\"},{\"id\":\"4230\",\"type\":\"GlyphRenderer\"}],\"title\":{\"id\":\"4189\",\"type\":\"Title\"},\"toolbar\":{\"id\":\"4215\",\"type\":\"Toolbar\"},\"x_range\":{\"id\":\"4191\",\"type\":\"DataRange1d\"},\"x_scale\":{\"id\":\"4195\",\"type\":\"LinearScale\"},\"y_range\":{\"id\":\"4193\",\"type\":\"DataRange1d\"},\"y_scale\":{\"id\":\"4197\",\"type\":\"LinearScale\"}},\"id\":\"4188\",\"subtype\":\"Figure\",\"type\":\"Plot\"},{\"attributes\":{\"active_drag\":\"auto\",\"active_inspect\":\"auto\",\"active_multi\":null,\"active_scroll\":\"auto\",\"active_tap\":\"auto\",\"tools\":[{\"id\":\"4209\",\"type\":\"PanTool\"},{\"id\":\"4210\",\"type\":\"WheelZoomTool\"},{\"id\":\"4211\",\"type\":\"BoxZoomTool\"},{\"id\":\"4212\",\"type\":\"SaveTool\"},{\"id\":\"4213\",\"type\":\"ResetTool\"},{\"id\":\"4214\",\"type\":\"HelpTool\"}]},\"id\":\"4215\",\"type\":\"Toolbar\"},{\"attributes\":{\"source\":{\"id\":\"4222\",\"type\":\"ColumnDataSource\"}},\"id\":\"4226\",\"type\":\"CDSView\"},{\"attributes\":{},\"id\":\"4494\",\"type\":\"Selection\"},{\"attributes\":{},\"id\":\"4209\",\"type\":\"PanTool\"},{\"attributes\":{\"base\":24,\"mantissas\":[1,2,4,6,8,12],\"max_interval\":43200000.0,\"min_interval\":3600000.0,\"num_minor_ticks\":0},\"id\":\"4481\",\"type\":\"AdaptiveTicker\"},{\"attributes\":{},\"id\":\"4195\",\"type\":\"LinearScale\"},{\"attributes\":{\"source\":{\"id\":\"4227\",\"type\":\"ColumnDataSource\"}},\"id\":\"4231\",\"type\":\"CDSView\"},{\"attributes\":{\"days\":[1,15]},\"id\":\"4485\",\"type\":\"DaysTicker\"},{\"attributes\":{\"dimension\":1,\"ticker\":{\"id\":\"4205\",\"type\":\"BasicTicker\"}},\"id\":\"4208\",\"type\":\"Grid\"},{\"attributes\":{\"text\":\"value\"},\"id\":\"4189\",\"type\":\"Title\"},{\"attributes\":{\"fill_color\":{\"value\":\"red\"},\"line_color\":{\"value\":\"#1f77b4\"},\"size\":{\"units\":\"screen\",\"value\":6},\"x\":{\"field\":\"x\"},\"y\":{\"field\":\"y\"}},\"id\":\"4228\",\"type\":\"Circle\"},{\"attributes\":{},\"id\":\"4490\",\"type\":\"YearsTicker\"},{\"attributes\":{\"data_source\":{\"id\":\"4222\",\"type\":\"ColumnDataSource\"},\"glyph\":{\"id\":\"4223\",\"type\":\"Step\"},\"hover_glyph\":null,\"muted_glyph\":null,\"nonselection_glyph\":{\"id\":\"4224\",\"type\":\"Step\"},\"selection_glyph\":null,\"view\":{\"id\":\"4226\",\"type\":\"CDSView\"}},\"id\":\"4225\",\"type\":\"GlyphRenderer\"},{\"attributes\":{},\"id\":\"4197\",\"type\":\"LinearScale\"},{\"attributes\":{\"days\":[1,4,7,10,13,16,19,22,25,28]},\"id\":\"4483\",\"type\":\"DaysTicker\"},{\"attributes\":{\"months\":[0,6]},\"id\":\"4489\",\"type\":\"MonthsTicker\"},{\"attributes\":{\"base\":60,\"mantissas\":[1,2,5,10,15,20,30],\"max_interval\":1800000.0,\"min_interval\":1000.0,\"num_minor_ticks\":0},\"id\":\"4480\",\"type\":\"AdaptiveTicker\"},{\"attributes\":{\"data_source\":{\"id\":\"4227\",\"type\":\"ColumnDataSource\"},\"glyph\":{\"id\":\"4228\",\"type\":\"Circle\"},\"hover_glyph\":null,\"muted_glyph\":null,\"nonselection_glyph\":{\"id\":\"4229\",\"type\":\"Circle\"},\"selection_glyph\":null,\"view\":{\"id\":\"4231\",\"type\":\"CDSView\"}},\"id\":\"4230\",\"type\":\"GlyphRenderer\"},{\"attributes\":{\"line_alpha\":{\"value\":0.1},\"line_color\":{\"value\":\"#1f77b4\"},\"line_dash\":[4,4],\"line_width\":{\"value\":2},\"mode\":\"after\",\"x\":{\"field\":\"x\"},\"y\":{\"field\":\"y\"}},\"id\":\"4224\",\"type\":\"Step\"},{\"attributes\":{\"mantissas\":[1,2,5],\"max_interval\":500.0,\"num_minor_ticks\":0},\"id\":\"4479\",\"type\":\"AdaptiveTicker\"},{\"attributes\":{},\"id\":\"4491\",\"type\":\"UnionRenderers\"},{\"attributes\":{},\"id\":\"4477\",\"type\":\"BasicTickFormatter\"},{\"attributes\":{},\"id\":\"4213\",\"type\":\"ResetTool\"},{\"attributes\":{\"callback\":null},\"id\":\"4191\",\"type\":\"DataRange1d\"},{\"attributes\":{\"num_minor_ticks\":5,\"tickers\":[{\"id\":\"4479\",\"type\":\"AdaptiveTicker\"},{\"id\":\"4480\",\"type\":\"AdaptiveTicker\"},{\"id\":\"4481\",\"type\":\"AdaptiveTicker\"},{\"id\":\"4482\",\"type\":\"DaysTicker\"},{\"id\":\"4483\",\"type\":\"DaysTicker\"},{\"id\":\"4484\",\"type\":\"DaysTicker\"},{\"id\":\"4485\",\"type\":\"DaysTicker\"},{\"id\":\"4486\",\"type\":\"MonthsTicker\"},{\"id\":\"4487\",\"type\":\"MonthsTicker\"},{\"id\":\"4488\",\"type\":\"MonthsTicker\"},{\"id\":\"4489\",\"type\":\"MonthsTicker\"},{\"id\":\"4490\",\"type\":\"YearsTicker\"}]},\"id\":\"4200\",\"type\":\"DatetimeTicker\"},{\"attributes\":{\"months\":[0,2,4,6,8,10]},\"id\":\"4487\",\"type\":\"MonthsTicker\"},{\"attributes\":{\"days\":[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31]},\"id\":\"4482\",\"type\":\"DaysTicker\"},{\"attributes\":{},\"id\":\"4492\",\"type\":\"Selection\"},{\"attributes\":{\"ticker\":{\"id\":\"4200\",\"type\":\"DatetimeTicker\"}},\"id\":\"4203\",\"type\":\"Grid\"},{\"attributes\":{\"callback\":null,\"data\":{\"x\":[1546300800000.0,1546301400000.0,1546301700000.0],\"y\":[10,20,10]},\"selected\":{\"id\":\"4494\",\"type\":\"Selection\"},\"selection_policy\":{\"id\":\"4493\",\"type\":\"UnionRenderers\"}},\"id\":\"4227\",\"type\":\"ColumnDataSource\"},{\"attributes\":{},\"id\":\"4475\",\"type\":\"DatetimeTickFormatter\"},{\"attributes\":{\"callback\":null},\"id\":\"4193\",\"type\":\"DataRange1d\"},{\"attributes\":{\"bottom_units\":\"screen\",\"fill_alpha\":{\"value\":0.5},\"fill_color\":{\"value\":\"lightgrey\"},\"left_units\":\"screen\",\"level\":\"overlay\",\"line_alpha\":{\"value\":1.0},\"line_color\":{\"value\":\"black\"},\"line_dash\":[4,4],\"line_width\":{\"value\":2},\"render_mode\":\"css\",\"right_units\":\"screen\",\"top_units\":\"screen\"},\"id\":\"4495\",\"type\":\"BoxAnnotation\"},{\"attributes\":{},\"id\":\"4212\",\"type\":\"SaveTool\"},{\"attributes\":{\"formatter\":{\"id\":\"4477\",\"type\":\"BasicTickFormatter\"},\"ticker\":{\"id\":\"4205\",\"type\":\"BasicTicker\"}},\"id\":\"4204\",\"type\":\"LinearAxis\"},{\"attributes\":{\"fill_alpha\":{\"value\":0.1},\"fill_color\":{\"value\":\"#1f77b4\"},\"line_alpha\":{\"value\":0.1},\"line_color\":{\"value\":\"#1f77b4\"},\"size\":{\"units\":\"screen\",\"value\":6},\"x\":{\"field\":\"x\"},\"y\":{\"field\":\"y\"}},\"id\":\"4229\",\"type\":\"Circle\"},{\"attributes\":{},\"id\":\"4214\",\"type\":\"HelpTool\"},{\"attributes\":{\"months\":[0,4,8]},\"id\":\"4488\",\"type\":\"MonthsTicker\"},{\"attributes\":{},\"id\":\"4205\",\"type\":\"BasicTicker\"},{\"attributes\":{},\"id\":\"4493\",\"type\":\"UnionRenderers\"},{\"attributes\":{\"months\":[0,1,2,3,4,5,6,7,8,9,10,11]},\"id\":\"4486\",\"type\":\"MonthsTicker\"},{\"attributes\":{\"overlay\":{\"id\":\"4495\",\"type\":\"BoxAnnotation\"}},\"id\":\"4211\",\"type\":\"BoxZoomTool\"},{\"attributes\":{\"days\":[1,8,15,22]},\"id\":\"4484\",\"type\":\"DaysTicker\"},{\"attributes\":{\"callback\":null,\"data\":{\"x\":[1546300800000.0,1546301400000.0,1546301700000.0],\"y\":[10,20,10]},\"selected\":{\"id\":\"4492\",\"type\":\"Selection\"},\"selection_policy\":{\"id\":\"4491\",\"type\":\"UnionRenderers\"}},\"id\":\"4222\",\"type\":\"ColumnDataSource\"},{\"attributes\":{\"axis_label\":\"timestamp\",\"formatter\":{\"id\":\"4475\",\"type\":\"DatetimeTickFormatter\"},\"ticker\":{\"id\":\"4200\",\"type\":\"DatetimeTicker\"}},\"id\":\"4199\",\"type\":\"DatetimeAxis\"},{\"attributes\":{},\"id\":\"4210\",\"type\":\"WheelZoomTool\"},{\"attributes\":{\"line_color\":{\"value\":\"#1f77b4\"},\"line_dash\":[4,4],\"line_width\":{\"value\":2},\"mode\":\"after\",\"x\":{\"field\":\"x\"},\"y\":{\"field\":\"y\"}},\"id\":\"4223\",\"type\":\"Step\"}],\"root_ids\":[\"4188\"]},\"title\":\"Bokeh Application\",\"version\":\"1.3.1\"}};\n",
-                            "  var render_items = [{\"docid\":\"29e3fb21-5984-4de9-b335-d36c8a606364\",\"roots\":{\"4188\":\"6d6ba3f3-17f9-4014-b289-2880b1c95389\"}}];\n",
-                            "  root.Bokeh.embed.embed_items_notebook(docs_json, render_items);\n",
-                            "\n",
+                            "  const docs_json = {\"ee38bb15-9a94-4e8f-82c6-91c66c75f5be\":{\"version\":\"3.4.1\",\"title\":\"Bokeh Application\",\"roots\":[{\"type\":\"object\",\"name\":\"Figure\",\"id\":\"p1001\",\"attributes\":{\"width\":400,\"height\":220,\"x_range\":{\"type\":\"object\",\"name\":\"DataRange1d\",\"id\":\"p1002\"},\"y_range\":{\"type\":\"object\",\"name\":\"DataRange1d\",\"id\":\"p1003\"},\"x_scale\":{\"type\":\"object\",\"name\":\"LinearScale\",\"id\":\"p1011\"},\"y_scale\":{\"type\":\"object\",\"name\":\"LinearScale\",\"id\":\"p1012\"},\"title\":{\"type\":\"object\",\"name\":\"Title\",\"id\":\"p1004\",\"attributes\":{\"text\":\"value\"}},\"renderers\":[{\"type\":\"object\",\"name\":\"GlyphRenderer\",\"id\":\"p1052\",\"attributes\":{\"data_source\":{\"type\":\"object\",\"name\":\"ColumnDataSource\",\"id\":\"p1046\",\"attributes\":{\"selected\":{\"type\":\"object\",\"name\":\"Selection\",\"id\":\"p1047\",\"attributes\":{\"indices\":[],\"line_indices\":[]}},\"selection_policy\":{\"type\":\"object\",\"name\":\"UnionRenderers\",\"id\":\"p1048\"},\"data\":{\"type\":\"map\",\"entries\":[[\"x\",[1546300800000.0,1546301400000.0,1546301700000.0]],[\"y\",[10,20,10]]]}}},\"view\":{\"type\":\"object\",\"name\":\"CDSView\",\"id\":\"p1053\",\"attributes\":{\"filter\":{\"type\":\"object\",\"name\":\"AllIndices\",\"id\":\"p1054\"}}},\"glyph\":{\"type\":\"object\",\"name\":\"Step\",\"id\":\"p1049\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"line_color\":\"#1f77b4\",\"line_width\":2,\"line_dash\":[4,4],\"mode\":\"after\"}},\"nonselection_glyph\":{\"type\":\"object\",\"name\":\"Step\",\"id\":\"p1050\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"line_color\":\"#1f77b4\",\"line_alpha\":0.1,\"line_width\":2,\"line_dash\":[4,4],\"mode\":\"after\"}},\"muted_glyph\":{\"type\":\"object\",\"name\":\"Step\",\"id\":\"p1051\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"line_color\":\"#1f77b4\",\"line_alpha\":0.2,\"line_width\":2,\"line_dash\":[4,4],\"mode\":\"after\"}}}},{\"type\":\"object\",\"name\":\"GlyphRenderer\",\"id\":\"p1061\",\"attributes\":{\"data_source\":{\"type\":\"object\",\"name\":\"ColumnDataSource\",\"id\":\"p1055\",\"attributes\":{\"selected\":{\"type\":\"object\",\"name\":\"Selection\",\"id\":\"p1056\",\"attributes\":{\"indices\":[],\"line_indices\":[]}},\"selection_policy\":{\"type\":\"object\",\"name\":\"UnionRenderers\",\"id\":\"p1057\"},\"data\":{\"type\":\"map\",\"entries\":[[\"x\",[1546300800000.0,1546301400000.0,1546301700000.0]],[\"y\",[10,20,10]]]}}},\"view\":{\"type\":\"object\",\"name\":\"CDSView\",\"id\":\"p1062\",\"attributes\":{\"filter\":{\"type\":\"object\",\"name\":\"AllIndices\",\"id\":\"p1063\"}}},\"glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1058\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"size\":{\"type\":\"value\",\"value\":6},\"line_color\":{\"type\":\"value\",\"value\":\"#1f77b4\"},\"fill_color\":{\"type\":\"value\",\"value\":\"red\"}}},\"nonselection_glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1059\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"size\":{\"type\":\"value\",\"value\":6},\"line_color\":{\"type\":\"value\",\"value\":\"#1f77b4\"},\"line_alpha\":{\"type\":\"value\",\"value\":0.1},\"fill_color\":{\"type\":\"value\",\"value\":\"red\"},\"fill_alpha\":{\"type\":\"value\",\"value\":0.1},\"hatch_alpha\":{\"type\":\"value\",\"value\":0.1}}},\"muted_glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1060\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"size\":{\"type\":\"value\",\"value\":6},\"line_color\":{\"type\":\"value\",\"value\":\"#1f77b4\"},\"line_alpha\":{\"type\":\"value\",\"value\":0.2},\"fill_color\":{\"type\":\"value\",\"value\":\"red\"},\"fill_alpha\":{\"type\":\"value\",\"value\":0.2},\"hatch_alpha\":{\"type\":\"value\",\"value\":0.2}}}}}],\"toolbar\":{\"type\":\"object\",\"name\":\"Toolbar\",\"id\":\"p1010\",\"attributes\":{\"tools\":[{\"type\":\"object\",\"name\":\"PanTool\",\"id\":\"p1035\"},{\"type\":\"object\",\"name\":\"WheelZoomTool\",\"id\":\"p1036\",\"attributes\":{\"renderers\":\"auto\"}},{\"type\":\"object\",\"name\":\"BoxZoomTool\",\"id\":\"p1037\",\"attributes\":{\"overlay\":{\"type\":\"object\",\"name\":\"BoxAnnotation\",\"id\":\"p1038\",\"attributes\":{\"syncable\":false,\"level\":\"overlay\",\"visible\":false,\"left\":{\"type\":\"number\",\"value\":\"nan\"},\"right\":{\"type\":\"number\",\"value\":\"nan\"},\"top\":{\"type\":\"number\",\"value\":\"nan\"},\"bottom\":{\"type\":\"number\",\"value\":\"nan\"},\"left_units\":\"canvas\",\"right_units\":\"canvas\",\"top_units\":\"canvas\",\"bottom_units\":\"canvas\",\"line_color\":\"black\",\"line_alpha\":1.0,\"line_width\":2,\"line_dash\":[4,4],\"fill_color\":\"lightgrey\",\"fill_alpha\":0.5}}}},{\"type\":\"object\",\"name\":\"SaveTool\",\"id\":\"p1043\"},{\"type\":\"object\",\"name\":\"ResetTool\",\"id\":\"p1044\"},{\"type\":\"object\",\"name\":\"HelpTool\",\"id\":\"p1045\"}]}},\"left\":[{\"type\":\"object\",\"name\":\"LinearAxis\",\"id\":\"p1030\",\"attributes\":{\"ticker\":{\"type\":\"object\",\"name\":\"BasicTicker\",\"id\":\"p1031\",\"attributes\":{\"mantissas\":[1,2,5]}},\"formatter\":{\"type\":\"object\",\"name\":\"BasicTickFormatter\",\"id\":\"p1032\"},\"major_label_policy\":{\"type\":\"object\",\"name\":\"AllLabels\",\"id\":\"p1033\"}}}],\"below\":[{\"type\":\"object\",\"name\":\"DatetimeAxis\",\"id\":\"p1013\",\"attributes\":{\"ticker\":{\"type\":\"object\",\"name\":\"DatetimeTicker\",\"id\":\"p1014\",\"attributes\":{\"num_minor_ticks\":5,\"tickers\":[{\"type\":\"object\",\"name\":\"AdaptiveTicker\",\"id\":\"p1015\",\"attributes\":{\"num_minor_ticks\":0,\"mantissas\":[1,2,5],\"max_interval\":500.0}},{\"type\":\"object\",\"name\":\"AdaptiveTicker\",\"id\":\"p1016\",\"attributes\":{\"num_minor_ticks\":0,\"base\":60,\"mantissas\":[1,2,5,10,15,20,30],\"min_interval\":1000.0,\"max_interval\":1800000.0}},{\"type\":\"object\",\"name\":\"AdaptiveTicker\",\"id\":\"p1017\",\"attributes\":{\"num_minor_ticks\":0,\"base\":24,\"mantissas\":[1,2,4,6,8,12],\"min_interval\":3600000.0,\"max_interval\":43200000.0}},{\"type\":\"object\",\"name\":\"DaysTicker\",\"id\":\"p1018\",\"attributes\":{\"days\":[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31]}},{\"type\":\"object\",\"name\":\"DaysTicker\",\"id\":\"p1019\",\"attributes\":{\"days\":[1,4,7,10,13,16,19,22,25,28]}},{\"type\":\"object\",\"name\":\"DaysTicker\",\"id\":\"p1020\",\"attributes\":{\"days\":[1,8,15,22]}},{\"type\":\"object\",\"name\":\"DaysTicker\",\"id\":\"p1021\",\"attributes\":{\"days\":[1,15]}},{\"type\":\"object\",\"name\":\"MonthsTicker\",\"id\":\"p1022\",\"attributes\":{\"months\":[0,1,2,3,4,5,6,7,8,9,10,11]}},{\"type\":\"object\",\"name\":\"MonthsTicker\",\"id\":\"p1023\",\"attributes\":{\"months\":[0,2,4,6,8,10]}},{\"type\":\"object\",\"name\":\"MonthsTicker\",\"id\":\"p1024\",\"attributes\":{\"months\":[0,4,8]}},{\"type\":\"object\",\"name\":\"MonthsTicker\",\"id\":\"p1025\",\"attributes\":{\"months\":[0,6]}},{\"type\":\"object\",\"name\":\"YearsTicker\",\"id\":\"p1026\"}]}},\"formatter\":{\"type\":\"object\",\"name\":\"DatetimeTickFormatter\",\"id\":\"p1027\"},\"axis_label\":\"timestamp\",\"major_label_policy\":{\"type\":\"object\",\"name\":\"AllLabels\",\"id\":\"p1028\"}}}],\"center\":[{\"type\":\"object\",\"name\":\"Grid\",\"id\":\"p1029\",\"attributes\":{\"axis\":{\"id\":\"p1013\"}}},{\"type\":\"object\",\"name\":\"Grid\",\"id\":\"p1034\",\"attributes\":{\"dimension\":1,\"axis\":{\"id\":\"p1030\"}}}]}}]}};\n",
+                            "  const render_items = [{\"docid\":\"ee38bb15-9a94-4e8f-82c6-91c66c75f5be\",\"roots\":{\"p1001\":\"a7a692fc-231b-4f31-99dd-a2ce200de572\"},\"root_ids\":[\"p1001\"]}];\n",
+                            "  void root.Bokeh.embed.embed_items_notebook(docs_json, render_items);\n",
                             "  }\n",
                             "  if (root.Bokeh !== undefined) {\n",
                             "    embed_document(root);\n",
                             "  } else {\n",
-                            "    var attempts = 0;\n",
-                            "    var timer = setInterval(function(root) {\n",
+                            "    let attempts = 0;\n",
+                            "    const timer = setInterval(function(root) {\n",
                             "      if (root.Bokeh !== undefined) {\n",
-                            "        embed_document(root);\n",
-                            "        clearInterval(timer);\n",
-                            "      }\n",
-                            "      attempts++;\n",
-                            "      if (attempts > 100) {\n",
-                            "        console.log(\"Bokeh: ERROR: Unable to run BokehJS code because BokehJS library is missing\");\n",
                             "        clearInterval(timer);\n",
+                            "        embed_document(root);\n",
+                            "      } else {\n",
+                            "        attempts++;\n",
+                            "        if (attempts > 100) {\n",
+                            "          clearInterval(timer);\n",
+                            "          console.log(\"Bokeh: ERROR: Unable to run BokehJS code because BokehJS library is missing\");\n",
+                            "        }\n",
                             "      }\n",
                             "    }, 10, root)\n",
                             "  }\n",
                             "})(window);"
                         ],
                         "application/vnd.bokehjs_exec.v0+json": ""
                     },
                     "metadata": {
                         "application/vnd.bokehjs_exec.v0+json": {
-                            "id": "4188"
+                            "id": "p1001"
                         }
                     },
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"display: table;\"><div style=\"display: table-row;\"><div style=\"display: table-cell;\"><b title=\"bokeh.plotting.figure.Figure\">Figure</b>(</div><div style=\"display: table-cell;\">id&nbsp;=&nbsp;'4188', <span id=\"4629\" style=\"cursor: pointer;\">&hellip;)</span></div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">above&nbsp;=&nbsp;[],</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">align&nbsp;=&nbsp;'start',</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">aspect_ratio&nbsp;=&nbsp;None,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">aspect_scale&nbsp;=&nbsp;1,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">background&nbsp;=&nbsp;None,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">background_fill_alpha&nbsp;=&nbsp;{'value': 1.0},</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">background_fill_color&nbsp;=&nbsp;{'value': '#ffffff'},</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">below&nbsp;=&nbsp;[DatetimeAxis(id='4199', ...)],</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">border_fill_alpha&nbsp;=&nbsp;{'value': 1.0},</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">border_fill_color&nbsp;=&nbsp;{'value': '#ffffff'},</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">center&nbsp;=&nbsp;[Grid(id='4203', ...), Grid(id='4208', ...)],</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">css_classes&nbsp;=&nbsp;[],</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">disabled&nbsp;=&nbsp;False,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">extra_x_ranges&nbsp;=&nbsp;{},</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">extra_y_ranges&nbsp;=&nbsp;{},</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">frame_height&nbsp;=&nbsp;None,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">frame_width&nbsp;=&nbsp;None,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">height&nbsp;=&nbsp;None,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">height_policy&nbsp;=&nbsp;'auto',</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">hidpi&nbsp;=&nbsp;True,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">js_event_callbacks&nbsp;=&nbsp;{},</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">js_property_callbacks&nbsp;=&nbsp;{},</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">left&nbsp;=&nbsp;[LinearAxis(id='4204', ...)],</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">lod_factor&nbsp;=&nbsp;10,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">lod_interval&nbsp;=&nbsp;300,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">lod_threshold&nbsp;=&nbsp;2000,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">lod_timeout&nbsp;=&nbsp;500,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">margin&nbsp;=&nbsp;(0, 0, 0, 0),</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">match_aspect&nbsp;=&nbsp;False,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">max_height&nbsp;=&nbsp;None,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">max_width&nbsp;=&nbsp;None,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border&nbsp;=&nbsp;5,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border_bottom&nbsp;=&nbsp;None,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border_left&nbsp;=&nbsp;None,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border_right&nbsp;=&nbsp;None,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border_top&nbsp;=&nbsp;None,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_height&nbsp;=&nbsp;None,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_width&nbsp;=&nbsp;None,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">name&nbsp;=&nbsp;None,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_alpha&nbsp;=&nbsp;{'value': 1.0},</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_cap&nbsp;=&nbsp;'butt',</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_color&nbsp;=&nbsp;{'value': '#e5e5e5'},</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_dash&nbsp;=&nbsp;[],</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_dash_offset&nbsp;=&nbsp;0,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_join&nbsp;=&nbsp;'bevel',</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_width&nbsp;=&nbsp;{'value': 1},</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">output_backend&nbsp;=&nbsp;'canvas',</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">plot_height&nbsp;=&nbsp;220,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">plot_width&nbsp;=&nbsp;400,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">renderers&nbsp;=&nbsp;[GlyphRenderer(id='4225', ...), GlyphRenderer(id='4230', ...)],</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">reset_policy&nbsp;=&nbsp;'standard',</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">right&nbsp;=&nbsp;[],</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">sizing_mode&nbsp;=&nbsp;None,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">subscribed_events&nbsp;=&nbsp;[],</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">tags&nbsp;=&nbsp;[],</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">title&nbsp;=&nbsp;Title(id='4189', ...),</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">title_location&nbsp;=&nbsp;'above',</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">toolbar&nbsp;=&nbsp;Toolbar(id='4215', ...),</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">toolbar_location&nbsp;=&nbsp;'right',</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">toolbar_sticky&nbsp;=&nbsp;True,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">visible&nbsp;=&nbsp;True,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">width&nbsp;=&nbsp;None,</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">width_policy&nbsp;=&nbsp;'auto',</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">x_range&nbsp;=&nbsp;DataRange1d(id='4191', ...),</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">x_scale&nbsp;=&nbsp;LinearScale(id='4195', ...),</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">y_range&nbsp;=&nbsp;DataRange1d(id='4193', ...),</div></div><div class=\"4628\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">y_scale&nbsp;=&nbsp;LinearScale(id='4197', ...))</div></div></div>\n",
+                            "<div style=\"display: table;\"><div style=\"display: table-row;\"><div style=\"display: table-cell;\"><b title=\"bokeh.plotting._figure.figure\">figure</b>(</div><div style=\"display: table-cell;\">id&nbsp;=&nbsp;'p1001', <span id=\"p1065\" style=\"cursor: pointer;\">&hellip;)</span></div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">above&nbsp;=&nbsp;[],</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">align&nbsp;=&nbsp;'auto',</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">aspect_ratio&nbsp;=&nbsp;None,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">aspect_scale&nbsp;=&nbsp;1,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">attribution&nbsp;=&nbsp;[],</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">background_fill_alpha&nbsp;=&nbsp;1.0,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">background_fill_color&nbsp;=&nbsp;'#ffffff',</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">below&nbsp;=&nbsp;[DatetimeAxis(id='p1013', ...)],</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">border_fill_alpha&nbsp;=&nbsp;1.0,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">border_fill_color&nbsp;=&nbsp;'#ffffff',</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">center&nbsp;=&nbsp;[Grid(id='p1029', ...), Grid(id='p1034', ...)],</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">context_menu&nbsp;=&nbsp;None,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">css_classes&nbsp;=&nbsp;[],</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">css_variables&nbsp;=&nbsp;{},</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">disabled&nbsp;=&nbsp;False,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">elements&nbsp;=&nbsp;[],</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">extra_x_ranges&nbsp;=&nbsp;{},</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">extra_x_scales&nbsp;=&nbsp;{},</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">extra_y_ranges&nbsp;=&nbsp;{},</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">extra_y_scales&nbsp;=&nbsp;{},</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">flow_mode&nbsp;=&nbsp;'block',</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">frame_align&nbsp;=&nbsp;True,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">frame_height&nbsp;=&nbsp;None,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">frame_width&nbsp;=&nbsp;None,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">height&nbsp;=&nbsp;220,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">height_policy&nbsp;=&nbsp;'auto',</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">hidpi&nbsp;=&nbsp;True,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">hold_render&nbsp;=&nbsp;False,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">js_event_callbacks&nbsp;=&nbsp;{},</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">js_property_callbacks&nbsp;=&nbsp;{},</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">left&nbsp;=&nbsp;[LinearAxis(id='p1030', ...)],</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">lod_factor&nbsp;=&nbsp;10,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">lod_interval&nbsp;=&nbsp;300,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">lod_threshold&nbsp;=&nbsp;2000,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">lod_timeout&nbsp;=&nbsp;500,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">margin&nbsp;=&nbsp;None,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">match_aspect&nbsp;=&nbsp;False,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">max_height&nbsp;=&nbsp;None,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">max_width&nbsp;=&nbsp;None,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border&nbsp;=&nbsp;5,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border_bottom&nbsp;=&nbsp;None,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border_left&nbsp;=&nbsp;None,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border_right&nbsp;=&nbsp;None,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border_top&nbsp;=&nbsp;None,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_height&nbsp;=&nbsp;None,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_width&nbsp;=&nbsp;None,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">name&nbsp;=&nbsp;None,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_alpha&nbsp;=&nbsp;1.0,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_cap&nbsp;=&nbsp;'butt',</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_color&nbsp;=&nbsp;'#e5e5e5',</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_dash&nbsp;=&nbsp;[],</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_dash_offset&nbsp;=&nbsp;0,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_join&nbsp;=&nbsp;'bevel',</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_width&nbsp;=&nbsp;1,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">output_backend&nbsp;=&nbsp;'canvas',</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">renderers&nbsp;=&nbsp;[GlyphRenderer(id='p1052', ...), GlyphRenderer(id='p1061', ...)],</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">reset_policy&nbsp;=&nbsp;'standard',</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">resizable&nbsp;=&nbsp;False,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">right&nbsp;=&nbsp;[],</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">sizing_mode&nbsp;=&nbsp;None,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">styles&nbsp;=&nbsp;{},</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">stylesheets&nbsp;=&nbsp;[],</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">subscribed_events&nbsp;=&nbsp;PropertyValueSet(),</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">syncable&nbsp;=&nbsp;True,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">tags&nbsp;=&nbsp;[],</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">title&nbsp;=&nbsp;Title(id='p1004', ...),</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">title_location&nbsp;=&nbsp;'above',</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">toolbar&nbsp;=&nbsp;Toolbar(id='p1010', ...),</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">toolbar_inner&nbsp;=&nbsp;False,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">toolbar_location&nbsp;=&nbsp;'right',</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">toolbar_sticky&nbsp;=&nbsp;True,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">visible&nbsp;=&nbsp;True,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">width&nbsp;=&nbsp;400,</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">width_policy&nbsp;=&nbsp;'auto',</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">x_range&nbsp;=&nbsp;DataRange1d(id='p1002', ...),</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">x_scale&nbsp;=&nbsp;LinearScale(id='p1011', ...),</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">y_range&nbsp;=&nbsp;DataRange1d(id='p1003', ...),</div></div><div class=\"p1064\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">y_scale&nbsp;=&nbsp;LinearScale(id='p1012', ...))</div></div></div>\n",
                             "<script>\n",
                             "(function() {\n",
-                            "  var expanded = false;\n",
-                            "  var ellipsis = document.getElementById(\"4629\");\n",
+                            "  let expanded = false;\n",
+                            "  const ellipsis = document.getElementById(\"p1065\");\n",
                             "  ellipsis.addEventListener(\"click\", function() {\n",
-                            "    var rows = document.getElementsByClassName(\"4628\");\n",
-                            "    for (var i = 0; i < rows.length; i++) {\n",
-                            "      var el = rows[i];\n",
+                            "    const rows = document.getElementsByClassName(\"p1064\");\n",
+                            "    for (let i = 0; i < rows.length; i++) {\n",
+                            "      const el = rows[i];\n",
                             "      el.style.display = expanded ? \"none\" : \"table-row\";\n",
                             "    }\n",
                             "    ellipsis.innerHTML = expanded ? \"&hellip;)\" : \"&lsaquo;&lsaquo;&lsaquo;\";\n",
                             "    expanded = !expanded;\n",
                             "  });\n",
                             "})();\n",
                             "</script>\n"
                         ],
                         "text/plain": [
-                            "Figure(id='4188', ...)"
+                            "figure(id='p1001', ...)"
                         ]
                     },
-                    "execution_count": 29,
+                    "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# If bokeh is installed, you got access to `iplot` method\n",
-                "ts.iplot(plot_width=400, plot_height=220, show=True)"
+                "ts.iplot(width=400, height=220, show=True)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 30,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "20"
                         ]
                     },
-                    "execution_count": 30,
+                    "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Can access any timestamp, if the timestamp is not part of the keys, it will get the previous value\n",
                 "ts['2019-01-01 00:13:00']"
@@ -519,113 +551,118 @@
             "source": [
                 "## Operations\n",
                 "-----"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 31,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [],
             "source": [
                 "start = Timestamp('2018-12-31 23:57:00')\n",
                 "end = Timestamp('2019-01-01 00:20:00')\n",
-                "kwargs_plot = dict(plot_width=400, plot_height=220, x_range=(start, end), y_range=(-5, 37))"
+                "kwargs_plot = dict(width=400, height=220, x_range=(start, end), y_range=(-5, 37))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 32,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Let's define another one\n",
                 "ts2 = TimeSeries(default=0)\n",
                 "ts2['2019-01-01 00:07:00'] = -1\n",
                 "ts2['2019-01-01 00:10:00'] = 5\n",
                 "ts2['2019-01-01 00:12:00'] = 14"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 33,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "<TimeSeries>\n",
-                        "2019-01-01T00:00:00+00:00: 10,\n",
-                        "2019-01-01T00:07:00+00:00: 9,\n",
-                        "2019-01-01T00:10:00+00:00: 25,\n",
-                        "2019-01-01T00:12:00+00:00: 34,\n",
-                        "2019-01-01T00:15:00+00:00: 24,\n"
-                    ]
+                    "data": {
+                        "text/html": [
+                            "<pre style=\"white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace\"><span style=\"font-weight: bold\">&lt;</span><span style=\"color: #ff00ff; text-decoration-color: #ff00ff; font-weight: bold\">TimeSeries</span><span style=\"font-weight: bold\">&gt;</span>\n",
+                            "<span style=\"color: #800080; text-decoration-color: #800080\">2019</span>-<span style=\"color: #800080; text-decoration-color: #800080\">01</span>-01T<span style=\"color: #00ff00; text-decoration-color: #00ff00; font-weight: bold\">00:00:00</span>+<span style=\"color: #00ff00; text-decoration-color: #00ff00; font-weight: bold\">00:00</span>: <span style=\"color: #800080; text-decoration-color: #800080\">10</span>,\n",
+                            "<span style=\"color: #800080; text-decoration-color: #800080\">2019</span>-<span style=\"color: #800080; text-decoration-color: #800080\">01</span>-01T<span style=\"color: #00ff00; text-decoration-color: #00ff00; font-weight: bold\">00:07:00</span>+<span style=\"color: #00ff00; text-decoration-color: #00ff00; font-weight: bold\">00:00</span>: <span style=\"color: #800080; text-decoration-color: #800080\">9</span>,\n",
+                            "<span style=\"color: #800080; text-decoration-color: #800080\">2019</span>-<span style=\"color: #800080; text-decoration-color: #800080\">01</span>-01T<span style=\"color: #00ff00; text-decoration-color: #00ff00; font-weight: bold\">00:10:00</span>+<span style=\"color: #00ff00; text-decoration-color: #00ff00; font-weight: bold\">00:00</span>: <span style=\"color: #800080; text-decoration-color: #800080\">25</span>,\n",
+                            "<span style=\"color: #800080; text-decoration-color: #800080\">2019</span>-<span style=\"color: #800080; text-decoration-color: #800080\">01</span>-01T<span style=\"color: #00ff00; text-decoration-color: #00ff00; font-weight: bold\">00:12:00</span>+<span style=\"color: #00ff00; text-decoration-color: #00ff00; font-weight: bold\">00:00</span>: <span style=\"color: #800080; text-decoration-color: #800080\">34</span>,\n",
+                            "<span style=\"color: #800080; text-decoration-color: #800080\">2019</span>-<span style=\"color: #800080; text-decoration-color: #800080\">01</span>-01T<span style=\"color: #00ff00; text-decoration-color: #00ff00; font-weight: bold\">00:15:00</span>+<span style=\"color: #00ff00; text-decoration-color: #00ff00; font-weight: bold\">00:00</span>: <span style=\"color: #800080; text-decoration-color: #800080\">24</span>,\n",
+                            "</pre>\n"
+                        ],
+                        "text/plain": [
+                            "\u001b[1m<\u001b[0m\u001b[1;95mTimeSeries\u001b[0m\u001b[1m>\u001b[0m\n",
+                            "\u001b[35m2019\u001b[0m-\u001b[35m01\u001b[0m-01T\u001b[1;92m00:00:00\u001b[0m+\u001b[1;92m00:00\u001b[0m: \u001b[35m10\u001b[0m,\n",
+                            "\u001b[35m2019\u001b[0m-\u001b[35m01\u001b[0m-01T\u001b[1;92m00:07:00\u001b[0m+\u001b[1;92m00:00\u001b[0m: \u001b[35m9\u001b[0m,\n",
+                            "\u001b[35m2019\u001b[0m-\u001b[35m01\u001b[0m-01T\u001b[1;92m00:10:00\u001b[0m+\u001b[1;92m00:00\u001b[0m: \u001b[35m25\u001b[0m,\n",
+                            "\u001b[35m2019\u001b[0m-\u001b[35m01\u001b[0m-01T\u001b[1;92m00:12:00\u001b[0m+\u001b[1;92m00:00\u001b[0m: \u001b[35m34\u001b[0m,\n",
+                            "\u001b[35m2019\u001b[0m-\u001b[35m01\u001b[0m-01T\u001b[1;92m00:15:00\u001b[0m+\u001b[1;92m00:00\u001b[0m: \u001b[35m24\u001b[0m,\n"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
                 }
             ],
             "source": [
                 "sum_ts = ts + ts2  # realize the sum of step functions\n",
                 "print(sum_ts)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 34,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "\n",
-                            "\n",
-                            "\n",
-                            "\n",
-                            "\n",
-                            "\n",
-                            "  <div class=\"bk-root\" id=\"50a17b9b-ba48-4cf2-b52a-5dec36549701\" data-root-id=\"4763\"></div>\n"
+                            "  <div id=\"e9117200-8ad9-48ec-a404-f7fcbf924171\" data-root-id=\"p1261\" style=\"display: contents;\"></div>\n"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/javascript": [
                             "(function(root) {\n",
                             "  function embed_document(root) {\n",
-                            "    \n",
-                            "  var docs_json = {\"db59b3b4-a00a-4f93-9a68-4e31e0ea1f16\":{\"roots\":{\"references\":[{\"attributes\":{\"children\":[{\"id\":\"4631\",\"subtype\":\"Figure\",\"type\":\"Plot\"},{\"id\":\"4675\",\"subtype\":\"Figure\",\"type\":\"Plot\"},{\"id\":\"4719\",\"subtype\":\"Figure\",\"type\":\"Plot\"}]},\"id\":\"4763\",\"type\":\"Row\"},{\"attributes\":{\"below\":[{\"id\":\"4642\",\"type\":\"DatetimeAxis\"}],\"center\":[{\"id\":\"4646\",\"type\":\"Grid\"},{\"id\":\"4651\",\"type\":\"Grid\"}],\"left\":[{\"id\":\"4647\",\"type\":\"LinearAxis\"}],\"plot_height\":220,\"plot_width\":400,\"renderers\":[{\"id\":\"4668\",\"type\":\"GlyphRenderer\"},{\"id\":\"4673\",\"type\":\"GlyphRenderer\"}],\"title\":{\"id\":\"4632\",\"type\":\"Title\"},\"toolbar\":{\"id\":\"4658\",\"type\":\"Toolbar\"},\"x_range\":{\"id\":\"4634\",\"type\":\"Range1d\"},\"x_scale\":{\"id\":\"4638\",\"type\":\"LinearScale\"},\"y_range\":{\"id\":\"4636\",\"type\":\"Range1d\"},\"y_scale\":{\"id\":\"4640\",\"type\":\"LinearScale\"}},\"id\":\"4631\",\"subtype\":\"Figure\",\"type\":\"Plot\"},{\"attributes\":{\"callback\":null,\"end\":1546302000000.0,\"start\":1546300620000.0},\"id\":\"4678\",\"type\":\"Range1d\"},{\"attributes\":{\"days\":[1,15]},\"id\":\"5066\",\"type\":\"DaysTicker\"},{\"attributes\":{},\"id\":\"4697\",\"type\":\"WheelZoomTool\"},{\"attributes\":{},\"id\":\"4692\",\"type\":\"BasicTicker\"},{\"attributes\":{},\"id\":\"4699\",\"type\":\"SaveTool\"},{\"attributes\":{\"axis_label\":\"timestamp\",\"formatter\":{\"id\":\"5035\",\"type\":\"DatetimeTickFormatter\"},\"ticker\":{\"id\":\"4687\",\"type\":\"DatetimeTicker\"}},\"id\":\"4686\",\"type\":\"DatetimeAxis\"},{\"attributes\":{\"text\":\"value\"},\"id\":\"4632\",\"type\":\"Title\"},{\"attributes\":{\"line_color\":{\"value\":\"#1f77b4\"},\"line_dash\":[4,4],\"line_width\":{\"value\":2},\"mode\":\"after\",\"x\":{\"field\":\"x\"},\"y\":{\"field\":\"y\"}},\"id\":\"4710\",\"type\":\"Step\"},{\"attributes\":{\"dimension\":1,\"ticker\":{\"id\":\"4692\",\"type\":\"BasicTicker\"}},\"id\":\"4695\",\"type\":\"Grid\"},{\"attributes\":{},\"id\":\"4696\",\"type\":\"PanTool\"},{\"attributes\":{\"formatter\":{\"id\":\"5037\",\"type\":\"BasicTickFormatter\"},\"ticker\":{\"id\":\"4692\",\"type\":\"BasicTicker\"}},\"id\":\"4691\",\"type\":\"LinearAxis\"},{\"attributes\":{\"line_alpha\":{\"value\":0.1},\"line_color\":{\"value\":\"#1f77b4\"},\"line_dash\":[4,4],\"line_width\":{\"value\":2},\"mode\":\"after\",\"x\":{\"field\":\"x\"},\"y\":{\"field\":\"y\"}},\"id\":\"4711\",\"type\":\"Step\"},{\"attributes\":{\"callback\":null,\"data\":{\"x\":[1546301220000.0,1546301400000.0,1546301520000.0],\"y\":[-1,5,14]},\"selected\":{\"id\":\"5073\",\"type\":\"Selection\"},\"selection_policy\":{\"id\":\"5072\",\"type\":\"UnionRenderers\"}},\"id\":\"4709\",\"type\":\"ColumnDataSource\"},{\"attributes\":{\"overlay\":{\"id\":\"5076\",\"type\":\"BoxAnnotation\"}},\"id\":\"4698\",\"type\":\"BoxZoomTool\"},{\"attributes\":{\"callback\":null,\"data\":{\"x\":[1546300800000.0,1546301400000.0,1546301700000.0],\"y\":[10,20,10]},\"selected\":{\"id\":\"5056\",\"type\":\"Selection\"},\"selection_policy\":{\"id\":\"5055\",\"type\":\"UnionRenderers\"}},\"id\":\"4665\",\"type\":\"ColumnDataSource\"},{\"attributes\":{\"num_minor_ticks\":5,\"tickers\":[{\"id\":\"5060\",\"type\":\"AdaptiveTicker\"},{\"id\":\"5061\",\"type\":\"AdaptiveTicker\"},{\"id\":\"5062\",\"type\":\"AdaptiveTicker\"},{\"id\":\"5063\",\"type\":\"DaysTicker\"},{\"id\":\"5064\",\"type\":\"DaysTicker\"},{\"id\":\"5065\",\"type\":\"DaysTicker\"},{\"id\":\"5066\",\"type\":\"DaysTicker\"},{\"id\":\"5067\",\"type\":\"MonthsTicker\"},{\"id\":\"5068\",\"type\":\"MonthsTicker\"},{\"id\":\"5069\",\"type\":\"MonthsTicker\"},{\"id\":\"5070\",\"type\":\"MonthsTicker\"},{\"id\":\"5071\",\"type\":\"YearsTicker\"}]},\"id\":\"4687\",\"type\":\"DatetimeTicker\"},{\"attributes\":{},\"id\":\"4700\",\"type\":\"ResetTool\"},{\"attributes\":{\"ticker\":{\"id\":\"4687\",\"type\":\"DatetimeTicker\"}},\"id\":\"4690\",\"type\":\"Grid\"},{\"attributes\":{\"fill_color\":{\"value\":\"red\"},\"line_color\":{\"value\":\"#1f77b4\"},\"size\":{\"units\":\"screen\",\"value\":6},\"x\":{\"field\":\"x\"},\"y\":{\"field\":\"y\"}},\"id\":\"4759\",\"type\":\"Circle\"},{\"attributes\":{\"months\":[0,1,2,3,4,5,6,7,8,9,10,11]},\"id\":\"5067\",\"type\":\"MonthsTicker\"},{\"attributes\":{\"fill_alpha\":{\"value\":0.1},\"fill_color\":{\"value\":\"#1f77b4\"},\"line_alpha\":{\"value\":0.1},\"line_color\":{\"value\":\"#1f77b4\"},\"size\":{\"units\":\"screen\",\"value\":6},\"x\":{\"field\":\"x\"},\"y\":{\"field\":\"y\"}},\"id\":\"4760\",\"type\":\"Circle\"},{\"attributes\":{\"months\":[0,2,4,6,8,10]},\"id\":\"5068\",\"type\":\"MonthsTicker\"},{\"attributes\":{},\"id\":\"4648\",\"type\":\"BasicTicker\"},{\"attributes\":{\"source\":{\"id\":\"4758\",\"type\":\"ColumnDataSource\"}},\"id\":\"4762\",\"type\":\"CDSView\"},{\"attributes\":{},\"id\":\"4745\",\"type\":\"HelpTool\"},{\"attributes\":{\"months\":[0,4,8]},\"id\":\"5069\",\"type\":\"MonthsTicker\"},{\"attributes\":{\"callback\":null,\"end\":1546302000000.0,\"start\":1546300620000.0},\"id\":\"4634\",\"type\":\"Range1d\"},{\"attributes\":{},\"id\":\"4701\",\"type\":\"HelpTool\"},{\"attributes\":{\"source\":{\"id\":\"4753\",\"type\":\"ColumnDataSource\"}},\"id\":\"4757\",\"type\":\"CDSView\"},{\"attributes\":{\"data_source\":{\"id\":\"4753\",\"type\":\"ColumnDataSource\"},\"glyph\":{\"id\":\"4754\",\"type\":\"Step\"},\"hover_glyph\":null,\"muted_glyph\":null,\"nonselection_glyph\":{\"id\":\"4755\",\"type\":\"Step\"},\"selection_glyph\":null,\"view\":{\"id\":\"4757\",\"type\":\"CDSView\"}},\"id\":\"4756\",\"type\":\"GlyphRenderer\"},{\"attributes\":{\"months\":[0,6]},\"id\":\"5070\",\"type\":\"MonthsTicker\"},{\"attributes\":{\"axis_label\":\"timestamp\",\"formatter\":{\"id\":\"5031\",\"type\":\"DatetimeTickFormatter\"},\"ticker\":{\"id\":\"4643\",\"type\":\"DatetimeTicker\"}},\"id\":\"4642\",\"type\":\"DatetimeAxis\"},{\"attributes\":{},\"id\":\"5071\",\"type\":\"YearsTicker\"},{\"attributes\":{\"dimension\":1,\"ticker\":{\"id\":\"4648\",\"type\":\"BasicTicker\"}},\"id\":\"4651\",\"type\":\"Grid\"},{\"attributes\":{\"callback\":null,\"data\":{\"x\":[1546301220000.0,1546301400000.0,1546301520000.0],\"y\":[-1,5,14]},\"selected\":{\"id\":\"5075\",\"type\":\"Selection\"},\"selection_policy\":{\"id\":\"5074\",\"type\":\"UnionRenderers\"}},\"id\":\"4714\",\"type\":\"ColumnDataSource\"},{\"attributes\":{},\"id\":\"5031\",\"type\":\"DatetimeTickFormatter\"},{\"attributes\":{},\"id\":\"4657\",\"type\":\"HelpTool\"},{\"attributes\":{},\"id\":\"5072\",\"type\":\"UnionRenderers\"},{\"attributes\":{\"ticker\":{\"id\":\"4643\",\"type\":\"DatetimeTicker\"}},\"id\":\"4646\",\"type\":\"Grid\"},{\"attributes\":{\"axis_label\":\"timestamp\",\"formatter\":{\"id\":\"5039\",\"type\":\"DatetimeTickFormatter\"},\"ticker\":{\"id\":\"4731\",\"type\":\"DatetimeTicker\"}},\"id\":\"4730\",\"type\":\"DatetimeAxis\"},{\"attributes\":{},\"id\":\"4744\",\"type\":\"ResetTool\"},{\"attributes\":{},\"id\":\"5033\",\"type\":\"BasicTickFormatter\"},{\"attributes\":{\"line_color\":{\"value\":\"#1f77b4\"},\"line_dash\":[4,4],\"line_width\":{\"value\":2},\"mode\":\"after\",\"x\":{\"field\":\"x\"},\"y\":{\"field\":\"y\"}},\"id\":\"4666\",\"type\":\"Step\"},{\"attributes\":{},\"id\":\"5073\",\"type\":\"Selection\"},{\"attributes\":{\"line_color\":{\"value\":\"#1f77b4\"},\"line_dash\":[4,4],\"line_width\":{\"value\":2},\"mode\":\"after\",\"x\":{\"field\":\"x\"},\"y\":{\"field\":\"y\"}},\"id\":\"4754\",\"type\":\"Step\"},{\"attributes\":{\"callback\":null,\"data\":{\"x\":[1546300800000.0,1546301220000.0,1546301400000.0,1546301520000.0,1546301700000.0],\"y\":[10,9,25,34,24]},\"selected\":{\"id\":\"5092\",\"type\":\"Selection\"},\"selection_policy\":{\"id\":\"5091\",\"type\":\"UnionRenderers\"}},\"id\":\"4758\",\"type\":\"ColumnDataSource\"},{\"attributes\":{},\"id\":\"5035\",\"type\":\"DatetimeTickFormatter\"},{\"attributes\":{},\"id\":\"5074\",\"type\":\"UnionRenderers\"},{\"attributes\":{},\"id\":\"4640\",\"type\":\"LinearScale\"},{\"attributes\":{},\"id\":\"4728\",\"type\":\"LinearScale\"},{\"attributes\":{},\"id\":\"4655\",\"type\":\"SaveTool\"},{\"attributes\":{\"num_minor_ticks\":5,\"tickers\":[{\"id\":\"5043\",\"type\":\"AdaptiveTicker\"},{\"id\":\"5044\",\"type\":\"AdaptiveTicker\"},{\"id\":\"5045\",\"type\":\"AdaptiveTicker\"},{\"id\":\"5046\",\"type\":\"DaysTicker\"},{\"id\":\"5047\",\"type\":\"DaysTicker\"},{\"id\":\"5048\",\"type\":\"DaysTicker\"},{\"id\":\"5049\",\"type\":\"DaysTicker\"},{\"id\":\"5050\",\"type\":\"MonthsTicker\"},{\"id\":\"5051\",\"type\":\"MonthsTicker\"},{\"id\":\"5052\",\"type\":\"MonthsTicker\"},{\"id\":\"5053\",\"type\":\"MonthsTicker\"},{\"id\":\"5054\",\"type\":\"YearsTicker\"}]},\"id\":\"4643\",\"type\":\"DatetimeTicker\"},{\"attributes\":{},\"id\":\"5037\",\"type\":\"BasicTickFormatter\"},{\"attributes\":{},\"id\":\"5075\",\"type\":\"Selection\"},{\"attributes\":{},\"id\":\"5039\",\"type\":\"DatetimeTickFormatter\"},{\"attributes\":{\"bottom_units\":\"screen\",\"fill_alpha\":{\"value\":0.5},\"fill_color\":{\"value\":\"lightgrey\"},\"left_units\":\"screen\",\"level\":\"overlay\",\"line_alpha\":{\"value\":1.0},\"line_color\":{\"value\":\"black\"},\"line_dash\":[4,4],\"line_width\":{\"value\":2},\"render_mode\":\"css\",\"right_units\":\"screen\",\"top_units\":\"screen\"},\"id\":\"5076\",\"type\":\"BoxAnnotation\"},{\"attributes\":{\"active_drag\":\"auto\",\"active_inspect\":\"auto\",\"active_multi\":null,\"active_scroll\":\"auto\",\"active_tap\":\"auto\",\"tools\":[{\"id\":\"4652\",\"type\":\"PanTool\"},{\"id\":\"4653\",\"type\":\"WheelZoomTool\"},{\"id\":\"4654\",\"type\":\"BoxZoomTool\"},{\"id\":\"4655\",\"type\":\"SaveTool\"},{\"id\":\"4656\",\"type\":\"ResetTool\"},{\"id\":\"4657\",\"type\":\"HelpTool\"}]},\"id\":\"4658\",\"type\":\"Toolbar\"},{\"attributes\":{},\"id\":\"5041\",\"type\":\"BasicTickFormatter\"},{\"attributes\":{\"mantissas\":[1,2,5],\"max_interval\":500.0,\"num_minor_ticks\":0},\"id\":\"5077\",\"type\":\"AdaptiveTicker\"},{\"attributes\":{\"mantissas\":[1,2,5],\"max_interval\":500.0,\"num_minor_ticks\":0},\"id\":\"5043\",\"type\":\"AdaptiveTicker\"},{\"attributes\":{},\"id\":\"4638\",\"type\":\"LinearScale\"},{\"attributes\":{\"text\":\"value\"},\"id\":\"4720\",\"type\":\"Title\"},{\"attributes\":{\"base\":60,\"mantissas\":[1,2,5,10,15,20,30],\"max_interval\":1800000.0,\"min_interval\":1000.0,\"num_minor_ticks\":0},\"id\":\"5078\",\"type\":\"AdaptiveTicker\"},{\"attributes\":{\"callback\":null,\"end\":37,\"start\":-5},\"id\":\"4636\",\"type\":\"Range1d\"},{\"attributes\":{},\"id\":\"4726\",\"type\":\"LinearScale\"},{\"attributes\":{},\"id\":\"4652\",\"type\":\"PanTool\"},{\"attributes\":{\"base\":60,\"mantissas\":[1,2,5,10,15,20,30],\"max_interval\":1800000.0,\"min_interval\":1000.0,\"num_minor_ticks\":0},\"id\":\"5044\",\"type\":\"AdaptiveTicker\"},{\"attributes\":{\"line_alpha\":{\"value\":0.1},\"line_color\":{\"value\":\"#1f77b4\"},\"line_dash\":[4,4],\"line_width\":{\"value\":2},\"mode\":\"after\",\"x\":{\"field\":\"x\"},\"y\":{\"field\":\"y\"}},\"id\":\"4667\",\"type\":\"Step\"},{\"attributes\":{\"base\":24,\"mantissas\":[1,2,4,6,8,12],\"max_interval\":43200000.0,\"min_interval\":3600000.0,\"num_minor_ticks\":0},\"id\":\"5079\",\"type\":\"AdaptiveTicker\"},{\"attributes\":{\"below\":[{\"id\":\"4730\",\"type\":\"DatetimeAxis\"}],\"center\":[{\"id\":\"4734\",\"type\":\"Grid\"},{\"id\":\"4739\",\"type\":\"Grid\"}],\"left\":[{\"id\":\"4735\",\"type\":\"LinearAxis\"}],\"plot_height\":220,\"plot_width\":400,\"renderers\":[{\"id\":\"4756\",\"type\":\"GlyphRenderer\"},{\"id\":\"4761\",\"type\":\"GlyphRenderer\"}],\"title\":{\"id\":\"4720\",\"type\":\"Title\"},\"toolbar\":{\"id\":\"4746\",\"type\":\"Toolbar\"},\"x_range\":{\"id\":\"4722\",\"type\":\"Range1d\"},\"x_scale\":{\"id\":\"4726\",\"type\":\"LinearScale\"},\"y_range\":{\"id\":\"4724\",\"type\":\"Range1d\"},\"y_scale\":{\"id\":\"4728\",\"type\":\"LinearScale\"}},\"id\":\"4719\",\"subtype\":\"Figure\",\"type\":\"Plot\"},{\"attributes\":{\"formatter\":{\"id\":\"5033\",\"type\":\"BasicTickFormatter\"},\"ticker\":{\"id\":\"4648\",\"type\":\"BasicTicker\"}},\"id\":\"4647\",\"type\":\"LinearAxis\"},{\"attributes\":{\"base\":24,\"mantissas\":[1,2,4,6,8,12],\"max_interval\":43200000.0,\"min_interval\":3600000.0,\"num_minor_ticks\":0},\"id\":\"5045\",\"type\":\"AdaptiveTicker\"},{\"attributes\":{\"days\":[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31]},\"id\":\"5080\",\"type\":\"DaysTicker\"},{\"attributes\":{\"dimension\":1,\"ticker\":{\"id\":\"4736\",\"type\":\"BasicTicker\"}},\"id\":\"4739\",\"type\":\"Grid\"},{\"attributes\":{\"source\":{\"id\":\"4709\",\"type\":\"ColumnDataSource\"}},\"id\":\"4713\",\"type\":\"CDSView\"},{\"attributes\":{\"days\":[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31]},\"id\":\"5046\",\"type\":\"DaysTicker\"},{\"attributes\":{\"source\":{\"id\":\"4665\",\"type\":\"ColumnDataSource\"}},\"id\":\"4669\",\"type\":\"CDSView\"},{\"attributes\":{\"days\":[1,4,7,10,13,16,19,22,25,28]},\"id\":\"5081\",\"type\":\"DaysTicker\"},{\"attributes\":{\"days\":[1,4,7,10,13,16,19,22,25,28]},\"id\":\"5047\",\"type\":\"DaysTicker\"},{\"attributes\":{\"days\":[1,8,15,22]},\"id\":\"5082\",\"type\":\"DaysTicker\"},{\"attributes\":{\"overlay\":{\"id\":\"5059\",\"type\":\"BoxAnnotation\"}},\"id\":\"4654\",\"type\":\"BoxZoomTool\"},{\"attributes\":{\"days\":[1,8,15,22]},\"id\":\"5048\",\"type\":\"DaysTicker\"},{\"attributes\":{\"days\":[1,15]},\"id\":\"5083\",\"type\":\"DaysTicker\"},{\"attributes\":{\"fill_color\":{\"value\":\"red\"},\"line_color\":{\"value\":\"#1f77b4\"},\"size\":{\"units\":\"screen\",\"value\":6},\"x\":{\"field\":\"x\"},\"y\":{\"field\":\"y\"}},\"id\":\"4671\",\"type\":\"Circle\"},{\"attributes\":{\"data_source\":{\"id\":\"4709\",\"type\":\"ColumnDataSource\"},\"glyph\":{\"id\":\"4710\",\"type\":\"Step\"},\"hover_glyph\":null,\"muted_glyph\":null,\"nonselection_glyph\":{\"id\":\"4711\",\"type\":\"Step\"},\"selection_glyph\":null,\"view\":{\"id\":\"4713\",\"type\":\"CDSView\"}},\"id\":\"4712\",\"type\":\"GlyphRenderer\"},{\"attributes\":{\"days\":[1,15]},\"id\":\"5049\",\"type\":\"DaysTicker\"},{\"attributes\":{\"months\":[0,1,2,3,4,5,6,7,8,9,10,11]},\"id\":\"5084\",\"type\":\"MonthsTicker\"},{\"attributes\":{},\"id\":\"4656\",\"type\":\"ResetTool\"},{\"attributes\":{\"fill_color\":{\"value\":\"red\"},\"line_color\":{\"value\":\"#1f77b4\"},\"size\":{\"units\":\"screen\",\"value\":6},\"x\":{\"field\":\"x\"},\"y\":{\"field\":\"y\"}},\"id\":\"4715\",\"type\":\"Circle\"},{\"attributes\":{\"months\":[0,1,2,3,4,5,6,7,8,9,10,11]},\"id\":\"5050\",\"type\":\"MonthsTicker\"},{\"attributes\":{\"months\":[0,2,4,6,8,10]},\"id\":\"5085\",\"type\":\"MonthsTicker\"},{\"attributes\":{\"active_drag\":\"auto\",\"active_inspect\":\"auto\",\"active_multi\":null,\"active_scroll\":\"auto\",\"active_tap\":\"auto\",\"tools\":[{\"id\":\"4696\",\"type\":\"PanTool\"},{\"id\":\"4697\",\"type\":\"WheelZoomTool\"},{\"id\":\"4698\",\"type\":\"BoxZoomTool\"},{\"id\":\"4699\",\"type\":\"SaveTool\"},{\"id\":\"4700\",\"type\":\"ResetTool\"},{\"id\":\"4701\",\"type\":\"HelpTool\"}]},\"id\":\"4702\",\"type\":\"Toolbar\"},{\"attributes\":{},\"id\":\"4653\",\"type\":\"WheelZoomTool\"},{\"attributes\":{\"months\":[0,2,4,6,8,10]},\"id\":\"5051\",\"type\":\"MonthsTicker\"},{\"attributes\":{\"months\":[0,4,8]},\"id\":\"5086\",\"type\":\"MonthsTicker\"},{\"attributes\":{\"months\":[0,4,8]},\"id\":\"5052\",\"type\":\"MonthsTicker\"},{\"attributes\":{\"months\":[0,6]},\"id\":\"5087\",\"type\":\"MonthsTicker\"},{\"attributes\":{\"fill_alpha\":{\"value\":0.1},\"fill_color\":{\"value\":\"#1f77b4\"},\"line_alpha\":{\"value\":0.1},\"line_color\":{\"value\":\"#1f77b4\"},\"size\":{\"units\":\"screen\",\"value\":6},\"x\":{\"field\":\"x\"},\"y\":{\"field\":\"y\"}},\"id\":\"4716\",\"type\":\"Circle\"},{\"attributes\":{\"months\":[0,6]},\"id\":\"5053\",\"type\":\"MonthsTicker\"},{\"attributes\":{},\"id\":\"5088\",\"type\":\"YearsTicker\"},{\"attributes\":{\"callback\":null,\"data\":{\"x\":[1546300800000.0,1546301400000.0,1546301700000.0],\"y\":[10,20,10]},\"selected\":{\"id\":\"5058\",\"type\":\"Selection\"},\"selection_policy\":{\"id\":\"5057\",\"type\":\"UnionRenderers\"}},\"id\":\"4670\",\"type\":\"ColumnDataSource\"},{\"attributes\":{\"data_source\":{\"id\":\"4758\",\"type\":\"ColumnDataSource\"},\"glyph\":{\"id\":\"4759\",\"type\":\"Circle\"},\"hover_glyph\":null,\"muted_glyph\":null,\"nonselection_glyph\":{\"id\":\"4760\",\"type\":\"Circle\"},\"selection_glyph\":null,\"view\":{\"id\":\"4762\",\"type\":\"CDSView\"}},\"id\":\"4761\",\"type\":\"GlyphRenderer\"},{\"attributes\":{},\"id\":\"5054\",\"type\":\"YearsTicker\"},{\"attributes\":{},\"id\":\"5089\",\"type\":\"UnionRenderers\"},{\"attributes\":{\"data_source\":{\"id\":\"4665\",\"type\":\"ColumnDataSource\"},\"glyph\":{\"id\":\"4666\",\"type\":\"Step\"},\"hover_glyph\":null,\"muted_glyph\":null,\"nonselection_glyph\":{\"id\":\"4667\",\"type\":\"Step\"},\"selection_glyph\":null,\"view\":{\"id\":\"4669\",\"type\":\"CDSView\"}},\"id\":\"4668\",\"type\":\"GlyphRenderer\"},{\"attributes\":{},\"id\":\"4743\",\"type\":\"SaveTool\"},{\"attributes\":{},\"id\":\"5055\",\"type\":\"UnionRenderers\"},{\"attributes\":{},\"id\":\"5090\",\"type\":\"Selection\"},{\"attributes\":{\"data_source\":{\"id\":\"4670\",\"type\":\"ColumnDataSource\"},\"glyph\":{\"id\":\"4671\",\"type\":\"Circle\"},\"hover_glyph\":null,\"muted_glyph\":null,\"nonselection_glyph\":{\"id\":\"4672\",\"type\":\"Circle\"},\"selection_glyph\":null,\"view\":{\"id\":\"4674\",\"type\":\"CDSView\"}},\"id\":\"4673\",\"type\":\"GlyphRenderer\"},{\"attributes\":{},\"id\":\"5056\",\"type\":\"Selection\"},{\"attributes\":{},\"id\":\"5091\",\"type\":\"UnionRenderers\"},{\"attributes\":{\"fill_alpha\":{\"value\":0.1},\"fill_color\":{\"value\":\"#1f77b4\"},\"line_alpha\":{\"value\":0.1},\"line_color\":{\"value\":\"#1f77b4\"},\"size\":{\"units\":\"screen\",\"value\":6},\"x\":{\"field\":\"x\"},\"y\":{\"field\":\"y\"}},\"id\":\"4672\",\"type\":\"Circle\"},{\"attributes\":{},\"id\":\"5057\",\"type\":\"UnionRenderers\"},{\"attributes\":{},\"id\":\"5092\",\"type\":\"Selection\"},{\"attributes\":{},\"id\":\"4684\",\"type\":\"LinearScale\"},{\"attributes\":{},\"id\":\"4741\",\"type\":\"WheelZoomTool\"},{\"attributes\":{},\"id\":\"5058\",\"type\":\"Selection\"},{\"attributes\":{\"bottom_units\":\"screen\",\"fill_alpha\":{\"value\":0.5},\"fill_color\":{\"value\":\"lightgrey\"},\"left_units\":\"screen\",\"level\":\"overlay\",\"line_alpha\":{\"value\":1.0},\"line_color\":{\"value\":\"black\"},\"line_dash\":[4,4],\"line_width\":{\"value\":2},\"render_mode\":\"css\",\"right_units\":\"screen\",\"top_units\":\"screen\"},\"id\":\"5093\",\"type\":\"BoxAnnotation\"},{\"attributes\":{\"overlay\":{\"id\":\"5093\",\"type\":\"BoxAnnotation\"}},\"id\":\"4742\",\"type\":\"BoxZoomTool\"},{\"attributes\":{\"bottom_units\":\"screen\",\"fill_alpha\":{\"value\":0.5},\"fill_color\":{\"value\":\"lightgrey\"},\"left_units\":\"screen\",\"level\":\"overlay\",\"line_alpha\":{\"value\":1.0},\"line_color\":{\"value\":\"black\"},\"line_dash\":[4,4],\"line_width\":{\"value\":2},\"render_mode\":\"css\",\"right_units\":\"screen\",\"top_units\":\"screen\"},\"id\":\"5059\",\"type\":\"BoxAnnotation\"},{\"attributes\":{\"formatter\":{\"id\":\"5041\",\"type\":\"BasicTickFormatter\"},\"ticker\":{\"id\":\"4736\",\"type\":\"BasicTicker\"}},\"id\":\"4735\",\"type\":\"LinearAxis\"},{\"attributes\":{\"source\":{\"id\":\"4714\",\"type\":\"ColumnDataSource\"}},\"id\":\"4718\",\"type\":\"CDSView\"},{\"attributes\":{\"mantissas\":[1,2,5],\"max_interval\":500.0,\"num_minor_ticks\":0},\"id\":\"5060\",\"type\":\"AdaptiveTicker\"},{\"attributes\":{\"num_minor_ticks\":5,\"tickers\":[{\"id\":\"5077\",\"type\":\"AdaptiveTicker\"},{\"id\":\"5078\",\"type\":\"AdaptiveTicker\"},{\"id\":\"5079\",\"type\":\"AdaptiveTicker\"},{\"id\":\"5080\",\"type\":\"DaysTicker\"},{\"id\":\"5081\",\"type\":\"DaysTicker\"},{\"id\":\"5082\",\"type\":\"DaysTicker\"},{\"id\":\"5083\",\"type\":\"DaysTicker\"},{\"id\":\"5084\",\"type\":\"MonthsTicker\"},{\"id\":\"5085\",\"type\":\"MonthsTicker\"},{\"id\":\"5086\",\"type\":\"MonthsTicker\"},{\"id\":\"5087\",\"type\":\"MonthsTicker\"},{\"id\":\"5088\",\"type\":\"YearsTicker\"}]},\"id\":\"4731\",\"type\":\"DatetimeTicker\"},{\"attributes\":{\"callback\":null,\"end\":37,\"start\":-5},\"id\":\"4680\",\"type\":\"Range1d\"},{\"attributes\":{\"base\":60,\"mantissas\":[1,2,5,10,15,20,30],\"max_interval\":1800000.0,\"min_interval\":1000.0,\"num_minor_ticks\":0},\"id\":\"5061\",\"type\":\"AdaptiveTicker\"},{\"attributes\":{\"text\":\"value\"},\"id\":\"4676\",\"type\":\"Title\"},{\"attributes\":{\"active_drag\":\"auto\",\"active_inspect\":\"auto\",\"active_multi\":null,\"active_scroll\":\"auto\",\"active_tap\":\"auto\",\"tools\":[{\"id\":\"4740\",\"type\":\"PanTool\"},{\"id\":\"4741\",\"type\":\"WheelZoomTool\"},{\"id\":\"4742\",\"type\":\"BoxZoomTool\"},{\"id\":\"4743\",\"type\":\"SaveTool\"},{\"id\":\"4744\",\"type\":\"ResetTool\"},{\"id\":\"4745\",\"type\":\"HelpTool\"}]},\"id\":\"4746\",\"type\":\"Toolbar\"},{\"attributes\":{},\"id\":\"4736\",\"type\":\"BasicTicker\"},{\"attributes\":{\"base\":24,\"mantissas\":[1,2,4,6,8,12],\"max_interval\":43200000.0,\"min_interval\":3600000.0,\"num_minor_ticks\":0},\"id\":\"5062\",\"type\":\"AdaptiveTicker\"},{\"attributes\":{\"ticker\":{\"id\":\"4731\",\"type\":\"DatetimeTicker\"}},\"id\":\"4734\",\"type\":\"Grid\"},{\"attributes\":{\"callback\":null,\"end\":37,\"start\":-5},\"id\":\"4724\",\"type\":\"Range1d\"},{\"attributes\":{},\"id\":\"4740\",\"type\":\"PanTool\"},{\"attributes\":{\"days\":[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31]},\"id\":\"5063\",\"type\":\"DaysTicker\"},{\"attributes\":{\"below\":[{\"id\":\"4686\",\"type\":\"DatetimeAxis\"}],\"center\":[{\"id\":\"4690\",\"type\":\"Grid\"},{\"id\":\"4695\",\"type\":\"Grid\"}],\"left\":[{\"id\":\"4691\",\"type\":\"LinearAxis\"}],\"plot_height\":220,\"plot_width\":400,\"renderers\":[{\"id\":\"4712\",\"type\":\"GlyphRenderer\"},{\"id\":\"4717\",\"type\":\"GlyphRenderer\"}],\"title\":{\"id\":\"4676\",\"type\":\"Title\"},\"toolbar\":{\"id\":\"4702\",\"type\":\"Toolbar\"},\"x_range\":{\"id\":\"4678\",\"type\":\"Range1d\"},\"x_scale\":{\"id\":\"4682\",\"type\":\"LinearScale\"},\"y_range\":{\"id\":\"4680\",\"type\":\"Range1d\"},\"y_scale\":{\"id\":\"4684\",\"type\":\"LinearScale\"}},\"id\":\"4675\",\"subtype\":\"Figure\",\"type\":\"Plot\"},{\"attributes\":{\"callback\":null,\"end\":1546302000000.0,\"start\":1546300620000.0},\"id\":\"4722\",\"type\":\"Range1d\"},{\"attributes\":{\"days\":[1,4,7,10,13,16,19,22,25,28]},\"id\":\"5064\",\"type\":\"DaysTicker\"},{\"attributes\":{\"data_source\":{\"id\":\"4714\",\"type\":\"ColumnDataSource\"},\"glyph\":{\"id\":\"4715\",\"type\":\"Circle\"},\"hover_glyph\":null,\"muted_glyph\":null,\"nonselection_glyph\":{\"id\":\"4716\",\"type\":\"Circle\"},\"selection_glyph\":null,\"view\":{\"id\":\"4718\",\"type\":\"CDSView\"}},\"id\":\"4717\",\"type\":\"GlyphRenderer\"},{\"attributes\":{\"source\":{\"id\":\"4670\",\"type\":\"ColumnDataSource\"}},\"id\":\"4674\",\"type\":\"CDSView\"},{\"attributes\":{\"days\":[1,8,15,22]},\"id\":\"5065\",\"type\":\"DaysTicker\"},{\"attributes\":{\"line_alpha\":{\"value\":0.1},\"line_color\":{\"value\":\"#1f77b4\"},\"line_dash\":[4,4],\"line_width\":{\"value\":2},\"mode\":\"after\",\"x\":{\"field\":\"x\"},\"y\":{\"field\":\"y\"}},\"id\":\"4755\",\"type\":\"Step\"},{\"attributes\":{},\"id\":\"4682\",\"type\":\"LinearScale\"},{\"attributes\":{\"callback\":null,\"data\":{\"x\":[1546300800000.0,1546301220000.0,1546301400000.0,1546301520000.0,1546301700000.0],\"y\":[10,9,25,34,24]},\"selected\":{\"id\":\"5090\",\"type\":\"Selection\"},\"selection_policy\":{\"id\":\"5089\",\"type\":\"UnionRenderers\"}},\"id\":\"4753\",\"type\":\"ColumnDataSource\"}],\"root_ids\":[\"4763\"]},\"title\":\"Bokeh Application\",\"version\":\"1.3.1\"}};\n",
-                            "  var render_items = [{\"docid\":\"db59b3b4-a00a-4f93-9a68-4e31e0ea1f16\",\"roots\":{\"4763\":\"50a17b9b-ba48-4cf2-b52a-5dec36549701\"}}];\n",
-                            "  root.Bokeh.embed.embed_items_notebook(docs_json, render_items);\n",
-                            "\n",
+                            "  const docs_json = {\"f84e2a8a-d2f7-43a1-94d5-04f0cb83641c\":{\"version\":\"3.4.1\",\"title\":\"Bokeh Application\",\"roots\":[{\"type\":\"object\",\"name\":\"Row\",\"id\":\"p1261\",\"attributes\":{\"children\":[{\"type\":\"object\",\"name\":\"Figure\",\"id\":\"p1066\",\"attributes\":{\"width\":400,\"height\":220,\"x_range\":{\"type\":\"object\",\"name\":\"Range1d\",\"id\":\"p1076\",\"attributes\":{\"start\":1546300620000.0,\"end\":1546302000000.0}},\"y_range\":{\"type\":\"object\",\"name\":\"Range1d\",\"id\":\"p1077\",\"attributes\":{\"start\":-5,\"end\":37}},\"x_scale\":{\"type\":\"object\",\"name\":\"LinearScale\",\"id\":\"p1078\"},\"y_scale\":{\"type\":\"object\",\"name\":\"LinearScale\",\"id\":\"p1079\"},\"title\":{\"type\":\"object\",\"name\":\"Title\",\"id\":\"p1069\",\"attributes\":{\"text\":\"value\"}},\"renderers\":[{\"type\":\"object\",\"name\":\"GlyphRenderer\",\"id\":\"p1119\",\"attributes\":{\"data_source\":{\"type\":\"object\",\"name\":\"ColumnDataSource\",\"id\":\"p1113\",\"attributes\":{\"selected\":{\"type\":\"object\",\"name\":\"Selection\",\"id\":\"p1114\",\"attributes\":{\"indices\":[],\"line_indices\":[]}},\"selection_policy\":{\"type\":\"object\",\"name\":\"UnionRenderers\",\"id\":\"p1115\"},\"data\":{\"type\":\"map\",\"entries\":[[\"x\",[1546300800000.0,1546301400000.0,1546301700000.0]],[\"y\",[10,20,10]]]}}},\"view\":{\"type\":\"object\",\"name\":\"CDSView\",\"id\":\"p1120\",\"attributes\":{\"filter\":{\"type\":\"object\",\"name\":\"AllIndices\",\"id\":\"p1121\"}}},\"glyph\":{\"type\":\"object\",\"name\":\"Step\",\"id\":\"p1116\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"line_color\":\"#1f77b4\",\"line_width\":2,\"line_dash\":[4,4],\"mode\":\"after\"}},\"nonselection_glyph\":{\"type\":\"object\",\"name\":\"Step\",\"id\":\"p1117\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"line_color\":\"#1f77b4\",\"line_alpha\":0.1,\"line_width\":2,\"line_dash\":[4,4],\"mode\":\"after\"}},\"muted_glyph\":{\"type\":\"object\",\"name\":\"Step\",\"id\":\"p1118\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"line_color\":\"#1f77b4\",\"line_alpha\":0.2,\"line_width\":2,\"line_dash\":[4,4],\"mode\":\"after\"}}}},{\"type\":\"object\",\"name\":\"GlyphRenderer\",\"id\":\"p1128\",\"attributes\":{\"data_source\":{\"type\":\"object\",\"name\":\"ColumnDataSource\",\"id\":\"p1122\",\"attributes\":{\"selected\":{\"type\":\"object\",\"name\":\"Selection\",\"id\":\"p1123\",\"attributes\":{\"indices\":[],\"line_indices\":[]}},\"selection_policy\":{\"type\":\"object\",\"name\":\"UnionRenderers\",\"id\":\"p1124\"},\"data\":{\"type\":\"map\",\"entries\":[[\"x\",[1546300800000.0,1546301400000.0,1546301700000.0]],[\"y\",[10,20,10]]]}}},\"view\":{\"type\":\"object\",\"name\":\"CDSView\",\"id\":\"p1129\",\"attributes\":{\"filter\":{\"type\":\"object\",\"name\":\"AllIndices\",\"id\":\"p1130\"}}},\"glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1125\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"size\":{\"type\":\"value\",\"value\":6},\"line_color\":{\"type\":\"value\",\"value\":\"#1f77b4\"},\"fill_color\":{\"type\":\"value\",\"value\":\"red\"}}},\"nonselection_glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1126\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"size\":{\"type\":\"value\",\"value\":6},\"line_color\":{\"type\":\"value\",\"value\":\"#1f77b4\"},\"line_alpha\":{\"type\":\"value\",\"value\":0.1},\"fill_color\":{\"type\":\"value\",\"value\":\"red\"},\"fill_alpha\":{\"type\":\"value\",\"value\":0.1},\"hatch_alpha\":{\"type\":\"value\",\"value\":0.1}}},\"muted_glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1127\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"size\":{\"type\":\"value\",\"value\":6},\"line_color\":{\"type\":\"value\",\"value\":\"#1f77b4\"},\"line_alpha\":{\"type\":\"value\",\"value\":0.2},\"fill_color\":{\"type\":\"value\",\"value\":\"red\"},\"fill_alpha\":{\"type\":\"value\",\"value\":0.2},\"hatch_alpha\":{\"type\":\"value\",\"value\":0.2}}}}}],\"toolbar\":{\"type\":\"object\",\"name\":\"Toolbar\",\"id\":\"p1075\",\"attributes\":{\"tools\":[{\"type\":\"object\",\"name\":\"PanTool\",\"id\":\"p1102\"},{\"type\":\"object\",\"name\":\"WheelZoomTool\",\"id\":\"p1103\",\"attributes\":{\"renderers\":\"auto\"}},{\"type\":\"object\",\"name\":\"BoxZoomTool\",\"id\":\"p1104\",\"attributes\":{\"overlay\":{\"type\":\"object\",\"name\":\"BoxAnnotation\",\"id\":\"p1105\",\"attributes\":{\"syncable\":false,\"level\":\"overlay\",\"visible\":false,\"left\":{\"type\":\"number\",\"value\":\"nan\"},\"right\":{\"type\":\"number\",\"value\":\"nan\"},\"top\":{\"type\":\"number\",\"value\":\"nan\"},\"bottom\":{\"type\":\"number\",\"value\":\"nan\"},\"left_units\":\"canvas\",\"right_units\":\"canvas\",\"top_units\":\"canvas\",\"bottom_units\":\"canvas\",\"line_color\":\"black\",\"line_alpha\":1.0,\"line_width\":2,\"line_dash\":[4,4],\"fill_color\":\"lightgrey\",\"fill_alpha\":0.5}}}},{\"type\":\"object\",\"name\":\"SaveTool\",\"id\":\"p1110\"},{\"type\":\"object\",\"name\":\"ResetTool\",\"id\":\"p1111\"},{\"type\":\"object\",\"name\":\"HelpTool\",\"id\":\"p1112\"}]}},\"left\":[{\"type\":\"object\",\"name\":\"LinearAxis\",\"id\":\"p1097\",\"attributes\":{\"ticker\":{\"type\":\"object\",\"name\":\"BasicTicker\",\"id\":\"p1098\",\"attributes\":{\"mantissas\":[1,2,5]}},\"formatter\":{\"type\":\"object\",\"name\":\"BasicTickFormatter\",\"id\":\"p1099\"},\"major_label_policy\":{\"type\":\"object\",\"name\":\"AllLabels\",\"id\":\"p1100\"}}}],\"below\":[{\"type\":\"object\",\"name\":\"DatetimeAxis\",\"id\":\"p1080\",\"attributes\":{\"ticker\":{\"type\":\"object\",\"name\":\"DatetimeTicker\",\"id\":\"p1081\",\"attributes\":{\"num_minor_ticks\":5,\"tickers\":[{\"type\":\"object\",\"name\":\"AdaptiveTicker\",\"id\":\"p1082\",\"attributes\":{\"num_minor_ticks\":0,\"mantissas\":[1,2,5],\"max_interval\":500.0}},{\"type\":\"object\",\"name\":\"AdaptiveTicker\",\"id\":\"p1083\",\"attributes\":{\"num_minor_ticks\":0,\"base\":60,\"mantissas\":[1,2,5,10,15,20,30],\"min_interval\":1000.0,\"max_interval\":1800000.0}},{\"type\":\"object\",\"name\":\"AdaptiveTicker\",\"id\":\"p1084\",\"attributes\":{\"num_minor_ticks\":0,\"base\":24,\"mantissas\":[1,2,4,6,8,12],\"min_interval\":3600000.0,\"max_interval\":43200000.0}},{\"type\":\"object\",\"name\":\"DaysTicker\",\"id\":\"p1085\",\"attributes\":{\"days\":[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31]}},{\"type\":\"object\",\"name\":\"DaysTicker\",\"id\":\"p1086\",\"attributes\":{\"days\":[1,4,7,10,13,16,19,22,25,28]}},{\"type\":\"object\",\"name\":\"DaysTicker\",\"id\":\"p1087\",\"attributes\":{\"days\":[1,8,15,22]}},{\"type\":\"object\",\"name\":\"DaysTicker\",\"id\":\"p1088\",\"attributes\":{\"days\":[1,15]}},{\"type\":\"object\",\"name\":\"MonthsTicker\",\"id\":\"p1089\",\"attributes\":{\"months\":[0,1,2,3,4,5,6,7,8,9,10,11]}},{\"type\":\"object\",\"name\":\"MonthsTicker\",\"id\":\"p1090\",\"attributes\":{\"months\":[0,2,4,6,8,10]}},{\"type\":\"object\",\"name\":\"MonthsTicker\",\"id\":\"p1091\",\"attributes\":{\"months\":[0,4,8]}},{\"type\":\"object\",\"name\":\"MonthsTicker\",\"id\":\"p1092\",\"attributes\":{\"months\":[0,6]}},{\"type\":\"object\",\"name\":\"YearsTicker\",\"id\":\"p1093\"}]}},\"formatter\":{\"type\":\"object\",\"name\":\"DatetimeTickFormatter\",\"id\":\"p1094\"},\"axis_label\":\"timestamp\",\"major_label_policy\":{\"type\":\"object\",\"name\":\"AllLabels\",\"id\":\"p1095\"}}}],\"center\":[{\"type\":\"object\",\"name\":\"Grid\",\"id\":\"p1096\",\"attributes\":{\"axis\":{\"id\":\"p1080\"}}},{\"type\":\"object\",\"name\":\"Grid\",\"id\":\"p1101\",\"attributes\":{\"dimension\":1,\"axis\":{\"id\":\"p1097\"}}}]}},{\"type\":\"object\",\"name\":\"Figure\",\"id\":\"p1131\",\"attributes\":{\"width\":400,\"height\":220,\"x_range\":{\"type\":\"object\",\"name\":\"Range1d\",\"id\":\"p1141\",\"attributes\":{\"start\":1546300620000.0,\"end\":1546302000000.0}},\"y_range\":{\"type\":\"object\",\"name\":\"Range1d\",\"id\":\"p1142\",\"attributes\":{\"start\":-5,\"end\":37}},\"x_scale\":{\"type\":\"object\",\"name\":\"LinearScale\",\"id\":\"p1143\"},\"y_scale\":{\"type\":\"object\",\"name\":\"LinearScale\",\"id\":\"p1144\"},\"title\":{\"type\":\"object\",\"name\":\"Title\",\"id\":\"p1134\",\"attributes\":{\"text\":\"value\"}},\"renderers\":[{\"type\":\"object\",\"name\":\"GlyphRenderer\",\"id\":\"p1184\",\"attributes\":{\"data_source\":{\"type\":\"object\",\"name\":\"ColumnDataSource\",\"id\":\"p1178\",\"attributes\":{\"selected\":{\"type\":\"object\",\"name\":\"Selection\",\"id\":\"p1179\",\"attributes\":{\"indices\":[],\"line_indices\":[]}},\"selection_policy\":{\"type\":\"object\",\"name\":\"UnionRenderers\",\"id\":\"p1180\"},\"data\":{\"type\":\"map\",\"entries\":[[\"x\",[1546301220000.0,1546301400000.0,1546301520000.0]],[\"y\",[-1,5,14]]]}}},\"view\":{\"type\":\"object\",\"name\":\"CDSView\",\"id\":\"p1185\",\"attributes\":{\"filter\":{\"type\":\"object\",\"name\":\"AllIndices\",\"id\":\"p1186\"}}},\"glyph\":{\"type\":\"object\",\"name\":\"Step\",\"id\":\"p1181\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"line_color\":\"#1f77b4\",\"line_width\":2,\"line_dash\":[4,4],\"mode\":\"after\"}},\"nonselection_glyph\":{\"type\":\"object\",\"name\":\"Step\",\"id\":\"p1182\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"line_color\":\"#1f77b4\",\"line_alpha\":0.1,\"line_width\":2,\"line_dash\":[4,4],\"mode\":\"after\"}},\"muted_glyph\":{\"type\":\"object\",\"name\":\"Step\",\"id\":\"p1183\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"line_color\":\"#1f77b4\",\"line_alpha\":0.2,\"line_width\":2,\"line_dash\":[4,4],\"mode\":\"after\"}}}},{\"type\":\"object\",\"name\":\"GlyphRenderer\",\"id\":\"p1193\",\"attributes\":{\"data_source\":{\"type\":\"object\",\"name\":\"ColumnDataSource\",\"id\":\"p1187\",\"attributes\":{\"selected\":{\"type\":\"object\",\"name\":\"Selection\",\"id\":\"p1188\",\"attributes\":{\"indices\":[],\"line_indices\":[]}},\"selection_policy\":{\"type\":\"object\",\"name\":\"UnionRenderers\",\"id\":\"p1189\"},\"data\":{\"type\":\"map\",\"entries\":[[\"x\",[1546301220000.0,1546301400000.0,1546301520000.0]],[\"y\",[-1,5,14]]]}}},\"view\":{\"type\":\"object\",\"name\":\"CDSView\",\"id\":\"p1194\",\"attributes\":{\"filter\":{\"type\":\"object\",\"name\":\"AllIndices\",\"id\":\"p1195\"}}},\"glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1190\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"size\":{\"type\":\"value\",\"value\":6},\"line_color\":{\"type\":\"value\",\"value\":\"#1f77b4\"},\"fill_color\":{\"type\":\"value\",\"value\":\"red\"}}},\"nonselection_glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1191\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"size\":{\"type\":\"value\",\"value\":6},\"line_color\":{\"type\":\"value\",\"value\":\"#1f77b4\"},\"line_alpha\":{\"type\":\"value\",\"value\":0.1},\"fill_color\":{\"type\":\"value\",\"value\":\"red\"},\"fill_alpha\":{\"type\":\"value\",\"value\":0.1},\"hatch_alpha\":{\"type\":\"value\",\"value\":0.1}}},\"muted_glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1192\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"size\":{\"type\":\"value\",\"value\":6},\"line_color\":{\"type\":\"value\",\"value\":\"#1f77b4\"},\"line_alpha\":{\"type\":\"value\",\"value\":0.2},\"fill_color\":{\"type\":\"value\",\"value\":\"red\"},\"fill_alpha\":{\"type\":\"value\",\"value\":0.2},\"hatch_alpha\":{\"type\":\"value\",\"value\":0.2}}}}}],\"toolbar\":{\"type\":\"object\",\"name\":\"Toolbar\",\"id\":\"p1140\",\"attributes\":{\"tools\":[{\"type\":\"object\",\"name\":\"PanTool\",\"id\":\"p1167\"},{\"type\":\"object\",\"name\":\"WheelZoomTool\",\"id\":\"p1168\",\"attributes\":{\"renderers\":\"auto\"}},{\"type\":\"object\",\"name\":\"BoxZoomTool\",\"id\":\"p1169\",\"attributes\":{\"overlay\":{\"type\":\"object\",\"name\":\"BoxAnnotation\",\"id\":\"p1170\",\"attributes\":{\"syncable\":false,\"level\":\"overlay\",\"visible\":false,\"left\":{\"type\":\"number\",\"value\":\"nan\"},\"right\":{\"type\":\"number\",\"value\":\"nan\"},\"top\":{\"type\":\"number\",\"value\":\"nan\"},\"bottom\":{\"type\":\"number\",\"value\":\"nan\"},\"left_units\":\"canvas\",\"right_units\":\"canvas\",\"top_units\":\"canvas\",\"bottom_units\":\"canvas\",\"line_color\":\"black\",\"line_alpha\":1.0,\"line_width\":2,\"line_dash\":[4,4],\"fill_color\":\"lightgrey\",\"fill_alpha\":0.5}}}},{\"type\":\"object\",\"name\":\"SaveTool\",\"id\":\"p1175\"},{\"type\":\"object\",\"name\":\"ResetTool\",\"id\":\"p1176\"},{\"type\":\"object\",\"name\":\"HelpTool\",\"id\":\"p1177\"}]}},\"left\":[{\"type\":\"object\",\"name\":\"LinearAxis\",\"id\":\"p1162\",\"attributes\":{\"ticker\":{\"type\":\"object\",\"name\":\"BasicTicker\",\"id\":\"p1163\",\"attributes\":{\"mantissas\":[1,2,5]}},\"formatter\":{\"type\":\"object\",\"name\":\"BasicTickFormatter\",\"id\":\"p1164\"},\"major_label_policy\":{\"type\":\"object\",\"name\":\"AllLabels\",\"id\":\"p1165\"}}}],\"below\":[{\"type\":\"object\",\"name\":\"DatetimeAxis\",\"id\":\"p1145\",\"attributes\":{\"ticker\":{\"type\":\"object\",\"name\":\"DatetimeTicker\",\"id\":\"p1146\",\"attributes\":{\"num_minor_ticks\":5,\"tickers\":[{\"type\":\"object\",\"name\":\"AdaptiveTicker\",\"id\":\"p1147\",\"attributes\":{\"num_minor_ticks\":0,\"mantissas\":[1,2,5],\"max_interval\":500.0}},{\"type\":\"object\",\"name\":\"AdaptiveTicker\",\"id\":\"p1148\",\"attributes\":{\"num_minor_ticks\":0,\"base\":60,\"mantissas\":[1,2,5,10,15,20,30],\"min_interval\":1000.0,\"max_interval\":1800000.0}},{\"type\":\"object\",\"name\":\"AdaptiveTicker\",\"id\":\"p1149\",\"attributes\":{\"num_minor_ticks\":0,\"base\":24,\"mantissas\":[1,2,4,6,8,12],\"min_interval\":3600000.0,\"max_interval\":43200000.0}},{\"type\":\"object\",\"name\":\"DaysTicker\",\"id\":\"p1150\",\"attributes\":{\"days\":[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31]}},{\"type\":\"object\",\"name\":\"DaysTicker\",\"id\":\"p1151\",\"attributes\":{\"days\":[1,4,7,10,13,16,19,22,25,28]}},{\"type\":\"object\",\"name\":\"DaysTicker\",\"id\":\"p1152\",\"attributes\":{\"days\":[1,8,15,22]}},{\"type\":\"object\",\"name\":\"DaysTicker\",\"id\":\"p1153\",\"attributes\":{\"days\":[1,15]}},{\"type\":\"object\",\"name\":\"MonthsTicker\",\"id\":\"p1154\",\"attributes\":{\"months\":[0,1,2,3,4,5,6,7,8,9,10,11]}},{\"type\":\"object\",\"name\":\"MonthsTicker\",\"id\":\"p1155\",\"attributes\":{\"months\":[0,2,4,6,8,10]}},{\"type\":\"object\",\"name\":\"MonthsTicker\",\"id\":\"p1156\",\"attributes\":{\"months\":[0,4,8]}},{\"type\":\"object\",\"name\":\"MonthsTicker\",\"id\":\"p1157\",\"attributes\":{\"months\":[0,6]}},{\"type\":\"object\",\"name\":\"YearsTicker\",\"id\":\"p1158\"}]}},\"formatter\":{\"type\":\"object\",\"name\":\"DatetimeTickFormatter\",\"id\":\"p1159\"},\"axis_label\":\"timestamp\",\"major_label_policy\":{\"type\":\"object\",\"name\":\"AllLabels\",\"id\":\"p1160\"}}}],\"center\":[{\"type\":\"object\",\"name\":\"Grid\",\"id\":\"p1161\",\"attributes\":{\"axis\":{\"id\":\"p1145\"}}},{\"type\":\"object\",\"name\":\"Grid\",\"id\":\"p1166\",\"attributes\":{\"dimension\":1,\"axis\":{\"id\":\"p1162\"}}}]}},{\"type\":\"object\",\"name\":\"Figure\",\"id\":\"p1196\",\"attributes\":{\"width\":400,\"height\":220,\"x_range\":{\"type\":\"object\",\"name\":\"Range1d\",\"id\":\"p1206\",\"attributes\":{\"start\":1546300620000.0,\"end\":1546302000000.0}},\"y_range\":{\"type\":\"object\",\"name\":\"Range1d\",\"id\":\"p1207\",\"attributes\":{\"start\":-5,\"end\":37}},\"x_scale\":{\"type\":\"object\",\"name\":\"LinearScale\",\"id\":\"p1208\"},\"y_scale\":{\"type\":\"object\",\"name\":\"LinearScale\",\"id\":\"p1209\"},\"title\":{\"type\":\"object\",\"name\":\"Title\",\"id\":\"p1199\",\"attributes\":{\"text\":\"value\"}},\"renderers\":[{\"type\":\"object\",\"name\":\"GlyphRenderer\",\"id\":\"p1249\",\"attributes\":{\"data_source\":{\"type\":\"object\",\"name\":\"ColumnDataSource\",\"id\":\"p1243\",\"attributes\":{\"selected\":{\"type\":\"object\",\"name\":\"Selection\",\"id\":\"p1244\",\"attributes\":{\"indices\":[],\"line_indices\":[]}},\"selection_policy\":{\"type\":\"object\",\"name\":\"UnionRenderers\",\"id\":\"p1245\"},\"data\":{\"type\":\"map\",\"entries\":[[\"x\",[1546300800000.0,1546301220000.0,1546301400000.0,1546301520000.0,1546301700000.0]],[\"y\",[10,9,25,34,24]]]}}},\"view\":{\"type\":\"object\",\"name\":\"CDSView\",\"id\":\"p1250\",\"attributes\":{\"filter\":{\"type\":\"object\",\"name\":\"AllIndices\",\"id\":\"p1251\"}}},\"glyph\":{\"type\":\"object\",\"name\":\"Step\",\"id\":\"p1246\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"line_color\":\"#1f77b4\",\"line_width\":2,\"line_dash\":[4,4],\"mode\":\"after\"}},\"nonselection_glyph\":{\"type\":\"object\",\"name\":\"Step\",\"id\":\"p1247\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"line_color\":\"#1f77b4\",\"line_alpha\":0.1,\"line_width\":2,\"line_dash\":[4,4],\"mode\":\"after\"}},\"muted_glyph\":{\"type\":\"object\",\"name\":\"Step\",\"id\":\"p1248\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"line_color\":\"#1f77b4\",\"line_alpha\":0.2,\"line_width\":2,\"line_dash\":[4,4],\"mode\":\"after\"}}}},{\"type\":\"object\",\"name\":\"GlyphRenderer\",\"id\":\"p1258\",\"attributes\":{\"data_source\":{\"type\":\"object\",\"name\":\"ColumnDataSource\",\"id\":\"p1252\",\"attributes\":{\"selected\":{\"type\":\"object\",\"name\":\"Selection\",\"id\":\"p1253\",\"attributes\":{\"indices\":[],\"line_indices\":[]}},\"selection_policy\":{\"type\":\"object\",\"name\":\"UnionRenderers\",\"id\":\"p1254\"},\"data\":{\"type\":\"map\",\"entries\":[[\"x\",[1546300800000.0,1546301220000.0,1546301400000.0,1546301520000.0,1546301700000.0]],[\"y\",[10,9,25,34,24]]]}}},\"view\":{\"type\":\"object\",\"name\":\"CDSView\",\"id\":\"p1259\",\"attributes\":{\"filter\":{\"type\":\"object\",\"name\":\"AllIndices\",\"id\":\"p1260\"}}},\"glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1255\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"size\":{\"type\":\"value\",\"value\":6},\"line_color\":{\"type\":\"value\",\"value\":\"#1f77b4\"},\"fill_color\":{\"type\":\"value\",\"value\":\"red\"}}},\"nonselection_glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1256\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"size\":{\"type\":\"value\",\"value\":6},\"line_color\":{\"type\":\"value\",\"value\":\"#1f77b4\"},\"line_alpha\":{\"type\":\"value\",\"value\":0.1},\"fill_color\":{\"type\":\"value\",\"value\":\"red\"},\"fill_alpha\":{\"type\":\"value\",\"value\":0.1},\"hatch_alpha\":{\"type\":\"value\",\"value\":0.1}}},\"muted_glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1257\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"size\":{\"type\":\"value\",\"value\":6},\"line_color\":{\"type\":\"value\",\"value\":\"#1f77b4\"},\"line_alpha\":{\"type\":\"value\",\"value\":0.2},\"fill_color\":{\"type\":\"value\",\"value\":\"red\"},\"fill_alpha\":{\"type\":\"value\",\"value\":0.2},\"hatch_alpha\":{\"type\":\"value\",\"value\":0.2}}}}}],\"toolbar\":{\"type\":\"object\",\"name\":\"Toolbar\",\"id\":\"p1205\",\"attributes\":{\"tools\":[{\"type\":\"object\",\"name\":\"PanTool\",\"id\":\"p1232\"},{\"type\":\"object\",\"name\":\"WheelZoomTool\",\"id\":\"p1233\",\"attributes\":{\"renderers\":\"auto\"}},{\"type\":\"object\",\"name\":\"BoxZoomTool\",\"id\":\"p1234\",\"attributes\":{\"overlay\":{\"type\":\"object\",\"name\":\"BoxAnnotation\",\"id\":\"p1235\",\"attributes\":{\"syncable\":false,\"level\":\"overlay\",\"visible\":false,\"left\":{\"type\":\"number\",\"value\":\"nan\"},\"right\":{\"type\":\"number\",\"value\":\"nan\"},\"top\":{\"type\":\"number\",\"value\":\"nan\"},\"bottom\":{\"type\":\"number\",\"value\":\"nan\"},\"left_units\":\"canvas\",\"right_units\":\"canvas\",\"top_units\":\"canvas\",\"bottom_units\":\"canvas\",\"line_color\":\"black\",\"line_alpha\":1.0,\"line_width\":2,\"line_dash\":[4,4],\"fill_color\":\"lightgrey\",\"fill_alpha\":0.5}}}},{\"type\":\"object\",\"name\":\"SaveTool\",\"id\":\"p1240\"},{\"type\":\"object\",\"name\":\"ResetTool\",\"id\":\"p1241\"},{\"type\":\"object\",\"name\":\"HelpTool\",\"id\":\"p1242\"}]}},\"left\":[{\"type\":\"object\",\"name\":\"LinearAxis\",\"id\":\"p1227\",\"attributes\":{\"ticker\":{\"type\":\"object\",\"name\":\"BasicTicker\",\"id\":\"p1228\",\"attributes\":{\"mantissas\":[1,2,5]}},\"formatter\":{\"type\":\"object\",\"name\":\"BasicTickFormatter\",\"id\":\"p1229\"},\"major_label_policy\":{\"type\":\"object\",\"name\":\"AllLabels\",\"id\":\"p1230\"}}}],\"below\":[{\"type\":\"object\",\"name\":\"DatetimeAxis\",\"id\":\"p1210\",\"attributes\":{\"ticker\":{\"type\":\"object\",\"name\":\"DatetimeTicker\",\"id\":\"p1211\",\"attributes\":{\"num_minor_ticks\":5,\"tickers\":[{\"type\":\"object\",\"name\":\"AdaptiveTicker\",\"id\":\"p1212\",\"attributes\":{\"num_minor_ticks\":0,\"mantissas\":[1,2,5],\"max_interval\":500.0}},{\"type\":\"object\",\"name\":\"AdaptiveTicker\",\"id\":\"p1213\",\"attributes\":{\"num_minor_ticks\":0,\"base\":60,\"mantissas\":[1,2,5,10,15,20,30],\"min_interval\":1000.0,\"max_interval\":1800000.0}},{\"type\":\"object\",\"name\":\"AdaptiveTicker\",\"id\":\"p1214\",\"attributes\":{\"num_minor_ticks\":0,\"base\":24,\"mantissas\":[1,2,4,6,8,12],\"min_interval\":3600000.0,\"max_interval\":43200000.0}},{\"type\":\"object\",\"name\":\"DaysTicker\",\"id\":\"p1215\",\"attributes\":{\"days\":[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31]}},{\"type\":\"object\",\"name\":\"DaysTicker\",\"id\":\"p1216\",\"attributes\":{\"days\":[1,4,7,10,13,16,19,22,25,28]}},{\"type\":\"object\",\"name\":\"DaysTicker\",\"id\":\"p1217\",\"attributes\":{\"days\":[1,8,15,22]}},{\"type\":\"object\",\"name\":\"DaysTicker\",\"id\":\"p1218\",\"attributes\":{\"days\":[1,15]}},{\"type\":\"object\",\"name\":\"MonthsTicker\",\"id\":\"p1219\",\"attributes\":{\"months\":[0,1,2,3,4,5,6,7,8,9,10,11]}},{\"type\":\"object\",\"name\":\"MonthsTicker\",\"id\":\"p1220\",\"attributes\":{\"months\":[0,2,4,6,8,10]}},{\"type\":\"object\",\"name\":\"MonthsTicker\",\"id\":\"p1221\",\"attributes\":{\"months\":[0,4,8]}},{\"type\":\"object\",\"name\":\"MonthsTicker\",\"id\":\"p1222\",\"attributes\":{\"months\":[0,6]}},{\"type\":\"object\",\"name\":\"YearsTicker\",\"id\":\"p1223\"}]}},\"formatter\":{\"type\":\"object\",\"name\":\"DatetimeTickFormatter\",\"id\":\"p1224\"},\"axis_label\":\"timestamp\",\"major_label_policy\":{\"type\":\"object\",\"name\":\"AllLabels\",\"id\":\"p1225\"}}}],\"center\":[{\"type\":\"object\",\"name\":\"Grid\",\"id\":\"p1226\",\"attributes\":{\"axis\":{\"id\":\"p1210\"}}},{\"type\":\"object\",\"name\":\"Grid\",\"id\":\"p1231\",\"attributes\":{\"dimension\":1,\"axis\":{\"id\":\"p1227\"}}}]}}]}}]}};\n",
+                            "  const render_items = [{\"docid\":\"f84e2a8a-d2f7-43a1-94d5-04f0cb83641c\",\"roots\":{\"p1261\":\"e9117200-8ad9-48ec-a404-f7fcbf924171\"},\"root_ids\":[\"p1261\"]}];\n",
+                            "  void root.Bokeh.embed.embed_items_notebook(docs_json, render_items);\n",
                             "  }\n",
                             "  if (root.Bokeh !== undefined) {\n",
                             "    embed_document(root);\n",
                             "  } else {\n",
-                            "    var attempts = 0;\n",
-                            "    var timer = setInterval(function(root) {\n",
+                            "    let attempts = 0;\n",
+                            "    const timer = setInterval(function(root) {\n",
                             "      if (root.Bokeh !== undefined) {\n",
-                            "        embed_document(root);\n",
-                            "        clearInterval(timer);\n",
-                            "      }\n",
-                            "      attempts++;\n",
-                            "      if (attempts > 100) {\n",
-                            "        console.log(\"Bokeh: ERROR: Unable to run BokehJS code because BokehJS library is missing\");\n",
                             "        clearInterval(timer);\n",
+                            "        embed_document(root);\n",
+                            "      } else {\n",
+                            "        attempts++;\n",
+                            "        if (attempts > 100) {\n",
+                            "          clearInterval(timer);\n",
+                            "          console.log(\"Bokeh: ERROR: Unable to run BokehJS code because BokehJS library is missing\");\n",
+                            "        }\n",
                             "      }\n",
                             "    }, 10, root)\n",
                             "  }\n",
                             "})(window);"
                         ],
                         "application/vnd.bokehjs_exec.v0+json": ""
                     },
                     "metadata": {
                         "application/vnd.bokehjs_exec.v0+json": {
-                            "id": "4763"
+                            "id": "p1261"
                         }
                     },
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "# Let's visualize it\n",
@@ -645,188 +682,176 @@
                 "## Switching worlds\n",
                 "\n",
                 "From unevenly-spaced to evenly-spaced"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 35,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "\n",
-                            "\n",
-                            "\n",
-                            "\n",
-                            "\n",
-                            "\n",
-                            "  <div class=\"bk-root\" id=\"6c489570-e46f-4a61-99b0-e54e783ee6b9\" data-root-id=\"5490\"></div>\n"
+                            "  <div id=\"aaae0036-aad8-4b25-9a13-25835eae8831\" data-root-id=\"p1262\" style=\"display: contents;\"></div>\n"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/javascript": [
                             "(function(root) {\n",
                             "  function embed_document(root) {\n",
-                            "    \n",
-                            "  var docs_json = {\"75d9092b-3216-4a3c-a413-233f1cad1900\":{\"roots\":{\"references\":[{\"attributes\":{\"below\":[{\"id\":\"5501\",\"type\":\"DatetimeAxis\"}],\"center\":[{\"id\":\"5505\",\"type\":\"Grid\"},{\"id\":\"5510\",\"type\":\"Grid\"}],\"left\":[{\"id\":\"5506\",\"type\":\"LinearAxis\"}],\"plot_height\":220,\"plot_width\":400,\"renderers\":[{\"id\":\"5527\",\"type\":\"GlyphRenderer\"},{\"id\":\"5532\",\"type\":\"GlyphRenderer\"}],\"title\":{\"id\":\"5491\",\"type\":\"Title\"},\"toolbar\":{\"id\":\"5517\",\"type\":\"Toolbar\"},\"x_range\":{\"id\":\"5493\",\"type\":\"Range1d\"},\"x_scale\":{\"id\":\"5497\",\"type\":\"LinearScale\"},\"y_range\":{\"id\":\"5495\",\"type\":\"Range1d\"},\"y_scale\":{\"id\":\"5499\",\"type\":\"LinearScale\"}},\"id\":\"5490\",\"subtype\":\"Figure\",\"type\":\"Plot\"},{\"attributes\":{},\"id\":\"5867\",\"type\":\"BasicTickFormatter\"},{\"attributes\":{\"dimension\":1,\"ticker\":{\"id\":\"5507\",\"type\":\"BasicTicker\"}},\"id\":\"5510\",\"type\":\"Grid\"},{\"attributes\":{\"mantissas\":[1,2,5],\"max_interval\":500.0,\"num_minor_ticks\":0},\"id\":\"5869\",\"type\":\"AdaptiveTicker\"},{\"attributes\":{\"line_alpha\":{\"value\":0.1},\"line_color\":{\"value\":\"#1f77b4\"},\"line_dash\":[4,4],\"line_width\":{\"value\":2},\"mode\":\"after\",\"x\":{\"field\":\"x\"},\"y\":{\"field\":\"y\"}},\"id\":\"5526\",\"type\":\"Step\"},{\"attributes\":{\"line_color\":{\"value\":\"#1f77b4\"},\"line_dash\":[4,4],\"line_width\":{\"value\":2},\"mode\":\"after\",\"x\":{\"field\":\"x\"},\"y\":{\"field\":\"y\"}},\"id\":\"5525\",\"type\":\"Step\"},{\"attributes\":{\"base\":60,\"mantissas\":[1,2,5,10,15,20,30],\"max_interval\":1800000.0,\"min_interval\":1000.0,\"num_minor_ticks\":0},\"id\":\"5870\",\"type\":\"AdaptiveTicker\"},{\"attributes\":{\"active_drag\":\"auto\",\"active_inspect\":\"auto\",\"active_multi\":null,\"active_scroll\":\"auto\",\"active_tap\":\"auto\",\"tools\":[{\"id\":\"5511\",\"type\":\"PanTool\"},{\"id\":\"5512\",\"type\":\"WheelZoomTool\"},{\"id\":\"5513\",\"type\":\"BoxZoomTool\"},{\"id\":\"5514\",\"type\":\"SaveTool\"},{\"id\":\"5515\",\"type\":\"ResetTool\"},{\"id\":\"5516\",\"type\":\"HelpTool\"}]},\"id\":\"5517\",\"type\":\"Toolbar\"},{\"attributes\":{\"base\":24,\"mantissas\":[1,2,4,6,8,12],\"max_interval\":43200000.0,\"min_interval\":3600000.0,\"num_minor_ticks\":0},\"id\":\"5871\",\"type\":\"AdaptiveTicker\"},{\"attributes\":{\"callback\":null,\"end\":37,\"start\":-5},\"id\":\"5495\",\"type\":\"Range1d\"},{\"attributes\":{},\"id\":\"5511\",\"type\":\"PanTool\"},{\"attributes\":{\"days\":[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31]},\"id\":\"5872\",\"type\":\"DaysTicker\"},{\"attributes\":{},\"id\":\"5512\",\"type\":\"WheelZoomTool\"},{\"attributes\":{\"days\":[1,4,7,10,13,16,19,22,25,28]},\"id\":\"5873\",\"type\":\"DaysTicker\"},{\"attributes\":{\"overlay\":{\"id\":\"5885\",\"type\":\"BoxAnnotation\"}},\"id\":\"5513\",\"type\":\"BoxZoomTool\"},{\"attributes\":{\"days\":[1,8,15,22]},\"id\":\"5874\",\"type\":\"DaysTicker\"},{\"attributes\":{},\"id\":\"5514\",\"type\":\"SaveTool\"},{\"attributes\":{\"days\":[1,15]},\"id\":\"5875\",\"type\":\"DaysTicker\"},{\"attributes\":{},\"id\":\"5515\",\"type\":\"ResetTool\"},{\"attributes\":{\"months\":[0,1,2,3,4,5,6,7,8,9,10,11]},\"id\":\"5876\",\"type\":\"MonthsTicker\"},{\"attributes\":{},\"id\":\"5516\",\"type\":\"HelpTool\"},{\"attributes\":{\"months\":[0,2,4,6,8,10]},\"id\":\"5877\",\"type\":\"MonthsTicker\"},{\"attributes\":{\"bottom_units\":\"screen\",\"fill_alpha\":{\"value\":0.5},\"fill_color\":{\"value\":\"lightgrey\"},\"left_units\":\"screen\",\"level\":\"overlay\",\"line_alpha\":{\"value\":1.0},\"line_color\":{\"value\":\"black\"},\"line_dash\":[4,4],\"line_width\":{\"value\":2},\"render_mode\":\"css\",\"right_units\":\"screen\",\"top_units\":\"screen\"},\"id\":\"5885\",\"type\":\"BoxAnnotation\"},{\"attributes\":{\"text\":\"value\"},\"id\":\"5491\",\"type\":\"Title\"},{\"attributes\":{},\"id\":\"5865\",\"type\":\"DatetimeTickFormatter\"},{\"attributes\":{\"months\":[0,4,8]},\"id\":\"5878\",\"type\":\"MonthsTicker\"},{\"attributes\":{},\"id\":\"5497\",\"type\":\"LinearScale\"},{\"attributes\":{\"data_source\":{\"id\":\"5524\",\"type\":\"ColumnDataSource\"},\"glyph\":{\"id\":\"5525\",\"type\":\"Step\"},\"hover_glyph\":null,\"muted_glyph\":null,\"nonselection_glyph\":{\"id\":\"5526\",\"type\":\"Step\"},\"selection_glyph\":null,\"view\":{\"id\":\"5528\",\"type\":\"CDSView\"}},\"id\":\"5527\",\"type\":\"GlyphRenderer\"},{\"attributes\":{},\"id\":\"5499\",\"type\":\"LinearScale\"},{\"attributes\":{\"callback\":null,\"data\":{\"x\":[1546300800000.0,1546300860000.0,1546300920000.0,1546300980000.0,1546301040000.0,1546301100000.0,1546301160000.0,1546301220000.0,1546301280000.0,1546301340000.0,1546301400000.0,1546301460000.0,1546301520000.0,1546301580000.0,1546301640000.0,1546301700000.0],\"y\":[10,10,10,10,10,10,10,10,10,10,20,20,20,20,20,10]},\"selected\":{\"id\":\"5882\",\"type\":\"Selection\"},\"selection_policy\":{\"id\":\"5881\",\"type\":\"UnionRenderers\"}},\"id\":\"5524\",\"type\":\"ColumnDataSource\"},{\"attributes\":{\"source\":{\"id\":\"5524\",\"type\":\"ColumnDataSource\"}},\"id\":\"5528\",\"type\":\"CDSView\"},{\"attributes\":{\"months\":[0,6]},\"id\":\"5879\",\"type\":\"MonthsTicker\"},{\"attributes\":{},\"id\":\"5880\",\"type\":\"YearsTicker\"},{\"attributes\":{\"callback\":null,\"data\":{\"x\":[1546300800000.0,1546300860000.0,1546300920000.0,1546300980000.0,1546301040000.0,1546301100000.0,1546301160000.0,1546301220000.0,1546301280000.0,1546301340000.0,1546301400000.0,1546301460000.0,1546301520000.0,1546301580000.0,1546301640000.0,1546301700000.0],\"y\":[10,10,10,10,10,10,10,10,10,10,20,20,20,20,20,10]},\"selected\":{\"id\":\"5884\",\"type\":\"Selection\"},\"selection_policy\":{\"id\":\"5883\",\"type\":\"UnionRenderers\"}},\"id\":\"5529\",\"type\":\"ColumnDataSource\"},{\"attributes\":{},\"id\":\"5507\",\"type\":\"BasicTicker\"},{\"attributes\":{},\"id\":\"5881\",\"type\":\"UnionRenderers\"},{\"attributes\":{\"fill_color\":{\"value\":\"red\"},\"line_color\":{\"value\":\"#1f77b4\"},\"size\":{\"units\":\"screen\",\"value\":6},\"x\":{\"field\":\"x\"},\"y\":{\"field\":\"y\"}},\"id\":\"5530\",\"type\":\"Circle\"},{\"attributes\":{\"fill_alpha\":{\"value\":0.1},\"fill_color\":{\"value\":\"#1f77b4\"},\"line_alpha\":{\"value\":0.1},\"line_color\":{\"value\":\"#1f77b4\"},\"size\":{\"units\":\"screen\",\"value\":6},\"x\":{\"field\":\"x\"},\"y\":{\"field\":\"y\"}},\"id\":\"5531\",\"type\":\"Circle\"},{\"attributes\":{},\"id\":\"5882\",\"type\":\"Selection\"},{\"attributes\":{\"axis_label\":\"timestamp\",\"formatter\":{\"id\":\"5865\",\"type\":\"DatetimeTickFormatter\"},\"ticker\":{\"id\":\"5502\",\"type\":\"DatetimeTicker\"}},\"id\":\"5501\",\"type\":\"DatetimeAxis\"},{\"attributes\":{},\"id\":\"5883\",\"type\":\"UnionRenderers\"},{\"attributes\":{\"data_source\":{\"id\":\"5529\",\"type\":\"ColumnDataSource\"},\"glyph\":{\"id\":\"5530\",\"type\":\"Circle\"},\"hover_glyph\":null,\"muted_glyph\":null,\"nonselection_glyph\":{\"id\":\"5531\",\"type\":\"Circle\"},\"selection_glyph\":null,\"view\":{\"id\":\"5533\",\"type\":\"CDSView\"}},\"id\":\"5532\",\"type\":\"GlyphRenderer\"},{\"attributes\":{\"num_minor_ticks\":5,\"tickers\":[{\"id\":\"5869\",\"type\":\"AdaptiveTicker\"},{\"id\":\"5870\",\"type\":\"AdaptiveTicker\"},{\"id\":\"5871\",\"type\":\"AdaptiveTicker\"},{\"id\":\"5872\",\"type\":\"DaysTicker\"},{\"id\":\"5873\",\"type\":\"DaysTicker\"},{\"id\":\"5874\",\"type\":\"DaysTicker\"},{\"id\":\"5875\",\"type\":\"DaysTicker\"},{\"id\":\"5876\",\"type\":\"MonthsTicker\"},{\"id\":\"5877\",\"type\":\"MonthsTicker\"},{\"id\":\"5878\",\"type\":\"MonthsTicker\"},{\"id\":\"5879\",\"type\":\"MonthsTicker\"},{\"id\":\"5880\",\"type\":\"YearsTicker\"}]},\"id\":\"5502\",\"type\":\"DatetimeTicker\"},{\"attributes\":{\"ticker\":{\"id\":\"5502\",\"type\":\"DatetimeTicker\"}},\"id\":\"5505\",\"type\":\"Grid\"},{\"attributes\":{\"formatter\":{\"id\":\"5867\",\"type\":\"BasicTickFormatter\"},\"ticker\":{\"id\":\"5507\",\"type\":\"BasicTicker\"}},\"id\":\"5506\",\"type\":\"LinearAxis\"},{\"attributes\":{},\"id\":\"5884\",\"type\":\"Selection\"},{\"attributes\":{\"source\":{\"id\":\"5529\",\"type\":\"ColumnDataSource\"}},\"id\":\"5533\",\"type\":\"CDSView\"},{\"attributes\":{\"callback\":null,\"end\":1546302000000.0,\"start\":1546300620000.0},\"id\":\"5493\",\"type\":\"Range1d\"}],\"root_ids\":[\"5490\"]},\"title\":\"Bokeh Application\",\"version\":\"1.3.1\"}};\n",
-                            "  var render_items = [{\"docid\":\"75d9092b-3216-4a3c-a413-233f1cad1900\",\"roots\":{\"5490\":\"6c489570-e46f-4a61-99b0-e54e783ee6b9\"}}];\n",
-                            "  root.Bokeh.embed.embed_items_notebook(docs_json, render_items);\n",
-                            "\n",
+                            "  const docs_json = {\"5d53cdfa-931c-49ed-8c5c-c7efcaaceb21\":{\"version\":\"3.4.1\",\"title\":\"Bokeh Application\",\"roots\":[{\"type\":\"object\",\"name\":\"Figure\",\"id\":\"p1262\",\"attributes\":{\"width\":400,\"height\":220,\"x_range\":{\"type\":\"object\",\"name\":\"Range1d\",\"id\":\"p1272\",\"attributes\":{\"start\":1546300620000.0,\"end\":1546302000000.0}},\"y_range\":{\"type\":\"object\",\"name\":\"Range1d\",\"id\":\"p1273\",\"attributes\":{\"start\":-5,\"end\":37}},\"x_scale\":{\"type\":\"object\",\"name\":\"LinearScale\",\"id\":\"p1274\"},\"y_scale\":{\"type\":\"object\",\"name\":\"LinearScale\",\"id\":\"p1275\"},\"title\":{\"type\":\"object\",\"name\":\"Title\",\"id\":\"p1265\",\"attributes\":{\"text\":\"value\"}},\"renderers\":[{\"type\":\"object\",\"name\":\"GlyphRenderer\",\"id\":\"p1315\",\"attributes\":{\"data_source\":{\"type\":\"object\",\"name\":\"ColumnDataSource\",\"id\":\"p1309\",\"attributes\":{\"selected\":{\"type\":\"object\",\"name\":\"Selection\",\"id\":\"p1310\",\"attributes\":{\"indices\":[],\"line_indices\":[]}},\"selection_policy\":{\"type\":\"object\",\"name\":\"UnionRenderers\",\"id\":\"p1311\"},\"data\":{\"type\":\"map\",\"entries\":[[\"x\",[1546300800000.0,1546300860000.0,1546300920000.0,1546300980000.0,1546301040000.0,1546301100000.0,1546301160000.0,1546301220000.0,1546301280000.0,1546301340000.0,1546301400000.0,1546301460000.0,1546301520000.0,1546301580000.0,1546301640000.0,1546301700000.0]],[\"y\",[10,10,10,10,10,10,10,10,10,10,20,20,20,20,20,10]]]}}},\"view\":{\"type\":\"object\",\"name\":\"CDSView\",\"id\":\"p1316\",\"attributes\":{\"filter\":{\"type\":\"object\",\"name\":\"AllIndices\",\"id\":\"p1317\"}}},\"glyph\":{\"type\":\"object\",\"name\":\"Step\",\"id\":\"p1312\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"line_color\":\"#1f77b4\",\"line_width\":2,\"line_dash\":[4,4],\"mode\":\"after\"}},\"nonselection_glyph\":{\"type\":\"object\",\"name\":\"Step\",\"id\":\"p1313\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"line_color\":\"#1f77b4\",\"line_alpha\":0.1,\"line_width\":2,\"line_dash\":[4,4],\"mode\":\"after\"}},\"muted_glyph\":{\"type\":\"object\",\"name\":\"Step\",\"id\":\"p1314\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"line_color\":\"#1f77b4\",\"line_alpha\":0.2,\"line_width\":2,\"line_dash\":[4,4],\"mode\":\"after\"}}}},{\"type\":\"object\",\"name\":\"GlyphRenderer\",\"id\":\"p1324\",\"attributes\":{\"data_source\":{\"type\":\"object\",\"name\":\"ColumnDataSource\",\"id\":\"p1318\",\"attributes\":{\"selected\":{\"type\":\"object\",\"name\":\"Selection\",\"id\":\"p1319\",\"attributes\":{\"indices\":[],\"line_indices\":[]}},\"selection_policy\":{\"type\":\"object\",\"name\":\"UnionRenderers\",\"id\":\"p1320\"},\"data\":{\"type\":\"map\",\"entries\":[[\"x\",[1546300800000.0,1546300860000.0,1546300920000.0,1546300980000.0,1546301040000.0,1546301100000.0,1546301160000.0,1546301220000.0,1546301280000.0,1546301340000.0,1546301400000.0,1546301460000.0,1546301520000.0,1546301580000.0,1546301640000.0,1546301700000.0]],[\"y\",[10,10,10,10,10,10,10,10,10,10,20,20,20,20,20,10]]]}}},\"view\":{\"type\":\"object\",\"name\":\"CDSView\",\"id\":\"p1325\",\"attributes\":{\"filter\":{\"type\":\"object\",\"name\":\"AllIndices\",\"id\":\"p1326\"}}},\"glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1321\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"size\":{\"type\":\"value\",\"value\":6},\"line_color\":{\"type\":\"value\",\"value\":\"#1f77b4\"},\"fill_color\":{\"type\":\"value\",\"value\":\"red\"}}},\"nonselection_glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1322\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"size\":{\"type\":\"value\",\"value\":6},\"line_color\":{\"type\":\"value\",\"value\":\"#1f77b4\"},\"line_alpha\":{\"type\":\"value\",\"value\":0.1},\"fill_color\":{\"type\":\"value\",\"value\":\"red\"},\"fill_alpha\":{\"type\":\"value\",\"value\":0.1},\"hatch_alpha\":{\"type\":\"value\",\"value\":0.1}}},\"muted_glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1323\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"size\":{\"type\":\"value\",\"value\":6},\"line_color\":{\"type\":\"value\",\"value\":\"#1f77b4\"},\"line_alpha\":{\"type\":\"value\",\"value\":0.2},\"fill_color\":{\"type\":\"value\",\"value\":\"red\"},\"fill_alpha\":{\"type\":\"value\",\"value\":0.2},\"hatch_alpha\":{\"type\":\"value\",\"value\":0.2}}}}}],\"toolbar\":{\"type\":\"object\",\"name\":\"Toolbar\",\"id\":\"p1271\",\"attributes\":{\"tools\":[{\"type\":\"object\",\"name\":\"PanTool\",\"id\":\"p1298\"},{\"type\":\"object\",\"name\":\"WheelZoomTool\",\"id\":\"p1299\",\"attributes\":{\"renderers\":\"auto\"}},{\"type\":\"object\",\"name\":\"BoxZoomTool\",\"id\":\"p1300\",\"attributes\":{\"overlay\":{\"type\":\"object\",\"name\":\"BoxAnnotation\",\"id\":\"p1301\",\"attributes\":{\"syncable\":false,\"level\":\"overlay\",\"visible\":false,\"left\":{\"type\":\"number\",\"value\":\"nan\"},\"right\":{\"type\":\"number\",\"value\":\"nan\"},\"top\":{\"type\":\"number\",\"value\":\"nan\"},\"bottom\":{\"type\":\"number\",\"value\":\"nan\"},\"left_units\":\"canvas\",\"right_units\":\"canvas\",\"top_units\":\"canvas\",\"bottom_units\":\"canvas\",\"line_color\":\"black\",\"line_alpha\":1.0,\"line_width\":2,\"line_dash\":[4,4],\"fill_color\":\"lightgrey\",\"fill_alpha\":0.5}}}},{\"type\":\"object\",\"name\":\"SaveTool\",\"id\":\"p1306\"},{\"type\":\"object\",\"name\":\"ResetTool\",\"id\":\"p1307\"},{\"type\":\"object\",\"name\":\"HelpTool\",\"id\":\"p1308\"}]}},\"left\":[{\"type\":\"object\",\"name\":\"LinearAxis\",\"id\":\"p1293\",\"attributes\":{\"ticker\":{\"type\":\"object\",\"name\":\"BasicTicker\",\"id\":\"p1294\",\"attributes\":{\"mantissas\":[1,2,5]}},\"formatter\":{\"type\":\"object\",\"name\":\"BasicTickFormatter\",\"id\":\"p1295\"},\"major_label_policy\":{\"type\":\"object\",\"name\":\"AllLabels\",\"id\":\"p1296\"}}}],\"below\":[{\"type\":\"object\",\"name\":\"DatetimeAxis\",\"id\":\"p1276\",\"attributes\":{\"ticker\":{\"type\":\"object\",\"name\":\"DatetimeTicker\",\"id\":\"p1277\",\"attributes\":{\"num_minor_ticks\":5,\"tickers\":[{\"type\":\"object\",\"name\":\"AdaptiveTicker\",\"id\":\"p1278\",\"attributes\":{\"num_minor_ticks\":0,\"mantissas\":[1,2,5],\"max_interval\":500.0}},{\"type\":\"object\",\"name\":\"AdaptiveTicker\",\"id\":\"p1279\",\"attributes\":{\"num_minor_ticks\":0,\"base\":60,\"mantissas\":[1,2,5,10,15,20,30],\"min_interval\":1000.0,\"max_interval\":1800000.0}},{\"type\":\"object\",\"name\":\"AdaptiveTicker\",\"id\":\"p1280\",\"attributes\":{\"num_minor_ticks\":0,\"base\":24,\"mantissas\":[1,2,4,6,8,12],\"min_interval\":3600000.0,\"max_interval\":43200000.0}},{\"type\":\"object\",\"name\":\"DaysTicker\",\"id\":\"p1281\",\"attributes\":{\"days\":[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31]}},{\"type\":\"object\",\"name\":\"DaysTicker\",\"id\":\"p1282\",\"attributes\":{\"days\":[1,4,7,10,13,16,19,22,25,28]}},{\"type\":\"object\",\"name\":\"DaysTicker\",\"id\":\"p1283\",\"attributes\":{\"days\":[1,8,15,22]}},{\"type\":\"object\",\"name\":\"DaysTicker\",\"id\":\"p1284\",\"attributes\":{\"days\":[1,15]}},{\"type\":\"object\",\"name\":\"MonthsTicker\",\"id\":\"p1285\",\"attributes\":{\"months\":[0,1,2,3,4,5,6,7,8,9,10,11]}},{\"type\":\"object\",\"name\":\"MonthsTicker\",\"id\":\"p1286\",\"attributes\":{\"months\":[0,2,4,6,8,10]}},{\"type\":\"object\",\"name\":\"MonthsTicker\",\"id\":\"p1287\",\"attributes\":{\"months\":[0,4,8]}},{\"type\":\"object\",\"name\":\"MonthsTicker\",\"id\":\"p1288\",\"attributes\":{\"months\":[0,6]}},{\"type\":\"object\",\"name\":\"YearsTicker\",\"id\":\"p1289\"}]}},\"formatter\":{\"type\":\"object\",\"name\":\"DatetimeTickFormatter\",\"id\":\"p1290\"},\"axis_label\":\"timestamp\",\"major_label_policy\":{\"type\":\"object\",\"name\":\"AllLabels\",\"id\":\"p1291\"}}}],\"center\":[{\"type\":\"object\",\"name\":\"Grid\",\"id\":\"p1292\",\"attributes\":{\"axis\":{\"id\":\"p1276\"}}},{\"type\":\"object\",\"name\":\"Grid\",\"id\":\"p1297\",\"attributes\":{\"dimension\":1,\"axis\":{\"id\":\"p1293\"}}}]}}]}};\n",
+                            "  const render_items = [{\"docid\":\"5d53cdfa-931c-49ed-8c5c-c7efcaaceb21\",\"roots\":{\"p1262\":\"aaae0036-aad8-4b25-9a13-25835eae8831\"},\"root_ids\":[\"p1262\"]}];\n",
+                            "  void root.Bokeh.embed.embed_items_notebook(docs_json, render_items);\n",
                             "  }\n",
                             "  if (root.Bokeh !== undefined) {\n",
                             "    embed_document(root);\n",
                             "  } else {\n",
-                            "    var attempts = 0;\n",
-                            "    var timer = setInterval(function(root) {\n",
+                            "    let attempts = 0;\n",
+                            "    const timer = setInterval(function(root) {\n",
                             "      if (root.Bokeh !== undefined) {\n",
-                            "        embed_document(root);\n",
-                            "        clearInterval(timer);\n",
-                            "      }\n",
-                            "      attempts++;\n",
-                            "      if (attempts > 100) {\n",
-                            "        console.log(\"Bokeh: ERROR: Unable to run BokehJS code because BokehJS library is missing\");\n",
                             "        clearInterval(timer);\n",
+                            "        embed_document(root);\n",
+                            "      } else {\n",
+                            "        attempts++;\n",
+                            "        if (attempts > 100) {\n",
+                            "          clearInterval(timer);\n",
+                            "          console.log(\"Bokeh: ERROR: Unable to run BokehJS code because BokehJS library is missing\");\n",
+                            "        }\n",
                             "      }\n",
                             "    }, 10, root)\n",
                             "  }\n",
                             "})(window);"
                         ],
                         "application/vnd.bokehjs_exec.v0+json": ""
                     },
                     "metadata": {
                         "application/vnd.bokehjs_exec.v0+json": {
-                            "id": "5490"
+                            "id": "p1262"
                         }
                     },
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"display: table;\"><div style=\"display: table-row;\"><div style=\"display: table-cell;\"><b title=\"bokeh.plotting.figure.Figure\">Figure</b>(</div><div style=\"display: table-cell;\">id&nbsp;=&nbsp;'5490', <span id=\"6019\" style=\"cursor: pointer;\">&hellip;)</span></div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">above&nbsp;=&nbsp;[],</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">align&nbsp;=&nbsp;'start',</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">aspect_ratio&nbsp;=&nbsp;None,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">aspect_scale&nbsp;=&nbsp;1,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">background&nbsp;=&nbsp;None,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">background_fill_alpha&nbsp;=&nbsp;{'value': 1.0},</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">background_fill_color&nbsp;=&nbsp;{'value': '#ffffff'},</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">below&nbsp;=&nbsp;[DatetimeAxis(id='5501', ...)],</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">border_fill_alpha&nbsp;=&nbsp;{'value': 1.0},</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">border_fill_color&nbsp;=&nbsp;{'value': '#ffffff'},</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">center&nbsp;=&nbsp;[Grid(id='5505', ...), Grid(id='5510', ...)],</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">css_classes&nbsp;=&nbsp;[],</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">disabled&nbsp;=&nbsp;False,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">extra_x_ranges&nbsp;=&nbsp;{},</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">extra_y_ranges&nbsp;=&nbsp;{},</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">frame_height&nbsp;=&nbsp;None,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">frame_width&nbsp;=&nbsp;None,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">height&nbsp;=&nbsp;None,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">height_policy&nbsp;=&nbsp;'auto',</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">hidpi&nbsp;=&nbsp;True,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">js_event_callbacks&nbsp;=&nbsp;{},</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">js_property_callbacks&nbsp;=&nbsp;{},</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">left&nbsp;=&nbsp;[LinearAxis(id='5506', ...)],</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">lod_factor&nbsp;=&nbsp;10,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">lod_interval&nbsp;=&nbsp;300,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">lod_threshold&nbsp;=&nbsp;2000,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">lod_timeout&nbsp;=&nbsp;500,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">margin&nbsp;=&nbsp;(0, 0, 0, 0),</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">match_aspect&nbsp;=&nbsp;False,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">max_height&nbsp;=&nbsp;None,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">max_width&nbsp;=&nbsp;None,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border&nbsp;=&nbsp;5,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border_bottom&nbsp;=&nbsp;None,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border_left&nbsp;=&nbsp;None,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border_right&nbsp;=&nbsp;None,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border_top&nbsp;=&nbsp;None,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_height&nbsp;=&nbsp;None,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_width&nbsp;=&nbsp;None,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">name&nbsp;=&nbsp;None,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_alpha&nbsp;=&nbsp;{'value': 1.0},</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_cap&nbsp;=&nbsp;'butt',</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_color&nbsp;=&nbsp;{'value': '#e5e5e5'},</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_dash&nbsp;=&nbsp;[],</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_dash_offset&nbsp;=&nbsp;0,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_join&nbsp;=&nbsp;'bevel',</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_width&nbsp;=&nbsp;{'value': 1},</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">output_backend&nbsp;=&nbsp;'canvas',</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">plot_height&nbsp;=&nbsp;220,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">plot_width&nbsp;=&nbsp;400,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">renderers&nbsp;=&nbsp;[GlyphRenderer(id='5527', ...), GlyphRenderer(id='5532', ...)],</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">reset_policy&nbsp;=&nbsp;'standard',</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">right&nbsp;=&nbsp;[],</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">sizing_mode&nbsp;=&nbsp;None,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">subscribed_events&nbsp;=&nbsp;[],</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">tags&nbsp;=&nbsp;[],</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">title&nbsp;=&nbsp;Title(id='5491', ...),</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">title_location&nbsp;=&nbsp;'above',</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">toolbar&nbsp;=&nbsp;Toolbar(id='5517', ...),</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">toolbar_location&nbsp;=&nbsp;'right',</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">toolbar_sticky&nbsp;=&nbsp;True,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">visible&nbsp;=&nbsp;True,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">width&nbsp;=&nbsp;None,</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">width_policy&nbsp;=&nbsp;'auto',</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">x_range&nbsp;=&nbsp;Range1d(id='5493', ...),</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">x_scale&nbsp;=&nbsp;LinearScale(id='5497', ...),</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">y_range&nbsp;=&nbsp;Range1d(id='5495', ...),</div></div><div class=\"6018\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">y_scale&nbsp;=&nbsp;LinearScale(id='5499', ...))</div></div></div>\n",
+                            "<div style=\"display: table;\"><div style=\"display: table-row;\"><div style=\"display: table-cell;\"><b title=\"bokeh.plotting._figure.figure\">figure</b>(</div><div style=\"display: table-cell;\">id&nbsp;=&nbsp;'p1262', <span id=\"p1328\" style=\"cursor: pointer;\">&hellip;)</span></div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">above&nbsp;=&nbsp;[],</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">align&nbsp;=&nbsp;'auto',</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">aspect_ratio&nbsp;=&nbsp;None,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">aspect_scale&nbsp;=&nbsp;1,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">attribution&nbsp;=&nbsp;[],</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">background_fill_alpha&nbsp;=&nbsp;1.0,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">background_fill_color&nbsp;=&nbsp;'#ffffff',</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">below&nbsp;=&nbsp;[DatetimeAxis(id='p1276', ...)],</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">border_fill_alpha&nbsp;=&nbsp;1.0,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">border_fill_color&nbsp;=&nbsp;'#ffffff',</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">center&nbsp;=&nbsp;[Grid(id='p1292', ...), Grid(id='p1297', ...)],</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">context_menu&nbsp;=&nbsp;None,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">css_classes&nbsp;=&nbsp;[],</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">css_variables&nbsp;=&nbsp;{},</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">disabled&nbsp;=&nbsp;False,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">elements&nbsp;=&nbsp;[],</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">extra_x_ranges&nbsp;=&nbsp;{},</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">extra_x_scales&nbsp;=&nbsp;{},</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">extra_y_ranges&nbsp;=&nbsp;{},</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">extra_y_scales&nbsp;=&nbsp;{},</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">flow_mode&nbsp;=&nbsp;'block',</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">frame_align&nbsp;=&nbsp;True,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">frame_height&nbsp;=&nbsp;None,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">frame_width&nbsp;=&nbsp;None,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">height&nbsp;=&nbsp;220,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">height_policy&nbsp;=&nbsp;'auto',</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">hidpi&nbsp;=&nbsp;True,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">hold_render&nbsp;=&nbsp;False,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">js_event_callbacks&nbsp;=&nbsp;{},</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">js_property_callbacks&nbsp;=&nbsp;{},</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">left&nbsp;=&nbsp;[LinearAxis(id='p1293', ...)],</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">lod_factor&nbsp;=&nbsp;10,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">lod_interval&nbsp;=&nbsp;300,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">lod_threshold&nbsp;=&nbsp;2000,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">lod_timeout&nbsp;=&nbsp;500,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">margin&nbsp;=&nbsp;None,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">match_aspect&nbsp;=&nbsp;False,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">max_height&nbsp;=&nbsp;None,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">max_width&nbsp;=&nbsp;None,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border&nbsp;=&nbsp;5,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border_bottom&nbsp;=&nbsp;None,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border_left&nbsp;=&nbsp;None,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border_right&nbsp;=&nbsp;None,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border_top&nbsp;=&nbsp;None,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_height&nbsp;=&nbsp;None,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_width&nbsp;=&nbsp;None,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">name&nbsp;=&nbsp;None,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_alpha&nbsp;=&nbsp;1.0,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_cap&nbsp;=&nbsp;'butt',</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_color&nbsp;=&nbsp;'#e5e5e5',</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_dash&nbsp;=&nbsp;[],</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_dash_offset&nbsp;=&nbsp;0,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_join&nbsp;=&nbsp;'bevel',</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_width&nbsp;=&nbsp;1,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">output_backend&nbsp;=&nbsp;'canvas',</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">renderers&nbsp;=&nbsp;[GlyphRenderer(id='p1315', ...), GlyphRenderer(id='p1324', ...)],</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">reset_policy&nbsp;=&nbsp;'standard',</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">resizable&nbsp;=&nbsp;False,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">right&nbsp;=&nbsp;[],</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">sizing_mode&nbsp;=&nbsp;None,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">styles&nbsp;=&nbsp;{},</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">stylesheets&nbsp;=&nbsp;[],</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">subscribed_events&nbsp;=&nbsp;PropertyValueSet(),</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">syncable&nbsp;=&nbsp;True,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">tags&nbsp;=&nbsp;[],</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">title&nbsp;=&nbsp;Title(id='p1265', ...),</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">title_location&nbsp;=&nbsp;'above',</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">toolbar&nbsp;=&nbsp;Toolbar(id='p1271', ...),</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">toolbar_inner&nbsp;=&nbsp;False,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">toolbar_location&nbsp;=&nbsp;'right',</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">toolbar_sticky&nbsp;=&nbsp;True,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">visible&nbsp;=&nbsp;True,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">width&nbsp;=&nbsp;400,</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">width_policy&nbsp;=&nbsp;'auto',</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">x_range&nbsp;=&nbsp;Range1d(id='p1272', ...),</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">x_scale&nbsp;=&nbsp;LinearScale(id='p1274', ...),</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">y_range&nbsp;=&nbsp;Range1d(id='p1273', ...),</div></div><div class=\"p1327\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">y_scale&nbsp;=&nbsp;LinearScale(id='p1275', ...))</div></div></div>\n",
                             "<script>\n",
                             "(function() {\n",
-                            "  var expanded = false;\n",
-                            "  var ellipsis = document.getElementById(\"6019\");\n",
+                            "  let expanded = false;\n",
+                            "  const ellipsis = document.getElementById(\"p1328\");\n",
                             "  ellipsis.addEventListener(\"click\", function() {\n",
-                            "    var rows = document.getElementsByClassName(\"6018\");\n",
-                            "    for (var i = 0; i < rows.length; i++) {\n",
-                            "      var el = rows[i];\n",
+                            "    const rows = document.getElementsByClassName(\"p1327\");\n",
+                            "    for (let i = 0; i < rows.length; i++) {\n",
+                            "      const el = rows[i];\n",
                             "      el.style.display = expanded ? \"none\" : \"table-row\";\n",
                             "    }\n",
                             "    ellipsis.innerHTML = expanded ? \"&hellip;)\" : \"&lsaquo;&lsaquo;&lsaquo;\";\n",
                             "    expanded = !expanded;\n",
                             "  });\n",
                             "})();\n",
                             "</script>\n"
                         ],
                         "text/plain": [
-                            "Figure(id='5490', ...)"
+                            "figure(id='p1262', ...)"
                         ]
                     },
-                    "execution_count": 35,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Go back to Evenly Spaced timeseries\n",
                 "evenly_ts = ts.sample(freq='1Min')\n",
                 "evenly_ts.iplot(**kwargs_plot, show=True)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 36,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "\n",
-                            "\n",
-                            "\n",
-                            "\n",
-                            "\n",
-                            "\n",
-                            "  <div class=\"bk-root\" id=\"14e6b9a6-578b-42e2-a91f-62603931ce15\" data-root-id=\"6021\"></div>\n"
+                            "  <div id=\"e4aa8380-fb9f-43e4-a289-25b61a70ad56\" data-root-id=\"p1329\" style=\"display: contents;\"></div>\n"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/javascript": [
                             "(function(root) {\n",
                             "  function embed_document(root) {\n",
-                            "    \n",
-                            "  var docs_json = {\"2da2f1b0-39d2-49ca-a6cb-62a2ee2bf7f9\":{\"roots\":{\"references\":[{\"attributes\":{\"below\":[{\"id\":\"6032\",\"type\":\"DatetimeAxis\"}],\"center\":[{\"id\":\"6036\",\"type\":\"Grid\"},{\"id\":\"6041\",\"type\":\"Grid\"}],\"left\":[{\"id\":\"6037\",\"type\":\"LinearAxis\"}],\"plot_height\":220,\"plot_width\":400,\"renderers\":[{\"id\":\"6058\",\"type\":\"GlyphRenderer\"},{\"id\":\"6063\",\"type\":\"GlyphRenderer\"}],\"title\":{\"id\":\"6022\",\"type\":\"Title\"},\"toolbar\":{\"id\":\"6048\",\"type\":\"Toolbar\"},\"x_range\":{\"id\":\"6024\",\"type\":\"Range1d\"},\"x_scale\":{\"id\":\"6028\",\"type\":\"LinearScale\"},\"y_range\":{\"id\":\"6026\",\"type\":\"Range1d\"},\"y_scale\":{\"id\":\"6030\",\"type\":\"LinearScale\"}},\"id\":\"6021\",\"subtype\":\"Figure\",\"type\":\"Plot\"},{\"attributes\":{\"callback\":null,\"end\":1546302000000.0,\"start\":1546300620000.0},\"id\":\"6024\",\"type\":\"Range1d\"},{\"attributes\":{\"days\":[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31]},\"id\":\"6425\",\"type\":\"DaysTicker\"},{\"attributes\":{\"bottom_units\":\"screen\",\"fill_alpha\":{\"value\":0.5},\"fill_color\":{\"value\":\"lightgrey\"},\"left_units\":\"screen\",\"level\":\"overlay\",\"line_alpha\":{\"value\":1.0},\"line_color\":{\"value\":\"black\"},\"line_dash\":[4,4],\"line_width\":{\"value\":2},\"render_mode\":\"css\",\"right_units\":\"screen\",\"top_units\":\"screen\"},\"id\":\"6438\",\"type\":\"BoxAnnotation\"},{\"attributes\":{\"text\":\"value\"},\"id\":\"6022\",\"type\":\"Title\"},{\"attributes\":{\"days\":[1,4,7,10,13,16,19,22,25,28]},\"id\":\"6426\",\"type\":\"DaysTicker\"},{\"attributes\":{\"active_drag\":\"auto\",\"active_inspect\":\"auto\",\"active_multi\":null,\"active_scroll\":\"auto\",\"active_tap\":\"auto\",\"tools\":[{\"id\":\"6042\",\"type\":\"PanTool\"},{\"id\":\"6043\",\"type\":\"WheelZoomTool\"},{\"id\":\"6044\",\"type\":\"BoxZoomTool\"},{\"id\":\"6045\",\"type\":\"SaveTool\"},{\"id\":\"6046\",\"type\":\"ResetTool\"},{\"id\":\"6047\",\"type\":\"HelpTool\"}]},\"id\":\"6048\",\"type\":\"Toolbar\"},{\"attributes\":{},\"id\":\"6042\",\"type\":\"PanTool\"},{\"attributes\":{\"days\":[1,8,15,22]},\"id\":\"6427\",\"type\":\"DaysTicker\"},{\"attributes\":{},\"id\":\"6420\",\"type\":\"BasicTickFormatter\"},{\"attributes\":{\"overlay\":{\"id\":\"6438\",\"type\":\"BoxAnnotation\"}},\"id\":\"6044\",\"type\":\"BoxZoomTool\"},{\"attributes\":{},\"id\":\"6045\",\"type\":\"SaveTool\"},{\"attributes\":{\"base\":60,\"mantissas\":[1,2,5,10,15,20,30],\"max_interval\":1800000.0,\"min_interval\":1000.0,\"num_minor_ticks\":0},\"id\":\"6423\",\"type\":\"AdaptiveTicker\"},{\"attributes\":{\"days\":[1,15]},\"id\":\"6428\",\"type\":\"DaysTicker\"},{\"attributes\":{},\"id\":\"6043\",\"type\":\"WheelZoomTool\"},{\"attributes\":{\"base\":24,\"mantissas\":[1,2,4,6,8,12],\"max_interval\":43200000.0,\"min_interval\":3600000.0,\"num_minor_ticks\":0},\"id\":\"6424\",\"type\":\"AdaptiveTicker\"},{\"attributes\":{\"months\":[0,1,2,3,4,5,6,7,8,9,10,11]},\"id\":\"6429\",\"type\":\"MonthsTicker\"},{\"attributes\":{\"callback\":null,\"data\":{\"x\":[1546300800000.0,1546301400000.0,1546301700000.0],\"y\":[10,20,10]},\"selected\":{\"id\":\"6435\",\"type\":\"Selection\"},\"selection_policy\":{\"id\":\"6434\",\"type\":\"UnionRenderers\"}},\"id\":\"6055\",\"type\":\"ColumnDataSource\"},{\"attributes\":{\"months\":[0,2,4,6,8,10]},\"id\":\"6430\",\"type\":\"MonthsTicker\"},{\"attributes\":{\"months\":[0,4,8]},\"id\":\"6431\",\"type\":\"MonthsTicker\"},{\"attributes\":{},\"id\":\"6047\",\"type\":\"HelpTool\"},{\"attributes\":{\"dimension\":1,\"ticker\":{\"id\":\"6038\",\"type\":\"BasicTicker\"}},\"id\":\"6041\",\"type\":\"Grid\"},{\"attributes\":{},\"id\":\"6046\",\"type\":\"ResetTool\"},{\"attributes\":{\"months\":[0,6]},\"id\":\"6432\",\"type\":\"MonthsTicker\"},{\"attributes\":{\"line_color\":{\"value\":\"#1f77b4\"},\"line_dash\":[4,4],\"line_width\":{\"value\":2},\"mode\":\"after\",\"x\":{\"field\":\"x\"},\"y\":{\"field\":\"y\"}},\"id\":\"6056\",\"type\":\"Step\"},{\"attributes\":{\"line_alpha\":{\"value\":0.1},\"line_color\":{\"value\":\"#1f77b4\"},\"line_dash\":[4,4],\"line_width\":{\"value\":2},\"mode\":\"after\",\"x\":{\"field\":\"x\"},\"y\":{\"field\":\"y\"}},\"id\":\"6057\",\"type\":\"Step\"},{\"attributes\":{\"data_source\":{\"id\":\"6055\",\"type\":\"ColumnDataSource\"},\"glyph\":{\"id\":\"6056\",\"type\":\"Step\"},\"hover_glyph\":null,\"muted_glyph\":null,\"nonselection_glyph\":{\"id\":\"6057\",\"type\":\"Step\"},\"selection_glyph\":null,\"view\":{\"id\":\"6059\",\"type\":\"CDSView\"}},\"id\":\"6058\",\"type\":\"GlyphRenderer\"},{\"attributes\":{},\"id\":\"6433\",\"type\":\"YearsTicker\"},{\"attributes\":{},\"id\":\"6038\",\"type\":\"BasicTicker\"},{\"attributes\":{},\"id\":\"6434\",\"type\":\"UnionRenderers\"},{\"attributes\":{\"formatter\":{\"id\":\"6420\",\"type\":\"BasicTickFormatter\"},\"ticker\":{\"id\":\"6038\",\"type\":\"BasicTicker\"}},\"id\":\"6037\",\"type\":\"LinearAxis\"},{\"attributes\":{\"source\":{\"id\":\"6055\",\"type\":\"ColumnDataSource\"}},\"id\":\"6059\",\"type\":\"CDSView\"},{\"attributes\":{},\"id\":\"6435\",\"type\":\"Selection\"},{\"attributes\":{\"num_minor_ticks\":5,\"tickers\":[{\"id\":\"6422\",\"type\":\"AdaptiveTicker\"},{\"id\":\"6423\",\"type\":\"AdaptiveTicker\"},{\"id\":\"6424\",\"type\":\"AdaptiveTicker\"},{\"id\":\"6425\",\"type\":\"DaysTicker\"},{\"id\":\"6426\",\"type\":\"DaysTicker\"},{\"id\":\"6427\",\"type\":\"DaysTicker\"},{\"id\":\"6428\",\"type\":\"DaysTicker\"},{\"id\":\"6429\",\"type\":\"MonthsTicker\"},{\"id\":\"6430\",\"type\":\"MonthsTicker\"},{\"id\":\"6431\",\"type\":\"MonthsTicker\"},{\"id\":\"6432\",\"type\":\"MonthsTicker\"},{\"id\":\"6433\",\"type\":\"YearsTicker\"}]},\"id\":\"6033\",\"type\":\"DatetimeTicker\"},{\"attributes\":{\"source\":{\"id\":\"6060\",\"type\":\"ColumnDataSource\"}},\"id\":\"6064\",\"type\":\"CDSView\"},{\"attributes\":{},\"id\":\"6436\",\"type\":\"UnionRenderers\"},{\"attributes\":{\"ticker\":{\"id\":\"6033\",\"type\":\"DatetimeTicker\"}},\"id\":\"6036\",\"type\":\"Grid\"},{\"attributes\":{\"fill_color\":{\"value\":\"red\"},\"line_color\":{\"value\":\"#1f77b4\"},\"size\":{\"units\":\"screen\",\"value\":6},\"x\":{\"field\":\"x\"},\"y\":{\"field\":\"y\"}},\"id\":\"6061\",\"type\":\"Circle\"},{\"attributes\":{},\"id\":\"6437\",\"type\":\"Selection\"},{\"attributes\":{},\"id\":\"6418\",\"type\":\"DatetimeTickFormatter\"},{\"attributes\":{\"callback\":null,\"end\":37,\"start\":-5},\"id\":\"6026\",\"type\":\"Range1d\"},{\"attributes\":{\"axis_label\":\"timestamp\",\"formatter\":{\"id\":\"6418\",\"type\":\"DatetimeTickFormatter\"},\"ticker\":{\"id\":\"6033\",\"type\":\"DatetimeTicker\"}},\"id\":\"6032\",\"type\":\"DatetimeAxis\"},{\"attributes\":{\"fill_alpha\":{\"value\":0.1},\"fill_color\":{\"value\":\"#1f77b4\"},\"line_alpha\":{\"value\":0.1},\"line_color\":{\"value\":\"#1f77b4\"},\"size\":{\"units\":\"screen\",\"value\":6},\"x\":{\"field\":\"x\"},\"y\":{\"field\":\"y\"}},\"id\":\"6062\",\"type\":\"Circle\"},{\"attributes\":{},\"id\":\"6030\",\"type\":\"LinearScale\"},{\"attributes\":{\"callback\":null,\"data\":{\"x\":[1546300800000.0,1546301400000.0,1546301700000.0],\"y\":[10,20,10]},\"selected\":{\"id\":\"6437\",\"type\":\"Selection\"},\"selection_policy\":{\"id\":\"6436\",\"type\":\"UnionRenderers\"}},\"id\":\"6060\",\"type\":\"ColumnDataSource\"},{\"attributes\":{},\"id\":\"6028\",\"type\":\"LinearScale\"},{\"attributes\":{\"data_source\":{\"id\":\"6060\",\"type\":\"ColumnDataSource\"},\"glyph\":{\"id\":\"6061\",\"type\":\"Circle\"},\"hover_glyph\":null,\"muted_glyph\":null,\"nonselection_glyph\":{\"id\":\"6062\",\"type\":\"Circle\"},\"selection_glyph\":null,\"view\":{\"id\":\"6064\",\"type\":\"CDSView\"}},\"id\":\"6063\",\"type\":\"GlyphRenderer\"},{\"attributes\":{\"mantissas\":[1,2,5],\"max_interval\":500.0,\"num_minor_ticks\":0},\"id\":\"6422\",\"type\":\"AdaptiveTicker\"}],\"root_ids\":[\"6021\"]},\"title\":\"Bokeh Application\",\"version\":\"1.3.1\"}};\n",
-                            "  var render_items = [{\"docid\":\"2da2f1b0-39d2-49ca-a6cb-62a2ee2bf7f9\",\"roots\":{\"6021\":\"14e6b9a6-578b-42e2-a91f-62603931ce15\"}}];\n",
-                            "  root.Bokeh.embed.embed_items_notebook(docs_json, render_items);\n",
-                            "\n",
+                            "  const docs_json = {\"f4c3551f-c6cb-4e6d-ac4a-1b7a9a48bead\":{\"version\":\"3.4.1\",\"title\":\"Bokeh Application\",\"roots\":[{\"type\":\"object\",\"name\":\"Figure\",\"id\":\"p1329\",\"attributes\":{\"width\":400,\"height\":220,\"x_range\":{\"type\":\"object\",\"name\":\"Range1d\",\"id\":\"p1339\",\"attributes\":{\"start\":1546300620000.0,\"end\":1546302000000.0}},\"y_range\":{\"type\":\"object\",\"name\":\"Range1d\",\"id\":\"p1340\",\"attributes\":{\"start\":-5,\"end\":37}},\"x_scale\":{\"type\":\"object\",\"name\":\"LinearScale\",\"id\":\"p1341\"},\"y_scale\":{\"type\":\"object\",\"name\":\"LinearScale\",\"id\":\"p1342\"},\"title\":{\"type\":\"object\",\"name\":\"Title\",\"id\":\"p1332\",\"attributes\":{\"text\":\"value\"}},\"renderers\":[{\"type\":\"object\",\"name\":\"GlyphRenderer\",\"id\":\"p1382\",\"attributes\":{\"data_source\":{\"type\":\"object\",\"name\":\"ColumnDataSource\",\"id\":\"p1376\",\"attributes\":{\"selected\":{\"type\":\"object\",\"name\":\"Selection\",\"id\":\"p1377\",\"attributes\":{\"indices\":[],\"line_indices\":[]}},\"selection_policy\":{\"type\":\"object\",\"name\":\"UnionRenderers\",\"id\":\"p1378\"},\"data\":{\"type\":\"map\",\"entries\":[[\"x\",[1546300800000.0,1546301400000.0,1546301700000.0]],[\"y\",[10,20,10]]]}}},\"view\":{\"type\":\"object\",\"name\":\"CDSView\",\"id\":\"p1383\",\"attributes\":{\"filter\":{\"type\":\"object\",\"name\":\"AllIndices\",\"id\":\"p1384\"}}},\"glyph\":{\"type\":\"object\",\"name\":\"Step\",\"id\":\"p1379\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"line_color\":\"#1f77b4\",\"line_width\":2,\"line_dash\":[4,4],\"mode\":\"after\"}},\"nonselection_glyph\":{\"type\":\"object\",\"name\":\"Step\",\"id\":\"p1380\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"line_color\":\"#1f77b4\",\"line_alpha\":0.1,\"line_width\":2,\"line_dash\":[4,4],\"mode\":\"after\"}},\"muted_glyph\":{\"type\":\"object\",\"name\":\"Step\",\"id\":\"p1381\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"line_color\":\"#1f77b4\",\"line_alpha\":0.2,\"line_width\":2,\"line_dash\":[4,4],\"mode\":\"after\"}}}},{\"type\":\"object\",\"name\":\"GlyphRenderer\",\"id\":\"p1391\",\"attributes\":{\"data_source\":{\"type\":\"object\",\"name\":\"ColumnDataSource\",\"id\":\"p1385\",\"attributes\":{\"selected\":{\"type\":\"object\",\"name\":\"Selection\",\"id\":\"p1386\",\"attributes\":{\"indices\":[],\"line_indices\":[]}},\"selection_policy\":{\"type\":\"object\",\"name\":\"UnionRenderers\",\"id\":\"p1387\"},\"data\":{\"type\":\"map\",\"entries\":[[\"x\",[1546300800000.0,1546301400000.0,1546301700000.0]],[\"y\",[10,20,10]]]}}},\"view\":{\"type\":\"object\",\"name\":\"CDSView\",\"id\":\"p1392\",\"attributes\":{\"filter\":{\"type\":\"object\",\"name\":\"AllIndices\",\"id\":\"p1393\"}}},\"glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1388\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"size\":{\"type\":\"value\",\"value\":6},\"line_color\":{\"type\":\"value\",\"value\":\"#1f77b4\"},\"fill_color\":{\"type\":\"value\",\"value\":\"red\"}}},\"nonselection_glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1389\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"size\":{\"type\":\"value\",\"value\":6},\"line_color\":{\"type\":\"value\",\"value\":\"#1f77b4\"},\"line_alpha\":{\"type\":\"value\",\"value\":0.1},\"fill_color\":{\"type\":\"value\",\"value\":\"red\"},\"fill_alpha\":{\"type\":\"value\",\"value\":0.1},\"hatch_alpha\":{\"type\":\"value\",\"value\":0.1}}},\"muted_glyph\":{\"type\":\"object\",\"name\":\"Scatter\",\"id\":\"p1390\",\"attributes\":{\"x\":{\"type\":\"field\",\"field\":\"x\"},\"y\":{\"type\":\"field\",\"field\":\"y\"},\"size\":{\"type\":\"value\",\"value\":6},\"line_color\":{\"type\":\"value\",\"value\":\"#1f77b4\"},\"line_alpha\":{\"type\":\"value\",\"value\":0.2},\"fill_color\":{\"type\":\"value\",\"value\":\"red\"},\"fill_alpha\":{\"type\":\"value\",\"value\":0.2},\"hatch_alpha\":{\"type\":\"value\",\"value\":0.2}}}}}],\"toolbar\":{\"type\":\"object\",\"name\":\"Toolbar\",\"id\":\"p1338\",\"attributes\":{\"tools\":[{\"type\":\"object\",\"name\":\"PanTool\",\"id\":\"p1365\"},{\"type\":\"object\",\"name\":\"WheelZoomTool\",\"id\":\"p1366\",\"attributes\":{\"renderers\":\"auto\"}},{\"type\":\"object\",\"name\":\"BoxZoomTool\",\"id\":\"p1367\",\"attributes\":{\"overlay\":{\"type\":\"object\",\"name\":\"BoxAnnotation\",\"id\":\"p1368\",\"attributes\":{\"syncable\":false,\"level\":\"overlay\",\"visible\":false,\"left\":{\"type\":\"number\",\"value\":\"nan\"},\"right\":{\"type\":\"number\",\"value\":\"nan\"},\"top\":{\"type\":\"number\",\"value\":\"nan\"},\"bottom\":{\"type\":\"number\",\"value\":\"nan\"},\"left_units\":\"canvas\",\"right_units\":\"canvas\",\"top_units\":\"canvas\",\"bottom_units\":\"canvas\",\"line_color\":\"black\",\"line_alpha\":1.0,\"line_width\":2,\"line_dash\":[4,4],\"fill_color\":\"lightgrey\",\"fill_alpha\":0.5}}}},{\"type\":\"object\",\"name\":\"SaveTool\",\"id\":\"p1373\"},{\"type\":\"object\",\"name\":\"ResetTool\",\"id\":\"p1374\"},{\"type\":\"object\",\"name\":\"HelpTool\",\"id\":\"p1375\"}]}},\"left\":[{\"type\":\"object\",\"name\":\"LinearAxis\",\"id\":\"p1360\",\"attributes\":{\"ticker\":{\"type\":\"object\",\"name\":\"BasicTicker\",\"id\":\"p1361\",\"attributes\":{\"mantissas\":[1,2,5]}},\"formatter\":{\"type\":\"object\",\"name\":\"BasicTickFormatter\",\"id\":\"p1362\"},\"major_label_policy\":{\"type\":\"object\",\"name\":\"AllLabels\",\"id\":\"p1363\"}}}],\"below\":[{\"type\":\"object\",\"name\":\"DatetimeAxis\",\"id\":\"p1343\",\"attributes\":{\"ticker\":{\"type\":\"object\",\"name\":\"DatetimeTicker\",\"id\":\"p1344\",\"attributes\":{\"num_minor_ticks\":5,\"tickers\":[{\"type\":\"object\",\"name\":\"AdaptiveTicker\",\"id\":\"p1345\",\"attributes\":{\"num_minor_ticks\":0,\"mantissas\":[1,2,5],\"max_interval\":500.0}},{\"type\":\"object\",\"name\":\"AdaptiveTicker\",\"id\":\"p1346\",\"attributes\":{\"num_minor_ticks\":0,\"base\":60,\"mantissas\":[1,2,5,10,15,20,30],\"min_interval\":1000.0,\"max_interval\":1800000.0}},{\"type\":\"object\",\"name\":\"AdaptiveTicker\",\"id\":\"p1347\",\"attributes\":{\"num_minor_ticks\":0,\"base\":24,\"mantissas\":[1,2,4,6,8,12],\"min_interval\":3600000.0,\"max_interval\":43200000.0}},{\"type\":\"object\",\"name\":\"DaysTicker\",\"id\":\"p1348\",\"attributes\":{\"days\":[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31]}},{\"type\":\"object\",\"name\":\"DaysTicker\",\"id\":\"p1349\",\"attributes\":{\"days\":[1,4,7,10,13,16,19,22,25,28]}},{\"type\":\"object\",\"name\":\"DaysTicker\",\"id\":\"p1350\",\"attributes\":{\"days\":[1,8,15,22]}},{\"type\":\"object\",\"name\":\"DaysTicker\",\"id\":\"p1351\",\"attributes\":{\"days\":[1,15]}},{\"type\":\"object\",\"name\":\"MonthsTicker\",\"id\":\"p1352\",\"attributes\":{\"months\":[0,1,2,3,4,5,6,7,8,9,10,11]}},{\"type\":\"object\",\"name\":\"MonthsTicker\",\"id\":\"p1353\",\"attributes\":{\"months\":[0,2,4,6,8,10]}},{\"type\":\"object\",\"name\":\"MonthsTicker\",\"id\":\"p1354\",\"attributes\":{\"months\":[0,4,8]}},{\"type\":\"object\",\"name\":\"MonthsTicker\",\"id\":\"p1355\",\"attributes\":{\"months\":[0,6]}},{\"type\":\"object\",\"name\":\"YearsTicker\",\"id\":\"p1356\"}]}},\"formatter\":{\"type\":\"object\",\"name\":\"DatetimeTickFormatter\",\"id\":\"p1357\"},\"axis_label\":\"timestamp\",\"major_label_policy\":{\"type\":\"object\",\"name\":\"AllLabels\",\"id\":\"p1358\"}}}],\"center\":[{\"type\":\"object\",\"name\":\"Grid\",\"id\":\"p1359\",\"attributes\":{\"axis\":{\"id\":\"p1343\"}}},{\"type\":\"object\",\"name\":\"Grid\",\"id\":\"p1364\",\"attributes\":{\"dimension\":1,\"axis\":{\"id\":\"p1360\"}}}]}}]}};\n",
+                            "  const render_items = [{\"docid\":\"f4c3551f-c6cb-4e6d-ac4a-1b7a9a48bead\",\"roots\":{\"p1329\":\"e4aa8380-fb9f-43e4-a289-25b61a70ad56\"},\"root_ids\":[\"p1329\"]}];\n",
+                            "  void root.Bokeh.embed.embed_items_notebook(docs_json, render_items);\n",
                             "  }\n",
                             "  if (root.Bokeh !== undefined) {\n",
                             "    embed_document(root);\n",
                             "  } else {\n",
-                            "    var attempts = 0;\n",
-                            "    var timer = setInterval(function(root) {\n",
+                            "    let attempts = 0;\n",
+                            "    const timer = setInterval(function(root) {\n",
                             "      if (root.Bokeh !== undefined) {\n",
-                            "        embed_document(root);\n",
-                            "        clearInterval(timer);\n",
-                            "      }\n",
-                            "      attempts++;\n",
-                            "      if (attempts > 100) {\n",
-                            "        console.log(\"Bokeh: ERROR: Unable to run BokehJS code because BokehJS library is missing\");\n",
                             "        clearInterval(timer);\n",
+                            "        embed_document(root);\n",
+                            "      } else {\n",
+                            "        attempts++;\n",
+                            "        if (attempts > 100) {\n",
+                            "          clearInterval(timer);\n",
+                            "          console.log(\"Bokeh: ERROR: Unable to run BokehJS code because BokehJS library is missing\");\n",
+                            "        }\n",
                             "      }\n",
                             "    }, 10, root)\n",
                             "  }\n",
                             "})(window);"
                         ],
                         "application/vnd.bokehjs_exec.v0+json": ""
                     },
                     "metadata": {
                         "application/vnd.bokehjs_exec.v0+json": {
-                            "id": "6021"
+                            "id": "p1329"
                         }
                     },
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"display: table;\"><div style=\"display: table-row;\"><div style=\"display: table-cell;\"><b title=\"bokeh.plotting.figure.Figure\">Figure</b>(</div><div style=\"display: table-cell;\">id&nbsp;=&nbsp;'6021', <span id=\"6572\" style=\"cursor: pointer;\">&hellip;)</span></div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">above&nbsp;=&nbsp;[],</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">align&nbsp;=&nbsp;'start',</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">aspect_ratio&nbsp;=&nbsp;None,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">aspect_scale&nbsp;=&nbsp;1,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">background&nbsp;=&nbsp;None,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">background_fill_alpha&nbsp;=&nbsp;{'value': 1.0},</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">background_fill_color&nbsp;=&nbsp;{'value': '#ffffff'},</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">below&nbsp;=&nbsp;[DatetimeAxis(id='6032', ...)],</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">border_fill_alpha&nbsp;=&nbsp;{'value': 1.0},</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">border_fill_color&nbsp;=&nbsp;{'value': '#ffffff'},</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">center&nbsp;=&nbsp;[Grid(id='6036', ...), Grid(id='6041', ...)],</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">css_classes&nbsp;=&nbsp;[],</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">disabled&nbsp;=&nbsp;False,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">extra_x_ranges&nbsp;=&nbsp;{},</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">extra_y_ranges&nbsp;=&nbsp;{},</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">frame_height&nbsp;=&nbsp;None,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">frame_width&nbsp;=&nbsp;None,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">height&nbsp;=&nbsp;None,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">height_policy&nbsp;=&nbsp;'auto',</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">hidpi&nbsp;=&nbsp;True,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">js_event_callbacks&nbsp;=&nbsp;{},</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">js_property_callbacks&nbsp;=&nbsp;{},</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">left&nbsp;=&nbsp;[LinearAxis(id='6037', ...)],</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">lod_factor&nbsp;=&nbsp;10,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">lod_interval&nbsp;=&nbsp;300,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">lod_threshold&nbsp;=&nbsp;2000,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">lod_timeout&nbsp;=&nbsp;500,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">margin&nbsp;=&nbsp;(0, 0, 0, 0),</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">match_aspect&nbsp;=&nbsp;False,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">max_height&nbsp;=&nbsp;None,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">max_width&nbsp;=&nbsp;None,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border&nbsp;=&nbsp;5,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border_bottom&nbsp;=&nbsp;None,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border_left&nbsp;=&nbsp;None,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border_right&nbsp;=&nbsp;None,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border_top&nbsp;=&nbsp;None,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_height&nbsp;=&nbsp;None,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_width&nbsp;=&nbsp;None,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">name&nbsp;=&nbsp;None,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_alpha&nbsp;=&nbsp;{'value': 1.0},</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_cap&nbsp;=&nbsp;'butt',</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_color&nbsp;=&nbsp;{'value': '#e5e5e5'},</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_dash&nbsp;=&nbsp;[],</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_dash_offset&nbsp;=&nbsp;0,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_join&nbsp;=&nbsp;'bevel',</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_width&nbsp;=&nbsp;{'value': 1},</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">output_backend&nbsp;=&nbsp;'canvas',</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">plot_height&nbsp;=&nbsp;220,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">plot_width&nbsp;=&nbsp;400,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">renderers&nbsp;=&nbsp;[GlyphRenderer(id='6058', ...), GlyphRenderer(id='6063', ...)],</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">reset_policy&nbsp;=&nbsp;'standard',</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">right&nbsp;=&nbsp;[],</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">sizing_mode&nbsp;=&nbsp;None,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">subscribed_events&nbsp;=&nbsp;[],</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">tags&nbsp;=&nbsp;[],</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">title&nbsp;=&nbsp;Title(id='6022', ...),</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">title_location&nbsp;=&nbsp;'above',</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">toolbar&nbsp;=&nbsp;Toolbar(id='6048', ...),</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">toolbar_location&nbsp;=&nbsp;'right',</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">toolbar_sticky&nbsp;=&nbsp;True,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">visible&nbsp;=&nbsp;True,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">width&nbsp;=&nbsp;None,</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">width_policy&nbsp;=&nbsp;'auto',</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">x_range&nbsp;=&nbsp;Range1d(id='6024', ...),</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">x_scale&nbsp;=&nbsp;LinearScale(id='6028', ...),</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">y_range&nbsp;=&nbsp;Range1d(id='6026', ...),</div></div><div class=\"6571\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">y_scale&nbsp;=&nbsp;LinearScale(id='6030', ...))</div></div></div>\n",
+                            "<div style=\"display: table;\"><div style=\"display: table-row;\"><div style=\"display: table-cell;\"><b title=\"bokeh.plotting._figure.figure\">figure</b>(</div><div style=\"display: table-cell;\">id&nbsp;=&nbsp;'p1329', <span id=\"p1395\" style=\"cursor: pointer;\">&hellip;)</span></div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">above&nbsp;=&nbsp;[],</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">align&nbsp;=&nbsp;'auto',</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">aspect_ratio&nbsp;=&nbsp;None,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">aspect_scale&nbsp;=&nbsp;1,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">attribution&nbsp;=&nbsp;[],</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">background_fill_alpha&nbsp;=&nbsp;1.0,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">background_fill_color&nbsp;=&nbsp;'#ffffff',</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">below&nbsp;=&nbsp;[DatetimeAxis(id='p1343', ...)],</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">border_fill_alpha&nbsp;=&nbsp;1.0,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">border_fill_color&nbsp;=&nbsp;'#ffffff',</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">center&nbsp;=&nbsp;[Grid(id='p1359', ...), Grid(id='p1364', ...)],</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">context_menu&nbsp;=&nbsp;None,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">css_classes&nbsp;=&nbsp;[],</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">css_variables&nbsp;=&nbsp;{},</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">disabled&nbsp;=&nbsp;False,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">elements&nbsp;=&nbsp;[],</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">extra_x_ranges&nbsp;=&nbsp;{},</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">extra_x_scales&nbsp;=&nbsp;{},</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">extra_y_ranges&nbsp;=&nbsp;{},</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">extra_y_scales&nbsp;=&nbsp;{},</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">flow_mode&nbsp;=&nbsp;'block',</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">frame_align&nbsp;=&nbsp;True,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">frame_height&nbsp;=&nbsp;None,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">frame_width&nbsp;=&nbsp;None,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">height&nbsp;=&nbsp;220,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">height_policy&nbsp;=&nbsp;'auto',</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">hidpi&nbsp;=&nbsp;True,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">hold_render&nbsp;=&nbsp;False,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">js_event_callbacks&nbsp;=&nbsp;{},</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">js_property_callbacks&nbsp;=&nbsp;{},</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">left&nbsp;=&nbsp;[LinearAxis(id='p1360', ...)],</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">lod_factor&nbsp;=&nbsp;10,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">lod_interval&nbsp;=&nbsp;300,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">lod_threshold&nbsp;=&nbsp;2000,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">lod_timeout&nbsp;=&nbsp;500,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">margin&nbsp;=&nbsp;None,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">match_aspect&nbsp;=&nbsp;False,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">max_height&nbsp;=&nbsp;None,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">max_width&nbsp;=&nbsp;None,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border&nbsp;=&nbsp;5,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border_bottom&nbsp;=&nbsp;None,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border_left&nbsp;=&nbsp;None,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border_right&nbsp;=&nbsp;None,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_border_top&nbsp;=&nbsp;None,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_height&nbsp;=&nbsp;None,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">min_width&nbsp;=&nbsp;None,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">name&nbsp;=&nbsp;None,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_alpha&nbsp;=&nbsp;1.0,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_cap&nbsp;=&nbsp;'butt',</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_color&nbsp;=&nbsp;'#e5e5e5',</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_dash&nbsp;=&nbsp;[],</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_dash_offset&nbsp;=&nbsp;0,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_join&nbsp;=&nbsp;'bevel',</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">outline_line_width&nbsp;=&nbsp;1,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">output_backend&nbsp;=&nbsp;'canvas',</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">renderers&nbsp;=&nbsp;[GlyphRenderer(id='p1382', ...), GlyphRenderer(id='p1391', ...)],</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">reset_policy&nbsp;=&nbsp;'standard',</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">resizable&nbsp;=&nbsp;False,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">right&nbsp;=&nbsp;[],</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">sizing_mode&nbsp;=&nbsp;None,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">styles&nbsp;=&nbsp;{},</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">stylesheets&nbsp;=&nbsp;[],</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">subscribed_events&nbsp;=&nbsp;PropertyValueSet(),</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">syncable&nbsp;=&nbsp;True,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">tags&nbsp;=&nbsp;[],</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">title&nbsp;=&nbsp;Title(id='p1332', ...),</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">title_location&nbsp;=&nbsp;'above',</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">toolbar&nbsp;=&nbsp;Toolbar(id='p1338', ...),</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">toolbar_inner&nbsp;=&nbsp;False,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">toolbar_location&nbsp;=&nbsp;'right',</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">toolbar_sticky&nbsp;=&nbsp;True,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">visible&nbsp;=&nbsp;True,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">width&nbsp;=&nbsp;400,</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">width_policy&nbsp;=&nbsp;'auto',</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">x_range&nbsp;=&nbsp;Range1d(id='p1339', ...),</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">x_scale&nbsp;=&nbsp;LinearScale(id='p1341', ...),</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">y_range&nbsp;=&nbsp;Range1d(id='p1340', ...),</div></div><div class=\"p1394\" style=\"display: none;\"><div style=\"display: table-cell;\"></div><div style=\"display: table-cell;\">y_scale&nbsp;=&nbsp;LinearScale(id='p1342', ...))</div></div></div>\n",
                             "<script>\n",
                             "(function() {\n",
-                            "  var expanded = false;\n",
-                            "  var ellipsis = document.getElementById(\"6572\");\n",
+                            "  let expanded = false;\n",
+                            "  const ellipsis = document.getElementById(\"p1395\");\n",
                             "  ellipsis.addEventListener(\"click\", function() {\n",
-                            "    var rows = document.getElementsByClassName(\"6571\");\n",
-                            "    for (var i = 0; i < rows.length; i++) {\n",
-                            "      var el = rows[i];\n",
+                            "    const rows = document.getElementsByClassName(\"p1394\");\n",
+                            "    for (let i = 0; i < rows.length; i++) {\n",
+                            "      const el = rows[i];\n",
                             "      el.style.display = expanded ? \"none\" : \"table-row\";\n",
                             "    }\n",
                             "    ellipsis.innerHTML = expanded ? \"&hellip;)\" : \"&lsaquo;&lsaquo;&lsaquo;\";\n",
                             "    expanded = !expanded;\n",
                             "  });\n",
                             "})();\n",
                             "</script>\n"
                         ],
                         "text/plain": [
-                            "Figure(id='6021', ...)"
+                            "figure(id='p1329', ...)"
                         ]
                     },
-                    "execution_count": 36,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Remove consecutive same values\n",
                 "evenly_ts.compact().iplot(**kwargs_plot, show=True)"
@@ -839,15 +864,15 @@
             },
             "source": [
                 "## Pandas versus Ticts"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 37,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -890,64 +915,64 @@
                         "text/plain": [
                             "                           value\n",
                             "2019-01-01 00:00:00+00:00     10\n",
                             "2019-01-01 00:10:00+00:00     20\n",
                             "2019-01-01 00:15:00+00:00     10"
                         ]
                     },
-                    "execution_count": 37,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# From ticts to pandas and the other way arround\n",
                 "df = ts.to_dataframe()\n",
                 "df"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 38,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<TimeSeries>\n",
                             "2019-01-01T00:00:00+00:00: 10,\n",
                             "2019-01-01T00:10:00+00:00: 20,\n",
                             "2019-01-01T00:15:00+00:00: 10,"
                         ]
                     },
-                    "execution_count": 38,
+                    "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df.to_ticts()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.6.8"
+            "version": "3.11.9"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 4
 }
```

### Comparing `ticts-0.4.0/docs/_static/img/example.png` & `ticts-0.5.0/docs/img/example.png`

 * *Files identical despite different names*

### Comparing `ticts-0.4.0/docs/_static/img/logo.svg` & `ticts-0.5.0/docs/img/logo.svg`

 * *Files identical despite different names*

### Comparing `ticts-0.4.0/tests/conftest.py` & `ticts-0.5.0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from datetime import timedelta
 
 import pytest
 
 from ticts import TimeSeries
 from ticts.utils import timestamp_converter
 
-CURRENT = timestamp_converter('2019-01-01')
+CURRENT = timestamp_converter("2019-01-01")
 ONEHOUR = timedelta(hours=1)
 HALFHOUR = timedelta(minutes=30)
 ONEMIN = timedelta(minutes=1)
 
 
 @pytest.fixture
 def smalldict():
-    dct = dict()
+    dct = {}
     for i in range(10):
         dct[CURRENT + i * ONEHOUR] = i
     return dct
 
 
 @pytest.fixture
 def smallts(smalldict):
```

### Comparing `ticts-0.4.0/tests/test_io.py` & `ticts-0.5.0/tests/test_io.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,39 +2,34 @@
 
 from ticts import TimeSeries, testing
 
 
 class TestJSON:
     def test_serealize_iso(self, smallts):
         expected = {
-            'data': {key.isoformat(): value
-                     for key, value in smallts.items()},
-            'default': 'no_default',
-            'name': 'value'
+            "data": {key.isoformat(): value for key, value in smallts.items()},
+            "default": "no_default",
+            "name": "value",
         }
-        assert expected == smallts.serealize(date_format='iso')
+        assert expected == smallts.serealize(date_format="iso")
 
     def test_serealize_epoch(self, smallts):
         expected = {
-            'data': {key.value: value
-                     for key, value in smallts.items()},
-            'default': 'no_default',
-            'name': 'value'
+            "data": {key.value: value for key, value in smallts.items()},
+            "default": "no_default",
+            "name": "value",
         }
         assert expected == smallts.serealize()
 
     def test_to_json(self, smallts, tmpdir):
-        path = tmpdir.join('test.json')
+        path = tmpdir.join("test.json")
         smallts.to_json(path)
         expected = smallts.serealize()
-        expected['data'] = {
-            str(key): val
-            for key, val in expected['data'].items()
-        }
-        returned = json.load(open(path, "r"))
+        expected["data"] = {str(key): val for key, val in expected["data"].items()}
+        returned = json.load(open(path))
         assert returned == expected
 
     def test_it_returns_timeseries_from_json(self, smallts, tmpdir):
-        path = tmpdir.join('test.json')
+        path = tmpdir.join("test.json")
         smallts.to_json(path)
         ts_read = TimeSeries.from_json(path)
         testing.assert_ts_equal(smallts, ts_read)
```

### Comparing `ticts-0.4.0/tests/test_operation.py` & `ticts-0.5.0/tests/test_operation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import pytest
 
+from tests.conftest import CURRENT, HALFHOUR, ONEHOUR
 from ticts import TimeSeries, testing
-
-from .conftest import CURRENT, HALFHOUR, ONEHOUR
+from ticts.utils import NO_DEFAULT
 
 
 class TestTictsAdd:
     def test_simple_add(self, smallts, smalldict):
         ts = smallts + smallts
         newdct = {key: value + value for key, value in smalldict.items()}
         expected_ts = TimeSeries(newdct)
         testing.assert_ts_equal(ts, expected_ts)
 
     def test_simple_add_one_float(self, smallts):
         ts = smallts + 1000
         assert list(ts.values()) == list(range(1000, 1010))
 
-    def test_add_with_keys_differences_with_default(self, smallts_withdefault,
-                                                    otherts_withdefault):
+    def test_add_with_keys_differences_with_default(
+        self, smallts_withdefault, otherts_withdefault
+    ):
         ts = smallts_withdefault + otherts_withdefault
         assert ts.default == smallts_withdefault.default + otherts_withdefault.default
         assert ts[CURRENT + 1 * ONEHOUR] == 1 + otherts_withdefault.default
         assert ts[CURRENT + 2 * ONEHOUR] == 2 + 1000
         assert ts[CURRENT + 2 * ONEHOUR + HALFHOUR] == 2 + 2000
         assert ts[CURRENT + 3 * ONEHOUR] == 3 + 2000
         assert ts[CURRENT + 4 * ONEHOUR] == 4 + 3000
@@ -32,15 +33,16 @@
         assert CURRENT + 1 * ONEHOUR not in ts.index
         assert ts[CURRENT + 2 * ONEHOUR] == 2 + 1000
         assert ts[CURRENT + 2 * ONEHOUR + HALFHOUR] == 2 + 2000
         assert ts[CURRENT + 3 * ONEHOUR] == 3 + 2000
         assert ts[CURRENT + 4 * ONEHOUR] == 4 + 3000
 
     def test_add_with_keys_differences_with_mixed_default_nodefault(
-            self, smallts_withdefault, otherts):
+        self, smallts_withdefault, otherts
+    ):
         ts = smallts_withdefault + otherts
         assert not ts._has_default
         assert CURRENT + 1 * ONEHOUR not in ts.index
         assert ts[CURRENT + 2 * ONEHOUR] == 2 + 1000
         assert ts[CURRENT + 2 * ONEHOUR + HALFHOUR] == 2 + 2000
         assert ts[CURRENT + 3 * ONEHOUR] == 3 + 2000
         assert ts[CURRENT + 4 * ONEHOUR] == 4 + 3000
@@ -48,26 +50,41 @@
     def test_add_on_list_of_timeseries(self, smallts):
         lst_timeseries = [smallts, smallts, smallts]
         result = sum(lst_timeseries)
 
         for key in result:
             assert result[key] == 3 * smallts[key]
 
+    def test_add_on_no_default(self):
+        ts = TimeSeries({"2023-01-01": 1}, tz="CET")
+        result = ts + 0
+        assert result.default is NO_DEFAULT
+
+    def test_add_when_missing_values(self):
+        ts = TimeSeries({})
+        with pytest.raises(TypeError, match="Can't apply"):
+            ts + 0
+
+        ts = TimeSeries({}, default=1)
+        result = ts + 0
+        assert result.empty
+
 
 class TestTictsSub:
     def test_simple_sub(self, smallts):
         ts = smallts - smallts
-        assert all([val == 0 for val in ts.values()])
+        assert all(val == 0 for val in ts.values())
 
     def test_simple_sub_one_float(self, smallts):
         ts = smallts - 1
         assert list(ts.values()) == list(range(-1, 9))
 
-    def test_sub_with_keys_differences_with_default(self, smallts_withdefault,
-                                                    otherts_withdefault):
+    def test_sub_with_keys_differences_with_default(
+        self, smallts_withdefault, otherts_withdefault
+    ):
         ts = smallts_withdefault - otherts_withdefault
         assert ts[CURRENT + 1 * ONEHOUR] == 1 - 900
         assert ts[CURRENT + 2 * ONEHOUR] == 2 - 1000
         assert ts[CURRENT + 2 * ONEHOUR + HALFHOUR] == 2 - 2000
         assert ts[CURRENT + 3 * ONEHOUR] == 3 - 2000
         assert ts[CURRENT + 4 * ONEHOUR] == 4 - 3000
 
@@ -76,15 +93,16 @@
         assert CURRENT + 1 * ONEHOUR not in ts.index
         assert ts[CURRENT + 2 * ONEHOUR] == 2 - 1000
         assert ts[CURRENT + 2 * ONEHOUR + HALFHOUR] == 2 - 2000
         assert ts[CURRENT + 3 * ONEHOUR] == 3 - 2000
         assert ts[CURRENT + 4 * ONEHOUR] == 4 - 3000
 
     def test_sub_with_keys_differences_with_mixed_default_nodefault(
-            self, smallts_withdefault, otherts):
+        self, smallts_withdefault, otherts
+    ):
         ts = smallts_withdefault - otherts
         assert not ts._has_default
         assert CURRENT + 1 * ONEHOUR not in ts.index
         assert ts[CURRENT + 2 * ONEHOUR] == 2 - 1000
         assert ts[CURRENT + 2 * ONEHOUR + HALFHOUR] == 2 - 2000
         assert ts[CURRENT + 3 * ONEHOUR] == 3 - 2000
         assert ts[CURRENT + 4 * ONEHOUR] == 4 - 3000
@@ -92,16 +110,16 @@
 
 class TestTictsMul:
     def test_simple_mul(self, smallts):
         ts = smallts * smallts
         assert list(ts.values()) == [val * val for val in smallts.values()]
 
     def test_simple_mul_one_float(self, smallts):
-        ts = smallts * 1000.
-        assert list(ts.values()) == [val * 1000. for val in smallts.values()]
+        ts = smallts * 1000.0
+        assert list(ts.values()) == [val * 1000.0 for val in smallts.values()]
 
 
 class TestTictsDiv:
     def test_simple_div(self, smallts):
         smallts[CURRENT] = 1  # can't divide by zero
         ts = smallts / smallts
         assert list(ts.values()) == [val / val for val in smallts.values()]
@@ -109,71 +127,68 @@
     def test_simple_div_with_default_to_zero(self, smallts):
         smallts.default = 0
         smallts[CURRENT] = 1  # can't divide by zero
         ts = smallts / smallts
         assert not ts._has_default
 
     def test_simple_div_one_float(self, smallts):
-        ts = smallts / 1000.
-        assert list(ts.values()) == [val / 1000. for val in smallts.values()]
+        ts = smallts / 1000.0
+        assert list(ts.values()) == [val / 1000.0 for val in smallts.values()]
 
 
 class TestTictsBoolean:
     def test_simple_le(self, smallts):
         result = smallts >= 5
-        assert all([
-            not val for val in result[CURRENT:CURRENT + 4 * ONEHOUR].values()
-        ])
-        assert all([
-            val for val in result[CURRENT + 5 * ONEHOUR:CURRENT +
-                                  9 * ONEHOUR].values()
-        ])
+        assert all(not val for val in result[CURRENT : CURRENT + 4 * ONEHOUR].values())
+        assert all(
+            val
+            for val in result[CURRENT + 5 * ONEHOUR : CURRENT + 9 * ONEHOUR].values()
+        )
 
     def test_simple_lt(self, smallts):
         result = smallts > 5
-        assert all([
-            not val for val in result[CURRENT:CURRENT + 5 * ONEHOUR].values()
-        ])
-        assert all([
-            val for val in result[CURRENT + 6 * ONEHOUR:CURRENT +
-                                  9 * ONEHOUR].values()
-        ])
+        assert all(not val for val in result[CURRENT : CURRENT + 5 * ONEHOUR].values())
+        assert all(
+            val
+            for val in result[CURRENT + 6 * ONEHOUR : CURRENT + 9 * ONEHOUR].values()
+        )
 
     def test_simple_eq(self, smallts):
         ts = smallts == smallts
         assert all(ts.values())
 
 
 class TestTictsFloorCeil:
     def test_floor_on_float(self, smallts):
         ts = smallts.floor(2)
-        assert all([value <= 2 for value in ts.values()])
+        assert all(value <= 2 for value in ts.values())
 
     def test_floor_on_ts(self, smallts_withdefault, otherts_withdefault):
         ts = smallts_withdefault.floor(otherts_withdefault)
         assert ts[CURRENT + 1 * ONEHOUR] == 1
         assert ts[CURRENT + 2 * ONEHOUR] == 2
         assert ts[CURRENT + 2 * ONEHOUR + HALFHOUR] == 2
         assert ts[CURRENT + 3 * ONEHOUR] == 3
         assert ts[CURRENT + 4 * ONEHOUR] == 4
 
     def test_ceil_on_float(self, smallts):
         ts = smallts.ceil(7)
-        assert all([value >= 7 for value in ts.values()])
+        assert all(value >= 7 for value in ts.values())
 
     def test_ceil_on_ts(self, smallts_withdefault, otherts_withdefault):
         ts = smallts_withdefault.ceil(otherts_withdefault)
         assert ts[CURRENT + ONEHOUR] == 900
         assert ts[CURRENT + 2 * ONEHOUR] == 1000
         assert ts[CURRENT + 2 * ONEHOUR + HALFHOUR] == 2000
         assert ts[CURRENT + 3 * ONEHOUR] == 2000
         assert ts[CURRENT + 4 * ONEHOUR] == 3000
 
-    def test_ceil_on_ts_check_changing_default(self, smallts_withdefault,
-                                               otherts_withdefault):
+    def test_ceil_on_ts_check_changing_default(
+        self, smallts_withdefault, otherts_withdefault
+    ):
         otherts_withdefault.default = -10
         ts = smallts_withdefault.ceil(otherts_withdefault)
 
         assert ts[CURRENT + ONEHOUR] == 1
         assert ts[CURRENT + 2 * ONEHOUR] == 1000
         assert ts[CURRENT + 2 * ONEHOUR + HALFHOUR] == 2000
         assert ts[CURRENT + 3 * ONEHOUR] == 2000
@@ -199,43 +214,44 @@
     def test_simple_mask_update_raises_if_not_boolean(self, smallts):
         with pytest.raises(TypeError) as err:
             smallts.mask_update(smallts, smallts)
 
         assert "The values of the mask should all be boolean" in str(err.value)
 
     def test_mask_update_with_empty_no_default_other_raises(
-            self, smallts, emptyts, maskts):
+        self, smallts, emptyts, maskts
+    ):
         with pytest.raises(ValueError) as err:
             smallts.mask_update(emptyts, maskts)
-        assert 'other is empty and has no default set' in str(err.value)
+        assert "other is empty and has no default set" in str(err.value)
 
-    def test_mask_update_with_empty_and_no_default_mask_raises(
-            self, smallts, emptyts):
+    def test_mask_update_with_empty_and_no_default_mask_raises(self, smallts, emptyts):
         with pytest.raises(ValueError) as err:
             smallts.mask_update(smallts, emptyts)
-        assert 'mask is empty and has no default set' in str(err.value)
+        assert "mask is empty and has no default set" in str(err.value)
 
     def test_simple_mask_update(self, smallts, otherts, maskts):
         smallts_keys = smallts.index
         otherts_keys = otherts.index
         smallts.mask_update(otherts, maskts)
 
         assert set(smallts.index) == set(smallts_keys).union(set(otherts_keys))
 
         assert smallts[CURRENT + 2 * ONEHOUR] == 2
         assert smallts[CURRENT + 2 * ONEHOUR + HALFHOUR] == 2000
         assert smallts[CURRENT + 3 * ONEHOUR] == 2000
         assert smallts[CURRENT + 4 * ONEHOUR] == 4
 
     def test_mask_update_with_other_being_empty_with_default(
-            self, smallts, emptyts, maskts):
-        emptyts.default = -10.
+        self, smallts, emptyts, maskts
+    ):
+        emptyts.default = -10.0
         smallts.mask_update(emptyts, maskts)
 
         assert smallts[CURRENT + 2 * ONEHOUR] == 2
-        assert smallts[CURRENT + 3 * ONEHOUR] == -10.
+        assert smallts[CURRENT + 3 * ONEHOUR] == -10.0
         assert smallts[CURRENT + 4 * ONEHOUR] == 4
 
     def test_mask_update_on_emptyts(self, smallts, emptyts, maskts):
         emptyts.mask_update(smallts, maskts)
         expected_ts = TimeSeries({CURRENT + 3 * ONEHOUR: 3})
         testing.assert_ts_equal(emptyts, expected_ts)
```

### Comparing `ticts-0.4.0/tests/test_pandas_mixin.py` & `ticts-0.5.0/tests/test_pandas_mixin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,125 +1,131 @@
 import pandas as pd
 import pytest
 from pandas.tseries.frequencies import to_offset
 
+from tests.conftest import CURRENT, HALFHOUR, ONEHOUR, ONEMIN
 from ticts import TimeSeries, testing
 
-from .conftest import CURRENT, HALFHOUR, ONEHOUR, ONEMIN
-
 
 class TestToDataFrame:
     def test_to_dataframe(self, smallts):
-        smallts.name = 'SuperTS'
+        smallts.name = "SuperTS"
         df = smallts.to_dataframe()
         assert isinstance(df, pd.DataFrame)
-        assert df.columns.to_list() == ['SuperTS']
-        assert df.index.freq == '1H'
+        assert df.columns.to_list() == ["SuperTS"]
+        assert df.index.freq == "1H"
 
     def test_it_works_on_unevenly_spaced(self, otherts):
-        otherts.name = 'SuperTS'
+        otherts.name = "SuperTS"
         df = otherts.to_dataframe()
         assert isinstance(df, pd.DataFrame)
-        assert df.columns.to_list() == ['SuperTS']
+        assert df.columns.to_list() == ["SuperTS"]
         assert df.index.freq is None
 
 
 def test_from_df_to_ticst(smallts):
     df = smallts.to_dataframe()
     returned = df.to_ticts()
     testing.assert_ts_equal(smallts, returned)
 
 
 def test_from_series_to_ticst(smallts):
-    serie = smallts.to_dataframe()['value']
+    serie = smallts.to_dataframe()["value"]
     returned = serie.to_ticts()
     testing.assert_ts_equal(smallts, returned)
 
 
 class TestTimeSeriesSample:
     def test_it_raises_when_both_freq_and_index_are_none(self, smallts):
         with pytest.raises(Exception) as err:
             smallts.sample()
         assert "Both are None" in str(err.value)
 
     def test_simple_sample_on_default(self, smallts):
         ts = smallts.sample(HALFHOUR)
         expected_dict = {
             **smallts.data,
-            **{key + HALFHOUR: smallts[key]
-               for key in smallts.index[:-1]}
+            **{key + HALFHOUR: smallts[key] for key in smallts.index[:-1]},
         }
         expected_ts = TimeSeries(expected_dict, default=smallts.default)
         testing.assert_ts_equal(expected_ts, ts)
 
     def test_simple_by_passing_an_index(self, smallts):
         index = pd.date_range(
             start=smallts.lower_bound,
             end=smallts.upper_bound + 10 * ONEHOUR,
-            freq='3H',
-            closed='left')
+            freq="3H",
+            inclusive="left",
+        )
         ts = smallts.sample(index=index)
         assert list(ts.index) == index.to_list()
 
     def test_simple_sample_with_start_being_string(self, smallts):
-        start = '2019-01-01T09:00:00'
+        start = "2019-01-01T09:00:00"
         ts = smallts.sample(HALFHOUR, start=start)
         expected_ts = TimeSeries({start: 9})
         testing.assert_ts_equal(expected_ts, ts)
 
     def test_sample_out_of_left_bound_with_no_default_permissive_shorten_interval(
-            self, smallts):
+        self, smallts
+    ):
         ts = smallts.sample(
-            freq=HALFHOUR, start=CURRENT - ONEHOUR, end=CURRENT + ONEHOUR)
+            freq=HALFHOUR, start=CURRENT - ONEHOUR, end=CURRENT + ONEHOUR
+        )
         expected_ts = TimeSeries({CURRENT: 0, CURRENT + HALFHOUR: 0})
         testing.assert_ts_equal(expected_ts, ts)
 
     def test_sample_on_empty_return_empty_df(self, emptyts):
         assert emptyts.sample(freq=ONEHOUR).empty
 
     def test_sample_with_start_out_of_left_bounds_with_default(
-            self, smallts_withdefault):
+        self, smallts_withdefault
+    ):
         ts = smallts_withdefault.sample(freq=HALFHOUR, start=CURRENT - ONEHOUR)
         default = smallts_withdefault.default
         assert ts[CURRENT - ONEHOUR] == default
         assert ts[CURRENT - HALFHOUR] == default
         assert ts[CURRENT] == 0
         assert CURRENT + HALFHOUR in ts.index
 
     def test_sample_with_start_out_of_left_bounds(self, smallts):
         ts = smallts.sample(freq=HALFHOUR, start=CURRENT - ONEHOUR)
         CURRENT - ONEHOUR not in ts.index
         CURRENT - HALFHOUR not in ts.index
         assert ts[CURRENT] == 0
         assert CURRENT + HALFHOUR in ts.index
 
-    @pytest.mark.parametrize('freq', [
-        ONEMIN,
-        10 * ONEMIN,
-        '10Min',
-        pd.Timedelta(seconds=10),
-        ONEHOUR,
-        '1H',
-    ])
+    @pytest.mark.parametrize(
+        "freq",
+        [
+            ONEMIN,
+            10 * ONEMIN,
+            "10Min",
+            pd.Timedelta(seconds=10),
+            ONEHOUR,
+            "1H",
+        ],
+    )
     def test_sample_on_freq_with_end_and_start_in_bound(self, otherts, freq):
         start = CURRENT + 2 * ONEHOUR + HALFHOUR
         end = CURRENT + 3 * ONEHOUR + HALFHOUR
         ts = otherts.sample(freq=freq, start=start, end=end)
         freq = pd.Timedelta(freq)
         expected = [start + i * freq for i in range(int((end - start) / freq))]
         assert list(ts.index) == expected
 
-    @pytest.mark.parametrize('freq', ['MS', 'M', 'B'])
+    @pytest.mark.parametrize("freq", ["MS", "M", "B"])
     def test_sample_on_non_fixed_frequency(self, smallts, freq):
         ts = smallts.sample(freq)
         for start, end in ts.iterintervals():
             to_offset(end - start) == to_offset(freq)
 
     def test_sample_on_non_fixed_frequency_with_values(self, smallts):
-        freq = to_offset('MS')
+        freq = to_offset("MS")
         ts = smallts.sample(freq)
         expected_index = [smallts.lower_bound, smallts.lower_bound + freq]
         list(ts.index) == expected_index
         expected_values = [
-            smallts[smallts.lower_bound], smallts[smallts.lower_bound + freq]
+            smallts[smallts.lower_bound],
+            smallts[smallts.lower_bound + freq],
         ]
         list(ts.values()) == expected_values
```

### Comparing `ticts-0.4.0/tests/test_timeseries.py` & `ticts-0.5.0/tests/test_timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,94 +1,90 @@
 from copy import copy, deepcopy
 from datetime import datetime
 from unittest import mock
 
 import pandas as pd
 import pytest
 
+from tests.conftest import CURRENT, HALFHOUR, ONEHOUR, ONEMIN
 from ticts import TimeSeries, testing
 from ticts.utils import MAXTS, MINTS, timestamp_converter
 
-from .conftest import CURRENT, HALFHOUR, ONEHOUR, ONEMIN
-
 
 class TestTimeSeriesInit:
     def test_with_dict(self, smalldict):
         ts = TimeSeries(smalldict, default=10)
         assert ts[CURRENT + ONEHOUR] == 1
         assert ts.default == 10
 
     def test_with_dict_keys_being_strings(self):
         dct = {
-            '2019-01-01': 1,
-            '2019-02-01': 2,
-            timestamp_converter('2019-03-01'): 3,
+            "2019-01-01": 1,
+            "2019-02-01": 2,
+            timestamp_converter("2019-03-01"): 3,
         }
         ts = TimeSeries(dct, default=10)
-        expected = {
-            timestamp_converter(key): value
-            for key, value in dct.items()
-        }
+        expected = {timestamp_converter(key): value for key, value in dct.items()}
         assert ts.items() == expected.items()
         assert ts.default == 10
 
     def test_with_data_as_tuple(self):
         mytuple = (
             (CURRENT, 0),
-            ('2019-02-01', 1),
+            ("2019-02-01", 1),
         )
         ts = TimeSeries(mytuple, default=10)
         assert ts[CURRENT] == 0
-        assert ts['2019-02-01'] == 1
+        assert ts["2019-02-01"] == 1
         assert len(ts) == 2
         assert ts.default == 10
 
     def test_with_data_as_pandas_series(self, smalldict):
-        serie = pd.Series(data=smalldict, name='SomeName')
+        serie = pd.Series(data=smalldict, name="SomeName")
         ts = TimeSeries(serie)
-        assert ts.name == 'SomeName'
+        assert ts.name == "SomeName"
         assert ts[CURRENT] == 0
         assert len(ts) == len(serie)
 
     def test_with_data_as_dataframe(self, smalldict):
         df = pd.DataFrame(
-            data={'SomeName': list(smalldict.values())},
-            index=smalldict.keys())
+            data={"SomeName": list(smalldict.values())}, index=smalldict.keys()
+        )
         ts = TimeSeries(df, default=10)
         assert ts[CURRENT] == 0
-        assert ts.name == 'SomeName'
+        assert ts.name == "SomeName"
         assert len(ts) == df.shape[0]
         assert ts.default == 10
 
     def test_with_data_as_dataframe_raises_when_several_columns(self):
-        df = pd.DataFrame(columns=['Too', 'Many', 'Columns'])
+        df = pd.DataFrame(columns=["Too", "Many", "Columns"])
         with pytest.raises(Exception) as err:
             TimeSeries(df)
 
         expected = "Can't convert a DataFrame with several columns"
         assert expected in str(err.value)
 
     def test_with_data_as_ticts_timeserie(self, smallts):
         smallts.default = 1000
-        smallts.name = 'SomeName'
+        smallts.name = "SomeName"
         testing.assert_ts_equal(smallts, TimeSeries(smallts))
 
     def test_with_data_as_ticts_timeserie_and_default_given(self, smallts):
         smallts.default = 1000
-        smallts.name = 'SomeName'
-        newts = TimeSeries(smallts, default=1.)
+        smallts.name = "SomeName"
+        newts = TimeSeries(smallts, default=1.0)
         testing.assert_ts_equal(smallts, newts, check_default=False)
-        assert newts.default == 1.
+        assert newts.default == 1.0
 
     def test_with_data_as_ticts_timeserie_and_name_given(self, smallts):
         smallts.default = 1000
-        smallts.name = 'SomeName'
-        newts = TimeSeries(smallts, name='SomeOtherName')
+        smallts.name = "SomeName"
+        newts = TimeSeries(smallts, name="SomeOtherName")
         testing.assert_ts_equal(smallts, newts, check_name=False)
-        assert newts.name == 'SomeOtherName'
+        assert newts.name == "SomeOtherName"
 
 
 class TestTimeSeriesSetItem:
     def test_simple_setitem(self, smallts):
         smallts[CURRENT] = 1000
         assert smallts[CURRENT] == 1000
 
@@ -96,15 +92,15 @@
         smallts[CURRENT] = 1000
         first_time = TimeSeries(smallts)
         smallts[CURRENT] = 1000
         testing.assert_ts_equal(first_time, smallts)
 
     @mock.patch("ticts.TimeSeries.set_interval")
     def test_setitem_on_slice_calls_set_interval(self, set_interval, smallts):
-        smallts[CURRENT:CURRENT + 2 * ONEHOUR] = 1000
+        smallts[CURRENT : CURRENT + 2 * ONEHOUR] = 1000
         assert set_interval.call_count == 1
 
 
 class TestTictsMagicMixin:
     # Copy / Deepcopy
 
     def test_copy(self, smallts):
@@ -122,27 +118,27 @@
     def test_deepcopy_with_default(self, smallts_withdefault):
         deepcopied = deepcopy(smallts_withdefault)
         testing.assert_ts_equal(deepcopied, smallts_withdefault)
 
     # Repr
 
     def test_repr_on_otherts(self, otherts):
-        assert repr(otherts).count('\n') == 3
+        assert repr(otherts).count("\n") == 3
 
     def test_repr_on_large(self):
-        dct = dict()
+        dct = {}
         for i in range(100):
             dct[CURRENT + i * ONEHOUR] = i
         ts = TimeSeries(dct)
-        assert repr(ts).count('\n') == 11
+        assert repr(ts).count("\n") == 11
 
     def test_repr_with_default_and_name(self, smallts_withdefault):
-        smallts_withdefault.name = 'SuperCool'
-        assert 'default=' in repr(smallts_withdefault)
-        assert 'name=' in repr(smallts_withdefault)
+        smallts_withdefault.name = "SuperCool"
+        assert "default=" in repr(smallts_withdefault)
+        assert "name=" in repr(smallts_withdefault)
 
     # Accessors
 
     def test_values(self, smallts):
         values = smallts.values()
         series_values = [v for k, v in smallts.items()]
 
@@ -159,15 +155,15 @@
         assert CURRENT not in smallts.index
 
     # Update
 
     def test_update(self, smallts):
         og_ts = deepcopy(smallts)
         last_index = smallts.index[-1]
-        new_index = last_index + pd.Timedelta('2 days')
+        new_index = last_index + pd.Timedelta("2 days")
         new_value = 10
 
         # Updating with TimeSeries
         other = TimeSeries({new_index: new_value, last_index: new_value})
         og_ts.update(other)
 
         assert og_ts[new_index] == new_value
@@ -178,15 +174,15 @@
         other_tuple = tuple(other.items())
         og_ts.update(other_tuple)
 
         assert og_ts[new_index] == new_value
 
         # Updating with *args
         og_ts = deepcopy(smallts)
-        other_new_index = new_index + pd.Timedelta('2 hours')
+        other_new_index = new_index + pd.Timedelta("2 hours")
         other_new = TimeSeries({other_new_index: new_value})
         og_ts.update([other, other_new])
 
         assert og_ts[new_index] == new_value
         assert og_ts[other_new_index] == new_value
 
         # Updating with dict
@@ -198,15 +194,15 @@
         # Updating with **kwargs
         og_ts = deepcopy(smallts)
         with pytest.raises(TypeError):
             og_ts.update(**{new_index: new_value})
 
 
 class TestTimeSeriesDefault:
-    @pytest.mark.parametrize('default', [None, 0, False])
+    @pytest.mark.parametrize("default", [None, 0, False])
     def test_it_has_default(self, default):
         ts = TimeSeries(default=default)
         assert ts._has_default
 
     def test_it_has_no_default(self):
         ts = TimeSeries()
         assert not ts._has_default
@@ -242,240 +238,243 @@
 
 def test_timeseries_compact(smallts):
     smallts[CURRENT + ONEMIN] = 0
     assert (CURRENT + ONEMIN) not in smallts.compact().index
 
 
 class TestTimeSeriesGetitem:
-    available_interpolate = ['previous', 'linear']
+    available_interpolate = ["previous", "linear"]
 
     # tests on corner cases
 
     def test_get_item_out_of_left_bound_with_default_zero(self):
         mytuple = ((CURRENT, 0), (CURRENT + ONEHOUR, 1))
         ts = TimeSeries(mytuple, default=0)
         assert ts[CURRENT + ONEHOUR] == 1
         assert ts[CURRENT - ONEHOUR] == 0
 
     def test_getitem_out_of_left_bound_with_no_default_and_permissive_return_None(
-            self, smallts):
+        self, smallts
+    ):
         assert smallts[CURRENT - ONEMIN] is None
 
     def test_getitem_out_of_left_bound_with_no_default_and_not_permissive_raises(
-            self, smallts):
+        self, smallts
+    ):
         smallts.permissive = False
         with pytest.raises(KeyError) as err:
             smallts[CURRENT - ONEMIN]
-        assert 'default attribute is not set' in str(err.value)
+        assert "default attribute is not set" in str(err.value)
 
     def test_getitem_using_str(self, smallts):
-        smallts['2019-01-01'] == 0
+        smallts["2019-01-01"] == 0
 
-    @pytest.mark.parametrize('interpolate', available_interpolate)
+    @pytest.mark.parametrize("interpolate", available_interpolate)
     def test_getitem_out_of_left_bound_with_default_return_default(
-            self, smallts_withdefault, interpolate):
+        self, smallts_withdefault, interpolate
+    ):
         value = smallts_withdefault[CURRENT - ONEMIN, interpolate]
         assert value == smallts_withdefault.default
 
-    @pytest.mark.parametrize('interpolate', available_interpolate)
+    @pytest.mark.parametrize("interpolate", available_interpolate)
     def test_getitem_on_empty_when_no_default_not_permissive_raises(
-            self, emptyts, interpolate):
+        self, emptyts, interpolate
+    ):
         emptyts.permissive = False
         with pytest.raises(KeyError) as err:
             emptyts[CURRENT - ONEMIN, interpolate]
 
         expected = "default attribute is not set and timeseries is empty"
         assert expected in str(err.value)
 
-    @pytest.mark.parametrize('interpolate', available_interpolate)
-    def test_getitem_on_empty_when_no_default_return_None(
-            self, emptyts, interpolate):
+    @pytest.mark.parametrize("interpolate", available_interpolate)
+    def test_getitem_on_empty_when_no_default_return_None(self, emptyts, interpolate):
         emptyts[CURRENT - ONEMIN, interpolate] is None
 
     # tests on '_get_previous'
 
     @mock.patch("ticts.TimeSeries._get_previous")
-    def test_get_on_previous_is_default_interpolate(self, _get_previous,
-                                                    smallts):
+    def test_get_on_previous_is_default_interpolate(self, _get_previous, smallts):
         smallts[CURRENT + ONEMIN]
         assert _get_previous.call_count == 1
 
     def test_get_on_previous(self, smallts):
         assert smallts[CURRENT + ONEMIN] == 0
 
     def test_get_on_previous_out_of_right_bound(self, smallts):
         assert smallts[CURRENT + 10 * ONEHOUR] == 9
 
     def test_get_on_previous_out_of_left_bound_no_default(self, smallts):
         assert smallts[CURRENT - ONEHOUR] is None
 
-    def test_get_on_previous_out_of_left_bound_with_default(
-            self, smallts_withdefault):
-        assert smallts_withdefault[CURRENT -
-                                   ONEHOUR] == smallts_withdefault.default
+    def test_get_on_previous_out_of_left_bound_with_default(self, smallts_withdefault):
+        assert smallts_withdefault[CURRENT - ONEHOUR] == smallts_withdefault.default
 
     # tests on '_get_linear_interpolate'
 
-    @pytest.mark.parametrize('time_idx, expected', [
-        (CURRENT + HALFHOUR, 0.5),
-        (CURRENT + ONEHOUR + HALFHOUR, 1.5),
-        (CURRENT + 10 * ONEMIN, 0 + (1 - 0) * (10 * ONEMIN / ONEHOUR)),
-    ])
+    @pytest.mark.parametrize(
+        "time_idx, expected",
+        [
+            (CURRENT + HALFHOUR, 0.5),
+            (CURRENT + ONEHOUR + HALFHOUR, 1.5),
+            (CURRENT + 10 * ONEMIN, 0 + (1 - 0) * (10 * ONEMIN / ONEHOUR)),
+        ],
+    )
     def test_get_linear_interpolate(self, smallts, time_idx, expected):
-        assert smallts[time_idx, 'linear'] == expected
+        assert smallts[time_idx, "linear"] == expected
 
     def test_get_linear_interpolate_out_of_right_bound(self, smallts):
-        assert smallts[CURRENT + 10 * ONEHOUR, 'linear'] == 9
+        assert smallts[CURRENT + 10 * ONEHOUR, "linear"] == 9
 
-    def test_get_linear_interpolate_out_of_left_bound_no_default(
-            self, smallts):
-        assert smallts[CURRENT - ONEHOUR, 'linear'] is None
+    def test_get_linear_interpolate_out_of_left_bound_no_default(self, smallts):
+        assert smallts[CURRENT - ONEHOUR, "linear"] is None
 
     def test_get_linear_interpolate_out_of_left_bound_with_default(
-            self, smallts_withdefault):
-        assert smallts_withdefault[CURRENT - ONEHOUR,
-                                   'linear'] == smallts_withdefault.default
+        self, smallts_withdefault
+    ):
+        assert (
+            smallts_withdefault[CURRENT - ONEHOUR, "linear"]
+            == smallts_withdefault.default
+        )
 
     # test on 'slice'
 
-    def test_get_on_slice_exclude_upper_bound_include_lower_bound(
-            self, smallts):
+    def test_get_on_slice_exclude_upper_bound_include_lower_bound(self, smallts):
         start = CURRENT
         end = CURRENT + 1 * ONEHOUR
-        sliced_ts = smallts[start:end + ONEHOUR]
+        sliced_ts = smallts[start : end + ONEHOUR]
 
         data = {start: 0, end: 1}
         expected_ts = TimeSeries(data, default=smallts.default)
         testing.assert_ts_equal(sliced_ts, expected_ts)
 
-    def test_get_on_slice_add_back_previous_value_if_start_not_in_keys(
-            self, smallts):
+    def test_get_on_slice_add_back_previous_value_if_start_not_in_keys(self, smallts):
         start = CURRENT + HALFHOUR
         end = CURRENT + ONEHOUR
-        sliced_ts = smallts[start:end + ONEHOUR]
+        sliced_ts = smallts[start : end + ONEHOUR]
 
         data = {start: 0, end: 1}
         expected_ts = TimeSeries(data, default=smallts.default)
         testing.assert_ts_equal(sliced_ts, expected_ts)
 
     def test_get_on_slice_entirely_out_of_bounds_on_left_side(self, smallts):
-        assert smallts[CURRENT - 2 * ONEHOUR:CURRENT - 1 * ONEHOUR].empty
+        assert smallts[CURRENT - 2 * ONEHOUR : CURRENT - 1 * ONEHOUR].empty
 
     def test_get_on_slice_out_of_bounds_left_side(self, smallts):
         start = CURRENT - 2 * ONEHOUR
         end = CURRENT
         data = {CURRENT: 0}
-        sliced_ts = smallts[start:end + 1 * ONEHOUR]
+        sliced_ts = smallts[start : end + 1 * ONEHOUR]
         expected_ts = TimeSeries(data, default=smallts.default)
         testing.assert_ts_equal(sliced_ts, expected_ts)
 
     def test_get_on_slice_entirely_out_of_bounds_on_right_side(self, smallts):
         start = CURRENT + 10 * ONEHOUR
         end = CURRENT + 12 * ONEHOUR
         sliced_ts = smallts[start:end]
         expected_ts = TimeSeries({start: smallts[start]})
         testing.assert_ts_equal(sliced_ts, expected_ts)
 
     def test_get_on_slice_out_of_bounds_on_right_side(self, smallts):
-        sliced_ts = smallts[CURRENT + 9 * ONEHOUR:CURRENT + 12 * ONEHOUR]
+        sliced_ts = smallts[CURRENT + 9 * ONEHOUR : CURRENT + 12 * ONEHOUR]
         expected_dct = {CURRENT + 9 * ONEHOUR: 9}
         expected_ts = TimeSeries(expected_dct, default=smallts.default)
         testing.assert_ts_equal(sliced_ts, expected_ts)
 
 
 class TestTimeSeriesSetInterval:
     def test_set_interval_when_no_default_raises(self, smallts):
         with pytest.raises(NotImplementedError):
             smallts.set_interval(CURRENT, CURRENT + ONEHOUR, 1000)
 
     def test_single_set_interval_end_on_last_key(self, smallts_withdefault):
-        smallts_withdefault.set_interval(CURRENT + ONEHOUR,
-                                         CURRENT + 9 * ONEHOUR, 1000)
+        smallts_withdefault.set_interval(CURRENT + ONEHOUR, CURRENT + 9 * ONEHOUR, 1000)
         expected_keys = [CURRENT, CURRENT + ONEHOUR, CURRENT + 9 * ONEHOUR]
         assert list(smallts_withdefault.index) == expected_keys
         assert smallts_withdefault[CURRENT + ONEHOUR] == 1000
-        assert smallts_withdefault[CURRENT + 9 * ONEHOUR] == 9.
+        assert smallts_withdefault[CURRENT + 9 * ONEHOUR] == 9.0
 
     def test_single_set_interval_start_on_first_key(self, smallts_withdefault):
         smallts_withdefault.set_interval(CURRENT, CURRENT + 9 * ONEHOUR, 1000)
         expected_keys = [CURRENT, CURRENT + 9 * ONEHOUR]
         assert list(smallts_withdefault.index) == expected_keys
         assert smallts_withdefault[CURRENT] == 1000
-        assert smallts_withdefault[CURRENT + 9 * ONEHOUR] == 9.
+        assert smallts_withdefault[CURRENT + 9 * ONEHOUR] == 9.0
 
-    @pytest.mark.parametrize('start, end', [
-        (CURRENT + ONEHOUR, CURRENT + 10 * ONEHOUR),
-        (CURRENT + 4 * ONEHOUR, CURRENT + 11 * ONEHOUR),
-    ])
+    @pytest.mark.parametrize(
+        "start, end",
+        [
+            (CURRENT + ONEHOUR, CURRENT + 10 * ONEHOUR),
+            (CURRENT + 4 * ONEHOUR, CURRENT + 11 * ONEHOUR),
+        ],
+    )
     def test_single_set_interval_end_over_last_key_sets_to_last_value(
-            self, smallts_withdefault, start, end):
+        self, smallts_withdefault, start, end
+    ):
         last_key = smallts_withdefault.index[-1]
         last_val = smallts_withdefault[last_key]
 
         smallts_withdefault.set_interval(start, end, 1000)
         keys_before_start = []
         for key in smallts_withdefault.index:
             if key < start:
                 keys_before_start.append(key)
 
         expected_keys = [*keys_before_start, start, end]
         assert list(smallts_withdefault.index) == expected_keys
         assert smallts_withdefault[end] == last_val
 
     def test_single_set_interval_when_start_higher_than_upper_bound(
-            self, smallts_withdefault):
+        self, smallts_withdefault
+    ):
         start = CURRENT + 11 * ONEHOUR
         end = CURRENT + 13 * ONEHOUR
         smallts_withdefault.set_interval(start, end, 1000)
 
         assert CURRENT + 10 * ONEHOUR not in smallts_withdefault.index
         assert smallts_withdefault[CURRENT + 10 * ONEHOUR] == 9
 
         assert smallts_withdefault[start] == 1000
         assert smallts_withdefault[end] == 9
 
-    def test_single_set_interval_start_before_first_key(
-            self, smallts_withdefault):
-        smallts_withdefault.set_interval(CURRENT - ONEHOUR,
-                                         CURRENT + 9 * ONEHOUR, 1000)
+    def test_single_set_interval_start_before_first_key(self, smallts_withdefault):
+        smallts_withdefault.set_interval(CURRENT - ONEHOUR, CURRENT + 9 * ONEHOUR, 1000)
         expected_keys = [CURRENT - ONEHOUR, CURRENT + 9 * ONEHOUR]
         assert list(smallts_withdefault.index) == expected_keys
         assert smallts_withdefault[CURRENT - 1 * ONEHOUR] == 1000
 
-    def test_single_set_interval_on_bounds_not_being_keys(
-            self, smallts_withdefault):
-        smallts_withdefault.set_interval(CURRENT + ONEMIN,
-                                         CURRENT + 9 * ONEHOUR, 1000)
+    def test_single_set_interval_on_bounds_not_being_keys(self, smallts_withdefault):
+        smallts_withdefault.set_interval(CURRENT + ONEMIN, CURRENT + 9 * ONEHOUR, 1000)
         expected_keys = [CURRENT, CURRENT + ONEMIN, CURRENT + 9 * ONEHOUR]
         assert list(smallts_withdefault.index) == expected_keys
         assert smallts_withdefault[CURRENT + ONEMIN] == 1000
 
     def test_set_interval_on_empty(self, emptyts):
         emptyts.default = 10
         emptyts.set_interval(CURRENT, CURRENT + ONEHOUR, 1)
         assert emptyts[CURRENT] == 1
         assert emptyts[CURRENT + ONEHOUR] == 10
         assert len(emptyts.index) == 2
 
     def test_set_interval_on_empty_with_default(self, emptyts_withdefault):
         emptyts_withdefault.set_interval(CURRENT, CURRENT + ONEHOUR, 1)
         assert emptyts_withdefault[CURRENT] == 1
-        assert emptyts_withdefault[CURRENT +
-                                   ONEHOUR] == emptyts_withdefault.default
+        assert emptyts_withdefault[CURRENT + ONEHOUR] == emptyts_withdefault.default
         len(emptyts_withdefault.index) == 2
 
-    @pytest.mark.parametrize('start, end', (
-        (CURRENT, CURRENT + 9 * ONEHOUR),
-        (CURRENT + 5 * ONEHOUR, CURRENT + 12 * ONEHOUR),
-        (datetime(2019, 1, 1) + 5 * ONEHOUR,
-         datetime(2019, 1, 1) + 12 * ONEHOUR),
-        ('2019-01-01T05:00:00', '2019-01-01T12:00:00+02:00'),
-    ))
-    def test_same_consecutive_set_interval(self, smallts_withdefault, start,
-                                           end):
+    @pytest.mark.parametrize(
+        "start, end",
+        (
+            (CURRENT, CURRENT + 9 * ONEHOUR),
+            (CURRENT + 5 * ONEHOUR, CURRENT + 12 * ONEHOUR),
+            (datetime(2019, 1, 1) + 5 * ONEHOUR, datetime(2019, 1, 1) + 12 * ONEHOUR),
+            ("2019-01-01T05:00:00", "2019-01-01T12:00:00+02:00"),
+        ),
+    )
+    def test_same_consecutive_set_interval(self, smallts_withdefault, start, end):
         smallts_withdefault.set_interval(start, end, 1000)
         first_time = deepcopy(smallts_withdefault)
 
         for _ in range(10):
             smallts_withdefault.set_interval(start, end, 1000)
 
         testing.assert_ts_equal(first_time, smallts_withdefault)
@@ -490,53 +489,56 @@
         assert emptyts[CURRENT + 2 * ONEHOUR] == 10
         assert list(emptyts.index) == [CURRENT, CURRENT + 2 * ONEHOUR]
 
     def test_set_interval_when_no_keys_to_delete_with_default(self, emptyts):
         emptyts.default = 1000
         emptyts.set_interval(CURRENT, CURRENT + 1 * ONEHOUR, 0)
         emptyts.set_interval(CURRENT + 3 * ONEHOUR, CURRENT + 4 * ONEHOUR, 3)
-        emptyts.set_interval(CURRENT + 1 * ONEHOUR + HALFHOUR,
-                             CURRENT + 3 * ONEHOUR, 10)
+        emptyts.set_interval(
+            CURRENT + 1 * ONEHOUR + HALFHOUR, CURRENT + 3 * ONEHOUR, 10
+        )
 
         expected_dct = {
             CURRENT: 0,
-            CURRENT + 1 * ONEHOUR: 1000.,
+            CURRENT + 1 * ONEHOUR: 1000.0,
             CURRENT + 1 * ONEHOUR + HALFHOUR: 10,
             CURRENT + 3 * ONEHOUR: 3,
-            CURRENT + 4 * ONEHOUR: 1000
+            CURRENT + 4 * ONEHOUR: 1000,
         }
         assert list(emptyts.index) == list(expected_dct.keys())
 
         for key in expected_dct:
             assert emptyts[key] == expected_dct[key]
 
 
 class TestIterIntervals:
     def test_simple_iterintervals(self, smallts):
         iterator = smallts.iterintervals()
-        result = [(start, end) for start, end in iterator]
-        expected = [(CURRENT + i * ONEHOUR, CURRENT + (i + 1) * ONEHOUR)
-                    for i in range(9)]
+        result = list(iterator)
+        expected = [
+            (CURRENT + i * ONEHOUR, CURRENT + (i + 1) * ONEHOUR) for i in range(9)
+        ]
         assert sorted(result) == sorted(expected)
 
     def test_iterintervals_with_end(self, smallts):
         end = CURRENT + 3 * ONEHOUR + HALFHOUR
         iterator = smallts.iterintervals(end)
-        result = [(start, end) for start, end in iterator]
-        expected = [(CURRENT + i * ONEHOUR, CURRENT + (i + 1) * ONEHOUR)
-                    for i in range(3)]
+        result = list(iterator)
+        expected = [
+            (CURRENT + i * ONEHOUR, CURRENT + (i + 1) * ONEHOUR) for i in range(3)
+        ]
         expected.append((CURRENT + 3 * ONEHOUR, end))
         assert sorted(result) == sorted(expected)
 
 
 class TestTzConvert:
     def test_simple_tz_convert(self, smallts):
-        ts = smallts.tz_convert('CET')
-        assert ts.tz == 'CET'
-        assert smallts.tz == 'UTC'
+        ts = smallts.tz_convert("CET")
+        assert ts.tz == "CET"
+        assert smallts.tz == "UTC"
 
 
 def test_chain_operations_keep_meta_keys(smallts_withdefault):
     ts = smallts_withdefault
-    otherts = ts.compact().sample('1T')
+    otherts = ts.compact().sample("1T")
     for attr_name in ts._meta_keys:
         assert getattr(ts, attr_name) == getattr(otherts, attr_name)
```

### Comparing `ticts-0.4.0/ticts/operation.py` & `ticts-0.5.0/ticts/operation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
 
-from .utils import MINTS, NO_DEFAULT, operation_factory
+from ticts.utils import MINTS, NO_DEFAULT, operation_factory
 
 logger = logging.getLogger(__name__)
 
 
 def _get_keys_for_operation(ts1, ts2, *args):
     all_ts = [ts1, ts2, *args]
     for ts in all_ts:
-        if not ts.__class__.__name__ == 'TimeSeries':
-            raise TypeError("{} is not of type TimeSeries".format(ts))
+        if not ts.__class__.__name__ == "TimeSeries":
+            raise TypeError(f"{ts} is not of type TimeSeries")
 
     all_keys = set.union(*[set(ts.index) for ts in all_ts])
 
     lower_bound = MINTS
     for ts in all_ts:
         if not ts._has_default:
             lower_bound = max(lower_bound, ts.lower_bound)
@@ -22,82 +22,88 @@
 
 
 class TictsOperationMixin:
     def _operate(self, other, operator):
         if isinstance(other, self.__class__):
             return self._operate_on_ts(other, operator)
         else:
-            return self._operate_on_one_value(other, operator)
+            return self._operate_on_scalar(other, operator)
 
     def _operate_on_ts(self, other, operator):
         if not isinstance(other, self.__class__):
             raise TypeError
 
         all_keys = set(self.index).union(set(other.index))
 
         default = NO_DEFAULT
         if self._has_default and other._has_default:
             try:
                 default = operator(self.default, other.default)
             except ZeroDivisionError:
                 default = NO_DEFAULT
-                msg = ("The TimeSeries has 0. as default value."
-                       " Can't compute the resulting default.")
+                msg = (
+                    "The TimeSeries has 0. as default value."
+                    " Can't compute the resulting default."
+                )
                 logger.warning(msg)
 
         all_keys = _get_keys_for_operation(self, other)
 
         ts = self.__class__(default=default)
         for key in all_keys:
             ts[key] = operator(self[key], other[key])
 
         return ts
 
-    def _operate_on_one_value(self, value, operator):
-        sample_value = self.values()[0]
+    def _operate_on_scalar(self, value, operator):
+        sample_value = self.values()[0] if not self.empty else self.default
         try:
             operator(sample_value, value)
-        except Exception:
+        except Exception as err:
             msg = "Can't apply {} on {} with {}."
             raise TypeError(
-                msg.format(operator.__name__, sample_value.__class__.__name__,
-                           value.__class__.__name__))
+                msg.format(
+                    operator.__name__,
+                    sample_value.__class__.__name__,
+                    value.__class__.__name__,
+                )
+            ) from err
 
-        default = None
+        default = NO_DEFAULT
         if self._has_default:
             default = operator(self.default, value)
 
         ts = self.__class__(default=default)
         for key in self.index:
             ts[key] = operator(self[key], value)
 
         return ts
 
-    __add__ = operation_factory('__add__')
-    __radd__ = operation_factory('__add__')
-    __sub__ = operation_factory('__sub__')
-
-    __mul__ = operation_factory('__mul__')
-    __truediv__ = operation_factory('__truediv__')
-    __floordiv__ = operation_factory('__floordiv__')
-
-    __abs__ = operation_factory('__abs__')
-
-    __lt__ = operation_factory('__lt__')
-    __le__ = operation_factory('__le__')
-    __gt__ = operation_factory('__gt__')
-    __ge__ = operation_factory('__ge__')
-    __eq__ = operation_factory('__eq__')
-
-    __or__ = operation_factory('__or__')
-    __xor__ = operation_factory('__xor__')
-    __and__ = operation_factory('__and__')
+    __add__ = operation_factory("__add__")
+    __radd__ = operation_factory("__add__")
+    __sub__ = operation_factory("__sub__")
+
+    __mul__ = operation_factory("__mul__")
+    __truediv__ = operation_factory("__truediv__")
+    __floordiv__ = operation_factory("__floordiv__")
+
+    __abs__ = operation_factory("__abs__")
+
+    __lt__ = operation_factory("__lt__")
+    __le__ = operation_factory("__le__")
+    __gt__ = operation_factory("__gt__")
+    __ge__ = operation_factory("__ge__")
+    __eq__ = operation_factory("__eq__")
+
+    __or__ = operation_factory("__or__")
+    __xor__ = operation_factory("__xor__")
+    __and__ = operation_factory("__and__")
 
-    __inv__ = operation_factory('__inv__')
-    __not__ = operation_factory('__not__')
+    __inv__ = operation_factory("__inv__")
+    __not__ = operation_factory("__not__")
 
     def floor(self, other):
         """Floor your timeseries, applying a min key by key.
 
         Args:
             other (TimeSeries or numeric): values to floor on.
 
@@ -125,19 +131,19 @@
             mask (TimeSeries): timeseries with boolean values.
 
         Returns:
             TimeSeries
         """
         # Type checks
         if not isinstance(other, self.__class__):
-            msg = 'other should be of type TimeSeries, got {}'
+            msg = "other should be of type TimeSeries, got {}"
             raise TypeError(msg.format(type(other)))
 
-        if not all([isinstance(value, bool) for value in mask.values()]):
-            msg = 'The values of the mask should all be boolean.'
+        if not all(isinstance(value, bool) for value in mask.values()):
+            msg = "The values of the mask should all be boolean."
             raise TypeError(msg)
 
         # Empty ts checks
         if mask.empty and not mask._has_default:
             msg = "mask is empty and has no default set"
             raise ValueError(msg)
```

### Comparing `ticts-0.4.0/ticts/pandas_mixin.py` & `ticts-0.5.0/ticts/pandas_mixin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 import pandas as pd
 from pandas.tseries.frequencies import infer_freq, to_offset
 
-from .utils import timestamp_converter
+from ticts.utils import timestamp_converter
 
 
 class PandasMixin:
     def to_dataframe(self):
         df = pd.DataFrame(data={self.name: self.values()}, index=self.index)
 
         # Need at least 3 dates to infer frequency
         if len(df.index) >= 3:
             # Try to infer freq if is evenly-spaced to get the df.index.freq
             df.index.freq = infer_freq(df.index)
 
         return df
 
-    def sample(self,
-               freq=None,
-               start=None,
-               end=None,
-               index=None,
-               interpolate=None):
+    def sample(self, freq=None, start=None, end=None, index=None, interpolate=None):
         """Sample your timeseries into Evenly Spaced TimeSeries.
 
         Args:
             freq (timedelta): frequency to convert in.
             start (datetime): left bound. Default to None, which result into
                 :meth:`~timeseries.TimeSeries.lower_bound`.
             end (datetime): right bound. Default to None, which result into
                 :meth:`~timeseries.TimeSeries.upper_bound`.
 
         Returns:
             evenly-spaced timeseries.
         """
 
         if freq is None and index is None:
-            msg = ("You should either select one frequency OR an index for "
-                   "the sampling. Both are None.")
+            msg = (
+                "You should either select one frequency OR an index for "
+                "the sampling. Both are None."
+            )
             raise ValueError(msg)
 
         if not interpolate:
             interpolate = self._default_interpolate
 
         freq = to_offset(freq)
```

### Comparing `ticts-0.4.0/ticts/timeseries.py` & `ticts-0.5.0/ticts/timeseries.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,75 +1,73 @@
 import logging
 from copy import deepcopy
 
 import pandas as pd
 import pytz
 from sortedcontainers import SortedDict, SortedList
 
-from .io import TictsIOMixin
-from .iplot import TictsPlot
-from .operation import TictsOperationMixin
-from .pandas_mixin import PandasMixin
-from .utils import MAXTS, MINTS, NO_DEFAULT, timestamp_converter
+from ticts.io import TictsIOMixin
+from ticts.iplot import TictsPlot
+from ticts.operation import TictsOperationMixin
+from ticts.pandas_mixin import PandasMixin
+from ticts.utils import MAXTS, MINTS, NO_DEFAULT, timestamp_converter
 
 logger = logging.getLogger(__name__)
 
-DEFAULT_NAME = 'value'
+DEFAULT_NAME = "value"
 
 
 def _process_args(data, tz):
     if data is None:
         data = []
     if isinstance(data, (list, tuple, set)) and len(data) == 1:
         data = data[0]
 
     if isinstance(data, pd.DataFrame):
         # We should already have checked len(df.columns) == 1
         data = data.to_dict()[data.columns[0]]
     elif isinstance(data, pd.Series):
         data = data.to_dict()
 
-    if hasattr(data, 'items'):
+    if hasattr(data, "items"):
         data = data.items()
 
     return ((timestamp_converter(k, tz), v) for k, v in data)
 
 
 class TictsMagicMixin:
     def __copy__(self):
         return self.__class__(self)
 
     def __deepcopy__(self, memo):
-        return self.__class__(
-            data=deepcopy(self.data), **self._kwargs_special_keys)
+        return self.__class__(data=deepcopy(self.data), **self._kwargs_special_keys)
 
     def __repr__(self):
         header = "<TimeSeries>"
 
         meta = []
         if self._has_default:
-            meta.append('default={}'.format(self.default))
+            meta.append(f"default={self.default}")
         if self.name != DEFAULT_NAME:
-            meta.append("name='{}'".format(self.name))
+            meta.append(f"name='{self.name}'")
 
         if meta:
-            header = "{} ({})".format(header, ' | '.join(meta))
+            header = "{} ({})".format(header, " | ".join(meta))
 
         def generate_content(keys):
-            return '\n'.join(
-                ["{}: {},".format(key.isoformat(), self[key]) for key in keys])
+            return "\n".join([f"{key.isoformat()}: {self[key]}," for key in keys])
 
         if len(self) < 10:
             content = generate_content(self.index)
         else:
             content_head = generate_content(self.index[:5])
             content_tail = generate_content(self.index[-5:])
-            content = "{}\n[...]\n{}".format(content_head, content_tail)
+            content = f"{content_head}\n[...]\n{content_tail}"
 
-        return "{}\n{}".format(header, content)
+        return f"{header}\n{content}"
 
     # Methods redirecting to SortedDict data attribute method
     def __len__(self):
         return len(self.data)
 
     def __iter__(self):
         return self.data.__iter__()
@@ -110,27 +108,29 @@
 
             else:
                 new_args = args
 
         self.data.update(*new_args, **kwargs)
 
 
-class TimeSeries(TictsMagicMixin, TictsOperationMixin, PandasMixin,
-                 TictsIOMixin, TictsPlot):
-    """ TimeSeries object.
+class TimeSeries(
+    TictsMagicMixin, TictsOperationMixin, PandasMixin, TictsIOMixin, TictsPlot
+):
+    """TimeSeries object.
 
     Args:
         default: The default value of timeseries.
         permissive (bool): Whether to allow accessing non-existing values or not.
             If is True, getting non existing item returns None.
             If is False, getting non existing item raises.
     """
+
     _default_interpolate = "previous"
 
-    _meta_keys = ('default', 'name', 'permissive')
+    _meta_keys = ("default", "name", "permissive")
 
     @property
     def index(self):
         return self.data.keys()
 
     @property
     def lower_bound(self):
@@ -158,56 +158,60 @@
         return kwargs
 
     @property
     def empty(self):
         """Return whether the TimeSeries is empty or not."""
         return len(self) == 0
 
-    def __init__(self,
-                 data=None,
-                 default=NO_DEFAULT,
-                 name=DEFAULT_NAME,
-                 permissive=True,
-                 tz='UTC'):
+    def __init__(
+        self,
+        data=None,
+        default=NO_DEFAULT,
+        name=DEFAULT_NAME,
+        permissive=True,
+        tz="UTC",
+    ):
         """"""
         if isinstance(data, self.__class__):
-            for attr in ('data', *self._meta_keys):
+            for attr in ("data", *self._meta_keys):
                 setattr(self, attr, getattr(data, attr))
 
             # Only set 'default' and 'name' if is different from default
             if default != NO_DEFAULT:
-                setattr(self, 'default', default)
+                setattr(self, "default", default)
             if name != DEFAULT_NAME:
-                setattr(self, 'name', name)
+                setattr(self, "name", name)
             return
 
-        if hasattr(default, 'lower') and default.lower() == 'no_default':
+        if hasattr(default, "lower") and default.lower() == "no_default":
             # 'no_default' as string is used at JSON serealization time
             self.default = NO_DEFAULT
         else:
             self.default = default
 
         self.name = name
         self.permissive = permissive
 
         # Overwrite the name if data is an instance of pd.DataFrame or pd.Series
         if isinstance(data, pd.DataFrame):
             if len(data.columns) != 1:
-                msg = ("Can't convert a DataFrame with several columns into "
-                       "one timeseries: {}.")
+                msg = (
+                    "Can't convert a DataFrame with several columns into "
+                    "one timeseries: {}."
+                )
                 raise ValueError(msg.format(data.columns))
             self.name = data.columns[0]
 
         elif isinstance(data, pd.Series):
             self.name = data.name
 
         try:
             tz = pytz.timezone(tz)
-        except pytz.UnknownTimeZoneError:
-            raise ValueError('{} is not a valid timezone'.format(tz))
+        except pytz.UnknownTimeZoneError as err:
+            raise ValueError(f"{tz} is not a valid timezone") from err
 
         # SortedDict.__init__ does not use the __setitem__
         # Hence we got to parse datetime keys ourselves.
         # SortedDict use the first arg given and check if is a callable
         # in case you want to give your custom sorting function.
         self.data = SortedDict(None, _process_args(data, tz))
 
@@ -236,24 +240,23 @@
                 raise KeyError
 
         if isinstance(key, slice):
             return self.slice(key.start, key.stop)
 
         key = timestamp_converter(key, self.tz)
 
-        basemsg = "Getting {} but default attribute is not set".format(key)
+        basemsg = f"Getting {key} but default attribute is not set"
         if self.empty:
             if self._has_default:
                 return self.default
             else:
                 if self.permissive:
                     return
                 else:
-                    raise KeyError(
-                        "{} and timeseries is empty".format(basemsg))
+                    raise KeyError(f"{basemsg} and timeseries is empty")
 
         if key < self.lower_bound:
             if self._has_default:
                 return self.default
             else:
                 if self.permissive:
                     return
@@ -266,15 +269,15 @@
             return self.data[key]
 
         if interpolate.lower() == "previous":
             fn = self._get_previous
         elif interpolate.lower() == "linear":
             fn = self._get_linear_interpolate
         else:
-            raise ValueError("'{}' interpolation unknown.".format(interpolate))
+            raise ValueError(f"'{interpolate}' interpolation unknown.")
 
         return fn(key)
 
     def _get_previous(self, time):
         # In this case, bisect_left == bisect_right == bisect
         # And idx > 0 as we already handled other cases
         previous_idx = self.data.bisect(time) - 1
@@ -293,21 +296,20 @@
             return self.data[previous_time_idx]
 
         next_time_idx = self.index[idx]
 
         previous_value = self.data[previous_time_idx]
         next_value = self.data[next_time_idx]
 
-        coeff = (time - previous_time_idx) / (
-            next_time_idx - previous_time_idx)
+        coeff = (time - previous_time_idx) / (next_time_idx - previous_time_idx)
 
         value = previous_value + coeff * (next_value - previous_value)
         return value
 
-    def slice(self, start, end):  # noqa A003
+    def slice(self, start, end):  # A003
         """Slice your timeseries for give interval.
 
         Args:
             start (datetime or str): lower bound
             end (datetime or str): upper bound
 
         Returns:
@@ -317,16 +319,15 @@
         end = timestamp_converter(end, self.tz)
 
         newts = TimeSeries(**self._kwargs_special_keys)
 
         for key in self.data.irange(start, end, inclusive=(True, False)):
             newts[key] = self[key]
 
-        should_add_left_closure = (start not in newts.index
-                                   and start >= self.lower_bound)
+        should_add_left_closure = start not in newts.index and start >= self.lower_bound
         if should_add_left_closure:
             newts[start] = self[start]  # is applying get_previous on self
 
         return newts
 
     def set_interval(self, start, end, value):
         """Set a value for an interval of time.
@@ -391,16 +392,17 @@
             next_key = lst_keys[i + 1]
             if next_key > end:  # stop there
                 return
             yield key, next_key
 
     def equals(self, other, check_default=True, check_name=True):
         if not isinstance(other, self.__class__):
-            raise TypeError("Can't compare {} with {}".format(
-                self.__class__.__name__, other.__class__.__name__))
+            raise TypeError(
+                f"Can't compare {self.__class__.__name__} with {other.__class__.__name__}"
+            )
 
         is_equal = self.data == other.data
 
         if check_default:
             is_equal = is_equal and self.default == other.default
 
         if check_name:
@@ -413,16 +415,16 @@
         if self.empty:
             return pytz.UTC
         return str(self.index[0].tz)
 
     def tz_convert(self, tz):
         try:
             tz = pytz.timezone(tz)
-        except pytz.UnknownTimeZoneError:
-            raise ValueError('{} is not a valid timezone'.format(tz))
+        except pytz.UnknownTimeZoneError as err:
+            raise ValueError(f"{tz} is not a valid timezone") from err
 
         ts = deepcopy(self)
 
         for key in ts.index:
             ts[key.tz_convert(tz)] = ts.data.pop(key)
 
         return ts
```

