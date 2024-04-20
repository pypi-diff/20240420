# Comparing `tmp/contactmechanics-1.2.0.tar.gz` & `tmp/contactmechanics-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contactmechanics-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "contactmechanics-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `contactmechanics-1.2.0.tar` & `contactmechanics-1.3.0.tar`

### file list

```diff
@@ -1,105 +1,30 @@
--rw-r--r--   0        0        0      323 2024-01-14 16:51:02.633499 contactmechanics-1.2.0/.check_mufft_capabilities.py
--rw-r--r--   0        0        0      710 2024-01-14 16:51:02.633499 contactmechanics-1.2.0/.check_netcdf_capabilities.py
--rw-r--r--   0        0        0       30 2024-01-14 16:51:02.633499 contactmechanics-1.2.0/.gitattributes
--rw-r--r--   0        0        0      467 2024-01-14 16:51:02.633499 contactmechanics-1.2.0/.github/workflows/flake8.yml
--rw-r--r--   0        0        0     2206 2024-01-14 16:51:02.633499 contactmechanics-1.2.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2454 2024-01-14 16:51:02.633499 contactmechanics-1.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1597 2024-01-14 16:51:02.633499 contactmechanics-1.2.0/.github/workflows/test_examples.yml
--rw-r--r--   0        0        0      344 2024-01-14 16:51:02.633499 contactmechanics-1.2.0/.gitignore
--rw-r--r--   0        0        0      390 2024-01-14 16:51:02.633499 contactmechanics-1.2.0/AUTHORS
--rwxr-xr-x   0        0        0    14043 2024-01-14 16:51:02.633499 contactmechanics-1.2.0/ContactMechanics/ChangeLog.md
--rwxr-xr-x   0        0        0    25054 2024-01-14 16:51:02.633499 contactmechanics-1.2.0/ContactMechanics/CommandLineInterface/HardWall.py
--rw-r--r--   0        0        0     1112 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/ContactMechanics/CommandLineInterface/__init__.py
--rw-r--r--   0        0        0     2684 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/ContactMechanics/DiscoverVersion.py
--rw-r--r--   0        0        0    42973 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/ContactMechanics/FFTElasticHalfSpace.py
--rw-r--r--   0        0        0     7130 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/ContactMechanics/Factory.py
--rw-r--r--   0        0        0    10648 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/ContactMechanics/GreensFunctions/Anisotropic.py
--rw-r--r--   0        0        0     2999 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/ContactMechanics/GreensFunctions/Isotropic.py
--rw-r--r--   0        0        0     1283 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/ContactMechanics/GreensFunctions/__init__.py
--rw-r--r--   0        0        0    13683 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/ContactMechanics/IO/NetCDF.py
--rw-r--r--   0        0        0     1202 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/ContactMechanics/IO/__init__.py
--rwxr-xr-x   0        0        0    21146 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/ContactMechanics/Optimization/ConstrainedConjugateGradients.py
--rw-r--r--   0        0        0     1280 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/ContactMechanics/Optimization/__init__.py
--rw-r--r--   0        0        0    13994 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/ContactMechanics/PipelineFunction.py
--rwxr-xr-x   0        0        0     2606 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/ContactMechanics/PlasticSystemSpecialisations.py
--rw-r--r--   0        0        0     9614 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/ContactMechanics/ReferenceSolutions/Cone.py
--rwxr-xr-x   0        0        0     5213 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/ContactMechanics/ReferenceSolutions/GreenwoodTripp.py
--rw-r--r--   0        0        0    15578 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/ContactMechanics/ReferenceSolutions/Hertz.py
--rwxr-xr-x   0        0        0     6878 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/ContactMechanics/ReferenceSolutions/Westergaard.py
--rw-r--r--   0        0        0     1210 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/ContactMechanics/ReferenceSolutions/__init__.py
--rw-r--r--   0        0        0     6162 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/ContactMechanics/Substrates.py
--rwxr-xr-x   0        0        0    31880 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/ContactMechanics/Systems.py
--rw-r--r--   0        0        0     6778 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/ContactMechanics/Tools/Logger.py
--rw-r--r--   0        0        0     1271 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/ContactMechanics/Tools/__init__.py
--rw-r--r--   0        0        0     4940 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/ContactMechanics/Tools/common.py
--rw-r--r--   0        0        0     1733 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/ContactMechanics/__init__.py
--rw-r--r--   0        0        0     4801 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/ContactMechanics/test_surface_topography.py
--rw-r--r--   0        0        0     1040 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/LICENSE.md
--rw-r--r--   0        0        0     3127 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/README.md
--rw-r--r--   0        0        0     1990 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/commandline/plasticplot.plg
--rw-r--r--   0        0        0     1958 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/commandline/plot.plg
--rwxr-xr-x   0        0        0     2715 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/commandline/plotacf.py
--rwxr-xr-x   0        0        0     2740 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/commandline/plotmap.py
--rwxr-xr-x   0        0        0     2889 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/commandline/plotpsd.py
--rwxr-xr-x   0        0        0     1969 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/commandline/printrms.py
--rw-r--r--   0        0        0    17378 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/docs/Figures/fig_kinematics.svg
--rw-r--r--   0        0        0    24486 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/docs/Figures/geometry.svg
--rw-r--r--   0        0        0    22753 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/docs/Figures/geometry_pdf_tex.svg
--rw-r--r--   0        0        0      601 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/docs/Makefile
--rw-r--r--   0        0        0     5525 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/docs/conf.py
--rw-r--r--   0        0        0     5613 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/docs/contributing.rst
--rw-r--r--   0        0        0      322 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/docs/development.rst
--rw-r--r--   0        0        0     2104 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/docs/index.rst
--rw-r--r--   0        0        0     1145 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/docs/installation.rst
--rw-r--r--   0        0        0      808 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/docs/make.bat
--rw-r--r--   0        0        0     1280 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/docs/testing.rst
--rw-r--r--   0        0        0     1640 2024-01-14 16:51:02.637499 contactmechanics-1.2.0/docs/usage.rst
--rw-r--r--   0        0        0   495286 2024-01-14 16:51:02.641499 contactmechanics-1.2.0/examples/Hardwall_Simulation.ipynb
--rw-r--r--   0        0        0      131 2024-01-14 16:51:02.641499 contactmechanics-1.2.0/examples/check_examples.sh
--rw-r--r--   0        0        0     6892 2024-01-14 16:51:02.641499 contactmechanics-1.2.0/examples/constrained_conjugate_gradients.ipynb
--rw-r--r--   0        0        0     1642 2024-01-14 16:51:02.641499 contactmechanics-1.2.0/examples/contact_area_analysis.py
--rw-r--r--   0        0        0     4363 2024-01-14 16:51:02.641499 contactmechanics-1.2.0/examples/decoupling.py
--rw-r--r--   0        0        0    19250 2024-01-14 16:51:02.641499 contactmechanics-1.2.0/examples/easy_hardwall_simulation.ipynb
--rwxr-xr-x   0        0        0     4925 2024-01-14 16:51:02.641499 contactmechanics-1.2.0/examples/moving_contact.py
--rw-r--r--   0        0        0   650758 2024-01-14 16:51:02.645499 contactmechanics-1.2.0/examples/plastic_simulation_cone.ipynb
--rw-r--r--   0        0        0     3045 2024-01-14 16:51:02.645499 contactmechanics-1.2.0/examples/plot_greens_function.py
--rw-r--r--   0        0        0      155 2024-01-14 16:51:02.645499 contactmechanics-1.2.0/examples/run_examples.sh
--rw-r--r--   0        0        0    13486 2024-01-14 16:51:02.645499 contactmechanics-1.2.0/examples/simple_polonsky_keer.py
--rw-r--r--   0        0        0  6718237 2024-01-14 16:51:02.673499 contactmechanics-1.2.0/examples/surface1.out
--rw-r--r--   0        0        0  6581827 2024-01-14 16:51:02.701499 contactmechanics-1.2.0/examples/surface2.out
--rw-r--r--   0        0        0     7718 2024-01-14 16:51:02.701499 contactmechanics-1.2.0/long_tests/test_constrained_conjugate_gradients.py
--rw-r--r--   0        0        0     3369 2024-01-14 16:51:02.705499 contactmechanics-1.2.0/maintenance/copyright.py
--rw-r--r--   0        0        0     1492 2024-01-14 16:51:02.705499 contactmechanics-1.2.0/maintenance/replace_header.py
--rw-r--r--   0        0        0      350 2024-01-14 16:51:02.705499 contactmechanics-1.2.0/maintenance/update_license_headers.sh
--rw-r--r--   0        0        0     1355 2024-01-14 16:51:02.705499 contactmechanics-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       91 2024-01-14 16:51:02.705499 contactmechanics-1.2.0/pytest.ini
--rw-r--r--   0        0        0      353 2024-01-14 16:51:02.705499 contactmechanics-1.2.0/run-tests.py
--rw-r--r--   0        0        0      133 2024-01-14 16:51:02.705499 contactmechanics-1.2.0/setup.cfg
--rw-r--r--   0        0        0     1603 2024-01-14 16:51:02.705499 contactmechanics-1.2.0/snippets/eval_drep.py
--rwxr-xr-x   0        0        0     1343 2024-01-14 16:51:02.705499 contactmechanics-1.2.0/snippets/plot_area_vs_load.py
--rw-r--r--   0        0        0     1190 2024-01-14 16:51:02.705499 contactmechanics-1.2.0/test/GreensFunctions/__init__.py
--rw-r--r--   0        0        0     1978 2024-01-14 16:51:02.705499 contactmechanics-1.2.0/test/GreensFunctions/test_anisotropic.py
--rw-r--r--   0        0        0     3700 2024-01-14 16:51:02.705499 contactmechanics-1.2.0/test/ReferenceSolutions/test_reference_solutions.py
--rw-r--r--   0        0        0     1010 2024-01-14 16:51:02.705499 contactmechanics-1.2.0/test/ReferenceSolutions/test_westergaard.py
--rw-r--r--   0        0        0        0 2024-01-14 16:51:02.705499 contactmechanics-1.2.0/test/__init__.py
--rw-r--r--   0        0        0      825 2024-01-14 16:51:02.705499 contactmechanics-1.2.0/test/_test_parallel_testing.py
--rw-r--r--   0        0        0     1812 2024-01-14 16:51:02.705499 contactmechanics-1.2.0/test/commandline/test_hard_wall.py
--rw-r--r--   0        0        0     3016 2024-01-14 16:51:02.705499 contactmechanics-1.2.0/test/conftest.py
--rw-r--r--   0        0        0  6718237 2024-01-14 16:51:02.733500 contactmechanics-1.2.0/test/surface1.out
--rw-r--r--   0        0        0     3229 2024-01-14 16:51:02.733500 contactmechanics-1.2.0/test/test_ccg_without_restart_nonperiodic.py
--rw-r--r--   0        0        0      660 2024-01-14 16:51:02.733500 contactmechanics-1.2.0/test/test_cg.py
--rw-r--r--   0        0        0    21259 2024-01-14 16:51:02.733500 contactmechanics-1.2.0/test/test_fft_elastic_half_space.py
--rw-r--r--   0        0        0     3376 2024-01-14 16:51:02.733500 contactmechanics-1.2.0/test/test_flat_punch.py
--rw-r--r--   0        0        0     8830 2024-01-14 16:51:02.733500 contactmechanics-1.2.0/test/test_hertz.py
--rw-r--r--   0        0        0     8405 2024-01-14 16:51:02.733500 contactmechanics-1.2.0/test/test_mpi_free_elastic_half_space.py
--rw-r--r--   0        0        0    14393 2024-01-14 16:51:02.733500 contactmechanics-1.2.0/test/test_mpi_periodic_elastic_half_space.py
--rw-r--r--   0        0        0     3034 2024-01-14 16:51:02.733500 contactmechanics-1.2.0/test/test_mpi_system.py
--rw-r--r--   0        0        0     4933 2024-01-14 16:51:02.733500 contactmechanics-1.2.0/test/test_mpi_westergaard.py
--rw-r--r--   0        0        0     7603 2024-01-14 16:51:02.733500 contactmechanics-1.2.0/test/test_numpi_ccgs.py
--rw-r--r--   0        0        0     1903 2024-01-14 16:51:02.733500 contactmechanics-1.2.0/test/test_periodic.py
--rw-r--r--   0        0        0     5209 2024-01-14 16:51:02.733500 contactmechanics-1.2.0/test/test_pipeline.py
--rw-r--r--   0        0        0     8552 2024-01-14 16:51:02.733500 contactmechanics-1.2.0/test/test_plastic.py
--rw-r--r--   0        0        0     7294 2024-01-14 16:51:02.733500 contactmechanics-1.2.0/test/test_primal_dual_objective.py
--rw-r--r--   0        0        0     2312 2024-01-14 16:51:02.733500 contactmechanics-1.2.0/test/test_tools.py
--rw-r--r--   0        0        0     5635 2024-01-14 16:51:02.733500 contactmechanics-1.2.0/test/test_westergaard.py
--rw-r--r--   0        0        0     4470 1970-01-01 00:00:00.000000 contactmechanics-1.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0    14267 2024-04-20 18:13:09.678057 contactmechanics-1.3.0/ContactMechanics/ChangeLog.md
+-rwxr-xr-x   0        0        0    25054 2024-04-20 18:13:09.678057 contactmechanics-1.3.0/ContactMechanics/CommandLineInterface/HardWall.py
+-rw-r--r--   0        0        0     1112 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/ContactMechanics/CommandLineInterface/__init__.py
+-rw-r--r--   0        0        0    42973 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/ContactMechanics/FFTElasticHalfSpace.py
+-rw-r--r--   0        0        0     7130 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/ContactMechanics/Factory.py
+-rw-r--r--   0        0        0    10648 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/ContactMechanics/GreensFunctions/Anisotropic.py
+-rw-r--r--   0        0        0     2999 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/ContactMechanics/GreensFunctions/Isotropic.py
+-rw-r--r--   0        0        0     1283 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/ContactMechanics/GreensFunctions/__init__.py
+-rw-r--r--   0        0        0    13683 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/ContactMechanics/IO/NetCDF.py
+-rw-r--r--   0        0        0     1202 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/ContactMechanics/IO/__init__.py
+-rwxr-xr-x   0        0        0    21146 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/ContactMechanics/Optimization/ConstrainedConjugateGradients.py
+-rw-r--r--   0        0        0     1280 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/ContactMechanics/Optimization/__init__.py
+-rw-r--r--   0        0        0    13994 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/ContactMechanics/PipelineFunction.py
+-rwxr-xr-x   0        0        0     2606 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/ContactMechanics/PlasticSystemSpecialisations.py
+-rw-r--r--   0        0        0     9614 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/ContactMechanics/ReferenceSolutions/Cone.py
+-rwxr-xr-x   0        0        0     5213 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/ContactMechanics/ReferenceSolutions/GreenwoodTripp.py
+-rw-r--r--   0        0        0    15578 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/ContactMechanics/ReferenceSolutions/Hertz.py
+-rwxr-xr-x   0        0        0     6878 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/ContactMechanics/ReferenceSolutions/Westergaard.py
+-rw-r--r--   0        0        0     1210 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/ContactMechanics/ReferenceSolutions/__init__.py
+-rw-r--r--   0        0        0     6162 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/ContactMechanics/Substrates.py
+-rwxr-xr-x   0        0        0    37679 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/ContactMechanics/Systems.py
+-rw-r--r--   0        0        0     6778 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/ContactMechanics/Tools/Logger.py
+-rw-r--r--   0        0        0     1271 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/ContactMechanics/Tools/__init__.py
+-rw-r--r--   0        0        0     4940 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/ContactMechanics/Tools/common.py
+-rw-r--r--   0        0        0     1848 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/ContactMechanics/__init__.py
+-rw-r--r--   0        0        0     4801 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/ContactMechanics/test_surface_topography.py
+-rw-r--r--   0        0        0     1040 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/LICENSE.md
+-rw-r--r--   0        0        0     3127 2024-04-20 18:13:09.682057 contactmechanics-1.3.0/README.md
+-rw-r--r--   0        0        0     1397 2024-04-20 18:13:09.746056 contactmechanics-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4501 1970-01-01 00:00:00.000000 contactmechanics-1.3.0/PKG-INFO
```

