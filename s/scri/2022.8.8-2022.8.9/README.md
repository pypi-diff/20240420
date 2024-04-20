# Comparing `tmp/scri-2022.8.8.tar.gz` & `tmp/scri-2022.8.9.tar.gz`

## Comparing `scri-2022.8.8.tar` & `scri-2022.8.9.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 scri-2022.8.8/.readthedocs.yml
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 scri-2022.8.8/CITATION.cff
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 scri-2022.8.8/scri.bib
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 scri-2022.8.8/.github/scripts/parse_bump_rule.py
--rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 scri-2022.8.8/.github/workflows/build.yml
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 scri-2022.8.8/docs/.gitignore
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scri-2022.8.8/docs/Makefile
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 scri-2022.8.8/docs/README.md -> ../README.md
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 scri-2022.8.8/docs/api.rst
--rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 scri-2022.8.8/docs/conf.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 scri-2022.8.8/docs/environment.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scri-2022.8.8/docs/index.rst
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 scri-2022.8.8/docs/make.bat
--rw-r--r--   0        0        0    10936 2020-02-02 00:00:00.000000 scri-2022.8.8/docs/tutorial_abd.rst
--rw-r--r--   0        0        0    11070 2020-02-02 00:00:00.000000 scri-2022.8.8/docs/tutorial_bms.rst
--rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 scri-2022.8.8/docs/tutorial_extrapolation.rst
--rw-r--r--   0        0        0     9787 2020-02-02 00:00:00.000000 scri-2022.8.8/docs/tutorial_waveformmodes.rst
--rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/__version__.py
--rw-r--r--   0        0        0    25249 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/bms_transformations.py
--rw-r--r--   0        0        0    58879 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/extrapolation.py
--rw-r--r--   0        0        0    31544 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/flux.py
--rw-r--r--   0        0        0    21132 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/mode_calculations.py
--rw-r--r--   0        0        0     7928 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/modes_time_series.py
--rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/plotting.py
--rw-r--r--   0        0        0    16811 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/rotations.py
--rw-r--r--   0        0        0    31597 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/sample_waveforms.py
--rw-r--r--   0        0        0    15947 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/utilities.py
--rw-r--r--   0        0        0    45200 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/waveform_base.py
--rw-r--r--   0        0        0    34641 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/waveform_grid.py
--rw-r--r--   0        0        0    42665 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/waveform_modes.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/LVC/__init__.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/LVC/file_io.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/SpEC/__init__.py
--rwxr-xr-x   0        0        0    24782 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/SpEC/com_motion.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/SpEC/find_com_in_catalog.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/SpEC/remove_avg_com_from_catalog.py
--rw-r--r--   0        0        0    21138 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/SpEC/file_io/__init__.py
--rw-r--r--   0        0        0    10023 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/SpEC/file_io/corotating_paired_xor.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/SpEC/file_io/rotating_paired_xor_multishuffle_bzip2.py
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/SpEC/samples/metadata.txt
--rw-r--r--   0        0        0     7383 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/asymptotic_bondi_data/__init__.py
--rw-r--r--   0        0        0    10717 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/asymptotic_bondi_data/bms_charges.py
--rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/asymptotic_bondi_data/constraints.py
--rw-r--r--   0        0        0     7998 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/asymptotic_bondi_data/from_initial_values.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/asymptotic_bondi_data/map_to_abd_frame.py
--rw-r--r--   0        0        0    36962 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/asymptotic_bondi_data/map_to_superrest_frame.py
--rw-r--r--   0        0        0    22018 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/asymptotic_bondi_data/transformations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scri-2022.8.8/scri/pn/__init__.py
--rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 scri-2022.8.8/tests/conftest.py
--rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 scri-2022.8.8/tests/test_SpEC.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 scri-2022.8.8/tests/test_abd_frame.py
--rw-r--r--   0        0        0     9661 2020-02-02 00:00:00.000000 scri-2022.8.8/tests/test_abd_ivp.py
--rw-r--r--   0        0        0     8944 2020-02-02 00:00:00.000000 scri-2022.8.8/tests/test_asymptoticbondidata.py
--rw-r--r--   0        0        0    16494 2020-02-02 00:00:00.000000 scri-2022.8.8/tests/test_bms_transformations.py
--rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 scri-2022.8.8/tests/test_flux.py
--rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 scri-2022.8.8/tests/test_mode_calculations.py
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 scri-2022.8.8/tests/test_parity.py
--rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 scri-2022.8.8/tests/test_rotations.py
--rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 scri-2022.8.8/tests/test_superrest_frame.py
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 scri-2022.8.8/tests/test_utilities.py
--rw-r--r--   0        0        0    14746 2020-02-02 00:00:00.000000 scri-2022.8.8/tests/test_waveform.py
--rw-r--r--   0        0        0    11474 2020-02-02 00:00:00.000000 scri-2022.8.8/tests/test_waveform_grid.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 scri-2022.8.8/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 scri-2022.8.8/LICENSE
--rw-r--r--   0        0        0     7965 2020-02-02 00:00:00.000000 scri-2022.8.8/README.md
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 scri-2022.8.8/pyproject.toml
--rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 scri-2022.8.8/PKG-INFO
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 scri-2022.8.9/.readthedocs.yaml
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 scri-2022.8.9/CITATION.cff
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 scri-2022.8.9/scri.bib
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 scri-2022.8.9/.github/scripts/parse_bump_rule.py
+-rw-r--r--   0        0        0     5314 2020-02-02 00:00:00.000000 scri-2022.8.9/.github/workflows/build.yml
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 scri-2022.8.9/docs/.gitignore
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scri-2022.8.9/docs/Makefile
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 scri-2022.8.9/docs/README.md -> ../README.md
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 scri-2022.8.9/docs/api.rst
+-rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 scri-2022.8.9/docs/conf.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 scri-2022.8.9/docs/environment.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scri-2022.8.9/docs/index.rst
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 scri-2022.8.9/docs/make.bat
+-rw-r--r--   0        0        0    10936 2020-02-02 00:00:00.000000 scri-2022.8.9/docs/tutorial_abd.rst
+-rw-r--r--   0        0        0    11070 2020-02-02 00:00:00.000000 scri-2022.8.9/docs/tutorial_bms.rst
+-rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 scri-2022.8.9/docs/tutorial_extrapolation.rst
+-rw-r--r--   0        0        0     9787 2020-02-02 00:00:00.000000 scri-2022.8.9/docs/tutorial_waveformmodes.rst
+-rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/__version__.py
+-rw-r--r--   0        0        0    25519 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/bms_transformations.py
+-rw-r--r--   0        0        0    58879 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/extrapolation.py
+-rw-r--r--   0        0        0    31544 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/flux.py
+-rw-r--r--   0        0        0    21132 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/mode_calculations.py
+-rw-r--r--   0        0        0     7928 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/modes_time_series.py
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/plotting.py
+-rw-r--r--   0        0        0    16811 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/rotations.py
+-rw-r--r--   0        0        0    31597 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/sample_waveforms.py
+-rw-r--r--   0        0        0    15947 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/utilities.py
+-rw-r--r--   0        0        0    45200 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/waveform_base.py
+-rw-r--r--   0        0        0    34641 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/waveform_grid.py
+-rw-r--r--   0        0        0    42665 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/waveform_modes.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/LVC/__init__.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/LVC/file_io.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/SpEC/__init__.py
+-rwxr-xr-x   0        0        0    24782 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/SpEC/com_motion.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/SpEC/find_com_in_catalog.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/SpEC/remove_avg_com_from_catalog.py
+-rw-r--r--   0        0        0    21138 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/SpEC/file_io/__init__.py
+-rw-r--r--   0        0        0    10023 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/SpEC/file_io/corotating_paired_xor.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/SpEC/file_io/rotating_paired_xor_multishuffle_bzip2.py
+-rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/SpEC/samples/metadata.txt
+-rw-r--r--   0        0        0     7383 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/asymptotic_bondi_data/__init__.py
+-rw-r--r--   0        0        0    10717 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/asymptotic_bondi_data/bms_charges.py
+-rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/asymptotic_bondi_data/constraints.py
+-rw-r--r--   0        0        0     7998 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/asymptotic_bondi_data/from_initial_values.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/asymptotic_bondi_data/map_to_abd_frame.py
+-rw-r--r--   0        0        0    36962 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/asymptotic_bondi_data/map_to_superrest_frame.py
+-rw-r--r--   0        0        0    22018 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/asymptotic_bondi_data/transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scri-2022.8.9/scri/pn/__init__.py
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 scri-2022.8.9/tests/conftest.py
+-rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 scri-2022.8.9/tests/test_SpEC.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 scri-2022.8.9/tests/test_abd_frame.py
+-rw-r--r--   0        0        0     9661 2020-02-02 00:00:00.000000 scri-2022.8.9/tests/test_abd_ivp.py
+-rw-r--r--   0        0        0     8944 2020-02-02 00:00:00.000000 scri-2022.8.9/tests/test_asymptoticbondidata.py
+-rw-r--r--   0        0        0    16494 2020-02-02 00:00:00.000000 scri-2022.8.9/tests/test_bms_transformations.py
+-rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 scri-2022.8.9/tests/test_flux.py
+-rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 scri-2022.8.9/tests/test_mode_calculations.py
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 scri-2022.8.9/tests/test_parity.py
+-rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 scri-2022.8.9/tests/test_rotations.py
+-rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 scri-2022.8.9/tests/test_superrest_frame.py
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 scri-2022.8.9/tests/test_utilities.py
+-rw-r--r--   0        0        0    14746 2020-02-02 00:00:00.000000 scri-2022.8.9/tests/test_waveform.py
+-rw-r--r--   0        0        0    11474 2020-02-02 00:00:00.000000 scri-2022.8.9/tests/test_waveform_grid.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 scri-2022.8.9/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 scri-2022.8.9/LICENSE
+-rw-r--r--   0        0        0     7965 2020-02-02 00:00:00.000000 scri-2022.8.9/README.md
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 scri-2022.8.9/pyproject.toml
+-rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 scri-2022.8.9/PKG-INFO
```

### Comparing `scri-2022.8.8/CITATION.cff` & `scri-2022.8.9/CITATION.cff`

 * *Files 9% similar despite different names*

```diff
@@ -22,11 +22,11 @@
 - family-names: "Varma"
   given-names: "Vijay"
   orcid: "https://orcid.org/0000-0002-9994-1761"
 - family-names: "Mitman"
   given-names: "Keefe"
   orcid: "https://orcid.org/0000-0003-0276-3856"
 title: "scri"
