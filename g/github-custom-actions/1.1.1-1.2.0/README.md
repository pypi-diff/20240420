# Comparing `tmp/github_custom_actions-1.1.1.tar.gz` & `tmp/github_custom_actions-1.2.0.tar.gz`

## Comparing `github_custom_actions-1.1.1.tar` & `github_custom_actions-1.2.0.tar`

### file list

```diff
@@ -1,47 +1,54 @@
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/.coveragerc
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/.flake8
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/.mypy.ini
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/.pylintrc
--rwxr-xr-x   0        0        0     1339 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/activate.sh
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/invoke.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/pytest.ini
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/requirements.dev.in
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/requirements.dev.txt
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/requirements.in
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/requirements.txt
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/tasks.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/.github/workflows/pip_publish.yml
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/.github/workflows/static.yml
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/docs/mkdocs.yml
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/docs/src/en/index.md
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/docs/src/en/quick_start.md
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/docs/src/en/reference.md
--rw-r--r--   0        0        0   302032 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/docs/src/en/images/var_ide_hover_docstring.jpg
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/docs/src/ru/index.md
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/docs/src/ru/quick_start.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/scripts/__init__.py
--rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/scripts/build-docs.sh
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/scripts/build.sh
--rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/scripts/docs-render-config.sh
--rwxr-xr-x   0        0        0      243 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/scripts/docstrings.sh
--rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/scripts/include_pyproject_requirements.py
--rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/scripts/upload.sh
--rwxr-xr-x   0        0        0     2522 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/scripts/verup.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/src/github_custom_actions/__about__.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/src/github_custom_actions/__init__.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/src/github_custom_actions/action_base.py
--rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/src/github_custom_actions/github_vars.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/src/github_custom_actions/inputs_outputs.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/tests/conftest.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/tests/test_action_base.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/tests/test_github_custom_actions.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/tests/test_github_vars.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/tests/test_inputs_outputs.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/LICENSE.txt
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/README.md
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 github_custom_actions-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/.coveragerc
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/.flake8
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/.mypy.ini
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/.pylintrc
+-rwxr-xr-x   0        0        0     1339 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/activate.sh
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/invoke.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/pytest.ini
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/requirements.dev.in
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/requirements.dev.txt
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/requirements.in
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/requirements.txt
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/tasks.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/.github/workflows/pip_publish.yml
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/.github/workflows/static.yml
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/docs/mkdocs.yml
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/docs/src/en/github_env_vars.md
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/docs/src/en/index.md
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/docs/src/en/quick_start.md
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/docs/src/en/reference.md
+-rw-r--r--   0        0        0   302032 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/docs/src/en/images/var_ide_hover_docstring.jpg
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/docs/src/ru/github_env_vars.md
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/docs/src/ru/index.md
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/docs/src/ru/quick_start.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/scripts/__init__.py
+-rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/scripts/build.sh
+-rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/scripts/docs-render-config.sh
+-rwxr-xr-x   0        0        0      243 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/scripts/docstrings.sh
+-rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/scripts/include_pyproject_requirements.py
+-rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/scripts/upload.sh
+-rwxr-xr-x   0        0        0     2522 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/scripts/verup.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/src/github_custom_actions/__about__.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/src/github_custom_actions/__init__.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/src/github_custom_actions/action_base.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/src/github_custom_actions/attr_dict_vars.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/src/github_custom_actions/env_attr_dict_vars.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/src/github_custom_actions/file_attr_dict_vars.py
+-rw-r--r--   0        0        0    10652 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/src/github_custom_actions/github_vars.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/src/github_custom_actions/inputs_outputs.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/tests/conftest.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/tests/test_action_base.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/tests/test_env_attr_dict_vars.py
+-rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/tests/test_file_attr_dict_vars.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/tests/test_github_custom_actions.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/tests/test_github_vars.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/tests/test_inputs_outputs.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/README.md
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 github_custom_actions-1.2.0/PKG-INFO
```