### Comparing `contactmechanics-1.2.0/ContactMechanics/ChangeLog.md` & `contactmechanics-1.3.0/ContactMechanics/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Change log for ContactMechanics
 ===============================
 
+v1.3.0 (20Apr24)
+----------------
+
+- API: Homogeneized solver naming convention to use hypens rather than
+  underscores
+- MAINT: Bumped NuMPI to 0.5.0
+- MAINT: Changed version discovery to use the `DiscoverVersion` package
+
 v1.2.0 (14Jan24)
 ----------------
 
 - MAINT: Compatiblity with SurfaceTopography 1.12.x
 - MAINT: Update NuMPI-dependency to 0.4.0 for modern build system
 - BUG: Fixed `make_contact_system` pipeline function
```

### Comparing `contactmechanics-1.2.0/ContactMechanics/CommandLineInterface/HardWall.py` & `contactmechanics-1.3.0/ContactMechanics/CommandLineInterface/HardWall.py`

 * *Files identical despite different names*

### Comparing `contactmechanics-1.2.0/ContactMechanics/CommandLineInterface/__init__.py` & `contactmechanics-1.3.0/ContactMechanics/CommandLineInterface/__init__.py`

 * *Files identical despite different names*

### Comparing `contactmechanics-1.2.0/ContactMechanics/FFTElasticHalfSpace.py` & `contactmechanics-1.3.0/ContactMechanics/FFTElasticHalfSpace.py`

 * *Files identical despite different names*

### Comparing `contactmechanics-1.2.0/ContactMechanics/Factory.py` & `contactmechanics-1.3.0/ContactMechanics/Factory.py`

 * *Files identical despite different names*

### Comparing `contactmechanics-1.2.0/ContactMechanics/GreensFunctions/Anisotropic.py` & `contactmechanics-1.3.0/ContactMechanics/GreensFunctions/Anisotropic.py`

 * *Files identical despite different names*

### Comparing `contactmechanics-1.2.0/ContactMechanics/GreensFunctions/Isotropic.py` & `contactmechanics-1.3.0/ContactMechanics/GreensFunctions/Isotropic.py`

 * *Files identical despite different names*

### Comparing `contactmechanics-1.2.0/ContactMechanics/GreensFunctions/__init__.py` & `contactmechanics-1.3.0/ContactMechanics/GreensFunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `contactmechanics-1.2.0/ContactMechanics/IO/NetCDF.py` & `contactmechanics-1.3.0/ContactMechanics/IO/NetCDF.py`

 * *Files identical despite different names*

