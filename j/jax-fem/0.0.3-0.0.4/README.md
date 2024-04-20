# Comparing `tmp/jax-fem-0.0.3.tar.gz` & `tmp/jax_fem-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-fem-0.0.3.tar", last modified: Fri Mar  1 08:58:23 2024, max compression
+gzip compressed data, was "jax_fem-0.0.4.tar", last modified: Sat Apr 20 08:11:54 2024, max compression
```

## Comparing `jax-fem-0.0.3.tar` & `jax_fem-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 tianjuxue   (501) staff       (20)        0 2024-03-01 08:58:23.615468 jax-fem-0.0.3/
--rw-r--r--   0 tianjuxue   (501) staff       (20)    35149 2023-11-30 11:09:05.000000 jax-fem-0.0.3/LICENSE
--rw-r--r--   0 tianjuxue   (501) staff       (20)       49 2023-11-30 11:09:05.000000 jax-fem-0.0.3/MANIFEST.in
--rw-r--r--   0 tianjuxue   (501) staff       (20)     6842 2024-03-01 08:58:23.615359 jax-fem-0.0.3/PKG-INFO
--rw-r--r--   0 tianjuxue   (501) staff       (20)     6155 2024-02-15 07:31:35.000000 jax-fem-0.0.3/README.md
--rw-r--r--   0 tianjuxue   (501) staff       (20)        6 2023-11-30 11:09:05.000000 jax-fem-0.0.3/VERSION
-drwxr-xr-x   0 tianjuxue   (501) staff       (20)        0 2024-03-01 08:58:23.613400 jax-fem-0.0.3/jax_fem/
--rw-r--r--   0 tianjuxue   (501) staff       (20)      195 2024-02-22 06:39:19.000000 jax-fem-0.0.3/jax_fem/__init__.py
--rw-r--r--   0 tianjuxue   (501) staff       (20)     7315 2023-11-30 11:53:02.000000 jax-fem-0.0.3/jax_fem/autodiff_utils.py
--rw-r--r--   0 tianjuxue   (501) staff       (20)     7987 2023-12-10 08:19:07.000000 jax-fem-0.0.3/jax_fem/basis.py
--rw-r--r--   0 tianjuxue   (501) staff       (20)     4508 2023-11-30 11:09:05.000000 jax-fem-0.0.3/jax_fem/common.py
--rw-r--r--   0 tianjuxue   (501) staff       (20)    19067 2024-03-01 08:57:11.000000 jax-fem-0.0.3/jax_fem/fe.py
--rw-r--r--   0 tianjuxue   (501) staff       (20)     8203 2023-12-10 03:12:00.000000 jax-fem-0.0.3/jax_fem/generate_mesh.py
--rw-r--r--   0 tianjuxue   (501) staff       (20)      923 2023-11-30 11:09:05.000000 jax-fem-0.0.3/jax_fem/logger_setup.py
--rw-r--r--   0 tianjuxue   (501) staff       (20)    16855 2023-12-08 04:48:18.000000 jax-fem-0.0.3/jax_fem/mma.py
--rw-r--r--   0 tianjuxue   (501) staff       (20)    21071 2024-03-01 08:56:01.000000 jax-fem-0.0.3/jax_fem/problem.py
--rw-r--r--   0 tianjuxue   (501) staff       (20)    35154 2024-03-01 08:36:18.000000 jax-fem-0.0.3/jax_fem/solver.py
--rw-r--r--   0 tianjuxue   (501) staff       (20)     1808 2023-12-08 03:20:00.000000 jax-fem-0.0.3/jax_fem/utils.py
-drwxr-xr-x   0 tianjuxue   (501) staff       (20)        0 2024-03-01 08:58:23.615033 jax-fem-0.0.3/jax_fem.egg-info/
--rw-r--r--   0 tianjuxue   (501) staff       (20)     6842 2024-03-01 08:58:23.000000 jax-fem-0.0.3/jax_fem.egg-info/PKG-INFO
--rw-r--r--   0 tianjuxue   (501) staff       (20)      434 2024-03-01 08:58:23.000000 jax-fem-0.0.3/jax_fem.egg-info/SOURCES.txt
--rw-r--r--   0 tianjuxue   (501) staff       (20)        1 2024-03-01 08:58:23.000000 jax-fem-0.0.3/jax_fem.egg-info/dependency_links.txt
--rw-r--r--   0 tianjuxue   (501) staff       (20)        8 2024-03-01 08:58:23.000000 jax-fem-0.0.3/jax_fem.egg-info/top_level.txt
--rw-r--r--   0 tianjuxue   (501) staff       (20)       97 2023-11-30 11:09:05.000000 jax-fem-0.0.3/pyproject.toml
--rw-r--r--   0 tianjuxue   (501) staff       (20)      797 2024-03-01 08:58:23.615898 jax-fem-0.0.3/setup.cfg
-drwxr-xr-x   0 tianjuxue   (501) staff       (20)        0 2024-03-01 08:58:23.614697 jax-fem-0.0.3/tests/
--rw-r--r--   0 tianjuxue   (501) staff       (20)     4671 2023-11-30 11:09:05.000000 jax-fem-0.0.3/tests/test_autodiff_jvp_wrapper.py
+drwxr-xr-x   0 tianjuxue   (501) staff       (20)        0 2024-04-20 08:11:54.018318 jax_fem-0.0.4/
+-rw-r--r--   0 tianjuxue   (501) staff       (20)    35149 2023-11-30 11:09:05.000000 jax_fem-0.0.4/LICENSE
+-rw-r--r--   0 tianjuxue   (501) staff       (20)       49 2023-11-30 11:09:05.000000 jax_fem-0.0.4/MANIFEST.in
+-rw-r--r--   0 tianjuxue   (501) staff       (20)     6842 2024-04-20 08:11:54.018180 jax_fem-0.0.4/PKG-INFO
+-rw-r--r--   0 tianjuxue   (501) staff       (20)     6155 2024-02-15 07:31:35.000000 jax_fem-0.0.4/README.md
+-rw-r--r--   0 tianjuxue   (501) staff       (20)        6 2023-11-30 11:09:05.000000 jax_fem-0.0.4/VERSION
+drwxr-xr-x   0 tianjuxue   (501) staff       (20)        0 2024-04-20 08:11:54.014210 jax_fem-0.0.4/jax_fem/
+-rw-r--r--   0 tianjuxue   (501) staff       (20)      215 2024-04-20 08:10:13.000000 jax_fem-0.0.4/jax_fem/__init__.py
+-rw-r--r--   0 tianjuxue   (501) staff       (20)     7315 2023-11-30 11:53:02.000000 jax_fem-0.0.4/jax_fem/autodiff_utils.py
+-rw-r--r--   0 tianjuxue   (501) staff       (20)     7987 2023-12-10 08:19:07.000000 jax_fem-0.0.4/jax_fem/basis.py
+-rw-r--r--   0 tianjuxue   (501) staff       (20)     3966 2024-04-20 06:07:26.000000 jax_fem-0.0.4/jax_fem/common.py
+-rw-r--r--   0 tianjuxue   (501) staff       (20)    20172 2024-04-15 13:51:01.000000 jax_fem-0.0.4/jax_fem/fe.py
+-rw-r--r--   0 tianjuxue   (501) staff       (20)     8203 2023-12-10 03:12:00.000000 jax_fem-0.0.4/jax_fem/generate_mesh.py
+-rw-r--r--   0 tianjuxue   (501) staff       (20)      923 2023-11-30 11:09:05.000000 jax_fem-0.0.4/jax_fem/logger_setup.py
+-rw-r--r--   0 tianjuxue   (501) staff       (20)    16848 2024-04-20 06:14:26.000000 jax_fem-0.0.4/jax_fem/mma.py
+-rw-r--r--   0 tianjuxue   (501) staff       (20)    21741 2024-04-13 13:59:40.000000 jax_fem-0.0.4/jax_fem/problem.py
+-rw-r--r--   0 tianjuxue   (501) staff       (20)    25502 2024-04-20 08:05:58.000000 jax_fem-0.0.4/jax_fem/solver.py
+-rw-r--r--   0 tianjuxue   (501) staff       (20)     1808 2023-12-08 03:20:00.000000 jax_fem-0.0.4/jax_fem/utils.py
+drwxr-xr-x   0 tianjuxue   (501) staff       (20)        0 2024-04-20 08:11:54.017725 jax_fem-0.0.4/jax_fem.egg-info/
+-rw-r--r--   0 tianjuxue   (501) staff       (20)     6842 2024-04-20 08:11:53.000000 jax_fem-0.0.4/jax_fem.egg-info/PKG-INFO
+-rw-r--r--   0 tianjuxue   (501) staff       (20)      434 2024-04-20 08:11:53.000000 jax_fem-0.0.4/jax_fem.egg-info/SOURCES.txt
+-rw-r--r--   0 tianjuxue   (501) staff       (20)        1 2024-04-20 08:11:53.000000 jax_fem-0.0.4/jax_fem.egg-info/dependency_links.txt
+-rw-r--r--   0 tianjuxue   (501) staff       (20)        8 2024-04-20 08:11:53.000000 jax_fem-0.0.4/jax_fem.egg-info/top_level.txt
+-rw-r--r--   0 tianjuxue   (501) staff       (20)       97 2023-11-30 11:09:05.000000 jax_fem-0.0.4/pyproject.toml
+-rw-r--r--   0 tianjuxue   (501) staff       (20)      797 2024-04-20 08:11:54.018782 jax_fem-0.0.4/setup.cfg
+drwxr-xr-x   0 tianjuxue   (501) staff       (20)        0 2024-04-20 08:11:54.016963 jax_fem-0.0.4/tests/
+-rw-r--r--   0 tianjuxue   (501) staff       (20)     4671 2023-11-30 11:09:05.000000 jax_fem-0.0.4/tests/test_autodiff_jvp_wrapper.py
```

### Comparing `jax-fem-0.0.3/LICENSE` & `jax_fem-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jax-fem-0.0.3/PKG-INFO` & `jax_fem-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-fem
-Version: 0.0.3
+Version: 0.0.4
 Summary: GPU accelerated Finite element analysis package in JAX.
 Author: Tianju Xue
 Author-email: cetxue@ust.hk
 License: GPL-3.0 License
 Keywords: JAX,GPU,Python,Finite element analysis,Differentiable programming
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `jax-fem-0.0.3/README.md` & `jax_fem-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `jax-fem-0.0.3/jax_fem/autodiff_utils.py` & `jax_fem-0.0.4/jax_fem/autodiff_utils.py`

 * *Files identical despite different names*

### Comparing `jax-fem-0.0.3/jax_fem/basis.py` & `jax_fem-0.0.4/jax_fem/basis.py`

 * *Files identical despite different names*

### Comparing `jax-fem-0.0.3/jax_fem/common.py` & `jax_fem-0.0.4/jax_fem/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,17 @@
 import jax
 import numpy as onp
 import os
 import meshio
