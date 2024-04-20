# Comparing `tmp/esoc_events-0.0.1.tar.gz` & `tmp/esoc_events-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esoc_events-0.0.1.tar", max compression
+gzip compressed data, was "esoc_events-0.0.2.tar", max compression
```

## Comparing `esoc_events-0.0.1.tar` & `esoc_events-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     2888 2024-02-22 18:14:00.362238 esoc_events-0.0.1/README.md
--rw-r--r--   0        0        0     2177 2024-02-25 18:25:26.934683 esoc_events-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-22 18:14:00.404974 esoc_events-0.0.1/src/esoc_events/__init__.py
--rw-r--r--   0        0        0        0 2024-02-22 18:14:00.406177 esoc_events-0.0.1/src/esoc_events/py.typed
--rw-r--r--   0        0        0        0 2024-02-22 18:15:27.062370 esoc_events-0.0.1/src/esoc_events/utils/__init__.py
--rw-r--r--   0        0        0      232 2024-02-22 20:05:44.657158 esoc_events-0.0.1/src/esoc_events/utils/abstract_parser.py
--rw-r--r--   0        0        0      192 2024-02-23 16:11:13.842859 esoc_events-0.0.1/src/esoc_events/utils/evfm_parser.py
--rw-r--r--   0        0        0      192 2024-02-23 16:10:49.975610 esoc_events-0.0.1/src/esoc_events/utils/evtc_parser.py
--rw-r--r--   0        0        0     1104 2024-02-25 18:25:49.617398 esoc_events-0.0.1/src/esoc_events/utils/fecs_parser.py
--rw-r--r--   0        0        0     1213 2024-02-22 20:08:32.028246 esoc_events-0.0.1/src/esoc_events/utils/plnview_parser.py
--rw-r--r--   0        0        0      867 2024-02-25 18:25:26.934895 esoc_events-0.0.1/src/esoc_events/utils/time.py
--rw-r--r--   0        0        0      192 2024-02-23 16:11:42.350247 esoc_events-0.0.1/src/esoc_events/utils/uevt_parser.py
--rw-r--r--   0        0        0      373 2024-02-25 18:26:45.057090 esoc_events-0.0.1/src/esoc_events/utils/xml.py
--rw-r--r--   0        0        0     3744 1970-01-01 00:00:00.000000 esoc_events-0.0.1/setup.py
--rw-r--r--   0        0        0     4092 1970-01-01 00:00:00.000000 esoc_events-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2888 2024-02-22 18:14:00.362238 esoc_events-0.0.2/README.md
+-rw-r--r--   0        0        0     2177 2024-04-20 18:29:55.032340 esoc_events-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-22 18:14:00.404974 esoc_events-0.0.2/src/esoc_events/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-22 18:14:00.406177 esoc_events-0.0.2/src/esoc_events/py.typed
+-rw-r--r--   0        0        0        0 2024-02-22 18:15:27.062370 esoc_events-0.0.2/src/esoc_events/utils/__init__.py
+-rw-r--r--   0        0        0      232 2024-02-22 20:05:44.657158 esoc_events-0.0.2/src/esoc_events/utils/abstract_parser.py
+-rw-r--r--   0        0        0      192 2024-02-23 16:11:13.842859 esoc_events-0.0.2/src/esoc_events/utils/evfm_parser.py
+-rw-r--r--   0        0        0     1637 2024-04-20 18:51:45.509416 esoc_events-0.0.2/src/esoc_events/utils/evtc_parser.py
+-rw-r--r--   0        0        0     1104 2024-02-25 18:25:49.617398 esoc_events-0.0.2/src/esoc_events/utils/fecs_parser.py
+-rw-r--r--   0        0        0     1341 2024-04-20 18:42:04.567399 esoc_events-0.0.2/src/esoc_events/utils/plnview_parser.py
+-rw-r--r--   0        0        0     1693 2024-04-20 18:57:31.748778 esoc_events-0.0.2/src/esoc_events/utils/time.py
+-rw-r--r--   0        0        0      193 2024-04-20 18:42:01.675808 esoc_events-0.0.2/src/esoc_events/utils/uevt_parser.py
+-rw-r--r--   0        0        0     1829 2024-04-20 19:00:30.505468 esoc_events-0.0.2/src/esoc_events/utils/uevt_writer.py
+-rw-r--r--   0        0        0      603 2024-04-20 18:42:04.562007 esoc_events-0.0.2/src/esoc_events/utils/xml.py
+-rw-r--r--   0        0        0     3744 1970-01-01 00:00:00.000000 esoc_events-0.0.2/setup.py
+-rw-r--r--   0        0        0     4092 1970-01-01 00:00:00.000000 esoc_events-0.0.2/PKG-INFO
```

### Comparing `esoc_events-0.0.1/README.md` & `esoc_events-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `esoc_events-0.0.1/pyproject.toml` & `esoc_events-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "esoc_events"
-version = "0.0.1"
+version = "0.0.2"
 description = "Querying events comming from ESOC sources"
 authors = [
     "Rafael Andres <r.andres.blasco@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `esoc_events-0.0.1/src/esoc_events/utils/fecs_parser.py` & `esoc_events-0.0.2/src/esoc_events/utils/fecs_parser.py`

 * *Files identical despite different names*

### Comparing `esoc_events-0.0.1/src/esoc_events/utils/plnview_parser.py` & `esoc_events-0.0.2/src/esoc_events/utils/plnview_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from typing import Any
 