### Comparing `contactmechanics-1.2.0/ContactMechanics/IO/__init__.py` & `contactmechanics-1.3.0/ContactMechanics/IO/__init__.py`

 * *Files identical despite different names*

### Comparing `contactmechanics-1.2.0/ContactMechanics/Optimization/ConstrainedConjugateGradients.py` & `contactmechanics-1.3.0/ContactMechanics/Optimization/ConstrainedConjugateGradients.py`

 * *Files identical despite different names*

### Comparing `contactmechanics-1.2.0/ContactMechanics/Optimization/__init__.py` & `contactmechanics-1.3.0/ContactMechanics/Optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `contactmechanics-1.2.0/ContactMechanics/PipelineFunction.py` & `contactmechanics-1.3.0/ContactMechanics/PipelineFunction.py`

 * *Files identical despite different names*

### Comparing `contactmechanics-1.2.0/ContactMechanics/PlasticSystemSpecialisations.py` & `contactmechanics-1.3.0/ContactMechanics/PlasticSystemSpecialisations.py`

 * *Files identical despite different names*

### Comparing `contactmechanics-1.2.0/ContactMechanics/ReferenceSolutions/Cone.py` & `contactmechanics-1.3.0/ContactMechanics/ReferenceSolutions/Cone.py`

 * *Files identical despite different names*

