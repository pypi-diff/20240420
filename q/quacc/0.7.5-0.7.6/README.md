# Comparing `tmp/quacc-0.7.5.tar.gz` & `tmp/quacc-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quacc-0.7.5.tar", last modified: Tue Apr 16 16:09:27 2024, max compression
+gzip compressed data, was "quacc-0.7.6.tar", last modified: Sat Apr 20 17:25:13 2024, max compression
```

## Comparing `quacc-0.7.5.tar` & `quacc-0.7.6.tar`

### file list

```diff
@@ -1,178 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.515679 quacc-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-16 16:07:28.000000 quacc-0.7.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-16 16:07:28.000000 quacc-0.7.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-04-16 16:09:27.515679 quacc-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-16 16:07:28.000000 quacc-0.7.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-16 16:07:28.000000 quacc-0.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 16:09:27.515679 quacc-0.7.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.479679 quacc-0.7.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.483679 quacc-0.7.5/src/quacc/
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.487679 quacc-0.7.5/src/quacc/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/_cli/quacc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.487679 quacc-0.7.5/src/quacc/atoms/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/atoms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/atoms/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/atoms/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/atoms/deformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/atoms/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/atoms/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.487679 quacc-0.7.5/src/quacc/calculators/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.487679 quacc-0.7.5/src/quacc/calculators/espresso/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17249 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/espresso.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.491679 quacc-0.7.5/src/quacc/calculators/espresso/presets/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/esm_metal_slab_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/esm_metal_slab_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/metal_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/metal_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/molecule_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/semiconductors_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/semiconductors_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10583 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/espresso/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.491679 quacc-0.7.5/src/quacc/calculators/qchem/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/qchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/qchem/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/qchem/params.py
--rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/qchem/qchem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/qchem/qchem_custodian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.491679 quacc-0.7.5/src/quacc/calculators/vasp/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.491679 quacc-0.7.5/src/quacc/calculators/vasp/presets/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/presets/BulkSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/presets/QMOFSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/presets/SlabSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/presets/magmoms_MP.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/presets/magmoms_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/presets/setups_pbe54.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/presets/setups_qmof.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/calculators/vasp/vasp_custodian.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.495679 quacc-0.7.5/src/quacc/recipes/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.495679 quacc-0.7.5/src/quacc/recipes/common/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/common/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/common/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/common/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/common/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.495679 quacc-0.7.5/src/quacc/recipes/dftb/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/dftb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/dftb/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/dftb/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.495679 quacc-0.7.5/src/quacc/recipes/emt/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/emt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/emt/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/emt/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/emt/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/emt/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/emt/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.495679 quacc-0.7.5/src/quacc/recipes/espresso/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/espresso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/espresso/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12481 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/espresso/bands.py
--rw-r--r--   0 runner    (1001) docker     (127)    13566 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/espresso/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9598 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/espresso/dos.py
--rw-r--r--   0 runner    (1001) docker     (127)    23055 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/espresso/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.499679 quacc-0.7.5/src/quacc/recipes/gaussian/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/gaussian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/gaussian/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/gaussian/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.499679 quacc-0.7.5/src/quacc/recipes/gulp/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/gulp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/gulp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/gulp/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.499679 quacc-0.7.5/src/quacc/recipes/lj/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/lj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/lj/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.499679 quacc-0.7.5/src/quacc/recipes/mlp/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/mlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/mlp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/mlp/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/mlp/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.499679 quacc-0.7.5/src/quacc/recipes/newtonnet/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/newtonnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/newtonnet/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/newtonnet/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.499679 quacc-0.7.5/src/quacc/recipes/onetep/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/onetep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/onetep/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/onetep/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.499679 quacc-0.7.5/src/quacc/recipes/orca/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/orca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/orca/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/orca/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.503679 quacc-0.7.5/src/quacc/recipes/psi4/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/psi4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/psi4/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/psi4/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.503679 quacc-0.7.5/src/quacc/recipes/qchem/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/qchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/qchem/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/qchem/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/qchem/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.503679 quacc-0.7.5/src/quacc/recipes/tblite/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/tblite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/tblite/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/tblite/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.503679 quacc-0.7.5/src/quacc/recipes/vasp/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/vasp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/vasp/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14585 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/vasp/mp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/vasp/qmof.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/recipes/vasp/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.507679 quacc-0.7.5/src/quacc/runners/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/runners/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/runners/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/runners/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/runners/thermo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.507679 quacc-0.7.5/src/quacc/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.507679 quacc-0.7.5/src/quacc/schemas/_aliases/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/_aliases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/_aliases/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/_aliases/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/_aliases/cclib.py
--rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/_aliases/emmet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/_aliases/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/_aliases/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    15500 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)    18073 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/cclib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/schemas/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    16783 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.507679 quacc-0.7.5/src/quacc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/utils/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/utils/kpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/utils/lists.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.511679 quacc-0.7.5/src/quacc/wflow_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/wflow_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/wflow_tools/customizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/wflow_tools/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-04-16 16:07:28.000000 quacc-0.7.5/src/quacc/wflow_tools/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:09:27.511679 quacc-0.7.5/src/quacc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-04-16 16:09:27.000000 quacc-0.7.5/src/quacc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-16 16:09:27.000000 quacc-0.7.5/src/quacc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 16:09:27.000000 quacc-0.7.5/src/quacc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-16 16:09:27.000000 quacc-0.7.5/src/quacc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-16 16:09:27.000000 quacc-0.7.5/src/quacc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 16:09:27.000000 quacc-0.7.5/src/quacc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.230923 quacc-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-20 17:23:17.000000 quacc-0.7.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-20 17:23:17.000000 quacc-0.7.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-04-20 17:25:13.230923 quacc-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-20 17:23:17.000000 quacc-0.7.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-20 17:23:17.000000 quacc-0.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 17:25:13.230923 quacc-0.7.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.202923 quacc-0.7.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.206923 quacc-0.7.6/src/quacc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.206923 quacc-0.7.6/src/quacc/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/_cli/quacc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.206923 quacc-0.7.6/src/quacc/atoms/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/atoms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/atoms/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/atoms/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/atoms/deformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/atoms/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/atoms/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.206923 quacc-0.7.6/src/quacc/calculators/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.206923 quacc-0.7.6/src/quacc/calculators/espresso/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17623 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/espresso.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.210923 quacc-0.7.6/src/quacc/calculators/espresso/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/esm_metal_slab_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/esm_metal_slab_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/metal_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/metal_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/molecule_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/semiconductors_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/semiconductors_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10584 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.210923 quacc-0.7.6/src/quacc/calculators/qchem/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/qchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/qchem/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/qchem/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/qchem/qchem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/qchem/qchem_custodian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.210923 quacc-0.7.6/src/quacc/calculators/vasp/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.214923 quacc-0.7.6/src/quacc/calculators/vasp/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/presets/BulkSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/presets/QMOFSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/presets/SlabSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/presets/magmoms_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/presets/setups_pbe54.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/presets/setups_qmof.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/vasp_custodian.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.214923 quacc-0.7.6/src/quacc/recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.214923 quacc-0.7.6/src/quacc/recipes/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/common/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/common/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/common/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/common/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.214923 quacc-0.7.6/src/quacc/recipes/dftb/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/dftb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/dftb/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/dftb/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.214923 quacc-0.7.6/src/quacc/recipes/emt/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/emt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/emt/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/emt/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/emt/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/emt/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/emt/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.214923 quacc-0.7.6/src/quacc/recipes/espresso/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/espresso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/espresso/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13160 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/espresso/bands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15327 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/espresso/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/espresso/dos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24396 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/espresso/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.218923 quacc-0.7.6/src/quacc/recipes/gaussian/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/gaussian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/gaussian/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/gaussian/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.218923 quacc-0.7.6/src/quacc/recipes/gulp/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/gulp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/gulp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/gulp/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.218923 quacc-0.7.6/src/quacc/recipes/lj/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/lj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/lj/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.218923 quacc-0.7.6/src/quacc/recipes/mlp/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/mlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/mlp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/mlp/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/mlp/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.218923 quacc-0.7.6/src/quacc/recipes/newtonnet/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/newtonnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/newtonnet/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/newtonnet/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.218923 quacc-0.7.6/src/quacc/recipes/onetep/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/onetep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/onetep/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/onetep/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.218923 quacc-0.7.6/src/quacc/recipes/orca/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/orca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6236 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/orca/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/orca/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.218923 quacc-0.7.6/src/quacc/recipes/psi4/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/psi4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/psi4/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/psi4/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.222923 quacc-0.7.6/src/quacc/recipes/qchem/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/qchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/qchem/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/qchem/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/qchem/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.222923 quacc-0.7.6/src/quacc/recipes/tblite/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/tblite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/tblite/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/tblite/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.222923 quacc-0.7.6/src/quacc/recipes/vasp/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/vasp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/vasp/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14585 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/vasp/mp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/vasp/qmof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/vasp/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.222923 quacc-0.7.6/src/quacc/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/runners/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/runners/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/runners/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/runners/thermo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.222923 quacc-0.7.6/src/quacc/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.226923 quacc-0.7.6/src/quacc/schemas/_aliases/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/_aliases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/_aliases/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/_aliases/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/_aliases/cclib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/_aliases/emmet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/_aliases/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/_aliases/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15500 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18073 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/cclib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16783 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.226923 quacc-0.7.6/src/quacc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/utils/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/utils/kpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/utils/lists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.226923 quacc-0.7.6/src/quacc/wflow_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/wflow_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/wflow_tools/customizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/wflow_tools/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/wflow_tools/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.226923 quacc-0.7.6/src/quacc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-04-20 17:25:13.000000 quacc-0.7.6/src/quacc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-20 17:25:13.000000 quacc-0.7.6/src/quacc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 17:25:13.000000 quacc-0.7.6/src/quacc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-20 17:25:13.000000 quacc-0.7.6/src/quacc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-20 17:25:13.000000 quacc-0.7.6/src/quacc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-20 17:25:13.000000 quacc-0.7.6/src/quacc.egg-info/top_level.txt
```

### Comparing `quacc-0.7.5/LICENSE.md` & `quacc-0.7.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/PKG-INFO` & `quacc-0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quacc
-Version: 0.7.5
+Version: 0.7.6
 Summary: A platform to enable high-throughput, database-driven quantum chemistry and computational materials science
 Author-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 Maintainer-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 License: BSD-3
 Project-URL: repository, https://github.com/Quantum-Accelerators/quacc
 Project-URL: documentation, https://quantum-accelerators.github.io/quacc/
 Project-URL: changelog, https://github.com/Quantum-Accelerators/quacc/blob/main/CHANGELOG.md