### Comparing `github_custom_actions-1.1.1/.pre-commit-config.yaml` & `github_custom_actions-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.1.1/activate.sh` & `github_custom_actions-1.2.0/activate.sh`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.1.1/requirements.dev.txt` & `github_custom_actions-1.2.0/requirements.dev.txt`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.1.1/tasks.py` & `github_custom_actions-1.2.0/tasks.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.1.1/.github/workflows/ci.yml` & `github_custom_actions-1.2.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.1.1/.github/workflows/docs.yml` & `github_custom_actions-1.2.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.1.1/.github/workflows/pip_publish.yml` & `github_custom_actions-1.2.0/.github/workflows/pip_publish.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.1.1/.github/workflows/static.yml` & `github_custom_actions-1.2.0/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.1.1/docs/mkdocs.yml` & `github_custom_actions-1.2.0/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.1.1/docs/src/en/index.md` & `github_custom_actions-1.2.0/docs/src/en/index.md`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.1.1/docs/src/en/quick_start.md` & `github_custom_actions-1.2.0/docs/src/en/quick_start.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,71 @@
 # Quick start
 
-#### Example of usage
+## Example of usage
+
+#### Explicitly defined inputs and outputs
 
 ```python
-from github_custom_actions import ActionBase, ActionInputs
+from github_custom_actions import ActionBase, ActionInputs, ActionOutputs
 
 class MyInputs(ActionInputs):
     my_input: str
     """My input description"""
     
     my_path: Path
     """My path description"""
+    
+    
+class MyOutputs(ActionOutputs):
+    runner_os: str
+    """Runner OS description"""
 
+    
 class MyAction(ActionBase):
     def __init__(self):
-        super().__init__(inputs=MyInputs())
+        super().__init__(inputs=MyInputs(), outputs=MyOutputs())
         if self.inputs.my_path is None:
             raise ValueError("my_path is required")
 
     def main(self):
         self.inputs.my_path.mkdir(exist_ok=True)
-        self.outputs["RUNNER_OS"] = self.vars.runner_os
+        self.outputs.runner_os = self.vars.runner_os
         self.summary.text += (
             self.render(
                 "### {{ inputs.my_input }}.\n"
                 "Have a nice day!"
             )
         )
 
 if __name__ == "__main__":
     MyAction().run()
 ```
+
+#### Simplified version
+
+If you in no mood to scrupulously define your inputs and outputs, you can just use the inputs and outputs as a dict style:
+
+```python
+from github_custom_actions import ActionBase
+
+    
+class MyAction(ActionBase):
+    def __init__(self):
+        super().__init__()
+        if self.inputs.my_path is None:
+            raise ValueError("my_path is required")
+
+    def main(self):
+        self.inputs["my-path"].mkdir(exist_ok=True)
+        self.outputs["runner-os"] = self.vars.runner_os
+        self.summary.text += (
+            self.render(
+                "### {{ inputs.my_input }}.\n"
+                "Have a nice day!"
+            )
+        )
+
+if __name__ == "__main__":
+    MyAction().run()
+```
+
+Of course in this case you will not have the benefits of the type hints and the documentation, so choose the way that you prefer.
```

### Comparing `github_custom_actions-1.1.1/docs/src/en/images/var_ide_hover_docstring.jpg` & `github_custom_actions-1.2.0/docs/src/en/images/var_ide_hover_docstring.jpg`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.1.1/docs/src/ru/index.md` & `github_custom_actions-1.2.0/docs/src/ru/index.md`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.1.1/scripts/include_pyproject_requirements.py` & `github_custom_actions-1.2.0/scripts/include_pyproject_requirements.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.1.1/scripts/verup.sh` & `github_custom_actions-1.2.0/scripts/verup.sh`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.1.1/src/github_custom_actions/action_base.py` & `github_custom_actions-1.2.0/src/github_custom_actions/action_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 import traceback
-from typing import Any
+from typing import Any, Optional
 
 from jinja2 import Template
 
 from github_custom_actions.inputs_outputs import ActionOutputs, ActionInputs
 from github_custom_actions.github_vars import GithubVars
 
 
@@ -36,17 +36,21 @@
 
 class ActionBase:
     """Base class for GitHub Actions.
 
     Implement main() method in the subclass.
     """
 
-    def __init__(self, inputs: ActionInputs = ActionInputs()):
-        self.inputs = inputs
-        self.outputs = ActionOutputs()
+    def __init__(
+        self, inputs: Optional[ActionInputs] = None, outputs: Optional[ActionOutputs] = None
+    ) -> None:
+        # (!) AttrDictVars() works as dict so empty one is False.
+        # This is why we cannot use usual shorthand "or" here
+        self.inputs = inputs if inputs is not None else ActionInputs()
+        self.outputs = outputs if outputs is not None else ActionOutputs()
         self.vars = GithubVars()
 
     summary = FileTextProperty("github_step_summary")
 
     def main(self) -> None:
         """Main method."""
         raise NotImplementedError
```