### Comparing `contactmechanics-1.2.0/ContactMechanics/ReferenceSolutions/GreenwoodTripp.py` & `contactmechanics-1.3.0/ContactMechanics/ReferenceSolutions/GreenwoodTripp.py`

 * *Files identical despite different names*

### Comparing `contactmechanics-1.2.0/ContactMechanics/ReferenceSolutions/Hertz.py` & `contactmechanics-1.3.0/ContactMechanics/ReferenceSolutions/Hertz.py`

 * *Files identical despite different names*

### Comparing `contactmechanics-1.2.0/ContactMechanics/ReferenceSolutions/Westergaard.py` & `contactmechanics-1.3.0/ContactMechanics/ReferenceSolutions/Westergaard.py`

 * *Files identical despite different names*

### Comparing `contactmechanics-1.2.0/ContactMechanics/ReferenceSolutions/__init__.py` & `contactmechanics-1.3.0/ContactMechanics/ReferenceSolutions/__init__.py`

 * *Files identical despite different names*

### Comparing `contactmechanics-1.2.0/ContactMechanics/Substrates.py` & `contactmechanics-1.3.0/ContactMechanics/Substrates.py`

 * *Files identical despite different names*

### Comparing `contactmechanics-1.2.0/ContactMechanics/Systems.py` & `contactmechanics-1.3.0/ContactMechanics/Systems.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,19 +29,18 @@
 """
 
 import abc
 
 import numpy as np
 import scipy
 import scipy.optimize as optim
-
-from NuMPI.Optimization import ccg_without_restart, ccg_with_restart
+import SurfaceTopography
+from NuMPI.Optimization import CCGWithoutRestart, CCGWithRestart
 from NuMPI.Tools import Reduction
 
-import SurfaceTopography
 from .FFTElasticHalfSpace import ElasticSubstrate
 from .Optimization import constrained_conjugate_gradients
 from .Tools import compare_containers
 
 
 class IncompatibleFormulationError(Exception):
     # pylint: disable=missing-docstring
@@ -453,16 +452,44 @@
         return (['energy',
                  'substrate force', ],
                 [self.energy,
                  -self.reduction.sum(self.substrate.force), ])
 
     def evaluate(self, disp, offset, pot=True, forces=False, logger=None):
         """