```

### Comparing `quacc-0.7.5/README.md` & `quacc-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/pyproject.toml` & `quacc-0.7.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quacc"
 description="A platform to enable high-throughput, database-driven quantum chemistry and computational materials science"
-version = "0.7.5"
+version = "0.7.6"
 readme = "README.md"
 license = { text = "BSD-3" }
 authors = [{ name = "Andrew S. Rosen", email = "asrosen@princeton.edu" }]
 maintainers = [{ name = "Andrew S. Rosen", email = "asrosen@princeton.edu" }]
 keywords = ["high-throughput", "automated", "workflow", "dft"]
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `quacc-0.7.5/src/quacc/__init__.py` & `quacc-0.7.6/src/quacc/__init__.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/_cli/quacc.py` & `quacc-0.7.6/src/quacc/_cli/quacc.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/atoms/core.py` & `quacc-0.7.6/src/quacc/atoms/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/atoms/defects.py` & `quacc-0.7.6/src/quacc/atoms/defects.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/atoms/deformation.py` & `quacc-0.7.6/src/quacc/atoms/deformation.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/atoms/phonons.py` & `quacc-0.7.6/src/quacc/atoms/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/atoms/slabs.py` & `quacc-0.7.6/src/quacc/atoms/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/calculators/espresso/espresso.py` & `quacc-0.7.6/src/quacc/calculators/espresso/espresso.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,30 +25,34 @@
 from quacc import SETTINGS
 from quacc.calculators.espresso.utils import (
     espresso_prepare_dir,
     get_pseudopotential_info,
     remove_conflicting_kpts_kspacing,
 )
 from quacc.utils.dicts import Remove, recursive_dict_merge, remove_dict_entries
-from quacc.utils.files import load_yaml_calc
+from quacc.utils.files import load_yaml_calc, safe_decompress_dir
 
 if TYPE_CHECKING:
     from typing import Any
 
 LOGGER = logging.getLogger(__name__)
 
 
 class EspressoTemplate(EspressoTemplate_):
     """
     A wrapper around the ASE Espresso template that allows for the use of
     other binaries such as pw.x, ph.x, cp.x, etc.
     """
 
     def __init__(
-        self, binary: str = "pw", test_run: bool = False, autorestart: bool = False
+        self,
+        binary: str = "pw",
+        test_run: bool = False,
+        autorestart: bool = False,
+        outdir: str | Path | None = None,
     ) -> None:
         """
         Initialize the Espresso template.
 
         Parameters
         ----------
         binary
@@ -56,14 +60,17 @@
             input/output file names. By default we fall back to "pw".
         test_run
             If True, a test run is performed to check that the calculation
             input_data is correct or to generate some files/info if needed.
         autorestart
             If True, the calculation will automatically switch to 'restart'
             if this calculator performs more than one run. (ASE-relax/MD/NEB)
+        outdir
+            The directory that will be used as `outdir` in the input_data. If
+            None, the directory will be set to the current working directory.
 
         Returns
         -------
         None
         """
         super().__init__()
 
@@ -76,14 +83,16 @@
         self._ase_known_binary = self.binary in ALL_KEYS
 
         self.test_run = test_run
 
         self.nruns = 0
         self.autorestart = autorestart
 
+        self.outdir = outdir
+
     def write_input(
         self,
         profile: EspressoProfile,
         directory: Path | str,
         atoms: Atoms,
         parameters: dict[str, Any],
         properties: Any,
@@ -109,14 +118,17 @@
         -------
         None
         """
         directory = Path(directory)
         self._output_handler(parameters, directory)
         parameters = self._sanity_checks(parameters)
 
+        if self.outdir:
+            safe_decompress_dir(self.outdir)
+
         if self.test_run:
             self._test_run(parameters, directory)
 
         if self.binary == "pw":
             if self.autorestart and self.nruns > 0:
                 parameters["input_data"]["electrons"]["startingpot"] = "file"
                 parameters["input_data"]["electrons"]["startingwfc"] = "file"
@@ -258,15 +270,15 @@
         dict[str, Any]
             The merged kwargs
         """
         os.environ.pop("ESPRESSO_TMPDIR", None)
         os.environ.pop("ESPRESSO_FILDVSCF_DIR", None)
         os.environ.pop("ESPRESSO_FILDRHO_DIR", None)
 
-        espresso_outdir = Path(directory).expanduser().resolve()
+        espresso_outdir = Path(self.outdir or directory).expanduser().resolve()
         outkeys = espresso_prepare_dir(espresso_outdir, self.binary)
 
         input_data = parameters.get("input_data", {})
         input_data = recursive_dict_merge(input_data, outkeys, verbose=True)
 
         parameters["input_data"] = input_data
```

### Comparing `quacc-0.7.5/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml` & `quacc-0.7.6/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml` & `quacc-0.7.6/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml` & `quacc-0.7.6/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/calculators/espresso/utils.py` & `quacc-0.7.6/src/quacc/calculators/espresso/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,16 +89,16 @@
         ]
     }
 
     if lqdir or qpt == (0.0, 0.0, 0.0):
         files_to_copy[directory].extend(
             [
                 Path("pwscf.save", "charge-density.*"),
-                Path("pwscf.save", "data-file-schema.xml.*"),
-                Path("pwscf.save", "paw.txt.*"),
+                Path("pwscf.save", "data-file-schema.xml*"),
+                Path("pwscf.save", "paw.txt*"),
                 Path("pwscf.save", "wfc*.*"),
             ]
         )
         if qpt != (0.0, 0.0, 0.0):
             files_to_copy[directory].extend(
                 [
                     Path("_ph0", f"pwscf.q_{qnum}", "pwscf.save", "*"),
@@ -189,15 +189,15 @@
                 "outdir": outdir,
             }
         },
         "dvscf_q2r": {
             "input": {
                 "prefix": "pwscf",
                 "fildyn": "matdyn",
-                "outdir": ".",
+                "outdir": outdir,
                 "wpot_dir": Remove,
             }
         },
         "postahc": {"input": {"ahc_dir": "ahc_dir/", "flvec": "matdyn.modes"}},
     }
 
     return outkeys.get(binary, {})
