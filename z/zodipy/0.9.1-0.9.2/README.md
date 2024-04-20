# Comparing `tmp/zodipy-0.9.1.tar.gz` & `tmp/zodipy-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodipy-0.9.1.tar", max compression
+gzip compressed data, was "zodipy-0.9.2.tar", max compression
```

## Comparing `zodipy-0.9.1.tar` & `zodipy-0.9.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35148 2022-05-27 12:19:51.135025 zodipy-0.9.1/LICENSE
--rw-r--r--   0        0        0     5979 2024-04-19 07:14:30.048366 zodipy-0.9.1/README.md
--rw-r--r--   0        0        0     2426 2024-04-19 07:43:16.564636 zodipy-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      276 2024-03-21 02:36:07.680358 zodipy-0.9.1/zodipy/__init__.py
--rw-r--r--   0        0        0     2826 2023-02-03 09:26:36.666633 zodipy-0.9.1/zodipy/_bandpass.py
--rw-r--r--   0        0        0      580 2023-02-07 12:46:42.398482 zodipy-0.9.1/zodipy/_constants.py
--rw-r--r--   0        0        0     1677 2023-02-03 09:26:36.669642 zodipy-0.9.1/zodipy/_contour.py
--rw-r--r--   0        0        0     2976 2024-03-21 02:36:07.681352 zodipy-0.9.1/zodipy/_emission.py
--rw-r--r--   0        0        0     4353 2024-03-21 02:36:07.682256 zodipy-0.9.1/zodipy/_interpolate_source.py
--rw-r--r--   0        0        0     4434 2023-02-07 12:46:42.402979 zodipy-0.9.1/zodipy/_ipd_comps.py
--rw-r--r--   0        0        0    15213 2024-04-16 10:58:46.677595 zodipy-0.9.1/zodipy/_ipd_dens_funcs.py
--rw-r--r--   0        0        0     2942 2024-03-21 02:36:07.683943 zodipy-0.9.1/zodipy/_ipd_model.py
--rw-r--r--   0        0        0     3248 2024-02-02 15:01:26.320632 zodipy-0.9.1/zodipy/_line_of_sight.py
--rw-r--r--   0        0        0     2297 2024-03-21 02:36:07.685197 zodipy-0.9.1/zodipy/_sky_coords.py
--rw-r--r--   0        0        0     2752 2024-04-19 07:06:17.490036 zodipy-0.9.1/zodipy/_source_funcs.py
--rw-r--r--   0        0        0      311 2023-02-03 09:26:36.686612 zodipy-0.9.1/zodipy/_types.py
--rw-r--r--   0        0        0      998 2023-02-03 09:26:36.688761 zodipy-0.9.1/zodipy/_unit_vectors.py
--rw-r--r--   0        0        0     3298 2024-03-21 02:36:07.686171 zodipy-0.9.1/zodipy/_validators.py
--rw-r--r--   0        0        0     4667 2023-09-15 08:50:24.694430 zodipy-0.9.1/zodipy/comps.py
--rw-r--r--   0        0        0     1997 2023-09-15 08:50:24.696767 zodipy-0.9.1/zodipy/model_registry.py
--rw-r--r--   0        0        0        0 2022-11-28 11:09:29.298004 zodipy-0.9.1/zodipy/py.typed
--rw-r--r--   0        0        0     6165 2023-09-15 08:50:24.701308 zodipy-0.9.1/zodipy/source_params.py
--rw-r--r--   0        0        0    24080 2024-03-22 13:59:45.674281 zodipy-0.9.1/zodipy/zodipy.py
--rw-r--r--   0        0        0     7143 1970-01-01 00:00:00.000000 zodipy-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    35148 2022-05-27 12:19:51.135025 zodipy-0.9.2/LICENSE
+-rw-r--r--   0        0        0     6085 2024-04-20 14:00:16.424729 zodipy-0.9.2/README.md
+-rw-r--r--   0        0        0     2432 2024-04-20 14:00:12.467509 zodipy-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0      276 2024-03-21 02:36:07.680358 zodipy-0.9.2/zodipy/__init__.py
+-rw-r--r--   0        0        0     2826 2023-02-03 09:26:36.666633 zodipy-0.9.2/zodipy/_bandpass.py
+-rw-r--r--   0        0        0      580 2023-02-07 12:46:42.398482 zodipy-0.9.2/zodipy/_constants.py
+-rw-r--r--   0        0        0     1677 2023-02-03 09:26:36.669642 zodipy-0.9.2/zodipy/_contour.py
+-rw-r--r--   0        0        0     2976 2024-03-21 02:36:07.681352 zodipy-0.9.2/zodipy/_emission.py
+-rw-r--r--   0        0        0     4353 2024-03-21 02:36:07.682256 zodipy-0.9.2/zodipy/_interpolate_source.py
+-rw-r--r--   0        0        0     4434 2023-02-07 12:46:42.402979 zodipy-0.9.2/zodipy/_ipd_comps.py
+-rw-r--r--   0        0        0    15213 2024-04-16 10:58:46.677595 zodipy-0.9.2/zodipy/_ipd_dens_funcs.py
+-rw-r--r--   0        0        0     2942 2024-03-21 02:36:07.683943 zodipy-0.9.2/zodipy/_ipd_model.py
+-rw-r--r--   0        0        0     3248 2024-02-02 15:01:26.320632 zodipy-0.9.2/zodipy/_line_of_sight.py
+-rw-r--r--   0        0        0     2297 2024-03-21 02:36:07.685197 zodipy-0.9.2/zodipy/_sky_coords.py
+-rw-r--r--   0        0        0     2752 2024-04-19 07:06:17.490036 zodipy-0.9.2/zodipy/_source_funcs.py
+-rw-r--r--   0        0        0      311 2023-02-03 09:26:36.686612 zodipy-0.9.2/zodipy/_types.py
+-rw-r--r--   0        0        0      998 2023-02-03 09:26:36.688761 zodipy-0.9.2/zodipy/_unit_vectors.py
+-rw-r--r--   0        0        0     3298 2024-03-21 02:36:07.686171 zodipy-0.9.2/zodipy/_validators.py
+-rw-r--r--   0        0        0     4667 2023-09-15 08:50:24.694430 zodipy-0.9.2/zodipy/comps.py
+-rw-r--r--   0        0        0     1997 2023-09-15 08:50:24.696767 zodipy-0.9.2/zodipy/model_registry.py
+-rw-r--r--   0        0        0        0 2022-11-28 11:09:29.298004 zodipy-0.9.2/zodipy/py.typed
+-rw-r--r--   0        0        0     6165 2023-09-15 08:50:24.701308 zodipy-0.9.2/zodipy/source_params.py
+-rw-r--r--   0        0        0    24080 2024-03-22 13:59:45.674281 zodipy-0.9.2/zodipy/zodipy.py
+-rw-r--r--   0        0        0     7255 1970-01-01 00:00:00.000000 zodipy-0.9.2/PKG-INFO
```

### Comparing `zodipy-0.9.1/LICENSE` & `zodipy-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.1/README.md` & `zodipy-0.9.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,71 +1,72 @@
 
 <img src="docs/img/zodipy_logo.png" width="350">
 
