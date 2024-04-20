# Comparing `tmp/fse_baro-0.0.6.tar.gz` & `tmp/fse_baro-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fse_baro-0.0.6.tar", last modified: Fri Apr 19 07:47:39 2024, max compression
+gzip compressed data, was "fse_baro-0.0.7.tar", last modified: Sat Apr 20 17:13:38 2024, max compression
```

## Comparing `fse_baro-0.0.6.tar` & `fse_baro-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:47:39.974316 fse_baro-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:47:39.970316 fse_baro-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:47:39.970316 fse_baro-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-19 07:47:34.000000 fse_baro-0.0.6/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-19 07:47:34.000000 fse_baro-0.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-19 07:47:34.000000 fse_baro-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-19 07:47:34.000000 fse_baro-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-19 07:47:39.974316 fse_baro-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-19 07:47:34.000000 fse_baro-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:47:39.974316 fse_baro-0.0.6/baro/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 07:47:34.000000 fse_baro-0.0.6/baro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-19 07:47:34.000000 fse_baro-0.0.6/baro/_bocpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-19 07:47:34.000000 fse_baro-0.0.6/baro/anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-19 07:47:34.000000 fse_baro-0.0.6/baro/root_cause_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-19 07:47:34.000000 fse_baro-0.0.6/baro/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:47:39.974316 fse_baro-0.0.6/fse_baro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-19 07:47:39.000000 fse_baro-0.0.6/fse_baro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-19 07:47:39.000000 fse_baro-0.0.6/fse_baro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 07:47:39.000000 fse_baro-0.0.6/fse_baro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 07:47:39.000000 fse_baro-0.0.6/fse_baro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-19 07:47:39.000000 fse_baro-0.0.6/fse_baro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-19 07:47:34.000000 fse_baro-0.0.6/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-19 07:47:34.000000 fse_baro-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 07:47:39.974316 fse_baro-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:47:39.974316 fse_baro-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-19 07:47:34.000000 fse_baro-0.0.6/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:13:38.902778 fse_baro-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:13:38.898778 fse_baro-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:13:38.898778 fse_baro-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-20 17:13:28.000000 fse_baro-0.0.7/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-20 17:13:28.000000 fse_baro-0.0.7/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-20 17:13:28.000000 fse_baro-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-20 17:13:28.000000 fse_baro-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-20 17:13:38.902778 fse_baro-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-20 17:13:28.000000 fse_baro-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:13:38.902778 fse_baro-0.0.7/baro/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-20 17:13:28.000000 fse_baro-0.0.7/baro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-20 17:13:28.000000 fse_baro-0.0.7/baro/_bocpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-20 17:13:28.000000 fse_baro-0.0.7/baro/anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-20 17:13:28.000000 fse_baro-0.0.7/baro/root_cause_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-20 17:13:28.000000 fse_baro-0.0.7/baro/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:13:38.902778 fse_baro-0.0.7/fse_baro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-20 17:13:38.000000 fse_baro-0.0.7/fse_baro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-20 17:13:38.000000 fse_baro-0.0.7/fse_baro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 17:13:38.000000 fse_baro-0.0.7/fse_baro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-20 17:13:38.000000 fse_baro-0.0.7/fse_baro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-20 17:13:38.000000 fse_baro-0.0.7/fse_baro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-20 17:13:28.000000 fse_baro-0.0.7/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-20 17:13:28.000000 fse_baro-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 17:13:38.902778 fse_baro-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:13:38.902778 fse_baro-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-20 17:13:28.000000 fse_baro-0.0.7/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:13:38.902778 fse_baro-0.0.7/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-20 17:13:28.000000 fse_baro-0.0.7/tutorials/reproducibility.ipynb
```

### Comparing `fse_baro-0.0.6/.github/workflows/python-package.yml` & `fse_baro-0.0.7/.github/workflows/build-and-test.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This workflow will install Python dependencies, run tests and lint with a variety of Python versions
 # For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python
 