```

### Comparing `quacc-0.7.5/src/quacc/calculators/qchem/io.py` & `quacc-0.7.6/src/quacc/calculators/qchem/io.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/calculators/qchem/params.py` & `quacc-0.7.6/src/quacc/calculators/qchem/params.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/calculators/qchem/qchem.py` & `quacc-0.7.6/src/quacc/calculators/qchem/qchem.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/calculators/qchem/qchem_custodian.py` & `quacc-0.7.6/src/quacc/calculators/qchem/qchem_custodian.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/calculators/vasp/io.py` & `quacc-0.7.6/src/quacc/calculators/vasp/io.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/calculators/vasp/params.py` & `quacc-0.7.6/src/quacc/calculators/vasp/params.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml` & `quacc-0.7.6/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/calculators/vasp/presets/setups_pbe54.yaml` & `quacc-0.7.6/src/quacc/calculators/vasp/presets/setups_pbe54.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/calculators/vasp/presets/setups_qmof.yaml` & `quacc-0.7.6/src/quacc/calculators/vasp/presets/setups_qmof.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/calculators/vasp/vasp.py` & `quacc-0.7.6/src/quacc/calculators/vasp/vasp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/calculators/vasp/vasp_custodian.py` & `quacc-0.7.6/src/quacc/calculators/vasp/vasp_custodian.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/common/defects.py` & `quacc-0.7.6/src/quacc/recipes/common/defects.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/common/elastic.py` & `quacc-0.7.6/src/quacc/recipes/common/elastic.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/common/phonons.py` & `quacc-0.7.6/src/quacc/recipes/common/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/common/slabs.py` & `quacc-0.7.6/src/quacc/recipes/common/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/dftb/_base.py` & `quacc-0.7.6/src/quacc/recipes/dftb/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/dftb/core.py` & `quacc-0.7.6/src/quacc/recipes/dftb/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/emt/core.py` & `quacc-0.7.6/src/quacc/recipes/emt/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/emt/defects.py` & `quacc-0.7.6/src/quacc/recipes/emt/defects.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/emt/elastic.py` & `quacc-0.7.6/src/quacc/recipes/emt/elastic.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/emt/phonons.py` & `quacc-0.7.6/src/quacc/recipes/emt/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/emt/slabs.py` & `quacc-0.7.6/src/quacc/recipes/emt/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/espresso/_base.py` & `quacc-0.7.6/src/quacc/recipes/espresso/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/espresso/bands.py` & `quacc-0.7.6/src/quacc/recipes/espresso/bands.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,16 +31,20 @@
         fermi_surface: RunSchema
 
 
 @job
 def bands_pw_job(
     atoms: Atoms,
     copy_files: (
-        SourceDirectory | list[SourceDirectory] | dict[SourceDirectory, Filenames]
-    ),
+        SourceDirectory
+        | list[SourceDirectory]
+        | dict[SourceDirectory, Filenames]
+        | None
+    ) = None,
+    prev_outdir: SourceDirectory | None = None,
     make_bandpath: bool = True,
     line_density: float = 20,
     force_gamma: bool = True,
     parallel_info: dict[str] | None = None,
     test_run: bool = False,
     **calc_kwargs,
 ) -> RunSchema:
@@ -57,14 +61,18 @@
         The Atoms object.
     copy_files
         Source directory or directories to copy files from. If a `SourceDirectory` or a
         list of `SourceDirectory` is provided, this interface will automatically guess
         which files have to be copied over by looking at the binary and `input_data`.
         If a dict is provided, the mode is manual, keys are source directories and values
         are relative path to files or directories to copy. Glob patterns are supported.
+    prev_outdir
+        The output directory of a previous calculation. If provided, Quantum Espresso
+        will directly read the necessary files from this directory, eliminating the need
+        to manually copy files. The directory will be ungzipped if necessary.
     make_bandpath
         If True, it returns the primitive cell for your structure and generates
         the high symmetry k-path using Latmer-Munro approach.
         For more information look at
         [pymatgen.symmetry.bandstructure.HighSymmKpath][]
     line_density
         Density of kpoints along the band path if make_bandpath is True
@@ -101,48 +109,53 @@
                 {"line_density": line_density}, atoms, force_gamma=force_gamma
             )[0],
             cell=atoms.get_cell(),
         )
 
     return run_and_summarize(
         atoms,
-        template=EspressoTemplate("pw", test_run=test_run),
+        template=EspressoTemplate("pw", test_run=test_run, outdir=prev_outdir),
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
         parallel_info=parallel_info,
         additional_fields={"name": "pw.x bands"},
         copy_files=copy_files,
     )
 
 
 @job
 def bands_pp_job(
-    atoms: Atoms,
     copy_files: (
-        SourceDirectory | list[SourceDirectory] | dict[SourceDirectory, Filenames]
-    ),
+        SourceDirectory
+        | list[SourceDirectory]
+        | dict[SourceDirectory, Filenames]
+        | None
+    ) = None,
+    prev_outdir: SourceDirectory | None = None,
     parallel_info: dict[str] | None = None,
     test_run: bool = False,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to re-order bands and computes bands-related properties with bands.x.
     This allows to get the bands structure in a more readable way. This requires a
     previous [quacc.recipes.espresso.bands.bands_pw_job][] calculation.
 
     Parameters
     ----------
-    atoms
-        The Atoms object.
     copy_files
         Source directory or directories to copy files from. If a `SourceDirectory` or a
         list of `SourceDirectory` is provided, this interface will automatically guess
         which files have to be copied over by looking at the binary and `input_data`.
         If a dict is provided, the mode is manual, keys are source directories and values
         are relative path to files or directories to copy. Glob patterns are supported.
+    prev_outdir
+        The output directory of a previous calculation. If provided, Quantum Espresso
+        will directly read the necessary files from this directory, eliminating the need
+        to manually copy files. The directory will be ungzipped if necessary.
     parallel_info
         Dictionary containing information about the parallelization of the
         calculation. See the ASE documentation for more information.
     test_run
         If True, a test run is performed to check that the calculation input_data is correct or
         to generate some files/info if needed.
     **calc_kwargs
@@ -153,48 +166,52 @@
     Returns
     -------
     RunSchema
         Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
     return run_and_summarize(
-        atoms,
-        template=EspressoTemplate("bands", test_run=test_run),
+        template=EspressoTemplate("bands", test_run=test_run, outdir=prev_outdir),
         calc_defaults={},
         calc_swaps=calc_kwargs,
         parallel_info=parallel_info,
         additional_fields={"name": "bands.x post-processing"},
         copy_files=copy_files,
     )
 
 
 @job
 def fermi_surface_job(
-    atoms: Atoms,
     copy_files: (
-        SourceDirectory | list[SourceDirectory] | dict[SourceDirectory, Filenames]
-    ),
+        SourceDirectory
+        | list[SourceDirectory]
+        | dict[SourceDirectory, Filenames]
+        | None
+    ) = None,
+    prev_outdir: SourceDirectory | None = None,
     parallel_info: dict[str] | None = None,
     test_run: bool = False,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to retrieve the fermi surface with fs.x
     It requires a previous uniform unshifted k-point grid bands calculation.
 
     Parameters
     ----------
-    atoms
-        The Atoms object.
     copy_files
         Source directory or directories to copy files from. If a `SourceDirectory` or a
         list of `SourceDirectory` is provided, this interface will automatically guess
         which files have to be copied over by looking at the binary and `input_data`.
         If a dict is provided, the mode is manual, keys are source directories and values
         are relative path to files or directories to copy. Glob patterns are supported.
+    prev_outdir
+        The output directory of a previous calculation. If provided, Quantum Espresso
+        will directly read the necessary files from this directory, eliminating the need
+        to manually copy files. The directory will be ungzipped if necessary.
     parallel_info
         Dictionary containing information about the parallelization of the
         calculation. See the ASE documentation for more information.
     test_run
         If True, a test run is performed to check that the calculation input_data is correct or
         to generate some files/info if needed.
     **calc_kwargs
@@ -205,16 +222,15 @@
     Returns
     -------
     RunSchema
         Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
     return run_and_summarize(
-        atoms,
-        template=EspressoTemplate("fs", test_run=test_run),
+        template=EspressoTemplate("fs", test_run=test_run, outdir=prev_outdir),
         calc_defaults={},
         calc_swaps=calc_kwargs,
         parallel_info=parallel_info,
         additional_fields={"name": "fs.x fermi_surface"},
         copy_files=copy_files,
     )
 
@@ -227,15 +243,14 @@
     ),
     run_bands_pp: bool = True,
     run_fermi_surface: bool = False,
     make_bandpath: bool = True,
     line_density: float = 20,
     force_gamma: bool = True,
     parallel_info: dict[str] | None = None,