-[![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat-square)](http://www.astropy.org/)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/zodipy?style=flat-square)
-[![PyPI](https://img.shields.io/pypi/v/zodipy.svg?logo=python&style=flat-square)](https://pypi.org/project/zodipy)
-[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://img.shields.io/badge/repo_status-Active-success?style=flat-square)](https://www.repostatus.org/#active)
-[![Actions Status](https://img.shields.io/github/actions/workflow/status/Cosmoglobe/Zodipy/tests.yml?branch=main&logo=github&style=flat-square)](https://github.com/Cosmoglobe/Zodipy/actions)
+[![astropy](https://img.shields.io/badge/powered%20by-AstroPy-orange.svg)](http://www.astropy.org/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/zodipy)
+[![PyPI](https://img.shields.io/pypi/v/zodipy.svg?logo=python)](https://pypi.org/project/zodipy)
+[![Actions Status](https://img.shields.io/github/actions/workflow/status/Cosmoglobe/Zodipy/tests.yml?branch=main&logo=github)](https://github.com/Cosmoglobe/Zodipy/actions)
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/Cosmoglobe/zodipy/mkdocs-deploy.yml?branch=main&style=flat-square&logo=github&label=docs)
-[![Codecov](https://img.shields.io/codecov/c/github/Cosmoglobe/zodipy?token=VZP9L79EUJ&style=flat-square&logo=codecov)](https://app.codecov.io/gh/Cosmoglobe/zodipy)
-[![arXiv Paper](https://img.shields.io/badge/arXiv-2205.12962-green?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2205.12962)
-[![ascl:2306.012](https://img.shields.io/badge/ascl-2306.012-blue.svg?colorB=262255&style=flat-square)](https://ascl.net/2306.012)
+[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://img.shields.io/badge/repo_status-Active-success)](https://www.repostatus.org/#active)
+[![Codecov](https://img.shields.io/codecov/c/github/Cosmoglobe/zodipy?token=VZP9L79EUJ&logo=codecov)](https://app.codecov.io/gh/Cosmoglobe/zodipy)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![pyOpenSci](https://tinyurl.com/y22nb8up)](https://github.com/pyOpenSci/software-review/issues/161)
+[![ascl:2306.012](https://img.shields.io/badge/ascl-2306.012-blue.svg?colorB=262255)](https://ascl.net/2306.012)
+[![DOI](https://zenodo.org/badge/394929213.svg)](https://zenodo.org/doi/10.5281/zenodo.10999611)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.06648/status.svg)](https://doi.org/10.21105/joss.06648)
 ---
 
 
 ZodiPy is an [Astropy affiliated](https://www.astropy.org/affiliated/) package for simulating zodiacal light in intensity for arbitrary Solar system observers.
 
 ![plot](docs/img/zodipy_map.png)
 
-# Help
+## Documentation
 See the [documentation](https://cosmoglobe.github.io/zodipy/) for more information and examples on how to use ZodiPy for different applications.
 
-# Installation
-ZodiPy is installed using `pip install zodipy`.
-
-# Dependencies
-ZodiPy supports all Python versions >= 3.9, and has the following dependencies:
-- [Astropy](https://www.astropy.org/) (>=5.0.1)
-- [NumPy](https://numpy.org/)
-- [healpy](https://healpy.readthedocs.io/en/latest/)
-- [jplephem](https://pypi.org/project/jplephem/)
-- [SciPy](https://scipy.org/)
-
-
-# A simple example
+## A simple example
 ```python
 import astropy.units as u
 from astropy.time import Time
 
 from zodipy import Zodipy
 
 
-model = Zodipy("dirbe")
+model = Zodipy(model="dirbe")
 
 emission = model.get_emission_ang(
     25 * u.micron,
     theta=[10, 10.1, 10.2] * u.deg,
     phi=[90, 89, 88] * u.deg,
     obs_time=Time("2022-01-01 12:00:00"),
     obs="earth",
 )
 
 print(emission)
 #> [15.35392831 15.35495051 15.35616009] MJy / sr
 ```
 
-# Scientific paper and citation
-For an overview of the ZodiPy model approach and other information regarding zodiacal emission and interplanetary dust modeling we refer to the scientific paper on ZodiPy:
+## Related scientific papers
+See [CITATION](https://github.com/Cosmoglobe/zodipy/blob/dev/CITATION.bib)
 - [Cosmoglobe: Simulating zodiacal emission with ZodiPy (San et al. 2022)](https://arxiv.org/abs/2205.12962). 
+- [ZodiPy: A Python package for zodiacal light simulations (San 2024)](https://joss.theoj.org/papers/10.21105/joss.06648#). 
+
 
-See [CITATION](https://github.com/Cosmoglobe/zodipy/blob/dev/CITATION.bib) if you have used ZodiPy in your work and want to cite the software.
+## Install
+ZodiPy is installed using `pip install zodipy`.
 
+## Dependencies
+ZodiPy supports all Python versions >= 3.9, and has the following dependencies:
+- [Astropy](https://www.astropy.org/) (>=5.0.1)
+- [NumPy](https://numpy.org/)
+- [healpy](https://healpy.readthedocs.io/en/latest/)
+- [jplephem](https://pypi.org/project/jplephem/)
+- [SciPy](https://scipy.org/)
 
-# For developers
+## For developers
 Contributing developers will need to download the following additional dependencies to test, lint, format and build documentation locally:
 - pytest
 - pytest-cov
 - hypothesis
 - coverage
 - ruff
 - mypy
@@ -76,44 +77,44 @@
 - mkdocs-material
 - mkdocstrings
 - mkdocstrings-python
 - markdown (<3.4.0)
 
 which are required to test and build ZodiPy.
 
-## Poetry
+### Poetry
 Developers can install ZodiPy through [Poetry](https://python-poetry.org/) (Poetry >= 1.8.0) by first cloning or forking the repository, and then running 
 ```
 poetry install
 ```
 in a virtual environment from the repository root. This will read the `pyproject.toml` file in the repository and install all dependencies. 
 
-## pip
+### pip
 Developers not using Poetry can install ZodiPy in a virtual environment with all dependencies by first cloning or forking the repository and then running 
 ```
 pip install -r requirements-dev.txt
 ```
 from the repositry root. This will read and download all the dependencies from the `requirements-dev.txt` file in the repository. 
 
 Note that developers using Python 3.12 will need to upgrade their pip versions with `python3 -m pip install --upgrade pip` before being able to install ZodiPy. This is due to known incompatibilities between older pip versions and Python 3.12
 
-## Tests, linting and formatting
+### Tests, linting and formatting
 The following tools should be run from the root of the repository with no errors. (These are ran automatically as part of the CI workflows on GitHub, but should be tested locally first)
 
 - [pytest](https://docs.pytest.org/en/8.0.x/): Tests are run with pytest by simply running `pytest` in the command line in the root of the repository. 
 - [ruff](https://github.com/astral-sh/ruff): Formating and linting is done with `ruff` by simply running `ruff check` and `ruff format` in the command line in the root of the repository. 
 - [mypy](https://mypy-lang.org/): Type checking is done with `mypy` by simply running `mypy zodipy/` in the root of the repository.
 
 Remeber to add tests when implementing new features to maintain a high code coverage.
 
-## Documentation
+### Documentation
 We use [MkDocs](https://www.mkdocs.org/) to create our documentation. The documentation is built locally with `mkdocs build` from the repository root, and served with `mkdocs serve`.
 
 
-# Funding
+## Funding
 This work has received funding from the European Union's Horizon 2020 research and innovation programme under grant agreements No 776282 (COMPET-4; BeyondPlanck), 772253 (ERC; bits2cosmology) and 819478 (ERC; Cosmoglobe).
 
 
 <div style="display: flex; flex-direction: row; justify-content: space-evenly">
     <img style="width: 49%; height: auto; max-width: 500px; align-self: center" src="https://user-images.githubusercontent.com/28634670/170697040-d5ec2935-29d0-4847-8999-9bc4eaa59e56.jpeg"> 
     &nbsp; 
     <img style="width: 49%; height: auto; max-width: 500px; align-self: center" src="https://user-images.githubusercontent.com/28634670/170697140-b010aa69-9f9a-44c0-b702-8a05ec0b6d3e.jpeg">
```

### Comparing `zodipy-0.9.1/pyproject.toml` & `zodipy-0.9.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "zodipy"
-version = "0.9.1"
-description = "Software for simulating zodiacal emission"
+version = "0.9.2"
+description = "A Python package for zodiacal light simulations"
 authors = ["Metin San <metinisan@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 classifiers = [
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
```

### Comparing `zodipy-0.9.1/zodipy/_bandpass.py` & `zodipy-0.9.2/zodipy/_bandpass.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.1/zodipy/_constants.py` & `zodipy-0.9.2/zodipy/_constants.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.1/zodipy/_contour.py` & `zodipy-0.9.2/zodipy/_contour.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.1/zodipy/_emission.py` & `zodipy-0.9.2/zodipy/_emission.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.1/zodipy/_interpolate_source.py` & `zodipy-0.9.2/zodipy/_interpolate_source.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.1/zodipy/_ipd_comps.py` & `zodipy-0.9.2/zodipy/_ipd_comps.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.1/zodipy/_ipd_dens_funcs.py` & `zodipy-0.9.2/zodipy/_ipd_dens_funcs.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.1/zodipy/_ipd_model.py` & `zodipy-0.9.2/zodipy/_ipd_model.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.1/zodipy/_line_of_sight.py` & `zodipy-0.9.2/zodipy/_line_of_sight.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.1/zodipy/_sky_coords.py` & `zodipy-0.9.2/zodipy/_sky_coords.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.1/zodipy/_source_funcs.py` & `zodipy-0.9.2/zodipy/_source_funcs.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.1/zodipy/_unit_vectors.py` & `zodipy-0.9.2/zodipy/_unit_vectors.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.1/zodipy/_validators.py` & `zodipy-0.9.2/zodipy/_validators.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.1/zodipy/comps.py` & `zodipy-0.9.2/zodipy/comps.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.1/zodipy/model_registry.py` & `zodipy-0.9.2/zodipy/model_registry.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.1/zodipy/source_params.py` & `zodipy-0.9.2/zodipy/source_params.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.1/zodipy/zodipy.py` & `zodipy-0.9.2/zodipy/zodipy.py`

 * *Files identical despite different names*

### Comparing `zodipy-0.9.1/PKG-INFO` & `zodipy-0.9.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: zodipy
-Version: 0.9.1
-Summary: Software for simulating zodiacal emission
+Version: 0.9.2
+Summary: A Python package for zodiacal light simulations
 License: GPL-3.0-or-later
 Keywords: astronomy,astrophysics,cosmology,space,science
 Author: Metin San
 Author-email: metinisan@gmail.com
 Requires-Python: >=3.9
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -25,75 +25,76 @@
 Project-URL: documentation, https://cosmoglobe.github.io/zodipy/
 Project-URL: repository, https://github.com/cosmoglobe/zodipy
 Description-Content-Type: text/markdown
 
 
 <img src="docs/img/zodipy_logo.png" width="350">
 
-[![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat-square)](http://www.astropy.org/)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/zodipy?style=flat-square)
-[![PyPI](https://img.shields.io/pypi/v/zodipy.svg?logo=python&style=flat-square)](https://pypi.org/project/zodipy)
-[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://img.shields.io/badge/repo_status-Active-success?style=flat-square)](https://www.repostatus.org/#active)
-[![Actions Status](https://img.shields.io/github/actions/workflow/status/Cosmoglobe/Zodipy/tests.yml?branch=main&logo=github&style=flat-square)](https://github.com/Cosmoglobe/Zodipy/actions)
+[![astropy](https://img.shields.io/badge/powered%20by-AstroPy-orange.svg)](http://www.astropy.org/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/zodipy)
+[![PyPI](https://img.shields.io/pypi/v/zodipy.svg?logo=python)](https://pypi.org/project/zodipy)
+[![Actions Status](https://img.shields.io/github/actions/workflow/status/Cosmoglobe/Zodipy/tests.yml?branch=main&logo=github)](https://github.com/Cosmoglobe/Zodipy/actions)
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/Cosmoglobe/zodipy/mkdocs-deploy.yml?branch=main&style=flat-square&logo=github&label=docs)
-[![Codecov](https://img.shields.io/codecov/c/github/Cosmoglobe/zodipy?token=VZP9L79EUJ&style=flat-square&logo=codecov)](https://app.codecov.io/gh/Cosmoglobe/zodipy)
-[![arXiv Paper](https://img.shields.io/badge/arXiv-2205.12962-green?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2205.12962)
-[![ascl:2306.012](https://img.shields.io/badge/ascl-2306.012-blue.svg?colorB=262255&style=flat-square)](https://ascl.net/2306.012)
+[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://img.shields.io/badge/repo_status-Active-success)](https://www.repostatus.org/#active)
+[![Codecov](https://img.shields.io/codecov/c/github/Cosmoglobe/zodipy?token=VZP9L79EUJ&logo=codecov)](https://app.codecov.io/gh/Cosmoglobe/zodipy)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![pyOpenSci](https://tinyurl.com/y22nb8up)](https://github.com/pyOpenSci/software-review/issues/161)
+[![ascl:2306.012](https://img.shields.io/badge/ascl-2306.012-blue.svg?colorB=262255)](https://ascl.net/2306.012)
+[![DOI](https://zenodo.org/badge/394929213.svg)](https://zenodo.org/doi/10.5281/zenodo.10999611)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.06648/status.svg)](https://doi.org/10.21105/joss.06648)
 ---
 
 
 ZodiPy is an [Astropy affiliated](https://www.astropy.org/affiliated/) package for simulating zodiacal light in intensity for arbitrary Solar system observers.
 
 ![plot](docs/img/zodipy_map.png)
 
-# Help
+## Documentation
 See the [documentation](https://cosmoglobe.github.io/zodipy/) for more information and examples on how to use ZodiPy for different applications.
 
-# Installation
-ZodiPy is installed using `pip install zodipy`.
-
-# Dependencies
-ZodiPy supports all Python versions >= 3.9, and has the following dependencies:
-- [Astropy](https://www.astropy.org/) (>=5.0.1)
-- [NumPy](https://numpy.org/)
-- [healpy](https://healpy.readthedocs.io/en/latest/)
-- [jplephem](https://pypi.org/project/jplephem/)
-- [SciPy](https://scipy.org/)
-
-
-# A simple example
+## A simple example
 ```python
 import astropy.units as u
 from astropy.time import Time
 
 from zodipy import Zodipy
 
 
-model = Zodipy("dirbe")
+model = Zodipy(model="dirbe")
 
 emission = model.get_emission_ang(
     25 * u.micron,
     theta=[10, 10.1, 10.2] * u.deg,
     phi=[90, 89, 88] * u.deg,
     obs_time=Time("2022-01-01 12:00:00"),
     obs="earth",
 )
 
 print(emission)
 #> [15.35392831 15.35495051 15.35616009] MJy / sr
 ```
 
-# Scientific paper and citation
-For an overview of the ZodiPy model approach and other information regarding zodiacal emission and interplanetary dust modeling we refer to the scientific paper on ZodiPy:
+## Related scientific papers
+See [CITATION](https://github.com/Cosmoglobe/zodipy/blob/dev/CITATION.bib)
 - [Cosmoglobe: Simulating zodiacal emission with ZodiPy (San et al. 2022)](https://arxiv.org/abs/2205.12962). 
+- [ZodiPy: A Python package for zodiacal light simulations (San 2024)](https://joss.theoj.org/papers/10.21105/joss.06648#). 
+
 
-See [CITATION](https://github.com/Cosmoglobe/zodipy/blob/dev/CITATION.bib) if you have used ZodiPy in your work and want to cite the software.
+## Install
+ZodiPy is installed using `pip install zodipy`.
 
+## Dependencies
+ZodiPy supports all Python versions >= 3.9, and has the following dependencies:
+- [Astropy](https://www.astropy.org/) (>=5.0.1)
+- [NumPy](https://numpy.org/)
+- [healpy](https://healpy.readthedocs.io/en/latest/)
+- [jplephem](https://pypi.org/project/jplephem/)
+- [SciPy](https://scipy.org/)
 
-# For developers
+## For developers
 Contributing developers will need to download the following additional dependencies to test, lint, format and build documentation locally:
 - pytest
 - pytest-cov
 - hypothesis
 - coverage
 - ruff
 - mypy
@@ -104,44 +105,44 @@
 - mkdocs-material
 - mkdocstrings
 - mkdocstrings-python
 - markdown (<3.4.0)
 
 which are required to test and build ZodiPy.
 
-## Poetry
+### Poetry
 Developers can install ZodiPy through [Poetry](https://python-poetry.org/) (Poetry >= 1.8.0) by first cloning or forking the repository, and then running 
 ```
 poetry install
 ```
 in a virtual environment from the repository root. This will read the `pyproject.toml` file in the repository and install all dependencies. 
 
-## pip
+### pip
 Developers not using Poetry can install ZodiPy in a virtual environment with all dependencies by first cloning or forking the repository and then running 
 ```
 pip install -r requirements-dev.txt
 ```
 from the repositry root. This will read and download all the dependencies from the `requirements-dev.txt` file in the repository. 
 
 Note that developers using Python 3.12 will need to upgrade their pip versions with `python3 -m pip install --upgrade pip` before being able to install ZodiPy. This is due to known incompatibilities between older pip versions and Python 3.12
 
-## Tests, linting and formatting
+### Tests, linting and formatting
 The following tools should be run from the root of the repository with no errors. (These are ran automatically as part of the CI workflows on GitHub, but should be tested locally first)
 
 - [pytest](https://docs.pytest.org/en/8.0.x/): Tests are run with pytest by simply running `pytest` in the command line in the root of the repository. 
 - [ruff](https://github.com/astral-sh/ruff): Formating and linting is done with `ruff` by simply running `ruff check` and `ruff format` in the command line in the root of the repository. 
 - [mypy](https://mypy-lang.org/): Type checking is done with `mypy` by simply running `mypy zodipy/` in the root of the repository.
 
 Remeber to add tests when implementing new features to maintain a high code coverage.
 
-## Documentation
+### Documentation
 We use [MkDocs](https://www.mkdocs.org/) to create our documentation. The documentation is built locally with `mkdocs build` from the repository root, and served with `mkdocs serve`.
 
 
-# Funding
+## Funding
 This work has received funding from the European Union's Horizon 2020 research and innovation programme under grant agreements No 776282 (COMPET-4; BeyondPlanck), 772253 (ERC; bits2cosmology) and 819478 (ERC; Cosmoglobe).
 
 
 <div style="display: flex; flex-direction: row; justify-content: space-evenly">
     <img style="width: 49%; height: auto; max-width: 500px; align-self: center" src="https://user-images.githubusercontent.com/28634670/170697040-d5ec2935-29d0-4847-8999-9bc4eaa59e56.jpeg"> 
     &nbsp; 
     <img style="width: 49%; height: auto; max-width: 500px; align-self: center" src="https://user-images.githubusercontent.com/28634670/170697140-b010aa69-9f9a-44c0-b702-8a05ec0b6d3e.jpeg">
```