-version: 2022.8.8
+version: 2022.8.9
 doi: 10.5281/zenodo.4041971
-date-released: 2023-11-08
+date-released: 2024-02-21
 url: "https://github.com/moble/scri"
```

### Comparing `scri-2022.8.8/scri.bib` & `scri-2022.8.9/scri.bib`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/.github/workflows/build.yml` & `scri-2022.8.9/.github/workflows/build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
       matrix:
         os: [ubuntu-latest, macos-latest]
         python-version: ['3.8', '3.11']
 
     steps:
       - name: Skip replicates on main branch
         env:
-          skip_replicates: ${{ github.ref == 'refs/heads/main' && (matrix.os != 'ubuntu-latest' || matrix.python-version != '3.11') }}
+          skip_replicates: ${{ github.ref == 'refs/heads/main' && github.repository_owner == 'moble' && (matrix.os != 'ubuntu-latest' || matrix.python-version != '3.11') }}
         shell: bash
         run: |
           echo "skipping_build_and_test_replicate=${skip_replicates}" >> $GITHUB_ENV
 
       - name: Check out code
         if: ${{ env.skipping_build_and_test_replicate != 'true' }}
         uses: actions/checkout@v2
@@ -65,14 +65,15 @@
 
   release:
     name: Create release and send to PyPI
     needs: build
     runs-on: ubuntu-latest
     if: >-
         github.ref == 'refs/heads/main'
+        && github.repository_owner == 'moble'
         && !contains(github.event.head_commit.message, '[no release]')
         && (success() || contains(github.event.head_commit.message, '[skip tests]'))
 
     steps:
       - name: Check out code
         uses: actions/checkout@v3
```