-    test_run: bool = False,
     job_params: dict[str, Any] | None = None,
     job_decorators: dict[str, Callable | None] | None = None,
 ) -> BandsSchema:
     """
     Function to compute bands structure and fermi surface using pw.x, bands.x and fs.x.
 
     Consists of the following steps:
@@ -275,17 +290,14 @@
         For more information [quacc.utils.kpts.convert_pmg_kpts][]
     force_gamma
         Forces gamma-centered k-points when using make_bandpath
         For more information [quacc.utils.kpts.convert_pmg_kpts][]
     parallel_info
         Dictionary containing information about the parallelization of the
         calculation. See the ASE documentation for more information.
-    test_run
-        If True, a test run is performed to check that the calculation input_data is correct or
-        to generate some files/info if needed.
     job_params
         Custom parameters to pass to each Job in the Flow. This is a dictinoary where
         the keys are the names of the jobs and the values are dictionaries of parameters.
     job_decorators
         Custom decorators to apply to each Job in the Flow. This is a dictionary where
         the keys are the names of the jobs and the values are decorators.
 
@@ -298,36 +310,30 @@
     (bands_pw_job_, bands_pp_job_, fermi_surface_job_) = customize_funcs(
         ["bands_pw_job", "bands_pp_job", "fermi_surface_job"],
         [bands_pw_job, bands_pp_job, fermi_surface_job],
         parameters=job_params,
         decorators=job_decorators,
     )
 
-    bands_result = bands_pw_job_(
+    bands_results = bands_pw_job_(
         atoms,
         copy_files,
         make_bandpath=make_bandpath,
         line_density=line_density,
         force_gamma=force_gamma,
         parallel_info=parallel_info,
-        test_run=test_run,
     )
-    results = {"bands_pw": bands_result}
+    results = {"bands_pw": bands_results}
+
     if run_bands_pp:
         bands_pp_results = bands_pp_job_(
-            atoms,
-            bands_result["dir_name"],
-            parallel_info=parallel_info,
-            test_run=test_run,
+            prev_outdir=bands_results["dir_name"], parallel_info=parallel_info
         )
         results["bands_pp"] = bands_pp_results
 
     if run_fermi_surface:
         fermi_results = fermi_surface_job_(
-            atoms,
-            bands_result["dir_name"],
-            parallel_info=parallel_info,
-            test_run=test_run,
+            prev_outdir=bands_results["dir_name"], parallel_info=parallel_info
         )
         results["fermi_surface"] = fermi_results
 
     return results
```

### Comparing `quacc-0.7.5/src/quacc/recipes/espresso/core.py` & `quacc-0.7.6/src/quacc/recipes/espresso/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     test_run: bool = False,
     copy_files: (
         SourceDirectory
         | list[SourceDirectory]
         | dict[SourceDirectory, Filenames]
         | None
     ) = None,
+    prev_outdir: SourceDirectory | None = None,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a basic SCF calculation with pw.x.
 
     Parameters
     ----------
@@ -69,14 +70,18 @@
         to generate some files/info if needed.
     copy_files
         Source directory or directories to copy files from. If a `SourceDirectory` or a
         list of `SourceDirectory` is provided, this interface will automatically guess
         which files have to be copied over by looking at the binary and `input_data`.
         If a dict is provided, the mode is manual, keys are source directories and values
         are relative path to files or directories to copy. Glob patterns are supported.
+    prev_outdir
+        The output directory of a previous calculation. If provided, Quantum Espresso
+        will directly read the necessary files from this directory, eliminating the need
+        to manually copy files. The directory will be ungzipped if necessary.
     **calc_kwargs
         Additional keyword arguments to pass to the Espresso calculator. Set a value to
         `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
         [quacc.calculators.espresso.espresso.Espresso][] for more information.
 
     Returns
     -------
@@ -88,15 +93,15 @@
 
     calc_defaults = BASE_SET_METAL if is_metal else BASE_SET_NON_METAL
     calc_defaults["input_data"]["control"] = {"calculation": "scf"}
 
     return run_and_summarize(
         atoms,
         preset=preset,
-        template=EspressoTemplate("pw", test_run=test_run),
+        template=EspressoTemplate("pw", test_run=test_run, outdir=prev_outdir),
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
         parallel_info=parallel_info,
         additional_fields={"name": "pw.x Static"},
         copy_files=copy_files,
     )
 
@@ -110,14 +115,15 @@
     test_run: bool = False,
     copy_files: (
         SourceDirectory
         | list[SourceDirectory]
         | dict[SourceDirectory, Filenames]
         | None
     ) = None,
+    prev_outdir: SourceDirectory | None = None,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a structure relaxation with pw.x.
 
     Parameters
     ----------
@@ -137,14 +143,18 @@
         to generate some files/info if needed.
     copy_files
         Source directory or directories to copy files from. If a `SourceDirectory` or a
         list of `SourceDirectory` is provided, this interface will automatically guess
         which files have to be copied over by looking at the binary and `input_data`.
         If a dict is provided, the mode is manual, keys are source directories and values
         are relative path to files or directories to copy. Glob patterns are supported.
+    prev_outdir
+        The output directory of a previous calculation. If provided, Quantum Espresso
+        will directly read the necessary files from this directory, eliminating the need
+        to manually copy files. The directory will be ungzipped if necessary.
     **calc_kwargs
         Additional keyword arguments to pass to the Espresso calculator. Set a value to
         `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
         [quacc.calculators.espresso.espresso.Espresso][] for more information.
 
     Returns
     -------
@@ -158,15 +168,15 @@
     calc_defaults["input_data"]["control"] = {
         "calculation": "vc-relax" if relax_cell else "relax"
     }
 
     return run_and_summarize(
         atoms,
         preset=preset,
-        template=EspressoTemplate("pw", test_run=test_run),
+        template=EspressoTemplate("pw", test_run=test_run, outdir=prev_outdir),
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
         parallel_info=parallel_info,
         additional_fields={"name": "pw.x Relax"},
         copy_files=copy_files,
     )
 
@@ -181,14 +191,15 @@
     opt_params: dict[str, Any] | None = None,
     copy_files: (
         SourceDirectory
         | list[SourceDirectory]
         | dict[SourceDirectory, Filenames]
         | None
     ) = None,
+    prev_outdir: SourceDirectory | None = None,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a structure relaxation with pw.x using ASE
     external optimizers.
 
     Parameters
@@ -213,14 +224,18 @@
         of available keys, refer to [quacc.runners.ase.run_opt][].
     copy_files
         Source directory or directories to copy files from. If a `SourceDirectory` or a
         list of `SourceDirectory` is provided, this interface will automatically guess
         which files have to be copied over by looking at the binary and `input_data`.
         If a dict is provided, the mode is manual, keys are source directories and values
         are relative path to files or directories to copy. Glob patterns are supported.
+    prev_outdir
+        The output directory of a previous calculation. If provided, Quantum Espresso
+        will directly read the necessary files from this directory, eliminating the need
+        to manually copy files. The directory will be ungzipped if necessary.
     **calc_kwargs
         Additional keyword arguments to pass to the Espresso calculator. Set a value to
         `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
         [quacc.calculators.espresso.espresso.Espresso][] for more information.
 
     Returns
     -------
@@ -239,30 +254,34 @@
 
     opt_defaults = {"optimizer": BFGSLineSearch}
 
     return run_and_summarize_opt(
         atoms,
         preset=preset,
         relax_cell=relax_cell,
-        template=EspressoTemplate("pw", autorestart=autorestart),
+        template=EspressoTemplate("pw", autorestart=autorestart, outdir=prev_outdir),
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
         opt_defaults=opt_defaults,
         opt_params=opt_params,
         parallel_info=parallel_info,
         additional_fields={"name": "pw.x ExternalRelax"},
         copy_files=copy_files,
     )
 
 
 @job
 def post_processing_job(
     copy_files: (
-        SourceDirectory | list[SourceDirectory] | dict[SourceDirectory, Filenames]
-    ),
+        SourceDirectory
+        | list[SourceDirectory]
+        | dict[SourceDirectory, Filenames]
+        | None
+    ) = None,
+    prev_outdir: SourceDirectory | None = None,
     parallel_info: dict[str] | None = None,
     test_run: bool = False,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a basic pp.x calculation (post-processing).
     It is mainly used to extract the charge density from a previous pw.x calculation.
@@ -273,14 +292,18 @@
     ----------
     copy_files
         Source directory or directories to copy files from. If a `SourceDirectory` or a
         list of `SourceDirectory` is provided, this interface will automatically guess
         which files have to be copied over by looking at the binary and `input_data`.
         If a dict is provided, the mode is manual, keys are source directories and values
         are relative path to files or directories to copy. Glob patterns are supported.
+    prev_outdir
+        The output directory of a previous calculation. If provided, Quantum Espresso
+        will directly read the necessary files from this directory, eliminating the need
+        to manually copy files. The directory will be ungzipped if necessary.
     parallel_info
         Dictionary containing information about the parallelization of the
         calculation. See the ASE documentation for more information.
     **calc_kwargs
         Additional keyword arguments to pass to the Espresso calculator. Set a value to
         `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
         [quacc.calculators.espresso.espresso.Espresso][] for more information.
@@ -299,29 +322,33 @@
                 "output_format": 6,
                 "fileout": "pseudo_charge_density.cube",
             },
         }
     }
 
     return run_and_summarize(
-        template=EspressoTemplate("pp", test_run=test_run),
+        template=EspressoTemplate("pp", test_run=test_run, outdir=prev_outdir),
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
         parallel_info=parallel_info,
         additional_fields={"name": "pp.x post-processing"},
         copy_files=copy_files,
     )
 
 
 @job
 def non_scf_job(
     atoms: Atoms,
     copy_files: (
-        SourceDirectory | list[SourceDirectory] | dict[SourceDirectory, Filenames]
-    ),
+        SourceDirectory
+        | list[SourceDirectory]
+        | dict[SourceDirectory, Filenames]
+        | None
+    ) = None,
+    prev_outdir: SourceDirectory | None = None,
     preset: str | None = "sssp_1.3.0_pbe_efficiency",
     parallel_info: dict[str] | None = None,
     test_run: bool = False,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a basic NSCF calculation with pw.x.
@@ -332,14 +359,18 @@
         The Atoms object.
     copy_files
         Source directory or directories to copy files from. If a `SourceDirectory` or a
         list of `SourceDirectory` is provided, this interface will automatically guess
         which files have to be copied over by looking at the binary and `input_data`.
         If a dict is provided, the mode is manual, keys are source directories and values
         are relative path to files or directories to copy. Glob patterns are supported.
+    prev_outdir
+        The output directory of a previous calculation. If provided, Quantum Espresso
+        will directly read the necessary files from this directory, eliminating the need
+        to manually copy files. The directory will be ungzipped if necessary.
     preset
         The name of a YAML file containing a list of parameters to use as
         a "preset" for the calculator. quacc will automatically look in the
         `ESPRESSO_PRESET_DIR` (default: quacc/calculators/espresso/presets).
     parallel_info
         Dictionary containing information about the parallelization of the
         calculation. See the ASE documentation for more information.
@@ -358,14 +389,14 @@
         See the type-hint for the data structure.
     """
     calc_defaults = {"input_data": {"control": {"calculation": "nscf"}}}
 
     return run_and_summarize(
         atoms,
         preset=preset,
-        template=EspressoTemplate("pw", test_run=test_run),
+        template=EspressoTemplate("pw", test_run=test_run, outdir=prev_outdir),
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
         parallel_info=parallel_info,
         additional_fields={"name": "pw.x Non SCF"},
         copy_files=copy_files,
     )