-        Compute the energies and forces in the system for a given displacement
-        field
+        Compute the energies and forces in the system for a given displacement field.
+
+        This method calculates the gap between the surface and the substrate by calling the `compute_gap` method.
+        It then computes the displacement field by calling the `compute` method of the substrate.
+
+        If potential energy is to be computed, it is set to the energy of the substrate. Otherwise, it is set to None.
+
+        If forces are to be computed, they are set to the force of the substrate. Otherwise, they are set to None.
+
+        If a logger is provided, it logs the current state of the system.
+
+        Parameters
+        ----------
+        disp : array_like
+            The displacement field for which the energies and forces are to be computed.
+        offset : float
+            The offset value to be used in the computation.
+        pot : bool, optional
+            If True, the potential energy in the system is also computed. Default is True.
+        forces : bool, optional
+            If True, the forces in the system are also computed. Default is False.
+        logger : Logger, optional
+            Logger object to log information at each iteration. Default is None.
+
+        Returns
+        -------
+        energy : float
+            Total energy of the system. If potential energy is not computed, it is None.
+        force : array_like
+            Forces in the system. If forces are not computed, they are None.
         """
         # attention: the substrate may have a higher nb_grid_pts than the gap
         # and the interaction (e.g. FreeElasticHalfSpace)
         self.gap = self.compute_gap(disp, offset)
         self.substrate.compute(disp, pot, forces)
 
         self.energy = self.substrate.energy if pot else None
@@ -470,33 +497,41 @@
             self.force = self.substrate.force
         else:
             self.force = None
 
         if logger is not None:
             logger.st(*self.logger_input())
 
-        return (self.energy, self.force)
+        return self.energy, self.force
 
     def objective(self, offset, disp0=None, gradient=False, logger=None):
         """
         This helper method exposes a scipy.optimize-friendly interface to the
-        evaluate() method. Use this for optimization purposes, it makes sure
-        that the shape of disp is maintained and lets you set the offset and
-        'forces' flag without using scipy's cumbersome argument passing
-        interface. Returns a function of only disp
-        Parameters:
-        -----------
-        offset:
-            determines indentation depth
-        disp0:
-            unused variable, present only for interface compatibility
-            with inheriting classes
-        gradient: (default False)
-            whether the gradient is supposed to be
-            used
+        evaluate() method. It is used for optimization purposes and ensures
+        that the shape of displacement is maintained. It also allows setting the offset and
+        'forces' flag without using scipy's argument passing interface.
+
+        Parameters
+        ----------
+        offset : float
+            Determines the indentation depth.
+        disp0 : array_like, optional
+            Unused variable, present only for interface compatibility
+            with inheriting classes. Default is None.
+        gradient : bool, optional
+            If True, the gradient is supposed to be used. Default is False.
+        logger : Logger, optional
+            Logger object to log information at each iteration. Default is None.
+
+        Returns
+        -------
+        fun : function
+            A function of only displacement. If gradient is True, this function returns
+            the energy and the negative of the force when called with displacement.
+            If gradient is False, it returns only the energy.
         """
         # pylint: disable=arguments-differ
         res = self.substrate.nb_subdomain_grid_pts
         if gradient:
             def fun(disp):
                 # pylint: disable=missing-docstring
                 try:
@@ -509,27 +544,30 @@
                 # pylint: disable=missing-docstring
                 return self.evaluate(disp.reshape(res), offset, forces=False, logger=logger)[0]
 
         return fun
 
     def hessian_product(self, disp):
         """
-        computes the hessian product for objective
+        Computes the Hessian product for the objective function.
 
-        this is the same then primal_hessian_product
+        This method calculates the Hessian product by calling the `primal_hessian_product` method.
+        The Hessian product is the result of applying the Hessian matrix (second derivatives of the objective function)
+        to the displacement vector. This is used in optimization algorithms that utilize second-order information.
 
-        Parameters:
-        -----------
-        disp: float array
-            array of shape nb_subdomain_grid_pts or a flattened version of it
-
-        Returns:
-        --------
-        hessian product
+        Parameters
+        ----------
+        disp : array_like
+            The displacement vector to which the Hessian matrix is applied. It can be an array of shape
+            nb_subdomain_grid_pts or a flattened version of it.
 
+        Returns
+        -------
+        array_like
+            The Hessian product, which is the result of applying the Hessian matrix to the displacement vector.
         """
         return self.primal_hessian_product(disp)
 
     def minimize_proxy(self, solver=constrained_conjugate_gradients, **kwargs):
         """
         Convenience function. Eliminates boilerplate code for most minimisation
         problems by encapsulating the use of constrained minimisation.
@@ -567,48 +605,42 @@
             self.force = self.substrate.force = result.jac
             self.contact_zone = result.jac > 0
 
             self.substrate.check()
         return result
 
     def primal_objective(self, offset, gradient=True):
-        r"""To solve the primal objective using gap as the variable.
-        Can be fed directly to standard solvers ex: scipy solvers etc
-        and returns the elastic energy and it's gradient (negative of
-        the forces) as a function of the gap.
+        r"""
+        Solves the primal objective using gap as the variable. This function can be fed directly to standard solvers
+        such as scipy solvers etc. and returns the elastic energy and its gradient (negative of the forces) as a
+        function of the gap.
 
         Parameters
-        __________
-
-        gap : float
-            Gap between the contact surfaces.
+        ----------
         offset : float
             Constant value to add to the surface heights.
-        gradient : bool
-            Return gradient in addition to the energy.
-            (Default: True)
+        gradient : bool, optional
+            Return gradient in addition to the energy. Default is True.
 
         Returns
-        _______
+        -------
         energy : float
             Value of total energy.
         force : array_like
-            Value of the forces per surface node (only of gradient is true).
+            Value of the forces per surface node (only if gradient is True).
 
         Notes