-import json
-import yaml
-
 import time
 from functools import wraps
 
 from jax_fem import logger
 
 
-def json_parse(json_filepath):
-    with open(json_filepath) as f:
-        args = json.load(f)
-    json_formatted_str = json.dumps(args, indent=4)
-    print(json_formatted_str)
-    return args
-
-
-def yaml_parse(yaml_filepath):
-    with open(yaml_filepath) as f:
-        args = yaml.load(f, Loader=yaml.FullLoader)
-        print("YAML parameters:")
-        # TODO: These are just default parameters
-        print(yaml.dump(args, default_flow_style=False))
-        print("These are default parameters")
-    return args
-
-
 def box_mesh(Nx, Ny, Nz, domain_x, domain_y, domain_z):
     dim = 3
     x = onp.linspace(0, domain_x, Nx + 1)
     y = onp.linspace(0, domain_y, Ny + 1)
     z = onp.linspace(0, domain_z, Nz + 1)
     xv, yv, zv = onp.meshgrid(x, y, z, indexing='ij')
     points_xyz = onp.stack((xv, yv, zv), axis=dim)
```

### Comparing `jax-fem-0.0.3/jax_fem/fe.py` & `jax_fem-0.0.4/jax_fem/fe.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,20 +6,17 @@
 import functools
 from dataclasses import dataclass
 from typing import Any, Callable, Optional, List, Union
 from jax_fem.common import timeit
 from jax_fem.generate_mesh import Mesh
 from jax_fem.basis import get_face_shape_vals_and_grads, get_shape_vals_and_grads
 # from jax_fem.autodiff_utils import jax_array_list_to_numpy_diff