```

### Comparing `quacc-0.7.5/src/quacc/recipes/espresso/dos.py` & `quacc-0.7.6/src/quacc/recipes/espresso/dos.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,16 +28,20 @@
         static_job: RunSchema
         non_scf_job: RunSchema
 
 
 @job
 def dos_job(
     copy_files: (
-        SourceDirectory | list[SourceDirectory] | dict[SourceDirectory, Filenames]
-    ),
+        SourceDirectory
+        | list[SourceDirectory]
+        | dict[SourceDirectory, Filenames]
+        | None
+    ) = None,
+    prev_outdir: SourceDirectory | None = None,
     parallel_info: dict[str] | None = None,
     test_run: bool = False,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a basic dos.x calculation (density of states).
     It is mainly used to extract the charge density and wavefunction from a previous pw.x calculation.
@@ -48,14 +52,18 @@
     ----------
     copy_files
         Source directory or directories to copy files from. If a `SourceDirectory` or a
         list of `SourceDirectory` is provided, this interface will automatically guess
         which files have to be copied over by looking at the binary and `input_data`.
         If a dict is provided, the mode is manual, keys are source directories and values
         are relative path to files or directories to copy. Glob patterns are supported.
+    prev_outdir
+        The output directory of a previous calculation. If provided, Quantum Espresso
+        will directly read the necessary files from this directory, eliminating the need
+        to manually copy files. The directory will be ungzipped if necessary.
     parallel_info
         Dictionary containing information about the parallelization of the
         calculation. See the ASE documentation for more information.
     **calc_kwargs
         Additional keyword arguments to pass to the Espresso calculator. Set a value to
         `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
         `ase.io.espresso.write_fortran_namelist` for more information.
@@ -63,46 +71,54 @@
     Returns
     -------
     RunSchema
         Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
     return run_and_summarize(
-        template=EspressoTemplate("dos", test_run=test_run),
+        template=EspressoTemplate("dos", test_run=test_run, outdir=prev_outdir),
         calc_defaults=None,
         calc_swaps=calc_kwargs,
         parallel_info=parallel_info,
         additional_fields={"name": "dos.x Density-of-States"},
         copy_files=copy_files,
     )
 
 
 @job
 def projwfc_job(
     copy_files: (
-        SourceDirectory | list[SourceDirectory] | dict[SourceDirectory, Filenames]
-    ),
+        SourceDirectory
+        | list[SourceDirectory]
+        | dict[SourceDirectory, Filenames]
+        | None
+    ) = None,
+    prev_outdir: SourceDirectory | None = None,
     parallel_info: dict[str] | None = None,
     test_run: bool = False,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a basic projwfc.x calculation.
     It is mainly used to extract the charge density and wavefunction from a previous pw.x calculation.
-    It can generate partial dos, local dos, spilling paramenter and more. Fore more details please see
+    It can generate partial dos, local dos, spilling parameter and more. Fore more details please see
     https://www.quantum-espresso.org/Doc/INPUT_PROJWFC.html
 
     Parameters
     ----------
     copy_files
         Source directory or directories to copy files from. If a `SourceDirectory` or a
         list of `SourceDirectory` is provided, this interface will automatically guess
         which files have to be copied over by looking at the binary and `input_data`.
         If a dict is provided, the mode is manual, keys are source directories and values
         are relative path to files or directories to copy. Glob patterns are supported.
+    prev_outdir
+        The output directory of a previous calculation. If provided, Quantum Espresso
+        will directly read the necessary files from this directory, eliminating the need
+        to manually copy files. The directory will be ungzipped if necessary.
     parallel_info
         Dictionary containing information about the parallelization of the
         calculation. See the ASE documentation for more information.
     **calc_kwargs
         Additional keyword arguments to pass to the Espresso calculator. Set a value to
         `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
         `ase.io.espresso.write_fortran_namelist` for more information.
@@ -110,15 +126,15 @@
     Returns
     -------
     RunSchema
         Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
     return run_and_summarize(
-        template=EspressoTemplate("projwfc", test_run=test_run),
+        template=EspressoTemplate("projwfc", test_run=test_run, outdir=prev_outdir),
         calc_defaults=None,
         calc_swaps=calc_kwargs,
         parallel_info=parallel_info,
         additional_fields={"name": "projwfc.x Projects-wavefunctions"},
         copy_files=copy_files,
     )
 
@@ -190,17 +206,17 @@
         [static_job, non_scf_job, dos_job],
         parameters=job_params,
         decorators=job_decorators,
     )
 
     static_results = static_job_(atoms)
 
-    non_scf_results = non_scf_job_(atoms, static_results["dir_name"])
+    non_scf_results = non_scf_job_(atoms, prev_outdir=static_results["dir_name"])
 
-    dos_results = dos_job_(non_scf_results["dir_name"])
+    dos_results = dos_job_(prev_outdir=static_results["dir_name"])
 
     return {
         "static_job": static_results,
         "non_scf_job": non_scf_results,
         "dos_job": dos_results,
     }
 
@@ -272,16 +288,16 @@
         [static_job, non_scf_job, projwfc_job],
         parameters=job_params,
         decorators=job_decorators,
     )
 
     static_results = static_job_(atoms)
 
-    non_scf_results = non_scf_job_(atoms, static_results["dir_name"])
+    non_scf_results = non_scf_job_(atoms, prev_outdir=static_results["dir_name"])
 
-    projwfc_results = projwfc_job_(non_scf_results["dir_name"])
+    projwfc_results = projwfc_job_(prev_outdir=static_results["dir_name"])
 
     return {
         "static_job": static_results,
         "non_scf_job": non_scf_results,
         "projwfc_job": projwfc_results,
     }
```

### Comparing `quacc-0.7.5/src/quacc/recipes/espresso/phonons.py` & `quacc-0.7.6/src/quacc/recipes/espresso/phonons.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,16 +36,20 @@
         q2r_job: RunSchema
         matdyn_job: RunSchema
 
 
 @job
 def phonon_job(
     copy_files: (
-        SourceDirectory | list[SourceDirectory] | dict[SourceDirectory, Filenames]
-    ),
+        SourceDirectory
+        | list[SourceDirectory]
+        | dict[SourceDirectory, Filenames]
+        | None
+    ) = None,
+    prev_outdir: SourceDirectory | None = None,
     parallel_info: dict[str] | None = None,
     test_run: bool = False,
     use_phcg: bool = False,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a basic ph.x calculation. It should allow you to