+from esoc_events.utils.xml import xml_to_obj
+
 from .abstract_parser import AbstractParser
 
 
 class PlnViewParser(AbstractParser):
 
     def __init__(self, path: Any) -> None:
         AbstractParser.__init__(self, path)
         self._all = self.root.findall(".//service_session")
         self.reset()
 
     @property
     def sessions(self) -> list:
-        return self._sessions
+        return [
+            xml_to_obj(session).get("service_session") for session in self._sessions
+        ]
 
     def reset(self) -> Any:
         self._sessions = self._all
         return self
 
     def satellite(self, name: str) -> Any:
         return self.__query__(
```

### Comparing `esoc_events-0.0.1/setup.py` & `esoc_events-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pytest-html>=4.1.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'esoc-events',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'Querying events comming from ESOC sources',
     'long_description': "# esoc_events\n\n[![PyPI](https://img.shields.io/pypi/v/esoc_events?style=flat-square)](https://pypi.python.org/pypi/esoc_events/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/esoc_events?style=flat-square)](https://pypi.python.org/pypi/esoc_events/)\n[![PyPI - License](https://img.shields.io/pypi/l/esoc_events?style=flat-square)](https://pypi.python.org/pypi/esoc_events/)\n[![Coookiecutter - Wolt](https://img.shields.io/badge/cookiecutter-Wolt-00c2e8?style=flat-square&logo=cookiecutter&logoColor=D4AA00&link=https://github.com/woltapp/wolt-python-package-cookiecutter)](https://github.com/woltapp/wolt-python-package-cookiecutter)\n\n\n---\n\n**Documentation**: [https://r-andres.github.io/esoc_events](https://r-andres.github.io/esoc_events)\n\n**Source Code**: [https://github.com/r-andres/esoc_events](https://github.com/r-andres/esoc_events)\n\n**PyPI**: [https://pypi.org/project/esoc_events/](https://pypi.org/project/esoc_events/)\n\n---\n\nQuerying events comming from ESOC sources\n\n## Installation\n\n```sh\npip install esoc_events\n```\n\n## Development\n\n* Clone this repository\n* Requirements:\n  * [Poetry](https://python-poetry.org/)\n  * Python 3.7+\n* Create a virtual environment and install the dependencies\n\n```sh\npoetry install\n```\n\n* Activate the virtual environment\n\n```sh\npoetry shell\n```\n\n### Testing\n\n```sh\npytest\n```\n\n### Documentation\n\nThe documentation is automatically generated from the content of the [docs directory](./docs) and from the docstrings\n of the public signatures of the source code. The documentation is updated and published as a [Github project page\n ](https://pages.github.com/) automatically as part each release.\n\n### Releasing\n\nTrigger the [Draft release workflow](https://github.com/r-andres/esoc_events/actions/workflows/draft_release.yml)\n(press _Run workflow_). This will update the changelog & version and create a GitHub release which is in _Draft_ state.\n\nFind the draft release from the\n[GitHub releases](https://github.com/r-andres/esoc_events/releases) and publish it. When\n a release is published, it'll trigger [release](https://github.com/r-andres/esoc_events/blob/master/.github/workflows/release.yml) workflow which creates PyPI\n release and deploys updated documentation.\n\n### Pre-commit\n\nPre-commit hooks run all the auto-formatters (e.g. `black`, `isort`), linters (e.g. `mypy`, `flake8`), and other quality\n checks to make sure the changeset is in good shape before a commit/push happens.\n\nYou can install the hooks with (runs for each commit):\n\n```sh\npre-commit install\n```\n\nOr if you want them to run only for each push:\n\n```sh\npre-commit install -t pre-push\n```\n\nOr if you want e.g. want to run all checks manually for all files:\n\n```sh\npre-commit run --all-files\n```\n\n---\n\nThis project was generated using the [wolt-python-package-cookiecutter](https://github.com/woltapp/wolt-python-package-cookiecutter) template.\n",
     'author': 'Rafael Andres',
     'author_email': 'r.andres.blasco@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://r-andres.github.io/esoc_events',
```

### Comparing `esoc_events-0.0.1/PKG-INFO` & `esoc_events-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esoc-events
-Version: 0.0.1
+Version: 0.0.2
 Summary: Querying events comming from ESOC sources
 Home-page: https://r-andres.github.io/esoc_events
 License: MIT
 Author: Rafael Andres
 Author-email: r.andres.blasco@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

