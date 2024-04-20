# Comparing `tmp/npnn-0.0.2.tar.gz` & `tmp/npnn-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npnn-0.0.2.tar", last modified: Fri Apr 19 10:21:39 2024, max compression
+gzip compressed data, was "npnn-0.0.3.tar", last modified: Fri Apr 19 14:11:27 2024, max compression
```

## Comparing `npnn-0.0.2.tar` & `npnn-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 10:21:39.187020 npnn-0.0.2/
--rw-rw-rw-   0        0        0     1088 2024-04-17 13:52:58.000000 npnn-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     4055 2024-04-19 10:21:39.187020 npnn-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      821 2024-04-19 10:17:57.000000 npnn-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     2038 2024-04-19 10:21:15.000000 npnn-0.0.2/readme.md
--rw-rw-rw-   0        0        0       42 2024-04-19 10:21:39.187020 npnn-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-19 10:21:39.155770 npnn-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-19 10:21:39.171396 npnn-0.0.2/src/npnn/
--rw-rw-rw-   0        0        0      128 2024-04-17 15:10:44.000000 npnn-0.0.2/src/npnn/__init__.py
--rw-rw-rw-   0        0        0     4546 2024-04-17 14:53:17.000000 npnn-0.0.2/src/npnn/autograd.py
--rw-rw-rw-   0        0        0     1361 2024-04-17 11:15:59.000000 npnn-0.0.2/src/npnn/base.py
--rw-rw-rw-   0        0        0     7789 2024-04-17 06:42:46.000000 npnn-0.0.2/src/npnn/functional.py
--rw-rw-rw-   0        0        0     1232 2024-04-17 06:43:02.000000 npnn-0.0.2/src/npnn/nn.py
--rw-rw-rw-   0        0        0     6111 2024-04-19 10:17:48.000000 npnn-0.0.2/src/npnn/optim.py
--rw-rw-rw-   0        0        0     8580 2024-04-17 15:13:03.000000 npnn-0.0.2/src/npnn/test_autograd.py
-drwxrwxrwx   0        0        0        0 2024-04-19 10:21:39.187020 npnn-0.0.2/src/npnn.egg-info/
--rw-rw-rw-   0        0        0     4055 2024-04-19 10:21:39.000000 npnn-0.0.2/src/npnn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2024-04-19 10:21:39.000000 npnn-0.0.2/src/npnn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 10:21:39.000000 npnn-0.0.2/src/npnn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-19 10:21:39.000000 npnn-0.0.2/src/npnn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-19 10:21:39.000000 npnn-0.0.2/src/npnn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:11:27.549761 npnn-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-19 14:11:15.000000 npnn-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-04-19 14:11:27.549761 npnn-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-19 14:11:15.000000 npnn-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-19 14:11:15.000000 npnn-0.0.3/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:11:27.549761 npnn-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:11:27.545761 npnn-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:11:27.549761 npnn-0.0.3/src/npnn/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-19 14:11:15.000000 npnn-0.0.3/src/npnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-19 14:11:15.000000 npnn-0.0.3/src/npnn/autograd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-19 14:11:15.000000 npnn-0.0.3/src/npnn/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-19 14:11:16.000000 npnn-0.0.3/src/npnn/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-19 14:11:16.000000 npnn-0.0.3/src/npnn/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-04-19 14:11:16.000000 npnn-0.0.3/src/npnn/optim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:11:27.549761 npnn-0.0.3/src/npnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-04-19 14:11:27.000000 npnn-0.0.3/src/npnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-19 14:11:27.000000 npnn-0.0.3/src/npnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:11:27.000000 npnn-0.0.3/src/npnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-19 14:11:27.000000 npnn-0.0.3/src/npnn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-19 14:11:27.000000 npnn-0.0.3/src/npnn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:11:27.549761 npnn-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-19 14:11:16.000000 npnn-0.0.3/tests/test_autograd.py
```

### Comparing `npnn-0.0.2/PKG-INFO` & `npnn-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,96 +1,97 @@
-Metadata-Version: 2.1
-Name: npnn
-Version: 0.0.2
-Summary: NumPy Neural Network
-Author-email: Yang Zhang <mail@yangzhang.site>
-License: MIT License
-        
-        Copyright (c) 2024 Yang Zhang
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/AIboy996/npnn
-Keywords: numpy,neural network,machine learning,autograd
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Provides-Extra: cuda11x
-Requires-Dist: cupy-cuda11x; extra == "cuda11x"
-Provides-Extra: cuda12x
-Requires-Dist: cupy-cuda12x; extra == "cuda12x"
-
-# [npnn](https://pypi.org/project/npnn/0.0.1/)
-> NumPy Neural Network
-
-[![PyPI - Version](https://img.shields.io/pypi/v/npnn)](https://pypi.org/project/npnn/0.0.1/)
-![PyPI - Implementation](https://img.shields.io/pypi/implementation/npnn)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/npnn)
-<!-- ![PyPI - Downloads](https://img.shields.io/pypi/dm/npnn) -->
-
-
-## What's npnn?
-> `npnn` is a a **torch-like** Python module for **gradient descent based machine learning** implemented with `numpy`. 
-
-### Dependency
-Basically `npnn` only depends on `numpy`(the latest version 1.26.4 is verified).
-
-If you have CUDA devices available, then you can easily get a acceleration by installing suitable version of `cupy`.  In this case `npnn` will use `cupy` api rather than `numpy` api.
-
-For example, my PC have CUDA v12.x (x86_64), so I use command:
-```bash
-pip install cupy-cuda12x
-pip install npnn
-```
-or in short:
-```bash
-pip install npnn[cuda12x]
-```
-check [cupy documentation](https://docs.cupy.dev/en/stable/install.html#installing-cupy) for more information.
-
-
-### API references
-
-See [npnn WIKI](https://github.com/AIboy996/npnn/wiki).
-
-## Work with npnn!
-> Here we will construct a image classification neural network with npnn.
-
-BTW, this is a course assignment of *DATA620004, School of Data Science, Fudan University*.
-
-### Task
-Construct and Train a neural network on [Fashion-MNIST](https://github.com/zalandoresearch/fashion-mnist) to do image classification.
-
-- Implement gradient backpropagation algorithm by hand,you can use `numpy` but **DO NOT** use `pytorch` or `tensorflow` to do autograd.
-
-- Submit source code including at least four parts: `model definition`, `training`, `parameters searching` and `testing`.
-
-### Implementation
-
-- `dataset.py`: provide Fashion MNIST dataset
-- `model.py`: model definition
-- `train.py`: model training
-- `search.py`: parameters searching
-- `test.py`: model testing
-- `utils.py`: some misc function, such as `save_mode`
+Metadata-Version: 2.1
+Name: npnn
+Version: 0.0.3
+Summary: NumPy Neural Network
+Author-email: Yang Zhang <mail@yangzhang.site>
+License: MIT License
+        
+        Copyright (c) 2024 Yang Zhang
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/AIboy996/npnn
+Keywords: numpy,neural network,machine learning,autograd
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Provides-Extra: cuda11x
+Requires-Dist: cupy-cuda11x; extra == "cuda11x"
+Provides-Extra: cuda12x
+Requires-Dist: cupy-cuda12x; extra == "cuda12x"
+
+# [npnn](https://pypi.org/project/npnn/)
+> NumPy Neural Network
+
+[![PyPI - Version](https://img.shields.io/pypi/v/npnn)](https://pypi.org/project/npnn/)
+![PyPI - Implementation](https://img.shields.io/pypi/implementation/npnn)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/npnn)
+<!-- ![PyPI - Downloads](https://img.shields.io/pypi/dm/npnn) -->
+
+
+## What's npnn?
+> `npnn` is a a **torch-like** Python module for **gradient descent based machine learning** implemented with `numpy`. 
+
+### Dependency
+Basically `npnn` only depends on `numpy`(the latest version 1.26.4 is verified).
+
+If you have CUDA devices available, then you can easily get a acceleration by installing suitable version of `cupy`.  In this case `npnn` will use `cupy` api rather than `numpy` api.
+
+For example, my PC have CUDA v12.x (x86_64), so I use command:
+```bash
+pip install cupy-cuda12x
+pip install npnn
+```
+or in short:
+```bash
+pip install npnn[cuda12x]
+```
+check [cupy documentation](https://docs.cupy.dev/en/stable/install.html#installing-cupy) for more information.
+
+
+### API references
+
+See [npnn WIKI](https://github.com/AIboy996/npnn/wiki).
+
+## Work with npnn!
+> Here we will construct a image classification neural network with npnn.
+
+BTW, this is a course assignment of *DATA620004, School of Data Science, Fudan University*.
+
+### Task
+Construct and Train a neural network on [Fashion-MNIST](https://github.com/zalandoresearch/fashion-mnist) to do image classification.
+
+- Implement gradient backpropagation algorithm by hand,you can use `numpy` but **DO NOT** use `pytorch` or `tensorflow` to do autograd.
+
+- Submit source code including at least four parts: `model definition`, `training`, `parameters searching` and `testing`.
+
+### Implementation
+
+- `dataset.py`: provide Fashion MNIST dataset
+- `model.py`: model definition
+- `train.py`: model training
+- `search.py`: parameters searching
+- `test.py`: model testing
+- `viz.py`: visualization
+- `utils.py`: some misc function, such as `save_model`
```

### Comparing `npnn-0.0.2/readme.md` & `npnn-0.0.3/readme.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,54 @@
-# [npnn](https://pypi.org/project/npnn/0.0.1/)
-> NumPy Neural Network
-
-[![PyPI - Version](https://img.shields.io/pypi/v/npnn)](https://pypi.org/project/npnn/0.0.1/)
-![PyPI - Implementation](https://img.shields.io/pypi/implementation/npnn)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/npnn)
-<!-- ![PyPI - Downloads](https://img.shields.io/pypi/dm/npnn) -->
-
-
-## What's npnn?
-> `npnn` is a a **torch-like** Python module for **gradient descent based machine learning** implemented with `numpy`. 
-
-### Dependency
-Basically `npnn` only depends on `numpy`(the latest version 1.26.4 is verified).
-
-If you have CUDA devices available, then you can easily get a acceleration by installing suitable version of `cupy`.  In this case `npnn` will use `cupy` api rather than `numpy` api.
-
-For example, my PC have CUDA v12.x (x86_64), so I use command:
-```bash
-pip install cupy-cuda12x
-pip install npnn
-```
-or in short:
-```bash
-pip install npnn[cuda12x]
-```
-check [cupy documentation](https://docs.cupy.dev/en/stable/install.html#installing-cupy) for more information.
-
-
-### API references
-
-See [npnn WIKI](https://github.com/AIboy996/npnn/wiki).
-
-## Work with npnn!
-> Here we will construct a image classification neural network with npnn.
-
-BTW, this is a course assignment of *DATA620004, School of Data Science, Fudan University*.
-
-### Task
-Construct and Train a neural network on [Fashion-MNIST](https://github.com/zalandoresearch/fashion-mnist) to do image classification.
-
-- Implement gradient backpropagation algorithm by hand,you can use `numpy` but **DO NOT** use `pytorch` or `tensorflow` to do autograd.
-
-- Submit source code including at least four parts: `model definition`, `training`, `parameters searching` and `testing`.
-
-### Implementation
-
-- `dataset.py`: provide Fashion MNIST dataset
-- `model.py`: model definition
-- `train.py`: model training
-- `search.py`: parameters searching
-- `test.py`: model testing
-- `utils.py`: some misc function, such as `save_mode`
+# [npnn](https://pypi.org/project/npnn/)
+> NumPy Neural Network
+
+[![PyPI - Version](https://img.shields.io/pypi/v/npnn)](https://pypi.org/project/npnn/)
+![PyPI - Implementation](https://img.shields.io/pypi/implementation/npnn)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/npnn)
+<!-- ![PyPI - Downloads](https://img.shields.io/pypi/dm/npnn) -->
+
+
+## What's npnn?
+> `npnn` is a a **torch-like** Python module for **gradient descent based machine learning** implemented with `numpy`. 
+
+### Dependency
+Basically `npnn` only depends on `numpy`(the latest version 1.26.4 is verified).
+
+If you have CUDA devices available, then you can easily get a acceleration by installing suitable version of `cupy`.  In this case `npnn` will use `cupy` api rather than `numpy` api.
+
+For example, my PC have CUDA v12.x (x86_64), so I use command:
+```bash
+pip install cupy-cuda12x
+pip install npnn
+```
+or in short:
+```bash
+pip install npnn[cuda12x]
+```
+check [cupy documentation](https://docs.cupy.dev/en/stable/install.html#installing-cupy) for more information.
+
+
+### API references
+
+See [npnn WIKI](https://github.com/AIboy996/npnn/wiki).
+
+## Work with npnn!
+> Here we will construct a image classification neural network with npnn.
+
+BTW, this is a course assignment of *DATA620004, School of Data Science, Fudan University*.
+
+### Task
+Construct and Train a neural network on [Fashion-MNIST](https://github.com/zalandoresearch/fashion-mnist) to do image classification.
+
+- Implement gradient backpropagation algorithm by hand,you can use `numpy` but **DO NOT** use `pytorch` or `tensorflow` to do autograd.
+
+- Submit source code including at least four parts: `model definition`, `training`, `parameters searching` and `testing`.
+
+### Implementation
+
+- `dataset.py`: provide Fashion MNIST dataset
+- `model.py`: model definition
+- `train.py`: model training
+- `search.py`: parameters searching
+- `test.py`: model testing
+- `viz.py`: visualization
+- `utils.py`: some misc function, such as `save_model`
```

### Comparing `npnn-0.0.2/src/npnn/autograd.py` & `npnn-0.0.3/src/npnn/autograd.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,120 +1,122 @@
-"""
-Autograd algorithm implementation. 
-
-Calcute Tensor's grad by tracking `back_childs` and `back_f`(in fact these two generate a computional tree).
-"""
-
-from .base import Operation, np
-
-
-class Tensor:
-    """Data Container designed for gradient descent based Machine Learning."""
-
-    def __init__(self, arr: np.array, requires_grad: bool = False):
-        """
-        Note that:
-        we always have `self.back_f(*self.back_childs) == self`
-        unless `self.back_f is None`
-        """
-        self.data: np.array = arr
-        self.requires_grad: bool = requires_grad
-        self.back_f: Operation | None = (
-            None  # this indicates root node of the computional graph
-        )
-        self.back_childs: tuple[Tensor] = (self,)  # child nodes
-        if requires_grad:
-            # initialize grad if requires_grad = True
-            self.grad = np.zeros_like(arr)
-        else:
-            self.grad = None
-        self.back_counter = 0
-
-    def backward(self):
-        """
-        Backward Propagation algorithm.
-
-        We only consider:
-        1. input data is Vectors, shape = (m,)
-        2. output metric is Scalars, shape = (1,)
-        3. parameters are Matrices or Vectors, shape = (n,k) or (l,)
-
-        For example: l = MSE(y, u), y = sigmoid(Bh+c), h = sigmoid(Ax+b)
-        where
-        x.shape = (m,)  A.shape = (k,m)  b.shape = (k,)
-        h.shape = (k,)  B.shape = (n,k)  c.shape = (n,)
-        y.shape = (n,)  l.shape = (1,)
-
-        In this case, for i in range(k) for j in range(m) we have gradient:
-
-        (dl / dA) [i,j] = (dl / dy) @ (dy / dh) @ (dh / dA[i,j])
-
-        where each component is 2-d or 1-d array:
-        (dl / dy).shape = (n,)
-        (dy / dh).shape = (n,k)
-        (dh / dA[i,j]).shape = (k,)
-        """
-        assert self.data.shape == (1,), "Only scalars can do backward"
-        for idx, child in enumerate(self.back_childs):
-            if child.back_f is None:  # root node
-                if child.requires_grad:
-                    assert child.ndim <= 2, "Parameters should have ndim <= 2"
-                    # multivariable function, detivate of idx-th variable
-                    child.grad += self.back_f.gradient(self.back_childs, idx)
-                    child.back_counter += 1
-                else:
-                    pass
-            else:
-                child._bp(self.back_f.gradient(self.back_childs, idx))
-
-    def _bp(self, grad: np.ndarray):
-        """private gradient back propagation calculation"""
-        assert grad.ndim <= 2, grad.shape
-        assert self.ndim == 1, f"Only vectors can do _bp, {self.ndim = }"
-        for idx, child in enumerate(self.back_childs):
-            if child.back_f is None:
-                if child.requires_grad:
-                    assert child.ndim <= 2, "parameters should have ndim <= 2"
-                    # parameter is vector
-                    if child.ndim == 1:
-                        child.grad += grad @ self.back_f.gradient(self.back_childs, idx)
-                        child.back_counter += 1
-                    # parameter is matrix
-                    elif child.ndim == 2:
-                        child.grad += np.tensordot(
-                            grad,
-                            self.back_f.gradient(self.back_childs, idx),
-                            axes=(0, 0),
-                        )
-                        child.back_counter += 1
-                else:
-                    pass
-            else:
-                # just like
-                # (dl / dA) [i,j] = (dl / dy) @ (dy / dh) @ (dh / dA[i,j])
-                # we **recursively** propagate gradient
-                child._bp(grad @ self.back_f.gradient(self.back_childs, idx))
-
-    def __getattr__(self, name: str):
-        """
-        When attr not defined, try to find in `self.data`, for example `self.shape` or `self.ndim`
-        """
-        return self.data.__getattribute__(name)
-
-    def __repr__(self) -> str:
-        return f"tensor({self.data}, requires_grad={self.requires_grad}, back_f={self.back_f})"
-
-    def __neg__(self):
-        """This will set requires_grad to False"""
-        t = Tensor(-self.data)
-        t.backf = self.back_f
-        t.back_childs = self.back_childs
-        return t
-
-
-if __name__ == "__main__":
-    from src.functional import *
-
-    x = Tensor(np.random.random((3, 3)), requires_grad=True)
-    y = Norm()(Flatten()(x))
-    y.backward()
-    print(x.grad)
+"""
+Autograd algorithm implementation.
+Calcute Tensor's grad by tracking `back_childs` and `back_f`(in fact these two generate a computional tree).
+"""
+
+from .base import Operation, np
+
+
+class Tensor:
+    """Data Container designed for gradient descent based Machine Learning."""
+
+    def __init__(self, arr: np.array, requires_grad: bool = False):
+        """
+        Note that:
+        we always have `self.back_f(*self.back_childs) == self`
+        unless `self.back_f is None`
+        """
+        self.data: np.array = arr
+        self.requires_grad: bool = requires_grad
+        self.back_f: Operation | None = (
+            None  # this indicates root node of the computional graph
+        )
+        self.back_childs: tuple[Tensor] = (self,)  # child nodes
+        if requires_grad:
+            # initialize grad if requires_grad = True
+            self.grad = np.zeros_like(arr)
+        else:
+            self.grad = None
+        self.back_counter = 0
+
+    def backward(self):
+        """
+        Backward Propagation algorithm.
+
+        We only consider:
+        1. input data is Vectors, shape = (m,)
+        2. output metric is Scalars, shape = (1,)
+        3. parameters are Matrices or Vectors, shape = (n,k) or (l,)
+
+        For example: l = MSE(y, u), y = sigmoid(Bh+c), h = sigmoid(Ax+b)
+        where
+        x.shape = (m,)  A.shape = (k,m)  b.shape = (k,)
+        h.shape = (k,)  B.shape = (n,k)  c.shape = (n,)
+        y.shape = (n,)  l.shape = (1,)
+
+        In this case, for i in range(k) for j in range(m) we have gradient:
+
+        (dl / dA) [i,j] = (dl / dy) @ (dy / dh) @ (dh / dA[i,j])
+
+        where each component is 2-d or 1-d array:
+        (dl / dy).shape = (n,)
+        (dy / dh).shape = (n,k)
+        (dh / dA[i,j]).shape = (k,)
+        """
+        assert self.data.shape == (1,), "Only scalars can do backward"
+        for idx, child in enumerate(self.back_childs):
+            if child.back_f is None:  # root node
+                if child.requires_grad:
+                    assert child.ndim <= 2, "Parameters should have ndim <= 2"
+                    # multivariable function, detivate of idx-th variable
+                    child.grad += self.back_f.gradient(self.back_childs, idx)
+                    child.back_counter += 1
+                else:
+                    pass
+            else:
+                child._bp(self.back_f.gradient(self.back_childs, idx))
+
+    def _bp(self, grad: np.ndarray):
+        """private gradient back propagation calculation"""
+        assert grad.ndim <= 2, grad.shape
+        assert self.ndim == 1, f"Only vectors can do _bp, {self.ndim = }"
+        for idx, child in enumerate(self.back_childs):
+            if child.back_f is None:
+                if child.requires_grad:
+                    assert child.ndim <= 2, "parameters should have ndim <= 2"
+                    # parameter is vector
+                    if child.ndim == 1:
+                        child.grad += grad @ self.back_f.gradient(self.back_childs, idx)
+                        child.back_counter += 1
+                    # parameter is matrix
+                    elif child.ndim == 2:
+                        child.grad += np.tensordot(
+                            grad,
+                            self.back_f.gradient(self.back_childs, idx),
+                            axes=(0, 0),
+                        )
+                        child.back_counter += 1
+                else:
+                    pass
+            else:
+                # just like
+                # (dl / dA) [i,j] = (dl / dy) @ (dy / dh) @ (dh / dA[i,j])
+                # we **recursively** propagate gradient
+                child._bp(grad @ self.back_f.gradient(self.back_childs, idx))
+
+    def __getattr__(self, name: str):
+        """
+        When attr not defined, try to find in `self.data`, for example `self.shape` or `self.ndim`
+        """
+        # without this statement, `self.data` will raise a RecursionError in pickle.loads
+        if name == 'data':
+            return None
+        return self.data.__getattribute__(name)
+
+    def __repr__(self) -> str:
+        return f"tensor({self.data}, requires_grad={self.requires_grad}, back_f={self.back_f})"
+
+    def __neg__(self):
+        """This will set requires_grad to False"""
+        t = Tensor(-self.data)
+        t.backf = self.back_f
+        t.back_childs = self.back_childs
+        return t
+
+
+if __name__ == "__main__":
+    from .functional import Norm, Flatten
+
+    x = Tensor(np.random.random((3, 3)), requires_grad=True)
+    y = Norm()(Flatten()(x))
+    y.backward()
+    print(x.grad)
```

### Comparing `npnn-0.0.2/src/npnn/base.py` & `npnn-0.0.3/src/npnn/base.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-"""Base classes"""
-
-import logging
-logger = logging.getLogger(__name__)
-
-try:
-    import cupy as np
-except ImportError:
-    logger.warning("cupy acceleration is not available.")
-    import numpy as np
-
-
-class Operation:
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def __call__(self, *x):
-        """Forward call"""
-        return self.forward(*x)
-
-    def forward(self):
-        raise NotImplementedError
-
-    def gradient(self) -> np.ndarray:
-        """Gradietn function"""
-        raise NotImplementedError
-
-
-class Module:
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def __call__(self, *x):
-        """Forward call"""
-        return self.forward(*x)
-
-    def parameters(self) -> list:
-        """Return all parameters to be optimized."""
-        raise NotImplementedError
-
-    def __repr__(self) -> str:
-        return f"{self.__class__}"
-
-
-class Optimizer:
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def step(self):
-        """Take a step on gradient direction."""
-        raise NotImplementedError
-
-    def zero_grad(self):
-        """Only should call this if you want to perform mini-batch gradient descent."""
-        for param in self.params:
-            param.grad = np.zeros_like(param.data)
-            param.back_counter = 0
+"""Base classes"""
+
+import logging
+logger = logging.getLogger(__name__)
+
+try:
+    import cupy as np
+except ImportError:
+    logger.warning("cupy acceleration is not available.")
+    import numpy as np
+
+
+class Operation:
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def __call__(self, *x):
+        """Forward call"""
+        return self.forward(*x)
+
+    def forward(self):
+        raise NotImplementedError
+
+    def gradient(self) -> np.ndarray:
+        """Gradietn function"""
+        raise NotImplementedError
+
+
+class Module:
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def __call__(self, *x):
+        """Forward call"""
+        return self.forward(*x)
+
+    def parameters(self) -> list:
+        """Return all parameters to be optimized."""
+        raise NotImplementedError
+
+    def __repr__(self) -> str:
+        return f"{self.__class__}"
+
+
+class Optimizer:
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def step(self):
+        """Take a step on gradient direction."""
+        raise NotImplementedError
+
+    def zero_grad(self):
+        """Only should call this if you want to perform mini-batch gradient descent."""
+        for param in self.params:
+            param.grad = np.zeros_like(param.data)
+            param.back_counter = 0
```

### Comparing `npnn-0.0.2/src/npnn/functional.py` & `npnn-0.0.3/src/npnn/functional.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,293 +1,293 @@
-"""Tensor operation implementation"""
-
-from functools import wraps
-
-from .autograd import Tensor
-from .base import Operation, np
-
-__all__ = [
-    "Add",  # basic oprations
-    "Inner",
-    "Flatten",
-    "Sum",  # loss functions
-    "Norm",
-    "NLL",
-    "Log",  # activation functions
-    "Softmax",
-    "LogSoftmax",
-    "ReLU",
-]
-
-
-def one_hot(x, NUM_CLASS):
-    y = np.zeros((x.size, NUM_CLASS))
-    y[np.arange(x.size), x] = 1
-    return y
-
-
-def singleton(original_cls):
-    """
-    Decorator for basic operations, make them all **singleton**.
-    Otherwise eachtime we do operations, we will eastablish a new object.
-    code refer to https://igeorgiev.eu/python/design-patterns/python-singleton-pattern-decorator/
-    """
-    original_new_method = original_cls.__new__
-    instance = None
-
-    @wraps(original_cls.__new__)
-    def __new__(cls, *args, **kwargs):
-        nonlocal instance
-        if instance is None:
-            instance = original_new_method(cls, *args, **kwargs)
-        return instance
-
-    original_cls.__new__ = __new__
-    return original_cls
-
-
-@singleton
-class Add(Operation):
-    """z = x + y"""
-
-    def forward(self, x: Tensor, y: Tensor) -> Tensor:
-        res = Tensor(x.data + y.data)
-        res.back_f = self
-        res.back_childs = (x, y)
-        return res
-
-    def gradient(self, back_childs: tuple, idx=0) -> np.ndarray:
-        """
-        1. `d(X+Y) / dX = \mathbb{I} \otimes \mathbb{I}` if X is matrix
-        2. `d(x+y) / dx = \mathbb{I}` if x is vector
-        """
-        x = back_childs[idx]
-        assert x.ndim <= 2
-        if x.ndim == 1:
-            return np.eye(*x.shape)
-        else:
-            raise NotImplementedError("No need.")
-
-
-@singleton
-class Inner(Operation):
-    """
-    z = x @ y where z is vector or scalar
-    """
-
-    def forward(self, x: Tensor, y: Tensor) -> Tensor:
-        res = Tensor(x.data @ y.data)
-        assert res.ndim == 1, "result should be vector or scalar"
-        res.back_f = self
-        res.back_childs = (x, y)
-        return res
-
-    def gradient(self, back_childs: tuple, idx=0) -> np.ndarray:
-        """
-        if x is matrix
-        d x@y / dx[i,j] = [0,...,y[j],... ,0], where y[j] is the ith component
-        or in tensor product: `d x@y / dX = c' \otimes \mathbb{I}`
-
-        elif x is vector
-        d x@y / dx = y.T
-        """
-        x, y = back_childs
-        x, y = x.data, y.data
-        if idx == 0:
-            if x.ndim == 1:
-                return y.T
-            else:
-                m, n = x.shape
-                res = np.zeros((m, m, n))
-                res[np.arange(m), np.arange(m), :] = y
-                return res
-        else:
-            if y.ndim == 1:
-                return x
-            else:
-                m, n = y.shape
-                res = np.zeros((n, m, n))
-                res[np.arange(n), :, np.arange(n)] = x
-                return res
-
-
-@singleton
-class Flatten(Operation):
-    """y = x.flatten()"""
-
-    def forward(self, x: Tensor) -> Tensor:
-        res = Tensor(x.data.flatten())
-        res.back_f = self
-        res.back_childs = (x,)
-        return res
-
-    def gradient(self, back_childs: tuple, idx=0) -> np.ndarray:
-        x = back_childs[idx]
-        if x.ndim == 1:
-            return np.eye(*x.shape)
-        else:
-            m, n = x.shape
-            res = np.zeros((m * n, m, n))
-            for i in range(m * n):
-                res[i, i // m, i % n] = 1
-            return res
-
-
-@singleton
-class Sum(Operation):
-    """y = sum(X)"""
-
-    def forward(self, x: Tensor) -> Tensor:
-        res = Tensor(x.data.sum().reshape((1,)))
-        res.back_f = self
-        res.back_childs = (x,)
-        return res
-
-    def gradient(self, back_childs: tuple, idx=0) -> np.ndarray:
-        """Easy"""
-        return np.ones_like(back_childs[idx])
-
-
-@singleton
-class Norm(Operation):
-    """
-    y = sqrt(x.T @ x)
-    """
-
-    def forward(self, x: Tensor) -> Tensor:
-        m = np.abs(x.data).max()
-        a = x.data / m
-        # in my test, arr@arr is faster than np.inner(a,a) and np.dot(a,a)
-        # and np.sqrt(a@a) is faster than np.linalg.norm(a, 2)
-        res = Tensor(m * np.sqrt(a @ a).reshape((1,)))
-        res.back_f = self
-        res.back_childs = (x,)
-        return res
-
-    def gradient(self, back_childs: tuple, idx=0) -> np.ndarray:
-        """
-        `d norm2(x) / dx = x / norm2(x)`
-        """
-        x = back_childs[idx]
-        y = self.forward(x)
-        return x.data / y.data
-
-
-@singleton
-class NLL(Operation):
-    """
-    Negative Log Likelihod
-    l = -sum(x @ y)
-    """
-
-    def forward(self, x: Tensor, y: Tensor) -> Tensor:
-        res = Tensor(-(x.data @ y.data).sum().reshape((1,)))
-        res.back_f = self
-        res.back_childs = (x, y)
-        return res
-
-    def gradient(self, back_childs: tuple, idx=0) -> np.ndarray:
-        """
-        dl / dx = -y, dl / dy = -x
-        """
-        return -back_childs[1 - idx].data
-
-
-@singleton
-class Log(Operation):
-    """
-    y = x.log()
-    """
-
-    def forward(self, x: Tensor) -> Tensor:
-        assert (x.data > 0).all()
-        res = Tensor(np.log(x))
-        res.back_f = self
-        res.back_childs = (x,)
-        return res
-
-    def gradient(self, back_childs: tuple, idx=0) -> np.ndarray:
-        """
-        dy / dx = diag(1/x)
-        """
-        return np.diag(1 / back_childs[idx].data)
-
-
-@singleton
-class Softmax(Operation):
-    """
-    y = softmax(x) = x.exp() / x.exp().sum(), this is an approximation for `argamx`
-    """
-
-    @staticmethod
-    def softmax(x: np.ndarray) -> np.ndarray:
-        e = np.exp(x - x.max())
-        return e / e.sum()
-
-    def forward(self, x: Tensor) -> Tensor:
-        # avoid overflow
-        res = Tensor(Softmax.softmax(x.data))
-        res.back_f = self
-        res.back_childs = (x,)
-        return res
-
-    def gradient(self, back_childs: tuple, idx=0) -> np.ndarray:
-        x = back_childs[idx]
-        y = self.softmax(x.data)
-        vec = y.reshape((-1, 1))
-        # broadcast
-        return np.diag(y) - vec @ vec.T
-        # n = x.shape[0]
-        # grad = np.zeros((n, n))
-        # for i in range(n):
-        #     for j in range(i, n):
-        #         grad[i, j] = y[i] * (1 - y[i]) if i == j else -y[i] * y[j]
-        #         grad[j, i] = grad[i, j]
-        # return grad
-
-
-@singleton
-class LogSoftmax(Operation):
-    """
-    y = log(softmax(x)), more numerical stable version.
-    """
-
-    def forward(self, x: Tensor) -> Tensor:
-        a = x.data
-        m = np.abs(a).max()
-        e = np.exp(a - m)
-        # avoid overflow
-        res = Tensor(a - m - np.log(e.sum()))
-        res.back_f = self
-        res.back_childs = (x,)
-        return res
-
-    def gradient(self, back_childs: tuple, idx=0) -> np.ndarray:
-        x = back_childs[idx]
-        n = x.shape[0]
-        y = Softmax.softmax(x.data).reshape((1, n))
-        # broadcast
-        return np.eye(n) - y
-        # grad = np.zeros((n,n))
-        # for i in range(n):
-        #     for j in range(n):
-        #         grad[i, j] = 1 - y[j] if i == j else -y[j]
-        # return grad
-
-
-@singleton
-class ReLU(Operation):
-    """
-    y = relu(x) = max(0,x)
-    """
-
-    def forward(self, x: Tensor) -> Tensor:
-        res = Tensor(np.maximum(x.data, 0))
-        res.back_f = self
-        res.back_childs = (x,)
-        return res
-
-    def gradient(self, back_childs: tuple, idx=0) -> np.ndarray:
-        x = back_childs[idx].data
-        grad = np.zeros_like(x)
-        grad[x > 0] = 1
-        return np.diag(grad)
+"""Tensor operation implementation"""
+
+from functools import wraps
+
+from .autograd import Tensor
+from .base import Operation, np
+
+__all__ = [
+    "Add",  # basic oprations
+    "Inner",
+    "Flatten",
+    "Sum",  # loss functions
+    "Norm",
+    "NLL",
+    "Log",  # activation functions
+    "Softmax",
+    "LogSoftmax",
+    "ReLU",
+]
+
+
+def one_hot(x, NUM_CLASS):
+    y = np.zeros((x.size, NUM_CLASS))
+    y[np.arange(x.size), x] = 1
+    return y
+
+
+def singleton(original_cls):
+    """
+    Decorator for basic operations, make them all **singleton**.
+    Otherwise eachtime we do operations, we will eastablish a new object.
+    code refer to https://igeorgiev.eu/python/design-patterns/python-singleton-pattern-decorator/
+    """
+    original_new_method = original_cls.__new__
+    instance = None
+
+    @wraps(original_cls.__new__)
+    def __new__(cls, *args, **kwargs):
+        nonlocal instance
+        if instance is None:
+            instance = original_new_method(cls, *args, **kwargs)
+        return instance
+
+    original_cls.__new__ = __new__
+    return original_cls
+
+
+@singleton
+class Add(Operation):
+    """z = x + y"""
+
+    def forward(self, x: Tensor, y: Tensor) -> Tensor:
+        res = Tensor(x.data + y.data)
+        res.back_f = self
+        res.back_childs = (x, y)
+        return res
+
+    def gradient(self, back_childs: tuple, idx=0) -> np.ndarray:
+        r"""
+        1. `d(X+Y) / dX = \mathbb{I} \otimes \mathbb{I}` if X is matrix
+        2. `d(x+y) / dx = \mathbb{I}` if x is vector
+        """
+        x = back_childs[idx]
+        assert x.ndim <= 2
+        if x.ndim == 1:
+            return np.eye(*x.shape)
+        else:
+            raise NotImplementedError("No need.")
+
+
+@singleton
+class Inner(Operation):
+    """
+    z = x @ y where z is vector or scalar
+    """
+
+    def forward(self, x: Tensor, y: Tensor) -> Tensor:
+        res = Tensor(x.data @ y.data)
+        assert res.ndim == 1, "result should be vector or scalar"
+        res.back_f = self
+        res.back_childs = (x, y)
+        return res
+
+    def gradient(self, back_childs: tuple, idx=0) -> np.ndarray:
+        r"""
+        if x is matrix
+        d x@y / dx[i,j] = [0,...,y[j],... ,0], where y[j] is the ith component
+        or in tensor product: `d x@y / dX = c' \otimes \mathbb{I}`
+
+        elif x is vector
+        d x@y / dx = y.T
+        """
+        x, y = back_childs
+        x, y = x.data, y.data
+        if idx == 0:
+            if x.ndim == 1:
+                return y.T
+            else:
+                m, n = x.shape
+                res = np.zeros((m, m, n))
+                res[np.arange(m), np.arange(m), :] = y
+                return res
+        else:
+            if y.ndim == 1:
+                return x
+            else:
+                m, n = y.shape
+                res = np.zeros((n, m, n))
+                res[np.arange(n), :, np.arange(n)] = x
+                return res
+
+
+@singleton
+class Flatten(Operation):
+    """y = x.flatten()"""
+
+    def forward(self, x: Tensor) -> Tensor:
+        res = Tensor(x.data.flatten())
+        res.back_f = self
+        res.back_childs = (x,)
+        return res
+
+    def gradient(self, back_childs: tuple, idx=0) -> np.ndarray:
+        x = back_childs[idx]
+        if x.ndim == 1:
+            return np.eye(*x.shape)
+        else:
+            m, n = x.shape
+            res = np.zeros((m * n, m, n))
+            for i in range(m * n):
+                res[i, i // m, i % n] = 1
+            return res
+
+
+@singleton
+class Sum(Operation):
+    """y = sum(X)"""
+
+    def forward(self, x: Tensor) -> Tensor:
+        res = Tensor(x.data.sum().reshape((1,)))
+        res.back_f = self
+        res.back_childs = (x,)
+        return res
+
+    def gradient(self, back_childs: tuple, idx=0) -> np.ndarray:
+        """Easy"""
+        return np.ones_like(back_childs[idx])
+
+
+@singleton
+class Norm(Operation):
+    """
+    y = sqrt(x.T @ x)
+    """
+
+    def forward(self, x: Tensor) -> Tensor:
+        m = np.abs(x.data).max()
+        a = x.data / m
+        # in my test, arr@arr is faster than np.inner(a,a) and np.dot(a,a)
+        # and np.sqrt(a@a) is faster than np.linalg.norm(a, 2)
+        res = Tensor(m * np.sqrt(a @ a).reshape((1,)))
+        res.back_f = self
+        res.back_childs = (x,)
+        return res
+
+    def gradient(self, back_childs: tuple, idx=0) -> np.ndarray:
+        """
+        `d norm2(x) / dx = x / norm2(x)`
+        """
+        x = back_childs[idx]
+        y = self.forward(x)
+        return x.data / y.data
+
+
+@singleton
+class NLL(Operation):
+    """
+    Negative Log Likelihod
+    l = -sum(x @ y)
+    """
+
+    def forward(self, x: Tensor, y: Tensor) -> Tensor:
+        res = Tensor(-(x.data @ y.data).sum().reshape((1,)))
+        res.back_f = self
+        res.back_childs = (x, y)
+        return res
+
+    def gradient(self, back_childs: tuple, idx=0) -> np.ndarray:
+        """
+        dl / dx = -y, dl / dy = -x
+        """
+        return -back_childs[1 - idx].data
+
+
+@singleton
+class Log(Operation):
+    """
+    y = x.log()
+    """
+
+    def forward(self, x: Tensor) -> Tensor:
+        assert (x.data > 0).all()
+        res = Tensor(np.log(x))
+        res.back_f = self
+        res.back_childs = (x,)
+        return res
+
+    def gradient(self, back_childs: tuple, idx=0) -> np.ndarray:
+        """
+        dy / dx = diag(1/x)
+        """
+        return np.diag(1 / back_childs[idx].data)
+
+
+@singleton
+class Softmax(Operation):
+    """
+    y = softmax(x) = x.exp() / x.exp().sum(), this is an approximation for `argamx`
+    """
+
+    @staticmethod
+    def softmax(x: np.ndarray) -> np.ndarray:
+        e = np.exp(x - x.max())
+        return e / e.sum()
+
+    def forward(self, x: Tensor) -> Tensor:
+        # avoid overflow
+        res = Tensor(Softmax.softmax(x.data))
+        res.back_f = self
+        res.back_childs = (x,)
+        return res
+
+    def gradient(self, back_childs: tuple, idx=0) -> np.ndarray:
+        x = back_childs[idx]
+        y = self.softmax(x.data)
+        vec = y.reshape((-1, 1))
+        # broadcast
+        return np.diag(y) - vec @ vec.T
+        # n = x.shape[0]
+        # grad = np.zeros((n, n))
+        # for i in range(n):
+        #     for j in range(i, n):
+        #         grad[i, j] = y[i] * (1 - y[i]) if i == j else -y[i] * y[j]
+        #         grad[j, i] = grad[i, j]
+        # return grad
+
+
+@singleton
+class LogSoftmax(Operation):
+    """
+    y = log(softmax(x)), more numerical stable version.
+    """
+
+    def forward(self, x: Tensor) -> Tensor:
+        a = x.data
+        m = np.abs(a).max()
+        e = np.exp(a - m)
+        # avoid overflow
+        res = Tensor(a - m - np.log(e.sum()))
+        res.back_f = self
+        res.back_childs = (x,)
+        return res
+
+    def gradient(self, back_childs: tuple, idx=0) -> np.ndarray:
+        x = back_childs[idx]
+        n = x.shape[0]
+        y = Softmax.softmax(x.data).reshape((1, n))
+        # broadcast
+        return np.eye(n) - y
+        # grad = np.zeros((n,n))
+        # for i in range(n):
+        #     for j in range(n):
+        #         grad[i, j] = 1 - y[j] if i == j else -y[j]
+        # return grad
+
+
+@singleton
+class ReLU(Operation):
+    """
+    y = relu(x) = max(0,x)
+    """
+
+    def forward(self, x: Tensor) -> Tensor:
+        res = Tensor(np.maximum(x.data, 0))
+        res.back_f = self
+        res.back_childs = (x,)
+        return res
+
+    def gradient(self, back_childs: tuple, idx=0) -> np.ndarray:
+        x = back_childs[idx].data
+        grad = np.zeros_like(x)
+        grad[x > 0] = 1
+        return np.diag(grad)
```

### Comparing `npnn-0.0.2/src/npnn/nn.py` & `npnn-0.0.3/src/npnn/nn.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-"""Neural Network components implementation"""
-
-from .base import Module, np
-from .functional import Inner, Add
-from .autograd import Tensor
-
-rand = np.random.random
-
-
-class Linear(Module):
-
-    def __init__(self, in_size, out_size, bias=True) -> None:
-        super().__init__()
-        self.in_size = in_size
-        self.out_size = out_size
-        self.bias = bias
-        self.A = Tensor(rand((out_size, in_size)), requires_grad=True)
-        if self.bias:
-            self.b = Tensor(rand((out_size,)), requires_grad=True)
-
-    def forward(self, x: Tensor) -> Tensor:
-        inner = Inner()
-        add = Add()
-        return add(inner(self.A, x), self.b)
-
-    def parameters(self) -> list:
-        return [self.A, self.b]
-
-
-class Sequential(Module):
-
-    def __init__(self, *layers) -> None:
-        super().__init__()
-        self.layers = layers
-
-    def forward(self, x: Tensor) -> Tensor:
-        h = x
-        for layer in self.layers:
-            h = layer(h)
-        return h
-
-    def parameters(self) -> list:
-        res = []
-        for layer in self.layers:
-            if isinstance(layer, Module):
-                res.extend(layer.parameters())
-        return res
+"""Neural Network components implementation"""
+
+from .base import Module, np
+from .functional import Inner, Add
+from .autograd import Tensor
+
+rand = np.random.random
+
+
+class Linear(Module):
+
+    def __init__(self, in_size, out_size, bias=True) -> None:
+        super().__init__()
+        self.in_size = in_size
+        self.out_size = out_size
+        self.bias = bias
+        self.A = Tensor(rand((out_size, in_size)), requires_grad=True)
+        if self.bias:
+            self.b = Tensor(rand((out_size,)), requires_grad=True)
+
+    def forward(self, x: Tensor) -> Tensor:
+        inner = Inner()
+        add = Add()
+        return add(inner(self.A, x), self.b)
+
+    def parameters(self) -> list:
+        return [self.A, self.b]
+
+
+class Sequential(Module):
+
+    def __init__(self, *layers) -> None:
+        super().__init__()
+        self.layers = layers
+
+    def forward(self, x: Tensor) -> Tensor:
+        h = x
+        for layer in self.layers:
+            h = layer(h)
+        return h
+
+    def parameters(self) -> list:
+        res = []
+        for layer in self.layers:
+            if isinstance(layer, Module):
+                res.extend(layer.parameters())
+        return res
```

### Comparing `npnn-0.0.2/src/npnn/test_autograd.py` & `npnn-0.0.3/tests/test_autograd.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,266 +1,269 @@
-"""
-In this file we test npnn api, compared with torch api ^&^.
-"""
-
-import unittest
-
-from .base import np
-from .autograd import Tensor
-from .functional import *
-
-import torch  # only for test, ensure computation of npnn is right
-
-
-TEST_SIZE = 5
-rand = lambda size: np.random.random(size=size) - 0.5
-
-
-class TestAutograd(unittest.TestCase):
-
-    def test_Flatten(self):
-        """
-        y = sum(x.flatten())
-        """
-
-        # npnn api
-        x = Tensor(rand((3, 3)), requires_grad=True)
-        y = Sum()(Flatten()(x))
-        y.backward()
-        grad_nnn = x.grad
-
-        # torch api
-        if np.__name__ == "cupy":
-            x = torch.from_numpy(x.data.get())
-        elif np.__name__ == "numpy":
-            x = torch.from_numpy(x.data)
-        x.requires_grad = True
-        y = torch.sum(x.flatten())
-        y.backward()
-        grad_torh = x.grad.numpy()
-
-        # check float almost equal
-        self.assertTrue(np.allclose(grad_nnn, grad_torh))
-
-    def test_Linear(self):
-        """
-        Test linear function:
-
-        y = sum((A @ x) @ B + c)
-
-        by calcuting dy/dA and dy/db.
-        we use `sum` to test since its derivative is super simple.
-        """
-
-        # npnn api
-        A = Tensor(rand((TEST_SIZE, TEST_SIZE)), requires_grad=True)
-        B = Tensor(rand((TEST_SIZE, TEST_SIZE)), requires_grad=True)
-        c = Tensor(rand((TEST_SIZE,)), requires_grad=True)
-        x = Tensor(rand((TEST_SIZE,)))
-        inner = Inner()
-        sum = Sum()
-        add = Add()
-        y = sum(
-            add(
-                inner(inner(A, x), B),  # test left and right
-                c,
-            )
-        )
-        y.backward()
-        A_grad_nnn = A.grad
-        B_grad_nnn = B.grad
-        c_grad_nnn = c.grad
-
-        # torch api
-        if np.__name__ == "cupy":
-            A = torch.from_numpy(A.data.get())
-            B = torch.from_numpy(B.data.get())
-            c = torch.from_numpy(c.data.get())
-            x = torch.from_numpy(x.data.get())
-        elif np.__name__ == "numpy":
-            A = torch.from_numpy(A.data)
-            B = torch.from_numpy(B.data)
-            c = torch.from_numpy(c.data)
-            x = torch.from_numpy(x.data)
-        A.requires_grad = True
-        B.requires_grad = True
-        c.requires_grad = True
-        y = ((A @ x) @ B + c).sum()
-        y.backward()
-        A_grad_torch = A.grad.numpy()
-        B_grad_torch = B.grad.numpy()
-        c_grad_torch = c.grad.numpy()
-
-        # check float almost equal
-        self.assertTrue(np.allclose(A_grad_nnn, A_grad_torch))
-        self.assertTrue(np.allclose(B_grad_nnn, B_grad_torch))
-        self.assertTrue(np.allclose(c_grad_nnn, c_grad_torch))
-
-    def test_Activation(self):
-        """
-        Test linear layer + acitvation function:
-
-        y = sum(activation(h)), h = A @ x + b
-
-        by calcuting dy/dA and dy/db.
-        """
-        for act_nnn, act_torch in [
-            (Softmax(), torch.nn.Softmax(dim=0)),
-            (LogSoftmax(), torch.nn.LogSoftmax(dim=0)),
-            (ReLU(), torch.relu),
-        ]:
-            # npnn api
-            A = Tensor(rand((TEST_SIZE, TEST_SIZE)), requires_grad=True)
-            b = Tensor(rand((TEST_SIZE,)), requires_grad=True)
-            x = Tensor(rand((TEST_SIZE,)))
-            inner = Inner()
-            add = Add()
-            sum = Sum()
-            h = add(inner(A, x), b)
-            y = sum(act_nnn(h))
-            y.backward()
-            A_grad_nnn = A.grad
-            b_grad_nnn = b.grad
-
-            # torch api
-            if np.__name__ == "cupy":
-                A = torch.from_numpy(A.data.get())
-                b = torch.from_numpy(b.data.get())
-                x = torch.from_numpy(x.data.get())
-            elif np.__name__ == "numpy":
-                A = torch.from_numpy(A.data)
-                b = torch.from_numpy(b.data)
-                x = torch.from_numpy(x.data)
-            A.requires_grad = True
-            b.requires_grad = True
-            y = act_torch(A @ x + b).sum()
-            y.backward()
-            A_grad_torch = A.grad.numpy()
-            b_grad_torch = b.grad.numpy()
-            # check float almost equal
-            self.assertTrue(np.allclose(A_grad_nnn, A_grad_torch))
-            self.assertTrue(np.allclose(b_grad_nnn, b_grad_torch))
-
-    def test_Loss(self):
-        """
-        Test linear layer + loss function:
-
-        y = loss(A @ x + b - z)
-
-        by calcuting dy/dA and dy/db.
-        """
-        # npnn api
-        A = Tensor(rand((TEST_SIZE, TEST_SIZE)), requires_grad=True)
-        b = Tensor(rand((TEST_SIZE,)), requires_grad=True)
-        z = -Tensor(rand((TEST_SIZE,)))  # add netgative z
-        x = Tensor(rand((TEST_SIZE,)))
-        inner = Inner()
-        norm = Norm()
-        add = Add()
-        y = norm(
-            add(
-                add(
-                    inner(A, x),
-                    b,
-                ),
-                z,
-            )
-        )
-        y.backward()
-        A_grad_nnn = A.grad
-        b_grad_nnn = b.grad
-
-        # torch api
-        if np.__name__ == "cupy":
-            A = torch.from_numpy(A.data.get())
-            b = torch.from_numpy(b.data.get())
-            z = torch.from_numpy(z.data.get())
-            x = torch.from_numpy(x.data.get())
-        elif np.__name__ == "numpy":
-            A = torch.from_numpy(A.data)
-            b = torch.from_numpy(b.data)
-            z = torch.from_numpy(z.data)
-            x = torch.from_numpy(x.data)
-        A.requires_grad = True
-        b.requires_grad = True
-        y = torch.norm(A @ x + b + z, p=2)
-        y.backward()
-        A_grad_torch = A.grad.numpy()
-        b_grad_torch = b.grad.numpy()
-
-        # check float almost equal
-        self.assertTrue(np.allclose(A_grad_nnn, A_grad_torch))
-        self.assertTrue(np.allclose(b_grad_nnn, b_grad_torch))
-
-    def test_NN(self):
-        """
-        Test a Neural Network with 3-hidden layers:
-
-        h1 = relu(A @ x + a)
-        h2 = relu(B @ h1 + b)
-        y_hat = relu(C @ h2 + c)
-
-        choose L2 norm as loss function:
-
-        l = norm(y_hat + (-y))
-
-        """
-
-        # npnn api
-        A = Tensor(rand((TEST_SIZE, TEST_SIZE)), requires_grad=True)
-        B = Tensor(rand((TEST_SIZE, TEST_SIZE)), requires_grad=True)
-        C = Tensor(rand((TEST_SIZE, TEST_SIZE)), requires_grad=True)
-        a = Tensor(rand((TEST_SIZE,)), requires_grad=True)
-        b = Tensor(rand((TEST_SIZE,)), requires_grad=True)
-        c = Tensor(rand((TEST_SIZE,)), requires_grad=True)
-        x = Tensor(rand((TEST_SIZE,)))
-        y = Tensor(rand((TEST_SIZE,)))
-        inner = Inner()
-        norm = Norm()
-        add = Add()
-        relu = ReLU()
-        h1 = relu(add(inner(A, x), a))
-        h2 = relu(add(inner(B, h1), b))
-        y_hat = relu(add(inner(C, h2), c))
-        l = norm(add(y_hat, (-y)))
-        l.backward()
-        nnn_grad = [A.grad, B.grad, C.grad, a.grad, b.grad, c.grad]
-
-        # torch api
-        if np.__name__ == "cupy":
-            A = torch.from_numpy(A.data.get())
-            B = torch.from_numpy(B.data.get())
-            C = torch.from_numpy(C.data.get())
-            a = torch.from_numpy(a.data.get())
-            b = torch.from_numpy(b.data.get())
-            c = torch.from_numpy(c.data.get())
-            x = torch.from_numpy(x.data.get())
-            y = torch.from_numpy(y.data.get())
-        elif np.__name__ == "numpy":
-            A = torch.from_numpy(A.data)
-            B = torch.from_numpy(B.data)
-            C = torch.from_numpy(C.data)
-            a = torch.from_numpy(a.data)
-            b = torch.from_numpy(b.data)
-            c = torch.from_numpy(c.data)
-            x = torch.from_numpy(x.data)
-            y = torch.from_numpy(y.data)
-        A.requires_grad = True
-        B.requires_grad = True
-        C.requires_grad = True
-        a.requires_grad = True
-        b.requires_grad = True
-        c.requires_grad = True
-        h1 = torch.relu(A @ x + a)
-        h2 = torch.relu(B @ h1 + b)
-        y_hat = torch.relu(C @ h2 + c)
-        l = torch.norm(y_hat - y, p=2)
-        l.backward()
-        torch_grad = [A.grad, B.grad, C.grad, a.grad, b.grad, c.grad]
-
-        # check float almost equal
-        for g1, g2 in zip(nnn_grad, torch_grad):
-            self.assertTrue(np.allclose(g1, g2))
-
-
-if __name__ == "__main__":
-    unittest.main()
+"""
+In this file we test npnn api, compared with torch api ^&^.
+"""
+
+import unittest
+
+from npnn.base import np
+from npnn.autograd import Tensor
+from npnn.functional import Add, Norm, Inner, Sum, LogSoftmax, Softmax, ReLU, Flatten
+
+import torch  # only for test, ensure computation of npnn is right
+
+
+TEST_SIZE = 5
+
+
+def rand(size):
+    return np.random.random(size=size) - 0.5
+
+
+class TestAutograd(unittest.TestCase):
+
+    def test_Flatten(self):
+        """
+        y = sum(x.flatten())
+        """
+
+        # npnn api
+        x = Tensor(rand((3, 3)), requires_grad=True)
+        y = Sum()(Flatten()(x))
+        y.backward()
+        grad_nnn = x.grad
+
+        # torch api
+        if np.__name__ == "cupy":
+            x = torch.from_numpy(x.data.get())
+        elif np.__name__ == "numpy":
+            x = torch.from_numpy(x.data)
+        x.requires_grad = True
+        y = torch.sum(x.flatten())
+        y.backward()
+        grad_torh = x.grad.numpy()
+
+        # check float almost equal
+        self.assertTrue(np.allclose(grad_nnn, grad_torh))
+
+    def test_Linear(self):
+        """
+        Test linear function:
+
+        y = sum((A @ x) @ B + c)
+
+        by calcuting dy/dA and dy/db.
+        we use `sum` to test since its derivative is super simple.
+        """
+
+        # npnn api
+        A = Tensor(rand((TEST_SIZE, TEST_SIZE)), requires_grad=True)
+        B = Tensor(rand((TEST_SIZE, TEST_SIZE)), requires_grad=True)
+        c = Tensor(rand((TEST_SIZE,)), requires_grad=True)
+        x = Tensor(rand((TEST_SIZE,)))
+        inner = Inner()
+        sum = Sum()
+        add = Add()
+        y = sum(
+            add(
+                inner(inner(A, x), B),  # test left and right
+                c,
+            )
+        )
+        y.backward()
+        A_grad_nnn = A.grad
+        B_grad_nnn = B.grad
+        c_grad_nnn = c.grad
+
+        # torch api
+        if np.__name__ == "cupy":
+            A = torch.from_numpy(A.data.get())
+            B = torch.from_numpy(B.data.get())
+            c = torch.from_numpy(c.data.get())
+            x = torch.from_numpy(x.data.get())
+        elif np.__name__ == "numpy":
+            A = torch.from_numpy(A.data)
+            B = torch.from_numpy(B.data)
+            c = torch.from_numpy(c.data)
+            x = torch.from_numpy(x.data)
+        A.requires_grad = True
+        B.requires_grad = True
+        c.requires_grad = True
+        y = ((A @ x) @ B + c).sum()
+        y.backward()
+        A_grad_torch = A.grad.numpy()
+        B_grad_torch = B.grad.numpy()
+        c_grad_torch = c.grad.numpy()
+
+        # check float almost equal
+        self.assertTrue(np.allclose(A_grad_nnn, A_grad_torch))
+        self.assertTrue(np.allclose(B_grad_nnn, B_grad_torch))
+        self.assertTrue(np.allclose(c_grad_nnn, c_grad_torch))
+
+    def test_Activation(self):
+        """
+        Test linear layer + acitvation function:
+
+        y = sum(activation(h)), h = A @ x + b
+
+        by calcuting dy/dA and dy/db.
+        """
+        for act_nnn, act_torch in [
+            (Softmax(), torch.nn.Softmax(dim=0)),
+            (LogSoftmax(), torch.nn.LogSoftmax(dim=0)),
+            (ReLU(), torch.relu),
+        ]:
+            # npnn api
+            A = Tensor(rand((TEST_SIZE, TEST_SIZE)), requires_grad=True)
+            b = Tensor(rand((TEST_SIZE,)), requires_grad=True)
+            x = Tensor(rand((TEST_SIZE,)))
+            inner = Inner()
+            add = Add()
+            sum = Sum()
+            h = add(inner(A, x), b)
+            y = sum(act_nnn(h))
+            y.backward()
+            A_grad_nnn = A.grad
+            b_grad_nnn = b.grad
+
+            # torch api
+            if np.__name__ == "cupy":
+                A = torch.from_numpy(A.data.get())
+                b = torch.from_numpy(b.data.get())
+                x = torch.from_numpy(x.data.get())
+            elif np.__name__ == "numpy":
+                A = torch.from_numpy(A.data)
+                b = torch.from_numpy(b.data)
+                x = torch.from_numpy(x.data)
+            A.requires_grad = True
+            b.requires_grad = True
+            y = act_torch(A @ x + b).sum()
+            y.backward()
+            A_grad_torch = A.grad.numpy()
+            b_grad_torch = b.grad.numpy()
+            # check float almost equal
+            self.assertTrue(np.allclose(A_grad_nnn, A_grad_torch))
+            self.assertTrue(np.allclose(b_grad_nnn, b_grad_torch))
+
+    def test_Loss(self):
+        """
+        Test linear layer + loss function:
+
+        y = loss(A @ x + b - z)
+
+        by calcuting dy/dA and dy/db.
+        """
+        # npnn api
+        A = Tensor(rand((TEST_SIZE, TEST_SIZE)), requires_grad=True)
+        b = Tensor(rand((TEST_SIZE,)), requires_grad=True)
+        z = -Tensor(rand((TEST_SIZE,)))  # add netgative z
+        x = Tensor(rand((TEST_SIZE,)))
+        inner = Inner()
+        norm = Norm()
+        add = Add()
+        y = norm(
+            add(
+                add(
+                    inner(A, x),
+                    b,
+                ),
+                z,
+            )
+        )
+        y.backward()
+        A_grad_nnn = A.grad
+        b_grad_nnn = b.grad
+
+        # torch api
+        if np.__name__ == "cupy":
+            A = torch.from_numpy(A.data.get())
+            b = torch.from_numpy(b.data.get())
+            z = torch.from_numpy(z.data.get())
+            x = torch.from_numpy(x.data.get())
+        elif np.__name__ == "numpy":
+            A = torch.from_numpy(A.data)
+            b = torch.from_numpy(b.data)
+            z = torch.from_numpy(z.data)
+            x = torch.from_numpy(x.data)
+        A.requires_grad = True
+        b.requires_grad = True
+        y = torch.norm(A @ x + b + z, p=2)
+        y.backward()
+        A_grad_torch = A.grad.numpy()
+        b_grad_torch = b.grad.numpy()
+
+        # check float almost equal
+        self.assertTrue(np.allclose(A_grad_nnn, A_grad_torch))
+        self.assertTrue(np.allclose(b_grad_nnn, b_grad_torch))
+
+    def test_NN(self):
+        """
+        Test a Neural Network with 3-hidden layers:
+
+        h1 = relu(A @ x + a)
+        h2 = relu(B @ h1 + b)
+        y_hat = relu(C @ h2 + c)
+
+        choose L2 norm as loss function:
+
+        l = norm(y_hat + (-y))
+
+        """
+
+        # npnn api
+        A = Tensor(rand((TEST_SIZE, TEST_SIZE)), requires_grad=True)
+        B = Tensor(rand((TEST_SIZE, TEST_SIZE)), requires_grad=True)
+        C = Tensor(rand((TEST_SIZE, TEST_SIZE)), requires_grad=True)
+        a = Tensor(rand((TEST_SIZE,)), requires_grad=True)
+        b = Tensor(rand((TEST_SIZE,)), requires_grad=True)
+        c = Tensor(rand((TEST_SIZE,)), requires_grad=True)
+        x = Tensor(rand((TEST_SIZE,)))
+        y = Tensor(rand((TEST_SIZE,)))
+        inner = Inner()
+        norm = Norm()
+        add = Add()
+        relu = ReLU()
+        h1 = relu(add(inner(A, x), a))
+        h2 = relu(add(inner(B, h1), b))
+        y_hat = relu(add(inner(C, h2), c))
+        loss = norm(add(y_hat, (-y)))
+        loss.backward()
+        nnn_grad = [A.grad, B.grad, C.grad, a.grad, b.grad, c.grad]
+
+        # torch api
+        if np.__name__ == "cupy":
+            A = torch.from_numpy(A.data.get())
+            B = torch.from_numpy(B.data.get())
+            C = torch.from_numpy(C.data.get())
+            a = torch.from_numpy(a.data.get())
+            b = torch.from_numpy(b.data.get())
+            c = torch.from_numpy(c.data.get())
+            x = torch.from_numpy(x.data.get())
+            y = torch.from_numpy(y.data.get())
+        elif np.__name__ == "numpy":
+            A = torch.from_numpy(A.data)
+            B = torch.from_numpy(B.data)
+            C = torch.from_numpy(C.data)
+            a = torch.from_numpy(a.data)
+            b = torch.from_numpy(b.data)
+            c = torch.from_numpy(c.data)
+            x = torch.from_numpy(x.data)
+            y = torch.from_numpy(y.data)
+        A.requires_grad = True
+        B.requires_grad = True
+        C.requires_grad = True
+        a.requires_grad = True
+        b.requires_grad = True
+        c.requires_grad = True
+        h1 = torch.relu(A @ x + a)
+        h2 = torch.relu(B @ h1 + b)
+        y_hat = torch.relu(C @ h2 + c)
+        loss = torch.norm(y_hat - y, p=2)
+        loss.backward()
+        torch_grad = [A.grad, B.grad, C.grad, a.grad, b.grad, c.grad]
+
+        # check float almost equal
+        for g1, g2 in zip(nnn_grad, torch_grad):
+            self.assertTrue(np.allclose(g1, g2))
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `npnn-0.0.2/src/npnn.egg-info/PKG-INFO` & `npnn-0.0.3/src/npnn.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,96 +1,97 @@
-Metadata-Version: 2.1
-Name: npnn
-Version: 0.0.2
-Summary: NumPy Neural Network
-Author-email: Yang Zhang <mail@yangzhang.site>
-License: MIT License
-        
-        Copyright (c) 2024 Yang Zhang
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/AIboy996/npnn
-Keywords: numpy,neural network,machine learning,autograd
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Provides-Extra: cuda11x
-Requires-Dist: cupy-cuda11x; extra == "cuda11x"
-Provides-Extra: cuda12x
-Requires-Dist: cupy-cuda12x; extra == "cuda12x"
-
-# [npnn](https://pypi.org/project/npnn/0.0.1/)
-> NumPy Neural Network
-
-[![PyPI - Version](https://img.shields.io/pypi/v/npnn)](https://pypi.org/project/npnn/0.0.1/)
-![PyPI - Implementation](https://img.shields.io/pypi/implementation/npnn)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/npnn)
-<!-- ![PyPI - Downloads](https://img.shields.io/pypi/dm/npnn) -->
-
-
-## What's npnn?
-> `npnn` is a a **torch-like** Python module for **gradient descent based machine learning** implemented with `numpy`. 
-
-### Dependency
-Basically `npnn` only depends on `numpy`(the latest version 1.26.4 is verified).
-
-If you have CUDA devices available, then you can easily get a acceleration by installing suitable version of `cupy`.  In this case `npnn` will use `cupy` api rather than `numpy` api.
-
-For example, my PC have CUDA v12.x (x86_64), so I use command:
-```bash
-pip install cupy-cuda12x
-pip install npnn
-```
-or in short:
-```bash
-pip install npnn[cuda12x]
-```
-check [cupy documentation](https://docs.cupy.dev/en/stable/install.html#installing-cupy) for more information.
-
-
-### API references
-
-See [npnn WIKI](https://github.com/AIboy996/npnn/wiki).
-
-## Work with npnn!
-> Here we will construct a image classification neural network with npnn.
-
-BTW, this is a course assignment of *DATA620004, School of Data Science, Fudan University*.
-
-### Task
-Construct and Train a neural network on [Fashion-MNIST](https://github.com/zalandoresearch/fashion-mnist) to do image classification.
-
-- Implement gradient backpropagation algorithm by hand,you can use `numpy` but **DO NOT** use `pytorch` or `tensorflow` to do autograd.
-
-- Submit source code including at least four parts: `model definition`, `training`, `parameters searching` and `testing`.
-
-### Implementation
-
-- `dataset.py`: provide Fashion MNIST dataset
-- `model.py`: model definition
-- `train.py`: model training
-- `search.py`: parameters searching
-- `test.py`: model testing
-- `utils.py`: some misc function, such as `save_mode`
+Metadata-Version: 2.1
+Name: npnn
+Version: 0.0.3
+Summary: NumPy Neural Network
+Author-email: Yang Zhang <mail@yangzhang.site>
+License: MIT License
+        
+        Copyright (c) 2024 Yang Zhang
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/AIboy996/npnn
+Keywords: numpy,neural network,machine learning,autograd
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Provides-Extra: cuda11x
+Requires-Dist: cupy-cuda11x; extra == "cuda11x"
+Provides-Extra: cuda12x
+Requires-Dist: cupy-cuda12x; extra == "cuda12x"
+
+# [npnn](https://pypi.org/project/npnn/)
+> NumPy Neural Network
+
+[![PyPI - Version](https://img.shields.io/pypi/v/npnn)](https://pypi.org/project/npnn/)
+![PyPI - Implementation](https://img.shields.io/pypi/implementation/npnn)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/npnn)
+<!-- ![PyPI - Downloads](https://img.shields.io/pypi/dm/npnn) -->
+
+
+## What's npnn?
+> `npnn` is a a **torch-like** Python module for **gradient descent based machine learning** implemented with `numpy`. 
+
+### Dependency
+Basically `npnn` only depends on `numpy`(the latest version 1.26.4 is verified).
+
+If you have CUDA devices available, then you can easily get a acceleration by installing suitable version of `cupy`.  In this case `npnn` will use `cupy` api rather than `numpy` api.
+
+For example, my PC have CUDA v12.x (x86_64), so I use command:
+```bash
+pip install cupy-cuda12x
+pip install npnn
+```
+or in short:
+```bash
+pip install npnn[cuda12x]
+```
+check [cupy documentation](https://docs.cupy.dev/en/stable/install.html#installing-cupy) for more information.
+
+
+### API references
+
+See [npnn WIKI](https://github.com/AIboy996/npnn/wiki).
+
+## Work with npnn!
+> Here we will construct a image classification neural network with npnn.
+
+BTW, this is a course assignment of *DATA620004, School of Data Science, Fudan University*.
+
+### Task
+Construct and Train a neural network on [Fashion-MNIST](https://github.com/zalandoresearch/fashion-mnist) to do image classification.
+
+- Implement gradient backpropagation algorithm by hand,you can use `numpy` but **DO NOT** use `pytorch` or `tensorflow` to do autograd.
+
+- Submit source code including at least four parts: `model definition`, `training`, `parameters searching` and `testing`.
+
+### Implementation
+
+- `dataset.py`: provide Fashion MNIST dataset
+- `model.py`: model definition
+- `train.py`: model training
+- `search.py`: parameters searching
+- `test.py`: model testing
+- `viz.py`: visualization
+- `utils.py`: some misc function, such as `save_model`
```