### Comparing `scri-2022.8.8/docs/Makefile` & `scri-2022.8.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/docs/conf.py` & `scri-2022.8.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/docs/index.rst` & `scri-2022.8.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/docs/make.bat` & `scri-2022.8.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/docs/tutorial_abd.rst` & `scri-2022.8.9/docs/tutorial_abd.rst`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/docs/tutorial_bms.rst` & `scri-2022.8.9/docs/tutorial_bms.rst`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/docs/tutorial_extrapolation.rst` & `scri-2022.8.9/docs/tutorial_extrapolation.rst`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/docs/tutorial_waveformmodes.rst` & `scri-2022.8.9/docs/tutorial_waveformmodes.rst`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/__init__.py` & `scri-2022.8.9/scri/__init__.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/bms_transformations.py` & `scri-2022.8.9/scri/bms_transformations.py`

 * *Files 2% similar despite different names*

```diff
@@ -587,32 +587,40 @@
             supertranslation=S_composed,
             ell_max=ell_max,
             order=["supertranslation", "frame_rotation", "boost_velocity"],
         )
 
         return bms_composed
 
-    def to_file(self, filename):
+    def to_file(self, filename, file_write_mode="w", group=None):
         dt = h5py.special_dtype(vlen=str)
-        with h5py.File(filename, "w") as hf:
-            hf.create_dataset("supertranslation", data=self.supertranslation)
-            hf.create_dataset("frame_rotation", data=self.frame_rotation.components)
-            hf.create_dataset("boost_velocity", data=self.boost_velocity)
-            hf.create_dataset("order", data=self.order)
-            hf.create_dataset("ell_max", data=self.ell_max)
+        with h5py.File(filename, file_write_mode) as hf:
+            if group is not None:
+                g = hf.create_group(group)
+            else:
+                g = hf
+            g.create_dataset("supertranslation", data=self.supertranslation)
+            g.create_dataset("frame_rotation", data=self.frame_rotation.components)
+            g.create_dataset("boost_velocity", data=self.boost_velocity)
+            g.create_dataset("order", data=self.order)
+            g.create_dataset("ell_max", data=self.ell_max)
 
         return
 
-    def from_file(self, filename):
+    def from_file(self, filename, group=None):
         with h5py.File(filename, "r") as hf:
-            supertranslation = np.array(hf.get("supertranslation"))
-            frame_rotation = np.array(hf.get("frame_rotation"))
-            boost_velocity = np.array(hf.get("boost_velocity"))
-            order = [x.decode("utf-8") for x in np.array(hf.get("order"))]
-            ell_max = int(np.array(hf.get("ell_max")))
+            if group is not None:
+                g = hf[group]
+            else:
+                g = hf
+            supertranslation = np.array(g.get("supertranslation"))
+            frame_rotation = np.array(g.get("frame_rotation"))
+            boost_velocity = np.array(g.get("boost_velocity"))
+            order = [x.decode("utf-8") for x in np.array(g.get("order"))]
+            ell_max = int(np.array(g.get("ell_max")))
 
         BMS = BMSTransformation(
             frame_rotation=frame_rotation,
             boost_velocity=boost_velocity,
             supertranslation=supertranslation,
             order=order,
             ell_max=ell_max,
```