-        _____
-
-        Objective:
+        -----
+        The objective function is defined as:
 
         .. math ::
 
             \min_u f(u) = 1/2 u_i K_{ij} u_j \\
             \\
             \nabla f = K_{ij} u_j \ \ \ \text{which is the Force.} \\
-
         """
 
         res = self.substrate.nb_subdomain_grid_pts
         if gradient:
             def fun(gap):
                 disp = gap.reshape(res) + self.surface.heights() + offset
                 try:
@@ -622,75 +654,89 @@
                 disp = gap.reshape(res) + self.surface.heights() + offset
                 return self.evaluate(
                     disp.reshape(res), offset, forces=False)[0]
 
         return fun
 
     def primal_hessian_product(self, gap):
-        """Returns the hessian product of the primal_objective function.
         """
-        inres = gap.shape
-        res = self.substrate.nb_subdomain_grid_pts
-        hessp = -self.substrate.evaluate_force(gap.reshape(res)).reshape(inres)
-        return hessp
-
-    def primal_minimize_proxy(self, offset, init_gap=None,
-                              solver='ccg_without_restart', gtol=1e-8, maxiter=1000):
+        Returns the hessian product of the primal_objective function.
 
-        """Convenience function. Eliminates boilerplate code for
-        Primal minimisation problem (gap as variable) by encapsulating the use of constrained
-        minimisation.
+        The hessian product is the result of applying the hessian matrix (second derivatives of the objective function)
+        to the gap vector. This is used in optimization algorithms that utilize second-order information.
 
         Parameters
-        __________
+        ----------
+        gap : array_like
+            The gap vector to which the hessian matrix is applied.
 
-        offset     : determines indentation depth
-
-        init_force : initial guess for force.
+        Returns
+        -------
+        hessp : array_like
+            The hessian product, which is the result of applying the hessian matrix to the gap vector.
 
-        solver     : 'ccg_without_restart', 'ccg_with_restart',
-        'l-bfgs-b'
+        Notes
+        -----
+        The hessian product is computed as the negative of the force evaluated at the reshaped gap vector.
+        """
+        inres = gap.shape  # Store        inres = gap.shape
+        res = self.substrate.nb_subdomain_grid_pts
+        hessp = -self.substrate.evaluate_force(gap.reshape(res)).reshape(inres)
+        return hessp
 
-        gtol       : float, optional
-                    Default value : 1e-8
+    def primal_minimize_proxy(self, offset, init_gap=None, solver='ccg-without-restart', gtol=1e-8, maxiter=1000):
+        """
+        This function is a convenience function that simplifies the process of
+        solving the primal minimisation problem where the gap is the variable.
+        It does this by encapsulating the use of constrained minimisation.
 
-        maxiter    : maximum number of iterations allowed for
-        convergence
+        Parameters
+        ----------
+        offset : float
+            This parameter determines the indentation depth.
+        init_gap : array_like, optional
+            This is the initial guess for the gap. If not provided, it defaults to None.
+        solver : str, optional
+            This is the solver to be used for the minimisation. It can be one of
+            'ccg-without-restart', 'ccg-with-restart', or 'l-bfgs-b'. If not provided,
+            it defaults to 'ccg-without-restart'.
+        gtol : float, optional
+            This is the gradient tolerance for the solver. If not provided, it defaults to 1e-8.
+        maxiter : int, optional
+            This is the maximum number of iterations allowed for the solver to converge.
+            If not provided, it defaults to 1000.
 
         Returns
-        _______
-
-        gap : gap or gardient value
-
-        force   : final force of the system at the solution
-
-        disp    : displacement of the system at the solution
+        -------
+        result : OptimizeResult
+            The result of the minimisation. It contains information about the optimisation
+            result, including the final gap, force, and displacement of the system at the solution.
         """
 
-        solvers = {'ccg_without_restart', 'ccg_with_restart', 'l-bfgs-b'}
+        solvers = {'ccg-without-restart', 'ccg-with-restart', 'l-bfgs-b'}
 
         if solver not in solvers:
             raise ValueError(
                 'Input correct solver name from {}'.format(solvers))
 
         self.disp = None
         self.force = None
         self.contact_zone = None
         self.init_gap = init_gap
 
         lbounds = np.zeros(self.init_gap.shape)
         bnds = self._reshape_bounds(lbounds, )
 
-        if solver == 'ccg_without_restart':
-            result = ccg_without_restart.constrained_conjugate_gradients(
+        if solver == 'ccg-without-restart':
+            result = CCGWithoutRestart.constrained_conjugate_gradients(
                 self.primal_objective(offset, gradient=True),
                 self.primal_hessian_product, x0=init_gap, gtol=gtol,
                 maxiter=maxiter)
-        elif solver == 'ccg_with_restart':
-            result = ccg_with_restart.constrained_conjugate_gradients(
+        elif solver == 'ccg-with-restart':
+            result = CCGWithRestart.constrained_conjugate_gradients(
                 self.primal_objective(offset, gradient=True),
                 self.primal_hessian_product, x0=init_gap, gtol=gtol,
                 maxiter=maxiter)
         elif solver == 'l-bfgs-b':
             result = optim.minimize(
                 self.primal_objective(offset, gradient=True),
                 self.shape_minimisation_input(self.init_gap),
@@ -706,64 +752,86 @@
             self.disp = self.gap + offset + self.surface.heights().reshape(
                 self.gap.shape)
 
         return result
 
     def evaluate_dual(self, press, offset, forces=False):
         """