### Comparing `github_custom_actions-1.1.1/src/github_custom_actions/github_vars.py` & `github_custom_actions-1.2.0/src/github_custom_actions/github_vars.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 
-from github_custom_actions.inputs_outputs import DocumentedEnvVars
+from github_custom_actions.env_attr_dict_vars import EnvAttrDictVars
 
 
-class GithubVars(DocumentedEnvVars):
+class GithubVars(EnvAttrDictVars):
     """GitHub Action environment variables.
 
     https://docs.github.com/en/actions/learn-github-actions/variables#default-environment-variables
 
     Usage:
        class MyAction:
            @property
@@ -21,14 +21,19 @@
     We do not load the attributes on the class init but do it Lazily.
     Once read, the value is stored in the instance dictionary and is not extracted from env anymore.
 
     Only described Github vars are loaded.
     Paths and files have type Path.
     """
 
+    # pylint: disable=abstract-method  # we want RO implementation that raises NotImplementedError on write
+
+    def _attr_to_var_name(self, name: str) -> str:
+        return name  # leave as is
+
     CI: str
     """Always set to true."""
 
     github_action: str
     """The name of the action currently running, or the id of a step.
     For example, for an action, __repo-owner_name-of-action-repo.
     GitHub removes special characters, and uses the name __run when the current step runs a script
```

### Comparing `github_custom_actions-1.1.1/tests/conftest.py` & `github_custom_actions-1.2.0/tests/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from github_custom_actions.inputs_outputs import ActionInputs
+from github_custom_actions.inputs_outputs import ActionInputs, ActionOutputs
 from github_custom_actions.action_base import ActionBase
 import tempfile
 from unittest.mock import patch
 from pathlib import Path
 
 
 @pytest.fixture
@@ -30,10 +30,14 @@
 
 
 class Inputs(ActionInputs):
     my_input: str
     another_input: str
 
 
+class Outputs(ActionOutputs):
+    my_output: str
+
+
 @pytest.fixture(scope="function")
 def action(inputs, outputs):
-    return ActionBase(inputs=Inputs())
+    return ActionBase(inputs=Inputs(), outputs=Outputs())
```

### Comparing `github_custom_actions-1.1.1/tests/test_github_vars.py` & `github_custom_actions-1.2.0/tests/test_github_vars.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.1.1/tests/test_inputs_outputs.py` & `github_custom_actions-1.2.0/tests/test_inputs_outputs.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 
 def test_input_retrieval(action):
     """Test retrieval of input values."""
     assert action.inputs.my_input == "value1"
     assert action.inputs.another_input == "value2"
 
 
-def test_output_set_and_get(inputs, outputs):
+def test_output_set_and_read(action):
     """Test setting and getting output values."""
-    action = ActionBase()
     action.outputs["my_output"] = "output_value"
+    with pytest.raises(AttributeError):
+        action.outputs.my_output2 = "output_value2"
+    action.outputs.my_output = "output_value2"
 
-    assert outputs.read_text() == "my_output=output_value"
+    assert action.vars.github_output.read_text() == "my_output=output_value\nmy-output=output_value2"
 
 
 def test_input_caching(action, monkeypatch):
     """Test that input is loaded from env var only once."""
     monkeypatch.delenv("INPUT_MY-INPUT")
     with pytest.raises(AttributeError):
         assert action.inputs.my_input == "value1"
```

### Comparing `github_custom_actions-1.1.1/LICENSE.txt` & `github_custom_actions-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.1.1/README.md` & `github_custom_actions-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,32 +3,38 @@
 # github-custom-actions
 
 Python package for creating [custom GitHub Actions](https://docs.github.com/en/actions/creating-actions/about-custom-actions). 
 
 #### Example of usage
 
 ```python
-from github_custom_actions import ActionBase, ActionInputs
+from github_custom_actions import ActionBase, ActionInputs, ActionOutputs
 
 class MyInputs(ActionInputs):
     my_input: str
     """My input description"""
     
     my_path: Path
     """My path description"""
+    
+    
+class MyOutputs(ActionOutputs):
+    runner_os: str
+    """Runner OS description"""
 
+    
 class MyAction(ActionBase):
     def __init__(self):
-        super().__init__(inputs=MyInputs())
+        super().__init__(inputs=MyInputs(), outputs=MyOutputs())
         if self.inputs.my_path is None:
             raise ValueError("my_path is required")
 
     def main(self):
         self.inputs.my_path.mkdir(exist_ok=True)
-        self.outputs["RUNNER_OS"] = self.vars.runner_os
+        self.outputs.runner_os = self.vars.runner_os
         self.summary.text += (
             self.render(
                 "### {{ inputs.my_input }}.\n"
                 "Have a nice day!"
             )
         )
```

### Comparing `github_custom_actions-1.1.1/pyproject.toml` & `github_custom_actions-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.1.1/PKG-INFO` & `github_custom_actions-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: github-custom-actions
-Version: 1.1.1
+Version: 1.2.0
 Summary: Python package for creating custom GitHub Actions.
 Project-URL: Homepage, https://andgineer.github.io/github-custom-actions/
 Project-URL: Documentation, https://andgineer.github.io/github-custom-actions/
 Author-email: Andrey Sorokin <andrey@sorokin.engineer>
 License: Copyright (c) 2024 Andrey Sorokin <andrey@sorokin.engineer>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -38,32 +38,38 @@
 # github-custom-actions
 
 Python package for creating [custom GitHub Actions](https://docs.github.com/en/actions/creating-actions/about-custom-actions). 
 
 #### Example of usage
 
 ```python
-from github_custom_actions import ActionBase, ActionInputs
+from github_custom_actions import ActionBase, ActionInputs, ActionOutputs
 
 class MyInputs(ActionInputs):
     my_input: str
     """My input description"""
     
     my_path: Path
     """My path description"""
+    
+    
+class MyOutputs(ActionOutputs):
+    runner_os: str
+    """Runner OS description"""
 
+    
 class MyAction(ActionBase):
     def __init__(self):
-        super().__init__(inputs=MyInputs())
+        super().__init__(inputs=MyInputs(), outputs=MyOutputs())
         if self.inputs.my_path is None:
             raise ValueError("my_path is required")
 
     def main(self):
         self.inputs.my_path.mkdir(exist_ok=True)
-        self.outputs["RUNNER_OS"] = self.vars.runner_os
+        self.outputs.runner_os = self.vars.runner_os
         self.summary.text += (
             self.render(
                 "### {{ inputs.my_input }}.\n"
                 "Have a nice day!"
             )
         )
```