-from jax.config import config
 from jax_fem import logger
 
 
-# config.update("jax_enable_x64", True)
-
 onp.set_printoptions(threshold=sys.maxsize,
                      linewidth=1000,
                      suppress=True,
                      precision=5)
 
 
 @dataclass
@@ -211,15 +208,23 @@
         node_inds_list = []
         vec_inds_list = []
         vals_list = []
         if dirichlet_bc_info is not None:
             location_fns, vecs, value_fns = dirichlet_bc_info
             assert len(location_fns) == len(value_fns) and len(value_fns) == len(vecs)
             for i in range(len(location_fns)):
-                node_inds = onp.argwhere(jax.vmap(location_fns[i])(self.mesh.points)).reshape(-1)
+                num_args = location_fns[i].__code__.co_argcount
+                if num_args == 1:
+                    location_fn = lambda point, ind: location_fns[i](point)
+                elif num_args == 2:
+                    location_fn = location_fns[i]
+                else:
+                    raise ValueError(f"Wrong number of arguments for location_fn: must be 1 or 2, get {num_args}")
+
+                node_inds = onp.argwhere(jax.vmap(location_fn)(self.mesh.points, np.arange(self.num_total_nodes))).reshape(-1)
                 vec_inds = onp.ones_like(node_inds, dtype=onp.int32) * vecs[i]
                 values = jax.vmap(value_fns[i])(self.mesh.points[node_inds].reshape(-1, self.dim)).reshape(-1)
                 node_inds_list.append(node_inds)
                 vec_inds_list.append(vec_inds)
                 vals_list.append(values)
         return node_inds_list, vec_inds_list, vals_list
 
@@ -267,40 +272,51 @@
 
     def get_boundary_conditions_inds(self, location_fns):
         """Given location functions, compute which faces satisfy the condition.
 
         Parameters
         ----------
         location_fns : List[Callable]
-            Callable: a function that inputs a point (ndarray) and returns if the point satisfies the location condition
+            Callable: a location function that inputs a point (ndarray) and returns if the point satisfies the location condition
                       e.g., lambda x: np.isclose(x[0], 0.)
+                      If this location function takes 2 arguments, then the first is point and the second is index.
+                      e.g., lambda x, ind: np.isclose(x[0], 0.) & np.isin(ind, np.array([1, 3, 10]))
 
         Returns
         -------
         boundary_inds_list : List[onp.ndarray]
             (num_selected_faces, 2)
             boundary_inds_list[k][i, 0] returns the global cell index of the ith selected face of boundary subset k
             boundary_inds_list[k][i, 1] returns the local face index of the ith selected face of boundary subset k
         """
         # TODO: assume this works for all variables, and return the same result
         cell_points = onp.take(self.points, self.cells, axis=0)  # (num_cells, num_nodes, dim)
         cell_face_points = onp.take(cell_points, self.face_inds, axis=1)  # (num_cells, num_faces, num_face_nodes, dim)
+        cell_face_inds = onp.take(self.cells, self.face_inds, axis=1) # (num_cells, num_faces, num_face_nodes)
         boundary_inds_list = []
         if location_fns is not None:
             for i in range(len(location_fns)):
-                vmap_location_fn = jax.vmap(location_fns[i])
-
-                def on_boundary(cell_points):
-                    boundary_flag = vmap_location_fn(cell_points)
+                num_args = location_fns[i].__code__.co_argcount
+                if num_args == 1:
+                    location_fn = lambda point, ind: location_fns[i](point)
+                elif num_args == 2:
+                    location_fn = location_fns[i]
+                else:
+                    raise ValueError(f"Wrong number of arguments for location_fn: must be 1 or 2, get {num_args}")
+
+                vmap_location_fn = jax.vmap(location_fn)
+                def on_boundary(cell_points, cell_inds):
+                    boundary_flag = vmap_location_fn(cell_points, cell_inds)
                     return onp.all(boundary_flag)
 
                 vvmap_on_boundary = jax.vmap(jax.vmap(on_boundary))
-                boundary_flags = vvmap_on_boundary(cell_face_points)
+                boundary_flags = vvmap_on_boundary(cell_face_points, cell_face_inds)
                 boundary_inds = onp.argwhere(boundary_flags)  # (num_selected_faces, 2)
                 boundary_inds_list.append(boundary_inds)
+
         return boundary_inds_list
 
     def convert_from_dof_to_quad(self, sol):
         """Obtain quad values from nodal solution
 
         Parameters
         ----------
@@ -343,15 +359,14 @@
     def sol_to_grad(self, sol):
         """Obtain solution gradient from nodal solution
 
         Parameters
         ----------
         sol : np.DeviceArray
             (num_total_nodes, vec)