### Comparing `scri-2022.8.8/scri/extrapolation.py` & `scri-2022.8.9/scri/extrapolation.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/flux.py` & `scri-2022.8.9/scri/flux.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/mode_calculations.py` & `scri-2022.8.9/scri/mode_calculations.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/modes_time_series.py` & `scri-2022.8.9/scri/modes_time_series.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/plotting.py` & `scri-2022.8.9/scri/plotting.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/rotations.py` & `scri-2022.8.9/scri/rotations.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/sample_waveforms.py` & `scri-2022.8.9/scri/sample_waveforms.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/utilities.py` & `scri-2022.8.9/scri/utilities.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/waveform_base.py` & `scri-2022.8.9/scri/waveform_base.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/waveform_grid.py` & `scri-2022.8.9/scri/waveform_grid.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/waveform_modes.py` & `scri-2022.8.9/scri/waveform_modes.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/LVC/file_io.py` & `scri-2022.8.9/scri/LVC/file_io.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/SpEC/com_motion.py` & `scri-2022.8.9/scri/SpEC/com_motion.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/SpEC/find_com_in_catalog.py` & `scri-2022.8.9/scri/SpEC/find_com_in_catalog.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/SpEC/remove_avg_com_from_catalog.py` & `scri-2022.8.9/scri/SpEC/remove_avg_com_from_catalog.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/SpEC/file_io/__init__.py` & `scri-2022.8.9/scri/SpEC/file_io/__init__.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/SpEC/file_io/corotating_paired_xor.py` & `scri-2022.8.9/scri/SpEC/file_io/corotating_paired_xor.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/SpEC/file_io/rotating_paired_xor_multishuffle_bzip2.py` & `scri-2022.8.9/scri/SpEC/file_io/rotating_paired_xor_multishuffle_bzip2.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/SpEC/samples/metadata.txt` & `scri-2022.8.9/scri/SpEC/samples/metadata.txt`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/asymptotic_bondi_data/__init__.py` & `scri-2022.8.9/scri/asymptotic_bondi_data/__init__.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/asymptotic_bondi_data/bms_charges.py` & `scri-2022.8.9/scri/asymptotic_bondi_data/bms_charges.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/asymptotic_bondi_data/constraints.py` & `scri-2022.8.9/scri/asymptotic_bondi_data/constraints.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/asymptotic_bondi_data/from_initial_values.py` & `scri-2022.8.9/scri/asymptotic_bondi_data/from_initial_values.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/asymptotic_bondi_data/map_to_abd_frame.py` & `scri-2022.8.9/scri/asymptotic_bondi_data/map_to_abd_frame.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/asymptotic_bondi_data/map_to_superrest_frame.py` & `scri-2022.8.9/scri/asymptotic_bondi_data/map_to_superrest_frame.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/scri/asymptotic_bondi_data/transformations.py` & `scri-2022.8.9/scri/asymptotic_bondi_data/transformations.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/tests/conftest.py` & `scri-2022.8.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/tests/test_SpEC.py` & `scri-2022.8.9/tests/test_SpEC.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/tests/test_abd_frame.py` & `scri-2022.8.9/tests/test_abd_frame.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/tests/test_abd_ivp.py` & `scri-2022.8.9/tests/test_abd_ivp.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/tests/test_asymptoticbondidata.py` & `scri-2022.8.9/tests/test_asymptoticbondidata.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/tests/test_bms_transformations.py` & `scri-2022.8.9/tests/test_bms_transformations.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/tests/test_flux.py` & `scri-2022.8.9/tests/test_flux.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/tests/test_mode_calculations.py` & `scri-2022.8.9/tests/test_mode_calculations.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/tests/test_parity.py` & `scri-2022.8.9/tests/test_parity.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/tests/test_rotations.py` & `scri-2022.8.9/tests/test_rotations.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/tests/test_superrest_frame.py` & `scri-2022.8.9/tests/test_superrest_frame.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/tests/test_utilities.py` & `scri-2022.8.9/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/tests/test_waveform.py` & `scri-2022.8.9/tests/test_waveform.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/tests/test_waveform_grid.py` & `scri-2022.8.9/tests/test_waveform_grid.py`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/.gitignore` & `scri-2022.8.9/.gitignore`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/LICENSE` & `scri-2022.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/README.md` & `scri-2022.8.9/README.md`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/pyproject.toml` & `scri-2022.8.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scri-2022.8.8/PKG-INFO` & `scri-2022.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scri
-Version: 2022.8.8
+Version: 2022.8.9
 Summary: Time-dependent functions of spin-weighted spherical harmonics on future null infinity
 Project-URL: Homepage, https://github.com/moble/scri
 Project-URL: Documentation, https://scri.readthedocs.io/
 Author-email: Michael Boyle <michael.oliver.boyle@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Mike Boyle
```