@@ -59,14 +63,18 @@
     ----------
     copy_files
         Source directory or directories to copy files from. If a `SourceDirectory` or a
         list of `SourceDirectory` is provided, this interface will automatically guess
         which files have to be copied over by looking at the binary and `input_data`.
         If a dict is provided, the mode is manual, keys are source directories and values
         are relative path to files or directories to copy. Glob patterns are supported.
+    prev_outdir
+        The output directory of a previous calculation. If provided, Quantum Espresso
+        will directly read the necessary files from this directory, eliminating the need
+        to manually copy files. The directory will be ungzipped if necessary.
     parallel_info
         Dictionary containing information about the parallelization of the
         calculation. See the ASE documentation for more information.
     test_run
         If True, a test run is performed to check that the calculation input_data is correct or
         to generate some files/info if needed.
     use_phcg
@@ -90,28 +98,31 @@
         },
         "qpts": (0, 0, 0),
     }
 
     binary = "phcg" if use_phcg else "ph"
 
     return run_and_summarize(
-        template=EspressoTemplate(binary, test_run=test_run),
+        template=EspressoTemplate(binary, test_run=test_run, outdir=prev_outdir),
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
         parallel_info=parallel_info,
         additional_fields={"name": f"{binary}.x Phonon"},
         copy_files=copy_files,
     )
 
 
 @job
 def q2r_job(
     copy_files: (
-        SourceDirectory | list[SourceDirectory] | dict[SourceDirectory, Filenames]
-    ),
+        SourceDirectory
+        | list[SourceDirectory]
+        | dict[SourceDirectory, Filenames]
+        | None
+    ) = None,
     parallel_info: dict[str] | None = None,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a basic q2r.x calculation. It should allow you to
     use all the features of the [q2r.x binary](https://www.quantum-espresso.org/Doc/INPUT_Q2R.html#idm51)
 
@@ -150,16 +161,19 @@
         copy_files=copy_files,
     )
 
 
 @job
 def matdyn_job(
     copy_files: (
-        SourceDirectory | list[SourceDirectory] | dict[SourceDirectory, Filenames]
-    ),
+        SourceDirectory
+        | list[SourceDirectory]
+        | dict[SourceDirectory, Filenames]
+        | None
+    ) = None,
     parallel_info: dict[str] | None = None,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a basic `matdyn.x` calculation. It should allow you to use
     all the features of the [matdyn.x binary](https://www.quantum-espresso.org/Doc/INPUT_MATDYN.html#idm138)
 
@@ -276,17 +290,17 @@
         ["relax_job", "phonon_job", "q2r_job", "matdyn_job"],
         [relax_job, phonon_job, q2r_job, matdyn_job],
         parameters=job_params,
         decorators=job_decorators,
     )
 
     pw_job_results = pw_job(atoms)
-    ph_job_results = ph_job(pw_job_results["dir_name"])
-    fc_job_results = fc_job(ph_job_results["dir_name"])
-    dos_job_results = dos_job(fc_job_results["dir_name"])
+    ph_job_results = ph_job(prev_outdir=pw_job_results["dir_name"])
+    fc_job_results = fc_job(copy_files=ph_job_results["dir_name"])
+    dos_job_results = dos_job(copy_files=fc_job_results["dir_name"])
 
     return {
         "relax_job": pw_job_results,
         "phonon_job": ph_job_results,
         "q2r_job": fc_job_results,
         "matdyn_job": dos_job_results,
     }
@@ -403,21 +417,25 @@
         -------
         list[RunSchema]
             A list of results from each phonon job.
         """
         ph_input_data = Namelist(ph_input_data)
         ph_input_data.to_nested(binary="ph")
 
+        prev_outdir = ph_init_job_results["parameters"]["input_data"]["inputph"][
+            "outdir"
+        ]
+
         grid_results = []
         for qnum, qdata in ph_init_job_results["results"].items():
             ph_input_data["inputph"]["start_q"] = qnum
             ph_input_data["inputph"]["last_q"] = qnum
             repr_to_do = grid_prepare_repr(qdata["representations"], nblocks)
             files_to_copy = grid_copy_files(
-                ph_input_data, ph_init_job_results["dir_name"], qnum, qdata["qpoint"]
+                ph_input_data, prev_outdir, qnum, qdata["qpoint"]
             )
             for representation in repr_to_do:
                 ph_input_data["inputph"]["start_irr"] = representation[0]
                 ph_input_data["inputph"]["last_irr"] = representation[-1]
                 ph_job_results = ph_job(
                     deepcopy(files_to_copy), input_data=deepcopy(ph_input_data)
                 )
@@ -460,28 +478,32 @@
         [relax_job, phonon_job, phonon_job, phonon_job],
         parameters=job_params,
         decorators=job_decorators,
     )
 
     pw_job_results = pw_job(atoms)
 
-    ph_init_job_results = ph_init_job(pw_job_results["dir_name"])
+    ph_init_job_results = ph_init_job(prev_outdir=pw_job_results["dir_name"])
 
     grid_results = _grid_phonon_subflow(
         job_params["ph_job"]["input_data"], ph_init_job_results, ph_job, nblocks=nblocks
     )
 
     return _ph_recover_subflow(grid_results)
 
 
 @job
 def dvscf_q2r_job(
     copy_files: (
-        SourceDirectory | list[SourceDirectory] | dict[SourceDirectory, Filenames]
-    ),
+        SourceDirectory
+        | list[SourceDirectory]
+        | dict[SourceDirectory, Filenames]
+        | None
+    ) = None,
+    prev_outdir: SourceDirectory | None = None,
     parallel_info: dict[str] | None = None,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a basic dvscf_q2r calculation allowing phonon potential
     interpolation from coarse to fine q-point grids using Fourier interpolation.
     It should allow you to use all the features of the dvscf_q2r binary which does
@@ -516,14 +538,18 @@
     ----------
     copy_files
         Source directory or directories to copy files from. If a `SourceDirectory` or a
         list of `SourceDirectory` is provided, this interface will automatically guess
         which files have to be copied over by looking at the binary and `input_data`.
         If a dict is provided, the mode is manual, keys are source directories and values
         are relative path to files or directories to copy. Glob patterns are supported.
+    prev_outdir
+        The output directory of a previous calculation. If provided, Quantum Espresso
+        will directly read the necessary files from this directory, eliminating the need
+        to manually copy files. The directory will be ungzipped if necessary.
     parallel_info
         Dictionary containing information about the parallelization of the
         calculation. See the ASE documentation for more information.
     **calc_kwargs
         Additional keyword arguments to pass to the Espresso calculator. Set a value to
         `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
         [quacc.calculators.espresso.espresso.Espresso][] for more information.
@@ -531,28 +557,32 @@
     Returns
     -------
     RunSchema
         Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
     return run_and_summarize(
-        template=EspressoTemplate("dvscf_q2r"),
+        template=EspressoTemplate("dvscf_q2r", outdir=prev_outdir),
         calc_defaults={},
         calc_swaps=calc_kwargs,
         parallel_info=parallel_info,
         additional_fields={"name": "dvscf_q2r Phonon"},
         copy_files=copy_files,
     )
 
 
 @job
 def postahc_job(
     copy_files: (
-        SourceDirectory | list[SourceDirectory] | dict[SourceDirectory, Filenames]
-    ),
+        SourceDirectory
+        | list[SourceDirectory]
+        | dict[SourceDirectory, Filenames]
+        | None
+    ) = None,
+    prev_outdir: SourceDirectory | None = None,
     parallel_info: dict[str] | None = None,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a basic postahc calculation. It should allow you to
     use all the features of the [postahc.x binary](https://www.quantum-espresso.org/Doc/INPUT_POSTAHC.html#idm11)
 
@@ -572,14 +602,18 @@
     ----------
     copy_files
         Source directory or directories to copy files from. If a `SourceDirectory` or a
         list of `SourceDirectory` is provided, this interface will automatically guess
         which files have to be copied over by looking at the binary and `input_data`.
         If a dict is provided, the mode is manual, keys are source directories and values
         are relative path to files or directories to copy. Glob patterns are supported.
+    prev_outdir
+        The output directory of a previous calculation. If provided, Quantum Espresso
+        will directly read the necessary files from this directory, eliminating the need
+        to manually copy files. The directory will be ungzipped if necessary.
     parallel_info
         Dictionary containing information about the parallelization of the
         calculation. See the ASE documentation for more information.
     **calc_kwargs
         Additional keyword arguments to pass to the Espresso calculator. Set a value to
         `quacc.Remove` to remove a pre-existing key entirely. See the docstring of
         [quacc.calculators.espresso.espresso.Espresso][] for more information.
@@ -587,14 +621,14 @@
     Returns
     -------
     RunSchema
         Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
     return run_and_summarize(
-        template=EspressoTemplate("postahc"),
+        template=EspressoTemplate("postahc", outdir=prev_outdir),
         calc_defaults={},
         calc_swaps=calc_kwargs,
         parallel_info=parallel_info,
         additional_fields={"name": "postahc Phonon"},
         copy_files=copy_files,
     )
```

### Comparing `quacc-0.7.5/src/quacc/recipes/gaussian/_base.py` & `quacc-0.7.6/src/quacc/recipes/gaussian/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/gaussian/core.py` & `quacc-0.7.6/src/quacc/recipes/gaussian/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/gulp/_base.py` & `quacc-0.7.6/src/quacc/recipes/gulp/_base.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     library: str | None = None,
     keyword_defaults: list[str] | None = None,
     option_defaults: list[str] | None = None,
     keyword_swaps: list[str] | None = None,
     option_swaps: list[str] | None = None,
     additional_fields: dict[str, Any] | None = None,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
+    **calc_kwargs,
 ) -> RunSchema:
     """
     Base job function for GULP recipes.
 
     Parameters
     ----------
     atoms
