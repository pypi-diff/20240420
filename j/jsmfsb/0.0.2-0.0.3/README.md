# Comparing `tmp/jsmfsb-0.0.2.tar.gz` & `tmp/jsmfsb-0.0.3.tar.gz`

## Comparing `jsmfsb-0.0.2.tar` & `jsmfsb-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,25 @@
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jsmfsb-0.0.2/Makefile
--rw-r--r--   0        0        0    12704 2020-02-02 00:00:00.000000 jsmfsb-0.0.2/demos/lv.pdf
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 jsmfsb-0.0.2/demos/lv.py
--rw-r--r--   0        0        0     8088 2020-02-02 00:00:00.000000 jsmfsb-0.0.2/demos/lvH.pdf
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 jsmfsb-0.0.2/demos/shbuild.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 jsmfsb-0.0.2/src/jsmfsb/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 jsmfsb-0.0.2/src/jsmfsb/models.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 jsmfsb-0.0.2/src/jsmfsb/sim.py
--rw-r--r--   0        0        0     5371 2020-02-02 00:00:00.000000 jsmfsb-0.0.2/src/jsmfsb/smfsbSbml.py
--rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 jsmfsb-0.0.2/src/jsmfsb/spn.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 jsmfsb-0.0.2/tests/test_sim.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 jsmfsb-0.0.2/tests/test_spn.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 jsmfsb-0.0.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jsmfsb-0.0.2/LICENSE
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 jsmfsb-0.0.2/README.md
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 jsmfsb-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 jsmfsb-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/.readthedocs.yaml
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/Makefile
+-rw-r--r--   0        0        0    12704 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/demos/lv.pdf
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/demos/lv.py
+-rw-r--r--   0        0        0     8088 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/demos/lvH.pdf
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/demos/shbuild.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/docs/Makefile
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/docs/conf.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/docs/make.bat
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/docs/requirements.txt
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/docs/source/jsmfsb.rst
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/docs/source/modules.rst
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/src/jsmfsb/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/src/jsmfsb/models.py
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/src/jsmfsb/sim.py
+-rw-r--r--   0        0        0     5371 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/src/jsmfsb/smfsbSbml.py
+-rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/src/jsmfsb/spn.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/tests/test_sim.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/tests/test_spn.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/README.md
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/PKG-INFO
```

### Comparing `jsmfsb-0.0.2/demos/lv.pdf` & `jsmfsb-0.0.3/demos/lv.pdf`

 * *Files 0% similar despite different names*

#### Comparing `jsmfsb-0.0.2/demos/lv.pdf` & `jsmfsb-0.0.3/demos/lv.pdf`

 * *Document info*

```diff
@@ -1,3 +1,3 @@
-CreationDate: "D:20240414222804+01'00'"
+CreationDate: "D:20240419190531+01'00'"
 Creator: 'Matplotlib v3.8.4, https://matplotlib.org'
 Producer: 'Matplotlib pdf backend v3.8.4'
```

### Comparing `jsmfsb-0.0.2/demos/lv.py` & `jsmfsb-0.0.3/demos/lv.py`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.2/demos/lvH.pdf` & `jsmfsb-0.0.3/demos/lvH.pdf`

 * *Files 2% similar despite different names*

#### Comparing `jsmfsb-0.0.2/demos/lvH.pdf` & `jsmfsb-0.0.3/demos/lvH.pdf`

 * *Document info*

```diff
@@ -1,3 +1,3 @@
-CreationDate: "D:20240414222810+01'00'"
+CreationDate: "D:20240419190537+01'00'"
 Creator: 'Matplotlib v3.8.4, https://matplotlib.org'
 Producer: 'Matplotlib pdf backend v3.8.4'
```