-        Computes the energies and forces in the system for a given displacement
-        field
+        Computes the energies and forces in the system for a given pressure field.
+
+        This method calculates the displacement field corresponding to the given pressure field
+        by calling the `evaluate_disp` method of the substrate. The negative of the pressure field
+        is passed as an argument to the `evaluate_disp` method.
+
+        If forces are to be computed, the gradient is calculated as the difference between the displacement
+        and the sum of the surface heights and the offset. Otherwise, the gradient is set to None.
+
+        The energy is then computed as half the sum of the product of the pressure and displacement fields,
+        minus the sum of the product of the pressure and the sum of the surface heights and the offset.
+
+        Parameters
+        ----------
+        press : array_like
+            The pressure field for which the displacement field is to be computed.
+        offset : float
+            The offset value to be used in the computation.
+        forces : bool, optional
+            If True, the forces in the system are also computed. Default is False.
+
+        Returns
+        -------
+        energy : float
+            Total energy of the system.
+        gradient : array_like
+            Gradient, which is the difference between the displacement and the sum of the
+            surface heights and the offset. If forces are not computed, the gradient is None.
         """
         disp = self.substrate.evaluate_disp(-press)
         if forces:
             self.gradient = disp - self.surface.heights() - offset
         else:
             self.gradient = None
 
         self.energy = 1 / 2 * np.sum(press * disp) - np.sum(
             press * (self.surface.heights() + offset))
 
-        return (self.energy, self.gradient)
+        return self.energy, self.gradient
 
     def dual_objective(self, offset, gradient=True):
-        r"""Objective function to handle dual objective, i.e. the Legendre
+        r"""
+        Objective function to handle dual objective, i.e. the Legendre
         transformation from displacements as variable to pressures
         (the Lagrange multiplier) as variable.
 
         Parameters
-        __________
-        pressure : float
-                pressure between the contact surfaces.
+        ----------
         offset : float
-                constant value to add to the surface heights
-        pot : (default False)
-        gradient : (default True)
+            Constant value to add to the surface heights.
+        gradient : bool, optional
+            Whether to return the gradient in addition to the energy. Default is True.
 
         Returns
-        _______
+        -------
         energy : float
-                value of energy(scalar value).
-
-        gradient : float,array
-                value of gradient(array) or the value of gap.
+            Value of total energy.
+        gradient : array_like
+            Value of the gradient (array) or the value of gap (if gradient is True).
 
         Notes
-        _____
-        Objective:
+        -----
+        The objective function is defined as:
 
         .. math ::
 
             \min_\lambda \ q(\lambda) = \frac{1}{2}\lambda_i  K^{-1}_{ij} \lambda_j - \lambda_i h_i \\
             \\
             \nabla q = K^{-1}_{ij} \lambda_j - h_i \hspace{0.1cm}
             \text{which is,} \\
             \text{gap} = \text{displacement} - \text{height} \\
-
         """
-
         res = self.substrate.nb_domain_grid_pts
         if gradient:
             def fun(pressure):
                 try:
                     self.evaluate_dual(
                         pressure.reshape(res), offset, forces=True)
                 except ValueError as err:
@@ -774,72 +842,84 @@
         else:
             def fun(gap):
                 return self.evaluate(gap.reshape(res), forces=False)[0]
 
         return fun
 
     def dual_hessian_product(self, pressure):
-        r"""Returns the hessian product of the dual_objective function.
+        """
+        Returns the hessian product of the dual_objective function.
+
+        The hessian product is the result of applying the hessian matrix (second derivatives of the objective function)
+        to the pressure vector. This is used in optimization algorithms that utilize second-order information.
+
+        Parameters
+        ----------
+        pressure : array_like
+            The pressure vector to which the hessian matrix is applied.
+
+        Returns
+        -------
+        hessp : array_like
+            The hessian product, which is the result of applying the hessian matrix to the pressure vector.
         """
         inres = pressure.shape
         res = self.substrate.nb_subdomain_grid_pts
         hessp = self.substrate.evaluate_disp(-pressure.reshape(res))
         return hessp.reshape(inres)
 
-    def dual_minimize_proxy(self, offset, init_force=None,
-                            solver='ccg_without_restart', gtol=1e-8, maxiter=1000):
+    def dual_minimize_proxy(self, offset, init_force=None, solver='ccg-without-restart', gtol=1e-8, maxiter=1000):
         """
-        Convenience function. Eliminates boilerplate code for DUAL minimisation (pixel forces as variables)
-        problems by encapsulating the use of constrained minimisation.
+        Convenience function for DUAL minimisation (pixel forces as variables).
+        This function simplifies the process of solving the dual minimisation problem
+        by encapsulating the use of constrained minimisation.
 
         Parameters
-        __________
-
-        offset     : determines indentation depth
-
-        init_force : initial guess for force.
-
-        solver     : 'ccg_without_restart', 'ccg_with_restart', 'l-bfgs-b'
-
-        gtol       : float, optional
-                    Default value : 1e-8
-
-        maxiter    : maximum number of iterations allowed for convergence
+        ----------
+        offset : float
+            Determines the indentation depth.
+        init_force : array_like, optional
+            Initial guess for the force. If not provided, it defaults to None.
+        solver : str, optional
+            The solver to be used for the minimisation. It can be one of
+            'ccg-without-restart', 'ccg-with-restart', or 'l-bfgs-b'. If not provided,
+            it defaults to 'ccg-without-restart'.
+        gtol : float, optional
+            The gradient tolerance for the solver. If not provided, it defaults to 1e-8.
+        maxiter : int, optional
+            The maximum number of iterations allowed for the solver to converge.
+            If not provided, it defaults to 1000.
 
         Returns