@@ -58,14 +59,16 @@
         Dictionary of custom `options` kwargs for the GULP calculator. To remove entries
         from the defaults, put a `#` in front of the name. For a list of
         available keys, refer to the `ase.calculators.gulp.GULP` calculator.
     additional_fields
         Additional field to supply to the summarizer.
     copy_files
         Files to copy (and decompress) from source to the runtime directory.
+    **calc_kwargs
+        Any other keyword arguments to pass to the `GULP` calculator.
 
     Returns
     -------
     RunSchema
         Dictionary of results from [quacc.schemas.ase.summarize_run][]
     """
     keyword_defaults = keyword_defaults or []
@@ -88,15 +91,19 @@
 
     gulp_keywords = " ".join(keywords)
     gulp_options = list(options)
 
     if SETTINGS.GULP_LIB:
         os.environ["GULP_LIB"] = str(SETTINGS.GULP_LIB)
     atoms.calc = GULP(
-        command=GULP_CMD, keywords=gulp_keywords, options=gulp_options, library=library
+        command=GULP_CMD,
+        keywords=gulp_keywords,
+        options=gulp_options,
+        library=library,
+        **calc_kwargs,
     )
     final_atoms = run_calc(
         atoms,
         geom_file=GEOM_FILE_PBC if atoms.pbc.any() else GEOM_FILE_NOPBC,
         copy_files=copy_files,
     )
```

### Comparing `quacc-0.7.5/src/quacc/recipes/gulp/core.py` & `quacc-0.7.6/src/quacc/recipes/gulp/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/lj/core.py` & `quacc-0.7.6/src/quacc/recipes/lj/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/mlp/_base.py` & `quacc-0.7.6/src/quacc/recipes/mlp/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/mlp/core.py` & `quacc-0.7.6/src/quacc/recipes/mlp/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/mlp/phonons.py` & `quacc-0.7.6/src/quacc/recipes/mlp/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/newtonnet/core.py` & `quacc-0.7.6/src/quacc/recipes/newtonnet/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/newtonnet/ts.py` & `quacc-0.7.6/src/quacc/recipes/newtonnet/ts.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/onetep/_base.py` & `quacc-0.7.6/src/quacc/recipes/onetep/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         Files to copy (and decompress) from source to the runtime directory.
 
     Returns
     -------
     RunSchema
         Dictionary of results from [quacc.schemas.ase.summarize_run][]
     """
-    atoms.calc = _prep_calculator(calc_defaults=calc_defaults, calc_swaps=calc_swaps)
+    atoms.calc = prep_calculator(calc_defaults=calc_defaults, calc_swaps=calc_swaps)
     final_atoms = run_calc(atoms, copy_files=copy_files)
 
     return summarize_run(final_atoms, atoms, additional_fields=additional_fields)
 
 
 def run_and_summarize_opt(
     atoms: Atoms,
@@ -92,22 +92,22 @@
     Returns
     -------
     RunSchema
         Dictionary of results from [quacc.schemas.ase.summarize_run][]
     """
     opt_flags = recursive_dict_merge(opt_defaults, opt_params)
 
-    atoms.calc = _prep_calculator(calc_defaults=calc_defaults, calc_swaps=calc_swaps)
+    atoms.calc = prep_calculator(calc_defaults=calc_defaults, calc_swaps=calc_swaps)
 
     dyn = run_opt(atoms, copy_files=copy_files, **opt_flags)
 
     return summarize_opt_run(dyn, additional_fields=additional_fields)
 
 
-def _prep_calculator(
+def prep_calculator(
     calc_defaults: dict[str, Any] | None = None,
     calc_swaps: dict[str, Any] | None = None,
 ) -> Onetep:
     """
     Prepare the Onetep calculator.
 
     Parameters
```

### Comparing `quacc-0.7.5/src/quacc/recipes/onetep/core.py` & `quacc-0.7.6/src/quacc/recipes/onetep/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/orca/_base.py` & `quacc-0.7.6/src/quacc/recipes/orca/_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     spin_multiplicity: int = 1,
     default_inputs: list[str] | None = None,
     default_blocks: list[str] | None = None,
     input_swaps: list[str] | None = None,
     block_swaps: list[str] | None = None,
     additional_fields: dict[str, Any] | None = None,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
+    **calc_kwargs,
 ) -> cclibSchema:
     """
     Base job function for ORCA recipes.
 
     Parameters
     ----------
     atoms
@@ -57,27 +58,30 @@
     block_swaps
         List of orcablock swaps for the calculator. To remove entries
         from the defaults, put a `#` in front of the name.
     additional_fields
         Any additional fields to supply to the summarizer.
     copy_files
         Files to copy (and decompress) from source to the runtime directory.
+    **calc_kwargs
+        Any other keyword arguments to pass to the `ORCA` calculator.
 
     Returns
     -------
     cclibSchema
         Dictionary of results
     """
-    atoms.calc = _prep_calculator(
+    atoms.calc = prep_calculator(
         charge=charge,
         spin_multiplicity=spin_multiplicity,
         default_inputs=default_inputs,
         default_blocks=default_blocks,
         input_swaps=input_swaps,
         block_swaps=block_swaps,
+        **calc_kwargs,
     )
 
     atoms = run_calc(atoms, geom_file=GEOM_FILE, copy_files=copy_files)
 
     return cclib_summarize_run(atoms, LOG_FILE, additional_fields=additional_fields)
 
 
@@ -89,14 +93,15 @@
     default_blocks: list[str] | None = None,
     input_swaps: list[str] | None = None,
     block_swaps: list[str] | None = None,
     opt_defaults: dict[str, Any] | None = None,
     opt_params: dict[str, Any] | None = None,
     additional_fields: dict[str, Any] | None = None,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
+    **calc_kwargs,
 ) -> cclibASEOptSchema:
     """
     Base job function for ORCA recipes with ASE optimizer.
 
     Parameters
     ----------
     atoms
@@ -119,41 +124,45 @@
         Default arguments for the ASE optimizer.
     opt_params
         Dictionary of custom kwargs for [quacc.runners.ase.run_opt][]
     additional_fields
         Any additional fields to supply to the summarizer.
     copy_files
         Files to copy (and decompress) from source to the runtime directory.
+    **calc_kwargs
+        Any other keyword arguments to pass to the `ORCA` calculator.
 
     Returns
     -------
     cclibASEOptSchema
         Dictionary of results
     """