-name: Python package
+name: Build and test
 
 on:
   push:
     branches: [ "main" ]
   pull_request:
     branches: [ "main" ]
```

### Comparing `fse_baro-0.0.6/.github/workflows/python-publish.yml` & `fse_baro-0.0.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.6/.gitignore` & `fse_baro-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.6/LICENSE` & `fse_baro-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.6/PKG-INFO` & `fse_baro-0.0.7/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fse-baro
-Version: 0.0.6
+Version: 0.0.7
 Summary: BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection
 Author-email: Luan Pham <phamquiluan@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luan Pham
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,61 +21,73 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: Homepage, https://github.com/phamquiluan/baro/
+Project-URL: Issues, https://github.com/phamquiluan/baro/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
 Requires-Dist: pytest
 Requires-Dist: tqdm
 Requires-Dist: requests
 Requires-Dist: matplotlib
 
 # BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection
 
 [![pypi package](https://img.shields.io/pypi/v/fse-baro.svg)](https://pypi.org/project/fse-baro)
-[![Build and test](https://github.com/phamquiluan/baro/actions/workflows/python-package.yml/badge.svg)](https://github.com/phamquiluan/baro/actions/workflows/python-package.yml)
+[![Build and test](https://github.com/phamquiluan/baro/actions/workflows/build-and-test.yml/badge.svg?branch=main)](https://github.com/phamquiluan/baro/actions/workflows/build-and-test.yml)
 
 
 In the progress of preparing the Artifact submission:
 - Deadline 30/4
 - https://2024.esec-fse.org/track/fse-2024-artifacts#submission-for-replicated-and-reproduced-badges
 - Can apply for all three badges: Available, Function, Reusable
 
+**Functional: The artifacts associated with the research are found to be documented, consistent, complete, exercisable, and include appropriate evidence of verification and validation.	
+**
+
+**Reusable: Functional + the artifacts associated with the paper are of a quality that significantly exceeds minimal functionality. They are very carefully documented and well-structured to the extent that reuse and repurposing is facilitated. In particular, norms and standards of the research community for artifacts of this type are strictly adhered to.	
+**
+
 TODO:
 
-- [ ] reproduce RobustScorer
+- [x] reproduce RobustScorer
 - [ ] reproduce BOCPD
+- [ ] make docs directly on readme, show available AD + RCA methods + tutorials
 - [ ] make the API
 - [ ] restructure + lint code
 - [ ] better readme
 - [ ] make a Helm chart
 
 ## Installation
 
-Build from source
+Install from [PyPI](https://pypi.org/project/fse-baro)
 
 ```bash
-git clone https://github.com/phamquiluan/baro.git && cd baro
-pip install -e .
+pip install fse-baro
 ```
 
-Install from [PyPI](https://pypi.org/project/fse-baro)
+Or, build from source
 
 ```bash
-pip install fse-baro
+git clone https://github.com/phamquiluan/baro.git && cd baro
+pip install -e .
 ```
 
 ## How-to-use
 
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1znckFNPny9zU0Rlc9_Q99E6h3hsJq764?usp=sharing)
+
+
 ```python
 from baro import BARO
 
 m = BARO()
 
 anomalies = m.detect_anomalies(data)
 root_causes = m.rca(data, anomalies=anomalies)
```

### Comparing `fse_baro-0.0.6/baro/_bocpd.py` & `fse_baro-0.0.7/baro/_bocpd.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.6/baro/anomaly_detection.py` & `fse_baro-0.0.7/baro/anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.6/baro/root_cause_analysis.py` & `fse_baro-0.0.7/baro/root_cause_analysis.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.6/baro/utility.py` & `fse_baro-0.0.7/baro/utility.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 import requests
+import json
 
 from tqdm import tqdm
 import pandas as pd
 import matplotlib.pyplot as plt
 
+def load_json(filename: str):
+    with open(filename) as f:
+        data = json.load(f)
+    return data
+              
+              
 def drop_constant(df: pd.DataFrame):
     return df.loc[:, (df != df.iloc[0]).any()]
 
 
 def drop_near_constant(df: pd.DataFrame, threshold: float = 0.1):
     return df.loc[:, (df != df.iloc[0]).mean() > threshold]
```

### Comparing `fse_baro-0.0.6/fse_baro.egg-info/PKG-INFO` & `fse_baro-0.0.7/fse_baro.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fse-baro
-Version: 0.0.6
+Version: 0.0.7
 Summary: BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection
 Author-email: Luan Pham <phamquiluan@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luan Pham
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,61 +21,73 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: Homepage, https://github.com/phamquiluan/baro/
+Project-URL: Issues, https://github.com/phamquiluan/baro/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
 Requires-Dist: pytest
 Requires-Dist: tqdm
 Requires-Dist: requests
 Requires-Dist: matplotlib
 
 # BARO: Robust Root Cause Analysis for Microservices via Multivariate Bayesian Online Change Point Detection
 
 [![pypi package](https://img.shields.io/pypi/v/fse-baro.svg)](https://pypi.org/project/fse-baro)
-[![Build and test](https://github.com/phamquiluan/baro/actions/workflows/python-package.yml/badge.svg)](https://github.com/phamquiluan/baro/actions/workflows/python-package.yml)
+[![Build and test](https://github.com/phamquiluan/baro/actions/workflows/build-and-test.yml/badge.svg?branch=main)](https://github.com/phamquiluan/baro/actions/workflows/build-and-test.yml)
 
 
 In the progress of preparing the Artifact submission:
 - Deadline 30/4
 - https://2024.esec-fse.org/track/fse-2024-artifacts#submission-for-replicated-and-reproduced-badges
 - Can apply for all three badges: Available, Function, Reusable
 
+**Functional: The artifacts associated with the research are found to be documented, consistent, complete, exercisable, and include appropriate evidence of verification and validation.	
+**
+
+**Reusable: Functional + the artifacts associated with the paper are of a quality that significantly exceeds minimal functionality. They are very carefully documented and well-structured to the extent that reuse and repurposing is facilitated. In particular, norms and standards of the research community for artifacts of this type are strictly adhered to.	
+**
+
 TODO:
 
-- [ ] reproduce RobustScorer
+- [x] reproduce RobustScorer
 - [ ] reproduce BOCPD
+- [ ] make docs directly on readme, show available AD + RCA methods + tutorials
 - [ ] make the API
 - [ ] restructure + lint code
 - [ ] better readme
 - [ ] make a Helm chart
 
 ## Installation
 
-Build from source
+Install from [PyPI](https://pypi.org/project/fse-baro)
 
 ```bash
-git clone https://github.com/phamquiluan/baro.git && cd baro
-pip install -e .
+pip install fse-baro
 ```
 
-Install from [PyPI](https://pypi.org/project/fse-baro)
+Or, build from source
 
 ```bash
-pip install fse-baro
+git clone https://github.com/phamquiluan/baro.git && cd baro
+pip install -e .
 ```
 
 ## How-to-use
 
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1znckFNPny9zU0Rlc9_Q99E6h3hsJq764?usp=sharing)
+
+
 ```python
 from baro import BARO
 
 m = BARO()
 
 anomalies = m.detect_anomalies(data)
 root_causes = m.rca(data, anomalies=anomalies)
```

### Comparing `fse_baro-0.0.6/main.py` & `fse_baro-0.0.7/main.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.6/pyproject.toml` & `fse_baro-0.0.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -22,14 +22,19 @@
 ]
 dynamic = ["version"]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
+[project.urls]
+Homepage = "https://github.com/phamquiluan/baro/"
+Issues = "https://github.com/phamquiluan/baro/issues"
+
+
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.package-dir]
 baro = "baro"
 
 [tool.setuptools.packages.find]
```

### Comparing `fse_baro-0.0.6/tests/test.py` & `fse_baro-0.0.7/tests/test.py`

 * *Files identical despite different names*