### Comparing `jsmfsb-0.0.2/demos/shbuild.py` & `jsmfsb-0.0.3/demos/shbuild.py`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.2/src/jsmfsb/models.py` & `jsmfsb-0.0.3/src/jsmfsb/models.py`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.2/src/jsmfsb/sim.py` & `jsmfsb-0.0.3/src/jsmfsb/sim.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 def simTs(key, x0, t0, tt, dt, stepFun):
     """Simulate a model on a regular grid of times, using a function (closure)
     for advancing the state of the model
 
     This function simulates single realisation of a model on a regular
     grid of times using a function (closure) for advancing the state
     of the model, such as created by ‘stepGillespie’ or
-    ‘stepEuler’.
+    ‘stepCLE’.
 
     Parameters
     ----------
+    key: JAX random number key
+        An unused random number key.
     x0: array of numbers
         The intial state of the system at time t0
     t0: float
         This intial time to be associated with the intial state.
     tt: float
         The terminal time of the simulation.
     dt: float
@@ -35,18 +37,19 @@
 
     Returns
     -------
     A matrix with rows representing the state of the system at successive times.
 
     Examples
     --------
-    >>> import smfsb.models
-    >>> lv = smfsb.models.lv()
+    >>> import jax
+    >>> import jsmfsb.models
+    >>> lv = jsmfsb.models.lv()
     >>> stepLv = lv.stepGillespie()
-    >>> smfsb.simTs([50, 100], 0, 100, 0.1, stepLv)
+    >>> jsmfsb.simTs(jax.random.key(42), lv.m, 0, 100, 0.1, stepLv)
     """
     n = int((tt-t0) // dt) + 1
     u = len(x0)
     keys = jax.random.split(key, n)
     @jit
     def advance(state, key):
         x, t = state
@@ -61,18 +64,20 @@
     """Simulate a many realisations of a model at a given fixed time in the
     future given an initial time and state, using a function (closure) for
     advancing the state of the model
 
     This function simulates many realisations of a model at a given
     fixed time in the future given an initial time and state, using a
     function (closure) for advancing the state of the model , such as
-    created by ‘stepGillespie’ or ‘stepEuler’.
+    created by ‘stepGillespie’ or ‘stepCLE’.
 
     Parameters
     ----------
+    key: JAX random number key
+        An unused random number key.
     n: int
         The number of samples required.
     x0: array of numbers
         The intial state of the system at time t0.
     t0: float
         The intial time to be associated with the initial state.
     deltat: float
@@ -84,18 +89,19 @@
 
     Returns
     -------
     A matrix with rows representing simulated states at time t0+deltat.
 
     Examples
     --------
-    >>> import smfsb.models
-    >>> lv = smfsb.models.lv()
+    >>> import jax
+    >>> import jsmfsb.models
+    >>> lv = jsmfsb.models.lv()
     >>> stepLv = lv.stepGillespie()
-    >>> smfsb.simSample(10, [50, 100], 0, 30, stepLv)
+    >>> jsmfsb.simSample(jax.random.key(42), 10, lv.m, 0, 30, stepLv)
     """
     u = len(x0)
     keys = jax.random.split(key, n)
     mat = jl.map(lambda k: stepFun(k, x0, t0, deltat), keys)
     return mat
```

### Comparing `jsmfsb-0.0.2/src/jsmfsb/smfsbSbml.py` & `jsmfsb-0.0.3/src/jsmfsb/smfsbSbml.py`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.2/src/jsmfsb/spn.py` & `jsmfsb-0.0.3/src/jsmfsb/spn.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,22 +39,23 @@
 
         Returns
         -------
         A object of class Spn.
 
         Examples
         --------
-        >>> import smfsb
+        >>> import jsmfsb
+        >>> import jax
         >>> import jax.numpy as jnp
-        >>> sir = smfsb.Spn(["S", "I", "R"], ["S->I", "I->R"],
+        >>> sir = jsmfsb.Spn(["S", "I", "R"], ["S->I", "I->R"],
               [[1,1,0],[0,1,0]], [[0,2,0],[0,0,1]],
 	      lambda x, t: jnp.array([0.3*x[0]*x[1]/200, 0.1*x[1]]),
 	      [197, 3, 0])
-        >>> stepSir = sir.stepPTS()
-        >>> smfsb.simSample(10, sir.m, 0, 20, stepSir)
+        >>> stepSir = sir.stepGillespie()
+        >>> jsmfsb.simSample(jax.random.key(42), 10, sir.m, 0, 20, stepSir)
         """
         self.n = n # species names
         self.t = t # reaction names
         self.pre = jnp.array(pre).astype(jnp.float32)
         self.post = jnp.array(post).astype(jnp.float32)
         self.h = h # hazard function
         self.m = jnp.array(m).astype(jnp.float32) # initial marking
@@ -86,18 +87,19 @@
         represent the initial state and time, and ‘deltat’ represents the
         amount of time by which the process should be advanced. The
         function closure returns a vector representing the simulated state
         of the system at the new time.
 
         Examples
         --------
-        >>> import smfsb.models
-        >>> lv = smfsb.models.lv()
+        >>> import jsmfsb.models
+        >>> import jax
+        >>> lv = jsmfsb.models.lv()
         >>> stepLv = lv.stepGillespie()
-        >>> stepLv([50, 100], 0, 1)
+        >>> stepLv(jax.random.key(42), lv.m, 0, 1)
         """
         S = (self.post - self.pre).T
         u, v = S.shape
         @jit
         def advance(state):
             key, x, t = state
             h = self.h(x, t)
@@ -145,18 +147,19 @@
         ‘x0’ and ‘t0’ represent the initial state and time, and ‘deltat’
         represents the amount of time by which the process should be
         advanced. The function closure returns a vector representing the
         simulated state of the system at the new time.
 
         Examples
         --------
-        >>> import smfsb.models
-        >>> lv = smfsb.models.lv()
+        >>> import jsmfsb.models
+        >>> import jax
+        >>> lv = jsmfsb.models.lv()
         >>> stepLv = lv.stepCLE(0.001)
-        >>> stepLv([50, 100], 0, 1)
+        >>> stepLv(jax.random.key(42), lv.m, 0, 1)
         """
         S = (self.post - self.pre).T
         v = S.shape[1]
         sdt = np.sqrt(dt)
         @jit
         def advance(state):
             key, x, t = state
```

### Comparing `jsmfsb-0.0.2/.gitignore` & `jsmfsb-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.2/LICENSE` & `jsmfsb-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.2/pyproject.toml` & `jsmfsb-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jsmfsb"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Darren Wilkinson", email="darrenjwilkinson@btinternet.com" },
 ]
 description = "Python+JAX code relating to the textbook, Stochastic modelling for systems biology, third edition"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
@@ -24,10 +24,10 @@
 ]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/jsmfsb"]
 
 [project.urls]
 Homepage = "https://github.com/darrenjw/jax-smfsb"
-Documentation = "https://jsmfsb.readthedocs.io/"
+Documentation = "https://jax-smfsb.readthedocs.io/"
 Issues = "https://github.com/darrenjw/jax-smfsb/issues"
```