-    atoms.calc = _prep_calculator(
+    atoms.calc = prep_calculator(
         charge=charge,
         spin_multiplicity=spin_multiplicity,
         default_inputs=default_inputs,
         default_blocks=default_blocks,
         input_swaps=input_swaps,
         block_swaps=block_swaps,
+        **calc_kwargs,
     )
 
     opt_flags = recursive_dict_merge(opt_defaults, opt_params)
     dyn = run_opt(atoms, copy_files=copy_files, **opt_flags)
     return summarize_cclib_opt_run(dyn, LOG_FILE, additional_fields=additional_fields)
 
 
-def _prep_calculator(
+def prep_calculator(
     charge: int = 0,
     spin_multiplicity: int = 1,
     default_inputs: list[str] | None = None,
     default_blocks: list[str] | None = None,
     input_swaps: list[str] | None = None,
     block_swaps: list[str] | None = None,
+    **calc_kwargs,
 ) -> ORCA:
     """
     Prepare the ORCA calculator.
 
     Parameters
     ----------
     charge
@@ -166,14 +175,16 @@
         Default block input parameters.
     input_swaps
         List of orcasimpleinput swaps for the calculator. To remove entries
         from the defaults, put a `#` in front of the name.
     block_swaps
         List of orcablock swaps for the calculator. To remove entries
         from the defaults, put a `#` in front of the name.
+    **calc_kwargs
+        Any other keyword arguments to pass to the `ORCA` calculator.
 
     Returns
     -------
     ORCA
         The ORCA calculator
     """
     inputs = merge_list_params(default_inputs, input_swaps)
@@ -185,8 +196,9 @@
 
     return ORCA(
         profile=OrcaProfile(SETTINGS.ORCA_CMD),
         charge=charge,
         mult=spin_multiplicity,
         orcasimpleinput=orcasimpleinput,
         orcablocks=orcablocks,
+        **calc_kwargs,
     )
```

### Comparing `quacc-0.7.5/src/quacc/recipes/orca/core.py` & `quacc-0.7.6/src/quacc/recipes/orca/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/psi4/_base.py` & `quacc-0.7.6/src/quacc/recipes/psi4/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/psi4/core.py` & `quacc-0.7.6/src/quacc/recipes/psi4/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 def static_job(
     atoms: Atoms,
     charge: int = 0,
     spin_multiplicity: int = 1,
     method: str = "wb97x-v",
     basis: str = "def2-tzvp",
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
-    **kwargs,
+    **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a single-point calculation.
 
     Parameters
     ----------
     atoms
@@ -45,15 +45,15 @@
         Multiplicity of the system.
     method
         The level of theory to use.
     basis
         Basis set
     copy_files
         Files to copy (and decompress) from source to the runtime directory.
-    **kwargs
+    **calc_kwargs
         Custom kwargs for the Psi4 calculator. Set a value to
         `quacc.Remove` to remove a pre-existing key entirely. For a list of available
         keys, refer to the [ase.calculators.psi4.Psi4][] calculator.
 
     Returns
     -------
     RunSchema
@@ -70,11 +70,11 @@
         "reference": "uks" if spin_multiplicity > 1 else "rks",
     }
     return run_and_summarize(
         atoms,
         charge=charge,
         spin_multiplicity=spin_multiplicity,
         calc_defaults=calc_defaults,
-        calc_swaps=kwargs,
+        calc_swaps=calc_kwargs,
         additional_fields={"name": "Psi4 Static"},
         copy_files=copy_files,
     )
```

### Comparing `quacc-0.7.5/src/quacc/recipes/qchem/_base.py` & `quacc-0.7.6/src/quacc/recipes/qchem/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/qchem/core.py` & `quacc-0.7.6/src/quacc/recipes/qchem/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/qchem/ts.py` & `quacc-0.7.6/src/quacc/recipes/qchem/ts.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/tblite/core.py` & `quacc-0.7.6/src/quacc/recipes/tblite/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/tblite/phonons.py` & `quacc-0.7.6/src/quacc/recipes/tblite/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/vasp/_base.py` & `quacc-0.7.6/src/quacc/recipes/vasp/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/vasp/core.py` & `quacc-0.7.6/src/quacc/recipes/vasp/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/vasp/mp.py` & `quacc-0.7.6/src/quacc/recipes/vasp/mp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/vasp/qmof.py` & `quacc-0.7.6/src/quacc/recipes/vasp/qmof.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/recipes/vasp/slabs.py` & `quacc-0.7.6/src/quacc/recipes/vasp/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/runners/ase.py` & `quacc-0.7.6/src/quacc/runners/ase.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/runners/phonons.py` & `quacc-0.7.6/src/quacc/runners/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/runners/prep.py` & `quacc-0.7.6/src/quacc/runners/prep.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/runners/thermo.py` & `quacc-0.7.6/src/quacc/runners/thermo.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/schemas/_aliases/ase.py` & `quacc-0.7.6/src/quacc/schemas/_aliases/ase.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/schemas/_aliases/atoms.py` & `quacc-0.7.6/src/quacc/schemas/_aliases/atoms.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/schemas/_aliases/cclib.py` & `quacc-0.7.6/src/quacc/schemas/_aliases/cclib.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/schemas/_aliases/emmet.py` & `quacc-0.7.6/src/quacc/schemas/_aliases/emmet.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/schemas/_aliases/phonons.py` & `quacc-0.7.6/src/quacc/schemas/_aliases/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/schemas/_aliases/vasp.py` & `quacc-0.7.6/src/quacc/schemas/_aliases/vasp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/schemas/ase.py` & `quacc-0.7.6/src/quacc/schemas/ase.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/schemas/atoms.py` & `quacc-0.7.6/src/quacc/schemas/atoms.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/schemas/cclib.py` & `quacc-0.7.6/src/quacc/schemas/cclib.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/schemas/phonons.py` & `quacc-0.7.6/src/quacc/schemas/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/schemas/prep.py` & `quacc-0.7.6/src/quacc/schemas/prep.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/schemas/vasp.py` & `quacc-0.7.6/src/quacc/schemas/vasp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/settings.py` & `quacc-0.7.6/src/quacc/settings.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/utils/dicts.py` & `quacc-0.7.6/src/quacc/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/utils/files.py` & `quacc-0.7.6/src/quacc/utils/files.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Utility functions for file and path handling."""
 
 from __future__ import annotations
 
 import contextlib
 import logging
+import os
 import socket
 from copy import deepcopy
 from datetime import datetime, timezone
 from pathlib import Path
 from random import randint
 from shutil import copy
 from typing import TYPE_CHECKING
@@ -284,7 +285,25 @@
         Full URI path, e.g., "fileserver.host.com:/full/path/of/dir_name".
     """
     fullpath = Path(directory).expanduser().resolve()
     hostname = socket.gethostname()
     with contextlib.suppress(socket.gaierror, socket.herror):
         hostname = socket.gethostbyaddr(hostname)[0]
     return f"{hostname}:{fullpath}"
+
+
+def safe_decompress_dir(path: str | Path) -> None:
+    """
+    Recursively decompresses all files in a directory.
+    This is a wrapper around the `decompress_file` function.
+
+
+    Args:
+        path (str | Path): Path to parent directory.
+    """
+    path = Path(path)
+    for parent, _, files in os.walk(path):
+        for f in files:
+            try:
+                decompress_file(Path(parent, f))
+            except FileNotFoundError:
+                logger.debug(f"Cannot find {f} in {parent}. Skipping.")
```

### Comparing `quacc-0.7.5/src/quacc/utils/kpts.py` & `quacc-0.7.6/src/quacc/utils/kpts.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/utils/lists.py` & `quacc-0.7.6/src/quacc/utils/lists.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/wflow_tools/customizers.py` & `quacc-0.7.6/src/quacc/wflow_tools/customizers.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/wflow_tools/db.py` & `quacc-0.7.6/src/quacc/wflow_tools/db.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc/wflow_tools/decorators.py` & `quacc-0.7.6/src/quacc/wflow_tools/decorators.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.5/src/quacc.egg-info/PKG-INFO` & `quacc-0.7.6/src/quacc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quacc
-Version: 0.7.5
+Version: 0.7.6
 Summary: A platform to enable high-throughput, database-driven quantum chemistry and computational materials science
 Author-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 Maintainer-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 License: BSD-3
 Project-URL: repository, https://github.com/Quantum-Accelerators/quacc
 Project-URL: documentation, https://quantum-accelerators.github.io/quacc/
 Project-URL: changelog, https://github.com/Quantum-Accelerators/quacc/blob/main/CHANGELOG.md
```

### Comparing `quacc-0.7.5/src/quacc.egg-info/SOURCES.txt` & `quacc-0.7.6/src/quacc.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 src/quacc/calculators/vasp/params.py
 src/quacc/calculators/vasp/vasp.py
 src/quacc/calculators/vasp/vasp_custodian.py
 src/quacc/calculators/vasp/presets/BulkSet.yaml
 src/quacc/calculators/vasp/presets/QMOFSet.yaml
 src/quacc/calculators/vasp/presets/SlabSet.yaml
 src/quacc/calculators/vasp/presets/__init__.py
-src/quacc/calculators/vasp/presets/magmoms_MP.yaml
 src/quacc/calculators/vasp/presets/magmoms_base.yaml
 src/quacc/calculators/vasp/presets/magmoms_qmof.yaml
 src/quacc/calculators/vasp/presets/setups_pbe54.yaml
 src/quacc/calculators/vasp/presets/setups_qmof.yaml
 src/quacc/recipes/__init__.py
 src/quacc/recipes/common/__init__.py
 src/quacc/recipes/common/defects.py
```

### Comparing `quacc-0.7.5/src/quacc.egg-info/requires.txt` & `quacc-0.7.6/src/quacc.egg-info/requires.txt`

 * *Files identical despite different names*

