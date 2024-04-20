# Comparing `tmp/lm_checkpoints-0.1.8.tar.gz` & `tmp/lm_checkpoints-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lm_checkpoints-0.1.8.tar", max compression
+gzip compressed data, was "lm_checkpoints-0.1.9.tar", max compression
```

## Comparing `lm_checkpoints-0.1.8.tar` & `lm_checkpoints-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-11-09 13:42:10.546502 lm_checkpoints-0.1.8/LICENSE
--rw-r--r--   0        0        0      878 2023-11-09 14:04:49.371901 lm_checkpoints-0.1.8/README.md
--rw-r--r--   0        0        0      140 2023-11-09 13:50:58.666038 lm_checkpoints-0.1.8/lm_checkpoints/__init__.py
--rw-r--r--   0        0        0     4340 2023-11-09 15:45:55.532074 lm_checkpoints-0.1.8/lm_checkpoints/checkpoints.py
--rw-r--r--   0        0        0     3482 2023-11-09 15:46:04.020594 lm_checkpoints-0.1.8/lm_checkpoints/multiberts.py
--rw-r--r--   0        0        0     3385 2023-11-09 15:46:10.145864 lm_checkpoints-0.1.8/lm_checkpoints/pythia.py
--rw-r--r--   0        0        0       36 2023-11-09 15:31:06.136661 lm_checkpoints-0.1.8/lm_checkpoints/testing/__init__.py
--rw-r--r--   0        0        0      750 2023-11-09 15:27:40.066997 lm_checkpoints-0.1.8/lm_checkpoints/testing/decorators.py
--rw-r--r--   0        0        0      522 2023-11-09 15:50:27.676122 lm_checkpoints-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1652 1970-01-01 00:00:00.000000 lm_checkpoints-0.1.8/setup.py
--rw-r--r--   0        0        0     1520 1970-01-01 00:00:00.000000 lm_checkpoints-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-11-09 13:42:10.546502 lm_checkpoints-0.1.9/LICENSE
+-rw-r--r--   0        0        0      878 2023-11-09 14:04:49.371901 lm_checkpoints-0.1.9/README.md
+-rw-r--r--   0        0        0      140 2023-11-09 13:50:58.666038 lm_checkpoints-0.1.9/lm_checkpoints/__init__.py
+-rw-r--r--   0        0        0     4360 2023-11-14 09:09:55.459852 lm_checkpoints-0.1.9/lm_checkpoints/checkpoints.py
+-rw-r--r--   0        0        0     3546 2023-11-14 09:11:01.932078 lm_checkpoints-0.1.9/lm_checkpoints/multiberts.py
+-rw-r--r--   0        0        0     3415 2023-11-14 09:10:37.808486 lm_checkpoints-0.1.9/lm_checkpoints/pythia.py
+-rw-r--r--   0        0        0       37 2023-11-09 15:51:46.591334 lm_checkpoints-0.1.9/lm_checkpoints/testing/__init__.py
+-rw-r--r--   0        0        0      752 2023-11-09 15:51:46.596037 lm_checkpoints-0.1.9/lm_checkpoints/testing/decorators.py
+-rw-r--r--   0        0        0      560 2023-11-14 09:13:29.046037 lm_checkpoints-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1661 1970-01-01 00:00:00.000000 lm_checkpoints-0.1.9/setup.py
+-rw-r--r--   0        0        0     1579 1970-01-01 00:00:00.000000 lm_checkpoints-0.1.9/PKG-INFO
```

### Comparing `lm_checkpoints-0.1.8/LICENSE` & `lm_checkpoints-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lm_checkpoints-0.1.8/README.md` & `lm_checkpoints-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `lm_checkpoints-0.1.8/lm_checkpoints/checkpoints.py` & `lm_checkpoints-0.1.9/lm_checkpoints/checkpoints.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from abc import ABC, abstractmethod
 from itertools import product
 import torch
 from pathlib import Path
 import numpy as np
+from typing import List, Dict, Union
 
 
-def records_to_list(list_of_dicts: list[dict[str, int]] | dict[str, int]):
+def records_to_list(list_of_dicts: Union[List[Dict[str, int]], Dict[str, int]]):
     """Transform a list of dictionaries to a dictionary of lists.
     If list_of_dicts is a dictionary, it will simply make a list of each values.
     From: https://stackoverflow.com/questions/5558418/list-of-dicts-to-from-dict-of-lists
 
     Args:
         list_of_dicts (list[dict[str, int]] | dict[str, int]): List of dictionaries, assuming each dictionary has the same keys.
 
@@ -42,20 +43,17 @@
     I = lambda i: int(round(i))
     return [L[I(size * i) : I(size * (i + 1))] for i in range(n)]
 
 
 class AbstractCheckpoints(ABC):
     """Abstract class for iterating over model checkpoints"""
 
-    def __init__(
-        self,
-        device="cpu"
-    ):
+    def __init__(self, device: str = "cpu"):
         self.low_cpu_mem_usage = True if device == "cpu" else False
-        
+
         self._device = device
         if device == "cpu":
             self.device = torch.device("cpu")
         elif device == "cuda":
             self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
         elif device == "mps":
             self.device = torch.device(
```