-        _______
-
-        gap : gap or gardient value
-
-        force   : final force of the system at the solution
-
-        disp    : displacement of the system at the solution
+        -------
+        result : OptimizeResult
+            The result of the minimisation. It contains information about the optimisation
+            result, including the final gap, force, and displacement of the system at the solution.
         """
-
-        solvers = {'ccg_without_restart', 'ccg_with_restart', 'l-bfgs-b'}
+        solvers = {'ccg-without-restart', 'ccg-with-restart', 'l-bfgs-b'}
 
         if solver not in solvers:
             raise ValueError(
                 'Input correct solver name from {}'.format(solvers))
 
         self.disp = None
         self.force = None
         self.contact_zone = None
         self.init_force = init_force
 
         lbounds = np.zeros(self.init_force.shape)
         bnds = self._reshape_bounds(lbounds, )
 
-        if solver == 'ccg_without_restart':
-            result = ccg_without_restart.constrained_conjugate_gradients(
+        if solver == 'ccg-without-restart':
+            result = CCGWithoutRestart.constrained_conjugate_gradients(
                 self.dual_objective(offset, gradient=True),
                 self.dual_hessian_product, x0=init_force, gtol=gtol,
                 maxiter=maxiter)
-        elif solver == 'ccg_with_restart':
-            result = ccg_with_restart.constrained_conjugate_gradients(
+        elif solver == 'ccg-with-restart':
+            result = CCGWithRestart.constrained_conjugate_gradients(
                 self.dual_objective(offset, gradient=True),
                 self.dual_hessian_product, x0=init_force, gtol=gtol,
                 maxiter=maxiter)
         elif solver == 'l-bfgs-b':
             result = optim.minimize(
                 self.dual_objective(offset, gradient=True),
                 self.shape_minimisation_input(self.init_force),
```

### Comparing `contactmechanics-1.2.0/ContactMechanics/Tools/Logger.py` & `contactmechanics-1.3.0/ContactMechanics/Tools/Logger.py`

 * *Files identical despite different names*

### Comparing `contactmechanics-1.2.0/ContactMechanics/Tools/__init__.py` & `contactmechanics-1.3.0/ContactMechanics/Tools/__init__.py`

 * *Files identical despite different names*

### Comparing `contactmechanics-1.2.0/ContactMechanics/Tools/common.py` & `contactmechanics-1.3.0/ContactMechanics/Tools/common.py`

 * *Files identical despite different names*

### Comparing `contactmechanics-1.2.0/ContactMechanics/__init__.py` & `contactmechanics-1.3.0/ContactMechanics/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,19 @@
 # SOFTWARE.
 #
 
 """
 Defines all solid mechanics model used in ContactMechanics
 """
 
-from .DiscoverVersion import __version__  # noqa: F401
+from DiscoverVersion import get_version
 
 # These imports are required to register the analysis functions!
 from . import Factory  # noqa: F401
-from .Factory import make_system, make_plastic_system  # noqa: F401
-from .FFTElasticHalfSpace import PeriodicFFTElasticHalfSpace, FreeFFTElasticHalfSpace  # noqa: F401
-from .Substrates import Substrate, ElasticSubstrate, PlasticSubstrate  # noqa: F401
+from .Factory import make_plastic_system, make_system  # noqa: F401
+from .FFTElasticHalfSpace import FreeFFTElasticHalfSpace  # noqa: F401
+from .FFTElasticHalfSpace import PeriodicFFTElasticHalfSpace  # noqa: F401
 from .PipelineFunction import contact_mechanics  # noqa: F401
+from .Substrates import (ElasticSubstrate, PlasticSubstrate,  # noqa: F401
+                         Substrate)
+
+__version__ = get_version('ContactMechanics', __file__)
```

### Comparing `contactmechanics-1.2.0/ContactMechanics/test_surface_topography.py` & `contactmechanics-1.3.0/ContactMechanics/test_surface_topography.py`

 * *Files identical despite different names*

### Comparing `contactmechanics-1.2.0/LICENSE.md` & `contactmechanics-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `contactmechanics-1.2.0/README.md` & `contactmechanics-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `contactmechanics-1.2.0/pyproject.toml` & `contactmechanics-1.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["flit_core>=3.2"]
+requires = ["flit_core>=3.2", "DiscoverVersion"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ContactMechanics"
 description = "Efficient contact mechanics using elastic half-space methods"
 readme = "README.md"
 license = { file = "LICENSE.md" }
@@ -15,17 +15,18 @@
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python"
 ]
 requires-python = ">=3.8.0"
 dynamic = [ "version" ]
 dependencies = [
+    "DiscoverVersion",
     "numpy",
     "scipy>=1.9.0",
-    "NuMPI>=0.4.0",
+    "NuMPI>=0.5.0",
     "muSpectre>=0.25.1",
     "SurfaceTopography>=1.12.2",
     "netCDF4"
 ]
 
 [project.optional-dependencies]
 test = [
```

### Comparing `contactmechanics-1.2.0/PKG-INFO` & `contactmechanics-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: ContactMechanics
-Version: 1.2.0
+Version: 1.3.0
 Summary: Efficient contact mechanics using elastic half-space methods
 Author-email: Till Junge <till.junge@altermail.ch>, Lars Pastewka <lars.pastewka@imtek.uni-freiburg.de>, Antoine Sanner <antoine.sanner@imtek.uni-freiburg.de>
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
+Requires-Dist: DiscoverVersion
 Requires-Dist: numpy
 Requires-Dist: scipy>=1.9.0
-Requires-Dist: NuMPI>=0.4.0
+Requires-Dist: NuMPI>=0.5.0
 Requires-Dist: muSpectre>=0.25.1
 Requires-Dist: SurfaceTopography>=1.12.2
 Requires-Dist: netCDF4
 Requires-Dist: sphinx ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme ; extra == "docs"
 Requires-Dist: myst_nb ; extra == "docs"
 Requires-Dist: numpydoc ; extra == "docs"
```