-        index : int
 
         Returns
         -------
         u_grads : np.DeviceArray
             (num_cells, num_quads, vec, dim)
         """
         # (num_cells, 1, num_nodes, vec, 1) * (num_cells, num_quads, num_nodes, 1, dim) -> (num_cells, num_quads, num_nodes, vec, dim)
```

### Comparing `jax-fem-0.0.3/jax_fem/generate_mesh.py` & `jax_fem-0.0.4/jax_fem/generate_mesh.py`

 * *Files identical despite different names*

### Comparing `jax-fem-0.0.3/jax_fem/logger_setup.py` & `jax_fem-0.0.4/jax_fem/logger_setup.py`

 * *Files identical despite different names*

### Comparing `jax-fem-0.0.3/jax_fem/mma.py` & `jax_fem-0.0.4/jax_fem/mma.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import jax
 import jax.numpy as jnp
 from jax import jit, grad, random, jacfwd, value_and_grad
 from functools import partial
 import time
 import scipy
 
-from jax.config import config
+from jax import config
 config.update("jax_enable_x64", True)
 
 
 def compute_filter_kd_tree(fe):
     """This function is created by Tianju. Not from the original code.
     We use k-d tree algorithm to compute the filter.
     """
```

### Comparing `jax-fem-0.0.3/jax_fem/problem.py` & `jax_fem-0.0.4/jax_fem/problem.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,15 +214,21 @@
             pushfwd = functools.partial(jax.jvp, f, (x, ))
             basis = np.eye(len(x.reshape(-1)), dtype=x.dtype).reshape(-1, *x.shape)
             y, jac = jax.vmap(pushfwd, out_axes=(None, -1))((basis, ))
             return y, jac
 
         def get_kernel_fn_cell():
             def kernel(cell_sol_flat, physical_quad_points, cell_shape_grads, cell_JxW, cell_v_grads_JxW, *cell_internal_vars):
+                """
+                universal_kernel should be able to cover all situations (including mass_kernel and laplace_kernel).
+                mass_kernel and laplace_kernel are from legacy JAX-FEM. They can still be used, but not mandatory.
+                """
 
+                # TODO: If there is no kernel map, returning 0. is not a good choice. 
+                # Return a zero array with proper shape will be better.
                 if hasattr(self, 'get_mass_map'):
                     mass_kernel = self.get_mass_kernel(self.get_mass_map())
                     mass_val = mass_kernel(cell_sol_flat, physical_quad_points, cell_JxW, *cell_internal_vars)
                 else:
                     mass_val = 0.
 
                 if hasattr(self, 'get_tensor_map'):
@@ -245,24 +251,28 @@
                 kernel_partial = lambda cell_sol_flat: kernel(cell_sol_flat, *args)
                 return value_and_jacfwd(kernel_partial, cell_sol_flat)  # kernel(cell_sol_flat, *args), jax.jacfwd(kernel)(cell_sol_flat, *args)
 
             return kernel, kernel_jac
 
         def get_kernel_fn_face(ind):
             def kernel(cell_sol_flat, physical_surface_quad_points, face_shape_vals, face_shape_grads, face_nanson_scale, *cell_internal_vars_surface):
+                """
+                universal_kernel should be able to cover all situations (including surface_kernel).
+                surface_kernel is from legacy JAX-FEM. It can still be used, but not mandatory.
+                """
                 if hasattr(self, 'get_surface_maps'):
                     surface_kernel = self.get_surface_kernel(self.get_surface_maps()[ind])
                     surface_val = surface_kernel(cell_sol_flat, physical_surface_quad_points, face_shape_vals,
                         face_shape_grads, face_nanson_scale, *cell_internal_vars_surface)
                 else:
                     surface_val = 0.
 
                 if hasattr(self, 'get_universal_kernels_surface'):
-                    surface_kernel = self.get_universal_kernels_surface()[ind]
-                    universal_val = surface_kernel(cell_sol_flat, physical_surface_quad_points, face_shape_vals,
+                    universal_kernel = self.get_universal_kernels_surface()[ind]
+                    universal_val = universal_kernel(cell_sol_flat, physical_surface_quad_points, face_shape_vals,
                         face_shape_grads, face_nanson_scale, *cell_internal_vars_surface)
                 else:
                     universal_val = 0.
 
                 return surface_val + universal_val
 
             def kernel_jac(cell_sol_flat, *args):
```

### Comparing `jax-fem-0.0.3/jax_fem/solver.py` & `jax_fem-0.0.4/jax_fem/solver.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import time
 
 # petsc4py.init()
 from petsc4py import PETSc
 
 from jax_fem import logger
 
-from jax.config import config
+from jax import config
 config.update("jax_enable_x64", True)
 
 ################################################################################
 # PETSc linear solver or JAX linear solver
 
 def petsc_solve(A, b, ksp_type, pc_type):
     rhs = PETSc.Vec().createSeq(len(b))
@@ -40,27 +40,26 @@
     err = np.linalg.norm(y.getArray() - rhs.getArray())
     logger.debug(f"PETSc linear solve res = {err}")
     # assert err < 0.1, f"PETSc linear solver failed to converge, err = {err}"
 
     return x.getArray()
 
 
-def jax_solve(problem, A_fn, b, x0, precond: bool, pc_matrix=None):
+def jax_solve(problem, A_fn, b, x0, precond, pc_matrix=None):
     """Solves the equilibrium equation using a JAX solver.
     Is fully traceable and runs on GPU.
 
     Parameters
     ----------
     precond
         Whether to calculate the preconditioner or not
     pc_matrix
         The matrix to use as preconditioner
     """
-    pc = get_jacobi_precond(
-        jacobi_preconditioner(problem)) if precond else None
+    pc = get_jacobi_precond(jacobi_preconditioner(problem)) if precond else None
     x, info = jax.scipy.sparse.linalg.bicgstab(A_fn,
                                                b,
                                                x0=x0,
                                                M=pc,
                                                tol=1e-10,
                                                atol=1e-10,
                                                maxiter=10000)
@@ -240,44 +239,22 @@
 def test_jacobi_precond(problem, jacobi, A_fn):
     """Not working, needs refactoring
     """
     num_total_dofs = problem.num_total_nodes * problem.vec
     for ind in range(500):
         test_vec = np.zeros(num_total_dofs)
         test_vec = test_vec.at[ind].set(1.)
-        logger.debug(
-            f"{A_fn(test_vec)[ind]}, {jacobi[ind]}, ratio = {A_fn(test_vec)[ind]/jacobi[ind]}"
-        )
+        logger.debug(f"{A_fn(test_vec)[ind]}, {jacobi[ind]}, ratio = {A_fn(test_vec)[ind]/jacobi[ind]}")
 
     logger.debug(f"test jacobi preconditioner")
-    logger.debug(
-        f"np.min(jacobi) = {np.min(jacobi)}, np.max(jacobi) = {np.max(jacobi)}"
-    )
+    logger.debug(f"np.min(jacobi) = {np.min(jacobi)}, np.max(jacobi) = {np.max(jacobi)}")
     logger.debug(f"finish jacobi preconditioner")
 
 
-# def linear_guess_solve(problem, A_fn, precond, use_petsc):
-#     """To be deprecated
-#     """
-#     logger.debug(f"Linear guess solve...")
-
-#     # TODO: b set to be pure zero may not be good...
-#     # b = np.zeros((problem.num_total_nodes, problem.vec))
-#     # b = problem.body_force + problem.neumann
-#     b = np.zeros(problem.num_total_dofs_all_vars)
-
-#     b = assign_bc(b, problem)
-#     if use_petsc:
-#         dofs = petsc_solve(A_fn, b, 'bcgsl', 'ilu')
-#     else:
-#         dofs = jax_solve(problem, A_fn, b, b, precond)
-#     return dofs
-
-
-def linear_incremental_solver(problem, res_vec, A_fn, dofs, precond, use_petsc, petsc_options):
+def linear_incremental_solver(problem, res_vec, A_fn, dofs, precond, use_petsc, petsc_options, line_search_flag):
     """Lift solver
     """
     logger.debug(f"Solving linear system with lift solver...")
     b = -res_vec
 
     if use_petsc:
         if petsc_options is not None:
@@ -290,22 +267,26 @@
     else:
         # x0 will always be correct at boundary locations
         x0_1 = assign_bc(np.zeros_like(b), problem)
         x0_2 = copy_bc(dofs, problem)
         x0 = x0_1 - x0_2
         inc = jax_solve(problem, A_fn, b, x0, precond)
 
-    dofs = dofs + inc
-
-    # dofs = line_search(problem, dofs, inc)
+    if line_search_flag:
+        dofs = line_search(problem, dofs, inc)
+    else:
+        dofs = dofs + inc
 
     return dofs
 
 
 def line_search(problem, dofs, inc):
+    """
+    TODO: This is useful for finite deformation plasticity.
+    """
     res_fn = problem.compute_residual
     res_fn = get_flatten_fn(res_fn, problem)
     res_fn = apply_bc(res_fn, problem)
 
     def res_norm_fn(alpha):
         res_vec = res_fn(dofs + alpha*inc)
         return np.linalg.norm(res_vec)
@@ -361,15 +342,15 @@
                 A.zeroRows(row_inds)
     else:
         A = row_elimination(compute_linearized_residual, problem)
 
     return A
 
 
-def solver_row_elimination(problem, linear, precond, initial_guess, use_petsc, petsc_options):
+def solver_row_elimination(problem, linear, precond, initial_guess, use_petsc, petsc_options, line_search_flag):
     """The solver imposes Dirichlet B.C. with "row elimination" method.
 
     Some memo:
 
     res(u) = D*r(u) + (I - D)u - u_b
     D = [[1 0 0 0]
          [0 1 0 0]
@@ -398,300 +379,48 @@
         A_fn = get_A_fn(problem, use_petsc)
         return res_vec, A_fn
 
     if linear:
         # We might not need this linear solver as well
         dofs = assign_bc(dofs, problem)
         res_vec, A_fn = newton_update_helper(dofs)
-        dofs = linear_incremental_solver(problem, res_vec, A_fn, dofs, precond, use_petsc, petsc_options)
+        dofs = linear_incremental_solver(problem, res_vec, A_fn, dofs, precond, use_petsc, petsc_options, line_search_flag)
         res_vec, A_fn = newton_update_helper(dofs)
         res_val = np.linalg.norm(res_vec)
         logger.debug(f"Linear solve, res l_2 = {res_val}")
 
     else:
-        # if initial_guess is None:
-        #     res_vec, A_fn = newton_update_helper(dofs)
-        #     # TODO: investigate the advantage of the guess solve, do we need it? For plasticity?
-        #     # Is this linear_guess_solve really being useful??
-        #     dofs = linear_guess_solve(problem, A_fn, precond, use_petsc)
-        # else:
-        #     dofs = initial_guess.reshape(-1)
-
         if initial_guess is not None:
             dofs = jax.flatten_util.ravel_pytree(initial_guess)[0]
 
         res_vec, A_fn = newton_update_helper(dofs)
         res_val = np.linalg.norm(res_vec)
         logger.debug(f"Before, res l_2 = {res_val}")
         tol = 1e-6
         while res_val > tol:
-            dofs = linear_incremental_solver(problem, res_vec, A_fn, dofs, precond, use_petsc, petsc_options)
+            dofs = linear_incremental_solver(problem, res_vec, A_fn, dofs, precond, use_petsc, petsc_options, line_search_flag)
             res_vec, A_fn = newton_update_helper(dofs)
             # test_jacobi_precond(problem, jacobi_preconditioner(problem, dofs), A_fn)
             res_val = np.linalg.norm(res_vec)
             logger.debug(f"res l_2 = {res_val}")
 
     assert np.all(np.isfinite(res_val)), f"res_val contains NaN, stop the program!"
-
     assert np.all(np.isfinite(dofs)), f"dofs contains NaN, stop the program!"
 
     sol_list = problem.unflatten_fn_sol_list(dofs)
     end = time.time()
     solve_time = end - start
     logger.info(f"Solve took {solve_time} [s]")
     logger.debug(f"max of dofs = {np.max(dofs)}")
     logger.debug(f"min of dofs = {np.min(dofs)}")
 
     return sol_list
 
 
 ################################################################################
-# Lagrangian multiplier solver
-
-# TODO: Old version, not working for multi-physics problems. Requires refactoring. 
-
-def aug_dof_w_zero_bc(problem, dofs):
-    aug_size = 0
-    for i in range(len(problem.node_inds_list)):
-        aug_size += len(problem.node_inds_list[i])
-    for i in range(len(problem.p_node_inds_list_A)):
-        aug_size += len(problem.p_node_inds_list_A[i])
-    return np.hstack((dofs, np.zeros(aug_size)))
-
-
-def aug_dof_w_bc(problem, dofs, p_num_eps):
-    aug_d = np.array([])
-    for i in range(len(problem.node_inds_list)):
-        aug_d = np.hstack((aug_d, p_num_eps * problem.vals_list[i]))
-    for i in range(len(problem.p_node_inds_list_A)):
-        aug_d = np.hstack(
-            (aug_d, np.zeros(len(problem.p_node_inds_list_A[i]))))
-    return np.hstack((dofs, aug_d))
-
-
-def linear_guess_solve_lm(problem, A_aug, p_num_eps, use_petsc):
-    b = (problem.body_force + problem.neumann).reshape(-1)
-    b_aug = aug_dof_w_bc(problem, b, p_num_eps)
-    if use_petsc:
-        dofs_aug = petsc_solve(A_aug, b_aug, 'minres', 'none')
-    else:
-        x0 = np.zeros((problem.num_total_nodes, problem.vec))
-        x0 = assign_bc(x0, problem)
-        x0 = aug_dof_w_zero_bc(problem, x0)
-        dofs_aug = jax_solve(problem, A_aug, b_aug, x0, None)
-    return dofs_aug
-
-
-def linear_incremental_solver_lm(problem, res_vec_aug, A_aug, dofs_aug,
-                                 p_num_eps, use_petsc):
-    b_aug = -res_vec_aug
-    if use_petsc:
-        inc_aug = petsc_solve(A_aug, b_aug, 'minres', 'none')
-    else:
-        inc_aug = jax_solve(problem, A_aug, b_aug, None, None)
-    dofs_aug = dofs_aug + inc_aug
-    return dofs_aug
-
-
-def compute_residual_lm(problem, res_vec, dofs_aug, p_num_eps):
-    """Some memo here
-    Saddle point problem energy function: L(u, lmbda) = E(u) + lmbda*(u - u0)
-    with dL/d(u, lmbda) = res_vec_aug and dE/du = res_vec
-    """
-    d_splits = np.cumsum(np.array([len(x) for x in problem.node_inds_list])).tolist()
-    p_splits = np.cumsum(np.array([len(x) for x in problem.p_node_inds_list_A])).tolist()
-
-    d_lmbda_len = d_splits[-1] if len(d_splits) > 0 else 0
-    p_lmbda_len = p_splits[-1] if len(p_splits) > 0 else 0
-
-    def get_Lagrangian():
-
-        def split_lamda(lmbda):
-            d_lmbda = lmbda[:d_lmbda_len]
-            p_lmbda = lmbda[d_lmbda_len:]
-            d_lmbda_split = np.split(d_lmbda, d_splits)
-            p_lmbda_split = np.split(p_lmbda, p_splits)
-            return d_lmbda_split, p_lmbda_split
-
-        # @jax.jit
-        def Lagrangian_fn(dofs_aug):
-            dofs, lmbda = dofs_aug[:problem.num_total_dofs], dofs_aug[problem.num_total_dofs:]
-            sol = dofs.reshape((problem.num_total_nodes, problem.vec))
-            d_lmbda_split, p_lmbda_split = split_lamda(lmbda)
-            lag = 0.
-            for i in range(len(problem.node_inds_list)):
-                lag += np.sum(d_lmbda_split[i] *
-                    (sol[problem.node_inds_list[i], problem.vec_inds_list[i]] - problem.vals_list[i]))
-
-            for i in range(len(problem.p_node_inds_list_A)):
-                lag += np.sum(p_lmbda_split[i] *
-                              (sol[problem.p_node_inds_list_A[i], problem.p_vec_inds_list[i]] -
-                               sol[problem.p_node_inds_list_B[i], problem.p_vec_inds_list[i]]))
-            return p_num_eps * lag
-
-        return Lagrangian_fn
-
-    Lagrangian_fn = get_Lagrangian()
-    A_fn = jax.grad(Lagrangian_fn)
-    res_vec_1 = A_fn(dofs_aug)
-    res_vec_2 = aug_dof_w_zero_bc(problem, res_vec)
-    res_vec_aug = res_vec_1 + res_vec_2
-
-    return res_vec_aug
-
-
-def get_A_fn_and_res_aug(problem, dofs_aug, res_vec, p_num_eps, use_petsc):
-
-    def symmetry(I, J, V):
-        I_sym = onp.hstack((I, J))
-        J_sym = onp.hstack((J, I))
-        V_sym = onp.hstack((V, V))
-        return I_sym, J_sym, V_sym
-
-    I_d = onp.array([])
-    J_d = onp.array([])
-    V_d = onp.array([])
-    group_index = problem.num_total_dofs
-    for i in range(len(problem.node_inds_list)):
-        group_size = len(problem.node_inds_list[i])
-        I_d = onp.hstack((I_d, problem.vec * problem.node_inds_list[i] +
-                          problem.vec_inds_list[i]))
-        J_d = onp.hstack((J_d, group_index + onp.arange(group_size)))
-        V_d = onp.hstack((V_d, p_num_eps * onp.ones(group_size)))
-        group_index += group_size
-    I_d_sym, J_d_sym, V_d_sym = symmetry(I_d, J_d, V_d)
-
-    I_p = onp.array([])
-    J_p = onp.array([])
-    V_p = onp.array([])
-    for i in range(len(problem.p_node_inds_list_A)):
-        group_size = len(problem.p_node_inds_list_A[i])
-        I_p = onp.hstack((I_p, problem.vec * problem.p_node_inds_list_A[i] +
-                          problem.p_vec_inds_list[i]))
-        J_p = onp.hstack((J_p, group_index + onp.arange(group_size)))
-        V_p = onp.hstack((V_p, p_num_eps * onp.ones(group_size)))
-        I_p = onp.hstack((I_p, problem.vec * problem.p_node_inds_list_B[i] +
-                          problem.p_vec_inds_list[i]))
-        J_p = onp.hstack((J_p, group_index + onp.arange(group_size)))
-        V_p = onp.hstack((V_p, -p_num_eps * onp.ones(group_size)))
-        group_index += group_size
-    I_p_sym, J_p_sym, V_p_sym = symmetry(I_p, J_p, V_p)
-
-    I = onp.hstack((problem.I, I_d_sym, I_p_sym))
-    J = onp.hstack((problem.J, J_d_sym, J_p_sym))
-    V = onp.hstack((problem.V, V_d_sym, V_p_sym))
-
-    logger.debug(f"Aug - Creating sparse matrix with scipy...")
-    A_sp_scipy_aug = scipy.sparse.csc_array((V, (I, J)), shape=(group_index, group_index))
-    # logger.info(f"Aug - Creating sparse matrix from scipy using JAX BCOO...")
-    A_sp_aug = BCOO.from_scipy_sparse(A_sp_scipy_aug).sort_indices()
-
-    # logger.info(f"Aug - Global sparse matrix takes about {A_sp_aug.data.shape[0]*8*3/2**30} G memory to store.")
-
-    # TODO: Potential bug
-    # Used only in jacobi_preconditioner
-    # problem.A_sp_scipy = A_sp_scipy_aug
-
-    def compute_linearized_residual(dofs_aug):
-        return A_sp_aug @ dofs_aug
-
-    if use_petsc:
-
-        A = PETSc.Mat().createAIJ(size=A_sp_scipy_aug.shape,
-                                  csr=(A_sp_scipy_aug.indptr.astype(PETSc.IntType, copy=False),
-                                       A_sp_scipy_aug.indices.astype(PETSc.IntType, copy=False),
-                                       A_sp_scipy_aug.data))
-
-        # A_aug = PETSc.Mat().createAIJ(size=A_sp_scipy_aug.shape,
-        #                               csr=(A_sp_scipy_aug.indptr,
-        #                                    A_sp_scipy_aug.indices,
-        #                                    A_sp_scipy_aug.data))
-    else:
-        A_aug = compute_linearized_residual
-
-    res_vec_aug = compute_residual_lm(problem, res_vec, dofs_aug, p_num_eps)
-
-    return A_aug, res_vec_aug
-
-
-def solver_lagrange_multiplier(problem, linear, use_petsc=True):
-    """The solver imposes Dirichlet B.C. and periodic B.C. with lagrangian multiplier method.
-
-    The global matrix is of the form
-    [A   B
-     B^T 0]
-    JAX built solver gmres and bicgstab sometimes fail to solve such a system.
-    PESTc solver minres seems to work.
-    TODO: explore which solver in PESTc is the best, and which preconditioner should be used.
-    Update: It seems that petsc_options={'ksp_type': 'tfqmr', 'pc_type': 'ilu'} works better.
-
-    Reference:
-    https://ethz.ch/content/dam/ethz/special-interest/baug/ibk/structural-mechanics-dam/education/femI/Presentation.pdf
-    """
-    logger.info(
-        f"Calling the lagrange multiplier solver for imposing Dirichlet B.C. and periodic B.C."
-    )
-    logger.info("Start timing")
-    start = time.time()
-    sol_shape = (problem.num_total_nodes, problem.vec)
-    dofs = np.zeros(sol_shape).reshape(-1)
-
-    # Ad-hoc parameter to get a better conditioned global matrix. Not useful for PETSc solver.
-    if hasattr(problem, 'p_num_eps'):
-        p_num_eps = problem.p_num_eps
-    else:
-        p_num_eps = 1.
-
-    if not use_petsc:
-        logger.info(
-            f"Setting p_num_eps = {p_num_eps}. If periodic B.C. fails to be applied, consider modifying this parameter."
-        )
-
-    def newton_update_helper(dofs_aug):
-        res_vec = problem.newton_update(
-            dofs_aug[:problem.num_total_dofs].reshape(sol_shape)).reshape(-1)
-        A_aug, res_vec_aug = get_A_fn_and_res_aug(problem, dofs_aug, res_vec,
-                                                  p_num_eps, use_petsc)
-        return res_vec_aug, A_aug
-
-    if linear:
-        # If we know the problem is linear, this way of solving seems faster.
-        dofs = assign_bc(dofs, problem)
-        dofs_aug = aug_dof_w_zero_bc(problem, dofs)
-        res_vec_aug, A_aug = newton_update_helper(dofs_aug)
-        dofs_aug = linear_incremental_solver_lm(problem, res_vec_aug, A_aug,
-                                                dofs_aug, p_num_eps, use_petsc)
-    else:
-        dofs_aug = aug_dof_w_zero_bc(problem, dofs)
-        res_vec_aug, A_aug = newton_update_helper(dofs_aug)
-        dofs_aug = linear_guess_solve_lm(problem, A_aug, p_num_eps, use_petsc)
-
-        res_vec_aug, A_aug = newton_update_helper(dofs_aug)
-        res_val = np.linalg.norm(res_vec_aug)
-        logger.debug(f"Before, res l_2 = {res_val}")
-        tol = 1e-6
-        while res_val > tol:
-            dofs_aug = linear_incremental_solver_lm(problem, res_vec_aug,
-                                                    A_aug, dofs_aug, p_num_eps,
-                                                    use_petsc)
-            res_vec_aug, A_aug = newton_update_helper(dofs_aug)
-            res_val = np.linalg.norm(res_vec_aug)
-            logger.debug(f"res l_2 dofs_aug = {res_val}")
-
-    sol = dofs_aug[:problem.num_total_dofs].reshape(sol_shape)
-    end = time.time()
-    solve_time = end - start
-    logger.info(f"Solve took {solve_time} [s]")
-    logger.debug(f"max of sol = {np.max(sol)}")
-    logger.debug(f"min of sol = {np.min(sol)}")
-
-    return sol
-
-
-################################################################################
 # Dynamic relaxation solver
 
 def assembleCSR(problem, dofs):
     sol_list = problem.unflatten_fn_sol_list(dofs)
     problem.newton_update(sol_list)
    
     A_sp_scipy = scipy.sparse.csr_array((problem.V, (problem.I, problem.J)),
@@ -871,31 +600,32 @@
 
 def solver(problem,
            linear=False,
            precond=True,
            initial_guess=None,
            use_petsc=False,
            petsc_options=None,
-           lagrangian_solver=False):
+           lagrangian_solver=False,
+           line_search_flag=False):
     """periodic B.C. is a special form of adding a linear constraint.
     Lagrange multiplier seems to be convenient to impose this constraint.
     """
     # TODO: print platform jax.lib.xla_bridge.get_backend().platform
     # and suggest PETSc or jax solver
     if lagrangian_solver:
         assert False, f"Lagrangian multiplier solver needs refactoring: Not working for now."
         return solver_lagrange_multiplier(problem, linear, use_petsc)
     else:
-        return solver_row_elimination(problem, linear, precond, initial_guess, use_petsc, petsc_options)
+        return solver_row_elimination(problem, linear, precond, initial_guess, use_petsc, petsc_options, line_search_flag)
 
 
 ################################################################################
 # Implicit differentiation with the adjoint method
 
-def implicit_vjp(problem, sol_list, params, v_list, use_petsc):
+def implicit_vjp(problem, sol_list, params, v_list, use_petsc_adjoint, petsc_options_adjoint):
 
     def constraint_fn(dofs, params):
         """c(u, p)
         """
         problem.set_params(params)
         res_fn = problem.compute_residual
         res_fn = get_flatten_fn(res_fn, problem)
@@ -934,54 +664,76 @@
             val, = f_vjp(v_list)
             return val
 
         return vjp_linear_fn
 
     problem.set_params(params)
     problem.newton_update(sol_list)
-    A_fn = get_A_fn(problem, use_petsc)
+    A_fn = get_A_fn(problem, use_petsc_adjoint)
 
     v_vec = jax.flatten_util.ravel_pytree(v_list)[0]
 
-    if use_petsc:
+    if use_petsc_adjoint:
         A_transpose = A_fn.transpose()
 
         # Remark: Eliminating rows seems to make A better conditioned.
         # If Dirichlet B.C. is part of the design variable, the following should NOT be implemented.
         # for i in range(len(problem.node_inds_list)):
         #     row_inds = onp.array(problem.node_inds_list[i]*problem.vec + problem.vec_inds_list[i], dtype=onp.int32)
         #     A_transpose.zeroRows(row_inds)
         # v = assign_zeros_bc(v, problem)
 
-        adjoint_vec = petsc_solve(A_transpose, v_vec, 'minres', 'ilu')
+        if petsc_options_adjoint is not None:
+            ksp_type = petsc_options_adjoint['ksp_type']
+            pc_type = petsc_options_adjoint['pc_type']
+        else:
+            ksp_type = 'minres'
+            pc_type = 'ilu'
+
+        adjoint_vec = petsc_solve(A_transpose, v_vec, ksp_type, pc_type)
     else:
         dofs = jax.flatten_util.ravel_pytree(sol_list)[0]
         adjoint_linear_fn = get_vjp_contraint_fn_dofs(dofs)
         adjoint_vec = jax_solve(problem, adjoint_linear_fn, v_vec, None, True)
 
     vjp_linear_fn = get_vjp_contraint_fn_params(params, sol_list)
     vjp_result = vjp_linear_fn(problem.unflatten_fn_sol_list(adjoint_vec))
     vjp_result = jax.tree_map(lambda x: -x, vjp_result)
 
     return vjp_result
 
 
-def ad_wrapper(problem, linear=False, use_petsc=False):
-
+def ad_wrapper(problem, linear=False, use_petsc=False, petsc_options=None, use_petsc_adjoint=False, petsc_options_adjoint=None):
+    """
+    Attributes
+    ----------
+    problem : Problem object
+        finite element problem instance
+    linear : bool   
+        if forward problem is linear (adjoint problem is alwasy linear, no need to specify)
+    use_petsc: bool
+        if PETSc solver should be called to solve the linear system for the forward problem
+    petsc_options: dic   
+        PETSc solver options specified by user for the forward problem
+    use_petsc_adjoint: bool
+        if PETSc solver should be called to solve the linear system for the adjoint problem
+    petsc_options_adjoint: dic   
+        PETSc solver options specified by user for the adjoint problem             
+    """
     @jax.custom_vjp
     def fwd_pred(params):
         problem.set_params(params)
-        sol_list = solver(problem, linear=linear, use_petsc=use_petsc)
+        sol_list = solver(problem, linear=linear, use_petsc=use_petsc, petsc_options=petsc_options)
         return sol_list
 
     def f_fwd(params):
         sol_list = fwd_pred(params)
         return sol_list, (params, sol_list)
 
     def f_bwd(res, v):
         logger.info("Running backward and solving the adjoint problem...")
         params, sol_list = res
-        vjp_result = implicit_vjp(problem, sol_list, params, v, use_petsc)
+        vjp_result = implicit_vjp(problem, sol_list, params, v, use_petsc_adjoint, petsc_options_adjoint)
         return (vjp_result, )
 
     fwd_pred.defvjp(f_fwd, f_bwd)
     return fwd_pred
```

### Comparing `jax-fem-0.0.3/jax_fem/utils.py` & `jax_fem-0.0.4/jax_fem/utils.py`

 * *Files identical despite different names*

### Comparing `jax-fem-0.0.3/jax_fem.egg-info/PKG-INFO` & `jax_fem-0.0.4/jax_fem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-fem
-Version: 0.0.3
+Version: 0.0.4
 Summary: GPU accelerated Finite element analysis package in JAX.
 Author: Tianju Xue
 Author-email: cetxue@ust.hk
 License: GPL-3.0 License
 Keywords: JAX,GPU,Python,Finite element analysis,Differentiable programming
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `jax-fem-0.0.3/setup.cfg` & `jax_fem-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = jax-fem
-version = 0.0.3
+version = 0.0.4
 author = Tianju Xue
 author_email = cetxue@ust.hk
 description = GPU accelerated Finite element analysis package in JAX.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = JAX, GPU, Python, Finite element analysis, Differentiable programming
 license = GPL-3.0 License
```

### Comparing `jax-fem-0.0.3/tests/test_autodiff_jvp_wrapper.py` & `jax_fem-0.0.4/tests/test_autodiff_jvp_wrapper.py`

 * *Files identical despite different names*