### Comparing `lm_checkpoints-0.1.8/lm_checkpoints/multiberts.py` & `lm_checkpoints-0.1.9/lm_checkpoints/multiberts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from lm_checkpoints import AbstractCheckpoints, Checkpoint
 from transformers import AutoConfig, AutoTokenizer, AutoModelForMaskedLM
 from itertools import product
+from typing import List, Dict
 
 
 class MultiBERTCheckpoints(AbstractCheckpoints):
     """Class for iterating over MultiBERT checkpoints"""
 
     def __init__(self, step=None, seed=None, **kwargs):
         """Initialize the MultiBERTCheckpoints.
@@ -86,15 +87,15 @@
 
         Returns:
             str: Name of the checkpoint on HF.
         """
         return f"google/multiberts-seed_{seed}-step_{step}k"
 
     @property
-    def checkpoints(self) -> list[dict[str, int]]:
+    def checkpoints(self) -> List[Dict[str, int]]:
         """Returns all step and seed combinations that make up the checkpoints.
 
         Returns:
             list[dict[str, int]]: List of dicts (seed, step) describing each checkpoint.
         """
         return list(
             {"seed": p[0], "step": p[1]} for p in product(self.seeds, self.steps)
@@ -106,15 +107,18 @@
     def get_checkpoint(self, seed, step) -> Checkpoint:
         model_name = self.get_model_name(step, seed)
         config = AutoConfig.from_pretrained(model_name)
 
         # Necessary here?
         config.output_scores = True
 
-        tokenizer = AutoTokenizer.from_pretrained(model_name, device=self.device,)
+        tokenizer = AutoTokenizer.from_pretrained(
+            model_name,
+            device=self.device,
+        )
 
         model = AutoModelForMaskedLM.from_pretrained(
             model_name,
             config=config,
             low_cpu_mem_usage=self.low_cpu_mem_usage,  # https://huggingface.co/docs/transformers/main_classes/model#large-model-loading
         )
         model.eval()
```

### Comparing `lm_checkpoints-0.1.8/lm_checkpoints/pythia.py` & `lm_checkpoints-0.1.9/lm_checkpoints/pythia.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from lm_checkpoints import AbstractCheckpoints, Checkpoint
 from itertools import product
 from transformers import AutoTokenizer, GPTNeoXForCausalLM
+from typing import List, Dict
 
 
 class PythiaCheckpoints(AbstractCheckpoints):
     """Class for iterating over Pythia checkpoints"""
 
     def __init__(
         self,
         size: int = 70,
-        step: list[int] = None,
-        seed: list[int] = None,
+        step: List[int] = None,
+        seed: List[int] = None,
         deduped: bool = False,
         **kwargs,
     ) -> None:
         """Initialize the PythiaCheckpoints.
 
         Args:
             size (int): Model size. Defaults to 70.
@@ -74,15 +75,15 @@
         """
         if seed == 0:
             return f"EleutherAI/pythia-{self.size}m"
         else:
             return f"EleutherAI/pythia-{self.size}m-seed{seed}"
 
     @property
-    def checkpoints(self) -> list[dict[str, int]]:
+    def checkpoints(self) -> List[Dict[str, int]]:
         """Returns all step and seed combinations that make up the checkpoints.
 
         Returns:
             list[dict[str, int]]: List of dicts (seed, step) describing each checkpoint.
         """
         return list(
             {"seed": p[0], "step": p[1]} for p in product(self.seeds, self.steps)
```

### Comparing `lm_checkpoints-0.1.8/lm_checkpoints/testing/decorators.py` & `lm_checkpoints-0.1.9/lm_checkpoints/testing/decorators.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 
 _available_devices = ["cpu"]
 if torch.cuda.is_available():
     _available_devices.append("cuda:0")
 if torch.backends.mps.is_available():
     _available_devices.append("mps")
 
+
 def multi_device(test_method):
     """
     Adapted from AllenNLP.
 
     Decorator that provides an argument `device` of type `str` to a test function.
 
     If you have a CUDA capable GPU available, device will be "cuda:0", otherwise the device will
     be "cpu".
 
     !!! Note
         If you have a CUDA capable GPU available, but you want to run the test using CPU only,
         just set the environment variable "CUDA_CAPABLE_DEVICES=''" before running pytest.
     """
-    return pytest.mark.parametrize("device", _available_devices)(test_method)
+    return pytest.mark.parametrize("device", _available_devices)(test_method)
```

### Comparing `lm_checkpoints-0.1.8/setup.py` & `lm_checkpoints-0.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 ['lm_checkpoints', 'lm_checkpoints.testing']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['accelerate>=0.24.1,<0.25.0',
- 'torch>=2.1.0,<3.0.0',
+ 'torch>=2.0.0,!=2.0.1,!=2.1.0',
  'transformers>=4.35.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'lm-checkpoints',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Simple library for loading checkpoints of language models.',
     'long_description': '# lm-checkpoints\nSimple library for dealing with language model checkpoints.\n\nInstall using `pip install lm-checkpoints`.\n\n## Example\nSay you want to compute some metrics for all model checkpoints of Pythia 160m, but only seed 0.\n\n```\nfrom lm_checkpoints import PythiaCheckpoints\n\nfor ckpt in PythiaCheckpoints(size=160,seed=[0]):\n    # Do something with ckpt.model or ckpt.tokenizer\n```\n\nOr if you only want to load steps `0, 1, 2, 4, 8, 16` for all available seeds:\n```\nfrom lm_checkpoints import PythiaCheckpoints\n\nfor ckpt in PythiaCheckpoints(size=160,step=[0, 1, 2, 4, 8, 16]):\n    # Do something with ckpt.model or ckpt.tokenizer\n```\n\nAlternatively, you may want to load all final checkpoints of MultiBERTs:\n```\nfrom lm_checkpoints import MultiBERTCheckpoints\n\nfor ckpt in MultiBERTCheckpoints.final_checkpoints():\n    # Do something with ckpt.model or ckpt.tokenizer\n```',
     'author': 'Oskar van der Wal',
     'author_email': 'odw@duck.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `lm_checkpoints-0.1.8/PKG-INFO` & `lm_checkpoints-0.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: lm-checkpoints
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simple library for loading checkpoints of language models.
 License: MIT
 Author: Oskar van der Wal
 Author-email: odw@duck.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: accelerate (>=0.24.1,<0.25.0)
-Requires-Dist: torch (>=2.1.0,<3.0.0)
+Requires-Dist: torch (>=2.0.0,!=2.0.1,!=2.1.0)
 Requires-Dist: transformers (>=4.35.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # lm-checkpoints
 Simple library for dealing with language model checkpoints.
 
 Install using `pip install lm-checkpoints`.
```

