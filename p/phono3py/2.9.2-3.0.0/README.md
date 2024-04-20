# Comparing `tmp/phono3py-2.9.2.tar.gz` & `tmp/phono3py-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phono3py-2.9.2.tar", last modified: Fri Feb  2 03:18:22 2024, max compression
+gzip compressed data, was "phono3py-3.0.0.tar", last modified: Fri Apr 19 08:24:44 2024, max compression
```

## Comparing `phono3py-2.9.2.tar` & `phono3py-3.0.0.tar`

### file list

```diff
@@ -1,262 +1,262 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.558063 phono3py-2.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-02-02 03:17:12.000000 phono3py-2.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-02 03:17:12.000000 phono3py-2.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-02-02 03:18:22.558063 phono3py-2.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-02-02 03:17:12.000000 phono3py-2.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-02 03:18:17.000000 phono3py-2.9.2/__nanoversion__.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.526063 phono3py-2.9.2/c/
--rw-r--r--   0 runner    (1001) docker     (127)    68789 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/_phono3py.c
--rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/_phononcalc.c
--rw-r--r--   0 runner    (1001) docker     (127)    15045 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/bzgrid.c
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/bzgrid.h
--rw-r--r--   0 runner    (1001) docker     (127)    12441 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/collision_matrix.c
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/collision_matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    29801 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/dynmat.c
--rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/dynmat.h
--rw-r--r--   0 runner    (1001) docker     (127)    23953 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/fc3.c
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/fc3.h
--rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/grgrid.c
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/grgrid.h
--rw-r--r--   0 runner    (1001) docker     (127)    11533 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/gridsys.c
--rw-r--r--   0 runner    (1001) docker     (127)    13952 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/gridsys.h
--rw-r--r--   0 runner    (1001) docker     (127)    16536 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/imag_self_energy_with_g.c
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/imag_self_energy_with_g.h
--rw-r--r--   0 runner    (1001) docker     (127)    12145 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/interaction.c
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/interaction.h
--rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/isotope.c
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/isotope.h
--rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/lagrid.c
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/lagrid.h
--rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/lapack_wrapper.c
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/lapack_wrapper.h
--rw-r--r--   0 runner    (1001) docker     (127)    14541 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/niggli.c
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/niggli.h
--rw-r--r--   0 runner    (1001) docker     (127)    32247 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/phono3py.c
--rw-r--r--   0 runner    (1001) docker     (127)    14106 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/phono3py.h
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/phonoc_array.h
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/phonoc_const.h
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/phonoc_utils.c
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/phonoc_utils.h
--rw-r--r--   0 runner    (1001) docker     (127)    20519 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/phonon.c
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/phonon.h
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/phononcalc.c
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/phononcalc.h
--rw-r--r--   0 runner    (1001) docker     (127)    11640 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/pp_collision.c
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/pp_collision.h
--rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/real_self_energy.c
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/real_self_energy.h
--rw-r--r--   0 runner    (1001) docker     (127)    15983 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/real_to_reciprocal.c
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/real_to_reciprocal.h
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/reciprocal_to_normal.c
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/reciprocal_to_normal.h
--rw-r--r--   0 runner    (1001) docker     (127)    14689 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/snf3x3.c
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/snf3x3.h
--rw-r--r--   0 runner    (1001) docker     (127)    38926 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/tetrahedron_method.c
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/tetrahedron_method.h
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/triplet.c
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/triplet.h
--rw-r--r--   0 runner    (1001) docker     (127)    18558 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/triplet_grid.c
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/triplet_grid.h
--rw-r--r--   0 runner    (1001) docker     (127)    13634 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/triplet_iw.c
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-02-02 03:17:12.000000 phono3py-2.9.2/c/triplet_iw.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.506063 phono3py-2.9.2/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.530063 phono3py-2.9.2/example/AlN-LDA/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/AlN-LDA/BORN
--rw-r--r--   0 runner    (1001) docker     (127)    86886 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/AlN-LDA/FORCES_FC2
--rw-r--r--   0 runner    (1001) docker     (127)   862253 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/AlN-LDA/FORCES_FC3.lzma
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/AlN-LDA/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/AlN-LDA/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   143873 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/AlN-LDA/phono3py_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   176702 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/AlN-LDA/phono3py_disp_dimfc2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.530063 phono3py-2.9.2/example/NaCl-alm/
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/NaCl-alm/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   303332 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/NaCl-alm/phono3py_params_NaCl222.yaml.xz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.530063 phono3py-2.9.2/example/Si-CRYSTAL/
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-CRYSTAL/FORCES_FC2
--rw-r--r--   0 runner    (1001) docker     (127)    52417 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-CRYSTAL/FORCES_FC3
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-CRYSTAL/README
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-CRYSTAL/TEMPLATE
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-CRYSTAL/TEMPLATE3
--rw-r--r--   0 runner    (1001) docker     (127)    50060 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-CRYSTAL/crystal.o
--rw-r--r--   0 runner    (1001) docker     (127)   801243 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-CRYSTAL/outputs.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.534063 phono3py-2.9.2/example/Si-LDA/
--rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-LDA/FORCES_FC3
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-LDA/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-LDA/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    32796 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-LDA/phono3py_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   305364 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-LDA/vasprun_xmls.tar.lzma
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.534063 phono3py-2.9.2/example/Si-PBE/
--rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-PBE/FORCES_FC3
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-PBE/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-PBE/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    32796 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-PBE/phono3py_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   314724 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-PBE/vasprun_xmls.tar.lzma
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.538063 phono3py-2.9.2/example/Si-PBEsol/
--rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-PBEsol/FORCES_FC3
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-PBEsol/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-PBEsol/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    46793 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-PBEsol/Si-band-DOS.png
--rw-r--r--   0 runner    (1001) docker     (127)    28346 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-PBEsol/Si-kaccum.png
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-PBEsol/Si.py
--rw-r--r--   0 runner    (1001) docker     (127)    32796 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-PBEsol/phono3py_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    95766 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-PBEsol/phono3py_disp_dimfc2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.502063 phono3py-2.9.2/example/Si-PBEsol/vasprun_xml_fc2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.538063 phono3py-2.9.2/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/INCAR
--rw-r--r--   0 runner    (1001) docker     (127)    31479 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)   291058 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/vasprun.xml
--rw-r--r--   0 runner    (1001) docker     (127)   300636 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-PBEsol/vasprun_xmls.tar.lzma
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.542063 phono3py-2.9.2/example/Si-QE/
--rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-QE/FORCES_FC3
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-QE/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-QE/Si.in
--rw-r--r--   0 runner    (1001) docker     (127)    32833 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-QE/phono3py_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   150928 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-QE/supercell_out.tar.lzma
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.542063 phono3py-2.9.2/example/Si-TURBOMOLE/
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-TURBOMOLE/FORCES_FC2
--rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-TURBOMOLE/FORCES_FC3
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-TURBOMOLE/README
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-TURBOMOLE/control
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-TURBOMOLE/coord
--rw-r--r--   0 runner    (1001) docker     (127)   278495 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Si-TURBOMOLE/outputs.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.546063 phono3py-2.9.2/example/Wigner_La2Zr2O7/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Wigner_La2Zr2O7/BORN
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Wigner_La2Zr2O7/POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Wigner_La2Zr2O7/command.sh
--rw-r--r--   0 runner    (1001) docker     (127)  1098761 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Wigner_La2Zr2O7/fc2.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)   339529 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Wigner_La2Zr2O7/kappa-m191919.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)   160648 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/Wigner_La2Zr2O7/tc_La2Zr2O7.out.xz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.546063 phono3py-2.9.2/example/zb-ZnTe-PBEsol/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/zb-ZnTe-PBEsol/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/zb-ZnTe-PBEsol/launch_phono3py_ZnTe_PBEsol_222.py
--rw-r--r--   0 runner    (1001) docker     (127)   131412 2024-02-02 03:17:12.000000 phono3py-2.9.2/example/zb-ZnTe-PBEsol/phono3py_params_ZnTe.yaml.xz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.510063 phono3py-2.9.2/phono3py/
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/api_isotope.py
--rw-r--r--   0 runner    (1001) docker     (127)    11563 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/api_jointdos.py
--rw-r--r--   0 runner    (1001) docker     (127)    98310 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/api_phono3py.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.510063 phono3py-2.9.2/phono3py/conductivity/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/conductivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31851 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/conductivity/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    71606 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/conductivity/direct_solution.py
--rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/conductivity/kubo.py
--rw-r--r--   0 runner    (1001) docker     (127)    41437 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/conductivity/rta.py
--rw-r--r--   0 runner    (1001) docker     (127)    44752 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/conductivity/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/conductivity/wigner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.510063 phono3py-2.9.2/phono3py/cui/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/cui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22784 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/cui/create_force_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/cui/create_supercells.py
--rw-r--r--   0 runner    (1001) docker     (127)    17235 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/cui/kaccum_script.py
--rw-r--r--   0 runner    (1001) docker     (127)    26187 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/cui/load.py
--rw-r--r--   0 runner    (1001) docker     (127)    24731 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/cui/phono3py_argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    51943 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/cui/phono3py_script.py
--rw-r--r--   0 runner    (1001) docker     (127)    37210 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/cui/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     9786 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/cui/show_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/cui/triplets_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    60329 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/file_IO.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.514063 phono3py-2.9.2/phono3py/interface/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/interface/alm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/interface/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/interface/fc_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)    22585 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/interface/phono3py_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.514063 phono3py-2.9.2/phono3py/other/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14813 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/other/isotope.py
--rw-r--r--   0 runner    (1001) docker     (127)     7450 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/other/kaccum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/other/tetrahedron_method.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.514063 phono3py-2.9.2/phono3py/phonon/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/phonon/func.py
--rw-r--r--   0 runner    (1001) docker     (127)    42765 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/phonon/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/phonon/group_velocity_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/phonon/heat_capacity_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/phonon/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/phonon/velocity_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.518063 phono3py-2.9.2/phono3py/phonon3/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/phonon3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/phonon3/collision_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/phonon3/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/phonon3/displacement_fc3.py
--rw-r--r--   0 runner    (1001) docker     (127)    30140 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/phonon3/fc3.py
--rw-r--r--   0 runner    (1001) docker     (127)    18127 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/phonon3/gruneisen.py
--rw-r--r--   0 runner    (1001) docker     (127)    38050 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/phonon3/imag_self_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)    38004 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/phonon3/interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    15788 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/phonon3/joint_dos.py
--rw-r--r--   0 runner    (1001) docker     (127)    25948 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/phonon3/real_self_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/phonon3/real_to_reciprocal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/phonon3/reciprocal_to_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)    13786 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/phonon3/spectral_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    14879 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/phonon3/triplets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.518063 phono3py-2.9.2/phono3py/sscha/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/sscha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19518 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/sscha/sscha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-02-02 03:17:12.000000 phono3py-2.9.2/phono3py/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.558063 phono3py-2.9.2/phono3py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-02-02 03:18:22.000000 phono3py-2.9.2/phono3py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-02-02 03:18:22.000000 phono3py-2.9.2/phono3py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 03:18:22.000000 phono3py-2.9.2/phono3py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-02 03:18:22.000000 phono3py-2.9.2/phono3py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-02 03:18:22.000000 phono3py-2.9.2/phono3py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-02-02 03:17:12.000000 phono3py-2.9.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.546063 phono3py-2.9.2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1831 2024-02-02 03:17:12.000000 phono3py-2.9.2/scripts/phono3py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3845 2024-02-02 03:17:12.000000 phono3py-2.9.2/scripts/phono3py-coleigplot
--rwxr-xr-x   0 runner    (1001) docker     (127)     1688 2024-02-02 03:17:12.000000 phono3py-2.9.2/scripts/phono3py-kaccum
--rwxr-xr-x   0 runner    (1001) docker     (127)     9488 2024-02-02 03:17:12.000000 phono3py-2.9.2/scripts/phono3py-kdeplot
--rwxr-xr-x   0 runner    (1001) docker     (127)     1797 2024-02-02 03:17:12.000000 phono3py-2.9.2/scripts/phono3py-load
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-02 03:18:22.558063 phono3py-2.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-02-02 03:17:12.000000 phono3py-2.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.554063 phono3py-2.9.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/AgNO2_cell.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/BORN_NaCl
--rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/FORCES_FC3_si_pbesol
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/FORCE_SETS_NaCl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.554063 phono3py-2.9.2/test/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/api/test_api_phono3py.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.554063 phono3py-2.9.2/test/conductivity/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/conductivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/conductivity/test_kappa_LBTE.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/conductivity/test_kappa_LBTE_Wigner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12437 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/conductivity/test_kappa_RTA.py
--rw-r--r--   0 runner    (1001) docker     (127)    12309 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/conductivity/test_kappa_RTA_Wigner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.554063 phono3py-2.9.2/test/cui/
--rw-r--r--   0 runner    (1001) docker     (127)    62552 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/cui/phono3py_params-qe-Si222.yaml.xz
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/cui/test_phono3py_load_script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.554063 phono3py-2.9.2/test/file_IO/
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/file_IO/test_file_IO.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.554063 phono3py-2.9.2/test/interface/
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/interface/test_phono3py_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.554063 phono3py-2.9.2/test/other/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/other/test_isotope.py
--rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/other/test_kaccum.py
--rw-r--r--   0 runner    (1001) docker     (127)   177468 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/phono3py_params-Si111-rd.yaml.xz
--rw-r--r--   0 runner    (1001) docker     (127)   943848 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/phono3py_params_AlN332.yaml.xz
--rw-r--r--   0 runner    (1001) docker     (127)    26352 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/phono3py_params_NaCl111.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    69120 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/phono3py_params_NaCl222.yaml.xz
--rw-r--r--   0 runner    (1001) docker     (127)    30693 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/phono3py_params_Si-111-222.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    18216 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/phono3py_params_Si111.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    32800 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/phono3py_si_pbesol.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.554063 phono3py-2.9.2/test/phonon/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51828 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/phonon/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    19749 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/phonon/test_velocity_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.558063 phono3py-2.9.2/test/phonon3/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/phonon3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/phonon3/test_displacements.py
--rw-r--r--   0 runner    (1001) docker     (127)    11450 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/phonon3/test_fc3.py
--rw-r--r--   0 runner    (1001) docker     (127)    47987 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/phonon3/test_imag_self_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/phonon3/test_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    11546 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/phonon3/test_joint_dos.py
--rw-r--r--   0 runner    (1001) docker     (127)    19498 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/phonon3/test_real_self_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)    19561 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/phonon3/test_spectral_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    41126 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/phonon3/test_triplets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12203 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/phonopy_disp_NaCl.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   286407 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/phonopy_params-Si111-iterha.yaml.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/phonopy_params_Si.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 03:18:22.558063 phono3py-2.9.2/test/sscha/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/sscha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8801 2024-02-02 03:17:12.000000 phono3py-2.9.2/test/sscha/test_sscha.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.540895 phono3py-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-19 08:23:43.000000 phono3py-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-19 08:23:43.000000 phono3py-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-19 08:24:44.540895 phono3py-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-19 08:23:43.000000 phono3py-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 08:24:39.000000 phono3py-3.0.0/__nanoversion__.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.508894 phono3py-3.0.0/c/
+-rw-r--r--   0 runner    (1001) docker     (127)    68786 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/_phono3py.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/_phononcalc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    15045 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/bzgrid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/bzgrid.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12441 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/collision_matrix.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/collision_matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29801 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/dynmat.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/dynmat.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23953 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/fc3.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/fc3.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/grgrid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/grgrid.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/gridsys.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/gridsys.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16545 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/imag_self_energy_with_g.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/imag_self_energy_with_g.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/interaction.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/interaction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/isotope.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/isotope.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/lagrid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/lagrid.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/lapack_wrapper.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/lapack_wrapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14541 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/niggli.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/niggli.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/phono3py.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/phono3py.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/phonoc_array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/phonoc_const.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/phonoc_utils.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/phonoc_utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20519 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/phonon.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/phonon.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/phononcalc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/phononcalc.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11627 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/pp_collision.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/pp_collision.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/real_self_energy.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/real_self_energy.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16752 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/real_to_reciprocal.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/real_to_reciprocal.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11975 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/reciprocal_to_normal.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/reciprocal_to_normal.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14689 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/snf3x3.c
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/snf3x3.h
+-rw-r--r--   0 runner    (1001) docker     (127)    38926 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/tetrahedron_method.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/tetrahedron_method.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5933 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/triplet.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/triplet.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18558 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/triplet_grid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/triplet_grid.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13656 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/triplet_iw.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-19 08:23:43.000000 phono3py-3.0.0/c/triplet_iw.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.488894 phono3py-3.0.0/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.512894 phono3py-3.0.0/example/AlN-LDA/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/AlN-LDA/BORN
+-rw-r--r--   0 runner    (1001) docker     (127)    86886 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/AlN-LDA/FORCES_FC2
+-rw-r--r--   0 runner    (1001) docker     (127)   862253 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/AlN-LDA/FORCES_FC3.lzma
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/AlN-LDA/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/AlN-LDA/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   143873 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/AlN-LDA/phono3py_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   176702 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/AlN-LDA/phono3py_disp_dimfc2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.512894 phono3py-3.0.0/example/NaCl-alm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/NaCl-alm/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   303332 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/NaCl-alm/phono3py_params_NaCl222.yaml.xz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.512894 phono3py-3.0.0/example/Si-CRYSTAL/
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-CRYSTAL/FORCES_FC2
+-rw-r--r--   0 runner    (1001) docker     (127)    52417 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-CRYSTAL/FORCES_FC3
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-CRYSTAL/README
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-CRYSTAL/TEMPLATE
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-CRYSTAL/TEMPLATE3
+-rw-r--r--   0 runner    (1001) docker     (127)    50060 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-CRYSTAL/crystal.o
+-rw-r--r--   0 runner    (1001) docker     (127)   801243 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-CRYSTAL/outputs.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.516894 phono3py-3.0.0/example/Si-LDA/
+-rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-LDA/FORCES_FC3
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-LDA/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-LDA/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32796 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-LDA/phono3py_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   305364 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-LDA/vasprun_xmls.tar.lzma
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.516894 phono3py-3.0.0/example/Si-PBE/
+-rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBE/FORCES_FC3
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBE/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBE/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32796 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBE/phono3py_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   314724 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBE/vasprun_xmls.tar.lzma
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.520894 phono3py-3.0.0/example/Si-PBEsol/
+-rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBEsol/FORCES_FC3
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBEsol/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBEsol/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    46793 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBEsol/Si-band-DOS.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28346 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBEsol/Si-kaccum.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBEsol/Si.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32796 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBEsol/phono3py_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    95766 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBEsol/phono3py_disp_dimfc2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.488894 phono3py-3.0.0/example/Si-PBEsol/vasprun_xml_fc2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.520894 phono3py-3.0.0/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/INCAR
+-rw-r--r--   0 runner    (1001) docker     (127)    31479 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)   291058 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/vasprun.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   300636 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-PBEsol/vasprun_xmls.tar.lzma
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.520894 phono3py-3.0.0/example/Si-QE/
+-rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-QE/FORCES_FC3
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-QE/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-QE/Si.in
+-rw-r--r--   0 runner    (1001) docker     (127)    32833 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-QE/phono3py_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   150928 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-QE/supercell_out.tar.lzma
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.524894 phono3py-3.0.0/example/Si-TURBOMOLE/
+-rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-TURBOMOLE/FORCES_FC2
+-rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-TURBOMOLE/FORCES_FC3
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-TURBOMOLE/README
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-TURBOMOLE/control
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-TURBOMOLE/coord
+-rw-r--r--   0 runner    (1001) docker     (127)   278495 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Si-TURBOMOLE/outputs.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.528895 phono3py-3.0.0/example/Wigner_La2Zr2O7/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Wigner_La2Zr2O7/BORN
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Wigner_La2Zr2O7/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Wigner_La2Zr2O7/command.sh
+-rw-r--r--   0 runner    (1001) docker     (127)  1098761 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Wigner_La2Zr2O7/fc2.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)   339529 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Wigner_La2Zr2O7/kappa-m191919.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)   160648 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/Wigner_La2Zr2O7/tc_La2Zr2O7.out.xz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.528895 phono3py-3.0.0/example/zb-ZnTe-PBEsol/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/zb-ZnTe-PBEsol/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/zb-ZnTe-PBEsol/launch_phono3py_ZnTe_PBEsol_222.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131412 2024-04-19 08:23:43.000000 phono3py-3.0.0/example/zb-ZnTe-PBEsol/phono3py_params_ZnTe.yaml.xz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.492894 phono3py-3.0.0/phono3py/
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/api_isotope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11563 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/api_jointdos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87780 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/api_phono3py.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.492894 phono3py-3.0.0/phono3py/conductivity/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/conductivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31851 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/conductivity/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71606 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/conductivity/direct_solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/conductivity/kubo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41437 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/conductivity/rta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44752 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/conductivity/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/conductivity/wigner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.496894 phono3py-3.0.0/phono3py/cui/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/cui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20611 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/cui/create_force_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/cui/create_supercells.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14312 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/cui/kaccum_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24757 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/cui/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24731 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/cui/phono3py_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51088 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/cui/phono3py_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37210 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/cui/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9786 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/cui/show_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/cui/triplets_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58029 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/file_IO.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.496894 phono3py-3.0.0/phono3py/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/interface/alm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/interface/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/interface/fc_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22585 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/interface/phono3py_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.496894 phono3py-3.0.0/phono3py/other/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14016 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/other/isotope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/other/kaccum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/other/tetrahedron_method.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.496894 phono3py-3.0.0/phono3py/phonon/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42765 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon/group_velocity_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon/heat_capacity_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon/velocity_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.500894 phono3py-3.0.0/phono3py/phonon3/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/collision_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/displacement_fc3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30148 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/fc3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/gruneisen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38050 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/imag_self_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37969 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15753 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/joint_dos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25948 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/real_self_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/real_to_reciprocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/reciprocal_to_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13786 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/spectral_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14879 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/phonon3/triplets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.500894 phono3py-3.0.0/phono3py/sscha/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/sscha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19518 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/sscha/sscha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-19 08:23:43.000000 phono3py-3.0.0/phono3py/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.540895 phono3py-3.0.0/phono3py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-19 08:24:44.000000 phono3py-3.0.0/phono3py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-04-19 08:24:44.000000 phono3py-3.0.0/phono3py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:24:44.000000 phono3py-3.0.0/phono3py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-19 08:24:44.000000 phono3py-3.0.0/phono3py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 08:24:44.000000 phono3py-3.0.0/phono3py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-19 08:23:43.000000 phono3py-3.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.528895 phono3py-3.0.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1831 2024-04-19 08:23:43.000000 phono3py-3.0.0/scripts/phono3py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3845 2024-04-19 08:23:43.000000 phono3py-3.0.0/scripts/phono3py-coleigplot
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1688 2024-04-19 08:23:43.000000 phono3py-3.0.0/scripts/phono3py-kaccum
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9488 2024-04-19 08:23:43.000000 phono3py-3.0.0/scripts/phono3py-kdeplot
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1797 2024-04-19 08:23:43.000000 phono3py-3.0.0/scripts/phono3py-load
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-19 08:24:44.540895 phono3py-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-04-19 08:23:43.000000 phono3py-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.532895 phono3py-3.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/AgNO2_cell.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/BORN_NaCl
+-rw-r--r--   0 runner    (1001) docker     (127)   357907 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/FORCES_FC3_si_pbesol
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/FORCE_SETS_NaCl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.532895 phono3py-3.0.0/test/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/api/test_api_phono3py.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.536895 phono3py-3.0.0/test/conductivity/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/conductivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/conductivity/test_kappa_LBTE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/conductivity/test_kappa_LBTE_Wigner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12437 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/conductivity/test_kappa_RTA.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12309 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/conductivity/test_kappa_RTA_Wigner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.536895 phono3py-3.0.0/test/cui/
+-rw-r--r--   0 runner    (1001) docker     (127)    62552 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/cui/phono3py_params-qe-Si222.yaml.xz
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/cui/test_phono3py_load_script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.536895 phono3py-3.0.0/test/file_IO/
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/file_IO/test_file_IO.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.536895 phono3py-3.0.0/test/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/interface/test_phono3py_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.536895 phono3py-3.0.0/test/other/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/other/test_isotope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/other/test_kaccum.py
+-rw-r--r--   0 runner    (1001) docker     (127)   177468 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phono3py_params-Si111-rd.yaml.xz
+-rw-r--r--   0 runner    (1001) docker     (127)   943848 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phono3py_params_AlN332.yaml.xz
+-rw-r--r--   0 runner    (1001) docker     (127)    26352 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phono3py_params_NaCl111.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    69120 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phono3py_params_NaCl222.yaml.xz
+-rw-r--r--   0 runner    (1001) docker     (127)    30693 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phono3py_params_Si-111-222.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    18216 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phono3py_params_Si111.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    32800 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phono3py_si_pbesol.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.536895 phono3py-3.0.0/test/phonon/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51828 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonon/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19747 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonon/test_velocity_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.540895 phono3py-3.0.0/test/phonon3/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonon3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonon3/test_displacements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11450 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonon3/test_fc3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47987 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonon3/test_imag_self_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonon3/test_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11546 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonon3/test_joint_dos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19498 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonon3/test_real_self_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19561 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonon3/test_spectral_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41126 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonon3/test_triplets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12203 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonopy_disp_NaCl.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   286407 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonopy_params-Si111-iterha.yaml.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/phonopy_params_Si.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:24:44.540895 phono3py-3.0.0/test/sscha/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/sscha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8801 2024-04-19 08:23:43.000000 phono3py-3.0.0/test/sscha/test_sscha.py
```

### Comparing `phono3py-2.9.2/LICENSE` & `phono3py-3.0.0/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-Copyright (c) 2014, Atsushi Togo
-All rights reserved.
+Copyright (c) 2015-2024, Phonopy. All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
 * Redistributions of source code must retain the above copyright
   notice, this list of conditions and the following disclaimer.
```

### Comparing `phono3py-2.9.2/README.md` & `phono3py-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/_phono3py.c` & `phono3py-3.0.0/c/_phono3py.c`

 * *Files 0% similar despite different names*

```diff
@@ -1415,15 +1415,15 @@
     frequencies2 = (double *)PyArray_DATA(py_frequencies2);
     num_band1 = (long)PyArray_DIMS(py_frequencies1)[1];
     num_band2 = (long)PyArray_DIMS(py_frequencies2)[1];
 
     ph3py_get_integration_weight(
         iw, iw_zero, frequency_points, num_band0, relative_grid_address, D_diag,
         triplets, num_triplets, bz_grid_addresses, bz_map, bz_grid_type,
-        frequencies1, num_band1, frequencies2, num_band2, tp_type, 1, 0);
+        frequencies1, num_band1, frequencies2, num_band2, tp_type, 1);
 
     Py_RETURN_NONE;
 }
 
 static PyObject *py_get_triplets_integration_weights_with_sigma(
     PyObject *self, PyObject *args) {
     PyArrayObject *py_iw;
```

### Comparing `phono3py-2.9.2/c/_phononcalc.c` & `phono3py-3.0.0/c/_phononcalc.c`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/bzgrid.c` & `phono3py-3.0.0/c/bzgrid.c`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/bzgrid.h` & `phono3py-3.0.0/c/bzgrid.h`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/collision_matrix.c` & `phono3py-3.0.0/c/collision_matrix.c`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/collision_matrix.h` & `phono3py-3.0.0/c/collision_matrix.h`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/dynmat.c` & `phono3py-3.0.0/c/dynmat.c`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/dynmat.h` & `phono3py-3.0.0/c/dynmat.h`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/fc3.c` & `phono3py-3.0.0/c/fc3.c`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/fc3.h` & `phono3py-3.0.0/c/fc3.h`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/grgrid.c` & `phono3py-3.0.0/c/grgrid.c`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/grgrid.h` & `phono3py-3.0.0/c/grgrid.h`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/gridsys.c` & `phono3py-3.0.0/c/gridsys.c`

 * *Files 1% similar despite different names*

```diff
@@ -262,15 +262,15 @@
 long gridsys_get_integration_weight(
     double *iw, char *iw_zero, const double *frequency_points,
     const long num_band0, const long relative_grid_address[24][4][3],
     const long D_diag[3], const long (*triplets)[3], const long num_triplets,
     const long (*bz_grid_addresses)[3], const long *bz_map,
     const long bz_grid_type, const double *frequencies1, const long num_band1,
     const double *frequencies2, const long num_band2, const long tp_type,
-    const long openmp_per_triplets, const long openmp_per_bands) {
+    const long openmp_per_triplets) {
     ConstBZGrid *bzgrid;
     long i;
 
     if ((bzgrid = (ConstBZGrid *)malloc(sizeof(ConstBZGrid))) == NULL) {
         warning_print("Memory could not be allocated.");
         return 0;
     }
@@ -278,18 +278,18 @@
     bzgrid->addresses = bz_grid_addresses;
     bzgrid->gp_map = bz_map;
     bzgrid->type = bz_grid_type;
     for (i = 0; i < 3; i++) {
         bzgrid->D_diag[i] = D_diag[i];
     }
 
-    tpl_get_integration_weight(
-        iw, iw_zero, frequency_points, num_band0, relative_grid_address,
-        triplets, num_triplets, bzgrid, frequencies1, num_band1, frequencies2,
-        num_band2, tp_type, openmp_per_triplets, openmp_per_bands);
+    tpl_get_integration_weight(iw, iw_zero, frequency_points, num_band0,
+                               relative_grid_address, triplets, num_triplets,
+                               bzgrid, frequencies1, num_band1, frequencies2,
+                               num_band2, tp_type, openmp_per_triplets);
     free(bzgrid);
     bzgrid = NULL;
 
     return 1;
 }
 
 void gridsys_get_integration_weight_with_sigma(
```

### Comparing `phono3py-2.9.2/c/gridsys.h` & `phono3py-3.0.0/c/gridsys.h`

 * *Files 1% similar despite different names*

```diff
@@ -306,15 +306,15 @@
 long gridsys_get_integration_weight(
     double *iw, char *iw_zero, const double *frequency_points,
     const long num_band0, const long relative_grid_address[24][4][3],
     const long D_diag[3], const long (*triplets)[3], const long num_triplets,
     const long (*bz_grid_addresses)[3], const long *bz_map,
     const long bz_grid_type, const double *frequencies1, const long num_band1,
     const double *frequencies2, const long num_band2, const long tp_type,
-    const long openmp_per_triplets, const long openmp_per_bands);
+    const long openmp_per_triplets);
 void gridsys_get_integration_weight_with_sigma(
     double *iw, char *iw_zero, const double sigma, const double sigma_cutoff,
     const double *frequency_points, const long num_band0,
     const long (*triplets)[3], const long num_triplets,
     const double *frequencies, const long num_band, const long tp_type);
 
 #ifdef __cplusplus
```

### Comparing `phono3py-2.9.2/c/imag_self_energy_with_g.c` & `phono3py-3.0.0/c/imag_self_energy_with_g.c`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
 
 void ise_imag_self_energy_at_triplet(
     double *imag_self_energy, const long num_band0, const long num_band,
     const double *fc3_normal_squared, const double *frequencies,
     const long triplet[3], const long triplet_weight, const double *g1,
     const double *g2_3, const long (*g_pos)[4], const long num_g_pos,
     const double *temperatures, const long num_temps,
-    const double cutoff_frequency, const long openmp_possible,
+    const double cutoff_frequency, const long openmp_per_triplets,
     const long at_a_frequency_point) {
     long i, j;
     double *n1, *n2, *ise_at_g_pos;
     long g_pos_3;
 
     n1 = (double *)malloc(sizeof(double) * num_temps * num_band);
     n2 = (double *)malloc(sizeof(double) * num_temps * num_band);
@@ -234,15 +234,15 @@
     for (i = 0; i < num_temps; i++) {
         set_occupations(n1 + i * num_band, n2 + i * num_band, num_band,
                         temperatures[i], triplet, frequencies,
                         cutoff_frequency);
     }
 
 #ifdef _OPENMP
-#pragma omp parallel for private(j, g_pos_3) if (openmp_possible)
+#pragma omp parallel for private(j, g_pos_3) if (!openmp_per_triplets)
 #endif
     for (i = 0; i < num_g_pos; i++) {
         if (at_a_frequency_point) {
             /** At a frequency point:
              * g_pos[i][3] is for Phi with the shape of (band0, band, band).
              * g_pos_3 is for g at-freq-point with the shape of (bands, bands).
              */
```

### Comparing `phono3py-2.9.2/c/imag_self_energy_with_g.h` & `phono3py-3.0.0/c/imag_self_energy_with_g.h`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/interaction.c` & `phono3py-3.0.0/c/interaction.c`

 * *Files 4% similar despite different names*

```diff
@@ -54,24 +54,24 @@
                            const lapack_complex_double *eigvecs2,
                            const double *fc3, const long is_compact_fc3,
                            const double q_vecs[3][3], /* q0, q1, q2 */
                            const AtomTriplets *atom_triplets,
                            const double *masses, const long *band_indices,
                            const long num_band, const double cutoff_frequency,
                            const long triplet_index, const long num_triplets,
-                           const long openmp_at_bands);
+                           const long openmp_per_triplets);
 static void real_to_normal_sym_q(
     double *fc3_normal_squared, const long (*g_pos)[4], const long num_g_pos,
     double *const freqs[3], lapack_complex_double *const eigvecs[3],
     const double *fc3, const long is_compact_fc3,
     const double q_vecs[3][3], /* q0, q1, q2 */
     const AtomTriplets *atom_triplets, const double *masses,
     const long *band_indices, const long num_band0, const long num_band,
     const double cutoff_frequency, const long triplet_index,
-    const long num_triplets, const long openmp_at_bands);
+    const long num_triplets, const long openmp_per_triplets);
 
 /* fc3_normal_squared[num_triplets, num_band0, num_band, num_band] */
 void itr_get_interaction(
     Darray *fc3_normal_squared, const char *g_zero, const Darray *frequencies,
     const lapack_complex_double *eigenvectors, const long (*triplets)[3],
     const long num_triplets, const ConstBZGrid *bzgrid, const double *fc3,
     const long is_compact_fc3, const AtomTriplets *atom_triplets,
@@ -97,15 +97,15 @@
                                   g_zero + i * num_band_prod);
 
         itr_get_interaction_at_triplet(
             fc3_normal_squared->data + i * num_band_prod, num_band0, num_band,
             g_pos, num_g_pos, frequencies->data, eigenvectors, triplets[i],
             bzgrid, fc3, is_compact_fc3, atom_triplets, masses, band_indices,
             symmetrize_fc3_q, cutoff_frequency, i, num_triplets,
-            1 - openmp_per_triplets);
+            openmp_per_triplets);
 
         free(g_pos);
         g_pos = NULL;
     }
 }
 
 void itr_get_interaction_at_triplet(
@@ -114,15 +114,15 @@
     const lapack_complex_double *eigenvectors, const long triplet[3],
     const ConstBZGrid *bzgrid, const double *fc3, const long is_compact_fc3,
     const AtomTriplets *atom_triplets, const double *masses,
     const long *band_indices, const long symmetrize_fc3_q,
     const double cutoff_frequency,
     const long triplet_index, /* only for print */
     const long num_triplets,  /* only for print */
-    const long openmp_at_bands) {
+    const long openmp_per_triplets) {
     long j, k;
     double *freqs[3];
     lapack_complex_double *eigvecs[3];
     double q_vecs[3][3];
 
     for (j = 0; j < 3; j++) {
         for (k = 0; k < 3; k++) {
@@ -145,15 +145,15 @@
                     eigenvectors[triplet[j] * num_band * num_band + k];
             }
         }
         real_to_normal_sym_q(
             fc3_normal_squared, g_pos, num_g_pos, freqs, eigvecs, fc3,
             is_compact_fc3, q_vecs, /* q0, q1, q2 */
             atom_triplets, masses, band_indices, num_band0, num_band,
-            cutoff_frequency, triplet_index, num_triplets, openmp_at_bands);
+            cutoff_frequency, triplet_index, num_triplets, openmp_per_triplets);
         for (j = 0; j < 3; j++) {
             free(freqs[j]);
             freqs[j] = NULL;
             free(eigvecs[j]);
             eigvecs[j] = NULL;
         }
     } else {
@@ -163,15 +163,15 @@
                        frequencies + triplet[2] * num_band,
                        eigenvectors + triplet[0] * num_band * num_band,
                        eigenvectors + triplet[1] * num_band * num_band,
                        eigenvectors + triplet[2] * num_band * num_band, fc3,
                        is_compact_fc3, q_vecs, /* q0, q1, q2 */
                        atom_triplets, masses, band_indices, num_band,
                        cutoff_frequency, triplet_index, num_triplets,
-                       openmp_at_bands);
+                       openmp_per_triplets);
     }
 }
 
 static void real_to_normal(double *fc3_normal_squared, const long (*g_pos)[4],
                            const long num_g_pos, const double *freqs0,
                            const double *freqs1, const double *freqs2,
                            const lapack_complex_double *eigvecs0,
@@ -179,52 +179,52 @@
                            const lapack_complex_double *eigvecs2,
                            const double *fc3, const long is_compact_fc3,
                            const double q_vecs[3][3], /* q0, q1, q2 */
                            const AtomTriplets *atom_triplets,
                            const double *masses, const long *band_indices,
                            const long num_band, const double cutoff_frequency,
                            const long triplet_index, const long num_triplets,
-                           const long openmp_at_bands) {
+                           const long openmp_per_triplets) {
     lapack_complex_double *fc3_reciprocal;
     lapack_complex_double comp_zero;
     long i;
 
     comp_zero = lapack_make_complex_double(0, 0);
     fc3_reciprocal = (lapack_complex_double *)malloc(
         sizeof(lapack_complex_double) * num_band * num_band * num_band);
     for (i = 0; i < num_band * num_band * num_band; i++) {
         fc3_reciprocal[i] = comp_zero;
     }
     r2r_real_to_reciprocal(fc3_reciprocal, q_vecs, fc3, is_compact_fc3,
-                           atom_triplets, openmp_at_bands);
+                           atom_triplets, openmp_per_triplets);
 
 #ifdef MEASURE_R2N
-    if (openmp_at_bands && num_triplets > 0) {
+    if ((!openmp_per_triplets) && num_triplets > 0) {
         printf("At triplet %d/%d (# of bands=%d):\n", triplet_index,
                num_triplets, num_band0);
     }
 #endif
     reciprocal_to_normal_squared(
         fc3_normal_squared, g_pos, num_g_pos, fc3_reciprocal, freqs0, freqs1,
         freqs2, eigvecs0, eigvecs1, eigvecs2, masses, band_indices, num_band,
-        cutoff_frequency, openmp_at_bands);
+        cutoff_frequency, openmp_per_triplets);
 
     free(fc3_reciprocal);
     fc3_reciprocal = NULL;
 }
 
 static void real_to_normal_sym_q(
     double *fc3_normal_squared, const long (*g_pos)[4], const long num_g_pos,
     double *const freqs[3], lapack_complex_double *const eigvecs[3],
     const double *fc3, const long is_compact_fc3,
     const double q_vecs[3][3], /* q0, q1, q2 */
     const AtomTriplets *atom_triplets, const double *masses,
     const long *band_indices, const long num_band0, const long num_band,
     const double cutoff_frequency, const long triplet_index,
-    const long num_triplets, const long openmp_at_bands) {
+    const long num_triplets, const long openmp_per_triplets) {
     long i, j, k, l;
     long band_ex[3];
     double q_vecs_ex[3][3];
     double *fc3_normal_squared_ex;
 
     fc3_normal_squared_ex =
         (double *)malloc(sizeof(double) * num_band * num_band * num_band);
@@ -242,15 +242,15 @@
         real_to_normal(
             fc3_normal_squared_ex, g_pos, num_g_pos,
             freqs[index_exchange[i][0]], freqs[index_exchange[i][1]],
             freqs[index_exchange[i][2]], eigvecs[index_exchange[i][0]],
             eigvecs[index_exchange[i][1]], eigvecs[index_exchange[i][2]], fc3,
             is_compact_fc3, q_vecs_ex, /* q0, q1, q2 */
             atom_triplets, masses, band_indices, num_band, cutoff_frequency,
-            triplet_index, num_triplets, openmp_at_bands);
+            triplet_index, num_triplets, openmp_per_triplets);
         for (j = 0; j < num_band0; j++) {
             for (k = 0; k < num_band; k++) {
                 for (l = 0; l < num_band; l++) {
                     band_ex[0] = band_indices[j];
                     band_ex[1] = k;
                     band_ex[2] = l;
                     fc3_normal_squared[j * num_band * num_band + k * num_band +
```

### Comparing `phono3py-2.9.2/c/interaction.h` & `phono3py-3.0.0/c/interaction.h`

 * *Files 1% similar despite different names*

```diff
@@ -53,10 +53,10 @@
     const lapack_complex_double *eigenvectors, const long triplet[3],
     const ConstBZGrid *bzgrid, const double *fc3, const long is_compact_fc3,
     const AtomTriplets *atom_triplets, const double *masses,
     const long *band_indices, const long symmetrize_fc3_q,
     const double cutoff_frequency,
     const long triplet_index, /* only for print */
     const long num_triplets,  /* only for print */
-    const long openmp_at_bands);
+    const long openmp_per_triplets);
 
 #endif
```

### Comparing `phono3py-2.9.2/c/isotope.c` & `phono3py-3.0.0/c/isotope.c`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/isotope.h` & `phono3py-3.0.0/c/isotope.h`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/lagrid.c` & `phono3py-3.0.0/c/lagrid.c`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/lagrid.h` & `phono3py-3.0.0/c/lagrid.h`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/lapack_wrapper.c` & `phono3py-3.0.0/c/lapack_wrapper.c`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/lapack_wrapper.h` & `phono3py-3.0.0/c/lapack_wrapper.h`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/niggli.c` & `phono3py-3.0.0/c/niggli.c`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/niggli.h` & `phono3py-3.0.0/c/niggli.h`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/phono3py.c` & `phono3py-3.0.0/c/phono3py.c`

 * *Files 0% similar despite different names*

```diff
@@ -431,15 +431,15 @@
 long ph3py_get_integration_weight(
     double *iw, char *iw_zero, const double *frequency_points,
     const long num_band0, const long relative_grid_address[24][4][3],
     const long D_diag[3], const long (*triplets)[3], const long num_triplets,
     const long (*bz_grid_addresses)[3], const long *bz_map,
     const long bz_grid_type, const double *frequencies1, const long num_band1,
     const double *frequencies2, const long num_band2, const long tp_type,
-    const long openmp_per_triplets, const long openmp_per_bands) {
+    const long openmp_per_triplets) {
     ConstBZGrid *bzgrid;
     long i;
 
     if ((bzgrid = (ConstBZGrid *)malloc(sizeof(ConstBZGrid))) == NULL) {
         warning_print("Memory could not be allocated.");
         return 0;
     }
@@ -447,18 +447,18 @@
     bzgrid->addresses = bz_grid_addresses;
     bzgrid->gp_map = bz_map;
     bzgrid->type = bz_grid_type;
     for (i = 0; i < 3; i++) {
         bzgrid->D_diag[i] = D_diag[i];
     }
 
-    tpl_get_integration_weight(
-        iw, iw_zero, frequency_points, num_band0, relative_grid_address,
-        triplets, num_triplets, bzgrid, frequencies1, num_band1, frequencies2,
-        num_band2, tp_type, openmp_per_triplets, openmp_per_bands);
+    tpl_get_integration_weight(iw, iw_zero, frequency_points, num_band0,
+                               relative_grid_address, triplets, num_triplets,
+                               bzgrid, frequencies1, num_band1, frequencies2,
+                               num_band2, tp_type, openmp_per_triplets);
     free(bzgrid);
     bzgrid = NULL;
 
     return 1;
 }
 
 void ph3py_get_integration_weight_with_sigma(
```

### Comparing `phono3py-2.9.2/c/phono3py.h` & `phono3py-3.0.0/c/phono3py.h`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
 long ph3py_get_integration_weight(
     double *iw, char *iw_zero, const double *frequency_points,
     const long num_band0, const long relative_grid_address[24][4][3],
     const long mesh[3], const long (*triplets)[3], const long num_triplets,
     const long (*bz_grid_addresses)[3], const long *bz_map,
     const long bz_grid_type, const double *frequencies1, const long num_band1,
     const double *frequencies2, const long num_band2, const long tp_type,
-    const long openmp_per_triplets, const long openmp_per_bands);
+    const long openmp_per_triplets);
 void ph3py_get_integration_weight_with_sigma(
     double *iw, char *iw_zero, const double sigma, const double sigma_cutoff,
     const double *frequency_points, const long num_band0,
     const long (*triplets)[3], const long num_triplets,
     const double *frequencies, const long num_band, const long tp_type);
 long ph3py_get_grid_index_from_address(const long address[3],
                                        const long mesh[3]);
```

### Comparing `phono3py-2.9.2/c/phonoc_array.h` & `phono3py-3.0.0/c/phonoc_array.h`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/phonoc_const.h` & `phono3py-3.0.0/c/phonoc_const.h`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/phonoc_utils.c` & `phono3py-3.0.0/c/phonoc_utils.c`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/phonoc_utils.h` & `phono3py-3.0.0/c/phonoc_utils.h`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/phonon.c` & `phono3py-3.0.0/c/phonon.c`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/phonon.h` & `phono3py-3.0.0/c/phonon.h`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/phononcalc.c` & `phono3py-3.0.0/c/phononcalc.c`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/phononcalc.h` & `phono3py-3.0.0/c/phononcalc.h`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/pp_collision.c` & `phono3py-3.0.0/c/pp_collision.c`

 * *Files 0% similar despite different names*

```diff
@@ -92,28 +92,27 @@
     for (i = 0; i < num_band0; i++) {
         freqs_at_gp[i] =
             frequencies[triplets[0][0] * num_band + band_indices->data[i]];
     }
 
     tpl_set_relative_grid_address(tp_relative_grid_address,
                                   relative_grid_address, 2);
-
 #ifdef _OPENMP
 #pragma omp parallel for schedule(guided) private( \
         g, g_zero) if (openmp_per_triplets)
 #endif
     for (i = 0; i < num_triplets; i++) {
         g = (double *)malloc(sizeof(double) * 2 * num_band_prod);
         g_zero = (char *)malloc(sizeof(char) * num_band_prod);
         tpi_get_integration_weight(g, g_zero, freqs_at_gp, /* used as f0 */
                                    num_band0, tp_relative_grid_address,
                                    triplets[i], 1, bzgrid,
                                    frequencies,           /* used as f1 */
                                    num_band, frequencies, /* used as f2 */
-                                   num_band, 2, 1 - openmp_per_triplets);
+                                   num_band, 2, openmp_per_triplets);
 
         get_collision(ise + i * num_temps * num_band0, num_band0, num_band,
                       num_temps, temperatures->data, g, g_zero, frequencies,
                       eigenvectors, triplets[i], triplet_weights[i], bzgrid,
                       fc3, is_compact_fc3, atom_triplets, masses,
                       band_indices->data, symmetrize_fc3_q, cutoff_frequency,
                       openmp_per_triplets);
@@ -175,15 +174,15 @@
         g, g_zero) if (openmp_per_triplets)
 #endif
     for (i = 0; i < num_triplets; i++) {
         g = (double *)malloc(sizeof(double) * 2 * num_band_prod);
         g_zero = (char *)malloc(sizeof(char) * num_band_prod);
         tpi_get_integration_weight_with_sigma(
             g, g_zero, sigma, cutoff, freqs_at_gp, num_band0, triplets[i],
-            const_adrs_shift, frequencies, num_band, 2, 0);
+            const_adrs_shift, frequencies, num_band, 2, 1);
 
         get_collision(ise + i * num_temps * num_band0, num_band0, num_band,
                       num_temps, temperatures->data, g, g_zero, frequencies,
                       eigenvectors, triplets[i], triplet_weights[i], bzgrid,
                       fc3, is_compact_fc3, atom_triplets, masses,
                       band_indices->data, symmetrize_fc3_q, cutoff_frequency,
                       openmp_per_triplets);
@@ -230,20 +229,20 @@
 
     num_g_pos = ise_set_g_pos(g_pos, num_band0, num_band, g_zero);
 
     itr_get_interaction_at_triplet(
         fc3_normal_squared, num_band0, num_band, g_pos, num_g_pos, frequencies,
         eigenvectors, triplet, bzgrid, fc3, is_compact_fc3, atom_triplets,
         masses, band_indices, symmetrize_fc3_q, cutoff_frequency, 0, 0,
-        1 - openmp_per_triplets);
+        openmp_per_triplets);
 
     ise_imag_self_energy_at_triplet(
         ise, num_band0, num_band, fc3_normal_squared, frequencies, triplet,
         triplet_weight, g, g + num_band_prod, g_pos, num_g_pos, temperatures,
-        num_temps, cutoff_frequency, 1 - openmp_per_triplets, 0);
+        num_temps, cutoff_frequency, openmp_per_triplets, 0);
 
     free(fc3_normal_squared);
     fc3_normal_squared = NULL;
     free(g_pos);
     g_pos = NULL;
 }
```

### Comparing `phono3py-2.9.2/c/pp_collision.h` & `phono3py-3.0.0/c/pp_collision.h`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/real_self_energy.c` & `phono3py-3.0.0/c/real_self_energy.c`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/real_self_energy.h` & `phono3py-3.0.0/c/real_self_energy.h`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/real_to_reciprocal.c` & `phono3py-3.0.0/c/real_to_reciprocal.c`

 * *Files 10% similar despite different names*

```diff
@@ -39,245 +39,283 @@
 #include <stdio.h>
 #include <stdlib.h>
 
 #include "lapack_wrapper.h"
 #include "phonoc_array.h"
 #include "phonoc_const.h"
 
-static void real_to_reciprocal_legacy(lapack_complex_double *fc3_reciprocal,
-                                      const double q_vecs[3][3],
-                                      const double *fc3,
-                                      const long is_compact_fc3,
-                                      const AtomTriplets *atom_triplets,
-                                      const long openmp_at_bands);
-static void real_to_reciprocal_r0_average(lapack_complex_double *fc3_reciprocal,
-                                          const double q_vecs[3][3],
-                                          const double *fc3,
-                                          const long is_compact_fc3,
-                                          const AtomTriplets *atom_triplets,
-                                          const long openmp_at_bands);
-static void real_to_reciprocal_elements(lapack_complex_double *fc3_rec_elem,
-                                        const double q1[3], const double q2[3],
-                                        const double *fc3,
-                                        const long is_compact_fc3,
-                                        const AtomTriplets *atom_triplets,
-                                        const long pi0, const long pi1,
-                                        const long pi2, const long leg_index);
+static void real_to_reciprocal_legacy(
+    lapack_complex_double *fc3_reciprocal,
+    const lapack_complex_double *pre_phase_factors,
+    const lapack_complex_double *phase_factor1,
+    const lapack_complex_double *phase_factor2, const double *fc3,
+    const long is_compact_fc3, const AtomTriplets *atom_triplets,
+    const long openmp_per_triplets);
+static void real_to_reciprocal_r0_average(
+    lapack_complex_double *fc3_reciprocal,
+    const lapack_complex_double *pre_phase_factors,
+    const lapack_complex_double *phase_factor0,
+    const lapack_complex_double *phase_factor1,
+    const lapack_complex_double *phase_factor2, const double *fc3,
+    const long is_compact_fc3, const AtomTriplets *atom_triplets,
+    const long openmp_per_triplets);
+static void real_to_reciprocal_elements(
+    lapack_complex_double *fc3_rec_elem,
+    const lapack_complex_double *phase_factor1,
+    const lapack_complex_double *phase_factor2, const double *fc3,
+    const long is_compact_fc3, const AtomTriplets *atom_triplets,
+    const long pi0, const long pi1, const long pi2, const long leg_index);
 static lapack_complex_double get_phase_factor(const double q[3],
                                               const double (*svecs)[3],
                                               const long multi[2]);
 static lapack_complex_double get_pre_phase_factor(
     const long i_patom, const double q_vecs[3][3],
     const AtomTriplets *atom_triplets);
 static lapack_complex_double sum_lapack_complex_double(lapack_complex_double a,
                                                        lapack_complex_double b);
 
 /* fc3_reciprocal[num_patom, num_patom, num_patom, 3, 3, 3] */
 void r2r_real_to_reciprocal(lapack_complex_double *fc3_reciprocal,
                             const double q_vecs[3][3], const double *fc3,
                             const long is_compact_fc3,
                             const AtomTriplets *atom_triplets,
-                            const long openmp_at_bands) {
-    long i, num_band;
+                            const long openmp_per_triplets) {
+    long i, j, num_band, num_patom, num_satom, adrs_vec;
+    lapack_complex_double *pre_phase_factors, *phase_factor0, *phase_factor1,
+        *phase_factor2;
+
+    num_patom = atom_triplets->multi_dims[1];
+    num_satom = atom_triplets->multi_dims[0];
+
+    pre_phase_factors = (lapack_complex_double *)malloc(
+        sizeof(lapack_complex_double) * num_patom);
+    for (i = 0; i < num_patom; i++) {
+        pre_phase_factors[i] = get_pre_phase_factor(i, q_vecs, atom_triplets);
+    }
+
+    phase_factor0 = (lapack_complex_double *)malloc(
+        sizeof(lapack_complex_double) * num_patom * num_satom);
+    phase_factor1 = (lapack_complex_double *)malloc(
+        sizeof(lapack_complex_double) * num_patom * num_satom);
+    phase_factor2 = (lapack_complex_double *)malloc(
+        sizeof(lapack_complex_double) * num_patom * num_satom);
+    for (i = 0; i < num_patom; i++) {
+        for (j = 0; j < num_satom; j++) {
+            adrs_vec = j * atom_triplets->multi_dims[1] + i;
+            phase_factor0[i * num_satom + j] =
+                get_phase_factor(q_vecs[0], atom_triplets->svecs,
+                                 atom_triplets->multiplicity[adrs_vec]);
+            phase_factor1[i * num_satom + j] =
+                get_phase_factor(q_vecs[1], atom_triplets->svecs,
+                                 atom_triplets->multiplicity[adrs_vec]);
+            phase_factor2[i * num_satom + j] =
+                get_phase_factor(q_vecs[2], atom_triplets->svecs,
+                                 atom_triplets->multiplicity[adrs_vec]);
+        }
+    }
 
     if (atom_triplets->make_r0_average) {
-        real_to_reciprocal_r0_average(fc3_reciprocal, q_vecs, fc3,
-                                      is_compact_fc3, atom_triplets,
-                                      openmp_at_bands);
+        real_to_reciprocal_r0_average(fc3_reciprocal, pre_phase_factors,
+                                      phase_factor0, phase_factor1,
+                                      phase_factor2, fc3, is_compact_fc3,
+                                      atom_triplets, openmp_per_triplets);
         num_band = atom_triplets->multi_dims[1] * 3;
         for (i = 0; i < num_band * num_band * num_band; i++) {
             fc3_reciprocal[i] = lapack_make_complex_double(
                 lapack_complex_double_real(fc3_reciprocal[i]) / 3,
                 lapack_complex_double_imag(fc3_reciprocal[i]) / 3);
         }
     } else {
-        real_to_reciprocal_legacy(fc3_reciprocal, q_vecs, fc3, is_compact_fc3,
-                                  atom_triplets, openmp_at_bands);
+        real_to_reciprocal_legacy(
+            fc3_reciprocal, pre_phase_factors, phase_factor1, phase_factor2,
+            fc3, is_compact_fc3, atom_triplets, openmp_per_triplets);
     }
+
+    free(pre_phase_factors);
+    pre_phase_factors = NULL;
+    free(phase_factor0);
+    phase_factor1 = NULL;
+    free(phase_factor1);
+    phase_factor1 = NULL;
+    free(phase_factor2);
+    phase_factor2 = NULL;
 }
 
-static void real_to_reciprocal_legacy(lapack_complex_double *fc3_reciprocal,
-                                      const double q_vecs[3][3],
-                                      const double *fc3,
-                                      const long is_compact_fc3,
-                                      const AtomTriplets *atom_triplets,
-                                      const long openmp_at_bands) {
+static void real_to_reciprocal_legacy(
+    lapack_complex_double *fc3_reciprocal,
+    const lapack_complex_double *pre_phase_factors,
+    const lapack_complex_double *phase_factor1,
+    const lapack_complex_double *phase_factor2, const double *fc3,
+    const long is_compact_fc3, const AtomTriplets *atom_triplets,
+    const long openmp_per_triplets) {
     long i, j, k, l, m, n, ijk;
-    long num_patom, num_band;
-    lapack_complex_double pre_phase_factor, fc3_rec_elem[27], fc3_rec;
+    long num_patom, num_satom, num_band;
+    lapack_complex_double fc3_rec_elem[27];
 
     num_patom = atom_triplets->multi_dims[1];
+    num_satom = atom_triplets->multi_dims[0];
     num_band = num_patom * 3;
 
 #ifdef _OPENMP
-#pragma omp parallel for private(i, j, k, l, m, n, fc3_rec_elem, fc3_rec, \
-                                     pre_phase_factor) if (openmp_at_bands)
+#pragma omp parallel for private(i, j, k, l, m, n, \
+                                     fc3_rec_elem) if (!openmp_per_triplets)
 #endif
     for (ijk = 0; ijk < num_patom * num_patom * num_patom; ijk++) {
         i = ijk / (num_patom * num_patom);
         j = (ijk - (i * num_patom * num_patom)) / num_patom;
         k = ijk % num_patom;
 
-        pre_phase_factor = get_pre_phase_factor(i, q_vecs, atom_triplets);
-
-        real_to_reciprocal_elements(fc3_rec_elem, q_vecs[1], q_vecs[2], fc3,
+        real_to_reciprocal_elements(fc3_rec_elem, phase_factor1 + i * num_satom,
+                                    phase_factor2 + i * num_satom, fc3,
                                     is_compact_fc3, atom_triplets, i, j, k, 0);
         for (l = 0; l < 3; l++) {
             for (m = 0; m < 3; m++) {
                 for (n = 0; n < 3; n++) {
-                    fc3_rec = phonoc_complex_prod(
-                        fc3_rec_elem[l * 9 + m * 3 + n], pre_phase_factor);
                     fc3_reciprocal[(i * 3 + l) * num_band * num_band +
                                    (j * 3 + m) * num_band + k * 3 + n] =
-                        sum_lapack_complex_double(
-                            fc3_reciprocal[(i * 3 + l) * num_band * num_band +
-                                           (j * 3 + m) * num_band + k * 3 + n],
-                            fc3_rec);
+                        phonoc_complex_prod(fc3_rec_elem[l * 9 + m * 3 + n],
+                                            pre_phase_factors[i]);
                 }
             }
         }
     }
 }
 
 // Summations are performed with respect to three different lattice reference
 // point for the index of real space fc3 when make_r0_average=True. For cubic
 // case, these three are roughly equivalent but small difference comes from the
 // q-points in triplets used for summation implemented in
 // real_to_reciprocal_elements().
 // --sym-fc3q makes them almost equivalent.
-static void real_to_reciprocal_r0_average(lapack_complex_double *fc3_reciprocal,
-                                          const double q_vecs[3][3],
-                                          const double *fc3,
-                                          const long is_compact_fc3,
-                                          const AtomTriplets *atom_triplets,
-                                          const long openmp_at_bands) {
+static void real_to_reciprocal_r0_average(
+    lapack_complex_double *fc3_reciprocal,
+    const lapack_complex_double *pre_phase_factors,
+    const lapack_complex_double *phase_factor0,
+    const lapack_complex_double *phase_factor1,
+    const lapack_complex_double *phase_factor2, const double *fc3,
+    const long is_compact_fc3, const AtomTriplets *atom_triplets,
+    const long openmp_per_triplets) {
     long i, j, k, l, m, n, ijk;
-    long num_patom, num_band;
-    lapack_complex_double pre_phase_factor, fc3_rec_elem[27], fc3_rec;
+    long num_patom, num_satom, num_band;
+    lapack_complex_double fc3_rec_elem[27], fc3_rec;
 
     num_patom = atom_triplets->multi_dims[1];
+    num_satom = atom_triplets->multi_dims[0];
     num_band = num_patom * 3;
 
 #ifdef _OPENMP
-#pragma omp parallel for private(i, j, k, l, m, n, fc3_rec_elem, fc3_rec, \
-                                     pre_phase_factor) if (openmp_at_bands)
+#pragma omp parallel for private(i, j, k, l, m, n, fc3_rec_elem, \
+                                     fc3_rec) if (!openmp_per_triplets)
 #endif
     for (ijk = 0; ijk < num_patom * num_patom * num_patom; ijk++) {
         i = ijk / (num_patom * num_patom);
         j = (ijk - (i * num_patom * num_patom)) / num_patom;
         k = ijk % num_patom;
 
-        pre_phase_factor = get_pre_phase_factor(i, q_vecs, atom_triplets);
-        real_to_reciprocal_elements(fc3_rec_elem, q_vecs[1], q_vecs[2], fc3,
+        real_to_reciprocal_elements(fc3_rec_elem, phase_factor1 + i * num_satom,
+                                    phase_factor2 + i * num_satom, fc3,
                                     is_compact_fc3, atom_triplets, i, j, k, 1);
         for (l = 0; l < 3; l++) {
             for (m = 0; m < 3; m++) {
                 for (n = 0; n < 3; n++) {
                     fc3_rec = phonoc_complex_prod(
-                        fc3_rec_elem[l * 9 + m * 3 + n], pre_phase_factor);
+                        fc3_rec_elem[l * 9 + m * 3 + n], pre_phase_factors[i]);
                     fc3_reciprocal[(i * 3 + l) * num_band * num_band +
                                    (j * 3 + m) * num_band + k * 3 + n] =
                         sum_lapack_complex_double(
                             fc3_reciprocal[(i * 3 + l) * num_band * num_band +
                                            (j * 3 + m) * num_band + k * 3 + n],
                             fc3_rec);
                 }
             }
         }
 
         // fc3_rec is stored in a way swapping jm <-> il.
-        pre_phase_factor = get_pre_phase_factor(j, q_vecs, atom_triplets);
-        real_to_reciprocal_elements(fc3_rec_elem, q_vecs[0], q_vecs[2], fc3,
+        real_to_reciprocal_elements(fc3_rec_elem, phase_factor0 + j * num_satom,
+                                    phase_factor2 + j * num_satom, fc3,
                                     is_compact_fc3, atom_triplets, j, i, k, 2);
         for (l = 0; l < 3; l++) {
             for (m = 0; m < 3; m++) {
                 for (n = 0; n < 3; n++) {
                     fc3_rec = phonoc_complex_prod(
-                        fc3_rec_elem[m * 9 + l * 3 + n], pre_phase_factor);
+                        fc3_rec_elem[m * 9 + l * 3 + n], pre_phase_factors[j]);
                     fc3_reciprocal[(i * 3 + l) * num_band * num_band +
                                    (j * 3 + m) * num_band + k * 3 + n] =
                         sum_lapack_complex_double(
                             fc3_reciprocal[(i * 3 + l) * num_band * num_band +
                                            (j * 3 + m) * num_band + k * 3 + n],
                             fc3_rec);
                 }
             }
         }
 
         // fc3_rec is stored in a way swapping kn <-> il.
-        pre_phase_factor = get_pre_phase_factor(k, q_vecs, atom_triplets);
-        real_to_reciprocal_elements(fc3_rec_elem, q_vecs[1], q_vecs[0], fc3,
+        real_to_reciprocal_elements(fc3_rec_elem, phase_factor1 + k * num_satom,
+                                    phase_factor0 + k * num_satom, fc3,
                                     is_compact_fc3, atom_triplets, k, j, i, 3);
         for (l = 0; l < 3; l++) {
             for (m = 0; m < 3; m++) {
                 for (n = 0; n < 3; n++) {
                     fc3_rec = phonoc_complex_prod(
-                        fc3_rec_elem[n * 9 + m * 3 + l], pre_phase_factor);
+                        fc3_rec_elem[n * 9 + m * 3 + l], pre_phase_factors[k]);
                     fc3_reciprocal[(i * 3 + l) * num_band * num_band +
                                    (j * 3 + m) * num_band + k * 3 + n] =
                         sum_lapack_complex_double(
                             fc3_reciprocal[(i * 3 + l) * num_band * num_band +
                                            (j * 3 + m) * num_band + k * 3 + n],
                             fc3_rec);
                 }
             }
         }
     }
 }
 
-static void real_to_reciprocal_elements(lapack_complex_double *fc3_rec_elem,
-                                        const double q1[3], const double q2[3],
-                                        const double *fc3,
-                                        const long is_compact_fc3,
-                                        const AtomTriplets *atom_triplets,
-                                        const long pi0, const long pi1,
-                                        const long pi2, const long leg_index) {
+static void real_to_reciprocal_elements(
+    lapack_complex_double *fc3_rec_elem,
+    const lapack_complex_double *phase_factor1,
+    const lapack_complex_double *phase_factor2, const double *fc3,
+    const long is_compact_fc3, const AtomTriplets *atom_triplets,
+    const long pi0, const long pi1, const long pi2, const long leg_index) {
     long i, j, k, l;
-    long num_satom, adrs_shift, adrs_vec1, adrs_vec2;
-    lapack_complex_double phase_factor, phase_factor1, phase_factor2;
+    long num_satom, adrs_shift;
+    lapack_complex_double phase_factor;
     double fc3_rec_real[27], fc3_rec_imag[27];
 
+    num_satom = atom_triplets->multi_dims[0];
+
     for (i = 0; i < 27; i++) {
         fc3_rec_real[i] = 0;
         fc3_rec_imag[i] = 0;
     }
 
-    num_satom = atom_triplets->multi_dims[0];
-
     if (is_compact_fc3) {
         i = pi0;
     } else {
         i = atom_triplets->p2s_map[pi0];
     }
 
     for (j = 0; j < num_satom; j++) {
         if (atom_triplets->s2p_map[j] != atom_triplets->p2s_map[pi1]) {
             continue;
         }
 
-        adrs_vec1 = j * atom_triplets->multi_dims[1] + pi0;
-        phase_factor1 = get_phase_factor(
-            q1, atom_triplets->svecs, atom_triplets->multiplicity[adrs_vec1]);
         for (k = 0; k < num_satom; k++) {
             if (atom_triplets->s2p_map[k] != atom_triplets->p2s_map[pi2]) {
                 continue;
             }
             if (leg_index > 1) {
                 if (atom_triplets->all_shortest[pi0 * num_satom * num_satom +
                                                 j * num_satom + k]) {
                     continue;
                 }
             }
-            adrs_vec2 = k * atom_triplets->multi_dims[1] + pi0;
-            phase_factor2 =
-                get_phase_factor(q2, atom_triplets->svecs,
-                                 atom_triplets->multiplicity[adrs_vec2]);
             adrs_shift =
                 i * 27 * num_satom * num_satom + j * 27 * num_satom + k * 27;
-            phase_factor = phonoc_complex_prod(phase_factor1, phase_factor2);
+            phase_factor =
+                phonoc_complex_prod(phase_factor1[j], phase_factor2[k]);
 
             if ((leg_index == 1) &&
                 (atom_triplets->all_shortest[pi0 * num_satom * num_satom +
                                              j * num_satom + k])) {
                 for (l = 0; l < 27; l++) {
                     fc3_rec_real[l] +=
                         lapack_complex_double_real(phase_factor) *
```

### Comparing `phono3py-2.9.2/c/real_to_reciprocal.h` & `phono3py-3.0.0/c/real_to_reciprocal.h`

 * *Files 1% similar despite different names*

```diff
@@ -48,9 +48,9 @@
     const char *all_shortest;
 } AtomTriplets;
 
 void r2r_real_to_reciprocal(lapack_complex_double *fc3_reciprocal,
                             const double q_vecs[3][3], const double *fc3,
                             const long is_compact_fc3,
                             const AtomTriplets *atom_triplets,
-                            const long openmp_at_bands);
+                            const long openmp_per_triplets);
 #endif
```

### Comparing `phono3py-2.9.2/c/reciprocal_to_normal.h` & `phono3py-3.0.0/c/reciprocal_to_normal.h`

 * *Files 2% similar despite different names*

```diff
@@ -41,10 +41,10 @@
     double *fc3_normal_squared, const long (*g_pos)[4], const long num_g_pos,
     const lapack_complex_double *fc3_reciprocal, const double *freqs0,
     const double *freqs1, const double *freqs2,
     const lapack_complex_double *eigvecs0,
     const lapack_complex_double *eigvecs1,
     const lapack_complex_double *eigvecs2, const double *masses,
     const long *band_indices, const long num_band,
-    const double cutoff_frequency, const long openmp_at_bands);
+    const double cutoff_frequency, const long openmp_per_triplets);
 
 #endif
```

### Comparing `phono3py-2.9.2/c/snf3x3.c` & `phono3py-3.0.0/c/snf3x3.c`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/tetrahedron_method.c` & `phono3py-3.0.0/c/tetrahedron_method.c`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/tetrahedron_method.h` & `phono3py-3.0.0/c/tetrahedron_method.h`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/triplet.c` & `phono3py-3.0.0/c/triplet.c`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 void tpl_get_integration_weight(
     double *iw, char *iw_zero, const double *frequency_points,
     const long num_band0, const long relative_grid_address[24][4][3],
     const long (*triplets)[3], const long num_triplets,
     const ConstBZGrid *bzgrid, const double *frequencies1, const long num_band1,
     const double *frequencies2, const long num_band2, const long tp_type,
-    const long openmp_per_triplets, const long openmp_per_bands) {
+    const long openmp_per_triplets) {
     long i, num_band_prod;
     long tp_relative_grid_address[2][24][4][3];
 
     tpl_set_relative_grid_address(tp_relative_grid_address,
                                   relative_grid_address, tp_type);
     num_band_prod = num_band0 * num_band1 * num_band2;
 
@@ -78,15 +78,15 @@
     for (i = 0; i < num_triplets; i++) {
         tpi_get_integration_weight(
             iw + i * num_band_prod, iw_zero + i * num_band_prod,
             frequency_points, /* f0 */
             num_band0, tp_relative_grid_address, triplets[i], num_triplets,
             bzgrid, frequencies1,    /* f1 */
             num_band1, frequencies2, /* f2 */
-            num_band2, tp_type, openmp_per_bands);
+            num_band2, tp_type, openmp_per_triplets);
     }
 }
 
 void tpl_get_integration_weight_with_sigma(
     double *iw, char *iw_zero, const double sigma, const double sigma_cutoff,
     const double *frequency_points, const long num_band0,
     const long (*triplets)[3], const long num_triplets,
```

### Comparing `phono3py-2.9.2/c/triplet.h` & `phono3py-3.0.0/c/triplet.h`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
                               const long *map_triplets);
 void tpl_get_integration_weight(
     double *iw, char *iw_zero, const double *frequency_points,
     const long num_band0, const long relative_grid_address[24][4][3],
     const long (*triplets)[3], const long num_triplets,
     const ConstBZGrid *bzgrid, const double *frequencies1, const long num_band1,
     const double *frequencies2, const long num_band2, const long tp_type,
-    const long openmp_per_triplets, const long openmp_per_bands);
+    const long openmp_per_triplets);
 void tpl_get_integration_weight_with_sigma(
     double *iw, char *iw_zero, const double sigma, const double sigma_cutoff,
     const double *frequency_points, const long num_band0,
     const long (*triplets)[3], const long num_triplets,
     const double *frequencies, const long num_band, const long tp_type);
 
 long tpl_is_N(const long triplet[3], const long (*bz_grid_addresses)[3]);
```

### Comparing `phono3py-2.9.2/c/triplet_grid.c` & `phono3py-3.0.0/c/triplet_grid.c`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/triplet_grid.h` & `phono3py-3.0.0/c/triplet_grid.h`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/c/triplet_iw.c` & `phono3py-3.0.0/c/triplet_iw.c`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 void tpi_get_integration_weight(
     double *iw, char *iw_zero, const double *frequency_points,
     const long num_band0, const long tp_relative_grid_address[2][24][4][3],
     const long triplets[3], const long num_triplets, const ConstBZGrid *bzgrid,
     const double *frequencies1, const long num_band1,
     const double *frequencies2, const long num_band2, const long tp_type,
-    const long openmp_per_bands) {
+    const long openmp_per_triplets) {
     long max_i, j, b1, b2, b12, num_band_prod, adrs_shift;
     long vertices[2][24][4];
     double g[3];
     double freq_vertices[3][24][4];
 
     get_triplet_tetrahedra_vertices(vertices, tp_relative_grid_address,
                                     triplets, bzgrid);
@@ -94,15 +94,15 @@
     }
     if (tp_type == 4) {
         max_i = 1;
     }
 
 #ifdef _OPENMP
 #pragma omp parallel for private(j, b1, b2, adrs_shift, g, \
-                                 freq_vertices) if (openmp_per_bands)
+                                     freq_vertices) if (!openmp_per_triplets)
 #endif
     for (b12 = 0; b12 < num_band1 * num_band2; b12++) {
         b1 = b12 / num_band2;
         b2 = b12 % num_band2;
         set_freq_vertices(freq_vertices, frequencies1, frequencies2, vertices,
                           num_band1, num_band2, b1, b2, tp_type);
         for (j = 0; j < num_band0; j++) {
@@ -128,21 +128,21 @@
     }
 }
 
 void tpi_get_integration_weight_with_sigma(
     double *iw, char *iw_zero, const double sigma, const double cutoff,
     const double *frequency_points, const long num_band0, const long triplet[3],
     const long const_adrs_shift, const double *frequencies, const long num_band,
-    const long tp_type, const long openmp_per_bands) {
+    const long tp_type, const long openmp_per_triplets) {
     long j, b12, b1, b2, adrs_shift;
     double f0, f1, f2, g0, g1, g2;
 
 #ifdef _OPENMP
 #pragma omp parallel for private(j, b1, b2, f0, f1, f2, g0, g1, g2, \
-                                 adrs_shift) if (openmp_per_bands)
+                                     adrs_shift) if (!openmp_per_triplets)
 #endif
     for (b12 = 0; b12 < num_band * num_band; b12++) {
         b1 = b12 / num_band;
         b2 = b12 % num_band;
         f1 = frequencies[triplet[1] * num_band + b1];
         f2 = frequencies[triplet[2] * num_band + b2];
         for (j = 0; j < num_band0; j++) {
```

### Comparing `phono3py-2.9.2/c/triplet_iw.h` & `phono3py-3.0.0/c/triplet_iw.h`

 * *Files 2% similar despite different names*

```diff
@@ -39,20 +39,20 @@
 
 void tpi_get_integration_weight(
     double *iw, char *iw_zero, const double *frequency_points,
     const long num_band0, const long tp_relative_grid_address[2][24][4][3],
     const long triplets[3], const long num_triplets, const ConstBZGrid *bzgrid,
     const double *frequencies1, const long num_band1,
     const double *frequencies2, const long num_band2, const long tp_type,
-    const long openmp_per_bands);
+    const long openmp_per_triplets);
 void tpi_get_integration_weight_with_sigma(
     double *iw, char *iw_zero, const double sigma, const double cutoff,
     const double *frequency_points, const long num_band0, const long triplet[3],
     const long const_adrs_shift, const double *frequencies, const long num_band,
-    const long tp_type, const long openmp_per_bands);
+    const long tp_type, const long openmp_per_triplets);
 void tpi_get_neighboring_grid_points(long *neighboring_grid_points,
                                      const long grid_point,
                                      const long (*relative_grid_address)[3],
                                      const long num_relative_grid_address,
                                      const ConstBZGrid *bzgrid);
 
 #endif
```

### Comparing `phono3py-2.9.2/example/AlN-LDA/FORCES_FC2` & `phono3py-3.0.0/example/AlN-LDA/FORCES_FC2`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/AlN-LDA/FORCES_FC3.lzma` & `phono3py-3.0.0/example/AlN-LDA/FORCES_FC3.lzma`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/AlN-LDA/README.md` & `phono3py-3.0.0/example/AlN-LDA/README.md`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/AlN-LDA/phono3py_disp.yaml` & `phono3py-3.0.0/example/AlN-LDA/phono3py_disp.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/AlN-LDA/phono3py_disp_dimfc2.yaml` & `phono3py-3.0.0/example/AlN-LDA/phono3py_disp_dimfc2.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/NaCl-alm/README.md` & `phono3py-3.0.0/example/NaCl-alm/README.md`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/NaCl-alm/phono3py_params_NaCl222.yaml.xz` & `phono3py-3.0.0/example/NaCl-alm/phono3py_params_NaCl222.yaml.xz`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-CRYSTAL/FORCES_FC2` & `phono3py-3.0.0/example/Si-CRYSTAL/FORCES_FC2`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-CRYSTAL/FORCES_FC3` & `phono3py-3.0.0/example/Si-CRYSTAL/FORCES_FC3`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-CRYSTAL/README` & `phono3py-3.0.0/example/Si-CRYSTAL/README`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-CRYSTAL/TEMPLATE` & `phono3py-3.0.0/example/Si-CRYSTAL/TEMPLATE`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-CRYSTAL/TEMPLATE3` & `phono3py-3.0.0/example/Si-CRYSTAL/TEMPLATE3`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-CRYSTAL/crystal.o` & `phono3py-3.0.0/example/Si-CRYSTAL/crystal.o`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-CRYSTAL/outputs.tar.gz` & `phono3py-3.0.0/example/Si-CRYSTAL/outputs.tar.gz`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-LDA/FORCES_FC3` & `phono3py-3.0.0/example/Si-LDA/FORCES_FC3`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-LDA/POSCAR-unitcell` & `phono3py-3.0.0/example/Si-LDA/POSCAR-unitcell`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-LDA/README.md` & `phono3py-3.0.0/example/Si-LDA/README.md`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-LDA/phono3py_disp.yaml` & `phono3py-3.0.0/example/Si-LDA/phono3py_disp.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-LDA/vasprun_xmls.tar.lzma` & `phono3py-3.0.0/example/Si-LDA/vasprun_xmls.tar.lzma`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-PBE/FORCES_FC3` & `phono3py-3.0.0/example/Si-PBE/FORCES_FC3`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-PBE/POSCAR-unitcell` & `phono3py-3.0.0/example/Si-PBE/POSCAR-unitcell`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-PBE/README.md` & `phono3py-3.0.0/example/Si-PBE/README.md`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-PBE/phono3py_disp.yaml` & `phono3py-3.0.0/example/Si-PBE/phono3py_disp.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-PBE/vasprun_xmls.tar.lzma` & `phono3py-3.0.0/example/Si-PBE/vasprun_xmls.tar.lzma`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-PBEsol/FORCES_FC3` & `phono3py-3.0.0/example/Si-PBEsol/FORCES_FC3`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-PBEsol/POSCAR-unitcell` & `phono3py-3.0.0/example/Si-PBEsol/POSCAR-unitcell`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-PBEsol/README.md` & `phono3py-3.0.0/example/Si-PBEsol/README.md`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-PBEsol/Si-band-DOS.png` & `phono3py-3.0.0/example/Si-PBEsol/Si-band-DOS.png`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-PBEsol/Si-kaccum.png` & `phono3py-3.0.0/example/Si-PBEsol/Si-kaccum.png`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-PBEsol/Si.py` & `phono3py-3.0.0/example/Si-PBEsol/Si.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-PBEsol/phono3py_disp.yaml` & `phono3py-3.0.0/example/Si-PBEsol/phono3py_disp.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-PBEsol/phono3py_disp_dimfc2.yaml` & `phono3py-3.0.0/example/Si-PBEsol/phono3py_disp_dimfc2.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/POSCAR` & `phono3py-3.0.0/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/POSCAR`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/vasprun.xml` & `phono3py-3.0.0/example/Si-PBEsol/vasprun_xml_fc2/disp-fc2-00001/vasprun.xml`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-PBEsol/vasprun_xmls.tar.lzma` & `phono3py-3.0.0/example/Si-PBEsol/vasprun_xmls.tar.lzma`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-QE/FORCES_FC3` & `phono3py-3.0.0/example/Si-QE/FORCES_FC3`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-QE/README.md` & `phono3py-3.0.0/example/Si-QE/README.md`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-QE/Si.in` & `phono3py-3.0.0/example/Si-QE/Si.in`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-QE/phono3py_disp.yaml` & `phono3py-3.0.0/example/Si-QE/phono3py_disp.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-QE/supercell_out.tar.lzma` & `phono3py-3.0.0/example/Si-QE/supercell_out.tar.lzma`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-TURBOMOLE/FORCES_FC2` & `phono3py-3.0.0/example/Si-TURBOMOLE/FORCES_FC2`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-TURBOMOLE/FORCES_FC3` & `phono3py-3.0.0/example/Si-TURBOMOLE/FORCES_FC3`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-TURBOMOLE/README` & `phono3py-3.0.0/example/Si-TURBOMOLE/README`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Si-TURBOMOLE/outputs.tar.gz` & `phono3py-3.0.0/example/Si-TURBOMOLE/outputs.tar.gz`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Wigner_La2Zr2O7/BORN` & `phono3py-3.0.0/example/Wigner_La2Zr2O7/BORN`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Wigner_La2Zr2O7/POSCAR` & `phono3py-3.0.0/example/Wigner_La2Zr2O7/POSCAR`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Wigner_La2Zr2O7/fc2.hdf5` & `phono3py-3.0.0/example/Wigner_La2Zr2O7/fc2.hdf5`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Wigner_La2Zr2O7/kappa-m191919.hdf5` & `phono3py-3.0.0/example/Wigner_La2Zr2O7/kappa-m191919.hdf5`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/Wigner_La2Zr2O7/tc_La2Zr2O7.out.xz` & `phono3py-3.0.0/example/Wigner_La2Zr2O7/tc_La2Zr2O7.out.xz`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/zb-ZnTe-PBEsol/README.md` & `phono3py-3.0.0/example/zb-ZnTe-PBEsol/README.md`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/zb-ZnTe-PBEsol/launch_phono3py_ZnTe_PBEsol_222.py` & `phono3py-3.0.0/example/zb-ZnTe-PBEsol/launch_phono3py_ZnTe_PBEsol_222.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/example/zb-ZnTe-PBEsol/phono3py_params_ZnTe.yaml.xz` & `phono3py-3.0.0/example/zb-ZnTe-PBEsol/phono3py_params_ZnTe.yaml.xz`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/__init__.py` & `phono3py-3.0.0/phono3py/__init__.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/api_isotope.py` & `phono3py-3.0.0/phono3py/api_isotope.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/api_jointdos.py` & `phono3py-3.0.0/phono3py/api_jointdos.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/api_phono3py.py` & `phono3py-3.0.0/phono3py/api_phono3py.py`

 * *Files 13% similar despite different names*

```diff
@@ -94,6052 +94,5394 @@
 000005d0: 204f 5220 4f54 4845 5257 4953 4529 2041   OR OTHERWISE) A
 000005e0: 5249 5349 4e47 2049 4e0a 2320 414e 5920  RISING IN.# ANY 
 000005f0: 5741 5920 4f55 5420 4f46 2054 4845 2055  WAY OUT OF THE U
 00000600: 5345 204f 4620 5448 4953 2053 4f46 5457  SE OF THIS SOFTW
 00000610: 4152 452c 2045 5645 4e20 4946 2041 4456  ARE, EVEN IF ADV
 00000620: 4953 4544 204f 4620 5448 450a 2320 504f  ISED OF THE.# PO
 00000630: 5353 4942 494c 4954 5920 4f46 2053 5543  SSIBILITY OF SUC
-00000640: 4820 4441 4d41 4745 2e0a 0a69 6d70 6f72  H DAMAGE...impor
-00000650: 7420 7761 726e 696e 6773 0a66 726f 6d20  t warnings.from 
-00000660: 636f 6c6c 6563 7469 6f6e 732e 6162 6320  collections.abc 
-00000670: 696d 706f 7274 2053 6571 7565 6e63 650a  import Sequence.
-00000680: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
-00000690: 7274 204f 7074 696f 6e61 6c2c 2055 6e69  rt Optional, Uni
-000006a0: 6f6e 0a0a 696d 706f 7274 206e 756d 7079  on..import numpy
-000006b0: 2061 7320 6e70 0a66 726f 6d20 7068 6f6e   as np.from phon
-000006c0: 6f70 792e 6578 6365 7074 696f 6e20 696d  opy.exception im
-000006d0: 706f 7274 2046 6f72 6365 4361 6c63 756c  port ForceCalcul
-000006e0: 6174 6f72 5265 7175 6972 6564 4572 726f  atorRequiredErro
-000006f0: 720a 6672 6f6d 2070 686f 6e6f 7079 2e68  r.from phonopy.h
-00000700: 6172 6d6f 6e69 632e 6469 7370 6c61 6365  armonic.displace
-00000710: 6d65 6e74 2069 6d70 6f72 7420 280a 2020  ment import (.  
-00000720: 2020 6469 7265 6374 696f 6e73 5f74 6f5f    directions_to_
-00000730: 6469 7370 6c61 6365 6d65 6e74 5f64 6174  displacement_dat
-00000740: 6173 6574 2c0a 2020 2020 6765 745f 6c65  aset,.    get_le
-00000750: 6173 745f 6469 7370 6c61 6365 6d65 6e74  ast_displacement
-00000760: 732c 0a29 0a66 726f 6d20 7068 6f6e 6f70  s,.).from phonop
-00000770: 792e 6861 726d 6f6e 6963 2e66 6f72 6365  y.harmonic.force
-00000780: 5f63 6f6e 7374 616e 7473 2069 6d70 6f72  _constants impor
-00000790: 7420 6765 745f 6663 3220 6173 2067 6574  t get_fc2 as get
-000007a0: 5f70 686f 6e6f 7079 5f66 6332 0a66 726f  _phonopy_fc2.fro
-000007b0: 6d20 7068 6f6e 6f70 792e 6861 726d 6f6e  m phonopy.harmon
-000007c0: 6963 2e66 6f72 6365 5f63 6f6e 7374 616e  ic.force_constan
-000007d0: 7473 2069 6d70 6f72 7420 280a 2020 2020  ts import (.    
-000007e0: 7365 745f 7065 726d 7574 6174 696f 6e5f  set_permutation_
-000007f0: 7379 6d6d 6574 7279 2c0a 2020 2020 7365  symmetry,.    se
-00000800: 745f 7472 616e 736c 6174 696f 6e61 6c5f  t_translational_
-00000810: 696e 7661 7269 616e 6365 2c0a 2020 2020  invariance,.    
-00000820: 7379 6d6d 6574 7269 7a65 5f63 6f6d 7061  symmetrize_compa
-00000830: 6374 5f66 6f72 6365 5f63 6f6e 7374 616e  ct_force_constan
-00000840: 7473 2c0a 2020 2020 7379 6d6d 6574 7269  ts,.    symmetri
-00000850: 7a65 5f66 6f72 6365 5f63 6f6e 7374 616e  ze_force_constan
-00000860: 7473 2c0a 290a 6672 6f6d 2070 686f 6e6f  ts,.).from phono
-00000870: 7079 2e69 6e74 6572 6661 6365 2e66 635f  py.interface.fc_
-00000880: 6361 6c63 756c 6174 6f72 2069 6d70 6f72  calculator impor
-00000890: 7420 6765 745f 6663 320a 6672 6f6d 2070  t get_fc2.from p
-000008a0: 686f 6e6f 7079 2e73 7472 7563 7475 7265  honopy.structure
-000008b0: 2e61 746f 6d73 2069 6d70 6f72 7420 5068  .atoms import Ph
-000008c0: 6f6e 6f70 7941 746f 6d73 0a66 726f 6d20  onopyAtoms.from 
-000008d0: 7068 6f6e 6f70 792e 7374 7275 6374 7572  phonopy.structur
-000008e0: 652e 6365 6c6c 7320 696d 706f 7274 2028  e.cells import (
-000008f0: 0a20 2020 2050 7269 6d69 7469 7665 2c0a  .    Primitive,.
-00000900: 2020 2020 5375 7065 7263 656c 6c2c 0a20      Supercell,. 
-00000910: 2020 2067 6574 5f70 7269 6d69 7469 7665     get_primitive
-00000920: 2c0a 2020 2020 6765 745f 7072 696d 6974  ,.    get_primit
-00000930: 6976 655f 6d61 7472 6978 2c0a 2020 2020  ive_matrix,.    
-00000940: 6765 745f 7375 7065 7263 656c 6c2c 0a20  get_supercell,. 
-00000950: 2020 2067 7565 7373 5f70 7269 6d69 7469     guess_primiti
-00000960: 7665 5f6d 6174 7269 782c 0a20 2020 2073  ve_matrix,.    s
-00000970: 6861 7065 5f73 7570 6572 6365 6c6c 5f6d  hape_supercell_m
-00000980: 6174 7269 782c 0a29 0a66 726f 6d20 7068  atrix,.).from ph
-00000990: 6f6e 6f70 792e 7374 7275 6374 7572 652e  onopy.structure.
-000009a0: 6461 7461 7365 7420 696d 706f 7274 2067  dataset import g
-000009b0: 6574 5f64 6973 706c 6163 656d 656e 7473  et_displacements
-000009c0: 5f61 6e64 5f66 6f72 6365 730a 6672 6f6d  _and_forces.from
-000009d0: 2070 686f 6e6f 7079 2e73 7472 7563 7475   phonopy.structu
-000009e0: 7265 2e73 796d 6d65 7472 7920 696d 706f  re.symmetry impo
-000009f0: 7274 2053 796d 6d65 7472 790a 6672 6f6d  rt Symmetry.from
-00000a00: 2070 686f 6e6f 7079 2e75 6e69 7473 2069   phonopy.units i
-00000a10: 6d70 6f72 7420 5661 7370 546f 5448 7a0a  mport VaspToTHz.
-00000a20: 0a66 726f 6d20 7068 6f6e 6f33 7079 2e63  .from phono3py.c
-00000a30: 6f6e 6475 6374 6976 6974 792e 6469 7265  onductivity.dire
-00000a40: 6374 5f73 6f6c 7574 696f 6e20 696d 706f  ct_solution impo
-00000a50: 7274 2067 6574 5f74 6865 726d 616c 5f63  rt get_thermal_c
-00000a60: 6f6e 6475 6374 6976 6974 795f 4c42 5445  onductivity_LBTE
-00000a70: 0a66 726f 6d20 7068 6f6e 6f33 7079 2e63  .from phono3py.c
-00000a80: 6f6e 6475 6374 6976 6974 792e 7274 6120  onductivity.rta 
-00000a90: 696d 706f 7274 2067 6574 5f74 6865 726d  import get_therm
-00000aa0: 616c 5f63 6f6e 6475 6374 6976 6974 795f  al_conductivity_
-00000ab0: 5254 410a 6672 6f6d 2070 686f 6e6f 3370  RTA.from phono3p
-00000ac0: 792e 696e 7465 7266 6163 652e 6663 5f63  y.interface.fc_c
-00000ad0: 616c 6375 6c61 746f 7220 696d 706f 7274  alculator import
-00000ae0: 2067 6574 5f66 6333 0a66 726f 6d20 7068   get_fc3.from ph
-00000af0: 6f6e 6f33 7079 2e69 6e74 6572 6661 6365  ono3py.interface
-00000b00: 2e70 686f 6e6f 3370 795f 7961 6d6c 2069  .phono3py_yaml i
-00000b10: 6d70 6f72 7420 5068 6f6e 6f33 7079 5961  mport Phono3pyYa
-00000b20: 6d6c 0a66 726f 6d20 7068 6f6e 6f33 7079  ml.from phono3py
-00000b30: 2e70 686f 6e6f 6e33 2e64 6174 6173 6574  .phonon3.dataset
-00000b40: 2069 6d70 6f72 7420 6765 745f 6469 7370   import get_disp
-00000b50: 6c61 6365 6d65 6e74 735f 616e 645f 666f  lacements_and_fo
-00000b60: 7263 6573 5f66 6333 0a66 726f 6d20 7068  rces_fc3.from ph
-00000b70: 6f6e 6f33 7079 2e70 686f 6e6f 6e33 2e64  ono3py.phonon3.d
-00000b80: 6973 706c 6163 656d 656e 745f 6663 3320  isplacement_fc3 
-00000b90: 696d 706f 7274 2028 0a20 2020 2064 6972  import (.    dir
-00000ba0: 6563 7469 6f6e 5f74 6f5f 6469 7370 6c61  ection_to_displa
-00000bb0: 6365 6d65 6e74 2c0a 2020 2020 6765 745f  cement,.    get_
-00000bc0: 7468 6972 645f 6f72 6465 725f 6469 7370  third_order_disp
-00000bd0: 6c61 6365 6d65 6e74 732c 0a29 0a66 726f  lacements,.).fro
-00000be0: 6d20 7068 6f6e 6f33 7079 2e70 686f 6e6f  m phono3py.phono
-00000bf0: 6e33 2e66 6333 2069 6d70 6f72 7420 6375  n3.fc3 import cu
-00000c00: 746f 6666 5f66 6333 5f62 795f 7a65 726f  toff_fc3_by_zero
-00000c10: 0a66 726f 6d20 7068 6f6e 6f33 7079 2e70  .from phono3py.p
-00000c20: 686f 6e6f 6e33 2e66 6333 2069 6d70 6f72  honon3.fc3 impor
-00000c30: 7420 6765 745f 6663 3320 6173 2067 6574  t get_fc3 as get
-00000c40: 5f70 686f 6e6f 3370 795f 6663 330a 6672  _phono3py_fc3.fr
-00000c50: 6f6d 2070 686f 6e6f 3370 792e 7068 6f6e  om phono3py.phon
-00000c60: 6f6e 332e 6663 3320 696d 706f 7274 2028  on3.fc3 import (
-00000c70: 0a20 2020 2073 6574 5f70 6572 6d75 7461  .    set_permuta
-00000c80: 7469 6f6e 5f73 796d 6d65 7472 795f 636f  tion_symmetry_co
-00000c90: 6d70 6163 745f 6663 332c 0a20 2020 2073  mpact_fc3,.    s
-00000ca0: 6574 5f70 6572 6d75 7461 7469 6f6e 5f73  et_permutation_s
-00000cb0: 796d 6d65 7472 795f 6663 332c 0a20 2020  ymmetry_fc3,.   
-00000cc0: 2073 6574 5f74 7261 6e73 6c61 7469 6f6e   set_translation
-00000cd0: 616c 5f69 6e76 6172 6961 6e63 655f 636f  al_invariance_co
-00000ce0: 6d70 6163 745f 6663 332c 0a20 2020 2073  mpact_fc3,.    s
-00000cf0: 6574 5f74 7261 6e73 6c61 7469 6f6e 616c  et_translational
-00000d00: 5f69 6e76 6172 6961 6e63 655f 6663 332c  _invariance_fc3,
-00000d10: 0a29 0a66 726f 6d20 7068 6f6e 6f33 7079  .).from phono3py
-00000d20: 2e70 686f 6e6f 6e33 2e69 6d61 675f 7365  .phonon3.imag_se
-00000d30: 6c66 5f65 6e65 7267 7920 696d 706f 7274  lf_energy import
-00000d40: 2028 0a20 2020 2067 6574 5f69 6d61 675f   (.    get_imag_
-00000d50: 7365 6c66 5f65 6e65 7267 792c 0a20 2020  self_energy,.   
-00000d60: 2077 7269 7465 5f69 6d61 675f 7365 6c66   write_imag_self
-00000d70: 5f65 6e65 7267 792c 0a29 0a66 726f 6d20  _energy,.).from 
-00000d80: 7068 6f6e 6f33 7079 2e70 686f 6e6f 6e33  phono3py.phonon3
-00000d90: 2e69 6e74 6572 6163 7469 6f6e 2069 6d70  .interaction imp
-00000da0: 6f72 7420 496e 7465 7261 6374 696f 6e0a  ort Interaction.
-00000db0: 6672 6f6d 2070 686f 6e6f 3370 792e 7068  from phono3py.ph
-00000dc0: 6f6e 6f6e 332e 7265 616c 5f73 656c 665f  onon3.real_self_
-00000dd0: 656e 6572 6779 2069 6d70 6f72 7420 280a  energy import (.
-00000de0: 2020 2020 6765 745f 7265 616c 5f73 656c      get_real_sel
-00000df0: 665f 656e 6572 6779 2c0a 2020 2020 7772  f_energy,.    wr
-00000e00: 6974 655f 7265 616c 5f73 656c 665f 656e  ite_real_self_en
-00000e10: 6572 6779 2c0a 290a 6672 6f6d 2070 686f  ergy,.).from pho
-00000e20: 6e6f 3370 792e 7068 6f6e 6f6e 332e 7370  no3py.phonon3.sp
-00000e30: 6563 7472 616c 5f66 756e 6374 696f 6e20  ectral_function 
-00000e40: 696d 706f 7274 2072 756e 5f73 7065 6374  import run_spect
-00000e50: 7261 6c5f 6675 6e63 7469 6f6e 0a66 726f  ral_function.fro
-00000e60: 6d20 7068 6f6e 6f33 7079 2e70 686f 6e6f  m phono3py.phono
-00000e70: 6e2e 6772 6964 2069 6d70 6f72 7420 425a  n.grid import BZ
-00000e80: 4772 6964 0a66 726f 6d20 7068 6f6e 6f33  Grid.from phono3
-00000e90: 7079 2e76 6572 7369 6f6e 2069 6d70 6f72  py.version impor
-00000ea0: 7420 5f5f 7665 7273 696f 6e5f 5f0a 0a0a  t __version__...
-00000eb0: 636c 6173 7320 5068 6f6e 6f33 7079 3a0a  class Phono3py:.
-00000ec0: 2020 2020 2222 2250 686f 6e6f 3370 7920      """Phono3py 
-00000ed0: 6d61 696e 2063 6c61 7373 2e0a 0a20 2020  main class...   
-00000ee0: 2041 7474 7269 6275 7465 730a 2020 2020   Attributes.    
-00000ef0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2076  ----------.    v
-00000f00: 6572 7369 6f6e 0a20 2020 2063 616c 6375  ersion.    calcu
-00000f10: 6c61 746f 720a 2020 2020 6663 3320 3a20  lator.    fc3 : 
-00000f20: 6765 7474 6572 2061 6e64 2073 6574 7465  getter and sette
-00000f30: 720a 2020 2020 6663 3220 3a20 6765 7474  r.    fc2 : gett
-00000f40: 6572 2061 6e64 2073 6574 7465 720a 2020  er and setter.  
-00000f50: 2020 666f 7263 655f 636f 6e73 7461 6e74    force_constant
-00000f60: 730a 2020 2020 7369 676d 6120 3a20 6765  s.    sigma : ge
-00000f70: 7474 6572 2061 6e64 2073 6574 7465 720a  tter and setter.
-00000f80: 2020 2020 7369 676d 615f 6375 746f 6666      sigma_cutoff
-00000f90: 203a 2067 6574 7465 7220 616e 6420 7365   : getter and se
-00000fa0: 7474 6572 0a20 2020 206e 6163 5f70 6172  tter.    nac_par
-00000fb0: 616d 7320 3a20 6765 7474 6572 2061 6e64  ams : getter and
-00000fc0: 2073 6574 7465 720a 2020 2020 6479 6e61   setter.    dyna
-00000fd0: 6d69 6361 6c5f 6d61 7472 6978 0a20 2020  mical_matrix.   
-00000fe0: 2070 7269 6d69 7469 7665 0a20 2020 2075   primitive.    u
-00000ff0: 6e69 7463 656c 6c0a 2020 2020 7375 7065  nitcell.    supe
-00001000: 7263 656c 6c0a 2020 2020 7068 6f6e 6f6e  rcell.    phonon
-00001010: 5f73 7570 6572 6365 6c6c 0a20 2020 2070  _supercell.    p
-00001020: 686f 6e6f 6e5f 7072 696d 6974 6976 650a  honon_primitive.
-00001030: 2020 2020 7379 6d6d 6574 7279 0a20 2020      symmetry.   
-00001040: 2070 7269 6d69 7469 7665 5f73 796d 6d65   primitive_symme
-00001050: 7472 790a 2020 2020 7068 6f6e 6f6e 5f73  try.    phonon_s
-00001060: 7570 6572 6365 6c6c 5f73 796d 6d65 7472  upercell_symmetr
-00001070: 790a 2020 2020 7375 7065 7263 656c 6c5f  y.    supercell_
-00001080: 6d61 7472 6978 0a20 2020 2070 686f 6e6f  matrix.    phono
-00001090: 6e5f 7375 7065 7263 656c 6c5f 6d61 7472  n_supercell_matr
-000010a0: 6978 0a20 2020 2070 7269 6d69 7469 7665  ix.    primitive
-000010b0: 5f6d 6174 7269 780a 2020 2020 756e 6974  _matrix.    unit
-000010c0: 5f63 6f6e 7665 7273 696f 6e5f 6661 6374  _conversion_fact
-000010d0: 6f72 0a20 2020 2064 6174 6173 6574 203a  or.    dataset :
-000010e0: 2067 6574 7465 7220 616e 6420 7365 7474   getter and sett
-000010f0: 6572 0a20 2020 2070 686f 6e6f 6e5f 6461  er.    phonon_da
-00001100: 7461 7365 7420 3a20 6765 7474 6572 2061  taset : getter a
-00001110: 6e64 2073 6574 7465 720a 2020 2020 6261  nd setter.    ba
-00001120: 6e64 5f69 6e64 6963 6573 203a 2067 6574  nd_indices : get
-00001130: 7465 7220 616e 6420 7365 7474 6572 0a20  ter and setter. 
-00001140: 2020 2070 686f 6e6f 6e5f 7375 7065 7263     phonon_superc
-00001150: 656c 6c73 5f77 6974 685f 6469 7370 6c61  ells_with_displa
-00001160: 6365 6d65 6e74 730a 2020 2020 7375 7065  cements.    supe
-00001170: 7263 656c 6c73 5f77 6974 685f 6469 7370  rcells_with_disp
-00001180: 6c61 6365 6d65 6e74 730a 2020 2020 6d65  lacements.    me
-00001190: 7368 5f6e 756d 6265 7273 203a 2067 6574  sh_numbers : get
-000011a0: 7465 7220 616e 6420 7365 7474 6572 0a20  ter and setter. 
-000011b0: 2020 2074 6865 726d 616c 5f63 6f6e 6475     thermal_condu
-000011c0: 6374 6976 6974 790a 2020 2020 6469 7370  ctivity.    disp
-000011d0: 6c61 6365 6d65 6e74 7320 3a20 6765 7474  lacements : gett
-000011e0: 6572 2061 6e64 2073 6574 7465 720a 2020  er and setter.  
-000011f0: 2020 666f 7263 6573 203a 2067 6574 7465    forces : gette
-00001200: 7220 616e 6420 7365 7474 6572 0a20 2020  r and setter.   
-00001210: 2070 686f 6e6f 6e5f 6469 7370 6c61 6365   phonon_displace
-00001220: 6d65 6e74 7320 3a20 6765 7474 6572 2061  ments : getter a
-00001230: 6e64 2073 6574 7465 720a 2020 2020 7068  nd setter.    ph
-00001240: 6f6e 6f6e 5f66 6f72 6365 7320 3a20 6765  onon_forces : ge
-00001250: 7474 6572 2061 6e64 2073 6574 7465 720a  tter and setter.
-00001260: 2020 2020 7068 7068 5f69 6e74 6572 6163      phph_interac
-00001270: 7469 6f6e 0a0a 2020 2020 2222 220a 0a20  tion..    """.. 
-00001280: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00001290: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-000012a0: 2020 2020 2020 2075 6e69 7463 656c 6c3a         unitcell:
-000012b0: 2050 686f 6e6f 7079 4174 6f6d 732c 0a20   PhonopyAtoms,. 
-000012c0: 2020 2020 2020 2073 7570 6572 6365 6c6c         supercell
-000012d0: 5f6d 6174 7269 783d 4e6f 6e65 2c0a 2020  _matrix=None,.  
-000012e0: 2020 2020 2020 7072 696d 6974 6976 655f        primitive_
-000012f0: 6d61 7472 6978 3d4e 6f6e 652c 0a20 2020  matrix=None,.   
-00001300: 2020 2020 2070 686f 6e6f 6e5f 7375 7065       phonon_supe
-00001310: 7263 656c 6c5f 6d61 7472 6978 3d4e 6f6e  rcell_matrix=Non
-00001320: 652c 0a20 2020 2020 2020 206d 6173 7365  e,.        masse
-00001330: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
-00001340: 6261 6e64 5f69 6e64 6963 6573 3d4e 6f6e  band_indices=Non
-00001350: 652c 0a20 2020 2020 2020 2073 6967 6d61  e,.        sigma
-00001360: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
-00001370: 7369 676d 615f 6375 746f 6666 3d4e 6f6e  sigma_cutoff=Non
-00001380: 652c 0a20 2020 2020 2020 2063 7574 6f66  e,.        cutof
-00001390: 665f 6672 6571 7565 6e63 793d 3165 2d34  f_frequency=1e-4
-000013a0: 2c0a 2020 2020 2020 2020 6672 6571 7565  ,.        freque
-000013b0: 6e63 795f 6661 6374 6f72 5f74 6f5f 5448  ncy_factor_to_TH
-000013c0: 7a3d 5661 7370 546f 5448 7a2c 0a20 2020  z=VaspToTHz,.   
-000013d0: 2020 2020 2069 735f 7379 6d6d 6574 7279       is_symmetry
-000013e0: 3d54 7275 652c 0a20 2020 2020 2020 2069  =True,.        i
-000013f0: 735f 6d65 7368 5f73 796d 6d65 7472 793d  s_mesh_symmetry=
-00001400: 5472 7565 2c0a 2020 2020 2020 2020 7573  True,.        us
-00001410: 655f 6772 673d 4661 6c73 652c 0a20 2020  e_grg=False,.   
-00001420: 2020 2020 2053 4e46 5f63 6f6f 7264 696e       SNF_coordin
-00001430: 6174 6573 3d22 7265 6369 7072 6f63 616c  ates="reciprocal
-00001440: 222c 0a20 2020 2020 2020 206d 616b 655f  ",.        make_
-00001450: 7230 5f61 7665 7261 6765 3a20 626f 6f6c  r0_average: bool
-00001460: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
-00001470: 2020 7379 6d70 7265 633d 3165 2d35 2c0a    symprec=1e-5,.
-00001480: 2020 2020 2020 2020 6361 6c63 756c 6174          calculat
-00001490: 6f72 3a20 4f70 7469 6f6e 616c 5b73 7472  or: Optional[str
-000014a0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-000014b0: 2020 6c6f 675f 6c65 7665 6c3d 302c 0a20    log_level=0,. 
-000014c0: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-000014d0: 2249 6e69 7420 6d65 7468 6f64 2e0a 0a20  "Init method... 
-000014e0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-000014f0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00001500: 2d2d 2d2d 0a20 2020 2020 2020 2075 6e69  ----.        uni
-00001510: 7463 656c 6c20 3a20 5068 6f6e 6f70 7941  tcell : PhonopyA
-00001520: 746f 6d73 2c20 6f70 7469 6f6e 616c 0a20  toms, optional. 
-00001530: 2020 2020 2020 2020 2020 2049 6e70 7574             Input
-00001540: 2075 6e69 7420 6365 6c6c 2e0a 2020 2020   unit cell..    
-00001550: 2020 2020 7375 7065 7263 656c 6c5f 6d61      supercell_ma
-00001560: 7472 6978 203a 2061 7272 6179 5f6c 696b  trix : array_lik
-00001570: 652c 206f 7074 696f 6e61 6c0a 2020 2020  e, optional.    
-00001580: 2020 2020 2020 2020 5375 7065 7263 656c          Supercel
-00001590: 6c20 6d61 7472 6978 206d 756c 7469 706c  l matrix multipl
-000015a0: 6965 6420 746f 2069 6e70 7574 2063 656c  ied to input cel
-000015b0: 6c20 6261 7369 7320 7665 6374 6f72 732e  l basis vectors.
-000015c0: 2073 6861 7065 3d28 332c 2029 0a20 2020   shape=(3, ).   
-000015d0: 2020 2020 2020 2020 206f 7220 2833 2c20           or (3, 
-000015e0: 3329 2c20 7768 6572 6520 7468 6520 666f  3), where the fo
-000015f0: 726d 6572 2069 7320 636f 6e73 6964 6572  rmer is consider
-00001600: 6564 2061 2064 6961 676f 6e61 6c20 6d61  ed a diagonal ma
-00001610: 7472 6978 2e20 5468 650a 2020 2020 2020  trix. The.      
-00001620: 2020 2020 2020 656c 656d 656e 7473 2068        elements h
-00001630: 6176 6520 746f 2062 6520 6769 7665 6e20  ave to be given 
-00001640: 6279 2069 6e74 6567 6572 732e 2041 6c74  by integers. Alt
-00001650: 686f 7567 6820 7468 6520 6465 6661 756c  hough the defaul
-00001660: 7420 6973 204e 6f6e 652c 0a20 2020 2020  t is None,.     
-00001670: 2020 2020 2020 2077 6869 6368 2072 6573         which res
-00001680: 756c 7473 2069 6e20 6964 656e 7469 7479  ults in identity
-00001690: 206d 6174 7269 782c 2069 7420 6973 2072   matrix, it is r
-000016a0: 6563 6f6d 6d65 6e64 6564 2074 6f20 6769  ecommended to gi
-000016b0: 7665 0a20 2020 2020 2020 2020 2020 2060  ve.            `
-000016c0: 7375 7065 7263 656c 6c5f 6d61 7472 6978  supercell_matrix
-000016d0: 6020 6578 706c 6963 6974 6c79 2e0a 2020  ` explicitly..  
-000016e0: 2020 2020 2020 7072 696d 6974 6976 655f        primitive_
-000016f0: 6d61 7472 6978 203a 2061 7272 6179 5f6c  matrix : array_l
-00001700: 696b 6520 6f72 2073 7472 2c20 6f70 7469  ike or str, opti
-00001710: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
-00001720: 2050 7269 6d69 7469 7665 206d 6174 7269   Primitive matri
-00001730: 7820 6d75 6c74 6970 6c69 6564 2074 6f20  x multiplied to 
-00001740: 696e 7075 7420 6365 6c6c 2062 6173 6973  input cell basis
-00001750: 2076 6563 746f 7273 2e20 4465 6661 756c   vectors. Defaul
-00001760: 7420 6973 0a20 2020 2020 2020 2020 2020  t is.           
-00001770: 2074 6865 2069 6465 6e74 6974 7920 6d61   the identity ma
-00001780: 7472 6978 2e20 5768 656e 2067 6976 656e  trix. When given
-00001790: 2061 7320 6172 7261 795f 6c69 6b65 2c20   as array_like, 
-000017a0: 7368 6170 653d 2833 2c20 3329 2c0a 2020  shape=(3, 3),.  
-000017b0: 2020 2020 2020 2020 2020 6474 7970 653d            dtype=
-000017c0: 666c 6f61 742e 2057 6865 6e20 2746 272c  float. When 'F',
-000017d0: 2027 4927 2c20 2741 272c 2027 4327 2c20   'I', 'A', 'C', 
-000017e0: 6f72 2027 5227 2069 7320 6769 7665 6e20  or 'R' is given 
-000017f0: 696e 7374 6561 6420 6f66 2061 0a20 2020  instead of a.   
-00001800: 2020 2020 2020 2020 2033 7833 206d 6174           3x3 mat
-00001810: 7269 782c 2074 6865 2070 7269 6d69 7469  rix, the primiti
-00001820: 7665 206d 6174 7269 7820 6465 6669 6e65  ve matrix define
-00001830: 6420 6174 0a20 2020 2020 2020 2020 2020  d at.           
-00001840: 2068 7474 7073 3a2f 2f73 7067 6c69 622e   https://spglib.
-00001850: 6769 7468 7562 2e69 6f2f 7370 676c 6962  github.io/spglib
-00001860: 2f64 6566 696e 6974 696f 6e2e 6874 6d6c  /definition.html
-00001870: 2069 7320 7573 6564 2e20 5768 656e 2027   is used. When '
-00001880: 6175 746f 270a 2020 2020 2020 2020 2020  auto'.          
-00001890: 2020 6973 2067 6976 656e 2c20 7468 6520    is given, the 
-000018a0: 6365 6e74 7269 6e67 2074 7970 6520 2827  centring type ('
-000018b0: 4627 2c20 2749 272c 2027 4127 2c20 2743  F', 'I', 'A', 'C
-000018c0: 272c 2027 5227 2c20 6f72 2070 7269 6d69  ', 'R', or primi
-000018d0: 7469 7665 0a20 2020 2020 2020 2020 2020  tive.           
-000018e0: 2027 5027 2920 6973 2061 7574 6f6d 6174   'P') is automat
-000018f0: 6963 616c 6c79 2063 686f 7365 6e2e 0a20  ically chosen.. 
-00001900: 2020 2020 2020 2070 686f 6e6f 6e5f 7375         phonon_su
-00001910: 7065 7263 656c 6c5f 6d61 7472 6978 203a  percell_matrix :
-00001920: 2061 7272 6179 5f6c 696b 652c 206f 7074   array_like, opt
-00001930: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
-00001940: 2020 5375 7065 7263 656c 6c20 6d61 7472    Supercell matr
-00001950: 6978 2075 7365 6420 666f 7220 6663 322e  ix used for fc2.
-00001960: 2049 6e20 7068 6f6e 6f33 7079 2c20 7375   In phono3py, su
-00001970: 7065 7263 656c 6c20 6d61 7472 6978 2066  percell matrix f
-00001980: 6f72 2066 6333 0a20 2020 2020 2020 2020  or fc3.         
-00001990: 2020 2061 6e64 2066 6332 2063 616e 2062     and fc2 can b
-000019a0: 6520 6469 6666 6572 656e 7420 746f 2073  e different to s
-000019b0: 7570 706f 7274 206c 6f6e 6765 7220 7261  upport longer ra
-000019c0: 6e67 6520 696e 7465 7261 6374 696f 6e20  nge interaction 
-000019d0: 6f66 2066 6332 0a20 2020 2020 2020 2020  of fc2.         
-000019e0: 2020 2074 6861 6e20 7468 6174 206f 6620     than that of 
-000019f0: 6663 332e 2055 6e6c 6573 7320 7365 7474  fc3. Unless sett
-00001a00: 696e 6720 7468 6973 2c20 7375 7065 7263  ing this, superc
-00001a10: 656c 6c5f 6d61 7472 6978 2069 7320 7573  ell_matrix is us
-00001a20: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
-00001a30: 5468 6973 2069 7320 6f6e 6c79 2076 616c  This is only val
-00001a40: 6964 6520 7768 656e 2075 6e69 7463 656c  ide when unitcel
-00001a50: 6c20 6f72 2075 6e69 7463 656c 6c5f 6669  l or unitcell_fi
-00001a60: 6c65 6e61 6d65 2069 7320 6769 7665 6e2e  lename is given.
-00001a70: 0a20 2020 2020 2020 2020 2020 2044 6566  .            Def
-00001a80: 6175 6c74 2069 7320 4e6f 6e65 2e0a 2020  ault is None..  
-00001a90: 2020 2020 2020 6d61 7373 6573 203a 2044        masses : D
-00001aa0: 6570 7265 6361 7465 642e 0a20 2020 2020  eprecated..     
-00001ab0: 2020 2020 2020 2055 7365 2050 686f 6e6f         Use Phono
-00001ac0: 3370 792e 6d61 7373 6573 2061 7474 7269  3py.masses attri
-00001ad0: 6275 7465 2061 6674 6572 2069 6e73 7461  bute after insta
-00001ae0: 6e63 6961 7469 6f6e 2e0a 2020 2020 2020  nciation..      
-00001af0: 2020 6261 6e64 5f69 6e64 6963 6573 203a    band_indices :
-00001b00: 2044 6570 7265 6361 7465 642e 0a20 2020   Deprecated..   
-00001b10: 2020 2020 2020 2020 2055 7365 2050 686f           Use Pho
-00001b20: 6e6f 3370 792e 6261 6e64 5f69 6e64 6963  no3py.band_indic
-00001b30: 6573 2061 7474 7269 6275 7465 2061 6674  es attribute aft
-00001b40: 6572 2069 6e73 7461 6e63 6961 7469 6f6e  er instanciation
-00001b50: 2e0a 2020 2020 2020 2020 7369 676d 6173  ..        sigmas
-00001b60: 203a 2044 6570 7265 6361 7465 642e 0a20   : Deprecated.. 
-00001b70: 2020 2020 2020 2020 2020 2055 7365 2050             Use P
-00001b80: 686f 6e6f 3370 792e 7369 676d 6173 2061  hono3py.sigmas a
-00001b90: 7474 7269 6275 7465 2061 6674 6572 2069  ttribute after i
-00001ba0: 6e73 7461 6e63 6961 7469 6f6e 2e0a 2020  nstanciation..  
-00001bb0: 2020 2020 2020 7369 676d 615f 6375 746f        sigma_cuto
-00001bc0: 6666 203a 2044 6570 7265 6361 7465 642e  ff : Deprecated.
-00001bd0: 0a20 2020 2020 2020 2020 2020 2055 7365  .            Use
-00001be0: 2050 686f 6e6f 3370 792e 7369 676d 615f   Phono3py.sigma_
-00001bf0: 6375 746f 6666 2061 7474 7269 6275 7465  cutoff attribute
-00001c00: 2061 6674 6572 2069 6e73 7461 6e63 6961   after instancia
-00001c10: 7469 6f6e 2e0a 2020 2020 2020 2020 6375  tion..        cu
-00001c20: 746f 6666 5f66 7265 7175 656e 6379 203a  toff_frequency :
-00001c30: 2066 6c6f 6174 2c20 6f70 7469 6f6e 616c   float, optional
-00001c40: 0a20 2020 2020 2020 2020 2020 2050 686f  .            Pho
-00001c50: 6e6f 6e20 6672 6571 7565 6e63 7920 6265  non frequency be
-00001c60: 6c6f 7720 7468 6973 2076 616c 7565 2069  low this value i
-00001c70: 7320 6967 6e6f 7265 6420 7768 656e 2074  s ignored when t
-00001c80: 6865 2063 7574 6f66 6620 6973 0a20 2020  he cutoff is.   
-00001c90: 2020 2020 2020 2020 206e 6565 6465 6420           needed 
-00001ca0: 666f 7220 7468 6520 636f 6d70 7574 6174  for the computat
-00001cb0: 696f 6e2e 2044 6566 6175 6c74 2069 7320  ion. Default is 
-00001cc0: 3165 2d34 2e0a 2020 2020 2020 2020 6672  1e-4..        fr
-00001cd0: 6571 7565 6e63 795f 6661 6374 6f72 5f74  equency_factor_t
-00001ce0: 6f5f 5448 7a20 3a20 666c 6f61 742c 206f  o_THz : float, o
-00001cf0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00001d00: 2020 2020 5068 6f6e 6f6e 2066 7265 7175      Phonon frequ
-00001d10: 656e 6379 2075 6e69 7420 636f 6e76 6572  ency unit conver
-00001d20: 7369 6f6e 2066 6163 746f 722e 2055 6e6c  sion factor. Unl
-00001d30: 6573 7320 7370 6563 6966 6965 642c 2064  ess specified, d
-00001d40: 6566 6175 6c74 0a20 2020 2020 2020 2020  efault.         
-00001d50: 2020 2075 6e69 7420 636f 6e76 6572 7369     unit conversi
-00001d60: 6f6e 2066 6163 746f 7220 666f 7220 6561  on factor for ea
-00001d70: 6368 2063 616c 6375 6c61 746f 7220 6973  ch calculator is
-00001d80: 2075 7365 642e 0a20 2020 2020 2020 2069   used..        i
-00001d90: 735f 7379 6d6d 6574 7279 203a 2062 6f6f  s_symmetry : boo
-00001da0: 6c2c 206f 7074 696f 6e61 6c0a 2020 2020  l, optional.    
-00001db0: 2020 2020 2020 2020 5573 6520 6372 7973          Use crys
-00001dc0: 7461 6c20 7379 6d6d 6574 7279 2069 6e20  tal symmetry in 
-00001dd0: 6d6f 7374 2063 616c 6375 6c61 7469 6f6e  most calculation
-00001de0: 7320 7768 656e 2054 7275 652e 2044 6566  s when True. Def
-00001df0: 6175 6c74 2069 730a 2020 2020 2020 2020  ault is.        
-00001e00: 2020 2020 5472 7565 2e0a 2020 2020 2020      True..      
-00001e10: 2020 6973 5f6d 6573 685f 7379 6d6d 6574    is_mesh_symmet
-00001e20: 7279 203a 2062 6f6f 6c2c 206f 7074 696f  ry : bool, optio
-00001e30: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
-00001e40: 5573 6520 6372 7973 7461 6c20 7379 6d6d  Use crystal symm
-00001e50: 6574 7279 2069 6e20 7265 6369 7072 6f63  etry in reciproc
-00001e60: 616c 2073 7061 6365 2067 7269 6420 6861  al space grid ha
-00001e70: 6e64 6c69 6e67 2077 6865 6e20 5472 7565  ndling when True
-00001e80: 2e0a 2020 2020 2020 2020 2020 2020 4465  ..            De
-00001e90: 6661 756c 7420 6973 2054 7275 652e 0a20  fault is True.. 
-00001ea0: 2020 2020 2020 2075 7365 5f67 7267 203a         use_grg :
-00001eb0: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0a   bool, optional.
-00001ec0: 2020 2020 2020 2020 2020 2020 5573 6520              Use 
-00001ed0: 6765 6e65 7261 6c69 7a65 6420 7265 6775  generalized regu
-00001ee0: 6c61 7220 6772 6964 2077 6865 6e20 5472  lar grid when Tr
-00001ef0: 7565 2e20 4465 6661 756c 7420 6973 2046  ue. Default is F
-00001f00: 616c 7365 2e0a 2020 2020 2020 2020 534e  alse..        SN
-00001f10: 465f 636f 6f72 6469 6e61 7465 7320 3a20  F_coordinates : 
-00001f20: 7374 722c 206f 7074 696f 6e61 6c0a 2020  str, optional.  
-00001f30: 2020 2020 2020 2020 2020 6072 6563 6970            `recip
-00001f40: 726f 6361 6c60 206f 7220 6064 6972 6563  rocal` or `direc
-00001f50: 7460 2e20 5370 6163 6520 6f66 2063 6f6f  t`. Space of coo
-00001f60: 7264 696e 6174 6573 2074 6f20 6765 6e65  rdinates to gene
-00001f70: 7261 7465 2067 7269 640a 2020 2020 2020  rate grid.      
-00001f80: 2020 2020 2020 6765 6e65 7261 7469 6e67        generating
-00001f90: 206d 6174 7269 7820 6569 7468 6572 2069   matrix either i
-00001fa0: 6e20 6469 7265 6374 206f 7220 7265 6369  n direct or reci
-00001fb0: 7072 6f63 616c 2073 7061 6365 2e20 5468  procal space. Th
-00001fc0: 6520 6465 6661 756c 740a 2020 2020 2020  e default.      
-00001fd0: 2020 2020 2020 6973 2060 7265 6369 7072        is `recipr
-00001fe0: 6f63 616c 602e 0a20 2020 2020 2020 206d  ocal`..        m
-00001ff0: 616b 655f 7230 5f61 7665 7261 6765 203a  ake_r0_average :
-00002000: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0a   bool, optional.
-00002010: 2020 2020 2020 2020 2020 2020 6663 3320              fc3 
-00002020: 7472 616e 7366 6f72 6d61 7469 6f6e 2066  transformation f
-00002030: 726f 6d20 7265 616c 2074 6f20 7265 6369  rom real to reci
-00002040: 7072 6f63 616c 2073 7061 6365 2069 7320  procal space is 
-00002050: 646f 6e65 0a20 2020 2020 2020 2020 2020  done.           
-00002060: 2061 726f 756e 6420 7468 7265 6520 6174   around three at
-00002070: 6f6d 7320 616e 6420 6176 6572 6167 6564  oms and averaged
-00002080: 2077 6865 6e20 5472 7565 2e20 4465 6661   when True. Defa
-00002090: 756c 7420 6973 2046 616c 7365 2c20 692e  ult is False, i.
-000020a0: 652e 2c0a 2020 2020 2020 2020 2020 2020  e.,.            
-000020b0: 6f6e 6c79 2061 726f 756e 6420 7468 6520  only around the 
-000020c0: 6669 7273 7420 6174 6f6d 2e20 5365 7474  first atom. Sett
-000020d0: 696e 6720 4661 6c73 6520 6973 2066 6f72  ing False is for
-000020e0: 2072 6f75 6768 2063 6f6d 7061 7469 6269   rough compatibi
-000020f0: 6c69 7479 0a20 2020 2020 2020 2020 2020  lity.           
-00002100: 2077 6974 6820 7632 2e78 2e20 4465 6661   with v2.x. Defa
-00002110: 756c 7420 6973 2054 7275 652e 0a20 2020  ult is True..   
-00002120: 2020 2020 2073 796d 7072 6563 203a 2066       symprec : f
-00002130: 6c6f 6174 2c20 6f70 7469 6f6e 616c 0a20  loat, optional. 
-00002140: 2020 2020 2020 2020 2020 2054 6f6c 6572             Toler
-00002150: 616e 6365 2075 7365 6420 746f 2066 696e  ance used to fin
-00002160: 6420 6372 7973 7461 6c20 7379 6d6d 6574  d crystal symmet
-00002170: 7279 2e20 4465 6661 756c 7420 6973 2031  ry. Default is 1
-00002180: 652d 352e 0a20 2020 2020 2020 2063 616c  e-5..        cal
-00002190: 6375 6c61 746f 7220 3a20 7374 722c 206f  culator : str, o
-000021a0: 7074 696f 6e61 6c2e 0a20 2020 2020 2020  ptional..       
-000021b0: 2020 2020 2043 616c 6375 6c61 746f 7220       Calculator 
-000021c0: 7573 6564 2066 6f72 2063 6f6d 7075 7469  used for computi
-000021d0: 6e67 2066 6f72 6365 732e 2054 6869 7320  ng forces. This 
-000021e0: 6973 2075 7365 6420 746f 2073 7769 7463  is used to switc
-000021f0: 6820 7468 6520 7365 740a 2020 2020 2020  h the set.      
-00002200: 2020 2020 2020 6f66 2070 6879 7369 6361        of physica
-00002210: 6c20 756e 6974 732e 2044 6566 6175 6c74  l units. Default
-00002220: 2069 7320 4e6f 6e65 2c20 7768 6963 6820   is None, which 
-00002230: 6973 2065 7175 6976 616c 656e 7420 746f  is equivalent to
-00002240: 2022 7661 7370 222e 0a20 2020 2020 2020   "vasp"..       
-00002250: 206c 6f67 5f6c 6576 656c 203a 2069 6e74   log_level : int
-00002260: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-00002270: 2020 2020 2020 2056 6572 626f 7369 7479         Verbosity
-00002280: 2063 6f6e 7472 6f6c 2e20 4465 6661 756c   control. Defaul
-00002290: 7420 6973 2030 2e20 5468 6973 2063 616e  t is 0. This can
-000022a0: 2062 6520 302c 2031 2c20 6f72 2032 2e0a   be 0, 1, or 2..
-000022b0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000022c0: 2020 2020 2073 656c 662e 5f73 796d 7072       self._sympr
-000022d0: 6563 203d 2073 796d 7072 6563 0a20 2020  ec = symprec.   
-000022e0: 2020 2020 2073 656c 662e 5f66 7265 7175       self._frequ
-000022f0: 656e 6379 5f66 6163 746f 725f 746f 5f54  ency_factor_to_T
-00002300: 487a 203d 2066 7265 7175 656e 6379 5f66  Hz = frequency_f
-00002310: 6163 746f 725f 746f 5f54 487a 0a20 2020  actor_to_THz.   
-00002320: 2020 2020 2073 656c 662e 5f69 735f 7379       self._is_sy
-00002330: 6d6d 6574 7279 203d 2069 735f 7379 6d6d  mmetry = is_symm
-00002340: 6574 7279 0a20 2020 2020 2020 2073 656c  etry.        sel
-00002350: 662e 5f69 735f 6d65 7368 5f73 796d 6d65  f._is_mesh_symme
-00002360: 7472 7920 3d20 6973 5f6d 6573 685f 7379  try = is_mesh_sy
-00002370: 6d6d 6574 7279 0a20 2020 2020 2020 2073  mmetry.        s
-00002380: 656c 662e 5f75 7365 5f67 7267 203d 2075  elf._use_grg = u
-00002390: 7365 5f67 7267 0a20 2020 2020 2020 2073  se_grg.        s
-000023a0: 656c 662e 5f53 4e46 5f63 6f6f 7264 696e  elf._SNF_coordin
-000023b0: 6174 6573 203d 2053 4e46 5f63 6f6f 7264  ates = SNF_coord
-000023c0: 696e 6174 6573 0a0a 2020 2020 2020 2020  inates..        
-000023d0: 7365 6c66 2e5f 6d61 6b65 5f72 305f 6176  self._make_r0_av
-000023e0: 6572 6167 6520 3d20 6d61 6b65 5f72 305f  erage = make_r0_
-000023f0: 6176 6572 6167 650a 0a20 2020 2020 2020  average..       
-00002400: 2073 656c 662e 5f63 7574 6f66 665f 6672   self._cutoff_fr
-00002410: 6571 7565 6e63 7920 3d20 6375 746f 6666  equency = cutoff
-00002420: 5f66 7265 7175 656e 6379 0a20 2020 2020  _frequency.     
-00002430: 2020 2073 656c 662e 5f63 616c 6375 6c61     self._calcula
-00002440: 746f 723a 204f 7074 696f 6e61 6c5b 7374  tor: Optional[st
-00002450: 725d 203d 2063 616c 6375 6c61 746f 720a  r] = calculator.
-00002460: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
-00002470: 675f 6c65 7665 6c20 3d20 6c6f 675f 6c65  g_level = log_le
-00002480: 7665 6c0a 0a20 2020 2020 2020 2023 2043  vel..        # C
-00002490: 7265 6174 6520 7375 7065 7263 656c 6c20  reate supercell 
-000024a0: 616e 6420 7072 696d 6974 6976 6520 6365  and primitive ce
-000024b0: 6c6c 0a20 2020 2020 2020 2073 656c 662e  ll.        self.
-000024c0: 5f75 6e69 7463 656c 6c20 3d20 756e 6974  _unitcell = unit
-000024d0: 6365 6c6c 0a20 2020 2020 2020 2073 656c  cell.        sel
-000024e0: 662e 5f73 7570 6572 6365 6c6c 5f6d 6174  f._supercell_mat
-000024f0: 7269 7820 3d20 6e70 2e61 7272 6179 280a  rix = np.array(.
-00002500: 2020 2020 2020 2020 2020 2020 7368 6170              shap
-00002510: 655f 7375 7065 7263 656c 6c5f 6d61 7472  e_supercell_matr
-00002520: 6978 2873 7570 6572 6365 6c6c 5f6d 6174  ix(supercell_mat
-00002530: 7269 7829 2c20 6474 7970 653d 2269 6e74  rix), dtype="int
-00002540: 5f22 2c20 6f72 6465 723d 2243 220a 2020  _", order="C".  
-00002550: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00002560: 706d 6174 203d 2073 656c 662e 5f64 6574  pmat = self._det
-00002570: 6572 6d69 6e65 5f70 7269 6d69 7469 7665  ermine_primitive
-00002580: 5f6d 6174 7269 7828 7072 696d 6974 6976  _matrix(primitiv
-00002590: 655f 6d61 7472 6978 290a 2020 2020 2020  e_matrix).      
-000025a0: 2020 7365 6c66 2e5f 7072 696d 6974 6976    self._primitiv
-000025b0: 655f 6d61 7472 6978 203d 2070 6d61 740a  e_matrix = pmat.
-000025c0: 2020 2020 2020 2020 7365 6c66 2e5f 6e61          self._na
-000025d0: 635f 7061 7261 6d73 203d 204e 6f6e 650a  c_params = None.
-000025e0: 2020 2020 2020 2020 6966 2070 686f 6e6f          if phono
-000025f0: 6e5f 7375 7065 7263 656c 6c5f 6d61 7472  n_supercell_matr
-00002600: 6978 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ix is not None:.
-00002610: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00002620: 2e5f 7068 6f6e 6f6e 5f73 7570 6572 6365  ._phonon_superce
-00002630: 6c6c 5f6d 6174 7269 7820 3d20 6e70 2e61  ll_matrix = np.a
-00002640: 7272 6179 280a 2020 2020 2020 2020 2020  rray(.          
-00002650: 2020 2020 2020 7368 6170 655f 7375 7065        shape_supe
-00002660: 7263 656c 6c5f 6d61 7472 6978 2870 686f  rcell_matrix(pho
-00002670: 6e6f 6e5f 7375 7065 7263 656c 6c5f 6d61  non_supercell_ma
-00002680: 7472 6978 292c 2064 7479 7065 3d22 696e  trix), dtype="in
-00002690: 745f 222c 206f 7264 6572 3d22 4322 0a20  t_", order="C". 
-000026a0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-000026b0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000026c0: 2020 2020 2020 2073 656c 662e 5f70 686f         self._pho
-000026d0: 6e6f 6e5f 7375 7065 7263 656c 6c5f 6d61  non_supercell_ma
-000026e0: 7472 6978 203d 204e 6f6e 650a 2020 2020  trix = None.    
-000026f0: 2020 2020 7365 6c66 2e5f 7375 7065 7263      self._superc
-00002700: 656c 6c20 3d20 4e6f 6e65 0a20 2020 2020  ell = None.     
-00002710: 2020 2073 656c 662e 5f70 7269 6d69 7469     self._primiti
-00002720: 7665 203d 204e 6f6e 650a 2020 2020 2020  ve = None.      
-00002730: 2020 7365 6c66 2e5f 7068 6f6e 6f6e 5f73    self._phonon_s
-00002740: 7570 6572 6365 6c6c 203d 204e 6f6e 650a  upercell = None.
-00002750: 2020 2020 2020 2020 7365 6c66 2e5f 7068          self._ph
-00002760: 6f6e 6f6e 5f70 7269 6d69 7469 7665 203d  onon_primitive =
-00002770: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
-00002780: 6c66 2e5f 6275 696c 645f 7375 7065 7263  lf._build_superc
-00002790: 656c 6c28 290a 2020 2020 2020 2020 7365  ell().        se
-000027a0: 6c66 2e5f 6275 696c 645f 7072 696d 6974  lf._build_primit
-000027b0: 6976 655f 6365 6c6c 2829 0a20 2020 2020  ive_cell().     
-000027c0: 2020 2073 656c 662e 5f62 7569 6c64 5f70     self._build_p
-000027d0: 686f 6e6f 6e5f 7375 7065 7263 656c 6c28  honon_supercell(
-000027e0: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
-000027f0: 6275 696c 645f 7068 6f6e 6f6e 5f70 7269  build_phonon_pri
-00002800: 6d69 7469 7665 5f63 656c 6c28 290a 0a20  mitive_cell().. 
-00002810: 2020 2020 2020 2073 656c 662e 5f73 6967         self._sig
-00002820: 6d61 7320 3d20 5b0a 2020 2020 2020 2020  mas = [.        
-00002830: 2020 2020 4e6f 6e65 2c0a 2020 2020 2020      None,.      
-00002840: 2020 5d0a 2020 2020 2020 2020 7365 6c66    ].        self
-00002850: 2e5f 7369 676d 615f 6375 746f 6666 203d  ._sigma_cutoff =
-00002860: 204e 6f6e 650a 0a20 2020 2020 2020 2023   None..        #
-00002870: 2047 7269 640a 2020 2020 2020 2020 7365   Grid.        se
-00002880: 6c66 2e5f 627a 5f67 7269 6420 3d20 4e6f  lf._bz_grid = No
-00002890: 6e65 0a0a 2020 2020 2020 2020 2320 5365  ne..        # Se
-000028a0: 7420 7375 7065 7263 656c 6c2c 2070 7269  t supercell, pri
-000028b0: 6d69 7469 7665 2c20 616e 6420 7068 6f6e  mitive, and phon
-000028c0: 6f6e 2073 7570 6572 6365 6c6c 2073 796d  on supercell sym
-000028d0: 6d65 7472 6965 730a 2020 2020 2020 2020  metries.        
-000028e0: 7365 6c66 2e5f 7379 6d6d 6574 7279 203d  self._symmetry =
-000028f0: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
-00002900: 6c66 2e5f 7072 696d 6974 6976 655f 7379  lf._primitive_sy
-00002910: 6d6d 6574 7279 203d 204e 6f6e 650a 2020  mmetry = None.  
-00002920: 2020 2020 2020 7365 6c66 2e5f 7068 6f6e        self._phon
-00002930: 6f6e 5f73 7570 6572 6365 6c6c 5f73 796d  on_supercell_sym
-00002940: 6d65 7472 7920 3d20 4e6f 6e65 0a20 2020  metry = None.   
-00002950: 2020 2020 2073 656c 662e 5f73 6561 7263       self._searc
-00002960: 685f 7379 6d6d 6574 7279 2829 0a20 2020  h_symmetry().   
-00002970: 2020 2020 2073 656c 662e 5f73 6561 7263       self._searc
-00002980: 685f 7072 696d 6974 6976 655f 7379 6d6d  h_primitive_symm
-00002990: 6574 7279 2829 0a20 2020 2020 2020 2073  etry().        s
-000029a0: 656c 662e 5f73 6561 7263 685f 7068 6f6e  elf._search_phon
-000029b0: 6f6e 5f73 7570 6572 6365 6c6c 5f73 796d  on_supercell_sym
-000029c0: 6d65 7472 7928 290a 0a20 2020 2020 2020  metry()..       
-000029d0: 2023 2044 6973 706c 6163 656d 656e 7473   # Displacements
-000029e0: 2061 6e64 2073 7570 6572 6365 6c6c 730a   and supercells.
-000029f0: 2020 2020 2020 2020 7365 6c66 2e5f 7375          self._su
-00002a00: 7065 7263 656c 6c73 5f77 6974 685f 6469  percells_with_di
-00002a10: 7370 6c61 6365 6d65 6e74 7320 3d20 4e6f  splacements = No
-00002a20: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
-00002a30: 5f64 6174 6173 6574 203d 204e 6f6e 650a  _dataset = None.
-00002a40: 2020 2020 2020 2020 7365 6c66 2e5f 7068          self._ph
-00002a50: 6f6e 6f6e 5f64 6174 6173 6574 203d 204e  onon_dataset = N
-00002a60: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
-00002a70: 2e5f 7068 6f6e 6f6e 5f73 7570 6572 6365  ._phonon_superce
-00002a80: 6c6c 735f 7769 7468 5f64 6973 706c 6163  lls_with_displac
-00002a90: 656d 656e 7473 203d 204e 6f6e 650a 0a20  ements = None.. 
-00002aa0: 2020 2020 2020 2023 2054 6865 726d 616c         # Thermal
-00002ab0: 2063 6f6e 6475 6374 6976 6974 790a 2020   conductivity.  
-00002ac0: 2020 2020 2020 2320 636f 6e64 7563 7469        # conducti
-00002ad0: 7669 7479 5f52 5441 206f 7220 636f 6e64  vity_RTA or cond
-00002ae0: 7563 7469 7669 7479 5f4c 4254 4520 636c  uctivity_LBTE cl
-00002af0: 6173 7320 696e 7374 616e 6365 0a20 2020  ass instance.   
-00002b00: 2020 2020 2073 656c 662e 5f74 6865 726d       self._therm
-00002b10: 616c 5f63 6f6e 6475 6374 6976 6974 7920  al_conductivity 
-00002b20: 3d20 4e6f 6e65 0a0a 2020 2020 2020 2020  = None..        
-00002b30: 2320 496d 6167 696e 6172 7920 7061 7274  # Imaginary part
-00002b40: 206f 6620 7365 6c66 2065 6e65 7267 7920   of self energy 
-00002b50: 6174 2066 7265 7175 656e 6379 2070 6f69  at frequency poi
-00002b60: 6e74 730a 2020 2020 2020 2020 7365 6c66  nts.        self
-00002b70: 2e5f 6761 6d6d 6173 203d 204e 6f6e 650a  ._gammas = None.
-00002b80: 2020 2020 2020 2020 7365 6c66 2e5f 7363          self._sc
-00002b90: 6174 7465 7269 6e67 5f65 7665 6e74 5f63  attering_event_c
-00002ba0: 6c61 7373 203d 204e 6f6e 650a 0a20 2020  lass = None..   
-00002bb0: 2020 2020 2023 2046 7265 7175 656e 6379       # Frequency
-00002bc0: 2073 6869 6674 2028 7265 616c 2070 6172   shift (real par
-00002bd0: 7420 6f66 2062 7562 626c 6520 6469 6167  t of bubble diag
-00002be0: 7261 6d29 0a20 2020 2020 2020 2073 656c  ram).        sel
-00002bf0: 662e 5f72 6561 6c5f 7365 6c66 5f65 6e65  f._real_self_ene
-00002c00: 7267 7920 3d20 4e6f 6e65 0a0a 2020 2020  rgy = None..    
-00002c10: 2020 2020 7365 6c66 2e5f 6772 6964 5f70      self._grid_p
-00002c20: 6f69 6e74 7320 3d20 4e6f 6e65 0a20 2020  oints = None.   
-00002c30: 2020 2020 2073 656c 662e 5f66 7265 7175       self._frequ
-00002c40: 656e 6379 5f70 6f69 6e74 7320 3d20 4e6f  ency_points = No
-00002c50: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
-00002c60: 5f74 656d 7065 7261 7475 7265 7320 3d20  _temperatures = 
-00002c70: 4e6f 6e65 0a0a 2020 2020 2020 2020 2320  None..        # 
-00002c80: 4f74 6865 7220 7661 7269 6162 6c65 730a  Other variables.
-00002c90: 2020 2020 2020 2020 7365 6c66 2e5f 6663          self._fc
-00002ca0: 3220 3d20 4e6f 6e65 0a20 2020 2020 2020  2 = None.       
-00002cb0: 2073 656c 662e 5f66 6333 203d 204e 6f6e   self._fc3 = Non
-00002cc0: 650a 0a20 2020 2020 2020 2023 2053 6574  e..        # Set
-00002cd0: 7570 2069 6e74 6572 6163 7469 6f6e 0a20  up interaction. 
-00002ce0: 2020 2020 2020 2073 656c 662e 5f69 6e74         self._int
-00002cf0: 6572 6163 7469 6f6e 203d 204e 6f6e 650a  eraction = None.
-00002d00: 2020 2020 2020 2020 7365 6c66 2e5f 6261          self._ba
-00002d10: 6e64 5f69 6e64 6963 6573 203d 204e 6f6e  nd_indices = Non
-00002d20: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
-00002d30: 6261 6e64 5f69 6e64 6963 6573 5f66 6c61  band_indices_fla
-00002d40: 7474 656e 203d 204e 6f6e 650a 2020 2020  tten = None.    
-00002d50: 2020 2020 7365 6c66 2e5f 7365 745f 6261      self._set_ba
-00002d60: 6e64 5f69 6e64 6963 6573 2829 0a0a 2020  nd_indices()..  
-00002d70: 2020 2020 2020 6966 206d 6173 7365 7320        if masses 
-00002d80: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00002d90: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
-00002da0: 732e 7761 726e 280a 2020 2020 2020 2020  s.warn(.        
-00002db0: 2020 2020 2020 2020 2250 686f 6e6f 3370          "Phono3p
-00002dc0: 7920 696e 6974 2070 6172 616d 6574 6572  y init parameter
-00002dd0: 206f 6620 6d61 7373 6573 2069 7320 6465   of masses is de
-00002de0: 7072 6563 6174 6564 2e20 220a 2020 2020  precated. ".    
-00002df0: 2020 2020 2020 2020 2020 2020 2255 7365              "Use
-00002e00: 2050 686f 6e6f 3370 792e 6d61 7373 6573   Phono3py.masses
-00002e10: 2061 7474 7269 6275 7465 2069 6e73 7465   attribute inste
-00002e20: 6164 2e22 2c0a 2020 2020 2020 2020 2020  ad.",.          
-00002e30: 2020 2020 2020 4465 7072 6563 6174 696f        Deprecatio
-00002e40: 6e57 6172 6e69 6e67 2c0a 2020 2020 2020  nWarning,.      
-00002e50: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00002e60: 2020 2020 7365 6c66 2e6d 6173 7365 7320      self.masses 
-00002e70: 3d20 6d61 7373 6573 0a0a 2020 2020 2020  = masses..      
-00002e80: 2020 6966 2062 616e 645f 696e 6469 6365    if band_indice
-00002e90: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-00002ea0: 2020 2020 2020 2020 2020 2077 6172 6e69             warni
-00002eb0: 6e67 732e 7761 726e 280a 2020 2020 2020  ngs.warn(.      
-00002ec0: 2020 2020 2020 2020 2020 2250 686f 6e6f            "Phono
-00002ed0: 3370 7920 696e 6974 2070 6172 616d 6574  3py init paramet
-00002ee0: 6572 206f 6620 6261 6e64 5f69 6e64 6963  er of band_indic
-00002ef0: 6573 2069 7320 6465 7072 6563 6174 6564  es is deprecated
-00002f00: 2e20 220a 2020 2020 2020 2020 2020 2020  . ".            
-00002f10: 2020 2020 2255 7365 2050 686f 6e6f 3370      "Use Phono3p
-00002f20: 792e 6261 6e64 5f69 6e64 6963 6573 2061  y.band_indices a
-00002f30: 7474 7269 6275 7465 2069 6e73 7465 6164  ttribute instead
-00002f40: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
-00002f50: 2020 2020 4465 7072 6563 6174 696f 6e57      DeprecationW
-00002f60: 6172 6e69 6e67 2c0a 2020 2020 2020 2020  arning,.        
-00002f70: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00002f80: 2020 7365 6c66 2e62 616e 645f 696e 6469    self.band_indi
-00002f90: 6365 7320 3d20 6261 6e64 5f69 6e64 6963  ces = band_indic
-00002fa0: 6573 0a0a 2020 2020 2020 2020 6966 2073  es..        if s
-00002fb0: 6967 6d61 7320 6973 206e 6f74 204e 6f6e  igmas is not Non
-00002fc0: 653a 0a20 2020 2020 2020 2020 2020 2077  e:.            w
-00002fd0: 6172 6e69 6e67 732e 7761 726e 280a 2020  arnings.warn(.  
-00002fe0: 2020 2020 2020 2020 2020 2020 2020 2250                "P
-00002ff0: 686f 6e6f 3370 7920 696e 6974 2070 6172  hono3py init par
-00003000: 616d 6574 6572 206f 6620 7369 676d 6173  ameter of sigmas
-00003010: 2069 7320 6465 7072 6563 6174 6564 2e20   is deprecated. 
-00003020: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00003030: 2020 2255 7365 2050 686f 6e6f 3370 792e    "Use Phono3py.
-00003040: 7369 676d 6173 2061 7474 7269 6275 7465  sigmas attribute
-00003050: 2069 6e73 7465 6164 2e22 2c0a 2020 2020   instead.",.    
-00003060: 2020 2020 2020 2020 2020 2020 4465 7072              Depr
-00003070: 6563 6174 696f 6e57 6172 6e69 6e67 2c0a  ecationWarning,.
-00003080: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00003090: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-000030a0: 6967 6d61 7320 3d20 7369 676d 6173 0a0a  igmas = sigmas..
-000030b0: 2020 2020 2020 2020 6966 2073 6967 6d61          if sigma
-000030c0: 5f63 7574 6f66 6620 6973 206e 6f74 204e  _cutoff is not N
-000030d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000030e0: 2077 6172 6e69 6e67 732e 7761 726e 280a   warnings.warn(.
-000030f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003100: 2250 686f 6e6f 3370 7920 696e 6974 2070  "Phono3py init p
-00003110: 6172 616d 6574 6572 206f 6620 7369 676d  arameter of sigm
-00003120: 615f 6375 746f 6666 2069 7320 6465 7072  a_cutoff is depr
-00003130: 6563 6174 6564 2e20 220a 2020 2020 2020  ecated. ".      
-00003140: 2020 2020 2020 2020 2020 2255 7365 2050            "Use P
-00003150: 686f 6e6f 3370 792e 7369 676d 615f 6375  hono3py.sigma_cu
-00003160: 746f 6666 2061 7474 7269 6275 7465 2069  toff attribute i
-00003170: 6e73 7465 6164 2e22 2c0a 2020 2020 2020  nstead.",.      
-00003180: 2020 2020 2020 2020 2020 4465 7072 6563            Deprec
-00003190: 6174 696f 6e57 6172 6e69 6e67 2c0a 2020  ationWarning,.  
-000031a0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-000031b0: 2020 2020 2020 2020 7365 6c66 2e73 6967          self.sig
-000031c0: 6d61 5f63 7574 6f66 6620 3d20 7369 676d  ma_cutoff = sigm
-000031d0: 615f 6375 746f 6666 0a0a 2020 2020 4070  a_cutoff..    @p
-000031e0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-000031f0: 7665 7273 696f 6e28 7365 6c66 293a 0a20  version(self):. 
-00003200: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
-00003210: 2070 686f 6e6f 3370 7920 7265 6c65 6173   phono3py releas
-00003220: 6520 7665 7273 696f 6e20 6e75 6d62 6572  e version number
-00003230: 2e0a 0a20 2020 2020 2020 2073 7472 0a20  ...        str. 
-00003240: 2020 2020 2020 2020 2020 2050 686f 6e6f             Phono
-00003250: 3370 7920 7265 6c65 6173 6520 7665 7273  3py release vers
-00003260: 696f 6e20 6e75 6d62 6572 0a0a 2020 2020  ion number..    
-00003270: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00003280: 7265 7475 726e 205f 5f76 6572 7369 6f6e  return __version
-00003290: 5f5f 0a0a 2020 2020 6465 6620 6765 745f  __..    def get_
-000032a0: 7665 7273 696f 6e28 7365 6c66 293a 0a20  version(self):. 
-000032b0: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
-000032c0: 2070 686f 6e6f 3370 7920 7265 6c65 6173   phono3py releas
-000032d0: 6520 7665 7273 696f 6e20 6e75 6d62 6572  e version number
-000032e0: 2e22 2222 0a20 2020 2020 2020 2077 6172  .""".        war
-000032f0: 6e69 6e67 732e 7761 726e 280a 2020 2020  nings.warn(.    
-00003300: 2020 2020 2020 2020 2250 686f 6e6f 3370          "Phono3p
-00003310: 792e 6765 745f 7665 7273 696f 6e28 2920  y.get_version() 
-00003320: 6973 2064 6570 7265 6361 7465 642e 220a  is deprecated.".
-00003330: 2020 2020 2020 2020 2020 2020 2255 7365              "Use
-00003340: 2050 686f 6e6f 3370 792e 7665 7273 696f   Phono3py.versio
-00003350: 6e20 6174 7472 6962 7574 6520 696e 7374  n attribute inst
-00003360: 6561 642e 222c 0a20 2020 2020 2020 2020  ead.",.         
-00003370: 2020 2044 6570 7265 6361 7469 6f6e 5761     DeprecationWa
-00003380: 726e 696e 672c 0a20 2020 2020 2020 2029  rning,.        )
-00003390: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000033a0: 7365 6c66 2e76 6572 7369 6f6e 0a0a 2020  self.version..  
-000033b0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-000033c0: 6465 6620 6361 6c63 756c 6174 6f72 2873  def calculator(s
-000033d0: 656c 6629 202d 3e20 4f70 7469 6f6e 616c  elf) -> Optional
-000033e0: 5b73 7472 5d3a 0a20 2020 2020 2020 2022  [str]:.        "
-000033f0: 2222 5265 7475 726e 2063 616c 6375 6c61  ""Return calcula
-00003400: 746f 7220 696e 7465 7266 6163 6520 6e61  tor interface na
-00003410: 6d65 2e0a 0a20 2020 2020 2020 2073 7472  me...        str
-00003420: 0a20 2020 2020 2020 2020 2020 2043 616c  .            Cal
-00003430: 6375 6c61 746f 7220 6e61 6d65 2073 7563  culator name suc
-00003440: 6820 6173 2027 7661 7370 272c 2027 7165  h as 'vasp', 'qe
-00003450: 272c 2065 7463 2e0a 0a20 2020 2020 2020  ', etc...       
-00003460: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-00003470: 7572 6e20 7365 6c66 2e5f 6361 6c63 756c  urn self._calcul
-00003480: 6174 6f72 0a0a 2020 2020 4070 726f 7065  ator..    @prope
-00003490: 7274 790a 2020 2020 6465 6620 6663 3328  rty.    def fc3(
-000034a0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-000034b0: 2222 5365 7474 6572 2061 6e64 2067 6574  ""Setter and get
-000034c0: 7465 7220 6f66 2074 6869 7264 206f 7264  ter of third ord
-000034d0: 6572 2066 6f72 6365 2063 6f6e 7374 616e  er force constan
-000034e0: 7473 2028 6663 3329 2e0a 0a20 2020 2020  ts (fc3)...     
-000034f0: 2020 206e 6461 7272 6179 0a20 2020 2020     ndarray.     
-00003500: 2020 2020 2020 2066 6333 2073 6861 7065         fc3 shape
-00003510: 2069 7320 6569 7468 6572 2028 7375 7065   is either (supe
-00003520: 7263 656c 6c2c 2073 7570 6563 656c 6c2c  rcell, supecell,
-00003530: 2073 7570 6572 6365 6c6c 2c20 332c 2033   supercell, 3, 3
-00003540: 2c20 3329 206f 720a 2020 2020 2020 2020  , 3) or.        
-00003550: 2020 2020 2870 7269 6d69 7469 7665 2c20      (primitive, 
-00003560: 7375 7065 7263 656c 6c2c 2073 7570 6563  supercell, supec
-00003570: 656c 6c2c 2033 2c20 332c 2033 292c 0a20  ell, 3, 3, 3),. 
-00003580: 2020 2020 2020 2020 2020 2077 6865 7265             where
-00003590: 2027 7375 7065 7263 656c 6c27 2061 6e64   'supercell' and
-000035a0: 2027 7072 696d 6974 6976 6527 2069 6e64   'primitive' ind
-000035b0: 6963 6174 6520 6e75 6d62 6572 206f 6620  icate number of 
-000035c0: 6174 6f6d 7320 696e 0a20 2020 2020 2020  atoms in.       
-000035d0: 2020 2020 2074 6865 7365 2063 656c 6c73       these cells
-000035e0: 2e0a 0a20 2020 2020 2020 2022 2222 0a20  ...        """. 
-000035f0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00003600: 6c66 2e5f 6663 330a 0a20 2020 2040 6663  lf._fc3..    @fc
-00003610: 332e 7365 7474 6572 0a20 2020 2064 6566  3.setter.    def
-00003620: 2066 6333 2873 656c 662c 2066 6333 293a   fc3(self, fc3):
-00003630: 0a20 2020 2020 2020 2073 656c 662e 5f66  .        self._f
-00003640: 6333 203d 2066 6333 0a0a 2020 2020 6465  c3 = fc3..    de
-00003650: 6620 6765 745f 6663 3328 7365 6c66 293a  f get_fc3(self):
-00003660: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-00003670: 726e 2074 6869 7264 206f 7264 6572 2066  rn third order f
-00003680: 6f72 6365 2063 6f6e 7374 616e 7473 2028  orce constants (
-00003690: 6663 3329 2e22 2222 0a20 2020 2020 2020  fc3).""".       
-000036a0: 2077 6172 6e69 6e67 732e 7761 726e 280a   warnings.warn(.
-000036b0: 2020 2020 2020 2020 2020 2020 2250 686f              "Pho
-000036c0: 6e6f 3370 792e 6765 745f 6663 3328 2920  no3py.get_fc3() 
-000036d0: 6973 2064 6570 7265 6361 7465 642e 2220  is deprecated." 
-000036e0: 2255 7365 2050 686f 6e6f 3370 792e 6663  "Use Phono3py.fc
-000036f0: 3320 6174 7472 6962 7574 6520 696e 7374  3 attribute inst
-00003700: 6561 642e 222c 0a20 2020 2020 2020 2020  ead.",.         
-00003710: 2020 2044 6570 7265 6361 7469 6f6e 5761     DeprecationWa
-00003720: 726e 696e 672c 0a20 2020 2020 2020 2029  rning,.        )
-00003730: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00003740: 7365 6c66 2e66 6333 0a0a 2020 2020 6465  self.fc3..    de
-00003750: 6620 7365 745f 6663 3328 7365 6c66 2c20  f set_fc3(self, 
-00003760: 6663 3329 3a0a 2020 2020 2020 2020 2222  fc3):.        ""
-00003770: 2253 6574 2066 6333 2e22 2222 0a20 2020  "Set fc3.""".   
-00003780: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
-00003790: 726e 280a 2020 2020 2020 2020 2020 2020  rn(.            
-000037a0: 2250 686f 6e6f 3370 792e 7365 745f 6663  "Phono3py.set_fc
-000037b0: 3328 2920 6973 2064 6570 7265 6361 7465  3() is deprecate
-000037c0: 642e 2220 2255 7365 2050 686f 6e6f 3370  d." "Use Phono3p
-000037d0: 792e 6663 3320 6174 7472 6962 7574 6520  y.fc3 attribute 
-000037e0: 696e 7374 6561 642e 222c 0a20 2020 2020  instead.",.     
-000037f0: 2020 2020 2020 2044 6570 7265 6361 7469         Deprecati
-00003800: 6f6e 5761 726e 696e 672c 0a20 2020 2020  onWarning,.     
-00003810: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
-00003820: 662e 6663 3320 3d20 6663 330a 0a20 2020  f.fc3 = fc3..   
-00003830: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00003840: 6566 2066 6332 2873 656c 6629 3a0a 2020  ef fc2(self):.  
-00003850: 2020 2020 2020 2222 2253 6574 7465 7220        """Setter 
-00003860: 616e 6420 6765 7474 6572 206f 6620 7365  and getter of se
-00003870: 636f 6e64 206f 7264 6572 2066 6f72 6365  cond order force
-00003880: 2063 6f6e 7374 616e 7473 2028 6663 3229   constants (fc2)
-00003890: 2e0a 0a20 2020 2020 2020 206e 6461 7272  ...        ndarr
-000038a0: 6179 0a20 2020 2020 2020 2020 2020 2066  ay.            f
-000038b0: 6332 2073 6861 7065 2069 7320 6569 7468  c2 shape is eith
-000038c0: 6572 2028 7375 7065 7263 656c 6c2c 2073  er (supercell, s
-000038d0: 7570 6563 656c 6c2c 2033 2c20 3329 206f  upecell, 3, 3) o
-000038e0: 720a 2020 2020 2020 2020 2020 2020 2870  r.            (p
-000038f0: 7269 6d69 7469 7665 2c20 7375 7065 6365  rimitive, supece
-00003900: 6c6c 2c20 332c 2033 292c 0a20 2020 2020  ll, 3, 3),.     
-00003910: 2020 2020 2020 2077 6865 7265 2027 7375         where 'su
-00003920: 7065 7263 656c 6c27 2061 6e64 2027 7072  percell' and 'pr
-00003930: 696d 6974 6976 6527 2069 6e64 6963 6174  imitive' indicat
-00003940: 6520 6e75 6d62 6572 206f 6620 6174 6f6d  e number of atom
-00003950: 7320 696e 0a20 2020 2020 2020 2020 2020  s in.           
-00003960: 2074 6865 7365 2063 656c 6c73 2e0a 0a20   these cells... 
-00003970: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00003980: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00003990: 6663 320a 0a20 2020 2040 6663 322e 7365  fc2..    @fc2.se
-000039a0: 7474 6572 0a20 2020 2064 6566 2066 6332  tter.    def fc2
-000039b0: 2873 656c 662c 2066 6332 293a 0a20 2020  (self, fc2):.   
-000039c0: 2020 2020 2073 656c 662e 5f66 6332 203d       self._fc2 =
-000039d0: 2066 6332 0a0a 2020 2020 6465 6620 6765   fc2..    def ge
-000039e0: 745f 6663 3228 7365 6c66 293a 0a20 2020  t_fc2(self):.   
-000039f0: 2020 2020 2022 2222 5265 7475 726e 2073       """Return s
-00003a00: 6563 6f6e 6420 6f72 6465 7220 666f 7263  econd order forc
-00003a10: 6520 636f 6e73 7461 6e74 7320 2866 6332  e constants (fc2
-00003a20: 292e 2222 220a 2020 2020 2020 2020 7761  ).""".        wa
-00003a30: 726e 696e 6773 2e77 6172 6e28 0a20 2020  rnings.warn(.   
-00003a40: 2020 2020 2020 2020 2022 5068 6f6e 6f33           "Phono3
-00003a50: 7079 2e67 6574 5f66 6332 2829 2069 7320  py.get_fc2() is 
-00003a60: 6465 7072 6563 6174 6564 2e22 2022 5573  deprecated." "Us
-00003a70: 6520 5068 6f6e 6f33 7079 2e66 6332 2061  e Phono3py.fc2 a
-00003a80: 7474 7269 6275 7465 2069 6e73 7465 6164  ttribute instead
-00003a90: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
-00003aa0: 4465 7072 6563 6174 696f 6e57 6172 6e69  DeprecationWarni
-00003ab0: 6e67 2c0a 2020 2020 2020 2020 290a 2020  ng,.        ).  
-00003ac0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00003ad0: 662e 6663 320a 0a20 2020 2064 6566 2073  f.fc2..    def s
-00003ae0: 6574 5f66 6332 2873 656c 662c 2066 6332  et_fc2(self, fc2
-00003af0: 293a 0a20 2020 2020 2020 2022 2222 5365  ):.        """Se
-00003b00: 7420 6663 322e 2222 220a 2020 2020 2020  t fc2.""".      
-00003b10: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
-00003b20: 0a20 2020 2020 2020 2020 2020 2022 5068  .            "Ph
-00003b30: 6f6e 6f33 7079 2e73 6574 5f66 6332 2829  ono3py.set_fc2()
-00003b40: 2069 7320 6465 7072 6563 6174 6564 2e22   is deprecated."
-00003b50: 2022 5573 6520 5068 6f6e 6f33 7079 2e66   "Use Phono3py.f
-00003b60: 6332 2061 7474 7269 6275 7465 2069 6e73  c2 attribute ins
-00003b70: 7465 6164 2e22 2c0a 2020 2020 2020 2020  tead.",.        
-00003b80: 2020 2020 4465 7072 6563 6174 696f 6e57      DeprecationW
-00003b90: 6172 6e69 6e67 2c0a 2020 2020 2020 2020  arning,.        
-00003ba0: 290a 2020 2020 2020 2020 7365 6c66 2e66  ).        self.f
-00003bb0: 6332 203d 2066 6332 0a0a 2020 2020 4070  c2 = fc2..    @p
-00003bc0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00003bd0: 666f 7263 655f 636f 6e73 7461 6e74 7328  force_constants(
-00003be0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00003bf0: 2222 5265 7475 726e 2066 6332 2e20 5468  ""Return fc2. Th
-00003c00: 6973 2069 7320 7361 6d65 2061 7320 7468  is is same as th
-00003c10: 6520 6765 7474 6572 2061 7474 7269 6275  e getter attribu
-00003c20: 7465 2060 6663 3260 2e22 2222 0a20 2020  te `fc2`.""".   
-00003c30: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00003c40: 2e66 6332 0a0a 2020 2020 4070 726f 7065  .fc2..    @prope
-00003c50: 7274 790a 2020 2020 6465 6620 7369 676d  rty.    def sigm
-00003c60: 6173 2873 656c 6629 3a0a 2020 2020 2020  as(self):.      
-00003c70: 2020 2222 2253 6574 7465 7220 616e 6420    """Setter and 
-00003c80: 6765 7474 6572 206f 6620 736d 6561 7269  getter of smeari
-00003c90: 6e67 2077 6964 7468 732e 0a0a 2020 2020  ng widths...    
-00003ca0: 2020 2020 6c69 7374 0a20 2020 2020 2020      list.       
-00003cb0: 2020 2020 2054 6865 2066 6c6f 6174 2076       The float v
-00003cc0: 616c 7565 7320 6172 6520 6769 7665 6e20  alues are given 
-00003cd0: 6173 2074 6865 2073 7461 6e64 6172 6420  as the standard 
-00003ce0: 6465 7669 6174 696f 6e73 206f 6620 4761  deviations of Ga
-00003cf0: 7573 7369 616e 0a20 2020 2020 2020 2020  ussian.         
-00003d00: 2020 2066 756e 6374 696f 6e2e 2049 6620     function. If 
-00003d10: 4e6f 6e65 2069 7320 6769 7665 6e20 6173  None is given as
-00003d20: 2061 6e20 656c 656d 656e 7420 6f66 2074   an element of t
-00003d30: 6869 7320 6c69 7374 2c20 6c69 6e65 6172  his list, linear
-00003d40: 0a20 2020 2020 2020 2020 2020 2074 6574  .            tet
-00003d50: 7261 6865 6472 6f6e 206d 6574 686f 6420  rahedron method 
-00003d60: 6973 2075 7365 6420 696e 7374 6561 6420  is used instead 
-00003d70: 6f66 2073 6d65 6172 696e 6720 6d65 7468  of smearing meth
-00003d80: 6f64 2e0a 0a20 2020 2020 2020 2022 2222  od...        """
-00003d90: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00003da0: 7365 6c66 2e5f 7369 676d 6173 0a0a 2020  self._sigmas..  
-00003db0: 2020 4073 6967 6d61 732e 7365 7474 6572    @sigmas.setter
-00003dc0: 0a20 2020 2064 6566 2073 6967 6d61 7328  .    def sigmas(
-00003dd0: 7365 6c66 2c20 7369 676d 6173 293a 0a20  self, sigmas):. 
-00003de0: 2020 2020 2020 2069 6620 7369 676d 6173         if sigmas
-00003df0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00003e00: 2020 2020 2020 7365 6c66 2e5f 7369 676d        self._sigm
-00003e10: 6173 203d 205b 0a20 2020 2020 2020 2020  as = [.         
-00003e20: 2020 2020 2020 204e 6f6e 652c 0a20 2020         None,.   
-00003e30: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-00003e40: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
-00003e50: 6365 2873 6967 6d61 732c 2066 6c6f 6174  ce(sigmas, float
-00003e60: 2920 6f72 2069 7369 6e73 7461 6e63 6528  ) or isinstance(
-00003e70: 7369 676d 6173 2c20 696e 7429 3a0a 2020  sigmas, int):.  
-00003e80: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00003e90: 7369 676d 6173 203d 205b 0a20 2020 2020  sigmas = [.     
-00003ea0: 2020 2020 2020 2020 2020 2066 6c6f 6174             float
-00003eb0: 2873 6967 6d61 7329 2c0a 2020 2020 2020  (sigmas),.      
-00003ec0: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
-00003ed0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00003ee0: 2020 7365 6c66 2e5f 7369 676d 6173 203d    self._sigmas =
-00003ef0: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
-00003f00: 666f 7220 7320 696e 2073 6967 6d61 733a  for s in sigmas:
-00003f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003f20: 2069 6620 6973 696e 7374 616e 6365 2873   if isinstance(s
-00003f30: 2c20 666c 6f61 7429 206f 7220 6973 696e  , float) or isin
-00003f40: 7374 616e 6365 2873 2c20 696e 7429 3a0a  stance(s, int):.
-00003f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f60: 2020 2020 7365 6c66 2e5f 7369 676d 6173      self._sigmas
-00003f70: 2e61 7070 656e 6428 666c 6f61 7428 7329  .append(float(s)
-00003f80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00003f90: 2020 656c 6966 2073 2069 7320 4e6f 6e65    elif s is None
-00003fa0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003fb0: 2020 2020 2020 7365 6c66 2e5f 7369 676d        self._sigm
-00003fc0: 6173 2e61 7070 656e 6428 4e6f 6e65 290a  as.append(None).
-00003fd0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00003fe0: 2020 2064 6566 2073 6967 6d61 5f63 7574     def sigma_cut
-00003ff0: 6f66 6628 7365 6c66 293a 0a20 2020 2020  off(self):.     
-00004000: 2020 2022 2222 5365 7474 6572 2061 6e64     """Setter and
-00004010: 2067 6574 7465 7220 6f66 2053 6d65 6172   getter of Smear
-00004020: 696e 6720 6375 746f 6666 2077 6964 7468  ing cutoff width
-00004030: 2e0a 0a20 2020 2020 2020 2054 6869 7320  ...        This 
-00004040: 6973 2067 6976 656e 2061 7320 6120 6d75  is given as a mu
-00004050: 6c74 6970 6c65 206f 6620 7468 6520 7374  ltiple of the st
-00004060: 616e 6461 7264 2064 6576 6961 7469 6f6e  andard deviation
-00004070: 2e0a 0a20 2020 2020 2020 2066 6c6f 6174  ...        float
-00004080: 0a20 2020 2020 2020 2020 2020 2046 6f72  .            For
-00004090: 2065 7861 6d70 6c65 2c20 6966 2074 6869   example, if thi
-000040a0: 7320 7661 6c75 6520 6973 2035 2c20 7468  s value is 5, th
-000040b0: 6520 7461 696c 206f 6620 7468 6520 4761  e tail of the Ga
-000040c0: 7573 7369 616e 2066 756e 6374 696f 6e0a  ussian function.
-000040d0: 2020 2020 2020 2020 2020 2020 6973 2063              is c
-000040e0: 7574 2061 7420 3520 7369 676d 612e 0a0a  ut at 5 sigma...
-000040f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00004100: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00004110: 5f73 6967 6d61 5f63 7574 6f66 660a 0a20  _sigma_cutoff.. 
-00004120: 2020 2040 7369 676d 615f 6375 746f 6666     @sigma_cutoff
-00004130: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
-00004140: 7369 676d 615f 6375 746f 6666 2873 656c  sigma_cutoff(sel
-00004150: 662c 2073 6967 6d61 5f63 7574 6f66 6629  f, sigma_cutoff)
-00004160: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-00004170: 7369 676d 615f 6375 746f 6666 203d 2073  sigma_cutoff = s
-00004180: 6967 6d61 5f63 7574 6f66 660a 0a20 2020  igma_cutoff..   
-00004190: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-000041a0: 6566 206e 6163 5f70 6172 616d 7328 7365  ef nac_params(se
-000041b0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-000041c0: 5365 7474 6572 2061 6e64 2067 6574 7465  Setter and gette
-000041d0: 7220 6f66 2070 6172 616d 6574 6572 7320  r of parameters 
-000041e0: 666f 7220 6e6f 6e2d 616e 616c 7974 6963  for non-analytic
-000041f0: 616c 2074 6572 6d20 636f 7272 6563 7469  al term correcti
-00004200: 6f6e 2e0a 0a20 2020 2020 2020 2064 6963  on...        dic
-00004210: 740a 2020 2020 2020 2020 2020 2020 5061  t.            Pa
-00004220: 7261 6d65 7465 7273 2075 7365 6420 666f  rameters used fo
-00004230: 7220 6e6f 6e2d 616e 616c 7974 6963 616c  r non-analytical
-00004240: 2074 6572 6d20 636f 7272 6563 7469 6f6e   term correction
-00004250: 0a20 2020 2020 2020 2020 2020 2027 626f  .            'bo
-00004260: 726e 273a 206e 6461 7272 6179 0a20 2020  rn': ndarray.   
-00004270: 2020 2020 2020 2020 2020 2020 2042 6f72               Bor
-00004280: 6e20 6566 6665 6374 6976 6520 6368 6172  n effective char
-00004290: 6765 730a 2020 2020 2020 2020 2020 2020  ges.            
-000042a0: 2020 2020 7368 6170 653d 2870 7269 6d69      shape=(primi
-000042b0: 7469 7665 2063 656c 6c20 6174 6f6d 732c  tive cell atoms,
-000042c0: 2033 2c20 3329 2c20 6474 7970 653d 2764   3, 3), dtype='d
-000042d0: 6f75 626c 6527 2c20 6f72 6465 723d 2743  ouble', order='C
-000042e0: 270a 2020 2020 2020 2020 2020 2020 2766  '.            'f
-000042f0: 6163 746f 7227 3a20 666c 6f61 740a 2020  actor': float.  
-00004300: 2020 2020 2020 2020 2020 2020 2020 556e                Un
-00004310: 6974 2063 6f6e 7665 7273 696f 6e20 6661  it conversion fa
-00004320: 6374 6f72 0a20 2020 2020 2020 2020 2020  ctor.           
-00004330: 2027 6469 656c 6563 7472 6963 273a 206e   'dielectric': n
-00004340: 6461 7272 6179 0a20 2020 2020 2020 2020  darray.         
-00004350: 2020 2020 2020 2044 6965 6c65 6374 7269         Dielectri
-00004360: 6320 636f 6e73 7461 6e74 2074 656e 736f  c constant tenso
-00004370: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-00004380: 2020 7368 6170 653d 2833 2c20 3329 2c20    shape=(3, 3), 
-00004390: 6474 7970 653d 2764 6f75 626c 6527 2c20  dtype='double', 
-000043a0: 6f72 6465 723d 2743 270a 0a20 2020 2020  order='C'..     
-000043b0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-000043c0: 6574 7572 6e20 7365 6c66 2e5f 6e61 635f  eturn self._nac_
-000043d0: 7061 7261 6d73 0a0a 2020 2020 406e 6163  params..    @nac
-000043e0: 5f70 6172 616d 732e 7365 7474 6572 0a20  _params.setter. 
-000043f0: 2020 2064 6566 206e 6163 5f70 6172 616d     def nac_param
-00004400: 7328 7365 6c66 2c20 6e61 635f 7061 7261  s(self, nac_para
-00004410: 6d73 293a 0a20 2020 2020 2020 2073 656c  ms):.        sel
-00004420: 662e 5f6e 6163 5f70 6172 616d 7320 3d20  f._nac_params = 
-00004430: 6e61 635f 7061 7261 6d73 0a20 2020 2020  nac_params.     
-00004440: 2020 2069 6620 7365 6c66 2e5f 696e 7465     if self._inte
-00004450: 7261 6374 696f 6e20 6973 206e 6f74 204e  raction is not N
-00004460: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00004470: 2073 656c 662e 5f69 6e69 745f 6479 6e61   self._init_dyna
-00004480: 6d69 6361 6c5f 6d61 7472 6978 2829 0a0a  mical_matrix()..
-00004490: 2020 2020 6465 6620 6765 745f 6e61 635f      def get_nac_
-000044a0: 7061 7261 6d73 2873 656c 6629 3a0a 2020  params(self):.  
-000044b0: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
-000044c0: 4e41 4320 7061 7261 6d65 7465 7273 2e22  NAC parameters."
-000044d0: 2222 0a20 2020 2020 2020 2077 6172 6e69  "".        warni
-000044e0: 6e67 732e 7761 726e 280a 2020 2020 2020  ngs.warn(.      
-000044f0: 2020 2020 2020 2250 686f 6e6f 3370 792e        "Phono3py.
-00004500: 6765 745f 6e61 635f 7061 7261 6d73 2829  get_nac_params()
-00004510: 2069 7320 6465 7072 6563 6174 6564 2e22   is deprecated."
-00004520: 0a20 2020 2020 2020 2020 2020 2022 5573  .            "Us
-00004530: 6520 5068 6f6e 6f33 7079 2e6e 6163 5f70  e Phono3py.nac_p
-00004540: 6172 616d 7320 6174 7472 6962 7574 6520  arams attribute 
-00004550: 696e 7374 6561 642e 222c 0a20 2020 2020  instead.",.     
-00004560: 2020 2020 2020 2044 6570 7265 6361 7469         Deprecati
-00004570: 6f6e 5761 726e 696e 672c 0a20 2020 2020  onWarning,.     
-00004580: 2020 2029 0a20 2020 2020 2020 2072 6574     ).        ret
-00004590: 7572 6e20 7365 6c66 2e6e 6163 5f70 6172  urn self.nac_par
-000045a0: 616d 730a 0a20 2020 2064 6566 2073 6574  ams..    def set
-000045b0: 5f6e 6163 5f70 6172 616d 7328 7365 6c66  _nac_params(self
-000045c0: 2c20 6e61 635f 7061 7261 6d73 293a 0a20  , nac_params):. 
-000045d0: 2020 2020 2020 2022 2222 5365 7420 4e41         """Set NA
-000045e0: 4320 7061 7261 6d65 7465 7273 2e22 2222  C parameters."""
-000045f0: 0a20 2020 2020 2020 2077 6172 6e69 6e67  .        warning
-00004600: 732e 7761 726e 280a 2020 2020 2020 2020  s.warn(.        
-00004610: 2020 2020 2250 686f 6e6f 3370 792e 7365      "Phono3py.se
-00004620: 745f 6e61 635f 7061 7261 6d73 2829 2069  t_nac_params() i
-00004630: 7320 6465 7072 6563 6174 6564 2e22 0a20  s deprecated.". 
-00004640: 2020 2020 2020 2020 2020 2022 5573 6520             "Use 
-00004650: 5068 6f6e 6f33 7079 2e6e 6163 5f70 6172  Phono3py.nac_par
-00004660: 616d 7320 6174 7472 6962 7574 6520 696e  ams attribute in
-00004670: 7374 6561 642e 222c 0a20 2020 2020 2020  stead.",.       
-00004680: 2020 2020 2044 6570 7265 6361 7469 6f6e       Deprecation
-00004690: 5761 726e 696e 672c 0a20 2020 2020 2020  Warning,.       
-000046a0: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
-000046b0: 6e61 635f 7061 7261 6d73 203d 206e 6163  nac_params = nac
-000046c0: 5f70 6172 616d 730a 0a20 2020 2040 7072  _params..    @pr
-000046d0: 6f70 6572 7479 0a20 2020 2064 6566 2064  operty.    def d
-000046e0: 796e 616d 6963 616c 5f6d 6174 7269 7828  ynamical_matrix(
-000046f0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00004700: 2222 5265 7475 726e 2044 796e 616d 6963  ""Return Dynamic
-00004710: 616c 4d61 7472 6978 2069 6e73 7461 6e63  alMatrix instanc
-00004720: 652e 0a0a 2020 2020 2020 2020 5468 6973  e...        This
-00004730: 2069 7320 6e6f 7420 6479 6e61 6d69 6361   is not dynamica
-00004740: 6c20 6d61 7472 6963 6573 2062 7574 2074  l matrices but t
-00004750: 6865 2069 6e73 7461 6e63 6520 6f66 2044  he instance of D
-00004760: 796e 616d 6963 616c 4d61 7472 6978 0a20  ynamicalMatrix. 
-00004770: 2020 2020 2020 2063 6c61 7373 2e0a 0a20         class... 
-00004780: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00004790: 2020 2069 6620 7365 6c66 2e5f 696e 7465     if self._inte
-000047a0: 7261 6374 696f 6e20 6973 204e 6f6e 653a  raction is None:
-000047b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000047c0: 7572 6e20 4e6f 6e65 0a20 2020 2020 2020  urn None.       
-000047d0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000047e0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-000047f0: 696e 7465 7261 6374 696f 6e2e 6479 6e61  interaction.dyna
-00004800: 6d69 6361 6c5f 6d61 7472 6978 0a0a 2020  mical_matrix..  
-00004810: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00004820: 6465 6620 7072 696d 6974 6976 6528 7365  def primitive(se
-00004830: 6c66 2920 2d3e 2050 7269 6d69 7469 7665  lf) -> Primitive
-00004840: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
-00004850: 7572 6e20 7072 696d 6974 6976 6520 6365  urn primitive ce
-00004860: 6c6c 2e0a 0a20 2020 2020 2020 2050 7269  ll...        Pri
-00004870: 6d69 7469 7665 0a20 2020 2020 2020 2020  mitive.         
-00004880: 2020 2050 7269 6d69 7469 7665 2063 656c     Primitive cel
-00004890: 6c2e 0a0a 2020 2020 2020 2020 2222 220a  l...        """.
-000048a0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000048b0: 656c 662e 5f70 7269 6d69 7469 7665 0a0a  elf._primitive..
-000048c0: 2020 2020 6465 6620 6765 745f 7072 696d      def get_prim
-000048d0: 6974 6976 6528 7365 6c66 293a 0a20 2020  itive(self):.   
-000048e0: 2020 2020 2022 2222 5265 7475 726e 2070       """Return p
-000048f0: 7269 6d69 7469 7665 2063 656c 6c2e 2222  rimitive cell.""
-00004900: 220a 2020 2020 2020 2020 7761 726e 696e  ".        warnin
-00004910: 6773 2e77 6172 6e28 0a20 2020 2020 2020  gs.warn(.       
-00004920: 2020 2020 2022 5068 6f6e 6f33 7079 2e67       "Phono3py.g
-00004930: 6574 5f70 7269 6d69 7469 7665 2829 2069  et_primitive() i
-00004940: 7320 6465 7072 6563 6174 6564 2e22 0a20  s deprecated.". 
-00004950: 2020 2020 2020 2020 2020 2022 5573 6520             "Use 
-00004960: 5068 6f6e 6f33 7079 2e70 7269 6d69 7469  Phono3py.primiti
-00004970: 7665 2061 7474 7269 6275 7465 2069 6e73  ve attribute ins
-00004980: 7465 6164 2e22 2c0a 2020 2020 2020 2020  tead.",.        
-00004990: 2020 2020 4465 7072 6563 6174 696f 6e57      DeprecationW
-000049a0: 6172 6e69 6e67 2c0a 2020 2020 2020 2020  arning,.        
-000049b0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000049c0: 2073 656c 662e 7072 696d 6974 6976 650a   self.primitive.
-000049d0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-000049e0: 2020 2064 6566 2075 6e69 7463 656c 6c28     def unitcell(
-000049f0: 7365 6c66 2920 2d3e 2050 686f 6e6f 7079  self) -> Phonopy
-00004a00: 4174 6f6d 733a 0a20 2020 2020 2020 2022  Atoms:.        "
-00004a10: 2222 5265 7475 726e 2055 6e69 7420 6365  ""Return Unit ce
-00004a20: 6c6c 2e0a 0a20 2020 2020 2020 2050 686f  ll...        Pho
-00004a30: 6e6f 7079 4174 6f6d 730a 2020 2020 2020  nopyAtoms.      
-00004a40: 2020 2020 2020 556e 6974 2063 656c 6c2e        Unit cell.
-00004a50: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00004a60: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00004a70: 662e 5f75 6e69 7463 656c 6c0a 0a20 2020  f._unitcell..   
-00004a80: 2064 6566 2067 6574 5f75 6e69 7463 656c   def get_unitcel
-00004a90: 6c28 7365 6c66 293a 0a20 2020 2020 2020  l(self):.       
-00004aa0: 2022 2222 5265 7475 726e 2055 6e69 7420   """Return Unit 
-00004ab0: 6365 6c6c 2e22 2222 0a20 2020 2020 2020  cell.""".       
-00004ac0: 2077 6172 6e69 6e67 732e 7761 726e 280a   warnings.warn(.
-00004ad0: 2020 2020 2020 2020 2020 2020 2250 686f              "Pho
-00004ae0: 6e6f 3370 792e 6765 745f 756e 6974 6365  no3py.get_unitce
-00004af0: 6c6c 2829 2069 7320 6465 7072 6563 6174  ll() is deprecat
-00004b00: 6564 2e22 0a20 2020 2020 2020 2020 2020  ed.".           
-00004b10: 2022 5573 6520 5068 6f6e 6f33 7079 2e75   "Use Phono3py.u
-00004b20: 6e69 7463 656c 6c20 6174 7472 6962 7574  nitcell attribut
-00004b30: 6520 696e 7374 6561 642e 222c 0a20 2020  e instead.",.   
-00004b40: 2020 2020 2020 2020 2044 6570 7265 6361           Depreca
-00004b50: 7469 6f6e 5761 726e 696e 672c 0a20 2020  tionWarning,.   
-00004b60: 2020 2020 2029 0a20 2020 2020 2020 2072       ).        r
-00004b70: 6574 7572 6e20 7365 6c66 2e75 6e69 7463  eturn self.unitc
-00004b80: 656c 6c0a 0a20 2020 2040 7072 6f70 6572  ell..    @proper
-00004b90: 7479 0a20 2020 2064 6566 2073 7570 6572  ty.    def super
-00004ba0: 6365 6c6c 2873 656c 6629 202d 3e20 5375  cell(self) -> Su
-00004bb0: 7065 7263 656c 6c3a 0a20 2020 2020 2020  percell:.       
-00004bc0: 2022 2222 5265 7475 726e 2073 7570 6572   """Return super
-00004bd0: 6365 6c6c 2e0a 0a20 2020 2020 2020 2053  cell...        S
-00004be0: 7570 6572 6365 6c6c 0a20 2020 2020 2020  upercell.       
-00004bf0: 2020 2020 2053 7570 6572 6365 6c6c 2e0a       Supercell..
-00004c00: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00004c10: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00004c20: 2e5f 7375 7065 7263 656c 6c0a 0a20 2020  ._supercell..   
-00004c30: 2064 6566 2067 6574 5f73 7570 6572 6365   def get_superce
-00004c40: 6c6c 2873 656c 6629 3a0a 2020 2020 2020  ll(self):.      
-00004c50: 2020 2222 2252 6574 7572 6e20 7375 7065    """Return supe
-00004c60: 7263 656c 6c2e 2222 220a 2020 2020 2020  rcell.""".      
-00004c70: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
-00004c80: 0a20 2020 2020 2020 2020 2020 2022 5068  .            "Ph
-00004c90: 6f6e 6f33 7079 2e67 6574 5f73 7570 6572  ono3py.get_super
-00004ca0: 6365 6c6c 2829 2069 7320 6465 7072 6563  cell() is deprec
-00004cb0: 6174 6564 2e22 0a20 2020 2020 2020 2020  ated.".         
-00004cc0: 2020 2022 5573 6520 5068 6f6e 6f33 7079     "Use Phono3py
-00004cd0: 2e73 7570 6572 6365 6c6c 2061 7474 7269  .supercell attri
-00004ce0: 6275 7465 2069 6e73 7465 6164 2e22 2c0a  bute instead.",.
-00004cf0: 2020 2020 2020 2020 2020 2020 4465 7072              Depr
-00004d00: 6563 6174 696f 6e57 6172 6e69 6e67 2c0a  ecationWarning,.
-00004d10: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00004d20: 2020 7265 7475 726e 2073 656c 662e 7375    return self.su
-00004d30: 7065 7263 656c 6c0a 0a20 2020 2040 7072  percell..    @pr
-00004d40: 6f70 6572 7479 0a20 2020 2064 6566 2070  operty.    def p
-00004d50: 686f 6e6f 6e5f 7375 7065 7263 656c 6c28  honon_supercell(
-00004d60: 7365 6c66 2920 2d3e 2053 7570 6572 6365  self) -> Superce
-00004d70: 6c6c 3a0a 2020 2020 2020 2020 2222 2252  ll:.        """R
-00004d80: 6574 7572 6e20 7375 7065 7263 656c 6c20  eturn supercell 
-00004d90: 666f 7220 6663 322e 0a0a 2020 2020 2020  for fc2...      
-00004da0: 2020 5375 7065 7263 656c 6c0a 2020 2020    Supercell.    
-00004db0: 2020 2020 2020 2020 5375 7065 7263 656c          Supercel
-00004dc0: 6c20 666f 7220 6663 322e 0a0a 2020 2020  l for fc2...    
-00004dd0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00004de0: 7265 7475 726e 2073 656c 662e 5f70 686f  return self._pho
-00004df0: 6e6f 6e5f 7375 7065 7263 656c 6c0a 0a20  non_supercell.. 
-00004e00: 2020 2064 6566 2067 6574 5f70 686f 6e6f     def get_phono
-00004e10: 6e5f 7375 7065 7263 656c 6c28 7365 6c66  n_supercell(self
-00004e20: 293a 0a20 2020 2020 2020 2022 2222 5265  ):.        """Re
-00004e30: 7475 726e 2073 7570 6572 6365 6c6c 2066  turn supercell f
-00004e40: 6f72 2066 6332 2e22 2222 0a20 2020 2020  or fc2.""".     
-00004e50: 2020 2077 6172 6e69 6e67 732e 7761 726e     warnings.warn
-00004e60: 280a 2020 2020 2020 2020 2020 2020 2250  (.            "P
-00004e70: 686f 6e6f 3370 792e 6765 745f 7068 6f6e  hono3py.get_phon
-00004e80: 6f6e 5f73 7570 6572 6365 6c6c 2829 2069  on_supercell() i
-00004e90: 7320 6465 7072 6563 6174 6564 2e22 0a20  s deprecated.". 
-00004ea0: 2020 2020 2020 2020 2020 2022 5573 6520             "Use 
-00004eb0: 5068 6f6e 6f33 7079 2e70 686f 6e6f 6e5f  Phono3py.phonon_
-00004ec0: 7375 7065 7263 656c 6c20 6174 7472 6962  supercell attrib
-00004ed0: 7574 6520 696e 7374 6561 642e 222c 0a20  ute instead.",. 
-00004ee0: 2020 2020 2020 2020 2020 2044 6570 7265             Depre
-00004ef0: 6361 7469 6f6e 5761 726e 696e 672c 0a20  cationWarning,. 
-00004f00: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00004f10: 2072 6574 7572 6e20 7365 6c66 2e70 686f   return self.pho
-00004f20: 6e6f 6e5f 7375 7065 7263 656c 6c0a 0a20  non_supercell.. 
-00004f30: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00004f40: 2064 6566 2070 686f 6e6f 6e5f 7072 696d   def phonon_prim
-00004f50: 6974 6976 6528 7365 6c66 2920 2d3e 2050  itive(self) -> P
-00004f60: 7269 6d69 7469 7665 3a0a 2020 2020 2020  rimitive:.      
-00004f70: 2020 2222 2252 6574 7572 6e20 7072 696d    """Return prim
-00004f80: 6974 6976 6520 6365 6c6c 2066 6f72 2066  itive cell for f
-00004f90: 6332 2e0a 0a20 2020 2020 2020 2050 7269  c2...        Pri
-00004fa0: 6d69 7469 7665 0a20 2020 2020 2020 2020  mitive.         
-00004fb0: 2020 2050 7269 6d69 7469 7665 2063 656c     Primitive cel
-00004fc0: 6c20 666f 7220 6663 322e 2054 6869 7320  l for fc2. This 
-00004fd0: 7368 6f75 6c64 2062 6520 7468 6520 7361  should be the sa
-00004fe0: 6d65 2061 7320 7468 6520 7072 696d 6974  me as the primit
-00004ff0: 6976 650a 2020 2020 2020 2020 2020 2020  ive.            
-00005000: 6365 6c6c 2066 6f72 2066 6333 2c20 6275  cell for fc3, bu
-00005010: 7420 7468 6973 2069 7320 6372 6561 7465  t this is create
-00005020: 6420 6672 6f6d 2073 7570 6572 6365 6c6c  d from supercell
-00005030: 2066 6f72 2066 6332 2061 6e64 0a20 2020   for fc2 and.   
-00005040: 2020 2020 2020 2020 2063 616e 2062 6520           can be 
-00005050: 6e6f 7420 6e75 6d65 7269 6361 6c6c 7920  not numerically 
-00005060: 7065 7266 6563 746c 7920 6964 656e 7469  perfectly identi
-00005070: 6361 6c2e 0a0a 2020 2020 2020 2020 2222  cal...        ""
-00005080: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-00005090: 2073 656c 662e 5f70 686f 6e6f 6e5f 7072   self._phonon_pr
-000050a0: 696d 6974 6976 650a 0a20 2020 2064 6566  imitive..    def
-000050b0: 2067 6574 5f70 686f 6e6f 6e5f 7072 696d   get_phonon_prim
-000050c0: 6974 6976 6528 7365 6c66 293a 0a20 2020  itive(self):.   
-000050d0: 2020 2020 2022 2222 5265 7475 726e 2070       """Return p
-000050e0: 7269 6d69 7469 7665 2063 656c 6c20 666f  rimitive cell fo
-000050f0: 7220 6663 322e 2222 220a 2020 2020 2020  r fc2.""".      
-00005100: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
-00005110: 0a20 2020 2020 2020 2020 2020 2022 5068  .            "Ph
-00005120: 6f6e 6f33 7079 2e67 6574 5f70 686f 6e6f  ono3py.get_phono
-00005130: 6e5f 7072 696d 6974 6976 6528 2920 6973  n_primitive() is
-00005140: 2064 6570 7265 6361 7465 642e 220a 2020   deprecated.".  
-00005150: 2020 2020 2020 2020 2020 2255 7365 2050            "Use P
-00005160: 686f 6e6f 3370 792e 7068 6f6e 6f6e 5f70  hono3py.phonon_p
-00005170: 7269 6d69 7469 7665 2061 7474 7269 6275  rimitive attribu
-00005180: 7465 2069 6e73 7465 6164 2e22 2c0a 2020  te instead.",.  
-00005190: 2020 2020 2020 2020 2020 4465 7072 6563            Deprec
-000051a0: 6174 696f 6e57 6172 6e69 6e67 2c0a 2020  ationWarning,.  
-000051b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000051c0: 7265 7475 726e 2073 656c 662e 7068 6f6e  return self.phon
-000051d0: 6f6e 5f70 7269 6d69 7469 7665 0a0a 2020  on_primitive..  
-000051e0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-000051f0: 6465 6620 7379 6d6d 6574 7279 2873 656c  def symmetry(sel
-00005200: 6629 202d 3e20 5379 6d6d 6574 7279 3a0a  f) -> Symmetry:.
-00005210: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
-00005220: 6e20 7379 6d6d 6574 7279 206f 6620 7375  n symmetry of su
-00005230: 7065 7263 656c 6c2e 0a0a 2020 2020 2020  percell...      
-00005240: 2020 5379 6d6d 6574 7279 0a20 2020 2020    Symmetry.     
-00005250: 2020 2020 2020 2053 796d 6d65 7472 7920         Symmetry 
-00005260: 6f66 2073 7570 6572 6365 6c6c 0a0a 2020  of supercell..  
-00005270: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00005280: 2020 7265 7475 726e 2073 656c 662e 5f73    return self._s
-00005290: 796d 6d65 7472 790a 0a20 2020 2064 6566  ymmetry..    def
-000052a0: 2067 6574 5f73 796d 6d65 7472 7928 7365   get_symmetry(se
-000052b0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-000052c0: 5265 7475 726e 2073 796d 6d65 7472 7920  Return symmetry 
-000052d0: 6f66 2073 7570 6572 6365 6c6c 2e22 2222  of supercell."""
-000052e0: 0a20 2020 2020 2020 2077 6172 6e69 6e67  .        warning
-000052f0: 732e 7761 726e 280a 2020 2020 2020 2020  s.warn(.        
-00005300: 2020 2020 2250 686f 6e6f 3370 792e 6765      "Phono3py.ge
-00005310: 745f 7379 6d6d 6574 7279 2829 2069 7320  t_symmetry() is 
-00005320: 6465 7072 6563 6174 6564 2e22 0a20 2020  deprecated.".   
-00005330: 2020 2020 2020 2020 2022 5573 6520 5068           "Use Ph
-00005340: 6f6e 6f33 7079 2e73 796d 6d65 7472 7920  ono3py.symmetry 
-00005350: 6174 7472 6962 7574 6520 696e 7374 6561  attribute instea
-00005360: 642e 222c 0a20 2020 2020 2020 2020 2020  d.",.           
-00005370: 2044 6570 7265 6361 7469 6f6e 5761 726e   DeprecationWarn
-00005380: 696e 672c 0a20 2020 2020 2020 2029 0a20  ing,.        ). 
-00005390: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000053a0: 6c66 2e73 796d 6d65 7472 790a 0a20 2020  lf.symmetry..   
-000053b0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-000053c0: 6566 2070 7269 6d69 7469 7665 5f73 796d  ef primitive_sym
-000053d0: 6d65 7472 7928 7365 6c66 2920 2d3e 2053  metry(self) -> S
-000053e0: 796d 6d65 7472 793a 0a20 2020 2020 2020  ymmetry:.       
-000053f0: 2022 2222 5265 7475 726e 2073 796d 6d65   """Return symme
-00005400: 7472 7920 6f66 2070 7269 6d69 7469 7665  try of primitive
-00005410: 2063 656c 6c2e 0a0a 2020 2020 2020 2020   cell...        
-00005420: 5379 6d6d 6574 7279 0a20 2020 2020 2020  Symmetry.       
-00005430: 2020 2020 2053 796d 6d65 7472 7920 6f66       Symmetry of
-00005440: 2070 7269 6d69 7469 7665 2063 656c 6c2e   primitive cell.
-00005450: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00005460: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00005470: 662e 5f70 7269 6d69 7469 7665 5f73 796d  f._primitive_sym
-00005480: 6d65 7472 790a 0a20 2020 2064 6566 2067  metry..    def g
-00005490: 6574 5f70 7269 6d69 7469 7665 5f73 796d  et_primitive_sym
-000054a0: 6d65 7472 7928 7365 6c66 293a 0a20 2020  metry(self):.   
-000054b0: 2020 2020 2022 2222 5265 7475 726e 2073       """Return s
-000054c0: 796d 6d65 7472 7920 6f66 2070 7269 6d69  ymmetry of primi
-000054d0: 7469 7665 2063 656c 6c2e 2222 220a 2020  tive cell.""".  
-000054e0: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
-000054f0: 6172 6e28 0a20 2020 2020 2020 2020 2020  arn(.           
-00005500: 2022 5068 6f6e 6f33 7079 2e67 6574 5f70   "Phono3py.get_p
-00005510: 7269 6d69 7469 7665 5f73 796d 6d65 7472  rimitive_symmetr
-00005520: 7928 2920 6973 2064 6570 7265 6361 7465  y() is deprecate
-00005530: 642e 220a 2020 2020 2020 2020 2020 2020  d.".            
-00005540: 2255 7365 2050 686f 6e6f 3370 792e 7072  "Use Phono3py.pr
-00005550: 696d 6974 6976 655f 7379 6d6d 6574 7279  imitive_symmetry
-00005560: 2061 7474 7269 6275 7465 2069 6e73 7465   attribute inste
-00005570: 6164 2e22 2c0a 2020 2020 2020 2020 2020  ad.",.          
-00005580: 2020 4465 7072 6563 6174 696f 6e57 6172    DeprecationWar
-00005590: 6e69 6e67 2c0a 2020 2020 2020 2020 290a  ning,.        ).
-000055a0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000055b0: 656c 662e 7072 696d 6974 6976 655f 7379  elf.primitive_sy
-000055c0: 6d6d 6574 7279 0a0a 2020 2020 4070 726f  mmetry..    @pro
-000055d0: 7065 7274 790a 2020 2020 6465 6620 7068  perty.    def ph
-000055e0: 6f6e 6f6e 5f73 7570 6572 6365 6c6c 5f73  onon_supercell_s
-000055f0: 796d 6d65 7472 7928 7365 6c66 2920 2d3e  ymmetry(self) ->
-00005600: 2053 796d 6d65 7472 793a 0a20 2020 2020   Symmetry:.     
-00005610: 2020 2022 2222 5265 7475 726e 2073 796d     """Return sym
-00005620: 6d65 7472 7920 6f66 2073 7570 6572 6365  metry of superce
-00005630: 6c6c 2066 6f72 2066 6332 2e0a 0a20 2020  ll for fc2...   
-00005640: 2020 2020 2053 796d 6d65 7472 790a 2020       Symmetry.  
-00005650: 2020 2020 2020 2020 2020 5379 6d6d 6574            Symmet
-00005660: 7279 206f 6620 7375 7065 7263 656c 6c20  ry of supercell 
-00005670: 666f 7220 6663 3220 2870 686f 6e6f 6e5f  for fc2 (phonon_
-00005680: 7375 7065 7263 656c 6c29 2e0a 0a20 2020  supercell)...   
-00005690: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000056a0: 2072 6574 7572 6e20 7365 6c66 2e5f 7068   return self._ph
-000056b0: 6f6e 6f6e 5f73 7570 6572 6365 6c6c 5f73  onon_supercell_s
-000056c0: 796d 6d65 7472 790a 0a20 2020 2064 6566  ymmetry..    def
-000056d0: 2067 6574 5f70 686f 6e6f 6e5f 7375 7065   get_phonon_supe
-000056e0: 7263 656c 6c5f 7379 6d6d 6574 7279 2873  rcell_symmetry(s
-000056f0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00005700: 2252 6574 7572 6e20 7379 6d6d 6574 7279  "Return symmetry
-00005710: 206f 6620 7375 7065 7263 656c 6c20 666f   of supercell fo
-00005720: 7220 6663 322e 2222 220a 2020 2020 2020  r fc2.""".      
-00005730: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
-00005740: 0a20 2020 2020 2020 2020 2020 2022 5068  .            "Ph
-00005750: 6f6e 6f33 7079 2e67 6574 5f70 686f 6e6f  ono3py.get_phono
-00005760: 6e5f 7375 7065 7263 656c 6c5f 7379 6d6d  n_supercell_symm
-00005770: 6574 7279 2829 2069 7320 6465 7072 6563  etry() is deprec
-00005780: 6174 6564 2e22 0a20 2020 2020 2020 2020  ated.".         
-00005790: 2020 2022 5573 6520 5068 6f6e 6f33 7079     "Use Phono3py
-000057a0: 2e70 686f 6e6f 6e5f 7375 7065 7263 656c  .phonon_supercel
-000057b0: 6c5f 7379 6d6d 6574 7279 2061 7474 7269  l_symmetry attri
-000057c0: 6275 7465 2069 6e73 7465 6164 2e22 2c0a  bute instead.",.
-000057d0: 2020 2020 2020 2020 2020 2020 4465 7072              Depr
-000057e0: 6563 6174 696f 6e57 6172 6e69 6e67 2c0a  ecationWarning,.
-000057f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00005800: 2020 7265 7475 726e 2073 656c 662e 7068    return self.ph
-00005810: 6f6e 6f6e 5f73 7570 6572 6365 6c6c 5f73  onon_supercell_s
-00005820: 796d 6d65 7472 790a 0a20 2020 2040 7072  ymmetry..    @pr
-00005830: 6f70 6572 7479 0a20 2020 2064 6566 2073  operty.    def s
-00005840: 7570 6572 6365 6c6c 5f6d 6174 7269 7828  upercell_matrix(
-00005850: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00005860: 2222 5265 7475 726e 2074 7261 6e73 666f  ""Return transfo
-00005870: 726d 6174 696f 6e20 6d61 7472 6978 2074  rmation matrix t
-00005880: 6f20 7375 7065 7263 656c 6c20 6365 6c6c  o supercell cell
-00005890: 2066 726f 6d20 756e 6974 2063 656c 6c2e   from unit cell.
-000058a0: 0a0a 2020 2020 2020 2020 6e64 6172 7261  ..        ndarra
-000058b0: 790a 2020 2020 2020 2020 2020 2020 5375  y.            Su
-000058c0: 7065 7263 656c 6c20 6d61 7472 6978 2077  percell matrix w
-000058d0: 6974 6820 7265 7370 6563 7420 746f 2075  ith respect to u
-000058e0: 6e69 7420 6365 6c6c 2e0a 2020 2020 2020  nit cell..      
-000058f0: 2020 2020 2020 7368 6170 653d 2833 2c20        shape=(3, 
-00005900: 3329 2c20 6474 7970 653d 2769 6e74 5f27  3), dtype='int_'
-00005910: 2c20 6f72 6465 723d 2743 270a 0a20 2020  , order='C'..   
-00005920: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00005930: 2072 6574 7572 6e20 7365 6c66 2e5f 7375   return self._su
-00005940: 7065 7263 656c 6c5f 6d61 7472 6978 0a0a  percell_matrix..
-00005950: 2020 2020 6465 6620 6765 745f 7375 7065      def get_supe
-00005960: 7263 656c 6c5f 6d61 7472 6978 2873 656c  rcell_matrix(sel
-00005970: 6629 3a0a 2020 2020 2020 2020 2222 2252  f):.        """R
-00005980: 6574 7572 6e20 7472 616e 7366 6f72 6d61  eturn transforma
-00005990: 7469 6f6e 206d 6174 7269 7820 746f 2073  tion matrix to s
-000059a0: 7570 6572 6365 6c6c 2063 656c 6c20 6672  upercell cell fr
-000059b0: 6f6d 2075 6e69 7420 6365 6c6c 2e22 2222  om unit cell."""
-000059c0: 0a20 2020 2020 2020 2077 6172 6e69 6e67  .        warning
-000059d0: 732e 7761 726e 280a 2020 2020 2020 2020  s.warn(.        
-000059e0: 2020 2020 2250 686f 6e6f 3370 792e 6765      "Phono3py.ge
-000059f0: 745f 7375 7065 7263 656c 6c5f 6d61 7472  t_supercell_matr
-00005a00: 6978 2829 2069 7320 6465 7072 6563 6174  ix() is deprecat
-00005a10: 6564 2e22 0a20 2020 2020 2020 2020 2020  ed.".           
-00005a20: 2022 5573 6520 5068 6f6e 6f33 7079 2e73   "Use Phono3py.s
-00005a30: 7570 6572 6365 6c6c 5f6d 6174 7269 7820  upercell_matrix 
-00005a40: 6174 7472 6962 7574 6520 696e 7374 6561  attribute instea
-00005a50: 642e 222c 0a20 2020 2020 2020 2020 2020  d.",.           
-00005a60: 2044 6570 7265 6361 7469 6f6e 5761 726e   DeprecationWarn
-00005a70: 696e 672c 0a20 2020 2020 2020 2029 0a20  ing,.        ). 
-00005a80: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00005a90: 6c66 2e73 7570 6572 6365 6c6c 5f6d 6174  lf.supercell_mat
-00005aa0: 7269 780a 0a20 2020 2040 7072 6f70 6572  rix..    @proper
-00005ab0: 7479 0a20 2020 2064 6566 2070 686f 6e6f  ty.    def phono
-00005ac0: 6e5f 7375 7065 7263 656c 6c5f 6d61 7472  n_supercell_matr
-00005ad0: 6978 2873 656c 6629 3a0a 2020 2020 2020  ix(self):.      
-00005ae0: 2020 2222 2252 6574 7572 6e20 7472 616e    """Return tran
-00005af0: 7366 6f72 6d61 7469 6f6e 206d 6174 7269  sformation matri
-00005b00: 7820 746f 2070 686f 6e6f 6e20 7375 7065  x to phonon supe
-00005b10: 7263 656c 6c20 6672 6f6d 2075 6e69 7420  rcell from unit 
-00005b20: 6365 6c6c 2e0a 0a20 2020 2020 2020 206e  cell...        n
-00005b30: 6461 7272 6179 0a20 2020 2020 2020 2020  darray.         
-00005b40: 2020 2053 7570 6572 6365 6c6c 206d 6174     Supercell mat
-00005b50: 7269 7820 7769 7468 2072 6573 7065 6374  rix with respect
-00005b60: 2074 6f20 756e 6974 2063 656c 6c2e 0a20   to unit cell.. 
-00005b70: 2020 2020 2020 2020 2020 2073 6861 7065             shape
-00005b80: 3d28 332c 2033 292c 2064 7479 7065 3d27  =(3, 3), dtype='
-00005b90: 696e 745f 272c 206f 7264 6572 3d27 4327  int_', order='C'
-00005ba0: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00005bb0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00005bc0: 662e 5f70 686f 6e6f 6e5f 7375 7065 7263  f._phonon_superc
-00005bd0: 656c 6c5f 6d61 7472 6978 0a0a 2020 2020  ell_matrix..    
-00005be0: 6465 6620 6765 745f 7068 6f6e 6f6e 5f73  def get_phonon_s
-00005bf0: 7570 6572 6365 6c6c 5f6d 6174 7269 7828  upercell_matrix(
-00005c00: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00005c10: 2222 5265 7475 726e 2074 7261 6e73 666f  ""Return transfo
-00005c20: 726d 6174 696f 6e20 6d61 7472 6978 2074  rmation matrix t
-00005c30: 6f20 7068 6f6e 6f6e 2073 7570 6572 6365  o phonon superce
-00005c40: 6c6c 2066 726f 6d20 756e 6974 2063 656c  ll from unit cel
-00005c50: 6c2e 2222 220a 2020 2020 2020 2020 7761  l.""".        wa
-00005c60: 726e 696e 6773 2e77 6172 6e28 0a20 2020  rnings.warn(.   
-00005c70: 2020 2020 2020 2020 2022 5068 6f6e 6f33           "Phono3
-00005c80: 7079 2e67 6574 5f70 686f 6e6f 6e5f 7375  py.get_phonon_su
-00005c90: 7065 7263 656c 6c5f 6d61 7472 6978 2829  percell_matrix()
-00005ca0: 2069 7320 6465 7072 6563 6174 6564 2e22   is deprecated."
-00005cb0: 0a20 2020 2020 2020 2020 2020 2022 5573  .            "Us
-00005cc0: 6520 5068 6f6e 6f33 7079 2e70 686f 6e6f  e Phono3py.phono
-00005cd0: 6e5f 7375 7065 7263 656c 6c5f 6d61 7472  n_supercell_matr
-00005ce0: 6978 2061 7474 7269 6275 7465 2069 6e73  ix attribute ins
-00005cf0: 7465 6164 2e22 2c0a 2020 2020 2020 2020  tead.",.        
-00005d00: 2020 2020 4465 7072 6563 6174 696f 6e57      DeprecationW
-00005d10: 6172 6e69 6e67 2c0a 2020 2020 2020 2020  arning,.        
-00005d20: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00005d30: 2073 656c 662e 7068 6f6e 6f6e 5f73 7570   self.phonon_sup
-00005d40: 6572 6365 6c6c 5f6d 6174 7269 780a 0a20  ercell_matrix.. 
-00005d50: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00005d60: 2064 6566 2070 7269 6d69 7469 7665 5f6d   def primitive_m
-00005d70: 6174 7269 7828 7365 6c66 293a 0a20 2020  atrix(self):.   
-00005d80: 2020 2020 2022 2222 5265 7475 726e 2074       """Return t
-00005d90: 7261 6e73 666f 726d 6174 696f 6e20 6d61  ransformation ma
-00005da0: 7472 6978 2074 6f20 7072 696d 6974 6976  trix to primitiv
-00005db0: 6520 6365 6c6c 2066 726f 6d20 756e 6974  e cell from unit
-00005dc0: 2063 656c 6c2e 0a0a 2020 2020 2020 2020   cell...        
-00005dd0: 6e64 6172 7261 790a 2020 2020 2020 2020  ndarray.        
-00005de0: 2020 2020 5072 696d 6974 6976 6520 6d61      Primitive ma
-00005df0: 7472 6978 2077 6974 6820 7265 7370 6563  trix with respec
-00005e00: 7420 746f 2075 6e69 7420 6365 6c6c 2e0a  t to unit cell..
-00005e10: 2020 2020 2020 2020 2020 2020 7368 6170              shap
-00005e20: 653d 2833 2c20 3329 2c20 6474 7970 653d  e=(3, 3), dtype=
-00005e30: 2764 6f75 626c 6527 2c20 6f72 6465 723d  'double', order=
-00005e40: 2743 270a 0a20 2020 2020 2020 2022 2222  'C'..        """
-00005e50: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00005e60: 7365 6c66 2e5f 7072 696d 6974 6976 655f  self._primitive_
-00005e70: 6d61 7472 6978 0a0a 2020 2020 6465 6620  matrix..    def 
-00005e80: 6765 745f 7072 696d 6974 6976 655f 6d61  get_primitive_ma
-00005e90: 7472 6978 2873 656c 6629 3a0a 2020 2020  trix(self):.    
-00005ea0: 2020 2020 2222 2252 6574 7572 6e20 7472      """Return tr
-00005eb0: 616e 7366 6f72 6d61 7469 6f6e 206d 6174  ansformation mat
-00005ec0: 7269 7820 746f 2070 7269 6d69 7469 7665  rix to primitive
-00005ed0: 2063 656c 6c20 6672 6f6d 2075 6e69 7420   cell from unit 
-00005ee0: 6365 6c6c 2e22 2222 0a20 2020 2020 2020  cell.""".       
-00005ef0: 2077 6172 6e69 6e67 732e 7761 726e 280a   warnings.warn(.
-00005f00: 2020 2020 2020 2020 2020 2020 2250 686f              "Pho
-00005f10: 6e6f 3370 792e 6765 745f 7072 696d 6974  no3py.get_primit
-00005f20: 6976 655f 6d61 7472 6978 2829 2069 7320  ive_matrix() is 
-00005f30: 6465 7072 6563 6174 6564 2e22 0a20 2020  deprecated.".   
-00005f40: 2020 2020 2020 2020 2022 5573 6520 5068           "Use Ph
-00005f50: 6f6e 6f33 7079 2e70 7269 6d69 7469 7665  ono3py.primitive
-00005f60: 5f6d 6174 7269 7820 6174 7472 6962 7574  _matrix attribut
-00005f70: 6520 696e 7374 6561 642e 222c 0a20 2020  e instead.",.   
-00005f80: 2020 2020 2020 2020 2044 6570 7265 6361           Depreca
-00005f90: 7469 6f6e 5761 726e 696e 672c 0a20 2020  tionWarning,.   
-00005fa0: 2020 2020 2029 0a20 2020 2020 2020 2072       ).        r
-00005fb0: 6574 7572 6e20 7365 6c66 2e70 7269 6d69  eturn self.primi
-00005fc0: 7469 7665 5f6d 6174 7269 780a 0a20 2020  tive_matrix..   
-00005fd0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00005fe0: 6566 2075 6e69 745f 636f 6e76 6572 7369  ef unit_conversi
-00005ff0: 6f6e 5f66 6163 746f 7228 7365 6c66 293a  on_factor(self):
-00006000: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-00006010: 726e 2070 686f 6e6f 6e20 6672 6571 7565  rn phonon freque
-00006020: 6e63 7920 756e 6974 2063 6f6e 7665 7273  ncy unit convers
-00006030: 696f 6e20 6661 6374 6f72 2e0a 0a20 2020  ion factor...   
-00006040: 2020 2020 2066 6c6f 6174 0a20 2020 2020       float.     
-00006050: 2020 2020 2020 2050 686f 6e6f 6e20 6672         Phonon fr
-00006060: 6571 7565 6e63 7920 756e 6974 2063 6f6e  equency unit con
-00006070: 7665 7273 696f 6e20 6661 6374 6f72 2e20  version factor. 
-00006080: 5468 6973 2066 6163 746f 720a 2020 2020  This factor.    
-00006090: 2020 2020 2020 2020 636f 6e76 6572 7473          converts
-000060a0: 2073 7172 7428 3c66 6f72 6365 3e2f 3c64   sqrt(<force>/<d
-000060b0: 6973 7461 6e63 653e 2f3c 414d 553e 292f  istance>/<AMU>)/
-000060c0: 3270 692f 3165 3132 2074 6f20 5448 7a0a  2pi/1e12 to THz.
-000060d0: 2020 2020 2020 2020 2020 2020 286f 7264              (ord
-000060e0: 696e 6172 7920 6672 6571 7565 6e63 7929  inary frequency)
-000060f0: 2e0a 0a20 2020 2020 2020 2022 2222 0a20  ...        """. 
-00006100: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00006110: 6c66 2e5f 6672 6571 7565 6e63 795f 6661  lf._frequency_fa
-00006120: 6374 6f72 5f74 6f5f 5448 7a0a 0a20 2020  ctor_to_THz..   
-00006130: 2064 6566 2073 6574 5f64 6973 706c 6163   def set_displac
-00006140: 656d 656e 745f 6461 7461 7365 7428 7365  ement_dataset(se
-00006150: 6c66 2c20 6461 7461 7365 7429 3a0a 2020  lf, dataset):.  
-00006160: 2020 2020 2020 2222 2253 6574 2064 6973        """Set dis
-00006170: 706c 6163 656d 656e 742d 666f 7263 6520  placement-force 
-00006180: 6461 7461 7365 742e 2222 220a 2020 2020  dataset.""".    
-00006190: 2020 2020 7761 726e 696e 6773 2e77 6172      warnings.war
-000061a0: 6e28 0a20 2020 2020 2020 2020 2020 2022  n(.            "
-000061b0: 5068 6f6e 6f33 7079 2e73 6574 5f64 6973  Phono3py.set_dis
-000061c0: 706c 6163 656d 656e 745f 6461 7461 7365  placement_datase
-000061d0: 7428 2920 6973 2064 6570 7265 6361 7465  t() is deprecate
-000061e0: 642e 220a 2020 2020 2020 2020 2020 2020  d.".            
-000061f0: 2255 7365 2050 686f 6e6f 3370 792e 6461  "Use Phono3py.da
-00006200: 7461 7365 7420 6174 7472 6962 7574 6520  taset attribute 
-00006210: 696e 7374 6561 642e 222c 0a20 2020 2020  instead.",.     
-00006220: 2020 2020 2020 2044 6570 7265 6361 7469         Deprecati
-00006230: 6f6e 5761 726e 696e 672c 0a20 2020 2020  onWarning,.     
-00006240: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
-00006250: 662e 5f64 6174 6173 6574 203d 2064 6174  f._dataset = dat
-00006260: 6173 6574 0a0a 2020 2020 4070 726f 7065  aset..    @prope
-00006270: 7274 790a 2020 2020 6465 6620 6461 7461  rty.    def data
-00006280: 7365 7428 7365 6c66 293a 0a20 2020 2020  set(self):.     
-00006290: 2020 2022 2222 5365 7474 6572 2061 6e64     """Setter and
-000062a0: 2067 6574 7465 7220 6f66 2064 6973 706c   getter of displ
-000062b0: 6163 656d 656e 742d 666f 7263 6520 6461  acement-force da
-000062c0: 7461 7365 742e 0a0a 2020 2020 2020 2020  taset...        
-000062d0: 6469 6374 0a20 2020 2020 2020 2020 2020  dict.           
-000062e0: 2044 6973 706c 6163 656d 656e 7473 2069   Displacements i
-000062f0: 6e20 7375 7065 7263 656c 6c73 2e20 5468  n supercells. Th
-00006300: 6572 6520 6172 6520 7477 6f20 7479 7065  ere are two type
-00006310: 7320 6f66 2066 6f72 6d61 7473 2e0a 2020  s of formats..  
-00006320: 2020 2020 2020 2020 2020 5479 7065 2031            Type 1
-00006330: 2e20 5477 6f20 6174 6f6d 6963 2064 6973  . Two atomic dis
-00006340: 706c 6163 656d 656e 7420 696e 2065 6163  placement in eac
-00006350: 6820 7375 7065 7263 656c 6c3a 0a20 2020  h supercell:.   
-00006360: 2020 2020 2020 2020 2020 2020 207b 276e               {'n
-00006370: 6174 6f6d 273a 206e 756d 6265 7220 6f66  atom': number of
-00006380: 2061 746f 6d73 2069 6e20 7375 7065 7263   atoms in superc
-00006390: 656c 6c2c 0a20 2020 2020 2020 2020 2020  ell,.           
-000063a0: 2020 2020 2020 2766 6972 7374 5f61 746f        'first_ato
-000063b0: 6d73 273a 205b 0a20 2020 2020 2020 2020  ms': [.         
-000063c0: 2020 2020 2020 2020 2020 7b27 6e75 6d62            {'numb
-000063d0: 6572 273a 2061 746f 6d20 696e 6465 7820  er': atom index 
-000063e0: 6f66 2066 6972 7374 2064 6973 706c 6163  of first displac
-000063f0: 6564 2061 746f 6d2c 0a20 2020 2020 2020  ed atom,.       
-00006400: 2020 2020 2020 2020 2020 2020 2027 6469               'di
-00006410: 7370 6c61 6365 6d65 6e74 273a 2064 6973  splacement': dis
-00006420: 706c 6163 656d 656e 7420 696e 2043 6172  placement in Car
-00006430: 7465 7369 616e 2063 6f6f 7264 696e 6174  tesian coordinat
-00006440: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-00006450: 2020 2020 2020 2020 2766 6f72 6365 7327          'forces'
-00006460: 3a20 666f 7263 6573 206f 6e20 6174 6f6d  : forces on atom
-00006470: 7320 696e 2073 7570 6572 6365 6c6c 2c0a  s in supercell,.
-00006480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006490: 2020 2020 2769 6427 3a20 6469 7370 6c61      'id': displa
-000064a0: 6365 6d65 6e74 2069 6420 2831 2c20 322c  cement id (1, 2,
-000064b0: 2e2e 2e2c 6e5f 6669 7273 745f 6174 6f6d  ...,n_first_atom
-000064c0: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
-000064d0: 2020 2020 2020 2027 7365 636f 6e64 5f61         'second_a
-000064e0: 746f 6d73 273a 205b 0a20 2020 2020 2020  toms': [.       
-000064f0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00006500: 276e 756d 6265 7227 3a20 6174 6f6d 2069  'number': atom i
-00006510: 6e64 6578 206f 6620 7365 636f 6e64 2064  ndex of second d
-00006520: 6973 706c 6163 6564 2061 746f 6d2c 0a20  isplaced atom,. 
-00006530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006540: 2020 2020 2020 2764 6973 706c 6163 656d        'displacem
-00006550: 656e 7427 3a20 6469 7370 6c61 6365 6d65  ent': displaceme
-00006560: 6e74 2069 6e20 4361 7274 6573 6961 6e20  nt in Cartesian 
-00006570: 636f 6f72 6469 6e61 7465 737d 2c0a 2020  coordinates},.  
-00006580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006590: 2020 2020 2027 666f 7263 6573 273a 2066       'forces': f
-000065a0: 6f72 6365 7320 6f6e 2061 746f 6d73 2069  orces on atoms i
-000065b0: 6e20 7375 7065 7263 656c 6c2c 0a20 2020  n supercell,.   
-000065c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065d0: 2020 2020 2770 6169 725f 6469 7374 616e      'pair_distan
-000065e0: 6365 273a 2064 6973 7461 6e63 6520 6265  ce': distance be
-000065f0: 7477 6565 6e20 7061 6972 6564 2061 746f  tween paired ato
-00006600: 6d73 2c0a 2020 2020 2020 2020 2020 2020  ms,.            
-00006610: 2020 2020 2020 2020 2020 2027 696e 636c             'incl
-00006620: 7564 6564 273a 2077 6974 6820 6375 746f  uded': with cuto
-00006630: 6666 2070 6169 7220 6469 7374 616e 6365  ff pair distance
-00006640: 2069 6e20 6469 7370 6c61 6365 6d65 6e74   in displacement
-00006650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006670: 2020 2020 7061 6972 2067 656e 6572 6174      pair generat
-00006680: 696f 6e2c 2074 6869 7320 696e 6469 6361  ion, this indica
-00006690: 7465 7320 6966 2074 6869 730a 2020 2020  tes if this.    
-000066a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066b0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000066c0: 6169 7220 6469 7370 6c61 6365 6d65 6e74  air displacement
-000066d0: 7320 6973 2069 6e63 6c75 6465 6420 746f  s is included to
-000066e0: 2063 6f6d 7075 7465 0a20 2020 2020 2020   compute.       
-000066f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006700: 2020 2020 2020 2020 2020 2020 6663 3320              fc3 
-00006710: 6f72 206e 6f74 2c0a 2020 2020 2020 2020  or not,.        
-00006720: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00006730: 6964 273a 2064 6973 706c 6163 656d 656e  id': displacemen
-00006740: 7420 6964 2e20 286e 5f66 6972 7374 5f61  t id. (n_first_a
-00006750: 746f 6d73 202b 2031 2c20 2e2e 2e29 0a20  toms + 1, ...). 
-00006760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006770: 2020 2020 202e 2e2e 205d 207d 2c20 2e2e       ... ] }, ..
-00006780: 2e20 5d20 7d0a 2020 2020 2020 2020 2020  . ] }.          
-00006790: 2020 5479 7065 2032 2e20 416c 6c20 6174    Type 2. All at
-000067a0: 6f6d 6963 2064 6973 706c 6163 656d 656e  omic displacemen
-000067b0: 7473 2069 6e20 6561 6368 2073 7570 6572  ts in each super
-000067c0: 6365 6c6c 3a0a 2020 2020 2020 2020 2020  cell:.          
-000067d0: 2020 2020 2020 7b27 6469 7370 6c61 6365        {'displace
-000067e0: 6d65 6e74 7327 3a20 6e64 6172 7261 792c  ments': ndarray,
-000067f0: 2064 7479 7065 3d27 646f 7562 6c65 272c   dtype='double',
-00006800: 206f 7264 6572 3d27 4327 2c0a 2020 2020   order='C',.    
-00006810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006820: 2020 2020 2020 2020 2020 2020 2020 7368                sh
-00006830: 6170 653d 2873 7570 6572 6365 6c6c 732c  ape=(supercells,
-00006840: 2061 746f 6d73 2069 6e20 7375 7065 7263   atoms in superc
-00006850: 656c 6c2c 2033 290a 2020 2020 2020 2020  ell, 3).        
-00006860: 2020 2020 2020 2020 2027 666f 7263 6573           'forces
-00006870: 273a 206e 6461 7272 6179 2c20 6474 7970  ': ndarray, dtyp
-00006880: 653d 2764 6f75 626c 6527 2c2c 206f 7264  e='double',, ord
-00006890: 6572 3d27 4327 2c0a 2020 2020 2020 2020  er='C',.        
-000068a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068b0: 2020 2020 2020 2020 2020 7368 6170 653d            shape=
-000068c0: 2873 7570 6572 6365 6c6c 732c 2061 746f  (supercells, ato
-000068d0: 6d73 2069 6e20 7375 7065 7263 656c 6c2c  ms in supercell,
-000068e0: 2033 297d 0a20 2020 2020 2020 2020 2020   3)}.           
-000068f0: 2049 6e20 7479 7065 2032 2c20 6469 7370   In type 2, disp
-00006900: 6c61 6365 6d65 6e74 7320 616e 6420 666f  lacements and fo
-00006910: 7263 6573 2063 616e 2062 6520 6769 7665  rces can be give
-00006920: 6e20 6279 206e 756d 7079 2061 7272 6179  n by numpy array
-00006930: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-00006940: 6820 6469 6666 6572 656e 7420 7368 6170  h different shap
-00006950: 6520 6275 7420 7468 6174 2063 616e 2062  e but that can b
-00006960: 6520 7265 7368 6170 6564 2074 6f0a 2020  e reshaped to.  
-00006970: 2020 2020 2020 2020 2020 2873 7570 6572            (super
-00006980: 6365 6c6c 732c 206e 6174 6f6d 2c20 3329  cells, natom, 3)
-00006990: 2e0a 0a20 2020 2020 2020 2020 2020 2049  ...            I
-000069a0: 6e20 6164 6469 7469 6f6e 2c20 2764 7570  n addition, 'dup
-000069b0: 6c69 6361 7465 7327 2061 6e64 2027 6375  licates' and 'cu
-000069c0: 746f 6666 5f64 6973 7461 6e63 6527 2063  toff_distance' c
-000069d0: 616e 2065 7869 7374 2069 6e20 7468 6973  an exist in this
-000069e0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-000069f0: 6173 6574 2069 6e20 6469 7370 6c61 6365  aset in displace
-00006a00: 6d65 6e74 2070 6169 7220 6765 6e65 7261  ment pair genera
-00006a10: 7469 6f6e 2e20 2764 7570 6c69 6361 7465  tion. 'duplicate
-00006a20: 7327 2067 6976 6573 0a20 2020 2020 2020  s' gives.       
-00006a30: 2020 2020 2064 7570 6c69 6361 7465 6420       duplicated 
-00006a40: 7375 7065 7263 656c 6c20 6964 7320 6173  supercell ids as
-00006a50: 2070 6169 7273 2e0a 0a20 2020 2020 2020   pairs...       
-00006a60: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-00006a70: 7572 6e20 7365 6c66 2e5f 6461 7461 7365  urn self._datase
-00006a80: 740a 0a20 2020 2040 6461 7461 7365 742e  t..    @dataset.
-00006a90: 7365 7474 6572 0a20 2020 2064 6566 2064  setter.    def d
-00006aa0: 6174 6173 6574 2873 656c 662c 2064 6174  ataset(self, dat
-00006ab0: 6173 6574 293a 0a20 2020 2020 2020 2073  aset):.        s
-00006ac0: 656c 662e 5f64 6174 6173 6574 203d 2064  elf._dataset = d
-00006ad0: 6174 6173 6574 0a20 2020 2020 2020 2073  ataset.        s
-00006ae0: 656c 662e 5f73 7570 6572 6365 6c6c 735f  elf._supercells_
-00006af0: 7769 7468 5f64 6973 706c 6163 656d 656e  with_displacemen
-00006b00: 7473 203d 204e 6f6e 650a 2020 2020 2020  ts = None.      
-00006b10: 2020 7365 6c66 2e5f 7068 6f6e 6f6e 5f73    self._phonon_s
-00006b20: 7570 6572 6365 6c6c 735f 7769 7468 5f64  upercells_with_d
-00006b30: 6973 706c 6163 656d 656e 7473 203d 204e  isplacements = N
-00006b40: 6f6e 650a 0a20 2020 2040 7072 6f70 6572  one..    @proper
-00006b50: 7479 0a20 2020 2064 6566 2064 6973 706c  ty.    def displ
-00006b60: 6163 656d 656e 745f 6461 7461 7365 7428  acement_dataset(
-00006b70: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00006b80: 2222 5265 7475 726e 2064 6973 706c 6163  ""Return displac
-00006b90: 656d 656e 742d 666f 7263 6520 6461 7461  ement-force data
-00006ba0: 7365 742e 2222 220a 2020 2020 2020 2020  set.""".        
-00006bb0: 7761 726e 696e 6773 2e77 6172 6e28 0a20  warnings.warn(. 
-00006bc0: 2020 2020 2020 2020 2020 2022 5068 6f6e             "Phon
-00006bd0: 6f33 7079 2e64 6973 706c 6163 656d 656e  o3py.displacemen
-00006be0: 745f 6461 7461 7365 7420 6973 2064 6570  t_dataset is dep
-00006bf0: 7265 6361 7465 642e 2220 2255 7365 2050  recated." "Use P
-00006c00: 686f 6e6f 3370 792e 6461 7461 7365 742e  hono3py.dataset.
-00006c10: 222c 0a20 2020 2020 2020 2020 2020 2044  ",.            D
-00006c20: 6570 7265 6361 7469 6f6e 5761 726e 696e  eprecationWarnin
-00006c30: 672c 0a20 2020 2020 2020 2029 0a20 2020  g,.        ).   
-00006c40: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00006c50: 2e64 6174 6173 6574 0a0a 2020 2020 6465  .dataset..    de
-00006c60: 6620 6765 745f 6469 7370 6c61 6365 6d65  f get_displaceme
-00006c70: 6e74 5f64 6174 6173 6574 2873 656c 6629  nt_dataset(self)
-00006c80: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
-00006c90: 7572 6e20 6469 7370 6c61 6365 6d65 6e74  urn displacement
-00006ca0: 2d66 6f72 6365 2064 6174 6173 6574 2e22  -force dataset."
-00006cb0: 2222 0a20 2020 2020 2020 2077 6172 6e69  "".        warni
-00006cc0: 6e67 732e 7761 726e 280a 2020 2020 2020  ngs.warn(.      
-00006cd0: 2020 2020 2020 2250 686f 6e6f 3370 792e        "Phono3py.
-00006ce0: 6765 745f 6469 7370 6c61 6365 6d65 6e74  get_displacement
-00006cf0: 5f64 6174 6173 6574 2829 2069 7320 6465  _dataset() is de
-00006d00: 7072 6563 6174 6564 2e22 0a20 2020 2020  precated.".     
-00006d10: 2020 2020 2020 2022 5573 6520 5068 6f6e         "Use Phon
-00006d20: 6f33 7079 2e64 6174 6173 6574 2e22 2c0a  o3py.dataset.",.
-00006d30: 2020 2020 2020 2020 2020 2020 4465 7072              Depr
-00006d40: 6563 6174 696f 6e57 6172 6e69 6e67 2c0a  ecationWarning,.
-00006d50: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00006d60: 2020 7265 7475 726e 2073 656c 662e 6469    return self.di
-00006d70: 7370 6c61 6365 6d65 6e74 5f64 6174 6173  splacement_datas
-00006d80: 6574 0a0a 2020 2020 4070 726f 7065 7274  et..    @propert
-00006d90: 790a 2020 2020 6465 6620 7068 6f6e 6f6e  y.    def phonon
-00006da0: 5f64 6174 6173 6574 2873 656c 6629 3a0a  _dataset(self):.
-00006db0: 2020 2020 2020 2020 2222 2253 6574 7465          """Sette
-00006dc0: 7220 616e 6420 6765 7474 6572 206f 6620  r and getter of 
-00006dd0: 6469 7370 6c61 6365 6d65 6e74 2d66 6f72  displacement-for
-00006de0: 6365 2064 6174 6173 6574 2066 6f72 2066  ce dataset for f
-00006df0: 6332 2e0a 0a20 2020 2020 2020 2064 6963  c2...        dic
-00006e00: 740a 2020 2020 2020 2020 2020 2020 4469  t.            Di
-00006e10: 7370 6c61 6365 6d65 6e74 7320 696e 2073  splacements in s
-00006e20: 7570 6572 6365 6c6c 732e 2054 6865 7265  upercells. There
-00006e30: 2061 7265 2074 776f 2074 7970 6573 206f   are two types o
-00006e40: 6620 666f 726d 6174 732e 0a20 2020 2020  f formats..     
-00006e50: 2020 2020 2020 2054 7970 6520 312e 2054         Type 1. T
-00006e60: 776f 2061 746f 6d69 6320 6469 7370 6c61  wo atomic displa
-00006e70: 6365 6d65 6e74 2069 6e20 6561 6368 2073  cement in each s
-00006e80: 7570 6572 6365 6c6c 3a0a 2020 2020 2020  upercell:.      
-00006e90: 2020 2020 2020 2020 2020 7b27 6e61 746f            {'nato
-00006ea0: 6d27 3a20 6e75 6d62 6572 206f 6620 6174  m': number of at
-00006eb0: 6f6d 7320 696e 2073 7570 6572 6365 6c6c  oms in supercell
-00006ec0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006ed0: 2020 2027 6669 7273 745f 6174 6f6d 7327     'first_atoms'
-00006ee0: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
-00006ef0: 2020 2020 2020 207b 276e 756d 6265 7227         {'number'
-00006f00: 3a20 6174 6f6d 2069 6e64 6578 206f 6620  : atom index of 
-00006f10: 6669 7273 7420 6469 7370 6c61 6365 6420  first displaced 
-00006f20: 6174 6f6d 2c0a 2020 2020 2020 2020 2020  atom,.          
-00006f30: 2020 2020 2020 2020 2020 2764 6973 706c            'displ
-00006f40: 6163 656d 656e 7427 3a20 6469 7370 6c61  acement': displa
-00006f50: 6365 6d65 6e74 2069 6e20 4361 7274 6573  cement in Cartes
-00006f60: 6961 6e20 636f 6f72 6469 6e61 7465 732c  ian coordinates,
-00006f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006f80: 2020 2020 2027 666f 7263 6573 273a 2066       'forces': f
-00006f90: 6f72 6365 7320 6f6e 2061 746f 6d73 2069  orces on atoms i
-00006fa0: 6e20 7375 7065 7263 656c 6c7d 202e 2e2e  n supercell} ...
-00006fb0: 205d 7d0a 2020 2020 2020 2020 2020 2020   ]}.            
-00006fc0: 5479 7065 2032 2e20 416c 6c20 6174 6f6d  Type 2. All atom
-00006fd0: 6963 2064 6973 706c 6163 656d 656e 7473  ic displacements
-00006fe0: 2069 6e20 6561 6368 2073 7570 6572 6365   in each superce
-00006ff0: 6c6c 3a0a 2020 2020 2020 2020 2020 2020  ll:.            
-00007000: 2020 2020 7b27 6469 7370 6c61 6365 6d65      {'displaceme
-00007010: 6e74 7327 3a20 6e64 6172 7261 792c 2064  nts': ndarray, d
-00007020: 7479 7065 3d27 646f 7562 6c65 272c 206f  type='double', o
-00007030: 7264 6572 3d27 4327 2c0a 2020 2020 2020  rder='C',.      
-00007040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007050: 2020 2020 2020 2020 2020 2020 7368 6170              shap
-00007060: 653d 2873 7570 6572 6365 6c6c 732c 2061  e=(supercells, a
-00007070: 746f 6d73 2069 6e20 7375 7065 7263 656c  toms in supercel
-00007080: 6c2c 2033 290a 2020 2020 2020 2020 2020  l, 3).          
-00007090: 2020 2020 2020 2027 666f 7263 6573 273a         'forces':
-000070a0: 206e 6461 7272 6179 2c20 6474 7970 653d   ndarray, dtype=
-000070b0: 2764 6f75 626c 6527 2c2c 206f 7264 6572  'double',, order
-000070c0: 3d27 4327 2c0a 2020 2020 2020 2020 2020  ='C',.          
-000070d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070e0: 2020 2020 2020 2020 7368 6170 653d 2873          shape=(s
-000070f0: 7570 6572 6365 6c6c 732c 2061 746f 6d73  upercells, atoms
-00007100: 2069 6e20 7375 7065 7263 656c 6c2c 2033   in supercell, 3
-00007110: 297d 0a20 2020 2020 2020 2020 2020 2049  )}.            I
-00007120: 6e20 7479 7065 2032 2c20 6469 7370 6c61  n type 2, displa
-00007130: 6365 6d65 6e74 7320 616e 6420 666f 7263  cements and forc
-00007140: 6573 2063 616e 2062 6520 6769 7665 6e20  es can be given 
-00007150: 6279 206e 756d 7079 2061 7272 6179 0a20  by numpy array. 
-00007160: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00007170: 6469 6666 6572 656e 7420 7368 6170 6520  different shape 
-00007180: 6275 7420 7468 6174 2063 616e 2062 6520  but that can be 
-00007190: 7265 7368 6170 6564 2074 6f0a 2020 2020  reshaped to.    
-000071a0: 2020 2020 2020 2020 2873 7570 6572 6365          (superce
-000071b0: 6c6c 732c 206e 6174 6f6d 2c20 3329 2e0a  lls, natom, 3)..
-000071c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000071d0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000071e0: 2e5f 7068 6f6e 6f6e 5f64 6174 6173 6574  ._phonon_dataset
-000071f0: 0a0a 2020 2020 4070 686f 6e6f 6e5f 6461  ..    @phonon_da
-00007200: 7461 7365 742e 7365 7474 6572 0a20 2020  taset.setter.   
-00007210: 2064 6566 2070 686f 6e6f 6e5f 6461 7461   def phonon_data
-00007220: 7365 7428 7365 6c66 2c20 6461 7461 7365  set(self, datase
-00007230: 7429 3a0a 2020 2020 2020 2020 7365 6c66  t):.        self
-00007240: 2e5f 7068 6f6e 6f6e 5f64 6174 6173 6574  ._phonon_dataset
-00007250: 203d 2064 6174 6173 6574 0a0a 2020 2020   = dataset..    
-00007260: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00007270: 6620 7068 6f6e 6f6e 5f64 6973 706c 6163  f phonon_displac
-00007280: 656d 656e 745f 6461 7461 7365 7428 7365  ement_dataset(se
-00007290: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-000072a0: 5265 7475 726e 2070 686f 6e6f 6e20 6469  Return phonon di
-000072b0: 7370 616c 6365 6d65 6e74 2d66 6f72 6365  spalcement-force
-000072c0: 2064 6174 6173 6574 2e22 2222 0a20 2020   dataset.""".   
-000072d0: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
-000072e0: 726e 280a 2020 2020 2020 2020 2020 2020  rn(.            
-000072f0: 2250 686f 6e6f 3370 792e 7068 6f6e 6f6e  "Phono3py.phonon
-00007300: 5f64 6973 706c 6163 656d 656e 745f 6461  _displacement_da
-00007310: 7461 7365 7420 6973 2064 6570 7265 6361  taset is depreca
-00007320: 7465 642e 220a 2020 2020 2020 2020 2020  ted.".          
-00007330: 2020 2255 7365 2050 686f 6e6f 3370 792e    "Use Phono3py.
-00007340: 7068 6f6e 6f6e 5f64 6174 6173 6574 2e22  phonon_dataset."
-00007350: 2c0a 2020 2020 2020 2020 2020 2020 4465  ,.            De
-00007360: 7072 6563 6174 696f 6e57 6172 6e69 6e67  precationWarning
-00007370: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-00007380: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00007390: 5f70 686f 6e6f 6e5f 6461 7461 7365 740a  _phonon_dataset.
-000073a0: 0a20 2020 2064 6566 2067 6574 5f70 686f  .    def get_pho
-000073b0: 6e6f 6e5f 6469 7370 6c61 6365 6d65 6e74  non_displacement
-000073c0: 5f64 6174 6173 6574 2873 656c 6629 3a0a  _dataset(self):.
-000073d0: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
-000073e0: 6e20 7068 6f6e 6f6e 2064 6973 7061 6c63  n phonon dispalc
-000073f0: 656d 656e 742d 666f 7263 6520 6461 7461  ement-force data
-00007400: 7365 742e 2222 220a 2020 2020 2020 2020  set.""".        
-00007410: 7761 726e 696e 6773 2e77 6172 6e28 0a20  warnings.warn(. 
-00007420: 2020 2020 2020 2020 2020 2022 5068 6f6e             "Phon
-00007430: 6f33 7079 2e67 6574 5f70 686f 6e6f 6e5f  o3py.get_phonon_
-00007440: 6469 7370 6c61 6365 6d65 6e74 5f64 6174  displacement_dat
-00007450: 6173 6574 2829 2069 7320 6465 7072 6563  aset() is deprec
-00007460: 6174 6564 2e22 0a20 2020 2020 2020 2020  ated.".         
-00007470: 2020 2022 5573 6520 5068 6f6e 6f33 7079     "Use Phono3py
-00007480: 2e70 686f 6e6f 6e5f 6461 7461 7365 742e  .phonon_dataset.
-00007490: 222c 0a20 2020 2020 2020 2020 2020 2044  ",.            D
-000074a0: 6570 7265 6361 7469 6f6e 5761 726e 696e  eprecationWarnin
-000074b0: 672c 0a20 2020 2020 2020 2029 0a20 2020  g,.        ).   
-000074c0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000074d0: 2e70 686f 6e6f 6e5f 6469 7370 6c61 6365  .phonon_displace
-000074e0: 6d65 6e74 5f64 6174 6173 6574 0a0a 2020  ment_dataset..  
-000074f0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00007500: 6465 6620 6261 6e64 5f69 6e64 6963 6573  def band_indices
-00007510: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00007520: 2222 2253 6574 7465 7220 616e 6420 6765  """Setter and ge
-00007530: 7474 6572 206f 6620 6261 6e64 2069 6e64  tter of band ind
-00007540: 6963 6573 2e0a 0a20 2020 2020 2020 2061  ices...        a
-00007550: 7272 6179 5f6c 696b 650a 2020 2020 2020  rray_like.      
-00007560: 2020 2020 2020 4c69 7374 206f 6620 6261        List of ba
-00007570: 6e64 2069 6e64 6963 6573 2073 7065 6369  nd indices speci
-00007580: 6669 6564 2074 6f20 7365 6c65 6374 2073  fied to select s
-00007590: 7065 6369 6669 6320 6261 6e64 730a 2020  pecific bands.  
-000075a0: 2020 2020 2020 2020 2020 746f 2063 6f6d            to com
-000075b0: 7075 7465 7220 7068 2d70 6820 696e 7465  puter ph-ph inte
-000075c0: 7261 6374 696f 6e20 7265 6c61 7465 6420  raction related 
-000075d0: 7072 6f70 6572 7469 6573 2e0a 0a20 2020  properties...   
-000075e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000075f0: 2072 6574 7572 6e20 7365 6c66 2e5f 6261   return self._ba
-00007600: 6e64 5f69 6e64 6963 6573 0a0a 2020 2020  nd_indices..    
-00007610: 4062 616e 645f 696e 6469 6365 732e 7365  @band_indices.se
-00007620: 7474 6572 0a20 2020 2064 6566 2062 616e  tter.    def ban
-00007630: 645f 696e 6469 6365 7328 7365 6c66 2c20  d_indices(self, 
-00007640: 6261 6e64 5f69 6e64 6963 6573 293a 0a20  band_indices):. 
-00007650: 2020 2020 2020 2073 656c 662e 5f73 6574         self._set
-00007660: 5f62 616e 645f 696e 6469 6365 7328 6261  _band_indices(ba
-00007670: 6e64 5f69 6e64 6963 6573 3d62 616e 645f  nd_indices=band_
-00007680: 696e 6469 6365 7329 0a0a 2020 2020 6465  indices)..    de
-00007690: 6620 7365 745f 6261 6e64 5f69 6e64 6963  f set_band_indic
-000076a0: 6573 2873 656c 662c 2062 616e 645f 696e  es(self, band_in
-000076b0: 6469 6365 7329 3a0a 2020 2020 2020 2020  dices):.        
-000076c0: 2222 2253 6574 2062 616e 6420 696e 6469  """Set band indi
-000076d0: 6365 732e 2222 220a 2020 2020 2020 2020  ces.""".        
-000076e0: 7761 726e 696e 6773 2e77 6172 6e28 0a20  warnings.warn(. 
-000076f0: 2020 2020 2020 2020 2020 2022 5068 6f6e             "Phon
-00007700: 6f33 7079 2e73 6574 5f62 616e 645f 696e  o3py.set_band_in
-00007710: 6469 6365 7328 2920 6973 2064 6570 7265  dices() is depre
-00007720: 6361 7465 642e 220a 2020 2020 2020 2020  cated.".        
-00007730: 2020 2020 2255 7365 2050 686f 6e6f 3370      "Use Phono3p
-00007740: 792e 6261 6e64 5f69 6e64 6963 6573 2061  y.band_indices a
-00007750: 7474 7269 6275 7465 2069 6e73 7465 6164  ttribute instead
-00007760: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
-00007770: 4465 7072 6563 6174 696f 6e57 6172 6e69  DeprecationWarni
-00007780: 6e67 2c0a 2020 2020 2020 2020 290a 2020  ng,.        ).  
-00007790: 2020 2020 2020 7365 6c66 2e62 616e 645f        self.band_
-000077a0: 696e 6469 6365 7320 3d20 6261 6e64 5f69  indices = band_i
-000077b0: 6e64 6963 6573 0a0a 2020 2020 6465 6620  ndices..    def 
-000077c0: 5f73 6574 5f62 616e 645f 696e 6469 6365  _set_band_indice
-000077d0: 7328 7365 6c66 2c20 6261 6e64 5f69 6e64  s(self, band_ind
-000077e0: 6963 6573 3d4e 6f6e 6529 3a0a 2020 2020  ices=None):.    
-000077f0: 2020 2020 6966 2062 616e 645f 696e 6469      if band_indi
-00007800: 6365 7320 6973 204e 6f6e 653a 0a20 2020  ces is None:.   
-00007810: 2020 2020 2020 2020 206e 756d 5f62 616e           num_ban
-00007820: 6420 3d20 6c65 6e28 7365 6c66 2e5f 7072  d = len(self._pr
-00007830: 696d 6974 6976 6529 202a 2033 0a20 2020  imitive) * 3.   
-00007840: 2020 2020 2020 2020 2073 656c 662e 5f62           self._b
-00007850: 616e 645f 696e 6469 6365 7320 3d20 5b6e  and_indices = [n
-00007860: 702e 6172 616e 6765 286e 756d 5f62 616e  p.arange(num_ban
-00007870: 642c 2064 7479 7065 3d22 696e 745f 2229  d, dtype="int_")
-00007880: 5d0a 2020 2020 2020 2020 656c 7365 3a0a  ].        else:.
-00007890: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000078a0: 2e5f 6261 6e64 5f69 6e64 6963 6573 203d  ._band_indices =
-000078b0: 2062 616e 645f 696e 6469 6365 730a 2020   band_indices.  
-000078c0: 2020 2020 2020 7365 6c66 2e5f 6261 6e64        self._band
-000078d0: 5f69 6e64 6963 6573 5f66 6c61 7474 656e  _indices_flatten
-000078e0: 203d 206e 702e 6873 7461 636b 2873 656c   = np.hstack(sel
-000078f0: 662e 5f62 616e 645f 696e 6469 6365 7329  f._band_indices)
-00007900: 2e61 7374 7970 6528 2269 6e74 5f22 290a  .astype("int_").
-00007910: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00007920: 2020 2064 6566 206d 6173 7365 7328 7365     def masses(se
-00007930: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00007940: 5365 7474 6572 2061 6e64 2067 6574 7465  Setter and gette
-00007950: 7220 6f66 2061 746f 6d69 6320 6d61 7373  r of atomic mass
-00007960: 6573 206f 6620 7072 696d 6974 6976 6520  es of primitive 
-00007970: 6365 6c6c 2e22 2222 0a20 2020 2020 2020  cell.""".       
-00007980: 2072 6574 7572 6e20 7365 6c66 2e5f 7072   return self._pr
-00007990: 696d 6974 6976 652e 6d61 7373 6573 0a0a  imitive.masses..
-000079a0: 2020 2020 406d 6173 7365 732e 7365 7474      @masses.sett
-000079b0: 6572 0a20 2020 2064 6566 206d 6173 7365  er.    def masse
-000079c0: 7328 7365 6c66 2c20 6d61 7373 6573 293a  s(self, masses):
-000079d0: 0a20 2020 2020 2020 2069 6620 6d61 7373  .        if mass
-000079e0: 6573 2069 7320 4e6f 6e65 3a0a 2020 2020  es is None:.    
-000079f0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00007a00: 2020 2020 2020 2070 5f6d 6173 7365 7320         p_masses 
-00007a10: 3d20 6e70 2e61 7272 6179 286d 6173 7365  = np.array(masse
-00007a20: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
-00007a30: 5f70 7269 6d69 7469 7665 2e6d 6173 7365  _primitive.masse
-00007a40: 7320 3d20 705f 6d61 7373 6573 0a20 2020  s = p_masses.   
-00007a50: 2020 2020 2070 3270 5f6d 6170 203d 2073       p2p_map = s
-00007a60: 656c 662e 5f70 7269 6d69 7469 7665 2e70  elf._primitive.p
-00007a70: 3270 5f6d 6170 0a20 2020 2020 2020 2073  2p_map.        s
-00007a80: 5f6d 6173 7365 7320 3d20 705f 6d61 7373  _masses = p_mass
-00007a90: 6573 5b5b 7032 705f 6d61 705b 785d 2066  es[[p2p_map[x] f
-00007aa0: 6f72 2078 2069 6e20 7365 6c66 2e5f 7072  or x in self._pr
-00007ab0: 696d 6974 6976 652e 7332 705f 6d61 705d  imitive.s2p_map]
-00007ac0: 5d0a 2020 2020 2020 2020 7365 6c66 2e5f  ].        self._
-00007ad0: 7375 7065 7263 656c 6c2e 6d61 7373 6573  supercell.masses
-00007ae0: 203d 2073 5f6d 6173 7365 730a 2020 2020   = s_masses.    
-00007af0: 2020 2020 7532 735f 6d61 7020 3d20 7365      u2s_map = se
-00007b00: 6c66 2e5f 7375 7065 7263 656c 6c2e 7532  lf._supercell.u2
-00007b10: 735f 6d61 700a 2020 2020 2020 2020 755f  s_map.        u_
-00007b20: 6d61 7373 6573 203d 2073 5f6d 6173 7365  masses = s_masse
-00007b30: 735b 7532 735f 6d61 705d 0a20 2020 2020  s[u2s_map].     
-00007b40: 2020 2073 656c 662e 5f75 6e69 7463 656c     self._unitcel
-00007b50: 6c2e 6d61 7373 6573 203d 2075 5f6d 6173  l.masses = u_mas
-00007b60: 7365 730a 2020 2020 2020 2020 7365 6c66  ses.        self
-00007b70: 2e5f 7068 6f6e 6f6e 5f70 7269 6d69 7469  ._phonon_primiti
-00007b80: 7665 2e6d 6173 7365 7320 3d20 705f 6d61  ve.masses = p_ma
-00007b90: 7373 6573 0a20 2020 2020 2020 2070 3270  sses.        p2p
-00007ba0: 5f6d 6170 203d 2073 656c 662e 5f70 686f  _map = self._pho
-00007bb0: 6e6f 6e5f 7072 696d 6974 6976 652e 7032  non_primitive.p2
-00007bc0: 705f 6d61 700a 2020 2020 2020 2020 735f  p_map.        s_
-00007bd0: 6d61 7373 6573 203d 2070 5f6d 6173 7365  masses = p_masse
-00007be0: 735b 5b70 3270 5f6d 6170 5b78 5d20 666f  s[[p2p_map[x] fo
-00007bf0: 7220 7820 696e 2073 656c 662e 5f70 686f  r x in self._pho
-00007c00: 6e6f 6e5f 7072 696d 6974 6976 652e 7332  non_primitive.s2
-00007c10: 705f 6d61 705d 5d0a 2020 2020 2020 2020  p_map]].        
-00007c20: 7365 6c66 2e5f 7068 6f6e 6f6e 5f73 7570  self._phonon_sup
-00007c30: 6572 6365 6c6c 2e6d 6173 7365 7320 3d20  ercell.masses = 
-00007c40: 735f 6d61 7373 6573 0a0a 2020 2020 4070  s_masses..    @p
-00007c50: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00007c60: 7375 7065 7263 656c 6c73 5f77 6974 685f  supercells_with_
-00007c70: 6469 7370 6c61 6365 6d65 6e74 7328 7365  displacements(se
-00007c80: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00007c90: 5265 7475 726e 2073 7570 6572 6365 6c6c  Return supercell
-00007ca0: 7320 7769 7468 2064 6973 706c 6163 656d  s with displacem
-00007cb0: 656e 7473 2e0a 0a20 2020 2020 2020 206c  ents...        l
-00007cc0: 6973 7420 6f66 2050 686f 6e6f 7079 4174  ist of PhonopyAt
-00007cd0: 6f6d 730a 2020 2020 2020 2020 2020 2020  oms.            
-00007ce0: 5375 7065 7263 656c 6c73 2077 6974 6820  Supercells with 
-00007cf0: 6469 7370 6c61 6365 6d65 6e74 7320 6765  displacements ge
-00007d00: 6e65 7261 7465 6420 6279 0a20 2020 2020  nerated by.     
-00007d10: 2020 2020 2020 2050 686f 6e6f 3370 792e         Phono3py.
-00007d20: 6765 6e65 7261 7465 5f64 6973 706c 6163  generate_displac
-00007d30: 656d 656e 7473 2e0a 0a20 2020 2020 2020  ements...       
-00007d40: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
-00007d50: 7365 6c66 2e5f 7375 7065 7263 656c 6c73  self._supercells
-00007d60: 5f77 6974 685f 6469 7370 6c61 6365 6d65  _with_displaceme
-00007d70: 6e74 7320 6973 204e 6f6e 653a 0a20 2020  nts is None:.   
-00007d80: 2020 2020 2020 2020 2073 656c 662e 5f62           self._b
-00007d90: 7569 6c64 5f73 7570 6572 6365 6c6c 735f  uild_supercells_
-00007da0: 7769 7468 5f64 6973 706c 6163 656d 656e  with_displacemen
-00007db0: 7473 2829 0a20 2020 2020 2020 2072 6574  ts().        ret
-00007dc0: 7572 6e20 7365 6c66 2e5f 7375 7065 7263  urn self._superc
-00007dd0: 656c 6c73 5f77 6974 685f 6469 7370 6c61  ells_with_displa
-00007de0: 6365 6d65 6e74 730a 0a20 2020 2064 6566  cements..    def
-00007df0: 2067 6574 5f73 7570 6572 6365 6c6c 735f   get_supercells_
-00007e00: 7769 7468 5f64 6973 706c 6163 656d 656e  with_displacemen
-00007e10: 7473 2873 656c 6629 3a0a 2020 2020 2020  ts(self):.      
-00007e20: 2020 2222 2252 6574 7572 6e20 7375 7065    """Return supe
-00007e30: 7263 656c 6c73 2077 6974 6820 6469 7370  rcells with disp
-00007e40: 6c61 6365 6d65 6e74 732e 2222 220a 2020  lacements.""".  
-00007e50: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
-00007e60: 6172 6e28 0a20 2020 2020 2020 2020 2020  arn(.           
-00007e70: 2022 5068 6f6e 6f33 7079 2e67 6574 5f73   "Phono3py.get_s
-00007e80: 7570 6572 6365 6c6c 735f 7769 7468 5f64  upercells_with_d
-00007e90: 6973 706c 6163 656d 656e 7473 2829 2069  isplacements() i
-00007ea0: 7320 6465 7072 6563 6174 6564 2e22 0a20  s deprecated.". 
-00007eb0: 2020 2020 2020 2020 2020 2022 5573 6520             "Use 
-00007ec0: 5068 6f6e 6f33 7079 2e73 7570 6572 6365  Phono3py.superce
-00007ed0: 6c6c 735f 7769 7468 5f64 6973 706c 6163  lls_with_displac
-00007ee0: 656d 656e 7473 2061 7474 7269 6275 7465  ements attribute
-00007ef0: 2069 6e73 7465 6164 2e22 2c0a 2020 2020   instead.",.    
-00007f00: 2020 2020 2020 2020 4465 7072 6563 6174          Deprecat
-00007f10: 696f 6e57 6172 6e69 6e67 2c0a 2020 2020  ionWarning,.    
-00007f20: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
-00007f30: 7475 726e 2073 656c 662e 7375 7065 7263  turn self.superc
-00007f40: 656c 6c73 5f77 6974 685f 6469 7370 6c61  ells_with_displa
-00007f50: 6365 6d65 6e74 730a 0a20 2020 2040 7072  cements..    @pr
-00007f60: 6f70 6572 7479 0a20 2020 2064 6566 2070  operty.    def p
-00007f70: 686f 6e6f 6e5f 7375 7065 7263 656c 6c73  honon_supercells
-00007f80: 5f77 6974 685f 6469 7370 6c61 6365 6d65  _with_displaceme
-00007f90: 6e74 7328 7365 6c66 293a 0a20 2020 2020  nts(self):.     
-00007fa0: 2020 2022 2222 5265 7475 726e 2073 7570     """Return sup
-00007fb0: 6572 6365 6c6c 7320 7769 7468 2064 6973  ercells with dis
-00007fc0: 706c 6163 656d 656e 7473 2066 6f72 2066  placements for f
-00007fd0: 6332 2e0a 0a20 2020 2020 2020 206c 6973  c2...        lis
-00007fe0: 7420 6f66 2050 686f 6e6f 7079 4174 6f6d  t of PhonopyAtom
-00007ff0: 730a 2020 2020 2020 2020 2020 2020 5375  s.            Su
-00008000: 7065 7263 656c 6c73 2077 6974 6820 6469  percells with di
-00008010: 7370 6c61 6365 6d65 6e74 7320 6765 6e65  splacements gene
-00008020: 7261 7465 6420 6279 0a20 2020 2020 2020  rated by.       
-00008030: 2020 2020 2050 686f 6e6f 3370 792e 6765       Phono3py.ge
-00008040: 6e65 7261 7465 5f64 6973 706c 6163 656d  nerate_displacem
-00008050: 656e 7473 2e0a 0a20 2020 2020 2020 2022  ents...        "
-00008060: 2222 0a20 2020 2020 2020 2069 6620 7365  "".        if se
-00008070: 6c66 2e5f 7068 6f6e 6f6e 5f73 7570 6572  lf._phonon_super
-00008080: 6365 6c6c 735f 7769 7468 5f64 6973 706c  cells_with_displ
-00008090: 6163 656d 656e 7473 2069 7320 4e6f 6e65  acements is None
-000080a0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-000080b0: 2073 656c 662e 5f70 686f 6e6f 6e5f 6461   self._phonon_da
-000080c0: 7461 7365 7420 6973 206e 6f74 204e 6f6e  taset is not Non
-000080d0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000080e0: 2020 2073 656c 662e 5f70 686f 6e6f 6e5f     self._phonon_
-000080f0: 7375 7065 7263 656c 6c73 5f77 6974 685f  supercells_with_
-00008100: 6469 7370 6c61 6365 6d65 6e74 7320 3d20  displacements = 
-00008110: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00008120: 2020 2020 2020 7365 6c66 2e5f 6275 696c        self._buil
-00008130: 645f 7068 6f6e 6f6e 5f73 7570 6572 6365  d_phonon_superce
-00008140: 6c6c 735f 7769 7468 5f64 6973 706c 6163  lls_with_displac
-00008150: 656d 656e 7473 280a 2020 2020 2020 2020  ements(.        
-00008160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008170: 7365 6c66 2e5f 7068 6f6e 6f6e 5f73 7570  self._phonon_sup
-00008180: 6572 6365 6c6c 2c20 7365 6c66 2e5f 7068  ercell, self._ph
-00008190: 6f6e 6f6e 5f64 6174 6173 6574 0a20 2020  onon_dataset.   
-000081a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081b0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-000081c0: 2020 2029 0a20 2020 2020 2020 2072 6574     ).        ret
-000081d0: 7572 6e20 7365 6c66 2e5f 7068 6f6e 6f6e  urn self._phonon
-000081e0: 5f73 7570 6572 6365 6c6c 735f 7769 7468  _supercells_with
-000081f0: 5f64 6973 706c 6163 656d 656e 7473 0a0a  _displacements..
-00008200: 2020 2020 6465 6620 6765 745f 7068 6f6e      def get_phon
-00008210: 6f6e 5f73 7570 6572 6365 6c6c 735f 7769  on_supercells_wi
-00008220: 7468 5f64 6973 706c 6163 656d 656e 7473  th_displacements
-00008230: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00008240: 2222 2252 6574 7572 6e20 7375 7065 7263  """Return superc
-00008250: 656c 6c73 2077 6974 6820 6469 7370 6c61  ells with displa
-00008260: 6365 6d65 6e74 7320 666f 7220 6663 322e  cements for fc2.
-00008270: 2222 220a 2020 2020 2020 2020 7761 726e  """.        warn
-00008280: 696e 6773 2e77 6172 6e28 0a20 2020 2020  ings.warn(.     
-00008290: 2020 2020 2020 2022 5068 6f6e 6f33 7079         "Phono3py
-000082a0: 2e67 6574 5f70 686f 6e6f 6e5f 7375 7065  .get_phonon_supe
-000082b0: 7263 656c 6c73 5f77 6974 685f 6469 7370  rcells_with_disp
-000082c0: 6c61 6365 6d65 6e74 7328 2920 220a 2020  lacements() ".  
-000082d0: 2020 2020 2020 2020 2020 2269 7320 6465            "is de
-000082e0: 7072 6563 6174 6564 2e20 5573 6520 5068  precated. Use Ph
-000082f0: 6f6e 6f33 7079 2e70 686f 6e6f 6e5f 7375  ono3py.phonon_su
-00008300: 7065 7263 656c 6c73 5f77 6974 685f 6469  percells_with_di
-00008310: 7370 6c61 6365 6d65 6e74 7320 220a 2020  splacements ".  
-00008320: 2020 2020 2020 2020 2020 2261 7474 7269            "attri
-00008330: 6275 7465 2069 6e73 7465 6164 2e22 2c0a  bute instead.",.
-00008340: 2020 2020 2020 2020 2020 2020 4465 7072              Depr
-00008350: 6563 6174 696f 6e57 6172 6e69 6e67 2c0a  ecationWarning,.
-00008360: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00008370: 2020 7265 7475 726e 2073 656c 662e 7068    return self.ph
-00008380: 6f6e 6f6e 5f73 7570 6572 6365 6c6c 735f  onon_supercells_
-00008390: 7769 7468 5f64 6973 706c 6163 656d 656e  with_displacemen
-000083a0: 7473 0a0a 2020 2020 4070 726f 7065 7274  ts..    @propert
-000083b0: 790a 2020 2020 6465 6620 6d65 7368 5f6e  y.    def mesh_n
-000083c0: 756d 6265 7273 2873 656c 6629 3a0a 2020  umbers(self):.  
-000083d0: 2020 2020 2020 2222 2253 6574 7465 7220        """Setter 
-000083e0: 616e 6420 6765 7474 6572 206f 6620 7361  and getter of sa
-000083f0: 6d70 6c69 6e67 206d 6573 6820 6e75 6d62  mpling mesh numb
-00008400: 6572 7320 696e 2072 6563 6970 726f 6361  ers in reciproca
-00008410: 6c20 7370 6163 652e 2222 220a 2020 2020  l space.""".    
-00008420: 2020 2020 6966 2073 656c 662e 5f62 7a5f      if self._bz_
-00008430: 6772 6964 2069 7320 4e6f 6e65 3a0a 2020  grid is None:.  
-00008440: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00008450: 204e 6f6e 650a 2020 2020 2020 2020 656c   None.        el
-00008460: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00008470: 7265 7475 726e 2073 656c 662e 5f62 7a5f  return self._bz_
-00008480: 6772 6964 2e44 5f64 6961 670a 0a20 2020  grid.D_diag..   
-00008490: 2040 6d65 7368 5f6e 756d 6265 7273 2e73   @mesh_numbers.s
-000084a0: 6574 7465 720a 2020 2020 6465 6620 6d65  etter.    def me
-000084b0: 7368 5f6e 756d 6265 7273 2873 656c 662c  sh_numbers(self,
-000084c0: 206d 6573 685f 6e75 6d62 6572 733a 2055   mesh_numbers: U
-000084d0: 6e69 6f6e 5b69 6e74 2c20 666c 6f61 742c  nion[int, float,
-000084e0: 2053 6571 7565 6e63 652c 206e 702e 6e64   Sequence, np.nd
-000084f0: 6172 7261 795d 293a 0a20 2020 2020 2020  array]):.       
-00008500: 2073 656c 662e 5f73 6574 5f6d 6573 685f   self._set_mesh_
-00008510: 6e75 6d62 6572 7328 6d65 7368 5f6e 756d  numbers(mesh_num
-00008520: 6265 7273 290a 0a20 2020 2040 7072 6f70  bers)..    @prop
-00008530: 6572 7479 0a20 2020 2064 6566 2074 6865  erty.    def the
-00008540: 726d 616c 5f63 6f6e 6475 6374 6976 6974  rmal_conductivit
-00008550: 7928 7365 6c66 293a 0a20 2020 2020 2020  y(self):.       
-00008560: 2022 2222 5265 7475 726e 2074 6865 726d   """Return therm
-00008570: 616c 2063 6f6e 6475 6374 6976 6974 7920  al conductivity 
-00008580: 636c 6173 7320 696e 7374 616e 6365 2e22  class instance."
-00008590: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-000085a0: 6e20 7365 6c66 2e5f 7468 6572 6d61 6c5f  n self._thermal_
-000085b0: 636f 6e64 7563 7469 7669 7479 0a0a 2020  conductivity..  
-000085c0: 2020 6465 6620 6765 745f 7468 6572 6d61    def get_therma
-000085d0: 6c5f 636f 6e64 7563 7469 7669 7479 2873  l_conductivity(s
-000085e0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-000085f0: 2252 6574 7572 6e20 7468 6572 6d61 6c20  "Return thermal 
-00008600: 636f 6e64 7563 7469 7669 7479 2063 6c61  conductivity cla
-00008610: 7373 2069 6e73 7461 6e63 652e 2222 220a  ss instance.""".
-00008620: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
-00008630: 2e77 6172 6e28 0a20 2020 2020 2020 2020  .warn(.         
-00008640: 2020 2022 5068 6f6e 6f33 7079 2e67 6574     "Phono3py.get
-00008650: 5f74 6865 726d 616c 5f63 6f6e 6475 6374  _thermal_conduct
-00008660: 6976 6974 7928 2920 6973 2064 6570 7265  ivity() is depre
-00008670: 6361 7465 642e 220a 2020 2020 2020 2020  cated.".        
-00008680: 2020 2020 2255 7365 2050 686f 6e6f 3370      "Use Phono3p
-00008690: 792e 7468 6572 6d61 6c5f 636f 6e64 7563  y.thermal_conduc
-000086a0: 7469 7669 7479 2061 7474 7269 6275 7465  tivity attribute
-000086b0: 2069 6e73 7465 6164 2e22 2c0a 2020 2020   instead.",.    
-000086c0: 2020 2020 2020 2020 4465 7072 6563 6174          Deprecat
-000086d0: 696f 6e57 6172 6e69 6e67 2c0a 2020 2020  ionWarning,.    
-000086e0: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
-000086f0: 7475 726e 2073 656c 662e 7468 6572 6d61  turn self.therma
-00008700: 6c5f 636f 6e64 7563 7469 7669 7479 0a0a  l_conductivity..
-00008710: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00008720: 2020 6465 6620 6469 7370 6c61 6365 6d65    def displaceme
-00008730: 6e74 7328 7365 6c66 293a 0a20 2020 2020  nts(self):.     
-00008740: 2020 2022 2222 5365 7474 6572 2061 6e64     """Setter and
-00008750: 2067 6574 7465 7220 6469 7370 6c61 6365   getter displace
-00008760: 6d65 6e74 7320 696e 2073 7570 6572 6365  ments in superce
-00008770: 6c6c 732e 0a0a 2020 2020 2020 2020 5468  lls...        Th
-00008780: 6572 6520 6172 6520 7477 6f20 7479 7065  ere are two type
-00008790: 7320 6f66 2064 6973 706c 6163 656d 656e  s of displacemen
-000087a0: 7420 6461 7461 7365 742e 2053 6565 2074  t dataset. See t
-000087b0: 6865 2064 6f63 7374 7269 6e67 0a20 2020  he docstring.   
-000087c0: 2020 2020 206f 6620 6461 7461 7365 7420       of dataset 
-000087d0: 6162 6f75 7420 7479 7065 7320 3120 616e  about types 1 an
-000087e0: 6420 3220 666f 7220 7468 6520 6469 7370  d 2 for the disp
-000087f0: 6c61 6365 6d65 6e74 2064 6174 6173 6574  lacement dataset
-00008800: 2066 6f72 6d61 7473 2e0a 2020 2020 2020   formats..      
-00008810: 2020 4469 7370 6c61 6365 6d65 6e74 7320    Displacements 
-00008820: 7365 7420 7265 7475 726e 6564 2064 6570  set returned dep
-00008830: 656e 6473 206f 6e20 6569 7468 6572 2074  ends on either t
-00008840: 7970 652d 3120 6f72 2074 7970 652d 3220  ype-1 or type-2 
-00008850: 6173 0a20 2020 2020 2020 2066 6f6c 6c6f  as.        follo
-00008860: 7773 3a0a 0a20 2020 2020 2020 2054 7970  ws:..        Typ
-00008870: 652d 312c 204c 6973 7420 6f66 206c 6973  e-1, List of lis
-00008880: 740a 2020 2020 2020 2020 2020 2020 5468  t.            Th
-00008890: 6520 696e 7465 726e 616c 206c 6973 7420  e internal list 
-000088a0: 6861 7320 3420 656c 656d 656e 7473 2073  has 4 elements s
-000088b0: 7563 6820 6173 205b 3332 2c20 302e 3031  uch as [32, 0.01
-000088c0: 2c20 302e 302c 2030 2e30 5d5d 2e0a 2020  , 0.0, 0.0]]..  
-000088d0: 2020 2020 2020 2020 2020 5468 6520 6669            The fi
-000088e0: 7273 7420 656c 656d 656e 7420 6973 2074  rst element is t
-000088f0: 6865 2073 7570 6572 6365 6c6c 2061 746f  he supercell ato
-00008900: 6d20 696e 6465 7820 7374 6172 7469 6e67  m index starting
-00008910: 2077 6974 6820 302e 0a20 2020 2020 2020   with 0..       
-00008920: 2020 2020 2054 6865 2072 656d 6169 6e69       The remaini
-00008930: 6e67 2074 6872 6565 2065 6c65 6d65 6e74  ng three element
-00008940: 7320 6769 7665 2074 6865 2064 6973 706c  s give the displ
-00008950: 6163 656d 656e 7420 696e 2043 6172 7465  acement in Carte
-00008960: 7369 616e 0a20 2020 2020 2020 2020 2020  sian.           
-00008970: 2063 6f6f 7264 696e 6174 6573 2e0a 2020   coordinates..  
-00008980: 2020 2020 2020 5479 7065 2d32 2c20 6172        Type-2, ar
-00008990: 7261 795f 6c69 6b65 0a20 2020 2020 2020  ray_like.       
-000089a0: 2020 2020 2044 6973 706c 6163 656d 656e       Displacemen
-000089b0: 7473 206f 6620 616c 6c20 6174 6f6d 7320  ts of all atoms 
-000089c0: 6f66 2061 6c6c 2073 7570 6572 6365 6c6c  of all supercell
-000089d0: 7320 696e 2043 6172 7465 7369 616e 0a20  s in Cartesian. 
-000089e0: 2020 2020 2020 2020 2020 2063 6f6f 7264             coord
-000089f0: 696e 6174 6573 2e0a 2020 2020 2020 2020  inates..        
-00008a00: 2020 2020 7368 6170 653d 2873 7570 6572      shape=(super
-00008a10: 6365 6c6c 732c 206e 6174 6f6d 2c20 3329  cells, natom, 3)
-00008a20: 0a20 2020 2020 2020 2020 2020 2064 7479  .            dty
-00008a30: 7065 3d27 646f 7562 6c65 270a 0a0a 2020  pe='double'...  
-00008a40: 2020 2020 2020 466f 7220 7365 7474 6572        For setter
-00008a50: 2c20 6f6e 6c79 2074 7970 652d 3220 6461  , only type-2 da
-00008a60: 7461 7365 7420 666f 726d 6174 2069 7320  taset format is 
-00008a70: 616c 6c6f 7765 642e 0a0a 2020 2020 2020  allowed...      
-00008a80: 2020 6469 7370 6c61 6365 6d65 6e74 7320    displacements 
-00008a90: 3a20 6172 7261 795f 6c69 6b65 0a20 2020  : array_like.   
-00008aa0: 2020 2020 2020 2020 2041 746f 6d69 6320           Atomic 
-00008ab0: 6469 7370 6c61 6365 6d65 6e74 7320 6f66  displacements of
-00008ac0: 2061 6c6c 2061 746f 6d73 206f 6620 616c   all atoms of al
-00008ad0: 6c20 7375 7065 7263 656c 6c73 2e0a 2020  l supercells..  
-00008ae0: 2020 2020 2020 2020 2020 4f6e 6c79 2061            Only a
-00008af0: 6c6c 2064 6973 706c 6163 656d 656e 7473  ll displacements
-00008b00: 2069 6e20 6561 6368 2073 7570 6572 6365   in each superce
-00008b10: 6c6c 2063 6173 6520 2874 7970 652d 3229  ll case (type-2)
-00008b20: 2069 730a 2020 2020 2020 2020 2020 2020   is.            
-00008b30: 7375 7070 6f72 7465 642e 0a20 2020 2020  supported..     
-00008b40: 2020 2020 2020 2073 6861 7065 3d28 7375         shape=(su
-00008b50: 7065 7263 656c 6c73 2c20 6e61 746f 6d2c  percells, natom,
-00008b60: 2033 292c 2064 7479 7065 3d27 646f 7562   3), dtype='doub
-00008b70: 6c65 272c 206f 7264 6572 3d27 4327 0a0a  le', order='C'..
-00008b80: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00008b90: 2020 2020 6461 7461 7365 7420 3d20 7365      dataset = se
-00008ba0: 6c66 2e5f 6461 7461 7365 740a 0a20 2020  lf._dataset..   
-00008bb0: 2020 2020 2069 6620 2266 6972 7374 5f61       if "first_a
-00008bc0: 746f 6d73 2220 696e 2064 6174 6173 6574  toms" in dataset
-00008bd0: 3a0a 2020 2020 2020 2020 2020 2020 6e75  :.            nu
-00008be0: 6d5f 7363 656c 6c73 203d 206c 656e 2864  m_scells = len(d
-00008bf0: 6174 6173 6574 5b22 6669 7273 745f 6174  ataset["first_at
-00008c00: 6f6d 7322 5d29 0a20 2020 2020 2020 2020  oms"]).         
-00008c10: 2020 2066 6f72 2064 6973 7031 2069 6e20     for disp1 in 
-00008c20: 6461 7461 7365 745b 2266 6972 7374 5f61  dataset["first_a
-00008c30: 746f 6d73 225d 3a0a 2020 2020 2020 2020  toms"]:.        
-00008c40: 2020 2020 2020 2020 6e75 6d5f 7363 656c          num_scel
-00008c50: 6c73 202b 3d20 6c65 6e28 6469 7370 315b  ls += len(disp1[
-00008c60: 2273 6563 6f6e 645f 6174 6f6d 7322 5d29  "second_atoms"])
-00008c70: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
-00008c80: 706c 6163 656d 656e 7473 203d 206e 702e  placements = np.
-00008c90: 7a65 726f 7328 0a20 2020 2020 2020 2020  zeros(.         
-00008ca0: 2020 2020 2020 2028 6e75 6d5f 7363 656c         (num_scel
-00008cb0: 6c73 2c20 7365 6c66 2e5f 7375 7065 7263  ls, self._superc
-00008cc0: 656c 6c2e 6765 745f 6e75 6d62 6572 5f6f  ell.get_number_o
-00008cd0: 665f 6174 6f6d 7328 292c 2033 292c 0a20  f_atoms(), 3),. 
-00008ce0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00008cf0: 7479 7065 3d22 646f 7562 6c65 222c 0a20  type="double",. 
-00008d00: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00008d10: 7264 6572 3d22 4322 2c0a 2020 2020 2020  rder="C",.      
-00008d20: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00008d30: 2020 2020 6920 3d20 300a 2020 2020 2020      i = 0.      
-00008d40: 2020 2020 2020 666f 7220 6469 7370 3120        for disp1 
-00008d50: 696e 2064 6174 6173 6574 5b22 6669 7273  in dataset["firs
-00008d60: 745f 6174 6f6d 7322 5d3a 0a20 2020 2020  t_atoms"]:.     
-00008d70: 2020 2020 2020 2020 2020 2064 6973 706c             displ
-00008d80: 6163 656d 656e 7473 5b69 2c20 6469 7370  acements[i, disp
-00008d90: 315b 226e 756d 6265 7222 5d5d 203d 2064  1["number"]] = d
-00008da0: 6973 7031 5b22 6469 7370 6c61 6365 6d65  isp1["displaceme
-00008db0: 6e74 225d 0a20 2020 2020 2020 2020 2020  nt"].           
-00008dc0: 2020 2020 2069 202b 3d20 310a 2020 2020       i += 1.    
-00008dd0: 2020 2020 2020 2020 666f 7220 6469 7370          for disp
-00008de0: 3120 696e 2064 6174 6173 6574 5b22 6669  1 in dataset["fi
-00008df0: 7273 745f 6174 6f6d 7322 5d3a 0a20 2020  rst_atoms"]:.   
-00008e00: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00008e10: 2064 6973 7032 2069 6e20 6469 7370 315b   disp2 in disp1[
-00008e20: 2273 6563 6f6e 645f 6174 6f6d 7322 5d3a  "second_atoms"]:
-00008e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008e40: 2020 2020 2064 6973 706c 6163 656d 656e       displacemen
-00008e50: 7473 5b69 2c20 6469 7370 325b 226e 756d  ts[i, disp2["num
-00008e60: 6265 7222 5d5d 203d 2064 6973 7032 5b22  ber"]] = disp2["
-00008e70: 6469 7370 6c61 6365 6d65 6e74 225d 0a20  displacement"]. 
-00008e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e90: 2020 2069 202b 3d20 310a 2020 2020 2020     i += 1.      
-00008ea0: 2020 656c 6966 2022 666f 7263 6573 2220    elif "forces" 
-00008eb0: 696e 2064 6174 6173 6574 206f 7220 2264  in dataset or "d
-00008ec0: 6973 706c 6163 656d 656e 7473 2220 696e  isplacements" in
-00008ed0: 2064 6174 6173 6574 3a0a 2020 2020 2020   dataset:.      
-00008ee0: 2020 2020 2020 6469 7370 6c61 6365 6d65        displaceme
-00008ef0: 6e74 7320 3d20 6461 7461 7365 745b 2264  nts = dataset["d
-00008f00: 6973 706c 6163 656d 656e 7473 225d 0a20  isplacements"]. 
-00008f10: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00008f20: 2020 2020 2020 2020 2072 6169 7365 2052           raise R
-00008f30: 756e 7469 6d65 4572 726f 7228 2264 6973  untimeError("dis
-00008f40: 706c 6163 656d 656e 7420 6461 7461 7365  placement datase
-00008f50: 7420 6861 7320 7772 6f6e 6720 666f 726d  t has wrong form
-00008f60: 6174 2e22 290a 0a20 2020 2020 2020 2072  at.")..        r
-00008f70: 6574 7572 6e20 6469 7370 6c61 6365 6d65  eturn displaceme
-00008f80: 6e74 730a 0a20 2020 2040 6469 7370 6c61  nts..    @displa
-00008f90: 6365 6d65 6e74 732e 7365 7474 6572 0a20  cements.setter. 
-00008fa0: 2020 2064 6566 2064 6973 706c 6163 656d     def displacem
-00008fb0: 656e 7473 2873 656c 662c 2064 6973 706c  ents(self, displ
-00008fc0: 6163 656d 656e 7473 293a 0a20 2020 2020  acements):.     
-00008fd0: 2020 2064 6973 7073 203d 206e 702e 6172     disps = np.ar
-00008fe0: 7261 7928 6469 7370 6c61 6365 6d65 6e74  ray(displacement
-00008ff0: 732c 2064 7479 7065 3d22 646f 7562 6c65  s, dtype="double
-00009000: 222c 206f 7264 6572 3d22 4322 290a 2020  ", order="C").  
-00009010: 2020 2020 2020 6e61 746f 6d20 3d20 6c65        natom = le
-00009020: 6e28 7365 6c66 2e5f 7375 7065 7263 656c  n(self._supercel
-00009030: 6c29 0a20 2020 2020 2020 2069 6620 6469  l).        if di
-00009040: 7370 732e 6e64 696d 2021 3d20 3320 6f72  sps.ndim != 3 or
-00009050: 2064 6973 7073 2e73 6861 7065 5b31 3a5d   disps.shape[1:]
-00009060: 2021 3d20 286e 6174 6f6d 2c20 3329 3a0a   != (natom, 3):.
-00009070: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00009080: 6520 5275 6e74 696d 6545 7272 6f72 2822  e RuntimeError("
-00009090: 4172 7261 7920 7368 6170 6520 6f66 2064  Array shape of d
-000090a0: 6973 706c 6163 656d 656e 7473 2069 7320  isplacements is 
-000090b0: 696e 636f 7272 6563 742e 2229 0a20 2020  incorrect.").   
-000090c0: 2020 2020 2069 6620 7365 6c66 2e5f 6461       if self._da
-000090d0: 7461 7365 7420 6973 204e 6f6e 653a 0a20  taset is None:. 
-000090e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000090f0: 5f64 6174 6173 6574 203d 207b 7d0a 2020  _dataset = {}.  
-00009100: 2020 2020 2020 656c 6966 2022 6669 7273        elif "firs
-00009110: 745f 6174 6f6d 7322 2069 6e20 7365 6c66  t_atoms" in self
-00009120: 2e5f 6461 7461 7365 743a 0a20 2020 2020  ._dataset:.     
-00009130: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
-00009140: 7469 6d65 4572 726f 7228 2244 6973 706c  timeError("Displ
-00009150: 6163 656d 656e 7473 2061 7265 2069 6e63  acements are inc
-00009160: 6f6d 7061 7469 626c 6520 7769 7468 2064  ompatible with d
-00009170: 6174 6173 6574 2e22 290a 2020 2020 2020  ataset.").      
-00009180: 2020 7365 6c66 2e5f 6461 7461 7365 745b    self._dataset[
-00009190: 2264 6973 706c 6163 656d 656e 7473 225d  "displacements"]
-000091a0: 203d 2064 6973 7073 0a20 2020 2020 2020   = disps.       
-000091b0: 2073 656c 662e 5f73 7570 6572 6365 6c6c   self._supercell
-000091c0: 735f 7769 7468 5f64 6973 706c 6163 656d  s_with_displacem
-000091d0: 656e 7473 203d 204e 6f6e 650a 0a20 2020  ents = None..   
-000091e0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-000091f0: 6566 2066 6f72 6365 7328 7365 6c66 293a  ef forces(self):
-00009200: 0a20 2020 2020 2020 2022 2222 5365 7474  .        """Sett
-00009210: 6572 2061 6e64 2067 6574 7465 7220 6f66  er and getter of
-00009220: 2066 6f72 6365 7320 696e 2064 6973 706c   forces in displ
-00009230: 6163 656d 656e 7420 6461 7461 7365 742e  acement dataset.
-00009240: 0a0a 2020 2020 2020 2020 4120 7365 7420  ..        A set 
-00009250: 6f66 2061 746f 6d69 6320 666f 7263 6573  of atomic forces
-00009260: 2069 6e20 6469 7370 6c61 6365 6420 7375   in displaced su
-00009270: 7065 7263 656c 6c73 2e20 5468 6520 6f72  percells. The or
-00009280: 6465 7220 6f66 0a20 2020 2020 2020 2064  der of.        d
-00009290: 6973 706c 6163 6564 2073 7570 6572 6365  isplaced superce
-000092a0: 6c6c 7320 6861 7320 746f 206d 6174 6368  lls has to match
-000092b0: 2077 6974 6820 7468 6174 2069 6e20 6469   with that in di
-000092c0: 7370 6c61 6365 6d65 6e74 2064 6174 6173  splacement datas
-000092d0: 6574 2e0a 2020 2020 2020 2020 7368 6170  et..        shap
-000092e0: 653d 2864 6973 706c 6163 6564 2073 7570  e=(displaced sup
-000092f0: 6572 6365 6c6c 732c 2061 746f 6d73 2069  ercells, atoms i
-00009300: 6e20 7375 7065 7263 656c 6c2c 2033 290a  n supercell, 3).
-00009310: 0a20 2020 2020 2020 2067 6574 7465 7220  .        getter 
-00009320: 3a20 6e64 6172 7261 790a 0a20 2020 2020  : ndarray..     
-00009330: 2020 2073 6574 7465 7220 3a20 6172 7261     setter : arra
-00009340: 795f 6c69 6b65 0a20 2020 2020 2020 2020  y_like.         
-00009350: 2020 2054 6865 206f 7264 6572 206f 6620     The order of 
-00009360: 7375 7065 7263 656c 6c73 2075 7365 6420  supercells used 
-00009370: 666f 7220 6361 6c63 756c 6174 696e 6720  for calculating 
-00009380: 666f 7263 6573 2068 6173 2074 6f0a 2020  forces has to.  
-00009390: 2020 2020 2020 2020 2020 6265 2074 6865            be the
-000093a0: 2073 616d 6520 6f72 6465 7220 6f66 2073   same order of s
-000093b0: 7570 6572 6365 6c6c 735f 7769 7468 5f64  upercells_with_d
-000093c0: 6973 706c 6163 656d 656e 7473 2e0a 0a20  isplacements... 
-000093d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000093e0: 2020 2064 6174 6173 6574 203d 2073 656c     dataset = sel
-000093f0: 662e 5f64 6174 6173 6574 0a20 2020 2020  f._dataset.     
-00009400: 2020 2069 6620 2266 6f72 6365 7322 2069     if "forces" i
-00009410: 6e20 6461 7461 7365 743a 0a20 2020 2020  n dataset:.     
-00009420: 2020 2020 2020 2072 6574 7572 6e20 6461         return da
-00009430: 7461 7365 745b 2266 6f72 6365 7322 5d0a  taset["forces"].
-00009440: 2020 2020 2020 2020 656c 6966 2022 6669          elif "fi
-00009450: 7273 745f 6174 6f6d 7322 2069 6e20 6461  rst_atoms" in da
-00009460: 7461 7365 743a 0a20 2020 2020 2020 2020  taset:.         
-00009470: 2020 206e 756d 5f73 6365 6c6c 7320 3d20     num_scells = 
-00009480: 6c65 6e28 6461 7461 7365 745b 2266 6972  len(dataset["fir
-00009490: 7374 5f61 746f 6d73 225d 290a 2020 2020  st_atoms"]).    
-000094a0: 2020 2020 2020 2020 666f 7220 6469 7370          for disp
-000094b0: 3120 696e 2064 6174 6173 6574 5b22 6669  1 in dataset["fi
-000094c0: 7273 745f 6174 6f6d 7322 5d3a 0a20 2020  rst_atoms"]:.   
-000094d0: 2020 2020 2020 2020 2020 2020 206e 756d               num
-000094e0: 5f73 6365 6c6c 7320 2b3d 206c 656e 2864  _scells += len(d
-000094f0: 6973 7031 5b22 7365 636f 6e64 5f61 746f  isp1["second_ato
-00009500: 6d73 225d 290a 2020 2020 2020 2020 2020  ms"]).          
-00009510: 2020 666f 7263 6573 203d 206e 702e 7a65    forces = np.ze
-00009520: 726f 7328 0a20 2020 2020 2020 2020 2020  ros(.           
-00009530: 2020 2020 2028 6e75 6d5f 7363 656c 6c73       (num_scells
-00009540: 2c20 7365 6c66 2e5f 7375 7065 7263 656c  , self._supercel
-00009550: 6c2e 6765 745f 6e75 6d62 6572 5f6f 665f  l.get_number_of_
-00009560: 6174 6f6d 7328 292c 2033 292c 0a20 2020  atoms(), 3),.   
-00009570: 2020 2020 2020 2020 2020 2020 2064 7479               dty
-00009580: 7065 3d22 646f 7562 6c65 222c 0a20 2020  pe="double",.   
-00009590: 2020 2020 2020 2020 2020 2020 206f 7264               ord
-000095a0: 6572 3d22 4322 2c0a 2020 2020 2020 2020  er="C",.        
-000095b0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-000095c0: 2020 6920 3d20 300a 2020 2020 2020 2020    i = 0.        
-000095d0: 2020 2020 666f 7220 6469 7370 3120 696e      for disp1 in
-000095e0: 2064 6174 6173 6574 5b22 6669 7273 745f   dataset["first_
-000095f0: 6174 6f6d 7322 5d3a 0a20 2020 2020 2020  atoms"]:.       
-00009600: 2020 2020 2020 2020 2066 6f72 6365 735b           forces[
-00009610: 695d 203d 2064 6973 7031 5b22 666f 7263  i] = disp1["forc
-00009620: 6573 225d 0a20 2020 2020 2020 2020 2020  es"].           
-00009630: 2020 2020 2069 202b 3d20 310a 2020 2020       i += 1.    
-00009640: 2020 2020 2020 2020 666f 7220 6469 7370          for disp
-00009650: 3120 696e 2064 6174 6173 6574 5b22 6669  1 in dataset["fi
-00009660: 7273 745f 6174 6f6d 7322 5d3a 0a20 2020  rst_atoms"]:.   
-00009670: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00009680: 2064 6973 7032 2069 6e20 6469 7370 315b   disp2 in disp1[
-00009690: 2273 6563 6f6e 645f 6174 6f6d 7322 5d3a  "second_atoms"]:
-000096a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000096b0: 2020 2020 2066 6f72 6365 735b 695d 203d       forces[i] =
-000096c0: 2064 6973 7032 5b22 666f 7263 6573 225d   disp2["forces"]
-000096d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000096e0: 2020 2020 2069 202b 3d20 310a 2020 2020       i += 1.    
-000096f0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-00009700: 6f72 6365 730a 2020 2020 2020 2020 656c  orces.        el
-00009710: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00009720: 7261 6973 6520 5275 6e74 696d 6545 7272  raise RuntimeErr
-00009730: 6f72 2822 6469 7370 6c61 6365 6d65 6e74  or("displacement
-00009740: 2064 6174 6173 6574 2068 6173 2077 726f   dataset has wro
-00009750: 6e67 2066 6f72 6d61 742e 2229 0a0a 2020  ng format.")..  
-00009760: 2020 4066 6f72 6365 732e 7365 7474 6572    @forces.setter
-00009770: 0a20 2020 2064 6566 2066 6f72 6365 7328  .    def forces(
-00009780: 7365 6c66 2c20 666f 7263 6573 5f66 6333  self, forces_fc3
-00009790: 293a 0a20 2020 2020 2020 2066 6f72 6365  ):.        force
-000097a0: 7320 3d20 6e70 2e61 7272 6179 2866 6f72  s = np.array(for
-000097b0: 6365 735f 6663 332c 2064 7479 7065 3d22  ces_fc3, dtype="
-000097c0: 646f 7562 6c65 222c 206f 7264 6572 3d22  double", order="
-000097d0: 4322 290a 2020 2020 2020 2020 6461 7461  C").        data
-000097e0: 7365 7420 3d20 7365 6c66 2e5f 6461 7461  set = self._data
-000097f0: 7365 740a 2020 2020 2020 2020 6966 2022  set.        if "
-00009800: 6669 7273 745f 6174 6f6d 7322 2069 6e20  first_atoms" in 
-00009810: 6461 7461 7365 743a 0a20 2020 2020 2020  dataset:.       
-00009820: 2020 2020 2069 203d 2030 0a20 2020 2020       i = 0.     
-00009830: 2020 2020 2020 2066 6f72 2064 6973 7031         for disp1
-00009840: 2069 6e20 6461 7461 7365 745b 2266 6972   in dataset["fir
-00009850: 7374 5f61 746f 6d73 225d 3a0a 2020 2020  st_atoms"]:.    
-00009860: 2020 2020 2020 2020 2020 2020 6469 7370              disp
-00009870: 315b 2266 6f72 6365 7322 5d20 3d20 666f  1["forces"] = fo
-00009880: 7263 6573 5b69 5d0a 2020 2020 2020 2020  rces[i].        
-00009890: 2020 2020 2020 2020 6920 2b3d 2031 0a20          i += 1. 
-000098a0: 2020 2020 2020 2020 2020 2066 6f72 2064             for d
-000098b0: 6973 7031 2069 6e20 6461 7461 7365 745b  isp1 in dataset[
-000098c0: 2266 6972 7374 5f61 746f 6d73 225d 3a0a  "first_atoms"]:.
-000098d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098e0: 666f 7220 6469 7370 3220 696e 2064 6973  for disp2 in dis
-000098f0: 7031 5b22 7365 636f 6e64 5f61 746f 6d73  p1["second_atoms
-00009900: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-00009910: 2020 2020 2020 2020 6469 7370 325b 2266          disp2["f
-00009920: 6f72 6365 7322 5d20 3d20 666f 7263 6573  orces"] = forces
-00009930: 5b69 5d0a 2020 2020 2020 2020 2020 2020  [i].            
-00009940: 2020 2020 2020 2020 6920 2b3d 2031 0a20          i += 1. 
-00009950: 2020 2020 2020 2065 6c69 6620 2264 6973         elif "dis
-00009960: 706c 6163 656d 656e 7473 2220 696e 2064  placements" in d
-00009970: 6174 6173 6574 206f 7220 2266 6f72 6365  ataset or "force
-00009980: 7322 2069 6e20 6461 7461 7365 743a 0a20  s" in dataset:. 
-00009990: 2020 2020 2020 2020 2020 2064 6174 6173             datas
-000099a0: 6574 5b22 666f 7263 6573 225d 203d 2066  et["forces"] = f
-000099b0: 6f72 6365 730a 0a20 2020 2040 7072 6f70  orces..    @prop
-000099c0: 6572 7479 0a20 2020 2064 6566 2070 686f  erty.    def pho
-000099d0: 6e6f 6e5f 6469 7370 6c61 6365 6d65 6e74  non_displacement
-000099e0: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
-000099f0: 2022 2222 5365 7474 6572 2061 6e64 2067   """Setter and g
-00009a00: 6574 7465 7220 6f66 2064 6973 706c 6163  etter of displac
-00009a10: 656d 656e 7473 2069 6e20 7375 7065 7263  ements in superc
-00009a20: 656c 6c73 2066 6f72 2066 6332 2e0a 0a20  ells for fc2... 
-00009a30: 2020 2020 2020 2054 6865 7265 2061 7265         There are
-00009a40: 2074 776f 2074 7970 6573 206f 6620 6469   two types of di
-00009a50: 7370 6c61 6365 6d65 6e74 2064 6174 6173  splacement datas
-00009a60: 6574 2e20 5365 6520 7468 6520 646f 6373  et. See the docs
-00009a70: 7472 696e 670a 2020 2020 2020 2020 6f66  tring.        of
-00009a80: 2064 6174 6173 6574 2061 626f 7574 2074   dataset about t
-00009a90: 7970 6573 2031 2061 6e64 2032 2066 6f72  ypes 1 and 2 for
-00009aa0: 2074 6865 2064 6973 706c 6163 656d 656e   the displacemen
-00009ab0: 7420 6461 7461 7365 7420 666f 726d 6174  t dataset format
-00009ac0: 732e 0a20 2020 2020 2020 2044 6973 706c  s..        Displ
-00009ad0: 6163 656d 656e 7473 2073 6574 2072 6574  acements set ret
-00009ae0: 7572 6e65 6420 6465 7065 6e64 7320 6f6e  urned depends on
-00009af0: 2065 6974 6865 7220 7479 7065 2d31 206f   either type-1 o
-00009b00: 7220 7479 7065 2d32 2061 730a 2020 2020  r type-2 as.    
-00009b10: 2020 2020 666f 6c6c 6f77 733a 0a0a 2020      follows:..  
-00009b20: 2020 2020 2020 5479 7065 2d31 2c20 4c69        Type-1, Li
-00009b30: 7374 206f 6620 6c69 7374 0a20 2020 2020  st of list.     
-00009b40: 2020 2020 2020 2054 6865 2069 6e74 6572         The inter
-00009b50: 6e61 6c20 6c69 7374 2068 6173 2034 2065  nal list has 4 e
-00009b60: 6c65 6d65 6e74 7320 7375 6368 2061 7320  lements such as 
-00009b70: 5b33 322c 2030 2e30 312c 2030 2e30 2c20  [32, 0.01, 0.0, 
-00009b80: 302e 305d 5d2e 0a20 2020 2020 2020 2020  0.0]]..         
-00009b90: 2020 2054 6865 2066 6972 7374 2065 6c65     The first ele
-00009ba0: 6d65 6e74 2069 7320 7468 6520 7375 7065  ment is the supe
-00009bb0: 7263 656c 6c20 6174 6f6d 2069 6e64 6578  rcell atom index
-00009bc0: 2073 7461 7274 696e 6720 7769 7468 2030   starting with 0
-00009bd0: 2e0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-00009be0: 6520 7265 6d61 696e 696e 6720 7468 7265  e remaining thre
-00009bf0: 6520 656c 656d 656e 7473 2067 6976 6520  e elements give 
-00009c00: 7468 6520 6469 7370 6c61 6365 6d65 6e74  the displacement
-00009c10: 2069 6e20 4361 7274 6573 6961 6e0a 2020   in Cartesian.  
-00009c20: 2020 2020 2020 2020 2020 636f 6f72 6469            coordi
-00009c30: 6e61 7465 732e 0a20 2020 2020 2020 2054  nates..        T
-00009c40: 7970 652d 322c 2061 7272 6179 5f6c 696b  ype-2, array_lik
-00009c50: 650a 2020 2020 2020 2020 2020 2020 4469  e.            Di
-00009c60: 7370 6c61 6365 6d65 6e74 7320 6f66 2061  splacements of a
-00009c70: 6c6c 2061 746f 6d73 206f 6620 616c 6c20  ll atoms of all 
-00009c80: 7375 7065 7263 656c 6c73 2069 6e20 4361  supercells in Ca
-00009c90: 7274 6573 6961 6e0a 2020 2020 2020 2020  rtesian.        
-00009ca0: 2020 2020 636f 6f72 6469 6e61 7465 732e      coordinates.
-00009cb0: 0a20 2020 2020 2020 2020 2020 2073 6861  .            sha
-00009cc0: 7065 3d28 7375 7065 7263 656c 6c73 2c20  pe=(supercells, 
-00009cd0: 6e61 746f 6d2c 2033 290a 2020 2020 2020  natom, 3).      
-00009ce0: 2020 2020 2020 6474 7970 653d 2764 6f75        dtype='dou
-00009cf0: 626c 6527 0a0a 0a20 2020 2020 2020 2046  ble'...        F
-00009d00: 6f72 2073 6574 7465 722c 206f 6e6c 7920  or setter, only 
-00009d10: 7479 7065 2d32 2064 6174 6173 6574 2066  type-2 dataset f
-00009d20: 6f72 6d61 7420 6973 2061 6c6c 6f77 6564  ormat is allowed
-00009d30: 2e0a 0a20 2020 2020 2020 2064 6973 706c  ...        displ
-00009d40: 6163 656d 656e 7473 203a 2061 7272 6179  acements : array
-00009d50: 5f6c 696b 650a 2020 2020 2020 2020 2020  _like.          
-00009d60: 2020 4174 6f6d 6963 2064 6973 706c 6163    Atomic displac
-00009d70: 656d 656e 7473 206f 6620 616c 6c20 6174  ements of all at
-00009d80: 6f6d 7320 6f66 2061 6c6c 2073 7570 6572  oms of all super
-00009d90: 6365 6c6c 732e 0a20 2020 2020 2020 2020  cells..         
-00009da0: 2020 204f 6e6c 7920 616c 6c20 6469 7370     Only all disp
-00009db0: 6c61 6365 6d65 6e74 7320 696e 2065 6163  lacements in eac
-00009dc0: 6820 7375 7065 7263 656c 6c20 6361 7365  h supercell case
-00009dd0: 2028 7479 7065 2d32 2920 6973 0a20 2020   (type-2) is.   
-00009de0: 2020 2020 2020 2020 2073 7570 706f 7274           support
-00009df0: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
-00009e00: 7368 6170 653d 2873 7570 6572 6365 6c6c  shape=(supercell
-00009e10: 732c 206e 6174 6f6d 2c20 3329 2c20 6474  s, natom, 3), dt
-00009e20: 7970 653d 2764 6f75 626c 6527 2c20 6f72  ype='double', or
-00009e30: 6465 723d 2743 270a 0a20 2020 2020 2020  der='C'..       
-00009e40: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
-00009e50: 7365 6c66 2e5f 7068 6f6e 6f6e 5f73 7570  self._phonon_sup
-00009e60: 6572 6365 6c6c 5f6d 6174 7269 7820 6973  ercell_matrix is
-00009e70: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00009e80: 2020 2072 6169 7365 2052 756e 7469 6d65     raise Runtime
-00009e90: 4572 726f 7228 2270 686f 6e6f 6e5f 7375  Error("phonon_su
-00009ea0: 7065 7263 656c 6c5f 6d61 7472 6978 2069  percell_matrix i
-00009eb0: 7320 6e6f 7420 7365 742e 2229 0a0a 2020  s not set.")..  
-00009ec0: 2020 2020 2020 6461 7461 7365 7420 3d20        dataset = 
-00009ed0: 7365 6c66 2e5f 7068 6f6e 6f6e 5f64 6174  self._phonon_dat
-00009ee0: 6173 6574 0a20 2020 2020 2020 2069 6620  aset.        if 
-00009ef0: 2266 6972 7374 5f61 746f 6d73 2220 696e  "first_atoms" in
-00009f00: 2064 6174 6173 6574 3a0a 2020 2020 2020   dataset:.      
-00009f10: 2020 2020 2020 6e75 6d5f 7363 656c 6c73        num_scells
-00009f20: 203d 206c 656e 2864 6174 6173 6574 5b22   = len(dataset["
-00009f30: 6669 7273 745f 6174 6f6d 7322 5d29 0a20  first_atoms"]). 
-00009f40: 2020 2020 2020 2020 2020 206e 6174 6f6d             natom
-00009f50: 203d 206c 656e 2873 656c 662e 5f70 686f   = len(self._pho
-00009f60: 6e6f 6e5f 7375 7065 7263 656c 6c29 0a20  non_supercell). 
-00009f70: 2020 2020 2020 2020 2020 2064 6973 706c             displ
-00009f80: 6163 656d 656e 7473 203d 206e 702e 7a65  acements = np.ze
-00009f90: 726f 7328 286e 756d 5f73 6365 6c6c 732c  ros((num_scells,
-00009fa0: 206e 6174 6f6d 2c20 3329 2c20 6474 7970   natom, 3), dtyp
-00009fb0: 653d 2264 6f75 626c 6522 2c20 6f72 6465  e="double", orde
-00009fc0: 723d 2243 2229 0a20 2020 2020 2020 2020  r="C").         
-00009fd0: 2020 2066 6f72 2069 2c20 6469 7370 3120     for i, disp1 
-00009fe0: 696e 2065 6e75 6d65 7261 7465 2864 6174  in enumerate(dat
-00009ff0: 6173 6574 5b22 6669 7273 745f 6174 6f6d  aset["first_atom
-0000a000: 7322 5d29 3a0a 2020 2020 2020 2020 2020  s"]):.          
-0000a010: 2020 2020 2020 6469 7370 6c61 6365 6d65        displaceme
-0000a020: 6e74 735b 692c 2064 6973 7031 5b22 6e75  nts[i, disp1["nu
-0000a030: 6d62 6572 225d 5d20 3d20 6469 7370 315b  mber"]] = disp1[
-0000a040: 2264 6973 706c 6163 656d 656e 7422 5d0a  "displacement"].
-0000a050: 2020 2020 2020 2020 656c 6966 2022 666f          elif "fo
-0000a060: 7263 6573 2220 696e 2064 6174 6173 6574  rces" in dataset
-0000a070: 206f 7220 2264 6973 706c 6163 656d 656e   or "displacemen
-0000a080: 7473 2220 696e 2064 6174 6173 6574 3a0a  ts" in dataset:.
-0000a090: 2020 2020 2020 2020 2020 2020 6469 7370              disp
-0000a0a0: 6c61 6365 6d65 6e74 7320 3d20 6461 7461  lacements = data
-0000a0b0: 7365 745b 2264 6973 706c 6163 656d 656e  set["displacemen
-0000a0c0: 7473 225d 0a20 2020 2020 2020 2065 6c73  ts"].        els
-0000a0d0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0000a0e0: 6169 7365 2052 756e 7469 6d65 4572 726f  aise RuntimeErro
-0000a0f0: 7228 2264 6973 706c 6163 656d 656e 7420  r("displacement 
-0000a100: 6461 7461 7365 7420 6861 7320 7772 6f6e  dataset has wron
-0000a110: 6720 666f 726d 6174 2e22 290a 0a20 2020  g format.")..   
-0000a120: 2020 2020 2072 6574 7572 6e20 6469 7370       return disp
-0000a130: 6c61 6365 6d65 6e74 730a 0a20 2020 2040  lacements..    @
-0000a140: 7068 6f6e 6f6e 5f64 6973 706c 6163 656d  phonon_displacem
-0000a150: 656e 7473 2e73 6574 7465 720a 2020 2020  ents.setter.    
-0000a160: 6465 6620 7068 6f6e 6f6e 5f64 6973 706c  def phonon_displ
-0000a170: 6163 656d 656e 7473 2873 656c 662c 2064  acements(self, d
-0000a180: 6973 706c 6163 656d 656e 7473 293a 0a20  isplacements):. 
-0000a190: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
-0000a1a0: 7068 6f6e 6f6e 5f73 7570 6572 6365 6c6c  phonon_supercell
-0000a1b0: 5f6d 6174 7269 7820 6973 204e 6f6e 653a  _matrix is None:
-0000a1c0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0000a1d0: 7365 2052 756e 7469 6d65 4572 726f 7228  se RuntimeError(
-0000a1e0: 2270 686f 6e6f 6e5f 7375 7065 7263 656c  "phonon_supercel
-0000a1f0: 6c5f 6d61 7472 6978 2069 7320 6e6f 7420  l_matrix is not 
-0000a200: 7365 742e 2229 0a0a 2020 2020 2020 2020  set.")..        
-0000a210: 6469 7370 7320 3d20 6e70 2e61 7272 6179  disps = np.array
-0000a220: 2864 6973 706c 6163 656d 656e 7473 2c20  (displacements, 
-0000a230: 6474 7970 653d 2264 6f75 626c 6522 2c20  dtype="double", 
-0000a240: 6f72 6465 723d 2243 2229 0a20 2020 2020  order="C").     
-0000a250: 2020 206e 6174 6f6d 203d 206c 656e 2873     natom = len(s
-0000a260: 656c 662e 5f70 686f 6e6f 6e5f 7375 7065  elf._phonon_supe
-0000a270: 7263 656c 6c29 0a20 2020 2020 2020 2069  rcell).        i
-0000a280: 6620 6469 7370 732e 6e64 696d 2021 3d20  f disps.ndim != 
-0000a290: 3320 6f72 2064 6973 7073 2e73 6861 7065  3 or disps.shape
-0000a2a0: 5b31 3a5d 2021 3d20 286e 6174 6f6d 2c20  [1:] != (natom, 
-0000a2b0: 3329 3a0a 2020 2020 2020 2020 2020 2020  3):.            
-0000a2c0: 7261 6973 6520 5275 6e74 696d 6545 7272  raise RuntimeErr
-0000a2d0: 6f72 2822 4172 7261 7920 7368 6170 6520  or("Array shape 
-0000a2e0: 6f66 2064 6973 706c 6163 656d 656e 7473  of displacements
-0000a2f0: 2069 7320 696e 636f 7272 6563 742e 2229   is incorrect.")
-0000a300: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000a310: 2e5f 7068 6f6e 6f6e 5f64 6174 6173 6574  ._phonon_dataset
-0000a320: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0000a330: 2020 2020 2020 7365 6c66 2e5f 7068 6f6e        self._phon
-0000a340: 6f6e 5f64 6174 6173 6574 203d 207b 7d0a  on_dataset = {}.
-0000a350: 2020 2020 2020 2020 656c 6966 2022 6669          elif "fi
-0000a360: 7273 745f 6174 6f6d 7322 2069 6e20 7365  rst_atoms" in se
-0000a370: 6c66 2e5f 7068 6f6e 6f6e 5f64 6174 6173  lf._phonon_datas
-0000a380: 6574 3a0a 2020 2020 2020 2020 2020 2020  et:.            
-0000a390: 7261 6973 6520 5275 6e74 696d 6545 7272  raise RuntimeErr
-0000a3a0: 6f72 2822 4469 7370 6c61 6365 6d65 6e74  or("Displacement
-0000a3b0: 7320 6172 6520 696e 636f 6d70 6174 6962  s are incompatib
-0000a3c0: 6c65 2077 6974 6820 6461 7461 7365 742e  le with dataset.
-0000a3d0: 2229 0a0a 2020 2020 2020 2020 7365 6c66  ")..        self
-0000a3e0: 2e5f 7068 6f6e 6f6e 5f64 6174 6173 6574  ._phonon_dataset
-0000a3f0: 5b22 6469 7370 6c61 6365 6d65 6e74 7322  ["displacements"
-0000a400: 5d20 3d20 6469 7370 730a 2020 2020 2020  ] = disps.      
-0000a410: 2020 7365 6c66 2e5f 7068 6f6e 6f6e 5f73    self._phonon_s
-0000a420: 7570 6572 6365 6c6c 735f 7769 7468 5f64  upercells_with_d
-0000a430: 6973 706c 6163 656d 656e 7473 203d 204e  isplacements = N
-0000a440: 6f6e 650a 0a20 2020 2040 7072 6f70 6572  one..    @proper
-0000a450: 7479 0a20 2020 2064 6566 2070 686f 6e6f  ty.    def phono
-0000a460: 6e5f 666f 7263 6573 2873 656c 6629 3a0a  n_forces(self):.
-0000a470: 2020 2020 2020 2020 2222 2253 6574 7465          """Sette
-0000a480: 7220 616e 6420 6765 7474 6572 206f 6620  r and getter of 
-0000a490: 666f 7263 6573 2069 6e20 6469 7370 6c61  forces in displa
-0000a4a0: 6365 6d65 6e74 2064 6174 6173 6574 2066  cement dataset f
-0000a4b0: 6f72 2066 6332 2e0a 0a20 2020 2020 2020  or fc2...       
-0000a4c0: 2041 2073 6574 206f 6620 6174 6f6d 6963   A set of atomic
-0000a4d0: 2066 6f72 6365 7320 696e 2064 6973 706c   forces in displ
-0000a4e0: 6163 6564 2073 7570 6572 6365 6c6c 732e  aced supercells.
-0000a4f0: 2054 6865 206f 7264 6572 206f 660a 2020   The order of.  
-0000a500: 2020 2020 2020 6469 7370 6c61 6365 6420        displaced 
-0000a510: 7375 7065 7263 656c 6c73 2068 6173 2074  supercells has t
-0000a520: 6f20 6d61 7463 6820 7769 7468 2074 6861  o match with tha
-0000a530: 7420 696e 2070 686f 6e6f 6e20 6469 7370  t in phonon disp
-0000a540: 6c61 6365 6d65 6e74 0a20 2020 2020 2020  lacement.       
-0000a550: 2064 6174 6173 6574 2e0a 2020 2020 2020   dataset..      
-0000a560: 2020 7368 6170 653d 2864 6973 706c 6163    shape=(displac
-0000a570: 6564 2073 7570 6572 6365 6c6c 732c 2061  ed supercells, a
-0000a580: 746f 6d73 2069 6e20 7375 7065 7263 656c  toms in supercel
-0000a590: 6c2c 2033 290a 0a20 2020 2020 2020 2067  l, 3)..        g
-0000a5a0: 6574 7465 7220 3a20 6e64 6172 7261 790a  etter : ndarray.
-0000a5b0: 0a20 2020 2020 2020 2073 6574 7465 7220  .        setter 
-0000a5c0: 3a20 6172 7261 795f 6c69 6b65 0a20 2020  : array_like.   
-0000a5d0: 2020 2020 2020 2020 2054 6865 206f 7264           The ord
-0000a5e0: 6572 206f 6620 7375 7065 7263 656c 6c73  er of supercells
-0000a5f0: 2075 7365 6420 666f 7220 6361 6c63 756c   used for calcul
-0000a600: 6174 696e 6720 666f 7263 6573 2068 6173  ating forces has
-0000a610: 2074 6f0a 2020 2020 2020 2020 2020 2020   to.            
-0000a620: 6265 2074 6865 2073 616d 6520 6f72 6465  be the same orde
-0000a630: 7220 6f66 2070 686f 6e6f 6e5f 7375 7065  r of phonon_supe
-0000a640: 7263 656c 6c73 5f77 6974 685f 6469 7370  rcells_with_disp
-0000a650: 6c61 6365 6d65 6e74 732e 0a0a 2020 2020  lacements...    
-0000a660: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000a670: 6966 2073 656c 662e 5f70 686f 6e6f 6e5f  if self._phonon_
-0000a680: 6461 7461 7365 7420 6973 204e 6f6e 653a  dataset is None:
-0000a690: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0000a6a0: 7365 2052 756e 7469 6d65 4572 726f 7228  se RuntimeError(
-0000a6b0: 2270 686f 6e6f 6e5f 6469 7370 6c61 6365  "phonon_displace
-0000a6c0: 6d65 6e74 5f64 6174 6173 6574 2064 6f65  ment_dataset doe
-0000a6d0: 7320 6e6f 7420 6578 6973 742e 2229 0a0a  s not exist.")..
-0000a6e0: 2020 2020 2020 2020 6461 7461 7365 7420          dataset 
-0000a6f0: 3d20 7365 6c66 2e5f 7068 6f6e 6f6e 5f64  = self._phonon_d
-0000a700: 6174 6173 6574 0a20 2020 2020 2020 2069  ataset.        i
-0000a710: 6620 2266 6f72 6365 7322 2069 6e20 6461  f "forces" in da
-0000a720: 7461 7365 743a 0a20 2020 2020 2020 2020  taset:.         
-0000a730: 2020 2072 6574 7572 6e20 6461 7461 7365     return datase
-0000a740: 745b 2266 6f72 6365 7322 5d0a 2020 2020  t["forces"].    
-0000a750: 2020 2020 656c 6966 2022 6669 7273 745f      elif "first_
-0000a760: 6174 6f6d 7322 2069 6e20 6461 7461 7365  atoms" in datase
-0000a770: 743a 0a20 2020 2020 2020 2020 2020 206e  t:.            n
-0000a780: 756d 5f73 6365 6c6c 7320 3d20 6c65 6e28  um_scells = len(
-0000a790: 6461 7461 7365 745b 2266 6972 7374 5f61  dataset["first_a
-0000a7a0: 746f 6d73 225d 290a 2020 2020 2020 2020  toms"]).        
-0000a7b0: 2020 2020 666f 7263 6573 203d 206e 702e      forces = np.
-0000a7c0: 7a65 726f 7328 0a20 2020 2020 2020 2020  zeros(.         
-0000a7d0: 2020 2020 2020 2028 6e75 6d5f 7363 656c         (num_scel
-0000a7e0: 6c73 2c20 7365 6c66 2e5f 7068 6f6e 6f6e  ls, self._phonon
-0000a7f0: 5f73 7570 6572 6365 6c6c 2e67 6574 5f6e  _supercell.get_n
-0000a800: 756d 6265 725f 6f66 5f61 746f 6d73 2829  umber_of_atoms()
-0000a810: 2c20 3329 2c0a 2020 2020 2020 2020 2020  , 3),.          
-0000a820: 2020 2020 2020 6474 7970 653d 2264 6f75        dtype="dou
-0000a830: 626c 6522 2c0a 2020 2020 2020 2020 2020  ble",.          
-0000a840: 2020 2020 2020 6f72 6465 723d 2243 222c        order="C",
-0000a850: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0000a860: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-0000a870: 2c20 6469 7370 3120 696e 2065 6e75 6d65  , disp1 in enume
-0000a880: 7261 7465 2864 6174 6173 6574 5b22 6669  rate(dataset["fi
-0000a890: 7273 745f 6174 6f6d 7322 5d29 3a0a 2020  rst_atoms"]):.  
-0000a8a0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000a8b0: 7263 6573 5b69 5d20 3d20 6469 7370 315b  rces[i] = disp1[
-0000a8c0: 2266 6f72 6365 7322 5d0a 2020 2020 2020  "forces"].      
-0000a8d0: 2020 2020 2020 7265 7475 726e 2066 6f72        return for
-0000a8e0: 6365 730a 2020 2020 2020 2020 656c 7365  ces.        else
-0000a8f0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-0000a900: 6973 6520 5275 6e74 696d 6545 7272 6f72  ise RuntimeError
-0000a910: 2822 6469 7370 6c61 6365 6d65 6e74 2064  ("displacement d
-0000a920: 6174 6173 6574 2068 6173 2077 726f 6e67  ataset has wrong
-0000a930: 2066 6f72 6d61 742e 2229 0a0a 2020 2020   format.")..    
-0000a940: 4070 686f 6e6f 6e5f 666f 7263 6573 2e73  @phonon_forces.s
-0000a950: 6574 7465 720a 2020 2020 6465 6620 7068  etter.    def ph
-0000a960: 6f6e 6f6e 5f66 6f72 6365 7328 7365 6c66  onon_forces(self
-0000a970: 2c20 666f 7263 6573 5f66 6332 293a 0a20  , forces_fc2):. 
-0000a980: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
-0000a990: 7068 6f6e 6f6e 5f64 6174 6173 6574 2069  phonon_dataset i
-0000a9a0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0000a9b0: 2020 2020 7261 6973 6520 5275 6e74 696d      raise Runtim
-0000a9c0: 6545 7272 6f72 2822 7068 6f6e 6f6e 5f64  eError("phonon_d
-0000a9d0: 6973 706c 6163 656d 656e 745f 6461 7461  isplacement_data
-0000a9e0: 7365 7420 646f 6573 206e 6f74 2065 7869  set does not exi
-0000a9f0: 7374 2e22 290a 0a20 2020 2020 2020 2066  st.")..        f
-0000aa00: 6f72 6365 7320 3d20 6e70 2e61 7272 6179  orces = np.array
-0000aa10: 2866 6f72 6365 735f 6663 322c 2064 7479  (forces_fc2, dty
-0000aa20: 7065 3d22 646f 7562 6c65 222c 206f 7264  pe="double", ord
-0000aa30: 6572 3d22 4322 290a 2020 2020 2020 2020  er="C").        
-0000aa40: 6461 7461 7365 7420 3d20 7365 6c66 2e5f  dataset = self._
-0000aa50: 7068 6f6e 6f6e 5f64 6174 6173 6574 0a20  phonon_dataset. 
-0000aa60: 2020 2020 2020 2069 6620 2266 6972 7374         if "first
-0000aa70: 5f61 746f 6d73 2220 696e 2064 6174 6173  _atoms" in datas
-0000aa80: 6574 3a0a 2020 2020 2020 2020 2020 2020  et:.            
-0000aa90: 6920 3d20 300a 2020 2020 2020 2020 2020  i = 0.          
-0000aaa0: 2020 666f 7220 692c 2064 6973 7031 2069    for i, disp1 i
-0000aab0: 6e20 656e 756d 6572 6174 6528 6461 7461  n enumerate(data
-0000aac0: 7365 745b 2266 6972 7374 5f61 746f 6d73  set["first_atoms
-0000aad0: 225d 293a 0a20 2020 2020 2020 2020 2020  "]):.           
-0000aae0: 2020 2020 2064 6973 7031 5b22 666f 7263       disp1["forc
-0000aaf0: 6573 225d 203d 2066 6f72 6365 735b 695d  es"] = forces[i]
-0000ab00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ab10: 2069 202b 3d20 310a 2020 2020 2020 2020   i += 1.        
-0000ab20: 656c 6966 2022 6469 7370 6c61 6365 6d65  elif "displaceme
-0000ab30: 6e74 7322 2069 6e20 6461 7461 7365 7420  nts" in dataset 
-0000ab40: 6f72 2022 666f 7263 6573 2220 696e 2064  or "forces" in d
-0000ab50: 6174 6173 6574 3a0a 2020 2020 2020 2020  ataset:.        
-0000ab60: 2020 2020 6461 7461 7365 745b 2266 6f72      dataset["for
-0000ab70: 6365 7322 5d20 3d20 666f 7263 6573 0a0a  ces"] = forces..
-0000ab80: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-0000ab90: 2020 6465 6620 7068 7068 5f69 6e74 6572    def phph_inter
-0000aba0: 6163 7469 6f6e 2873 656c 6629 3a0a 2020  action(self):.  
-0000abb0: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
-0000abc0: 496e 7465 7261 6374 696f 6e20 696e 7374  Interaction inst
-0000abd0: 616e 6365 2e22 2222 0a20 2020 2020 2020  ance.""".       
-0000abe0: 2072 6574 7572 6e20 7365 6c66 2e5f 696e   return self._in
-0000abf0: 7465 7261 6374 696f 6e0a 0a20 2020 2064  teraction..    d
-0000ac00: 6566 2067 6574 5f70 6870 685f 696e 7465  ef get_phph_inte
-0000ac10: 7261 6374 696f 6e28 7365 6c66 293a 0a20  raction(self):. 
-0000ac20: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
-0000ac30: 2049 6e74 6572 6163 7469 6f6e 2069 6e73   Interaction ins
-0000ac40: 7461 6e63 652e 2222 220a 2020 2020 2020  tance.""".      
-0000ac50: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
-0000ac60: 0a20 2020 2020 2020 2020 2020 2022 5068  .            "Ph
-0000ac70: 6f6e 6f33 7079 2e67 6574 5f70 6870 685f  ono3py.get_phph_
-0000ac80: 696e 7465 7261 6374 696f 6e28 2920 6973  interaction() is
-0000ac90: 2064 6570 7265 6361 7465 642e 220a 2020   deprecated.".  
-0000aca0: 2020 2020 2020 2020 2020 2255 7365 2050            "Use P
-0000acb0: 686f 6e6f 3370 792e 7068 7068 5f69 6e74  hono3py.phph_int
-0000acc0: 6572 6163 7469 6f6e 2061 7474 7269 6275  eraction attribu
-0000acd0: 7465 2069 6e73 7465 6164 2e22 2c0a 2020  te instead.",.  
-0000ace0: 2020 2020 2020 2020 2020 4465 7072 6563            Deprec
-0000acf0: 6174 696f 6e57 6172 6e69 6e67 2c0a 2020  ationWarning,.  
-0000ad00: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000ad10: 7265 7475 726e 2073 656c 662e 7068 7068  return self.phph
-0000ad20: 5f69 6e74 6572 6163 7469 6f6e 0a0a 2020  _interaction..  
-0000ad30: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-0000ad40: 6465 6620 6465 7461 696c 6564 5f67 616d  def detailed_gam
-0000ad50: 6d61 7328 7365 6c66 293a 0a20 2020 2020  mas(self):.     
-0000ad60: 2020 2022 2222 5265 7475 726e 2064 6574     """Return det
-0000ad70: 6169 6c65 6420 6761 6d6d 612e 2222 220a  ailed gamma.""".
-0000ad80: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000ad90: 656c 662e 5f64 6574 6169 6c65 645f 6761  elf._detailed_ga
-0000ada0: 6d6d 6173 0a0a 2020 2020 4070 726f 7065  mmas..    @prope
-0000adb0: 7274 790a 2020 2020 6465 6620 6772 6964  rty.    def grid
-0000adc0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000add0: 2222 2252 6574 7572 6e20 4272 696c 6c6f  """Return Brillo
-0000ade0: 7569 6e20 7a6f 6e65 2067 7269 6420 696e  uin zone grid in
-0000adf0: 666f 726d 6174 696f 6e2e 0a0a 2020 2020  formation...    
-0000ae00: 2020 2020 425a 4772 6964 0a20 2020 2020      BZGrid.     
-0000ae10: 2020 2020 2020 2041 6e20 696e 7374 616e         An instan
-0000ae20: 6365 206f 6620 425a 4772 6964 2075 7365  ce of BZGrid use
-0000ae30: 6420 666f 7220 656e 7469 7265 2070 686f  d for entire pho
-0000ae40: 6e6f 3370 7920 6361 6c63 756c 6174 696f  no3py calculatio
-0000ae50: 6e2e 0a0a 2020 2020 2020 2020 2222 220a  n...        """.
-0000ae60: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000ae70: 656c 662e 5f62 7a5f 6772 6964 0a0a 2020  elf._bz_grid..  
-0000ae80: 2020 6465 6620 696e 6974 5f70 6870 685f    def init_phph_
-0000ae90: 696e 7465 7261 6374 696f 6e28 0a20 2020  interaction(.   
-0000aea0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0000aeb0: 2020 206e 6163 5f71 5f64 6972 6563 7469     nac_q_directi
-0000aec0: 6f6e 3d4e 6f6e 652c 0a20 2020 2020 2020  on=None,.       
-0000aed0: 2063 6f6e 7374 616e 745f 6176 6572 6167   constant_averag
-0000aee0: 6564 5f69 6e74 6572 6163 7469 6f6e 3d4e  ed_interaction=N
-0000aef0: 6f6e 652c 0a20 2020 2020 2020 2066 7265  one,.        fre
-0000af00: 7175 656e 6379 5f73 6361 6c65 5f66 6163  quency_scale_fac
-0000af10: 746f 723d 4e6f 6e65 2c0a 2020 2020 2020  tor=None,.      
-0000af20: 2020 7379 6d6d 6574 7269 7a65 5f66 6333    symmetrize_fc3
-0000af30: 713a 2062 6f6f 6c20 3d20 4661 6c73 652c  q: bool = False,
-0000af40: 0a20 2020 2020 2020 206c 6170 6163 6b5f  .        lapack_
-0000af50: 7a68 6565 765f 7570 6c6f 3d22 4c22 2c0a  zheev_uplo="L",.
-0000af60: 2020 2020 2020 2020 6f70 656e 6d70 5f70          openmp_p
-0000af70: 6572 5f74 7269 706c 6574 733d 4e6f 6e65  er_triplets=None
-0000af80: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-0000af90: 2022 2222 496e 6974 6961 6c69 7a65 2070   """Initialize p
-0000afa0: 682d 7068 2069 6e74 6572 6163 7469 6f6e  h-ph interaction
-0000afb0: 2063 616c 6375 6c61 7469 6f6e 2e0a 0a20   calculation... 
-0000afc0: 2020 2020 2020 2054 6869 7320 6d65 7468         This meth
-0000afd0: 6f64 2063 7265 6174 6573 2061 6e20 696e  od creates an in
-0000afe0: 7374 616e 6365 206f 6620 496e 7465 7261  stance of Intera
-0000aff0: 6374 696f 6e20 636c 6173 732c 2077 6869  ction class, whi
-0000b000: 6368 0a20 2020 2020 2020 2069 7320 6e65  ch.        is ne
-0000b010: 6365 7373 6172 7920 746f 2072 756e 2070  cessary to run p
-0000b020: 682d 7068 2069 6e74 6572 6163 7469 6f6e  h-ph interaction
-0000b030: 2063 616c 6375 6c61 7469 6f6e 2e0a 2020   calculation..  
-0000b040: 2020 2020 2020 5468 6520 696e 7075 7420        The input 
-0000b050: 6461 7461 2073 7563 6820 6173 2067 7269  data such as gri
-0000b060: 6473 2c20 666f 7263 6520 636f 6e73 7461  ds, force consta
-0000b070: 6e74 732c 2065 7463 2c20 6172 650a 2020  nts, etc, are.  
-0000b080: 2020 2020 2020 7374 6f72 6564 2074 6f20        stored to 
-0000b090: 6265 2072 6561 6479 2066 6f72 2074 6865  be ready for the
-0000b0a0: 2063 616c 6375 6c61 7469 6f6e 2e0a 0a20   calculation... 
-0000b0b0: 2020 2020 2020 204e 6f74 650a 2020 2020         Note.    
-0000b0c0: 2020 2020 2d2d 2d2d 0a20 2020 2020 2020      ----.       
-0000b0d0: 2066 6333 2061 6e64 2066 6332 2c20 616e   fc3 and fc2, an
-0000b0e0: 6420 6f70 7469 6f6e 616c 6c79 206e 6163  d optionally nac
-0000b0f0: 5f70 6172 616d 7320 6861 7665 2074 6f20  _params have to 
-0000b100: 6265 2073 6574 2062 6566 6f72 6520 6361  be set before ca
-0000b110: 6c6c 696e 670a 2020 2020 2020 2020 7468  lling.        th
-0000b120: 6973 206d 6574 686f 642e 2066 6333 2061  is method. fc3 a
-0000b130: 6e64 2066 6332 2063 616e 2062 6520 6d61  nd fc2 can be ma
-0000b140: 6465 2065 6974 6865 7220 6672 6f6d 2073  de either from s
-0000b150: 6574 7320 6f66 2066 6f72 6365 730a 2020  ets of forces.  
-0000b160: 2020 2020 2020 616e 6420 6469 7370 6c61        and displa
-0000b170: 6365 6d65 6e74 7320 6f66 2073 7570 6572  cements of super
-0000b180: 6365 6c6c 7320 6f72 2062 6520 7365 7420  cells or be set 
-0000b190: 7369 6d70 6c79 2076 6961 2061 7474 7269  simply via attri
-0000b1a0: 6275 7465 732e 0a0a 2020 2020 2020 2020  butes...        
-0000b1b0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-0000b1c0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-0000b1d0: 2020 2020 2020 6e61 635f 715f 6469 7265        nac_q_dire
-0000b1e0: 6374 696f 6e20 3a20 6172 7261 795f 6c69  ction : array_li
-0000b1f0: 6b65 2c20 6f70 7469 6f6e 616c 0a20 2020  ke, optional.   
-0000b200: 2020 2020 2020 2020 2044 6972 6563 7469           Directi
-0000b210: 6f6e 206f 6620 712d 7665 6374 6f72 2077  on of q-vector w
-0000b220: 6174 6368 696e 6720 6672 6f6d 2047 616d  atching from Gam
-0000b230: 6d61 2070 6f69 6e74 2075 7365 6420 666f  ma point used fo
-0000b240: 720a 2020 2020 2020 2020 2020 2020 6e6f  r.            no
-0000b250: 6e2d 616e 616c 7974 6963 616c 2074 6572  n-analytical ter
-0000b260: 6d20 636f 7272 6563 7469 6f6e 2e20 5468  m correction. Th
-0000b270: 6973 2069 7320 6566 6665 6374 6976 6520  is is effective 
-0000b280: 6f6e 6c79 2061 7420 713d 300a 2020 2020  only at q=0.    
-0000b290: 2020 2020 2020 2020 2870 6879 7369 6361          (physica
-0000b2a0: 6c6c 7920 712d 3e30 292e 2054 6865 2064  lly q->0). The d
-0000b2b0: 6972 6563 7469 6f6e 2069 7320 6769 7665  irection is give
-0000b2c0: 6e20 696e 2063 7279 7374 616c 6c6f 6772  n in crystallogr
-0000b2d0: 6170 6869 630a 2020 2020 2020 2020 2020  aphic.          
-0000b2e0: 2020 2866 7261 6374 696f 6e61 6c29 2063    (fractional) c
-0000b2f0: 6f6f 7264 696e 6174 6573 2e0a 2020 2020  oordinates..    
-0000b300: 2020 2020 2020 2020 7368 6170 653d 2833          shape=(3
-0000b310: 2c29 2c20 6474 7970 653d 2764 6f75 626c  ,), dtype='doubl
-0000b320: 6527 2e0a 2020 2020 2020 2020 2020 2020  e'..            
-0000b330: 4465 6661 756c 7420 7661 6c75 6520 6973  Default value is
-0000b340: 204e 6f6e 652c 2077 6869 6368 206d 6561   None, which mea
-0000b350: 6e73 2074 6869 7320 6665 6174 7572 6520  ns this feature 
-0000b360: 6973 206e 6f74 2075 7365 642e 0a20 2020  is not used..   
-0000b370: 2020 2020 2063 6f6e 7374 616e 745f 6176       constant_av
-0000b380: 6572 6167 6564 5f69 6e74 6572 6163 7469  eraged_interacti
-0000b390: 6f6e 203a 2066 6c6f 6174 2c20 6f70 7469  on : float, opti
-0000b3a0: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
-0000b3b0: 2050 682d 7068 2069 6e74 6572 6163 7469   Ph-ph interacti
-0000b3c0: 6f6e 2073 7472 656e 6774 6820 6172 7261  on strength arra
-0000b3d0: 7920 6973 2072 6570 6c61 6365 6420 6279  y is replaced by
-0000b3e0: 2061 2073 6361 6c61 7220 7661 6c75 652e   a scalar value.
-0000b3f0: 0a20 2020 2020 2020 2020 2020 2044 6566  .            Def
-0000b400: 6175 6c74 2069 7320 4e6f 6e65 2c20 7768  ault is None, wh
-0000b410: 6963 6820 6d65 616e 7320 7468 6973 2066  ich means this f
-0000b420: 6561 7475 7265 2069 7320 6e6f 7420 7573  eature is not us
-0000b430: 6564 2e0a 2020 2020 2020 2020 6672 6571  ed..        freq
-0000b440: 7565 6e63 795f 7363 616c 655f 6661 6374  uency_scale_fact
-0000b450: 6f72 203a 2066 6c6f 6174 2c20 6f70 7469  or : float, opti
-0000b460: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
-0000b470: 2041 6c6c 2070 686f 6e6f 6e20 6672 6571   All phonon freq
-0000b480: 7565 6e63 6573 2061 7265 2073 6361 6c65  uences are scale
-0000b490: 6420 6279 2074 6869 7320 7661 6c75 652e  d by this value.
-0000b4a0: 2044 6566 6175 6c74 2069 7320 4e6f 6e65   Default is None
-0000b4b0: 2c0a 2020 2020 2020 2020 2020 2020 7768  ,.            wh
-0000b4c0: 6963 6820 6d65 616e 7320 7068 6f6e 6f6e  ich means phonon
-0000b4d0: 2066 7265 7175 656e 6369 6573 2061 7265   frequencies are
-0000b4e0: 206e 6f74 2073 6361 6c65 642e 0a20 2020   not scaled..   
-0000b4f0: 2020 2020 2073 796d 6d65 7472 697a 655f       symmetrize_
-0000b500: 6663 3371 203a 2062 6f6f 6c2c 206f 7074  fc3q : bool, opt
-0000b510: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
-0000b520: 2020 6663 3320 696e 2070 686f 6e6f 6e20    fc3 in phonon 
-0000b530: 7370 6163 6520 6973 2073 796d 6d65 7472  space is symmetr
-0000b540: 697a 6564 2062 7920 7065 726d 7574 6174  ized by permutat
-0000b550: 696f 6e20 7379 6d6d 6574 7279 2e0a 2020  ion symmetry..  
-0000b560: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-0000b570: 7420 6973 2046 616c 7365 2e0a 2020 2020  t is False..    
-0000b580: 2020 2020 6c61 7061 636b 5f7a 6865 6576      lapack_zheev
-0000b590: 5f75 706c 6f20 3a20 7374 722c 206f 7074  _uplo : str, opt
-0000b5a0: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
-0000b5b0: 2020 274c 2720 6f72 2027 5527 2e20 4465    'L' or 'U'. De
-0000b5c0: 6661 756c 7420 6973 2027 4c27 2e20 5468  fault is 'L'. Th
-0000b5d0: 6973 2069 7320 7061 7373 6564 2074 6f20  is is passed to 
-0000b5e0: 4c41 5041 434b 207a 6865 6576 0a20 2020  LAPACK zheev.   
-0000b5f0: 2020 2020 2020 2020 2075 7365 6420 666f           used fo
-0000b600: 7220 7068 6f6e 6f6e 2073 6f6c 7665 722e  r phonon solver.
-0000b610: 0a20 2020 2020 2020 206f 7065 6e6d 705f  .        openmp_
-0000b620: 7065 725f 7472 6970 6c65 7473 203a 2062  per_triplets : b
-0000b630: 6f6f 6c20 6f72 204e 6f6e 652c 206f 7074  ool or None, opt
-0000b640: 696f 6e61 6c2c 2064 6566 6175 6c74 2069  ional, default i
-0000b650: 7320 4e6f 6e65 0a20 2020 2020 2020 2020  s None.         
-0000b660: 2020 204e 6f72 6d61 6c6c 7920 7468 6973     Normally this
-0000b670: 2070 6172 616d 6574 6572 2073 686f 756c   parameter shoul
-0000b680: 6420 6e6f 7420 6265 2074 6f75 6368 6564  d not be touched
-0000b690: 2e0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
-0000b6a0: 656e 2060 5472 7565 602c 2070 682d 7068  en `True`, ph-ph
-0000b6b0: 2069 6e74 6572 6163 7469 6f6e 2073 7472   interaction str
-0000b6c0: 656e 6774 6820 6361 6c63 756c 6174 696f  ength calculatio
-0000b6d0: 6e20 7275 6e73 2077 6974 680a 2020 2020  n runs with.    
-0000b6e0: 2020 2020 2020 2020 4f70 656e 4d50 2064          OpenMP d
-0000b6f0: 6973 7472 6962 7574 696f 6e20 6f76 6572  istribution over
-0000b700: 2074 7269 706c 6574 732c 2061 6e64 206f   triplets, and o
-0000b710: 7665 7220 6261 6e64 7320 7768 656e 2060  ver bands when `
-0000b720: 4661 6c73 6560 2e0a 2020 2020 2020 2020  False`..        
-0000b730: 2020 2020 604e 6f6e 6560 2077 696c 6c20      `None` will 
-0000b740: 6368 6f6f 7365 206f 6e65 206f 6620 7468  choose one of th
-0000b750: 656d 2061 7574 6f6d 6174 6963 616c 6c79  em automatically
-0000b760: 2e0a 0a20 2020 2020 2020 2022 2222 0a20  ...        """. 
-0000b770: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
-0000b780: 6573 685f 6e75 6d62 6572 7320 6973 204e  esh_numbers is N
-0000b790: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000b7a0: 206d 7367 203d 2022 5068 6f6e 6f33 7079   msg = "Phono3py
-0000b7b0: 2e6d 6573 685f 6e75 6d62 6572 7320 6f66  .mesh_numbers of
-0000b7c0: 2069 6e73 7461 6e63 6520 6861 7320 746f   instance has to
-0000b7d0: 2062 6520 7365 742e 220a 2020 2020 2020   be set.".      
-0000b7e0: 2020 2020 2020 7261 6973 6520 5275 6e74        raise Runt
-0000b7f0: 696d 6545 7272 6f72 286d 7367 290a 0a20  imeError(msg).. 
-0000b800: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
-0000b810: 6663 3220 6973 204e 6f6e 653a 0a20 2020  fc2 is None:.   
-0000b820: 2020 2020 2020 2020 206d 7367 203d 2022           msg = "
-0000b830: 5068 6f6e 6f33 7079 2e66 6332 206f 6620  Phono3py.fc2 of 
-0000b840: 696e 7374 616e 6365 2069 7320 6e6f 7420  instance is not 
-0000b850: 666f 756e 642e 220a 2020 2020 2020 2020  found.".        
-0000b860: 2020 2020 7261 6973 6520 5275 6e74 696d      raise Runtim
-0000b870: 6545 7272 6f72 286d 7367 290a 0a20 2020  eError(msg)..   
-0000b880: 2020 2020 2073 656c 662e 5f69 6e74 6572       self._inter
-0000b890: 6163 7469 6f6e 203d 2049 6e74 6572 6163  action = Interac
-0000b8a0: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
-0000b8b0: 2020 7365 6c66 2e5f 7072 696d 6974 6976    self._primitiv
-0000b8c0: 652c 0a20 2020 2020 2020 2020 2020 2073  e,.            s
-0000b8d0: 656c 662e 5f62 7a5f 6772 6964 2c0a 2020  elf._bz_grid,.  
-0000b8e0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000b8f0: 7072 696d 6974 6976 655f 7379 6d6d 6574  primitive_symmet
-0000b900: 7279 2c0a 2020 2020 2020 2020 2020 2020  ry,.            
-0000b910: 6663 333d 7365 6c66 2e5f 6663 332c 0a20  fc3=self._fc3,. 
-0000b920: 2020 2020 2020 2020 2020 2062 616e 645f             band_
-0000b930: 696e 6469 6365 733d 7365 6c66 2e5f 6261  indices=self._ba
-0000b940: 6e64 5f69 6e64 6963 6573 5f66 6c61 7474  nd_indices_flatt
-0000b950: 656e 2c0a 2020 2020 2020 2020 2020 2020  en,.            
-0000b960: 636f 6e73 7461 6e74 5f61 7665 7261 6765  constant_average
-0000b970: 645f 696e 7465 7261 6374 696f 6e3d 636f  d_interaction=co
-0000b980: 6e73 7461 6e74 5f61 7665 7261 6765 645f  nstant_averaged_
-0000b990: 696e 7465 7261 6374 696f 6e2c 0a20 2020  interaction,.   
-0000b9a0: 2020 2020 2020 2020 2066 7265 7175 656e           frequen
-0000b9b0: 6379 5f66 6163 746f 725f 746f 5f54 487a  cy_factor_to_THz
-0000b9c0: 3d73 656c 662e 5f66 7265 7175 656e 6379  =self._frequency
-0000b9d0: 5f66 6163 746f 725f 746f 5f54 487a 2c0a  _factor_to_THz,.
-0000b9e0: 2020 2020 2020 2020 2020 2020 6672 6571              freq
-0000b9f0: 7565 6e63 795f 7363 616c 655f 6661 6374  uency_scale_fact
-0000ba00: 6f72 3d66 7265 7175 656e 6379 5f73 6361  or=frequency_sca
-0000ba10: 6c65 5f66 6163 746f 722c 0a20 2020 2020  le_factor,.     
-0000ba20: 2020 2020 2020 2063 7574 6f66 665f 6672         cutoff_fr
-0000ba30: 6571 7565 6e63 793d 7365 6c66 2e5f 6375  equency=self._cu
-0000ba40: 746f 6666 5f66 7265 7175 656e 6379 2c0a  toff_frequency,.
-0000ba50: 2020 2020 2020 2020 2020 2020 6973 5f6d              is_m
-0000ba60: 6573 685f 7379 6d6d 6574 7279 3d73 656c  esh_symmetry=sel
-0000ba70: 662e 5f69 735f 6d65 7368 5f73 796d 6d65  f._is_mesh_symme
-0000ba80: 7472 792c 0a20 2020 2020 2020 2020 2020  try,.           
-0000ba90: 2073 796d 6d65 7472 697a 655f 6663 3371   symmetrize_fc3q
-0000baa0: 3d73 796d 6d65 7472 697a 655f 6663 3371  =symmetrize_fc3q
-0000bab0: 2c0a 2020 2020 2020 2020 2020 2020 6d61  ,.            ma
-0000bac0: 6b65 5f72 305f 6176 6572 6167 653d 7365  ke_r0_average=se
-0000bad0: 6c66 2e5f 6d61 6b65 5f72 305f 6176 6572  lf._make_r0_aver
-0000bae0: 6167 652c 0a20 2020 2020 2020 2020 2020  age,.           
-0000baf0: 206c 6170 6163 6b5f 7a68 6565 765f 7570   lapack_zheev_up
-0000bb00: 6c6f 3d6c 6170 6163 6b5f 7a68 6565 765f  lo=lapack_zheev_
-0000bb10: 7570 6c6f 2c0a 2020 2020 2020 2020 2020  uplo,.          
-0000bb20: 2020 6f70 656e 6d70 5f70 6572 5f74 7269    openmp_per_tri
-0000bb30: 706c 6574 733d 6f70 656e 6d70 5f70 6572  plets=openmp_per
-0000bb40: 5f74 7269 706c 6574 732c 0a20 2020 2020  _triplets,.     
-0000bb50: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
-0000bb60: 662e 5f69 6e74 6572 6163 7469 6f6e 2e6e  f._interaction.n
-0000bb70: 6163 5f71 5f64 6972 6563 7469 6f6e 203d  ac_q_direction =
-0000bb80: 206e 6163 5f71 5f64 6972 6563 7469 6f6e   nac_q_direction
-0000bb90: 0a20 2020 2020 2020 2073 656c 662e 5f69  .        self._i
-0000bba0: 6e69 745f 6479 6e61 6d69 6361 6c5f 6d61  nit_dynamical_ma
-0000bbb0: 7472 6978 2829 0a0a 2020 2020 6465 6620  trix()..    def 
-0000bbc0: 7365 745f 7068 6f6e 6f6e 5f64 6174 6128  set_phonon_data(
-0000bbd0: 7365 6c66 2c20 6672 6571 7565 6e63 6965  self, frequencie
-0000bbe0: 732c 2065 6967 656e 7665 6374 6f72 732c  s, eigenvectors,
-0000bbf0: 2067 7269 645f 6164 6472 6573 7329 3a0a   grid_address):.
-0000bc00: 2020 2020 2020 2020 2222 2253 6574 2070          """Set p
-0000bc10: 686f 6e6f 6e20 6672 6571 7565 6e63 6965  honon frequencie
-0000bc20: 7320 616e 6420 6569 6765 6e76 6563 746f  s and eigenvecto
-0000bc30: 7273 2069 6e20 496e 7465 7261 6374 696f  rs in Interactio
-0000bc40: 6e20 696e 7374 616e 6365 2e0a 0a20 2020  n instance...   
-0000bc50: 2020 2020 2048 6172 6d6f 6e69 6320 7068       Harmonic ph
-0000bc60: 6f6e 6f6e 2069 6e66 6f72 6d61 7469 6f6e  onon information
-0000bc70: 2069 7320 7374 6f72 6564 2069 6e20 496e   is stored in In
-0000bc80: 7465 7261 6374 696f 6e20 696e 7374 616e  teraction instan
-0000bc90: 6365 2e20 466f 720a 2020 2020 2020 2020  ce. For.        
-0000bca0: 6578 616d 706c 652c 2074 6869 7320 696e  example, this in
-0000bcb0: 666f 726d 6174 696f 6e20 7374 6f72 6520  formation store 
-0000bcc0: 696e 2061 2066 696c 6520 6973 2072 6561  in a file is rea
-0000bcd0: 6420 616e 6420 7061 7373 6564 2074 6f0a  d and passed to.
-0000bce0: 2020 2020 2020 2020 5068 6f6e 6f33 7079          Phono3py
-0000bcf0: 2069 6e73 7461 6e63 6520 6279 2075 7369   instance by usi
-0000bd00: 6e67 2074 6869 7320 6d65 7468 6f64 2e20  ng this method. 
-0000bd10: 5468 6520 6772 6964 5f61 6464 7265 7373  The grid_address
-0000bd20: 2069 7320 7573 6564 0a20 2020 2020 2020   is used.       
-0000bd30: 2066 6f72 2074 6865 2063 6f6e 7369 7374   for the consist
-0000bd40: 656e 6379 2063 6865 636b 2e0a 0a20 2020  ency check...   
-0000bd50: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-0000bd60: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-0000bd70: 2d2d 0a20 2020 2020 2020 2066 7265 7175  --.        frequ
-0000bd80: 656e 6369 6573 203a 2061 7272 6179 5f6c  encies : array_l
-0000bd90: 696b 650a 2020 2020 2020 2020 2020 2020  ike.            
-0000bda0: 5068 6f6e 6f6e 2066 7265 7175 656e 6369  Phonon frequenci
-0000bdb0: 6573 2e0a 2020 2020 2020 2020 2020 2020  es..            
-0000bdc0: 7368 6170 653d 286e 756d 5f67 7269 645f  shape=(num_grid_
-0000bdd0: 706f 696e 7473 2c20 6e75 6d5f 6261 6e64  points, num_band
-0000bde0: 292c 2064 7479 7065 3d27 646f 7562 6c65  ), dtype='double
-0000bdf0: 272c 206f 7264 6572 3d27 4327 0a20 2020  ', order='C'.   
-0000be00: 2020 2020 2065 6967 656e 7665 6374 6f72       eigenvector
-0000be10: 7320 3a20 6172 7261 795f 6c69 6b65 0a20  s : array_like. 
-0000be20: 2020 2020 2020 2020 2020 2050 686f 6e6f             Phono
-0000be30: 6e20 6569 6765 6e76 6563 746f 7273 0a20  n eigenvectors. 
-0000be40: 2020 2020 2020 2020 2020 2073 6861 7065             shape
-0000be50: 3d28 6e75 6d5f 6772 6964 5f70 6f69 6e74  =(num_grid_point
-0000be60: 732c 206e 756d 5f62 616e 642c 206e 756d  s, num_band, num
-0000be70: 5f62 616e 6429 0a20 2020 2020 2020 2020  _band).         
-0000be80: 2020 2064 7479 7065 3d27 636f 6d70 6c65     dtype='comple
-0000be90: 7831 3238 272c 206f 7264 6572 3d27 4327  x128', order='C'
-0000bea0: 0a20 2020 2020 2020 2067 7269 645f 6164  .        grid_ad
-0000beb0: 6472 6573 7320 3a20 6172 7261 795f 6c69  dress : array_li
-0000bec0: 6b65 0a20 2020 2020 2020 2020 2020 2047  ke.            G
-0000bed0: 7269 6420 706f 696e 7420 6164 6472 6573  rid point addres
-0000bee0: 7365 7320 6279 2069 6e74 6567 6572 732e  ses by integers.
-0000bef0: 2054 6865 2066 6972 7374 2064 696d 656e   The first dimen
-0000bf00: 7369 6f6e 206d 6179 206e 6f74 2062 650a  sion may not be.
-0000bf10: 2020 2020 2020 2020 2020 2020 7072 6f64              prod
-0000bf20: 286d 6573 6829 2062 6563 6175 7365 2069  (mesh) because i
-0000bf30: 7420 696e 636c 7564 6573 2042 7269 6c6c  t includes Brill
-0000bf40: 6f75 696e 207a 6f6e 6520 626f 756e 6461  ouin zone bounda
-0000bf50: 7279 2e20 5468 6520 6465 7461 696c 0a20  ry. The detail. 
-0000bf60: 2020 2020 2020 2020 2020 2069 7320 666f             is fo
-0000bf70: 756e 6420 696e 2074 6865 2064 6f63 7374  und in the docst
-0000bf80: 7269 6e67 206f 660a 2020 2020 2020 2020  ring of.        
-0000bf90: 2020 2020 7068 6f6e 6f33 7079 2e70 686f      phono3py.pho
-0000bfa0: 6e6f 6e33 2e74 7269 706c 6574 732e 6765  non3.triplets.ge
-0000bfb0: 745f 7472 6970 6c65 7473 5f61 745f 712e  t_triplets_at_q.
-0000bfc0: 0a20 2020 2020 2020 2020 2020 2073 6861  .            sha
-0000bfd0: 7065 3d28 6e75 6d5f 6772 6964 5f70 6f69  pe=(num_grid_poi
-0000bfe0: 6e74 732c 2033 292c 2064 7479 7065 3d69  nts, 3), dtype=i
-0000bff0: 6e74 0a0a 2020 2020 2020 2020 2222 220a  nt..        """.
-0000c000: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000c010: 5f69 6e74 6572 6163 7469 6f6e 2069 7320  _interaction is 
-0000c020: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0000c030: 2020 2020 2020 7365 6c66 2e5f 696e 7465        self._inte
-0000c040: 7261 6374 696f 6e2e 7365 745f 7068 6f6e  raction.set_phon
-0000c050: 6f6e 5f64 6174 6128 6672 6571 7565 6e63  on_data(frequenc
-0000c060: 6965 732c 2065 6967 656e 7665 6374 6f72  ies, eigenvector
-0000c070: 732c 2067 7269 645f 6164 6472 6573 7329  s, grid_address)
-0000c080: 0a0a 2020 2020 6465 6620 6765 745f 7068  ..    def get_ph
-0000c090: 6f6e 6f6e 5f64 6174 6128 7365 6c66 293a  onon_data(self):
-0000c0a0: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
-0000c0b0: 7068 6f6e 6f6e 2066 7265 7175 656e 6369  phonon frequenci
-0000c0c0: 6573 2061 6e64 2065 6967 656e 7665 6374  es and eigenvect
-0000c0d0: 6f72 7320 696e 2049 6e74 6572 6163 7469  ors in Interacti
-0000c0e0: 6f6e 2069 6e73 7461 6e63 652e 0a0a 2020  on instance...  
-0000c0f0: 2020 2020 2020 4861 726d 6f6e 6963 2070        Harmonic p
-0000c100: 686f 6e6f 6e20 696e 666f 726d 6174 696f  honon informatio
-0000c110: 6e20 6973 2073 746f 7265 6420 696e 2049  n is stored in I
-0000c120: 6e74 6572 6163 7469 6f6e 2069 6e73 7461  nteraction insta
-0000c130: 6e63 652e 2054 6869 730a 2020 2020 2020  nce. This.      
-0000c140: 2020 696e 666f 726d 6174 696f 6e20 6361    information ca
-0000c150: 6e20 6265 206f 6274 6169 6e65 642e 2054  n be obtained. T
-0000c160: 6865 2067 7269 645f 6164 6472 6573 7320  he grid_address 
-0000c170: 7265 7475 726e 6564 2067 6976 6520 7468  returned give th
-0000c180: 650a 2020 2020 2020 2020 712d 706f 696e  e.        q-poin
-0000c190: 7473 206c 6f63 6174 696f 6e73 2077 6974  ts locations wit
-0000c1a0: 6820 7265 7370 6563 7420 746f 2072 6563  h respect to rec
-0000c1b0: 6970 726f 6361 6c20 6261 7369 7320 7665  iprocal basis ve
-0000c1c0: 6374 6f72 7320 6279 0a20 2020 2020 2020  ctors by.       
-0000c1d0: 2069 6e74 6567 6572 7320 696e 2074 6865   integers in the
-0000c1e0: 2077 6179 2074 6861 740a 2020 2020 2020   way that.      
-0000c1f0: 2020 2020 2020 715f 706f 696e 7473 203d        q_points =
-0000c200: 2067 7269 645f 6164 6472 6573 7320 2f20   grid_address / 
-0000c210: 6e70 2e61 7272 6179 286d 6573 682c 2064  np.array(mesh, d
-0000c220: 7479 7065 3d27 646f 7562 6c65 2729 2e0a  type='double')..
-0000c230: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-0000c240: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-0000c250: 0a20 2020 2020 2020 2074 7570 6c65 0a20  .        tuple. 
-0000c260: 2020 2020 2020 2020 2020 2028 6672 6571             (freq
-0000c270: 7565 6e63 6965 732c 2065 6967 656e 7665  uencies, eigenve
-0000c280: 6374 6f72 732c 2067 7269 645f 6164 6472  ctors, grid_addr
-0000c290: 6573 7329 0a20 2020 2020 2020 2020 2020  ess).           
-0000c2a0: 2053 6565 206d 6f72 6520 6465 7461 696c   See more detail
-0000c2b0: 7320 6174 2074 6865 2064 6f63 7374 7269  s at the docstri
-0000c2c0: 6e67 206f 6620 7365 745f 7068 6f6e 6f6e  ng of set_phonon
-0000c2d0: 5f64 6174 612e 0a0a 2020 2020 2020 2020  _data...        
-0000c2e0: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
-0000c2f0: 656c 662e 5f69 6e74 6572 6163 7469 6f6e  elf._interaction
-0000c300: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000c310: 2020 2020 2020 2020 2020 6672 6571 732c            freqs,
-0000c320: 2065 6967 7665 6373 2c20 5f20 3d20 7365   eigvecs, _ = se
-0000c330: 6c66 2e5f 696e 7465 7261 6374 696f 6e2e  lf._interaction.
-0000c340: 6765 745f 7068 6f6e 6f6e 7328 290a 2020  get_phonons().  
-0000c350: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000c360: 2066 7265 7173 2c20 6569 6776 6563 732c   freqs, eigvecs,
-0000c370: 2073 656c 662e 5f69 6e74 6572 6163 7469   self._interacti
-0000c380: 6f6e 2e62 7a5f 6772 6964 2e61 6464 7265  on.bz_grid.addre
-0000c390: 7373 6573 0a20 2020 2020 2020 2065 6c73  sses.        els
-0000c3a0: 653a 0a20 2020 2020 2020 2020 2020 206d  e:.            m
-0000c3b0: 7367 203d 2028 0a20 2020 2020 2020 2020  sg = (.         
-0000c3c0: 2020 2020 2020 2022 5068 6f6e 6f33 7079         "Phono3py
-0000c3d0: 2e69 6e69 745f 7068 7068 5f69 6e74 6572  .init_phph_inter
-0000c3e0: 6163 7469 6f6e 2068 6173 2074 6f20 6265  action has to be
-0000c3f0: 2063 616c 6c65 6420 220a 2020 2020 2020   called ".      
-0000c400: 2020 2020 2020 2020 2020 2262 6566 6f72            "befor
-0000c410: 6520 7275 6e6e 696e 6720 7468 6973 206d  e running this m
-0000c420: 6574 686f 642e 220a 2020 2020 2020 2020  ethod.".        
-0000c430: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000c440: 2020 7261 6973 6520 5275 6e74 696d 6545    raise RuntimeE
-0000c450: 7272 6f72 286d 7367 290a 0a20 2020 2064  rror(msg)..    d
-0000c460: 6566 2072 756e 5f70 686f 6e6f 6e5f 736f  ef run_phonon_so
-0000c470: 6c76 6572 2873 656c 662c 2067 7269 645f  lver(self, grid_
-0000c480: 706f 696e 7473 3d4e 6f6e 6529 3a0a 2020  points=None):.  
-0000c490: 2020 2020 2020 2222 2252 756e 2068 6172        """Run har
-0000c4a0: 6d6f 6e69 6320 7068 6f6e 6f6e 2063 616c  monic phonon cal
-0000c4b0: 6375 6c61 7469 6f6e 206f 6e20 6772 6964  culation on grid
-0000c4c0: 2070 6f69 6e74 732e 0a0a 2020 2020 2020   points...      
-0000c4d0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-0000c4e0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
-0000c4f0: 2020 2020 2020 2020 6772 6964 5f70 6f69          grid_poi
-0000c500: 6e74 7320 3a20 6172 7261 795f 6c69 6b65  nts : array_like
-0000c510: 206f 7220 4e6f 6e65 2c20 6f70 7469 6f6e   or None, option
-0000c520: 616c 0a20 2020 2020 2020 2020 2020 2041  al.            A
-0000c530: 206c 6973 7420 6f66 2067 7269 6420 706f   list of grid po
-0000c540: 696e 7420 696e 6469 6365 7320 6f66 2050  int indices of P
-0000c550: 686f 6e6f 3370 792e 6772 6964 2e61 6464  hono3py.grid.add
-0000c560: 7265 7373 6573 2e0a 2020 2020 2020 2020  resses..        
-0000c570: 2020 2020 5370 6563 6966 7969 6e67 204e      Specifying N
-0000c580: 6f6e 6520 7275 6e73 2061 6c6c 2070 686f  one runs all pho
-0000c590: 6e6f 6e73 206f 6e20 7468 6520 6772 6964  nons on the grid
-0000c5a0: 2070 6f69 6e74 7320 756e 6c65 7373 0a20   points unless. 
-0000c5b0: 2020 2020 2020 2020 2020 2074 686f 7365             those
-0000c5c0: 2070 686f 6e6f 6e73 2077 6572 6520 616c   phonons were al
-0000c5d0: 7265 6164 7920 6361 6c63 756c 6174 6564  ready calculated
-0000c5e0: 2e20 4e6f 726d 616c 6c79 2070 686f 6e6f  . Normally phono
-0000c5f0: 6e73 2061 740a 2020 2020 2020 2020 2020  ns at.          
-0000c600: 2020 5b30 2c20 302c 2030 5d20 706f 696e    [0, 0, 0] poin
-0000c610: 7420 6973 2061 6c72 6561 6479 2063 616c  t is already cal
-0000c620: 6375 6c61 7465 6420 6265 666f 7265 2063  culated before c
-0000c630: 616c 6c69 6e67 2074 6869 7320 6d65 7468  alling this meth
-0000c640: 6f64 2e0a 2020 2020 2020 2020 2020 2020  od..            
-0000c650: 5068 6f6e 6f6e 2063 616c 6375 6c61 7469  Phonon calculati
-0000c660: 6f6e 7320 6172 6520 7065 7266 6f72 6d65  ons are performe
-0000c670: 6420 6175 746f 6d61 7469 6361 6c6c 7920  d automatically 
-0000c680: 7768 656e 206e 6565 6465 640a 2020 2020  when needed.    
-0000c690: 2020 2020 2020 2020 696e 7465 726e 616c          internal
-0000c6a0: 6c79 2066 6f72 2070 682d 7068 2063 616c  ly for ph-ph cal
-0000c6b0: 6375 6c61 7469 6f6e 2e20 5468 6572 6566  culation. Theref
-0000c6c0: 6f72 6520 6361 6c6c 696e 6720 7468 6973  ore calling this
-0000c6d0: 206d 6574 686f 640a 2020 2020 2020 2020   method.        
-0000c6e0: 2020 2020 6973 206e 6f74 206e 6563 6573      is not neces
-0000c6f0: 7361 7279 2069 6e20 6d6f 7374 2063 6173  sary in most cas
-0000c700: 6573 2e0a 2020 2020 2020 2020 2020 2020  es..            
-0000c710: 5468 6520 7068 6f6e 6f6e 2072 6573 756c  The phonon resul
-0000c720: 7473 2061 7265 206f 6274 6169 6e65 6420  ts are obtained 
-0000c730: 6279 2050 686f 6e6f 3370 792e 6765 745f  by Phono3py.get_
-0000c740: 7068 6f6e 6f6e 5f64 6174 6128 292e 0a0a  phonon_data()...
-0000c750: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000c760: 2020 2020 6966 2073 656c 662e 5f69 6e74      if self._int
-0000c770: 6572 6163 7469 6f6e 2069 7320 6e6f 7420  eraction is not 
-0000c780: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000c790: 2020 7365 6c66 2e5f 696e 7465 7261 6374    self._interact
-0000c7a0: 696f 6e2e 7275 6e5f 7068 6f6e 6f6e 5f73  ion.run_phonon_s
-0000c7b0: 6f6c 7665 7228 6772 6964 5f70 6f69 6e74  olver(grid_point
-0000c7c0: 733d 6772 6964 5f70 6f69 6e74 7329 0a20  s=grid_points). 
-0000c7d0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000c7e0: 2020 2020 2020 2020 206d 7367 203d 2028           msg = (
-0000c7f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c800: 2022 5068 6f6e 6f33 7079 2e69 6e69 745f   "Phono3py.init_
-0000c810: 7068 7068 5f69 6e74 6572 6163 7469 6f6e  phph_interaction
-0000c820: 2068 6173 2074 6f20 6265 2063 616c 6c65   has to be calle
-0000c830: 6420 220a 2020 2020 2020 2020 2020 2020  d ".            
-0000c840: 2020 2020 2262 6566 6f72 6520 7275 6e6e      "before runn
-0000c850: 696e 6720 7468 6973 206d 6574 686f 642e  ing this method.
-0000c860: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
-0000c870: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000c880: 6520 5275 6e74 696d 6545 7272 6f72 286d  e RuntimeError(m
-0000c890: 7367 290a 0a20 2020 2064 6566 2067 656e  sg)..    def gen
-0000c8a0: 6572 6174 655f 6469 7370 6c61 6365 6d65  erate_displaceme
-0000c8b0: 6e74 7328 0a20 2020 2020 2020 2073 656c  nts(.        sel
-0000c8c0: 662c 0a20 2020 2020 2020 2064 6973 7461  f,.        dista
-0000c8d0: 6e63 653d 302e 3033 2c0a 2020 2020 2020  nce=0.03,.      
-0000c8e0: 2020 6375 746f 6666 5f70 6169 725f 6469    cutoff_pair_di
-0000c8f0: 7374 616e 6365 3d4e 6f6e 652c 0a20 2020  stance=None,.   
-0000c900: 2020 2020 2069 735f 706c 7573 6d69 6e75       is_plusminu
-0000c910: 733d 2261 7574 6f22 2c0a 2020 2020 2020  s="auto",.      
-0000c920: 2020 6973 5f64 6961 676f 6e61 6c3d 5472    is_diagonal=Tr
-0000c930: 7565 2c0a 2020 2020 293a 0a20 2020 2020  ue,.    ):.     
-0000c940: 2020 2022 2222 4765 6e65 7261 7465 2064     """Generate d
-0000c950: 6973 706c 6163 656d 656e 7420 6461 7461  isplacement data
-0000c960: 7365 7420 696e 2073 7570 6572 6365 6c6c  set in supercell
-0000c970: 2066 6f72 2066 6333 2e0a 0a20 2020 2020   for fc3...     
-0000c980: 2020 2054 6869 7320 7379 7374 656d 6174     This systemat
-0000c990: 6963 616c 6c79 2067 656e 6572 6174 6573  ically generates
-0000c9a0: 2073 696e 676c 6520 616e 6420 7061 6972   single and pair
-0000c9b0: 2061 746f 6d69 6320 6469 7370 6c61 6365   atomic displace
-0000c9c0: 6d65 6e74 730a 2020 2020 2020 2020 696e  ments.        in
-0000c9d0: 2073 7570 6572 6365 6c6c 7320 746f 2063   supercells to c
-0000c9e0: 616c 6375 6c61 7465 2066 6333 2063 6f6e  alculate fc3 con
-0000c9f0: 7369 6465 7269 6e67 2063 7279 7374 616c  sidering crystal
-0000ca00: 2073 796d 6d65 7472 792e 0a20 2020 2020   symmetry..     
-0000ca10: 2020 2057 6865 6e20 7468 6973 206d 6574     When this met
-0000ca20: 686f 6420 6973 2063 616c 6c65 642c 2065  hod is called, e
-0000ca30: 7869 7374 696e 6720 6361 6368 6520 6f66  xisting cache of
-0000ca40: 2073 7570 6572 6365 6c6c 7320 7769 7468   supercells with
-0000ca50: 0a20 2020 2020 2020 2064 6973 706c 6163  .        displac
-0000ca60: 656d 656e 7473 2066 6f72 2066 6333 2061  ements for fc3 a
-0000ca70: 7265 2072 656d 6f76 6564 2e0a 0a20 2020  re removed...   
-0000ca80: 2020 2020 2046 6f72 2066 6333 2c20 7477       For fc3, tw
-0000ca90: 6f20 6174 6f6d 7320 6172 6520 6469 7370  o atoms are disp
-0000caa0: 6c61 6365 6420 666f 7220 6561 6368 2063  laced for each c
-0000cab0: 6f6e 6669 6775 7261 7469 6f6e 0a20 2020  onfiguration.   
-0000cac0: 2020 2020 2063 6f6e 7369 6465 7269 6e67       considering
-0000cad0: 2063 7279 7374 616c 2073 796d 6d65 7472   crystal symmetr
-0000cae0: 792e 2054 6865 2066 6972 7374 2064 6973  y. The first dis
-0000caf0: 706c 6163 656d 656e 7420 6973 2063 686f  placement is cho
-0000cb00: 7365 6e0a 2020 2020 2020 2020 696e 2074  sen.        in t
-0000cb10: 6865 2070 6572 6665 6374 2073 7570 6572  he perfect super
-0000cb20: 6365 6c6c 2c20 616e 6420 7468 6520 7365  cell, and the se
-0000cb30: 636f 6e64 2064 6973 706c 6163 656d 656e  cond displacemen
-0000cb40: 7420 696e 2074 6865 0a20 2020 2020 2020  t in the.       
-0000cb50: 2064 6973 706c 6163 6564 2073 7570 6572   displaced super
-0000cb60: 6365 6c6c 2e20 5468 6520 6669 7273 7420  cell. The first 
-0000cb70: 6469 7370 6c61 6365 6d65 6e74 7320 6172  displacements ar
-0000cb80: 6520 7461 6b65 6e20 616c 6f6e 670a 2020  e taken along.  
-0000cb90: 2020 2020 2020 7468 6520 6261 7369 7320        the basis 
-0000cba0: 7665 6374 6f72 7320 6f66 2074 6865 2073  vectors of the s
-0000cbb0: 7570 6572 6365 6c6c 2e20 5468 6973 2069  upercell. This i
-0000cbc0: 7320 6265 6361 7573 6520 7468 650a 2020  s because the.  
-0000cbd0: 2020 2020 2020 7379 6d6d 6574 7279 2069        symmetry i
-0000cbe0: 7320 6578 7065 6374 6564 2074 6f20 6265  s expected to be
-0000cbf0: 206c 6573 7320 6272 6f6b 656e 2062 7920   less broken by 
-0000cc00: 7468 6520 696e 7472 6f64 7563 6564 2066  the introduced f
-0000cc10: 6972 7374 0a20 2020 2020 2020 2064 6973  irst.        dis
-0000cc20: 706c 6163 656d 656e 742c 2061 6e64 2061  placement, and a
-0000cc30: 7320 7468 6520 7265 7375 6c74 2c20 7468  s the result, th
-0000cc40: 6520 6e75 6d62 6572 206f 6620 7365 636f  e number of seco
-0000cc50: 6e64 0a20 2020 2020 2020 2064 6973 706c  nd.        displ
-0000cc60: 6163 656d 656e 7473 206d 6179 2062 6563  acements may bec
-0000cc70: 6f6d 6520 736d 616c 6c65 7220 7468 616e  ome smaller than
-0000cc80: 2074 6865 2063 6173 6520 7468 6174 2074   the case that t
-0000cc90: 6865 2066 6972 7374 0a20 2020 2020 2020  he first.       
-0000cca0: 2061 746f 6d20 6973 2064 6973 706c 6163   atom is displac
-0000ccb0: 6564 206e 6f74 2061 6c6f 6e67 2074 6865  ed not along the
-0000ccc0: 2062 6173 6973 2076 6563 746f 7273 2e0a   basis vectors..
-0000ccd0: 0a20 2020 2020 2020 204e 6f74 650a 2020  .        Note.  
-0000cce0: 2020 2020 2020 2d2d 2d2d 0a20 2020 2020        ----.     
-0000ccf0: 2020 2057 6865 6e20 7068 6f6e 6f6e 5f73     When phonon_s
-0000cd00: 7570 6572 6365 6c6c 5f6d 6174 7269 7820  upercell_matrix 
-0000cd10: 6973 206e 6f74 2067 6976 656e 2c20 6663  is not given, fc
-0000cd20: 3220 6973 2061 6c73 6f0a 2020 2020 2020  2 is also.      
-0000cd30: 2020 636f 6d70 7574 6564 2066 726f 6d20    computed from 
-0000cd40: 7468 6520 7361 6d65 2073 6574 206f 6620  the same set of 
-0000cd50: 7468 6520 6469 7370 6c61 6365 6d65 6e74  the displacement
-0000cd60: 7320 666f 7220 6663 3320 616e 640a 2020  s for fc3 and.  
-0000cd70: 2020 2020 2020 7265 7370 6563 7469 7665        respective
-0000cd80: 2073 7570 6572 6365 6c6c 2066 6f72 6365   supercell force
-0000cd90: 732e 2057 6865 6e20 7068 6f6e 6f6e 5f73  s. When phonon_s
-0000cda0: 7570 6572 6365 6c6c 5f6d 6174 7269 7820  upercell_matrix 
-0000cdb0: 6973 0a20 2020 2020 2020 2073 6574 2c20  is.        set, 
-0000cdc0: 7468 6520 6469 7370 6c61 6365 6d65 6e74  the displacement
-0000cdd0: 7320 696e 2070 686f 6e6f 6e5f 7375 7065  s in phonon_supe
-0000cde0: 7263 656c 6c20 6172 6520 6765 6e65 7261  rcell are genera
-0000cdf0: 7465 6420 756e 6c65 7373 0a20 2020 2020  ted unless.     
-0000ce00: 2020 2074 686f 7365 2061 6c72 6561 6479     those already
-0000ce10: 2065 7869 7374 2e0a 0a20 2020 2020 2020   exist...       
-0000ce20: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-0000ce30: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-0000ce40: 2020 2020 2020 2064 6973 7461 6e63 6520         distance 
-0000ce50: 3a20 666c 6f61 742c 206f 7074 696f 6e61  : float, optiona
-0000ce60: 6c0a 2020 2020 2020 2020 2020 2020 436f  l.            Co
-0000ce70: 6e73 7461 6e74 2064 6973 706c 6163 656d  nstant displacem
-0000ce80: 656e 7420 4575 636c 6964 6561 6e20 6469  ent Euclidean di
-0000ce90: 7374 616e 6365 2e20 4465 6661 756c 7420  stance. Default 
-0000cea0: 6973 2030 2e30 332e 0a20 2020 2020 2020  is 0.03..       
-0000ceb0: 2063 7574 6f66 665f 7061 6972 5f64 6973   cutoff_pair_dis
-0000cec0: 7461 6e63 6520 3a20 666c 6f61 742c 206f  tance : float, o
-0000ced0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-0000cee0: 2020 2020 5468 6973 2069 7320 7573 6564      This is used
-0000cef0: 2061 7320 6120 6375 746f 6666 2045 7563   as a cutoff Euc
-0000cf00: 6c69 6465 616e 2064 6973 7461 6e63 6520  lidean distance 
-0000cf10: 746f 2064 6574 6572 6d69 6e65 2069 660a  to determine if.
-0000cf20: 2020 2020 2020 2020 2020 2020 6561 6368              each
-0000cf30: 2070 6169 7220 6f66 2064 6973 706c 6163   pair of displac
-0000cf40: 656d 656e 7473 2069 7320 636f 6e73 6964  ements is consid
-0000cf50: 6572 6564 2074 6f20 6361 6c63 756c 6174  ered to calculat
-0000cf60: 6520 6663 3320 6f72 206e 6f74 2e0a 2020  e fc3 or not..  
-0000cf70: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-0000cf80: 7420 6973 204e 6f6e 652c 2077 6869 6368  t is None, which
-0000cf90: 206d 6561 6e73 2063 7574 6f66 6620 6973   means cutoff is
-0000cfa0: 206e 6f74 2075 7365 642e 0a20 2020 2020   not used..     
-0000cfb0: 2020 2069 735f 706c 7573 6d69 6e75 7320     is_plusminus 
-0000cfc0: 3a20 5472 7565 2c20 4661 6c73 652c 206f  : True, False, o
-0000cfd0: 7220 2761 7574 6f27 2c20 6f70 7469 6f6e  r 'auto', option
-0000cfe0: 616c 0a20 2020 2020 2020 2020 2020 2057  al.            W
-0000cff0: 6974 6820 5472 7565 2c20 6174 6f6d 6973  ith True, atomis
-0000d000: 2061 7265 2064 6973 706c 6163 6564 2069   are displaced i
-0000d010: 6e20 626f 7468 2070 6f73 6974 6976 6520  n both positive 
-0000d020: 616e 6420 6e65 6761 7469 7665 0a20 2020  and negative.   
-0000d030: 2020 2020 2020 2020 2064 6972 6563 7469           directi
-0000d040: 6f6e 732e 2057 6974 6820 4661 6c73 652c  ons. With False,
-0000d050: 206f 6e6c 7920 6f6e 6520 6469 7265 6374   only one direct
-0000d060: 696f 6e2e 2057 6974 6820 2761 7574 6f27  ion. With 'auto'
-0000d070: 2c0a 2020 2020 2020 2020 2020 2020 6d6f  ,.            mo
-0000d080: 7374 6c79 2065 7175 6976 616c 656e 7420  stly equivalent 
-0000d090: 746f 2069 735f 706c 7573 6d69 6e75 733d  to is_plusminus=
-0000d0a0: 5472 7565 2c20 6275 7420 6f6e 6c79 206f  True, but only o
-0000d0b0: 6e65 2064 6972 6563 7469 6f6e 0a20 2020  ne direction.   
-0000d0c0: 2020 2020 2020 2020 2069 7320 6368 6f73           is chos
-0000d0d0: 656e 2077 6865 6e20 7468 6520 6469 7370  en when the disp
-0000d0e0: 6c61 6365 6d65 6e74 7320 696e 2062 6f74  lacements in bot
-0000d0f0: 6820 6469 7265 6374 696f 6e73 2061 7265  h directions are
-0000d100: 0a20 2020 2020 2020 2020 2020 2073 796d  .            sym
-0000d110: 6d65 7472 6963 616c 6c79 2065 7175 6976  metrically equiv
-0000d120: 616c 656e 742e 2044 6566 6175 6c74 2069  alent. Default i
-0000d130: 7320 2761 7574 6f27 2e0a 2020 2020 2020  s 'auto'..      
-0000d140: 2020 6973 5f64 6961 676f 6e61 6c20 3a20    is_diagonal : 
-0000d150: 426f 6f6c 2c20 6f70 7469 6f6e 616c 0a20  Bool, optional. 
-0000d160: 2020 2020 2020 2020 2020 2057 6974 6820             With 
-0000d170: 4661 6c73 652c 2074 6865 2073 6563 6f6e  False, the secon
-0000d180: 6420 6469 7370 6c61 6365 6d65 6e74 7320  d displacements 
-0000d190: 6172 6520 6d61 6465 2061 6c6f 6e67 2074  are made along t
-0000d1a0: 6865 2062 6173 6973 0a20 2020 2020 2020  he basis.       
-0000d1b0: 2020 2020 2076 6563 746f 7273 206f 6620       vectors of 
-0000d1c0: 7468 6520 7375 7065 7263 656c 6c2e 2057  the supercell. W
-0000d1d0: 6974 6820 5472 7565 2c20 6469 7265 6374  ith True, direct
-0000d1e0: 696f 6e20 6e6f 7420 616c 6f6e 6720 7468  ion not along th
-0000d1f0: 6520 6261 7369 730a 2020 2020 2020 2020  e basis.        
-0000d200: 2020 2020 7665 6374 6f72 7320 6361 6e20      vectors can 
-0000d210: 6265 2063 686f 7365 6e20 7768 656e 2074  be chosen when t
-0000d220: 6865 206e 756d 6265 7220 6f66 2074 6865  he number of the
-0000d230: 2064 6973 706c 6163 656d 656e 7473 0a20   displacements. 
-0000d240: 2020 2020 2020 2020 2020 206d 6179 2062             may b
-0000d250: 6520 7265 6475 6365 642e 0a0a 2020 2020  e reduced...    
-0000d260: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000d270: 6469 7265 6374 696f 6e5f 6461 7461 7365  direction_datase
-0000d280: 7420 3d20 6765 745f 7468 6972 645f 6f72  t = get_third_or
-0000d290: 6465 725f 6469 7370 6c61 6365 6d65 6e74  der_displacement
-0000d2a0: 7328 0a20 2020 2020 2020 2020 2020 2073  s(.            s
-0000d2b0: 656c 662e 5f73 7570 6572 6365 6c6c 2c0a  elf._supercell,.
-0000d2c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d2d0: 2e5f 7379 6d6d 6574 7279 2c0a 2020 2020  ._symmetry,.    
-0000d2e0: 2020 2020 2020 2020 6973 5f70 6c75 736d          is_plusm
-0000d2f0: 696e 7573 3d69 735f 706c 7573 6d69 6e75  inus=is_plusminu
-0000d300: 732c 0a20 2020 2020 2020 2020 2020 2069  s,.            i
-0000d310: 735f 6469 6167 6f6e 616c 3d69 735f 6469  s_diagonal=is_di
-0000d320: 6167 6f6e 616c 2c0a 2020 2020 2020 2020  agonal,.        
-0000d330: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
-0000d340: 6461 7461 7365 7420 3d20 6469 7265 6374  dataset = direct
-0000d350: 696f 6e5f 746f 5f64 6973 706c 6163 656d  ion_to_displacem
-0000d360: 656e 7428 0a20 2020 2020 2020 2020 2020  ent(.           
-0000d370: 2064 6972 6563 7469 6f6e 5f64 6174 6173   direction_datas
-0000d380: 6574 2c0a 2020 2020 2020 2020 2020 2020  et,.            
-0000d390: 6469 7374 616e 6365 2c0a 2020 2020 2020  distance,.      
-0000d3a0: 2020 2020 2020 7365 6c66 2e5f 7375 7065        self._supe
-0000d3b0: 7263 656c 6c2c 0a20 2020 2020 2020 2020  rcell,.         
-0000d3c0: 2020 2063 7574 6f66 665f 6469 7374 616e     cutoff_distan
-0000d3d0: 6365 3d63 7574 6f66 665f 7061 6972 5f64  ce=cutoff_pair_d
-0000d3e0: 6973 7461 6e63 652c 0a20 2020 2020 2020  istance,.       
-0000d3f0: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
-0000d400: 5f73 7570 6572 6365 6c6c 735f 7769 7468  _supercells_with
-0000d410: 5f64 6973 706c 6163 656d 656e 7473 203d  _displacements =
-0000d420: 204e 6f6e 650a 0a20 2020 2020 2020 2069   None..        i
-0000d430: 6620 7365 6c66 2e5f 7068 6f6e 6f6e 5f73  f self._phonon_s
-0000d440: 7570 6572 6365 6c6c 5f6d 6174 7269 7820  upercell_matrix 
-0000d450: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
-0000d460: 7365 6c66 2e5f 7068 6f6e 6f6e 5f64 6174  self._phonon_dat
-0000d470: 6173 6574 2069 7320 4e6f 6e65 3a0a 2020  aset is None:.  
-0000d480: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
-0000d490: 656e 6572 6174 655f 6663 325f 6469 7370  enerate_fc2_disp
-0000d4a0: 6c61 6365 6d65 6e74 7328 0a20 2020 2020  lacements(.     
-0000d4b0: 2020 2020 2020 2020 2020 2064 6973 7461             dista
-0000d4c0: 6e63 653d 6469 7374 616e 6365 2c20 6973  nce=distance, is
-0000d4d0: 5f70 6c75 736d 696e 7573 3d69 735f 706c  _plusminus=is_pl
-0000d4e0: 7573 6d69 6e75 732c 2069 735f 6469 6167  usminus, is_diag
-0000d4f0: 6f6e 616c 3d46 616c 7365 0a20 2020 2020  onal=False.     
-0000d500: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-0000d510: 6620 6765 6e65 7261 7465 5f66 6332 5f64  f generate_fc2_d
-0000d520: 6973 706c 6163 656d 656e 7473 280a 2020  isplacements(.  
-0000d530: 2020 2020 2020 7365 6c66 2c20 6469 7374        self, dist
-0000d540: 616e 6365 3d30 2e30 332c 2069 735f 706c  ance=0.03, is_pl
-0000d550: 7573 6d69 6e75 733d 2261 7574 6f22 2c20  usminus="auto", 
-0000d560: 6973 5f64 6961 676f 6e61 6c3d 4661 6c73  is_diagonal=Fals
-0000d570: 650a 2020 2020 293a 0a20 2020 2020 2020  e.    ):.       
-0000d580: 2022 2222 4765 6e65 7261 7465 2064 6973   """Generate dis
-0000d590: 706c 6163 656d 656e 7420 6461 7461 7365  placement datase
-0000d5a0: 7420 696e 2070 686f 6e6f 6e20 7375 7065  t in phonon supe
-0000d5b0: 7263 656c 6c20 666f 7220 6663 322e 0a0a  rcell for fc2...
-0000d5c0: 2020 2020 2020 2020 5468 6973 2073 7973          This sys
-0000d5d0: 7465 6d61 7469 6361 6c6c 7920 6765 6e65  tematically gene
-0000d5e0: 7261 7465 7320 7369 6e67 6c65 2061 746f  rates single ato
-0000d5f0: 6d69 6320 6469 7370 6c61 6365 6d65 6e74  mic displacement
-0000d600: 730a 2020 2020 2020 2020 696e 2073 7570  s.        in sup
-0000d610: 6572 6365 6c6c 7320 746f 2063 616c 6375  ercells to calcu
-0000d620: 6c61 7465 2070 686f 6e6f 6e5f 6663 3220  late phonon_fc2 
-0000d630: 636f 6e73 6964 6572 696e 6720 6372 7973  considering crys
-0000d640: 7461 6c20 7379 6d6d 6574 7279 2e0a 2020  tal symmetry..  
-0000d650: 2020 2020 2020 5768 656e 2074 6869 7320        When this 
-0000d660: 6d65 7468 6f64 2069 7320 6361 6c6c 6564  method is called
-0000d670: 2c20 6578 6973 7469 6e67 2063 6163 6865  , existing cache
-0000d680: 206f 6620 7375 7065 7263 656c 6c73 2077   of supercells w
-0000d690: 6974 680a 2020 2020 2020 2020 6469 7370  ith.        disp
-0000d6a0: 6c61 6365 6d65 6e74 7320 666f 7220 6663  lacements for fc
-0000d6b0: 3220 6172 6520 7265 6d6f 7665 642e 0a0a  2 are removed...
-0000d6c0: 2020 2020 2020 2020 4e6f 7465 0a20 2020          Note.   
-0000d6d0: 2020 2020 202d 2d2d 2d0a 2020 2020 2020       ----.      
-0000d6e0: 2020 6973 5f64 6961 676f 6e61 6c3d 4661    is_diagonal=Fa
-0000d6f0: 6c73 6520 6973 2063 686f 7365 6e20 6173  lse is chosen as
-0000d700: 2074 6865 2064 6566 6175 6c74 2073 6574   the default set
-0000d710: 7469 6e67 2069 6e74 656e 7469 6f6e 616c  ting intentional
-0000d720: 6c79 0a20 2020 2020 2020 2074 6f20 6265  ly.        to be
-0000d730: 2063 6f6e 7369 7374 656e 7420 746f 2074   consistent to t
-0000d740: 6865 2066 6972 7374 2064 6973 706c 6163  he first displac
-0000d750: 656d 656e 7473 206f 6620 7468 6520 6663  ements of the fc
-0000d760: 3320 7061 6972 0a20 2020 2020 2020 2064  3 pair.        d
-0000d770: 6973 706c 6163 656d 6574 7320 696e 2073  isplacemets in s
-0000d780: 7570 6572 6365 6c6c 2e0a 0a20 2020 2020  upercell...     
-0000d790: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-0000d7a0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-0000d7b0: 0a20 2020 2020 2020 2064 6973 7461 6e63  .        distanc
-0000d7c0: 6520 3a20 666c 6f61 742c 206f 7074 696f  e : float, optio
-0000d7d0: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
-0000d7e0: 436f 6e73 7461 6e74 2064 6973 706c 6163  Constant displac
-0000d7f0: 656d 656e 7420 4575 636c 6964 6561 6e20  ement Euclidean 
-0000d800: 6469 7374 616e 6365 2e20 4465 6661 756c  distance. Defaul
-0000d810: 7420 6973 2030 2e30 332e 0a20 2020 2020  t is 0.03..     
-0000d820: 2020 2069 735f 706c 7573 6d69 6e75 7320     is_plusminus 
-0000d830: 3a20 5472 7565 2c20 4661 6c73 652c 206f  : True, False, o
-0000d840: 7220 2761 7574 6f27 2c20 6f70 7469 6f6e  r 'auto', option
-0000d850: 616c 0a20 2020 2020 2020 2020 2020 2057  al.            W
-0000d860: 6974 6820 5472 7565 2c20 6174 6f6d 6973  ith True, atomis
-0000d870: 2061 7265 2064 6973 706c 6163 6564 2069   are displaced i
-0000d880: 6e20 626f 7468 2070 6f73 6974 6976 6520  n both positive 
-0000d890: 616e 6420 6e65 6761 7469 7665 0a20 2020  and negative.   
-0000d8a0: 2020 2020 2020 2020 2064 6972 6563 7469           directi
-0000d8b0: 6f6e 732e 2057 6974 6820 4661 6c73 652c  ons. With False,
-0000d8c0: 206f 6e6c 7920 6f6e 6520 6469 7265 6374   only one direct
-0000d8d0: 696f 6e2e 2057 6974 6820 2761 7574 6f27  ion. With 'auto'
-0000d8e0: 2c0a 2020 2020 2020 2020 2020 2020 6d6f  ,.            mo
-0000d8f0: 7374 6c79 2065 7175 6976 616c 656e 7420  stly equivalent 
-0000d900: 746f 2069 735f 706c 7573 6d69 6e75 733d  to is_plusminus=
-0000d910: 5472 7565 2c20 6275 7420 6f6e 6c79 206f  True, but only o
-0000d920: 6e65 2064 6972 6563 7469 6f6e 0a20 2020  ne direction.   
-0000d930: 2020 2020 2020 2020 2069 7320 6368 6f73           is chos
-0000d940: 656e 2077 6865 6e20 7468 6520 6469 7370  en when the disp
-0000d950: 6c61 6365 6d65 6e74 7320 696e 2062 6f74  lacements in bot
-0000d960: 6820 6469 7265 6374 696f 6e73 2061 7265  h directions are
-0000d970: 0a20 2020 2020 2020 2020 2020 2073 796d  .            sym
-0000d980: 6d65 7472 6963 616c 6c79 2065 7175 6976  metrically equiv
-0000d990: 616c 656e 742e 2044 6566 6175 6c74 2069  alent. Default i
-0000d9a0: 7320 2761 7574 6f27 2e0a 2020 2020 2020  s 'auto'..      
-0000d9b0: 2020 6973 5f64 6961 676f 6e61 6c20 3a20    is_diagonal : 
-0000d9c0: 426f 6f6c 2c20 6f70 7469 6f6e 616c 0a20  Bool, optional. 
-0000d9d0: 2020 2020 2020 2020 2020 2057 6974 6820             With 
-0000d9e0: 4661 6c73 652c 2074 6865 2064 6973 706c  False, the displ
-0000d9f0: 6163 656d 656e 7473 2061 7265 206d 6164  acements are mad
-0000da00: 6520 616c 6f6e 6720 7468 6520 6261 7369  e along the basi
-0000da10: 730a 2020 2020 2020 2020 2020 2020 7665  s.            ve
-0000da20: 6374 6f72 7320 6f66 2074 6865 2073 7570  ctors of the sup
-0000da30: 6572 6365 6c6c 2e20 5769 7468 2054 7275  ercell. With Tru
-0000da40: 652c 2064 6972 6563 7469 6f6e 206e 6f74  e, direction not
-0000da50: 2061 6c6f 6e67 2074 6865 2062 6173 6973   along the basis
-0000da60: 0a20 2020 2020 2020 2020 2020 2076 6563  .            vec
-0000da70: 746f 7273 2063 616e 2062 6520 6368 6f73  tors can be chos
-0000da80: 656e 2077 6865 6e20 7468 6520 6e75 6d62  en when the numb
-0000da90: 6572 206f 6620 7468 6520 6469 7370 6c61  er of the displa
-0000daa0: 6365 6d65 6e74 730a 2020 2020 2020 2020  cements.        
-0000dab0: 2020 2020 6d61 7920 6265 2072 6564 7563      may be reduc
-0000dac0: 6564 2e20 4465 6661 756c 7420 6973 2046  ed. Default is F
-0000dad0: 616c 7365 2e0a 0a20 2020 2020 2020 2022  alse...        "
-0000dae0: 2222 0a20 2020 2020 2020 2069 6620 7365  "".        if se
-0000daf0: 6c66 2e5f 7068 6f6e 6f6e 5f73 7570 6572  lf._phonon_super
-0000db00: 6365 6c6c 5f6d 6174 7269 7820 6973 204e  cell_matrix is N
-0000db10: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000db20: 206d 7367 203d 2028 0a20 2020 2020 2020   msg = (.       
-0000db30: 2020 2020 2020 2020 2022 7068 6f6e 6f6e           "phonon
-0000db40: 5f73 7570 6572 6365 6c6c 5f6d 6174 7269  _supercell_matri
-0000db50: 7820 6973 206e 6f74 2073 6574 2e20 220a  x is not set. ".
-0000db60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db70: 2254 6869 7320 6d65 7468 6f64 2069 7320  "This method is 
-0000db80: 7573 6564 2074 6f20 6765 6e65 7261 7465  used to generate
-0000db90: 2064 6973 706c 6163 656d 656e 7473 2074   displacements t
-0000dba0: 6f20 220a 2020 2020 2020 2020 2020 2020  o ".            
-0000dbb0: 2020 2020 2263 616c 6375 6c61 7465 2070      "calculate p
-0000dbc0: 686f 6e6f 6e5f 6663 322e 220a 2020 2020  honon_fc2.".    
-0000dbd0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000dbe0: 2020 2020 2020 7261 6973 6520 5275 6e74        raise Runt
-0000dbf0: 696d 6545 7272 6f72 286d 7367 290a 0a20  imeError(msg).. 
-0000dc00: 2020 2020 2020 2070 686f 6e6f 6e5f 6469         phonon_di
-0000dc10: 7370 6c61 6365 6d65 6e74 5f64 6972 6563  splacement_direc
-0000dc20: 7469 6f6e 7320 3d20 6765 745f 6c65 6173  tions = get_leas
-0000dc30: 745f 6469 7370 6c61 6365 6d65 6e74 7328  t_displacements(
-0000dc40: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000dc50: 662e 5f70 686f 6e6f 6e5f 7375 7065 7263  f._phonon_superc
-0000dc60: 656c 6c5f 7379 6d6d 6574 7279 2c0a 2020  ell_symmetry,.  
-0000dc70: 2020 2020 2020 2020 2020 6973 5f70 6c75            is_plu
-0000dc80: 736d 696e 7573 3d69 735f 706c 7573 6d69  sminus=is_plusmi
-0000dc90: 6e75 732c 0a20 2020 2020 2020 2020 2020  nus,.           
-0000dca0: 2069 735f 6469 6167 6f6e 616c 3d69 735f   is_diagonal=is_
-0000dcb0: 6469 6167 6f6e 616c 2c0a 2020 2020 2020  diagonal,.      
-0000dcc0: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
-0000dcd0: 2e5f 7068 6f6e 6f6e 5f64 6174 6173 6574  ._phonon_dataset
-0000dce0: 203d 2064 6972 6563 7469 6f6e 735f 746f   = directions_to
-0000dcf0: 5f64 6973 706c 6163 656d 656e 745f 6461  _displacement_da
-0000dd00: 7461 7365 7428 0a20 2020 2020 2020 2020  taset(.         
-0000dd10: 2020 2070 686f 6e6f 6e5f 6469 7370 6c61     phonon_displa
-0000dd20: 6365 6d65 6e74 5f64 6972 6563 7469 6f6e  cement_direction
-0000dd30: 732c 2064 6973 7461 6e63 652c 2073 656c  s, distance, sel
-0000dd40: 662e 5f70 686f 6e6f 6e5f 7375 7065 7263  f._phonon_superc
-0000dd50: 656c 6c0a 2020 2020 2020 2020 290a 2020  ell.        ).  
-0000dd60: 2020 2020 2020 7365 6c66 2e5f 7068 6f6e        self._phon
-0000dd70: 6f6e 5f73 7570 6572 6365 6c6c 735f 7769  on_supercells_wi
-0000dd80: 7468 5f64 6973 706c 6163 656d 656e 7473  th_displacements
-0000dd90: 203d 204e 6f6e 650a 0a20 2020 2064 6566   = None..    def
-0000dda0: 2070 726f 6475 6365 5f66 6333 280a 2020   produce_fc3(.  
-0000ddb0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-0000ddc0: 2020 2020 7379 6d6d 6574 7269 7a65 5f66      symmetrize_f
-0000ddd0: 6333 723d 4661 6c73 652c 0a20 2020 2020  c3r=False,.     
-0000dde0: 2020 2069 735f 636f 6d70 6163 745f 6663     is_compact_fc
-0000ddf0: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-0000de00: 6663 5f63 616c 6375 6c61 746f 723d 4e6f  fc_calculator=No
-0000de10: 6e65 2c0a 2020 2020 2020 2020 6663 5f63  ne,.        fc_c
-0000de20: 616c 6375 6c61 746f 725f 6f70 7469 6f6e  alculator_option
-0000de30: 733d 4e6f 6e65 2c0a 2020 2020 293a 0a20  s=None,.    ):. 
-0000de40: 2020 2020 2020 2022 2222 4361 6c63 756c         """Calcul
-0000de50: 6174 6520 6663 3320 6672 6f6d 2064 6973  ate fc3 from dis
-0000de60: 706c 6163 656d 656e 7473 2061 6e64 2066  placements and f
-0000de70: 6f72 6365 732e 0a0a 2020 2020 2020 2020  orces...        
-0000de80: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-0000de90: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-0000dea0: 2020 2020 2020 7379 6d6d 6574 7269 7a65        symmetrize
-0000deb0: 5f66 6333 7220 3a20 626f 6f6c 0a20 2020  _fc3r : bool.   
-0000dec0: 2020 2020 2020 2020 204f 6e6c 7920 666f           Only fo
-0000ded0: 7220 7479 7065 2031 2064 6973 706c 6163  r type 1 displac
-0000dee0: 656d 656e 745f 6461 7461 7365 742c 2074  ement_dataset, t
-0000def0: 7261 6e73 6c61 7469 6f6e 616c 2061 6e64  ranslational and
-0000df00: 0a20 2020 2020 2020 2020 2020 2070 6572  .            per
-0000df10: 6d75 7461 7469 6f6e 2073 796d 6d65 7472  mutation symmetr
-0000df20: 6965 7320 6172 6520 6170 706c 6965 6420  ies are applied 
-0000df30: 6166 7465 7220 6372 6561 7469 6e67 2066  after creating f
-0000df40: 6333 2e20 5468 6973 0a20 2020 2020 2020  c3. This.       
-0000df50: 2020 2020 2073 796d 6d65 7472 697a 6174       symmetrizat
-0000df60: 696f 6e20 6973 206e 6f74 2076 6572 7920  ion is not very 
-0000df70: 736f 7068 6973 7469 6361 7465 6420 616e  sophisticated an
-0000df80: 6420 6361 6e20 6272 6561 6b20 7370 6163  d can break spac
-0000df90: 650a 2020 2020 2020 2020 2020 2020 6772  e.            gr
-0000dfa0: 6f75 7020 7379 6d6d 6574 7279 2c20 6275  oup symmetry, bu
-0000dfb0: 7420 6f66 7465 6e20 7573 6566 756c 2e20  t often useful. 
-0000dfc0: 4966 2062 6574 7465 7220 7379 6d6d 6574  If better symmet
-0000dfd0: 7269 7a61 7469 6f6e 2069 730a 2020 2020  rization is.    
-0000dfe0: 2020 2020 2020 2020 6578 7065 6374 6564          expected
-0000dff0: 2c20 6974 2069 7320 7265 636f 6d6d 656e  , it is recommen
-0000e000: 6465 6420 746f 2075 7365 2065 7874 6572  ded to use exter
-0000e010: 6e61 6c20 666f 7263 6520 636f 6e73 7461  nal force consta
-0000e020: 6e74 730a 2020 2020 2020 2020 2020 2020  nts.            
-0000e030: 6361 6c63 756c 6174 6f72 2073 7563 6820  calculator such 
-0000e040: 6173 2041 4c4d 2e20 4465 6661 756c 7420  as ALM. Default 
-0000e050: 6973 2046 616c 7365 2e0a 2020 2020 2020  is False..      
-0000e060: 2020 6973 5f63 6f6d 7061 6374 5f66 6320    is_compact_fc 
-0000e070: 3a20 626f 6f6c 0a20 2020 2020 2020 2020  : bool.         
-0000e080: 2020 2066 6333 2073 6861 7065 2069 730a     fc3 shape is.
-0000e090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0a0: 4661 6c73 653a 2028 7375 7065 7263 656c  False: (supercel
-0000e0b0: 6c2c 2073 7570 6572 6365 6c6c 2c20 7375  l, supercell, su
-0000e0c0: 7065 6365 6c6c 2c20 332c 2033 2c20 3329  pecell, 3, 3, 3)
-0000e0d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e0e0: 2054 7275 653a 2028 7072 696d 6974 6976   True: (primitiv
-0000e0f0: 652c 2073 7570 6572 6365 6c6c 2c20 7375  e, supercell, su
-0000e100: 7065 6365 6c6c 2c20 332c 2033 2c20 3329  pecell, 3, 3, 3)
-0000e110: 0a20 2020 2020 2020 2020 2020 2077 6865  .            whe
-0000e120: 7265 2027 7375 7065 7263 656c 6c27 2061  re 'supercell' a
-0000e130: 6e64 2027 7072 696d 6974 6976 6527 2069  nd 'primitive' i
-0000e140: 6e64 6963 6174 6520 6e75 6d62 6572 206f  ndicate number o
-0000e150: 6620 6174 6f6d 7320 696e 2074 6865 7365  f atoms in these
-0000e160: 0a20 2020 2020 2020 2020 2020 2063 656c  .            cel
-0000e170: 6c73 2e20 4465 6661 756c 7420 6973 2046  ls. Default is F
-0000e180: 616c 7365 2e0a 2020 2020 2020 2020 6663  alse..        fc
-0000e190: 5f63 616c 6375 6c61 746f 7220 3a20 7374  _calculator : st
-0000e1a0: 7220 6f72 204e 6f6e 650a 2020 2020 2020  r or None.      
-0000e1b0: 2020 2020 2020 466f 7263 6520 636f 6e73        Force cons
-0000e1c0: 7461 6e74 7320 6361 6c63 756c 6174 6f72  tants calculator
-0000e1d0: 2067 6976 656e 2062 7920 7374 722e 0a20   given by str.. 
-0000e1e0: 2020 2020 2020 2066 635f 6361 6c63 756c         fc_calcul
-0000e1f0: 6174 6f72 5f6f 7074 696f 6e73 203a 2064  ator_options : d
-0000e200: 6963 740a 2020 2020 2020 2020 2020 2020  ict.            
-0000e210: 4f70 7469 6f6e 7320 666f 7220 6578 7465  Options for exte
-0000e220: 726e 616c 2066 6f72 6365 2063 6f6e 7374  rnal force const
-0000e230: 616e 7473 2063 616c 6375 6c61 746f 722e  ants calculator.
-0000e240: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0000e250: 2020 2020 2020 6469 7370 5f64 6174 6173        disp_datas
-0000e260: 6574 203d 2073 656c 662e 5f64 6174 6173  et = self._datas
-0000e270: 6574 0a0a 2020 2020 2020 2020 6663 335f  et..        fc3_
-0000e280: 6361 6c63 756c 6174 6f72 2c20 6663 335f  calculator, fc3_
-0000e290: 6361 6c63 756c 6174 6f72 5f6f 7074 696f  calculator_optio
-0000e2a0: 6e73 203d 2073 656c 662e 5f65 7874 7261  ns = self._extra
-0000e2b0: 6374 5f66 6332 5f66 6333 5f63 616c 6375  ct_fc2_fc3_calcu
-0000e2c0: 6c61 746f 7273 280a 2020 2020 2020 2020  lators(.        
-0000e2d0: 2020 2020 6663 5f63 616c 6375 6c61 746f      fc_calculato
-0000e2e0: 722c 2066 635f 6361 6c63 756c 6174 6f72  r, fc_calculator
-0000e2f0: 5f6f 7074 696f 6e73 2c20 330a 2020 2020  _options, 3.    
-0000e300: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
-0000e310: 6620 6663 335f 6361 6c63 756c 6174 6f72  f fc3_calculator
-0000e320: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000e330: 2020 2020 2020 2020 2020 6469 7370 732c            disps,
-0000e340: 2066 6f72 6365 7320 3d20 6765 745f 6469   forces = get_di
-0000e350: 7370 6c61 6365 6d65 6e74 735f 616e 645f  splacements_and_
-0000e360: 666f 7263 6573 5f66 6333 2864 6973 705f  forces_fc3(disp_
-0000e370: 6461 7461 7365 7429 0a20 2020 2020 2020  dataset).       
-0000e380: 2020 2020 2066 6332 2c20 6663 3320 3d20       fc2, fc3 = 
-0000e390: 6765 745f 6663 3328 0a20 2020 2020 2020  get_fc3(.       
-0000e3a0: 2020 2020 2020 2020 2073 656c 662e 5f73           self._s
-0000e3b0: 7570 6572 6365 6c6c 2c0a 2020 2020 2020  upercell,.      
-0000e3c0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000e3d0: 7072 696d 6974 6976 652c 0a20 2020 2020  primitive,.     
-0000e3e0: 2020 2020 2020 2020 2020 2064 6973 7073             disps
-0000e3f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000e400: 2020 666f 7263 6573 2c0a 2020 2020 2020    forces,.      
-0000e410: 2020 2020 2020 2020 2020 6663 5f63 616c            fc_cal
-0000e420: 6375 6c61 746f 723d 6663 335f 6361 6c63  culator=fc3_calc
-0000e430: 756c 6174 6f72 2c0a 2020 2020 2020 2020  ulator,.        
-0000e440: 2020 2020 2020 2020 6663 5f63 616c 6375          fc_calcu
-0000e450: 6c61 746f 725f 6f70 7469 6f6e 733d 6663  lator_options=fc
-0000e460: 335f 6361 6c63 756c 6174 6f72 5f6f 7074  3_calculator_opt
-0000e470: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
-0000e480: 2020 2020 2020 6973 5f63 6f6d 7061 6374        is_compact
-0000e490: 5f66 633d 6973 5f63 6f6d 7061 6374 5f66  _fc=is_compact_f
-0000e4a0: 632c 0a20 2020 2020 2020 2020 2020 2020  c,.             
-0000e4b0: 2020 206c 6f67 5f6c 6576 656c 3d73 656c     log_level=sel
-0000e4c0: 662e 5f6c 6f67 5f6c 6576 656c 2c0a 2020  f._log_level,.  
-0000e4d0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000e4e0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000e4f0: 2020 2020 2020 6966 2022 6469 7370 6c61        if "displa
-0000e500: 6365 6d65 6e74 7322 2069 6e20 6469 7370  cements" in disp
-0000e510: 5f64 6174 6173 6574 3a0a 2020 2020 2020  _dataset:.      
-0000e520: 2020 2020 2020 2020 2020 6d73 6720 3d20            msg = 
-0000e530: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000e540: 2020 2020 2020 2266 635f 6361 6c63 756c        "fc_calcul
-0000e550: 6174 6f72 2068 6173 2074 6f20 6265 2073  ator has to be s
-0000e560: 6574 2074 6f20 7072 6f64 7563 6520 666f  et to produce fo
-0000e570: 7263 6520 220a 2020 2020 2020 2020 2020  rce ".          
-0000e580: 2020 2020 2020 2020 2020 2263 6f6e 7374            "const
-0000e590: 616e 7320 6672 6f6d 2074 6869 7320 6461  ans from this da
-0000e5a0: 7461 7365 742e 220a 2020 2020 2020 2020  taset.".        
-0000e5b0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000e5c0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000e5d0: 466f 7263 6543 616c 6375 6c61 746f 7252  ForceCalculatorR
-0000e5e0: 6571 7569 7265 6445 7272 6f72 286d 7367  equiredError(msg
-0000e5f0: 290a 2020 2020 2020 2020 2020 2020 6663  ).            fc
-0000e600: 322c 2066 6333 203d 2067 6574 5f70 686f  2, fc3 = get_pho
-0000e610: 6e6f 3370 795f 6663 3328 0a20 2020 2020  no3py_fc3(.     
-0000e620: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e630: 5f73 7570 6572 6365 6c6c 2c0a 2020 2020  _supercell,.    
-0000e640: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e650: 2e5f 7072 696d 6974 6976 652c 0a20 2020  ._primitive,.   
-0000e660: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-0000e670: 705f 6461 7461 7365 742c 0a20 2020 2020  p_dataset,.     
-0000e680: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e690: 5f73 796d 6d65 7472 792c 0a20 2020 2020  _symmetry,.     
-0000e6a0: 2020 2020 2020 2020 2020 2069 735f 636f             is_co
-0000e6b0: 6d70 6163 745f 6663 3d69 735f 636f 6d70  mpact_fc=is_comp
-0000e6c0: 6163 745f 6663 2c0a 2020 2020 2020 2020  act_fc,.        
-0000e6d0: 2020 2020 2020 2020 7665 7262 6f73 653d          verbose=
-0000e6e0: 7365 6c66 2e5f 6c6f 675f 6c65 7665 6c2c  self._log_level,
-0000e6f0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0000e700: 2020 2020 2020 2020 2020 2069 6620 7379             if sy
-0000e710: 6d6d 6574 7269 7a65 5f66 6333 723a 0a20  mmetrize_fc3r:. 
-0000e720: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000e730: 6620 6973 5f63 6f6d 7061 6374 5f66 633a  f is_compact_fc:
-0000e740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e750: 2020 2020 2073 6574 5f74 7261 6e73 6c61       set_transla
-0000e760: 7469 6f6e 616c 5f69 6e76 6172 6961 6e63  tional_invarianc
-0000e770: 655f 636f 6d70 6163 745f 6663 3328 6663  e_compact_fc3(fc
-0000e780: 332c 2073 656c 662e 5f70 7269 6d69 7469  3, self._primiti
-0000e790: 7665 290a 2020 2020 2020 2020 2020 2020  ve).            
-0000e7a0: 2020 2020 2020 2020 7365 745f 7065 726d          set_perm
-0000e7b0: 7574 6174 696f 6e5f 7379 6d6d 6574 7279  utation_symmetry
-0000e7c0: 5f63 6f6d 7061 6374 5f66 6333 2866 6333  _compact_fc3(fc3
-0000e7d0: 2c20 7365 6c66 2e5f 7072 696d 6974 6976  , self._primitiv
-0000e7e0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-0000e7f0: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
-0000e800: 6663 3220 6973 204e 6f6e 653a 0a20 2020  fc2 is None:.   
-0000e810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e820: 2020 2020 2073 796d 6d65 7472 697a 655f       symmetrize_
-0000e830: 636f 6d70 6163 745f 666f 7263 655f 636f  compact_force_co
-0000e840: 6e73 7461 6e74 7328 6663 322c 2073 656c  nstants(fc2, sel
-0000e850: 662e 5f70 7269 6d69 7469 7665 290a 2020  f._primitive).  
-0000e860: 2020 2020 2020 2020 2020 2020 2020 656c                el
-0000e870: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000e880: 2020 2020 2020 2020 7365 745f 7472 616e          set_tran
-0000e890: 736c 6174 696f 6e61 6c5f 696e 7661 7269  slational_invari
-0000e8a0: 616e 6365 5f66 6333 2866 6333 290a 2020  ance_fc3(fc3).  
-0000e8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8c0: 2020 7365 745f 7065 726d 7574 6174 696f    set_permutatio
-0000e8d0: 6e5f 7379 6d6d 6574 7279 5f66 6333 2866  n_symmetry_fc3(f
-0000e8e0: 6333 290a 2020 2020 2020 2020 2020 2020  c3).            
-0000e8f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000e900: 5f66 6332 2069 7320 4e6f 6e65 3a0a 2020  _fc2 is None:.  
-0000e910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e920: 2020 2020 2020 7379 6d6d 6574 7269 7a65        symmetrize
-0000e930: 5f66 6f72 6365 5f63 6f6e 7374 616e 7473  _force_constants
-0000e940: 2866 6332 290a 0a20 2020 2020 2020 2023  (fc2)..        #
-0000e950: 2053 6574 2066 6332 2061 6e64 2066 6333   Set fc2 and fc3
-0000e960: 0a20 2020 2020 2020 2073 656c 662e 5f66  .        self._f
-0000e970: 6333 203d 2066 6333 0a0a 2020 2020 2020  c3 = fc3..      
-0000e980: 2020 2320 6663 3220 6173 206f 6274 6169    # fc2 as obtai
-0000e990: 6e65 6420 6162 6f76 6520 7769 6c6c 206e  ned above will n
-0000e9a0: 6f74 2062 6520 7365 7420 7768 656e 2022  ot be set when "
-0000e9b0: 7c22 2069 6e20 6663 2d63 616c 6375 6c61  |" in fc-calcula
-0000e9c0: 746f 7220 7365 7474 696e 672e 0a20 2020  tor setting..   
-0000e9d0: 2020 2020 2069 6620 6663 5f63 616c 6375       if fc_calcu
-0000e9e0: 6c61 746f 7220 6973 206e 6f74 204e 6f6e  lator is not Non
-0000e9f0: 6520 616e 6420 227c 2220 696e 2066 635f  e and "|" in fc_
-0000ea00: 6361 6c63 756c 6174 6f72 3a0a 2020 2020  calculator:.    
-0000ea10: 2020 2020 2020 2020 6663 3220 3d20 4e6f          fc2 = No
-0000ea20: 6e65 0a20 2020 2020 2020 2069 6620 6663  ne.        if fc
-0000ea30: 5f63 616c 6375 6c61 746f 725f 6f70 7469  _calculator_opti
-0000ea40: 6f6e 7320 6973 206e 6f74 204e 6f6e 6520  ons is not None 
-0000ea50: 616e 6420 227c 2220 696e 2066 635f 6361  and "|" in fc_ca
-0000ea60: 6c63 756c 6174 6f72 5f6f 7074 696f 6e73  lculator_options
-0000ea70: 3a0a 2020 2020 2020 2020 2020 2020 6663  :.            fc
-0000ea80: 3220 3d20 4e6f 6e65 0a0a 2020 2020 2020  2 = None..      
-0000ea90: 2020 2320 4e6f 726d 616c 6c79 2073 656c    # Normally sel
-0000eaa0: 662e 5f66 6332 2069 7320 6f76 6572 7772  f._fc2 is overwr
-0000eab0: 6974 7465 6e20 696e 2070 726f 6475 6365  itten in produce
-0000eac0: 5f66 6332 0a20 2020 2020 2020 2069 6620  _fc2.        if 
-0000ead0: 7365 6c66 2e5f 6663 3220 6973 204e 6f6e  self._fc2 is Non
-0000eae0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0000eaf0: 656c 662e 5f66 6332 203d 2066 6332 0a0a  elf._fc2 = fc2..
-0000eb00: 2020 2020 6465 6620 7072 6f64 7563 655f      def produce_
-0000eb10: 6663 3228 0a20 2020 2020 2020 2073 656c  fc2(.        sel
-0000eb20: 662c 0a20 2020 2020 2020 2073 796d 6d65  f,.        symme
-0000eb30: 7472 697a 655f 6663 323d 4661 6c73 652c  trize_fc2=False,
-0000eb40: 0a20 2020 2020 2020 2069 735f 636f 6d70  .        is_comp
-0000eb50: 6163 745f 6663 3d46 616c 7365 2c0a 2020  act_fc=False,.  
-0000eb60: 2020 2020 2020 6663 5f63 616c 6375 6c61        fc_calcula
-0000eb70: 746f 723d 4e6f 6e65 2c0a 2020 2020 2020  tor=None,.      
-0000eb80: 2020 6663 5f63 616c 6375 6c61 746f 725f    fc_calculator_
-0000eb90: 6f70 7469 6f6e 733d 4e6f 6e65 2c0a 2020  options=None,.  
-0000eba0: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
-0000ebb0: 4361 6c63 756c 6174 6520 6663 3220 6672  Calculate fc2 fr
-0000ebc0: 6f6d 2064 6973 706c 6163 656d 656e 7473  om displacements
-0000ebd0: 2061 6e64 2066 6f72 6365 732e 0a0a 2020   and forces...  
-0000ebe0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-0000ebf0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-0000ec00: 2d2d 2d0a 2020 2020 2020 2020 7379 6d6d  ---.        symm
-0000ec10: 6574 7269 7a65 5f66 6332 203a 2062 6f6f  etrize_fc2 : boo
-0000ec20: 6c0a 2020 2020 2020 2020 2020 2020 4f6e  l.            On
-0000ec30: 6c79 2066 6f72 2074 7970 6520 3120 6469  ly for type 1 di
-0000ec40: 7370 6c61 6365 6d65 6e74 5f64 6174 6173  splacement_datas
-0000ec50: 6574 2c20 7472 616e 736c 6174 696f 6e61  et, translationa
-0000ec60: 6c20 616e 640a 2020 2020 2020 2020 2020  l and.          
-0000ec70: 2020 7065 726d 7574 6174 696f 6e20 7379    permutation sy
-0000ec80: 6d6d 6574 7269 6573 2061 7265 2061 7070  mmetries are app
-0000ec90: 6c69 6564 2061 6674 6572 2063 7265 6174  lied after creat
-0000eca0: 696e 6720 6663 332e 2054 6869 730a 2020  ing fc3. This.  
-0000ecb0: 2020 2020 2020 2020 2020 7379 6d6d 6574            symmet
-0000ecc0: 7269 7a61 7469 6f6e 2069 7320 6e6f 7420  rization is not 
-0000ecd0: 7665 7279 2073 6f70 6869 7374 6963 6174  very sophisticat
-0000ece0: 6564 2061 6e64 2063 616e 2062 7265 616b  ed and can break
-0000ecf0: 2073 7061 6365 0a20 2020 2020 2020 2020   space.         
-0000ed00: 2020 2067 726f 7570 2073 796d 6d65 7472     group symmetr
-0000ed10: 792c 2062 7574 206f 6674 656e 2075 7365  y, but often use
-0000ed20: 6675 6c2e 2049 6620 6265 7474 6572 2073  ful. If better s
-0000ed30: 796d 6d65 7472 697a 6174 696f 6e20 6973  ymmetrization is
-0000ed40: 0a20 2020 2020 2020 2020 2020 2065 7870  .            exp
-0000ed50: 6563 7465 642c 2069 7420 6973 2072 6563  ected, it is rec
-0000ed60: 6f6d 6d65 6e64 6564 2074 6f20 7573 6520  ommended to use 
-0000ed70: 6578 7465 726e 616c 2066 6f72 6365 2063  external force c
-0000ed80: 6f6e 7374 616e 7473 0a20 2020 2020 2020  onstants.       
-0000ed90: 2020 2020 2063 616c 6375 6c61 746f 7220       calculator 
-0000eda0: 7375 6368 2061 7320 414c 4d2e 2044 6566  such as ALM. Def
-0000edb0: 6175 6c74 2069 7320 4661 6c73 652e 0a20  ault is False.. 
-0000edc0: 2020 2020 2020 2069 735f 636f 6d70 6163         is_compac
-0000edd0: 745f 6663 203a 2062 6f6f 6c0a 2020 2020  t_fc : bool.    
-0000ede0: 2020 2020 2020 2020 6663 3220 7368 6170          fc2 shap
-0000edf0: 6520 6973 0a20 2020 2020 2020 2020 2020  e is.           
-0000ee00: 2020 2020 2046 616c 7365 3a20 2873 7570       False: (sup
-0000ee10: 6572 6365 6c6c 2c20 7375 7065 6365 6c6c  ercell, supecell
-0000ee20: 2c20 332c 2033 290a 2020 2020 2020 2020  , 3, 3).        
-0000ee30: 2020 2020 2020 2020 5472 7565 3a20 2870          True: (p
-0000ee40: 7269 6d69 7469 7665 2c20 7375 7065 6365  rimitive, supece
-0000ee50: 6c6c 2c20 332c 2033 290a 2020 2020 2020  ll, 3, 3).      
-0000ee60: 2020 2020 2020 7768 6572 6520 2773 7570        where 'sup
-0000ee70: 6572 6365 6c6c 2720 616e 6420 2770 7269  ercell' and 'pri
-0000ee80: 6d69 7469 7665 2720 696e 6469 6361 7465  mitive' indicate
-0000ee90: 206e 756d 6265 7220 6f66 2061 746f 6d73   number of atoms
-0000eea0: 2069 6e20 7468 6573 650a 2020 2020 2020   in these.      
-0000eeb0: 2020 2020 2020 6365 6c6c 732e 2044 6566        cells. Def
-0000eec0: 6175 6c74 2069 7320 4661 6c73 652e 0a20  ault is False.. 
-0000eed0: 2020 2020 2020 2066 635f 6361 6c63 756c         fc_calcul
-0000eee0: 6174 6f72 203a 2073 7472 206f 7220 4e6f  ator : str or No
-0000eef0: 6e65 0a20 2020 2020 2020 2020 2020 2046  ne.            F
-0000ef00: 6f72 6365 2063 6f6e 7374 616e 7473 2063  orce constants c
-0000ef10: 616c 6375 6c61 746f 7220 6769 7665 6e20  alculator given 
-0000ef20: 6279 2073 7472 2e0a 2020 2020 2020 2020  by str..        
-0000ef30: 6663 5f63 616c 6375 6c61 746f 725f 6f70  fc_calculator_op
-0000ef40: 7469 6f6e 7320 3a20 6469 6374 0a20 2020  tions : dict.   
-0000ef50: 2020 2020 2020 2020 204f 7074 696f 6e73           Options
-0000ef60: 2066 6f72 2065 7874 6572 6e61 6c20 666f   for external fo
-0000ef70: 7263 6520 636f 6e73 7461 6e74 7320 6361  rce constants ca
-0000ef80: 6c63 756c 6174 6f72 2e0a 0a20 2020 2020  lculator...     
-0000ef90: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-0000efa0: 6620 7365 6c66 2e5f 7068 6f6e 6f6e 5f64  f self._phonon_d
-0000efb0: 6174 6173 6574 2069 7320 4e6f 6e65 3a0a  ataset is None:.
-0000efc0: 2020 2020 2020 2020 2020 2020 6469 7370              disp
-0000efd0: 5f64 6174 6173 6574 203d 2073 656c 662e  _dataset = self.
-0000efe0: 5f64 6174 6173 6574 0a20 2020 2020 2020  _dataset.       
-0000eff0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000f000: 2020 2064 6973 705f 6461 7461 7365 7420     disp_dataset 
-0000f010: 3d20 7365 6c66 2e5f 7068 6f6e 6f6e 5f64  = self._phonon_d
-0000f020: 6174 6173 6574 0a0a 2020 2020 2020 2020  ataset..        
-0000f030: 6966 2069 735f 636f 6d70 6163 745f 6663  if is_compact_fc
-0000f040: 3a0a 2020 2020 2020 2020 2020 2020 7032  :.            p2
-0000f050: 735f 6d61 7020 3d20 7365 6c66 2e5f 7068  s_map = self._ph
-0000f060: 6f6e 6f6e 5f70 7269 6d69 7469 7665 2e70  onon_primitive.p
-0000f070: 3273 5f6d 6170 0a20 2020 2020 2020 2065  2s_map.        e
-0000f080: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000f090: 2070 3273 5f6d 6170 203d 204e 6f6e 650a   p2s_map = None.
-0000f0a0: 0a20 2020 2020 2020 2066 6332 5f63 616c  .        fc2_cal
-0000f0b0: 6375 6c61 746f 722c 2066 6332 5f63 616c  culator, fc2_cal
-0000f0c0: 6375 6c61 746f 725f 6f70 7469 6f6e 7320  culator_options 
-0000f0d0: 3d20 7365 6c66 2e5f 6578 7472 6163 745f  = self._extract_
-0000f0e0: 6663 325f 6663 335f 6361 6c63 756c 6174  fc2_fc3_calculat
-0000f0f0: 6f72 7328 0a20 2020 2020 2020 2020 2020  ors(.           
-0000f100: 2066 635f 6361 6c63 756c 6174 6f72 2c20   fc_calculator, 
-0000f110: 6663 5f63 616c 6375 6c61 746f 725f 6f70  fc_calculator_op
-0000f120: 7469 6f6e 732c 2032 0a20 2020 2020 2020  tions, 2.       
-0000f130: 2029 0a0a 2020 2020 2020 2020 6966 2066   )..        if f
-0000f140: 6332 5f63 616c 6375 6c61 746f 7220 6973  c2_calculator is
-0000f150: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000f160: 2020 2020 2020 2064 6973 7073 2c20 666f         disps, fo
-0000f170: 7263 6573 203d 2067 6574 5f64 6973 706c  rces = get_displ
-0000f180: 6163 656d 656e 7473 5f61 6e64 5f66 6f72  acements_and_for
-0000f190: 6365 7328 6469 7370 5f64 6174 6173 6574  ces(disp_dataset
-0000f1a0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-0000f1b0: 6c66 2e5f 6663 3220 3d20 6765 745f 6663  lf._fc2 = get_fc
-0000f1c0: 3228 0a20 2020 2020 2020 2020 2020 2020  2(.             
-0000f1d0: 2020 2073 656c 662e 5f70 686f 6e6f 6e5f     self._phonon_
-0000f1e0: 7375 7065 7263 656c 6c2c 0a20 2020 2020  supercell,.     
-0000f1f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f200: 5f70 686f 6e6f 6e5f 7072 696d 6974 6976  _phonon_primitiv
-0000f210: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0000f220: 2020 2064 6973 7073 2c0a 2020 2020 2020     disps,.      
-0000f230: 2020 2020 2020 2020 2020 666f 7263 6573            forces
-0000f240: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000f250: 2020 6663 5f63 616c 6375 6c61 746f 723d    fc_calculator=
-0000f260: 6663 325f 6361 6c63 756c 6174 6f72 2c0a  fc2_calculator,.
-0000f270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f280: 6663 5f63 616c 6375 6c61 746f 725f 6f70  fc_calculator_op
-0000f290: 7469 6f6e 733d 6663 325f 6361 6c63 756c  tions=fc2_calcul
-0000f2a0: 6174 6f72 5f6f 7074 696f 6e73 2c0a 2020  ator_options,.  
-0000f2b0: 2020 2020 2020 2020 2020 2020 2020 6174                at
-0000f2c0: 6f6d 5f6c 6973 743d 7032 735f 6d61 702c  om_list=p2s_map,
-0000f2d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f2e0: 206c 6f67 5f6c 6576 656c 3d73 656c 662e   log_level=self.
-0000f2f0: 5f6c 6f67 5f6c 6576 656c 2c0a 2020 2020  _log_level,.    
-0000f300: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000f310: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000f320: 2020 2020 6966 2022 6469 7370 6c61 6365      if "displace
-0000f330: 6d65 6e74 7322 2069 6e20 6469 7370 5f64  ments" in disp_d
-0000f340: 6174 6173 6574 3a0a 2020 2020 2020 2020  ataset:.        
-0000f350: 2020 2020 2020 2020 6d73 6720 3d20 280a          msg = (.
-0000f360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f370: 2020 2020 2266 635f 6361 6c63 756c 6174      "fc_calculat
-0000f380: 6f72 2068 6173 2074 6f20 6265 2073 6574  or has to be set
-0000f390: 2074 6f20 7072 6f64 7563 6520 666f 7263   to produce forc
-0000f3a0: 6520 220a 2020 2020 2020 2020 2020 2020  e ".            
-0000f3b0: 2020 2020 2020 2020 2263 6f6e 7374 616e          "constan
-0000f3c0: 7320 6672 6f6d 2074 6869 7320 6461 7461  s from this data
-0000f3d0: 7365 7420 666f 7220 6663 322e 220a 2020  set for fc2.".  
-0000f3e0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000f3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f400: 7261 6973 6520 5275 6e74 696d 6545 7272  raise RuntimeErr
-0000f410: 6f72 286d 7367 290a 2020 2020 2020 2020  or(msg).        
-0000f420: 2020 2020 7365 6c66 2e5f 6663 3220 3d20      self._fc2 = 
-0000f430: 6765 745f 7068 6f6e 6f70 795f 6663 3228  get_phonopy_fc2(
-0000f440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f450: 2073 656c 662e 5f70 686f 6e6f 6e5f 7375   self._phonon_su
-0000f460: 7065 7263 656c 6c2c 0a20 2020 2020 2020  percell,.       
-0000f470: 2020 2020 2020 2020 2073 656c 662e 5f70           self._p
-0000f480: 686f 6e6f 6e5f 7375 7065 7263 656c 6c5f  honon_supercell_
-0000f490: 7379 6d6d 6574 7279 2c0a 2020 2020 2020  symmetry,.      
-0000f4a0: 2020 2020 2020 2020 2020 6469 7370 5f64            disp_d
-0000f4b0: 6174 6173 6574 2c0a 2020 2020 2020 2020  ataset,.        
-0000f4c0: 2020 2020 2020 2020 6174 6f6d 5f6c 6973          atom_lis
-0000f4d0: 743d 7032 735f 6d61 702c 0a20 2020 2020  t=p2s_map,.     
-0000f4e0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000f4f0: 2020 2020 2069 6620 7379 6d6d 6574 7269       if symmetri
-0000f500: 7a65 5f66 6332 3a0a 2020 2020 2020 2020  ze_fc2:.        
-0000f510: 2020 2020 2020 2020 6966 2069 735f 636f          if is_co
-0000f520: 6d70 6163 745f 6663 3a0a 2020 2020 2020  mpact_fc:.      
-0000f530: 2020 2020 2020 2020 2020 2020 2020 7379                sy
-0000f540: 6d6d 6574 7269 7a65 5f63 6f6d 7061 6374  mmetrize_compact
-0000f550: 5f66 6f72 6365 5f63 6f6e 7374 616e 7473  _force_constants
-0000f560: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000f570: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000f580: 6663 322c 2073 656c 662e 5f70 686f 6e6f  fc2, self._phono
-0000f590: 6e5f 7072 696d 6974 6976 650a 2020 2020  n_primitive.    
-0000f5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000f5c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000f5d0: 2020 2020 2020 2020 2020 2020 7379 6d6d              symm
-0000f5e0: 6574 7269 7a65 5f66 6f72 6365 5f63 6f6e  etrize_force_con
-0000f5f0: 7374 616e 7473 2873 656c 662e 5f66 6332  stants(self._fc2
-0000f600: 290a 0a20 2020 2064 6566 2063 7574 6f66  )..    def cutof
-0000f610: 665f 6663 335f 6279 5f7a 6572 6f28 7365  f_fc3_by_zero(se
-0000f620: 6c66 2c20 6375 746f 6666 5f64 6973 7461  lf, cutoff_dista
-0000f630: 6e63 652c 2066 6333 3d4e 6f6e 6529 3a0a  nce, fc3=None):.
-0000f640: 2020 2020 2020 2020 2222 2253 6574 207a          """Set z
-0000f650: 6572 6f20 746f 2066 6333 2065 6c65 6d65  ero to fc3 eleme
-0000f660: 6e74 7320 6f75 7420 6f66 2063 7574 6f66  nts out of cutof
-0000f670: 6620 6469 7374 616e 6365 2e0a 0a20 2020  f distance...   
-0000f680: 2020 2020 204e 6f74 650a 2020 2020 2020       Note.      
-0000f690: 2020 2d2d 2d2d 0a20 2020 2020 2020 2066    ----.        f
-0000f6a0: 6333 2069 7320 6f76 6572 7772 6974 7465  c3 is overwritte
-0000f6b0: 6e2e 0a0a 2020 2020 2020 2020 5061 7261  n...        Para
-0000f6c0: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-0000f6d0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-0000f6e0: 2020 6375 746f 6666 5f64 6973 7461 6e63    cutoff_distanc
-0000f6f0: 6520 3a20 666c 6f61 740a 2020 2020 2020  e : float.      
-0000f700: 2020 2020 2020 4166 7465 7220 6372 6561        After crea
-0000f710: 7469 6e67 2066 6f72 6365 2063 6f6e 7374  ting force const
-0000f720: 616e 7473 2c20 6663 2065 6c65 6d65 6e74  ants, fc element
-0000f730: 7320 7768 6572 6520 616e 7920 7061 6972  s where any pair
-0000f740: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
-0000f750: 7461 6e63 6520 696e 2061 746f 6d20 7472  tance in atom tr
-0000f760: 6970 6c65 7473 206c 6172 6765 7220 7468  iplets larger th
-0000f770: 616e 2063 7574 6f66 665f 6469 7374 616e  an cutoff_distan
-0000f780: 6365 2061 7265 2073 6574 207a 6572 6f2e  ce are set zero.
-0000f790: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0000f7a0: 2020 2020 2020 6966 2066 6333 2069 7320        if fc3 is 
-0000f7b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000f7c0: 2020 5f66 6333 203d 2073 656c 662e 5f66    _fc3 = self._f
-0000f7d0: 6333 0a20 2020 2020 2020 2065 6c73 653a  c3.        else:
-0000f7e0: 0a20 2020 2020 2020 2020 2020 205f 6663  .            _fc
-0000f7f0: 3320 3d20 6663 330a 2020 2020 2020 2020  3 = fc3.        
-0000f800: 6375 746f 6666 5f66 6333 5f62 795f 7a65  cutoff_fc3_by_ze
-0000f810: 726f 280a 2020 2020 2020 2020 2020 2020  ro(.            
-0000f820: 5f66 6333 2c0a 2020 2020 2020 2020 2020  _fc3,.          
-0000f830: 2020 7365 6c66 2e5f 7375 7065 7263 656c    self._supercel
-0000f840: 6c2c 0a20 2020 2020 2020 2020 2020 2063  l,.            c
-0000f850: 7574 6f66 665f 6469 7374 616e 6365 2c0a  utoff_distance,.
-0000f860: 2020 2020 2020 2020 2020 2020 7032 735f              p2s_
-0000f870: 6d61 703d 7365 6c66 2e5f 7072 696d 6974  map=self._primit
-0000f880: 6976 652e 7032 735f 6d61 702c 0a20 2020  ive.p2s_map,.   
-0000f890: 2020 2020 2020 2020 2073 796d 7072 6563           symprec
-0000f8a0: 3d73 656c 662e 5f73 796d 7072 6563 2c0a  =self._symprec,.
-0000f8b0: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-0000f8c0: 6566 2073 6574 5f70 6572 6d75 7461 7469  ef set_permutati
-0000f8d0: 6f6e 5f73 796d 6d65 7472 7928 7365 6c66  on_symmetry(self
-0000f8e0: 293a 0a20 2020 2020 2020 2022 2222 456e  ):.        """En
-0000f8f0: 666f 7263 6520 7065 726d 7574 6174 696f  force permutatio
-0000f900: 6e20 7379 6d6d 6574 7279 2074 6f20 6663  n symmetry to fc
-0000f910: 3220 616e 6420 6663 332e 2222 220a 2020  2 and fc3.""".  
-0000f920: 2020 2020 2020 6966 2073 656c 662e 5f66        if self._f
-0000f930: 6332 2069 7320 6e6f 7420 4e6f 6e65 3a0a  c2 is not None:.
-0000f940: 2020 2020 2020 2020 2020 2020 7365 745f              set_
-0000f950: 7065 726d 7574 6174 696f 6e5f 7379 6d6d  permutation_symm
-0000f960: 6574 7279 2873 656c 662e 5f66 6332 290a  etry(self._fc2).
-0000f970: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000f980: 5f66 6333 2069 7320 6e6f 7420 4e6f 6e65  _fc3 is not None
-0000f990: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000f9a0: 745f 7065 726d 7574 6174 696f 6e5f 7379  t_permutation_sy
-0000f9b0: 6d6d 6574 7279 5f66 6333 2873 656c 662e  mmetry_fc3(self.
-0000f9c0: 5f66 6333 290a 0a20 2020 2064 6566 2073  _fc3)..    def s
-0000f9d0: 6574 5f74 7261 6e73 6c61 7469 6f6e 616c  et_translational
-0000f9e0: 5f69 6e76 6172 6961 6e63 6528 7365 6c66  _invariance(self
-0000f9f0: 293a 0a20 2020 2020 2020 2022 2222 456e  ):.        """En
-0000fa00: 666f 7263 6520 7472 616e 736c 6174 696f  force translatio
-0000fa10: 6e20 696e 7661 7269 616e 6365 2e0a 0a20  n invariance... 
-0000fa20: 2020 2020 2020 2054 6869 7320 7375 6274         This subt
-0000fa30: 7261 6374 7320 6472 6966 7420 6469 7669  racts drift divi
-0000fa40: 6465 6420 6279 206e 756d 6265 7220 6f66  ded by number of
-0000fa50: 2065 6c65 6d65 6e74 7320 696e 2065 6163   elements in eac
-0000fa60: 6820 726f 7720 616e 640a 2020 2020 2020  h row and.      
-0000fa70: 2020 636f 6c75 6d6e 2e0a 0a20 2020 2020    column...     
-0000fa80: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-0000fa90: 6620 7365 6c66 2e5f 6663 3220 6973 206e  f self._fc2 is n
-0000faa0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000fab0: 2020 2020 2073 6574 5f74 7261 6e73 6c61       set_transla
-0000fac0: 7469 6f6e 616c 5f69 6e76 6172 6961 6e63  tional_invarianc
-0000fad0: 6528 7365 6c66 2e5f 6663 3229 0a20 2020  e(self._fc2).   
-0000fae0: 2020 2020 2069 6620 7365 6c66 2e5f 6663       if self._fc
-0000faf0: 3320 6973 206e 6f74 204e 6f6e 653a 0a20  3 is not None:. 
-0000fb00: 2020 2020 2020 2020 2020 2073 6574 5f74             set_t
-0000fb10: 7261 6e73 6c61 7469 6f6e 616c 5f69 6e76  ranslational_inv
-0000fb20: 6172 6961 6e63 655f 6663 3328 7365 6c66  ariance_fc3(self
-0000fb30: 2e5f 6663 3329 0a0a 2020 2020 6465 6620  ._fc3)..    def 
-0000fb40: 7275 6e5f 696d 6167 5f73 656c 665f 656e  run_imag_self_en
-0000fb50: 6572 6779 280a 2020 2020 2020 2020 7365  ergy(.        se
-0000fb60: 6c66 2c0a 2020 2020 2020 2020 6772 6964  lf,.        grid
-0000fb70: 5f70 6f69 6e74 732c 0a20 2020 2020 2020  _points,.       
-0000fb80: 2074 656d 7065 7261 7475 7265 732c 0a20   temperatures,. 
-0000fb90: 2020 2020 2020 2066 7265 7175 656e 6379         frequency
-0000fba0: 5f70 6f69 6e74 733d 4e6f 6e65 2c0a 2020  _points=None,.  
-0000fbb0: 2020 2020 2020 6672 6571 7565 6e63 795f        frequency_
-0000fbc0: 7374 6570 3d4e 6f6e 652c 0a20 2020 2020  step=None,.     
-0000fbd0: 2020 206e 756d 5f66 7265 7175 656e 6379     num_frequency
-0000fbe0: 5f70 6f69 6e74 733d 4e6f 6e65 2c0a 2020  _points=None,.  
-0000fbf0: 2020 2020 2020 6e75 6d5f 706f 696e 7473        num_points
-0000fc00: 5f69 6e5f 6261 7463 683d 4e6f 6e65 2c0a  _in_batch=None,.
-0000fc10: 2020 2020 2020 2020 6672 6571 7565 6e63          frequenc
-0000fc20: 795f 706f 696e 7473 5f61 745f 6261 6e64  y_points_at_band
-0000fc30: 733d 4661 6c73 652c 0a20 2020 2020 2020  s=False,.       
-0000fc40: 2073 6361 7474 6572 696e 675f 6576 656e   scattering_even
-0000fc50: 745f 636c 6173 733d 4e6f 6e65 2c0a 2020  t_class=None,.  
-0000fc60: 2020 2020 2020 7772 6974 655f 7478 743d        write_txt=
-0000fc70: 4661 6c73 652c 0a20 2020 2020 2020 2077  False,.        w
-0000fc80: 7269 7465 5f67 616d 6d61 5f64 6574 6169  rite_gamma_detai
-0000fc90: 6c3d 4661 6c73 652c 0a20 2020 2020 2020  l=False,.       
-0000fca0: 206b 6565 705f 6761 6d6d 615f 6465 7461   keep_gamma_deta
-0000fcb0: 696c 3d46 616c 7365 2c0a 2020 2020 2020  il=False,.      
-0000fcc0: 2020 6f75 7470 7574 5f66 696c 656e 616d    output_filenam
-0000fcd0: 653d 4e6f 6e65 2c0a 2020 2020 293a 0a20  e=None,.    ):. 
-0000fce0: 2020 2020 2020 2022 2222 4361 6c63 756c         """Calcul
-0000fcf0: 6174 6520 696d 6167 696e 6172 7920 7061  ate imaginary pa
-0000fd00: 7274 206f 6620 7365 6c66 2d65 6e65 7267  rt of self-energ
-0000fd10: 7920 6f66 2062 7562 626c 6520 6469 6167  y of bubble diag
-0000fd20: 7261 6d20 2847 616d 6d61 292e 0a0a 2020  ram (Gamma)...  
-0000fd30: 2020 2020 2020 5069 203d 2044 656c 7461        Pi = Delta
-0000fd40: 202d 2069 2047 616d 6d61 2e0a 0a20 2020   - i Gamma...   
-0000fd50: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-0000fd60: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-0000fd70: 2d2d 0a20 2020 2020 2020 2067 7269 645f  --.        grid_
-0000fd80: 706f 696e 7473 203a 2061 7272 6179 5f6c  points : array_l
-0000fd90: 696b 650a 2020 2020 2020 2020 2020 2020  ike.            
-0000fda0: 4772 6964 2d70 6f69 6e74 2069 6e64 6963  Grid-point indic
-0000fdb0: 6573 2077 6865 7265 2069 6d61 6769 6e61  es where imagina
-0000fdc0: 7279 2070 6172 7420 6f66 2073 656c 662d  ry part of self-
-0000fdd0: 656e 6572 6769 6573 2061 7265 0a20 2020  energies are.   
-0000fde0: 2020 2020 2020 2020 2063 6163 6c63 756c           caclcul
-0000fdf0: 6174 6564 2e0a 2020 2020 2020 2020 2020  ated..          
-0000fe00: 2020 6474 7970 653d 696e 742c 2073 6861    dtype=int, sha
-0000fe10: 7065 3d28 6772 6964 5f70 6f69 6e74 732c  pe=(grid_points,
-0000fe20: 290a 2020 2020 2020 2020 7465 6d70 6572  ).        temper
-0000fe30: 6174 7572 6573 203a 2061 7272 6179 5f6c  atures : array_l
-0000fe40: 696b 650a 2020 2020 2020 2020 2020 2020  ike.            
-0000fe50: 5465 6d70 6572 6174 7572 6573 2077 6865  Temperatures whe
-0000fe60: 7265 2069 6d61 6769 6e61 7279 2070 6172  re imaginary par
-0000fe70: 7420 6f66 2073 656c 662d 656e 6572 6769  t of self-energi
-0000fe80: 6573 2061 7265 2063 616c 6375 6c61 7465  es are calculate
-0000fe90: 642e 0a20 2020 2020 2020 2020 2020 2064  d..            d
-0000fea0: 7479 7065 3d66 6c6f 6174 2c20 7368 6170  type=float, shap
-0000feb0: 653d 2874 656d 7065 7261 7475 7265 732c  e=(temperatures,
-0000fec0: 290a 2020 2020 2020 2020 6672 6571 7565  ).        freque
-0000fed0: 6e63 795f 706f 696e 7473 203a 2061 7272  ncy_points : arr
-0000fee0: 6179 5f6c 696b 652c 206f 7074 696f 6e61  ay_like, optiona
-0000fef0: 6c0a 2020 2020 2020 2020 2020 2020 4672  l.            Fr
-0000ff00: 6571 7565 6e63 7920 7361 6d70 6c69 6e67  equency sampling
-0000ff10: 2070 6f69 6e74 732e 2044 6566 6175 6c74   points. Default
-0000ff20: 2069 7320 4e6f 6e65 2e20 5769 7468 0a20   is None. With. 
-0000ff30: 2020 2020 2020 2020 2020 2066 7265 7175             frequ
-0000ff40: 656e 6379 5f70 6f69 6e74 735f 6174 5f62  ency_points_at_b
-0000ff50: 616e 6473 3d46 616c 7365 2061 6e64 2066  ands=False and f
-0000ff60: 7265 7175 656e 6379 5f70 6f69 6e74 7320  requency_points 
-0000ff70: 6973 204e 6f6e 652c 0a20 2020 2020 2020  is None,.       
-0000ff80: 2020 2020 206e 756d 5f66 7265 7175 656e       num_frequen
-0000ff90: 6379 5f70 6f69 6e74 7320 6f72 2066 7265  cy_points or fre
-0000ffa0: 7175 656e 6379 5f73 7465 7020 6973 2075  quency_step is u
-0000ffb0: 7365 6420 746f 2067 656e 6572 6174 6520  sed to generate 
-0000ffc0: 756e 6966 6f72 6d0a 2020 2020 2020 2020  uniform.        
-0000ffd0: 2020 2020 6672 6571 7565 6e63 7920 7361      frequency sa
-0000ffe0: 6d70 6c69 6e67 2070 6f69 6e74 732e 0a20  mpling points.. 
-0000fff0: 2020 2020 2020 2020 2020 2064 7479 7065             dtype
-00010000: 3d66 6c6f 6174 2c20 7368 6170 653d 2866  =float, shape=(f
-00010010: 7265 7175 656e 6379 5f70 6f69 6e74 732c  requency_points,
-00010020: 290a 2020 2020 2020 2020 6672 6571 7565  ).        freque
-00010030: 6e63 795f 7374 6570 203a 2066 6c6f 6174  ncy_step : float
-00010040: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-00010050: 2020 2020 2020 2055 6e69 666f 726d 2070         Uniform p
-00010060: 6974 6368 206f 6620 6672 6571 7565 6e63  itch of frequenc
-00010070: 7920 7361 6d70 6c69 6e67 2070 6f69 6e74  y sampling point
-00010080: 732e 2044 6566 6175 6c74 2069 7320 4e6f  s. Default is No
-00010090: 6e65 2e20 5468 6973 0a20 2020 2020 2020  ne. This.       
-000100a0: 2020 2020 2072 6573 756c 7473 2069 6e20       results in 
-000100b0: 7573 696e 6720 6e75 6d5f 6672 6571 7565  using num_freque
-000100c0: 6e63 795f 706f 696e 7473 2e0a 2020 2020  ncy_points..    
-000100d0: 2020 2020 6e75 6d5f 6672 6571 7565 6e63      num_frequenc
-000100e0: 795f 706f 696e 7473 3a20 496e 742c 206f  y_points: Int, o
-000100f0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00010100: 2020 2020 4e75 6d62 6572 206f 6620 7361      Number of sa
-00010110: 6d70 6c69 6e67 2073 616d 706c 696e 6720  mpling sampling 
-00010120: 706f 696e 7473 2074 6f20 6265 2075 7365  points to be use
-00010130: 6420 696e 7374 6561 6420 6f66 0a20 2020  d instead of.   
-00010140: 2020 2020 2020 2020 2066 7265 7175 656e           frequen
-00010150: 6379 5f73 7465 702e 2054 6869 7320 6e75  cy_step. This nu
-00010160: 6d62 6572 2069 6e63 6c75 6465 7320 656e  mber includes en
-00010170: 6420 706f 696e 7473 2e20 4465 6661 756c  d points. Defaul
-00010180: 7420 6973 204e 6f6e 652c 0a20 2020 2020  t is None,.     
-00010190: 2020 2020 2020 2077 6869 6368 2067 6976         which giv
-000101a0: 6573 2032 3031 2e0a 2020 2020 2020 2020  es 201..        
-000101b0: 6e75 6d5f 706f 696e 7473 5f69 6e5f 6261  num_points_in_ba
-000101c0: 7463 683a 2069 6e74 2c20 6f70 7469 6f6e  tch: int, option
-000101d0: 616c 0a20 2020 2020 2020 2020 2020 204e  al.            N
-000101e0: 756d 6265 7220 6f66 2073 616d 706c 696e  umber of samplin
-000101f0: 6720 706f 696e 7473 2069 6e20 6f6e 6520  g points in one 
-00010200: 6261 7463 682e 2054 6869 7320 6973 2066  batch. This is f
-00010210: 6f72 2074 6865 2066 7265 7175 656e 6379  or the frequency
-00010220: 0a20 2020 2020 2020 2020 2020 2073 616d  .            sam
-00010230: 706c 696e 6720 6d6f 6465 2061 6e64 2074  pling mode and t
-00010240: 6865 2073 616d 706c 696e 6720 706f 696e  he sampling poin
-00010250: 7473 2061 7265 2064 6976 6964 6564 2069  ts are divided i
-00010260: 6e74 6f20 6261 7463 6865 732e 0a20 2020  nto batches..   
-00010270: 2020 2020 2020 2020 204c 6167 6572 206e           Lager n
-00010280: 756d 6265 7220 7072 6f76 6964 6573 2065  umber provides e
-00010290: 6666 6963 6965 6e74 2075 7365 206f 6620  fficient use of 
-000102a0: 6d75 6c74 692d 636f 7265 7320 6275 7420  multi-cores but 
-000102b0: 6d6f 7265 0a20 2020 2020 2020 2020 2020  more.           
-000102c0: 206d 656d 6f72 7920 6465 6d61 6e64 696e   memory demandin
-000102d0: 672e 2044 6566 6175 6c74 2069 7320 4e6f  g. Default is No
-000102e0: 6e65 2c20 7768 6963 6820 6769 7665 2074  ne, which give t
-000102f0: 6865 206e 756d 6265 7220 6f66 2031 302e  he number of 10.
-00010300: 0a20 2020 2020 2020 2066 7265 7175 656e  .        frequen
-00010310: 6379 5f70 6f69 6e74 735f 6174 5f62 616e  cy_points_at_ban
-00010320: 6473 203a 2062 6f6f 6c2c 206f 7074 696f  ds : bool, optio
-00010330: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
-00010340: 5068 6f6e 6f6e 2062 616e 6420 6672 6571  Phonon band freq
-00010350: 7565 6e63 6965 7320 6172 6520 7573 6564  uencies are used
-00010360: 2061 7320 6672 6571 7565 6e63 7920 706f   as frequency po
-00010370: 696e 7473 2077 6865 6e20 5472 7565 2e0a  ints when True..
-00010380: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
-00010390: 756c 7420 6973 2046 616c 7365 2e0a 2020  ult is False..  
-000103a0: 2020 2020 2020 7363 6174 7465 7269 6e67        scattering
-000103b0: 5f65 7665 6e74 5f63 6c61 7373 203a 2069  _event_class : i
-000103c0: 6e74 2c20 6f70 7469 6f6e 616c 0a20 2020  nt, optional.   
-000103d0: 2020 2020 2020 2020 2053 7065 6369 6669           Specifi
-000103e0: 6320 6368 6f69 6365 206f 6620 7363 6174  c choice of scat
-000103f0: 7465 7269 6e67 2065 7665 6e74 2063 6c61  tering event cla
-00010400: 7373 2c20 3120 6f72 2032 2074 6861 7420  ss, 1 or 2 that 
-00010410: 6973 2073 7065 6369 6669 6564 0a20 2020  is specified.   
-00010420: 2020 2020 2020 2020 2031 206f 7220 322c           1 or 2,
-00010430: 2072 6573 7065 6374 6976 656c 792e 2054   respectively. T
-00010440: 6865 2072 6573 756c 7420 6973 2073 746f  he result is sto
-00010450: 7265 6420 696e 2067 616d 6d61 732e 2054  red in gammas. T
-00010460: 6865 7265 666f 7265 0a20 2020 2020 2020  herefore.       
-00010470: 2020 2020 2075 7375 616c 2067 616d 6d61       usual gamma
-00010480: 7320 6172 6520 6e6f 7420 7374 6f72 6564  s are not stored
-00010490: 2069 6e20 7468 6520 7661 7269 6162 6c65   in the variable
-000104a0: 2e20 4465 6661 756c 7420 6973 204e 6f6e  . Default is Non
-000104b0: 652c 2077 6869 6368 0a20 2020 2020 2020  e, which.       
-000104c0: 2020 2020 2064 6f65 736e 2774 2073 7065       doesn't spe
-000104d0: 6369 6679 2073 6361 7474 6572 696e 675f  cify scattering_
-000104e0: 6576 656e 745f 636c 6173 732e 0a20 2020  event_class..   
-000104f0: 2020 2020 2077 7269 7465 5f74 7874 203a       write_txt :
-00010500: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0a   bool, optional.
-00010510: 2020 2020 2020 2020 2020 2020 4672 6571              Freq
-00010520: 7565 6e63 7920 706f 696e 7473 2061 6e64  uency points and
-00010530: 2069 6d61 6769 6e61 7279 2070 6172 7420   imaginary part 
-00010540: 6f66 2073 656c 662d 656e 6572 6769 6573  of self-energies
-00010550: 2061 7265 2077 7269 7474 656e 0a20 2020   are written.   
-00010560: 2020 2020 2020 2020 2069 6e74 6f20 7465           into te
-00010570: 7874 2066 696c 6573 2e0a 2020 2020 2020  xt files..      
-00010580: 2020 7772 6974 655f 6761 6d6d 615f 6465    write_gamma_de
-00010590: 7461 696c 203a 2062 6f6f 6c2c 206f 7074  tail : bool, opt
-000105a0: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
-000105b0: 2020 4465 7461 696c 6564 2067 616d 6d61    Detailed gamma
-000105c0: 7320 6172 6520 7772 6974 7465 6e20 696e  s are written in
-000105d0: 746f 2061 2066 696c 6520 696e 2068 6466  to a file in hdf
-000105e0: 352e 2044 6566 6175 6c74 2069 7320 4661  5. Default is Fa
-000105f0: 6c73 652e 0a20 2020 2020 2020 206b 6565  lse..        kee
-00010600: 705f 6761 6d6d 615f 6465 7461 696c 203a  p_gamma_detail :
-00010610: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0a   bool, optional.
-00010620: 2020 2020 2020 2020 2020 2020 5769 7468              With
-00010630: 2054 7275 652c 2064 6574 6169 6c65 6420   True, detailed 
-00010640: 6761 6d6d 6173 2061 7265 2073 746f 7265  gammas are store
-00010650: 642e 2044 6566 6175 6c74 2069 7320 4661  d. Default is Fa
-00010660: 6c73 652e 0a20 2020 2020 2020 206f 7574  lse..        out
-00010670: 7075 745f 6669 6c65 6e61 6d65 203a 2073  put_filename : s
-00010680: 7472 0a20 2020 2020 2020 2020 2020 2054  tr.            T
-00010690: 6869 7320 7374 7269 6e67 2069 7320 696e  his string is in
-000106a0: 7365 7274 6564 2069 6e20 7468 6520 6f75  serted in the ou
-000106b0: 7470 7574 2066 696c 6520 6e61 6d65 732e  tput file names.
-000106c0: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-000106d0: 2020 2020 2020 6966 2073 656c 662e 5f69        if self._i
-000106e0: 6e74 6572 6163 7469 6f6e 2069 7320 4e6f  nteraction is No
-000106f0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00010700: 6d73 6720 3d20 280a 2020 2020 2020 2020  msg = (.        
-00010710: 2020 2020 2020 2020 2250 686f 6e6f 3370          "Phono3p
-00010720: 792e 696e 6974 5f70 6870 685f 696e 7465  y.init_phph_inte
-00010730: 7261 6374 696f 6e20 6861 7320 746f 2062  raction has to b
-00010740: 6520 6361 6c6c 6564 2022 0a20 2020 2020  e called ".     
-00010750: 2020 2020 2020 2020 2020 2022 6265 666f             "befo
-00010760: 7265 2072 756e 6e69 6e67 2074 6869 7320  re running this 
-00010770: 6d65 7468 6f64 2e22 0a20 2020 2020 2020  method.".       
-00010780: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00010790: 2020 2072 6169 7365 2052 756e 7469 6d65     raise Runtime
-000107a0: 4572 726f 7228 6d73 6729 0a0a 2020 2020  Error(msg)..    
-000107b0: 2020 2020 6966 2074 656d 7065 7261 7475      if temperatu
-000107c0: 7265 7320 6973 204e 6f6e 653a 0a20 2020  res is None:.   
-000107d0: 2020 2020 2020 2020 2073 656c 662e 5f74           self._t
-000107e0: 656d 7065 7261 7475 7265 7320 3d20 5b0a  emperatures = [.
-000107f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010800: 3330 302e 302c 0a20 2020 2020 2020 2020  300.0,.         
-00010810: 2020 205d 0a20 2020 2020 2020 2065 6c73     ].        els
-00010820: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00010830: 656c 662e 5f74 656d 7065 7261 7475 7265  elf._temperature
-00010840: 7320 3d20 7465 6d70 6572 6174 7572 6573  s = temperatures
-00010850: 0a20 2020 2020 2020 2073 656c 662e 5f67  .        self._g
-00010860: 7269 645f 706f 696e 7473 203d 2067 7269  rid_points = gri
-00010870: 645f 706f 696e 7473 0a20 2020 2020 2020  d_points.       
-00010880: 2073 656c 662e 5f73 6361 7474 6572 696e   self._scatterin
-00010890: 675f 6576 656e 745f 636c 6173 7320 3d20  g_event_class = 
-000108a0: 7363 6174 7465 7269 6e67 5f65 7665 6e74  scattering_event
-000108b0: 5f63 6c61 7373 0a20 2020 2020 2020 2076  _class.        v
-000108c0: 616c 7320 3d20 6765 745f 696d 6167 5f73  als = get_imag_s
-000108d0: 656c 665f 656e 6572 6779 280a 2020 2020  elf_energy(.    
-000108e0: 2020 2020 2020 2020 7365 6c66 2e5f 696e          self._in
-000108f0: 7465 7261 6374 696f 6e2c 0a20 2020 2020  teraction,.     
-00010900: 2020 2020 2020 2067 7269 645f 706f 696e         grid_poin
-00010910: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
-00010920: 7465 6d70 6572 6174 7572 6573 2c0a 2020  temperatures,.  
-00010930: 2020 2020 2020 2020 2020 7369 676d 6173            sigmas
-00010940: 3d73 656c 662e 5f73 6967 6d61 732c 0a20  =self._sigmas,. 
-00010950: 2020 2020 2020 2020 2020 2066 7265 7175             frequ
-00010960: 656e 6379 5f70 6f69 6e74 733d 6672 6571  ency_points=freq
-00010970: 7565 6e63 795f 706f 696e 7473 2c0a 2020  uency_points,.  
-00010980: 2020 2020 2020 2020 2020 6672 6571 7565            freque
-00010990: 6e63 795f 7374 6570 3d66 7265 7175 656e  ncy_step=frequen
-000109a0: 6379 5f73 7465 702c 0a20 2020 2020 2020  cy_step,.       
-000109b0: 2020 2020 2066 7265 7175 656e 6379 5f70       frequency_p
-000109c0: 6f69 6e74 735f 6174 5f62 616e 6473 3d66  oints_at_bands=f
-000109d0: 7265 7175 656e 6379 5f70 6f69 6e74 735f  requency_points_
-000109e0: 6174 5f62 616e 6473 2c0a 2020 2020 2020  at_bands,.      
-000109f0: 2020 2020 2020 6e75 6d5f 6672 6571 7565        num_freque
-00010a00: 6e63 795f 706f 696e 7473 3d6e 756d 5f66  ncy_points=num_f
-00010a10: 7265 7175 656e 6379 5f70 6f69 6e74 732c  requency_points,
-00010a20: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
-00010a30: 5f70 6f69 6e74 735f 696e 5f62 6174 6368  _points_in_batch
-00010a40: 3d6e 756d 5f70 6f69 6e74 735f 696e 5f62  =num_points_in_b
-00010a50: 6174 6368 2c0a 2020 2020 2020 2020 2020  atch,.          
-00010a60: 2020 7363 6174 7465 7269 6e67 5f65 7665    scattering_eve
-00010a70: 6e74 5f63 6c61 7373 3d73 6361 7474 6572  nt_class=scatter
-00010a80: 696e 675f 6576 656e 745f 636c 6173 732c  ing_event_class,
-00010a90: 0a20 2020 2020 2020 2020 2020 2077 7269  .            wri
-00010aa0: 7465 5f67 616d 6d61 5f64 6574 6169 6c3d  te_gamma_detail=
-00010ab0: 7772 6974 655f 6761 6d6d 615f 6465 7461  write_gamma_deta
-00010ac0: 696c 2c0a 2020 2020 2020 2020 2020 2020  il,.            
-00010ad0: 7265 7475 726e 5f67 616d 6d61 5f64 6574  return_gamma_det
-00010ae0: 6169 6c3d 6b65 6570 5f67 616d 6d61 5f64  ail=keep_gamma_d
-00010af0: 6574 6169 6c2c 0a20 2020 2020 2020 2020  etail,.         
-00010b00: 2020 206f 7574 7075 745f 6669 6c65 6e61     output_filena
-00010b10: 6d65 3d6f 7574 7075 745f 6669 6c65 6e61  me=output_filena
-00010b20: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-00010b30: 6c6f 675f 6c65 7665 6c3d 7365 6c66 2e5f  log_level=self._
-00010b40: 6c6f 675f 6c65 7665 6c2c 0a20 2020 2020  log_level,.     
-00010b50: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
-00010b60: 6b65 6570 5f67 616d 6d61 5f64 6574 6169  keep_gamma_detai
-00010b70: 6c3a 0a20 2020 2020 2020 2020 2020 2028  l:.            (
-00010b80: 7365 6c66 2e5f 6672 6571 7565 6e63 795f  self._frequency_
-00010b90: 706f 696e 7473 2c20 7365 6c66 2e5f 6761  points, self._ga
-00010ba0: 6d6d 6173 2c20 7365 6c66 2e5f 6465 7461  mmas, self._deta
-00010bb0: 696c 6564 5f67 616d 6d61 7329 203d 2076  iled_gammas) = v
-00010bc0: 616c 730a 2020 2020 2020 2020 656c 7365  als.        else
-00010bd0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00010be0: 6c66 2e5f 6672 6571 7565 6e63 795f 706f  lf._frequency_po
-00010bf0: 696e 7473 2c20 7365 6c66 2e5f 6761 6d6d  ints, self._gamm
-00010c00: 6173 203d 2076 616c 730a 0a20 2020 2020  as = vals..     
-00010c10: 2020 2069 6620 7772 6974 655f 7478 743a     if write_txt:
-00010c20: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00010c30: 662e 5f77 7269 7465 5f69 6d61 675f 7365  f._write_imag_se
-00010c40: 6c66 5f65 6e65 7267 7928 6f75 7470 7574  lf_energy(output
-00010c50: 5f66 696c 656e 616d 653d 6f75 7470 7574  _filename=output
-00010c60: 5f66 696c 656e 616d 6529 0a0a 2020 2020  _filename)..    
-00010c70: 2020 2020 7265 7475 726e 2076 616c 730a      return vals.
-00010c80: 0a20 2020 2064 6566 2077 7269 7465 5f69  .    def write_i
-00010c90: 6d61 675f 7365 6c66 5f65 6e65 7267 7928  mag_self_energy(
-00010ca0: 7365 6c66 2c20 6669 6c65 6e61 6d65 3d4e  self, filename=N
-00010cb0: 6f6e 6529 3a0a 2020 2020 2020 2020 2222  one):.        ""
-00010cc0: 2257 7269 7465 2069 6d61 6769 6e61 7279  "Write imaginary
-00010cd0: 2070 6172 7420 6f66 2073 656c 6620 656e   part of self en
-00010ce0: 6572 6779 2074 6f20 6120 6669 6c65 2e22  ergy to a file."
-00010cf0: 2222 0a20 2020 2020 2020 2077 6172 6e69  "".        warni
-00010d00: 6e67 732e 7761 726e 280a 2020 2020 2020  ngs.warn(.      
-00010d10: 2020 2020 2020 2250 686f 6e6f 3370 792e        "Phono3py.
-00010d20: 7772 6974 655f 696d 6167 5f73 656c 665f  write_imag_self_
-00010d30: 656e 6572 6779 2069 7320 6465 7072 6563  energy is deprec
-00010d40: 6174 6564 2e22 0a20 2020 2020 2020 2020  ated.".         
-00010d50: 2020 2022 5573 6520 5068 6f6e 6f33 7079     "Use Phono3py
-00010d60: 2e72 756e 5f69 6d61 675f 7365 6c66 5f65  .run_imag_self_e
-00010d70: 6e65 7267 7920 7769 7468 2077 7269 7465  nergy with write
-00010d80: 5f74 7874 3d54 7275 652e 222c 0a20 2020  _txt=True.",.   
-00010d90: 2020 2020 2020 2020 2044 6570 7265 6361           Depreca
-00010da0: 7469 6f6e 5761 726e 696e 672c 0a20 2020  tionWarning,.   
-00010db0: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
-00010dc0: 656c 662e 5f77 7269 7465 5f69 6d61 675f  elf._write_imag_
-00010dd0: 7365 6c66 5f65 6e65 7267 7928 6f75 7470  self_energy(outp
-00010de0: 7574 5f66 696c 656e 616d 653d 6669 6c65  ut_filename=file
-00010df0: 6e61 6d65 290a 0a20 2020 2064 6566 205f  name)..    def _
-00010e00: 7772 6974 655f 696d 6167 5f73 656c 665f  write_imag_self_
-00010e10: 656e 6572 6779 2873 656c 662c 206f 7574  energy(self, out
-00010e20: 7075 745f 6669 6c65 6e61 6d65 3d4e 6f6e  put_filename=Non
-00010e30: 6529 3a0a 2020 2020 2020 2020 7772 6974  e):.        writ
-00010e40: 655f 696d 6167 5f73 656c 665f 656e 6572  e_imag_self_ener
-00010e50: 6779 280a 2020 2020 2020 2020 2020 2020  gy(.            
-00010e60: 7365 6c66 2e5f 6761 6d6d 6173 2c0a 2020  self._gammas,.  
-00010e70: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00010e80: 6573 685f 6e75 6d62 6572 732c 0a20 2020  esh_numbers,.   
-00010e90: 2020 2020 2020 2020 2073 656c 662e 5f67           self._g
-00010ea0: 7269 645f 706f 696e 7473 2c0a 2020 2020  rid_points,.    
-00010eb0: 2020 2020 2020 2020 7365 6c66 2e5f 6261          self._ba
-00010ec0: 6e64 5f69 6e64 6963 6573 2c0a 2020 2020  nd_indices,.    
-00010ed0: 2020 2020 2020 2020 7365 6c66 2e5f 6672          self._fr
-00010ee0: 6571 7565 6e63 795f 706f 696e 7473 2c0a  equency_points,.
-00010ef0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010f00: 2e5f 7465 6d70 6572 6174 7572 6573 2c0a  ._temperatures,.
-00010f10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010f20: 2e5f 7369 676d 6173 2c0a 2020 2020 2020  ._sigmas,.      
-00010f30: 2020 2020 2020 7363 6174 7465 7269 6e67        scattering
-00010f40: 5f65 7665 6e74 5f63 6c61 7373 3d73 656c  _event_class=sel
-00010f50: 662e 5f73 6361 7474 6572 696e 675f 6576  f._scattering_ev
-00010f60: 656e 745f 636c 6173 732c 0a20 2020 2020  ent_class,.     
-00010f70: 2020 2020 2020 206f 7574 7075 745f 6669         output_fi
-00010f80: 6c65 6e61 6d65 3d6f 7574 7075 745f 6669  lename=output_fi
-00010f90: 6c65 6e61 6d65 2c0a 2020 2020 2020 2020  lename,.        
-00010fa0: 2020 2020 6973 5f6d 6573 685f 7379 6d6d      is_mesh_symm
-00010fb0: 6574 7279 3d73 656c 662e 5f69 735f 6d65  etry=self._is_me
-00010fc0: 7368 5f73 796d 6d65 7472 792c 0a20 2020  sh_symmetry,.   
-00010fd0: 2020 2020 2020 2020 206c 6f67 5f6c 6576           log_lev
-00010fe0: 656c 3d73 656c 662e 5f6c 6f67 5f6c 6576  el=self._log_lev
-00010ff0: 656c 2c0a 2020 2020 2020 2020 290a 0a20  el,.        ).. 
-00011000: 2020 2064 6566 2072 756e 5f72 6561 6c5f     def run_real_
-00011010: 7365 6c66 5f65 6e65 7267 7928 0a20 2020  self_energy(.   
-00011020: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00011030: 2020 2067 7269 645f 706f 696e 7473 2c0a     grid_points,.
-00011040: 2020 2020 2020 2020 7465 6d70 6572 6174          temperat
-00011050: 7572 6573 2c0a 2020 2020 2020 2020 6672  ures,.        fr
-00011060: 6571 7565 6e63 795f 706f 696e 7473 5f61  equency_points_a
-00011070: 745f 6261 6e64 733d 4661 6c73 652c 0a20  t_bands=False,. 
-00011080: 2020 2020 2020 2066 7265 7175 656e 6379         frequency
-00011090: 5f70 6f69 6e74 733d 4e6f 6e65 2c0a 2020  _points=None,.  
-000110a0: 2020 2020 2020 6672 6571 7565 6e63 795f        frequency_
-000110b0: 7374 6570 3d4e 6f6e 652c 0a20 2020 2020  step=None,.     
-000110c0: 2020 206e 756d 5f66 7265 7175 656e 6379     num_frequency
-000110d0: 5f70 6f69 6e74 733d 4e6f 6e65 2c0a 2020  _points=None,.  
-000110e0: 2020 2020 2020 6570 7369 6c6f 6e73 3d4e        epsilons=N
-000110f0: 6f6e 652c 0a20 2020 2020 2020 2077 7269  one,.        wri
-00011100: 7465 5f74 7874 3d46 616c 7365 2c0a 2020  te_txt=False,.  
-00011110: 2020 2020 2020 7772 6974 655f 6864 6635        write_hdf5
-00011120: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-00011130: 6f75 7470 7574 5f66 696c 656e 616d 653d  output_filename=
-00011140: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-00011150: 2020 2020 2022 2222 4361 6c63 756c 6174       """Calculat
-00011160: 6520 7265 616c 2d70 6172 7420 6f66 2073  e real-part of s
-00011170: 656c 662d 656e 6572 6779 206f 6620 6275  elf-energy of bu
-00011180: 6262 6c65 2064 6961 6772 616d 2028 4465  bble diagram (De
-00011190: 6c74 6129 2e0a 0a20 2020 2020 2020 2050  lta)...        P
-000111a0: 6920 3d20 4465 6c74 6120 2d20 6920 4761  i = Delta - i Ga
-000111b0: 6d6d 612e 0a0a 2020 2020 2020 2020 5061  mma...        Pa
-000111c0: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-000111d0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-000111e0: 2020 2020 6772 6964 5f70 6f69 6e74 7320      grid_points 
-000111f0: 3a20 6172 7261 795f 6c69 6b65 0a20 2020  : array_like.   
-00011200: 2020 2020 2020 2020 2047 7269 642d 706f           Grid-po
-00011210: 696e 7420 696e 6469 6365 7320 7768 6572  int indices wher
-00011220: 6520 7265 616c 2070 6172 7420 6f66 2073  e real part of s
-00011230: 656c 662d 656e 6572 6769 6573 2061 7265  elf-energies are
-00011240: 0a20 2020 2020 2020 2020 2020 2063 6163  .            cac
-00011250: 6c63 756c 6174 6564 2e0a 2020 2020 2020  lculated..      
-00011260: 2020 2020 2020 6474 7970 653d 696e 742c        dtype=int,
-00011270: 2073 6861 7065 3d28 6772 6964 5f70 6f69   shape=(grid_poi
-00011280: 6e74 732c 290a 2020 2020 2020 2020 7465  nts,).        te
-00011290: 6d70 6572 6174 7572 6573 203a 2061 7272  mperatures : arr
-000112a0: 6179 5f6c 696b 650a 2020 2020 2020 2020  ay_like.        
-000112b0: 2020 2020 5465 6d70 6572 6174 7572 6573      Temperatures
-000112c0: 2077 6865 7265 2072 6561 6c20 7061 7274   where real part
-000112d0: 206f 6620 7365 6c66 2d65 6e65 7267 6965   of self-energie
-000112e0: 7320 2061 7265 2063 616c 6375 6c61 7465  s  are calculate
-000112f0: 642e 0a20 2020 2020 2020 2020 2020 2064  d..            d
-00011300: 7479 7065 3d66 6c6f 6174 2c20 7368 6170  type=float, shap
-00011310: 653d 2874 656d 7065 7261 7475 7265 732c  e=(temperatures,
-00011320: 290a 2020 2020 2020 2020 6672 6571 7565  ).        freque
-00011330: 6e63 795f 706f 696e 7473 5f61 745f 6261  ncy_points_at_ba
-00011340: 6e64 7320 3a20 626f 6f6c 2c20 6f70 7469  nds : bool, opti
-00011350: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
-00011360: 2057 6974 6820 4661 6c73 652c 2066 7265   With False, fre
-00011370: 7175 656e 6379 2073 6869 6674 7320 6172  quency shifts ar
-00011380: 6520 6361 6c63 756c 6174 6564 2061 7420  e calculated at 
-00011390: 6672 7175 656e 6379 2073 616d 706c 696e  frquency samplin
-000113a0: 670a 2020 2020 2020 2020 2020 2020 706f  g.            po
-000113b0: 696e 7473 2e20 5768 656e 2054 7275 652c  ints. When True,
-000113c0: 2074 6865 7920 6172 6520 646f 6e65 2061   they are done a
-000113d0: 7420 7468 6520 7068 6f6e 6f6e 2066 7265  t the phonon fre
-000113e0: 7175 656e 6369 6573 2e0a 2020 2020 2020  quencies..      
-000113f0: 2020 2020 2020 4465 6661 756c 7420 6973        Default is
-00011400: 2046 616c 7365 2e0a 2020 2020 2020 2020   False..        
-00011410: 6672 6571 7565 6e63 795f 706f 696e 7473  frequency_points
-00011420: 203a 2061 7272 6179 5f6c 696b 652c 206f   : array_like, o
-00011430: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00011440: 2020 2020 4672 6571 7565 6e63 7920 7361      Frequency sa
-00011450: 6d70 6c69 6e67 2070 6f69 6e74 732e 2044  mpling points. D
-00011460: 6566 6175 6c74 2069 7320 4e6f 6e65 2e20  efault is None. 
-00011470: 496e 2074 6869 7320 6361 7365 2c0a 2020  In this case,.  
-00011480: 2020 2020 2020 2020 2020 6e75 6d5f 6672            num_fr
-00011490: 6571 7565 6e63 795f 706f 696e 7473 206f  equency_points o
-000114a0: 7220 6672 6571 7565 6e63 795f 7374 6570  r frequency_step
-000114b0: 2069 7320 7573 6564 2074 6f20 6765 6e65   is used to gene
-000114c0: 7261 7465 2075 6e69 666f 726d 0a20 2020  rate uniform.   
-000114d0: 2020 2020 2020 2020 2066 7265 7175 656e           frequen
-000114e0: 6379 2073 616d 706c 696e 6720 706f 696e  cy sampling poin
-000114f0: 7473 2e0a 2020 2020 2020 2020 2020 2020  ts..            
-00011500: 6474 7970 653d 666c 6f61 742c 2073 6861  dtype=float, sha
-00011510: 7065 3d28 6672 6571 7565 6e63 795f 706f  pe=(frequency_po
-00011520: 696e 7473 2c29 0a20 2020 2020 2020 2066  ints,).        f
-00011530: 7265 7175 656e 6379 5f73 7465 7020 3a20  requency_step : 
-00011540: 666c 6f61 742c 206f 7074 696f 6e61 6c0a  float, optional.
-00011550: 2020 2020 2020 2020 2020 2020 556e 6966              Unif
-00011560: 6f72 6d20 7069 7463 6820 6f66 2066 7265  orm pitch of fre
-00011570: 7175 656e 6379 2073 616d 706c 696e 6720  quency sampling 
-00011580: 706f 696e 7473 2e20 4465 6661 756c 7420  points. Default 
-00011590: 6973 204e 6f6e 652e 2054 6869 730a 2020  is None. This.  
-000115a0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000115b0: 7320 696e 2075 7369 6e67 206e 756d 5f66  s in using num_f
-000115c0: 7265 7175 656e 6379 5f70 6f69 6e74 732e  requency_points.
-000115d0: 0a20 2020 2020 2020 206e 756d 5f66 7265  .        num_fre
-000115e0: 7175 656e 6379 5f70 6f69 6e74 733a 2049  quency_points: I
-000115f0: 6e74 2c20 6f70 7469 6f6e 616c 0a20 2020  nt, optional.   
-00011600: 2020 2020 2020 2020 204e 756d 6265 7220           Number 
-00011610: 6f66 2073 616d 706c 696e 6720 7361 6d70  of sampling samp
-00011620: 6c69 6e67 2070 6f69 6e74 7320 746f 2062  ling points to b
-00011630: 6520 7573 6564 2069 6e73 7465 6164 206f  e used instead o
-00011640: 660a 2020 2020 2020 2020 2020 2020 6672  f.            fr
-00011650: 6571 7565 6e63 795f 7374 6570 2e20 5468  equency_step. Th
-00011660: 6973 206e 756d 6265 7220 696e 636c 7564  is number includ
-00011670: 6573 2065 6e64 2070 6f69 6e74 732e 2044  es end points. D
-00011680: 6566 6175 6c74 2069 7320 4e6f 6e65 2c0a  efault is None,.
-00011690: 2020 2020 2020 2020 2020 2020 7768 6963              whic
-000116a0: 6820 6769 7665 7320 3230 312e 0a20 2020  h gives 201..   
-000116b0: 2020 2020 2065 7073 696c 6f6e 7320 3a20       epsilons : 
-000116c0: 6172 7261 795f 6c69 6b65 0a20 2020 2020  array_like.     
-000116d0: 2020 2020 2020 2053 6d65 6172 696e 6720         Smearing 
-000116e0: 7769 6474 6873 2074 6f20 636f 6d70 7574  widths to comput
-000116f0: 6572 2070 7269 6e63 6970 616c 2070 6172  er principal par
-00011700: 742e 2057 6865 6e20 6d75 6c74 6970 6c65  t. When multiple
-00011710: 2076 616c 7565 730a 2020 2020 2020 2020   values.        
-00011720: 2020 2020 6172 6520 6769 7665 6e20 6672      are given fr
-00011730: 6571 7565 6e63 7920 7368 6966 7473 2066  equency shifts f
-00011740: 6f72 2074 686f 7365 2076 616c 7565 7320  or those values 
-00011750: 6172 6520 7265 7475 726e 6564 2e0a 2020  are returned..  
-00011760: 2020 2020 2020 2020 2020 6474 7970 653d            dtype=
-00011770: 666c 6f61 742c 2073 6861 7065 3d28 6570  float, shape=(ep
-00011780: 7369 6c6f 6e73 2c29 0a20 2020 2020 2020  silons,).       
-00011790: 2077 7269 7465 5f74 7874 203a 2062 6f6f   write_txt : boo
-000117a0: 6c2c 206f 7074 696f 6e61 6c0a 2020 2020  l, optional.    
-000117b0: 2020 2020 2020 2020 4672 6571 7565 6e63          Frequenc
-000117c0: 7920 706f 696e 7473 2061 6e64 2072 6561  y points and rea
-000117d0: 6c20 7061 7274 206f 6620 7365 6c66 2d65  l part of self-e
-000117e0: 6e65 7267 6965 7320 6172 6520 7772 6974  nergies are writ
-000117f0: 7465 6e0a 2020 2020 2020 2020 2020 2020  ten.            
-00011800: 696e 746f 2074 6578 7420 6669 6c65 732e  into text files.
-00011810: 0a20 2020 2020 2020 2077 7269 7465 5f68  .        write_h
-00011820: 6466 3520 3a20 626f 6f6c 0a20 2020 2020  df5 : bool.     
-00011830: 2020 2020 2020 2052 6573 756c 7473 2061         Results a
-00011840: 7265 2073 746f 7265 6420 696e 2068 6466  re stored in hdf
-00011850: 3520 6669 6c65 7320 696e 6465 7065 6e64  5 files independ
-00011860: 656e 746c 7920 6174 2067 7269 6420 706f  ently at grid po
-00011870: 696e 7473 2c0a 2020 2020 2020 2020 2020  ints,.          
-00011880: 2020 6570 7369 6c6f 6e73 2c20 616e 6420    epsilons, and 
-00011890: 7465 6d70 6572 6174 7572 6573 2e0a 2020  temperatures..  
-000118a0: 2020 2020 2020 6f75 7470 7574 5f66 696c        output_fil
-000118b0: 656e 616d 6520 3a20 7374 720a 2020 2020  ename : str.    
-000118c0: 2020 2020 2020 2020 5468 6973 2073 7472          This str
-000118d0: 696e 6720 6973 2069 6e73 6572 7465 6420  ing is inserted 
-000118e0: 696e 2074 6865 206f 7574 7075 7420 6669  in the output fi
-000118f0: 6c65 206e 616d 6573 2e0a 0a20 2020 2020  le names...     
-00011900: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-00011910: 6620 7365 6c66 2e5f 696e 7465 7261 6374  f self._interact
-00011920: 696f 6e20 6973 204e 6f6e 653a 0a20 2020  ion is None:.   
-00011930: 2020 2020 2020 2020 206d 7367 203d 2028           msg = (
-00011940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011950: 2022 5068 6f6e 6f33 7079 2e69 6e69 745f   "Phono3py.init_
-00011960: 7068 7068 5f69 6e74 6572 6163 7469 6f6e  phph_interaction
-00011970: 2068 6173 2074 6f20 6265 2063 616c 6c65   has to be calle
-00011980: 6420 220a 2020 2020 2020 2020 2020 2020  d ".            
-00011990: 2020 2020 2262 6566 6f72 6520 7275 6e6e      "before runn
-000119a0: 696e 6720 7468 6973 206d 6574 686f 642e  ing this method.
-000119b0: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
-000119c0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000119d0: 6520 5275 6e74 696d 6545 7272 6f72 286d  e RuntimeError(m
-000119e0: 7367 290a 0a20 2020 2020 2020 2069 6620  sg)..        if 
-000119f0: 6570 7369 6c6f 6e73 2069 7320 6e6f 7420  epsilons is not 
-00011a00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00011a10: 2020 5f65 7073 696c 6f6e 7320 3d20 6570    _epsilons = ep
-00011a20: 7369 6c6f 6e73 0a20 2020 2020 2020 2065  silons.        e
-00011a30: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00011a40: 2069 6620 6c65 6e28 7365 6c66 2e5f 7369   if len(self._si
-00011a50: 676d 6173 2920 3d3d 2031 2061 6e64 2073  gmas) == 1 and s
-00011a60: 656c 662e 5f73 6967 6d61 735b 305d 2069  elf._sigmas[0] i
-00011a70: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00011a80: 2020 2020 2020 2020 5f65 7073 696c 6f6e          _epsilon
-00011a90: 7320 3d20 4e6f 6e65 0a20 2020 2020 2020  s = None.       
-00011aa0: 2020 2020 2065 6c69 6620 7365 6c66 2e5f       elif self._
-00011ab0: 7369 676d 6173 5b30 5d20 6973 204e 6f6e  sigmas[0] is Non
-00011ac0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00011ad0: 2020 205f 6570 7369 6c6f 6e73 203d 2073     _epsilons = s
-00011ae0: 656c 662e 5f73 6967 6d61 735b 313a 5d0a  elf._sigmas[1:].
-00011af0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00011b00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00011b10: 2020 5f65 7073 696c 6f6e 7320 3d20 7365    _epsilons = se
-00011b20: 6c66 2e5f 7369 676d 6173 0a0a 2020 2020  lf._sigmas..    
-00011b30: 2020 2020 2320 2865 7073 696c 6f6e 2c20      # (epsilon, 
-00011b40: 6772 6964 5f70 6f69 6e74 2c20 7465 6d70  grid_point, temp
-00011b50: 6572 6174 7572 652c 2062 616e 6429 0a20  erature, band). 
-00011b60: 2020 2020 2020 2066 7265 7175 656e 6379         frequency
-00011b70: 5f70 6f69 6e74 732c 2064 656c 7461 7320  _points, deltas 
-00011b80: 3d20 6765 745f 7265 616c 5f73 656c 665f  = get_real_self_
-00011b90: 656e 6572 6779 280a 2020 2020 2020 2020  energy(.        
-00011ba0: 2020 2020 7365 6c66 2e5f 696e 7465 7261      self._intera
-00011bb0: 6374 696f 6e2c 0a20 2020 2020 2020 2020  ction,.         
-00011bc0: 2020 2067 7269 645f 706f 696e 7473 2c0a     grid_points,.
-00011bd0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-00011be0: 6572 6174 7572 6573 2c0a 2020 2020 2020  eratures,.      
-00011bf0: 2020 2020 2020 6570 7369 6c6f 6e73 3d5f        epsilons=_
-00011c00: 6570 7369 6c6f 6e73 2c0a 2020 2020 2020  epsilons,.      
-00011c10: 2020 2020 2020 6672 6571 7565 6e63 795f        frequency_
-00011c20: 706f 696e 7473 3d66 7265 7175 656e 6379  points=frequency
-00011c30: 5f70 6f69 6e74 732c 0a20 2020 2020 2020  _points,.       
-00011c40: 2020 2020 2066 7265 7175 656e 6379 5f73       frequency_s
-00011c50: 7465 703d 6672 6571 7565 6e63 795f 7374  tep=frequency_st
-00011c60: 6570 2c0a 2020 2020 2020 2020 2020 2020  ep,.            
-00011c70: 6e75 6d5f 6672 6571 7565 6e63 795f 706f  num_frequency_po
-00011c80: 696e 7473 3d6e 756d 5f66 7265 7175 656e  ints=num_frequen
-00011c90: 6379 5f70 6f69 6e74 732c 0a20 2020 2020  cy_points,.     
-00011ca0: 2020 2020 2020 2066 7265 7175 656e 6379         frequency
-00011cb0: 5f70 6f69 6e74 735f 6174 5f62 616e 6473  _points_at_bands
-00011cc0: 3d66 7265 7175 656e 6379 5f70 6f69 6e74  =frequency_point
-00011cd0: 735f 6174 5f62 616e 6473 2c0a 2020 2020  s_at_bands,.    
-00011ce0: 2020 2020 2020 2020 7772 6974 655f 6864          write_hd
-00011cf0: 6635 3d77 7269 7465 5f68 6466 352c 0a20  f5=write_hdf5,. 
-00011d00: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
-00011d10: 745f 6669 6c65 6e61 6d65 3d6f 7574 7075  t_filename=outpu
-00011d20: 745f 6669 6c65 6e61 6d65 2c0a 2020 2020  t_filename,.    
-00011d30: 2020 2020 2020 2020 6c6f 675f 6c65 7665          log_leve
-00011d40: 6c3d 7365 6c66 2e5f 6c6f 675f 6c65 7665  l=self._log_leve
-00011d50: 6c2c 0a20 2020 2020 2020 2029 0a0a 2020  l,.        )..  
-00011d60: 2020 2020 2020 6966 2077 7269 7465 5f74        if write_t
-00011d70: 7874 3a0a 2020 2020 2020 2020 2020 2020  xt:.            
-00011d80: 7772 6974 655f 7265 616c 5f73 656c 665f  write_real_self_
-00011d90: 656e 6572 6779 280a 2020 2020 2020 2020  energy(.        
-00011da0: 2020 2020 2020 2020 6465 6c74 6173 2c0a          deltas,.
-00011db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011dc0: 7365 6c66 2e6d 6573 685f 6e75 6d62 6572  self.mesh_number
-00011dd0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-00011de0: 2020 2067 7269 645f 706f 696e 7473 2c0a     grid_points,.
-00011df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e00: 7365 6c66 2e5f 6261 6e64 5f69 6e64 6963  self._band_indic
-00011e10: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-00011e20: 2020 2020 6672 6571 7565 6e63 795f 706f      frequency_po
-00011e30: 696e 7473 2c0a 2020 2020 2020 2020 2020  ints,.          
-00011e40: 2020 2020 2020 7465 6d70 6572 6174 7572        temperatur
-00011e50: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-00011e60: 2020 2020 5f65 7073 696c 6f6e 732c 0a20      _epsilons,. 
-00011e70: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00011e80: 7574 7075 745f 6669 6c65 6e61 6d65 3d6f  utput_filename=o
-00011e90: 7574 7075 745f 6669 6c65 6e61 6d65 2c0a  utput_filename,.
-00011ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011eb0: 6973 5f6d 6573 685f 7379 6d6d 6574 7279  is_mesh_symmetry
-00011ec0: 3d73 656c 662e 5f69 735f 6d65 7368 5f73  =self._is_mesh_s
-00011ed0: 796d 6d65 7472 792c 0a20 2020 2020 2020  ymmetry,.       
-00011ee0: 2020 2020 2020 2020 206c 6f67 5f6c 6576           log_lev
-00011ef0: 656c 3d73 656c 662e 5f6c 6f67 5f6c 6576  el=self._log_lev
-00011f00: 656c 2c0a 2020 2020 2020 2020 2020 2020  el,.            
-00011f10: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00011f20: 6e20 6672 6571 7565 6e63 795f 706f 696e  n frequency_poin
-00011f30: 7473 2c20 6465 6c74 6173 0a0a 2020 2020  ts, deltas..    
-00011f40: 6465 6620 7275 6e5f 7370 6563 7472 616c  def run_spectral
-00011f50: 5f66 756e 6374 696f 6e28 0a20 2020 2020  _function(.     
-00011f60: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00011f70: 2067 7269 645f 706f 696e 7473 2c0a 2020   grid_points,.  
-00011f80: 2020 2020 2020 7465 6d70 6572 6174 7572        temperatur
-00011f90: 6573 2c0a 2020 2020 2020 2020 6672 6571  es,.        freq
-00011fa0: 7565 6e63 795f 706f 696e 7473 3d4e 6f6e  uency_points=Non
-00011fb0: 652c 0a20 2020 2020 2020 2066 7265 7175  e,.        frequ
-00011fc0: 656e 6379 5f73 7465 703d 4e6f 6e65 2c0a  ency_step=None,.
-00011fd0: 2020 2020 2020 2020 6e75 6d5f 6672 6571          num_freq
-00011fe0: 7565 6e63 795f 706f 696e 7473 3d4e 6f6e  uency_points=Non
-00011ff0: 652c 0a20 2020 2020 2020 206e 756d 5f70  e,.        num_p
-00012000: 6f69 6e74 735f 696e 5f62 6174 6368 3d4e  oints_in_batch=N
-00012010: 6f6e 652c 0a20 2020 2020 2020 2077 7269  one,.        wri
-00012020: 7465 5f74 7874 3d46 616c 7365 2c0a 2020  te_txt=False,.  
-00012030: 2020 2020 2020 7772 6974 655f 6864 6635        write_hdf5
-00012040: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-00012050: 6f75 7470 7574 5f66 696c 656e 616d 653d  output_filename=
-00012060: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-00012070: 2020 2020 2022 2222 4672 6571 7565 6e63       """Frequenc
-00012080: 7920 7368 6966 7420 6672 6f6d 206c 6f77  y shift from low
-00012090: 6573 7420 6f72 6465 7220 6469 6167 7261  est order diagra
-000120a0: 6d20 6973 2063 616c 6375 6c61 7465 642e  m is calculated.
-000120b0: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-000120c0: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-000120d0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-000120e0: 6772 6964 5f70 6f69 6e74 7320 3a20 6172  grid_points : ar
-000120f0: 7261 795f 6c69 6b65 0a20 2020 2020 2020  ray_like.       
-00012100: 2020 2020 2047 7269 642d 706f 696e 7420       Grid-point 
-00012110: 696e 6469 6365 7320 7768 6572 6520 696d  indices where im
-00012120: 6167 2d73 656c 662d 656e 6572 6765 6973  ag-self-energeis
-00012130: 2061 7265 2063 6163 6c63 756c 6174 6564   are caclculated
-00012140: 2e0a 2020 2020 2020 2020 2020 2020 6474  ..            dt
-00012150: 7970 653d 696e 742c 2073 6861 7065 3d28  ype=int, shape=(
-00012160: 6772 6964 5f70 6f69 6e74 732c 290a 2020  grid_points,).  
-00012170: 2020 2020 2020 7465 6d70 6572 6174 7572        temperatur
-00012180: 6573 203a 2061 7272 6179 5f6c 696b 650a  es : array_like.
-00012190: 2020 2020 2020 2020 2020 2020 5465 6d70              Temp
-000121a0: 6572 6174 7572 6573 2077 6865 7265 2069  eratures where i
-000121b0: 6d61 672d 7365 6c66 2d65 6e65 7267 6965  mag-self-energie
-000121c0: 7320 6172 6520 6361 6c63 756c 6174 6564  s are calculated
-000121d0: 2e0a 2020 2020 2020 2020 2020 2020 6474  ..            dt
-000121e0: 7970 653d 666c 6f61 742c 2073 6861 7065  ype=float, shape
-000121f0: 3d28 7465 6d70 6572 6174 7572 6573 2c29  =(temperatures,)
-00012200: 0a20 2020 2020 2020 2066 7265 7175 656e  .        frequen
-00012210: 6379 5f70 6f69 6e74 7320 3a20 6172 7261  cy_points : arra
-00012220: 795f 6c69 6b65 2c20 6f70 7469 6f6e 616c  y_like, optional
-00012230: 0a20 2020 2020 2020 2020 2020 2046 7265  .            Fre
-00012240: 7175 656e 6379 2073 616d 706c 696e 6720  quency sampling 
-00012250: 706f 696e 7473 2e20 4465 6661 756c 7420  points. Default 
-00012260: 6973 204e 6f6e 652e 2049 6e20 7468 6973  is None. In this
-00012270: 2063 6173 652c 0a20 2020 2020 2020 2020   case,.         
-00012280: 2020 206e 756d 5f66 7265 7175 656e 6379     num_frequency
-00012290: 5f70 6f69 6e74 7320 6f72 2066 7265 7175  _points or frequ
-000122a0: 656e 6379 5f73 7465 7020 6973 2075 7365  ency_step is use
-000122b0: 6420 746f 2067 656e 6572 6174 6520 756e  d to generate un
-000122c0: 6966 6f72 6d0a 2020 2020 2020 2020 2020  iform.          
-000122d0: 2020 6672 6571 7565 6e63 7920 7361 6d70    frequency samp
-000122e0: 6c69 6e67 2070 6f69 6e74 732e 0a20 2020  ling points..   
-000122f0: 2020 2020 2020 2020 2064 7479 7065 3d66           dtype=f
-00012300: 6c6f 6174 2c20 7368 6170 653d 2866 7265  loat, shape=(fre
-00012310: 7175 656e 6379 5f70 6f69 6e74 732c 290a  quency_points,).
-00012320: 2020 2020 2020 2020 6672 6571 7565 6e63          frequenc
-00012330: 795f 7374 6570 203a 2066 6c6f 6174 2c20  y_step : float, 
-00012340: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-00012350: 2020 2020 2055 6e69 666f 726d 2070 6974       Uniform pit
-00012360: 6368 206f 6620 6672 6571 7565 6e63 7920  ch of frequency 
-00012370: 7361 6d70 6c69 6e67 2070 6f69 6e74 732e  sampling points.
-00012380: 2044 6566 6175 6c74 2069 7320 4e6f 6e65   Default is None
-00012390: 2e20 5468 6973 0a20 2020 2020 2020 2020  . This.         
-000123a0: 2020 2072 6573 756c 7473 2069 6e20 7573     results in us
-000123b0: 696e 6720 6e75 6d5f 6672 6571 7565 6e63  ing num_frequenc
-000123c0: 795f 706f 696e 7473 2e0a 2020 2020 2020  y_points..      
-000123d0: 2020 6e75 6d5f 6672 6571 7565 6e63 795f    num_frequency_
-000123e0: 706f 696e 7473 3a20 496e 742c 206f 7074  points: Int, opt
-000123f0: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
-00012400: 2020 4e75 6d62 6572 206f 6620 7361 6d70    Number of samp
-00012410: 6c69 6e67 2073 616d 706c 696e 6720 706f  ling sampling po
-00012420: 696e 7473 2074 6f20 6265 2075 7365 6420  ints to be used 
-00012430: 696e 7374 6561 6420 6f66 0a20 2020 2020  instead of.     
-00012440: 2020 2020 2020 2066 7265 7175 656e 6379         frequency
-00012450: 5f73 7465 702e 2054 6869 7320 6e75 6d62  _step. This numb
-00012460: 6572 2069 6e63 6c75 6465 7320 656e 6420  er includes end 
-00012470: 706f 696e 7473 2e20 4465 6661 756c 7420  points. Default 
-00012480: 6973 204e 6f6e 652c 0a20 2020 2020 2020  is None,.       
-00012490: 2020 2020 2077 6869 6368 2067 6976 6573       which gives
-000124a0: 2032 3031 2e0a 2020 2020 2020 2020 6e75   201..        nu
-000124b0: 6d5f 706f 696e 7473 5f69 6e5f 6261 7463  m_points_in_batc
-000124c0: 683a 2069 6e74 2c20 6f70 7469 6f6e 616c  h: int, optional
-000124d0: 0a20 2020 2020 2020 2020 2020 204e 756d  .            Num
-000124e0: 6265 7220 6f66 2073 616d 706c 696e 6720  ber of sampling 
-000124f0: 706f 696e 7473 2069 6e20 6f6e 6520 6261  points in one ba
-00012500: 7463 682e 2054 6869 7320 6973 2066 6f72  tch. This is for
-00012510: 2074 6865 2066 7265 7175 656e 6379 0a20   the frequency. 
-00012520: 2020 2020 2020 2020 2020 2073 616d 706c             sampl
-00012530: 696e 6720 6d6f 6465 2061 6e64 2074 6865  ing mode and the
-00012540: 2073 616d 706c 696e 6720 706f 696e 7473   sampling points
-00012550: 2061 7265 2064 6976 6964 6564 2069 6e74   are divided int
-00012560: 6f20 6261 7463 6865 732e 0a20 2020 2020  o batches..     
-00012570: 2020 2020 2020 204c 6167 6572 206e 756d         Lager num
-00012580: 6265 7220 7072 6f76 6964 6573 2065 6666  ber provides eff
-00012590: 6963 6965 6e74 2075 7365 206f 6620 6d75  icient use of mu
-000125a0: 6c74 692d 636f 7265 7320 6275 7420 6d6f  lti-cores but mo
-000125b0: 7265 0a20 2020 2020 2020 2020 2020 206d  re.            m
-000125c0: 656d 6f72 7920 6465 6d61 6e64 696e 672e  emory demanding.
-000125d0: 2044 6566 6175 6c74 2069 7320 4e6f 6e65   Default is None
-000125e0: 2c20 7768 6963 6820 6769 7665 2074 6865  , which give the
-000125f0: 206e 756d 6265 7220 6f66 2031 302e 0a20   number of 10.. 
-00012600: 2020 2020 2020 2077 7269 7465 5f74 7874         write_txt
-00012610: 203a 2062 6f6f 6c2c 206f 7074 696f 6e61   : bool, optiona
-00012620: 6c0a 2020 2020 2020 2020 2020 2020 4672  l.            Fr
-00012630: 6571 7565 6e63 7920 706f 696e 7473 2061  equency points a
-00012640: 6e64 2073 7065 6374 7261 6c20 6675 6e63  nd spectral func
-00012650: 7469 6f6e 7320 6172 6520 7772 6974 7465  tions are writte
-00012660: 6e0a 2020 2020 2020 2020 2020 2020 696e  n.            in
-00012670: 746f 2074 6578 7420 6669 6c65 732e 2044  to text files. D
-00012680: 6566 6175 6c74 2069 7320 4661 6c73 652e  efault is False.
-00012690: 0a20 2020 2020 2020 2077 7269 7465 5f68  .        write_h
-000126a0: 6466 3520 3a20 626f 6f6c 0a20 2020 2020  df5 : bool.     
-000126b0: 2020 2020 2020 2052 6573 756c 7473 2061         Results a
-000126c0: 7265 2073 746f 7265 6420 696e 2068 6466  re stored in hdf
-000126d0: 3520 6669 6c65 7320 696e 6465 7065 6e64  5 files independ
-000126e0: 656e 746c 7920 6174 2067 7269 6420 706f  ently at grid po
-000126f0: 696e 7473 2c0a 2020 2020 2020 2020 2020  ints,.          
-00012700: 2020 6570 7369 6c6f 6e73 2e20 4465 6661    epsilons. Defa
-00012710: 756c 7420 6973 2046 616c 7365 2e0a 2020  ult is False..  
-00012720: 2020 2020 2020 6f75 7470 7574 5f66 696c        output_fil
-00012730: 656e 616d 6520 3a20 7374 720a 2020 2020  ename : str.    
-00012740: 2020 2020 2020 2020 5468 6973 2073 7472          This str
-00012750: 696e 6720 6973 2069 6e73 6572 7465 6420  ing is inserted 
-00012760: 696e 2074 6865 206f 7574 7075 7420 6669  in the output fi
-00012770: 6c65 206e 616d 6573 2e0a 0a20 2020 2020  le names...     
-00012780: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-00012790: 6620 7365 6c66 2e5f 696e 7465 7261 6374  f self._interact
-000127a0: 696f 6e20 6973 204e 6f6e 653a 0a20 2020  ion is None:.   
-000127b0: 2020 2020 2020 2020 206d 7367 203d 2028           msg = (
-000127c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000127d0: 2022 5068 6f6e 6f33 7079 2e69 6e69 745f   "Phono3py.init_
-000127e0: 7068 7068 5f69 6e74 6572 6163 7469 6f6e  phph_interaction
-000127f0: 2068 6173 2074 6f20 6265 2063 616c 6c65   has to be calle
-00012800: 6420 220a 2020 2020 2020 2020 2020 2020  d ".            
-00012810: 2020 2020 2262 6566 6f72 6520 7275 6e6e      "before runn
-00012820: 696e 6720 7468 6973 206d 6574 686f 642e  ing this method.
-00012830: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
-00012840: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00012850: 6520 5275 6e74 696d 6545 7272 6f72 286d  e RuntimeError(m
-00012860: 7367 290a 0a20 2020 2020 2020 2073 656c  sg)..        sel
-00012870: 662e 5f73 7065 6374 7261 6c5f 6675 6e63  f._spectral_func
-00012880: 7469 6f6e 203d 2072 756e 5f73 7065 6374  tion = run_spect
-00012890: 7261 6c5f 6675 6e63 7469 6f6e 280a 2020  ral_function(.  
-000128a0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000128b0: 696e 7465 7261 6374 696f 6e2c 0a20 2020  interaction,.   
-000128c0: 2020 2020 2020 2020 2067 7269 645f 706f           grid_po
-000128d0: 696e 7473 2c0a 2020 2020 2020 2020 2020  ints,.          
-000128e0: 2020 7465 6d70 6572 6174 7572 6573 3d74    temperatures=t
-000128f0: 656d 7065 7261 7475 7265 732c 0a20 2020  emperatures,.   
-00012900: 2020 2020 2020 2020 2073 6967 6d61 733d           sigmas=
-00012910: 7365 6c66 2e5f 7369 676d 6173 2c0a 2020  self._sigmas,.  
-00012920: 2020 2020 2020 2020 2020 6672 6571 7565            freque
-00012930: 6e63 795f 706f 696e 7473 3d66 7265 7175  ncy_points=frequ
-00012940: 656e 6379 5f70 6f69 6e74 732c 0a20 2020  ency_points,.   
-00012950: 2020 2020 2020 2020 2066 7265 7175 656e           frequen
-00012960: 6379 5f73 7465 703d 6672 6571 7565 6e63  cy_step=frequenc
-00012970: 795f 7374 6570 2c0a 2020 2020 2020 2020  y_step,.        
-00012980: 2020 2020 6e75 6d5f 6672 6571 7565 6e63      num_frequenc
-00012990: 795f 706f 696e 7473 3d6e 756d 5f66 7265  y_points=num_fre
-000129a0: 7175 656e 6379 5f70 6f69 6e74 732c 0a20  quency_points,. 
-000129b0: 2020 2020 2020 2020 2020 206e 756d 5f70             num_p
-000129c0: 6f69 6e74 735f 696e 5f62 6174 6368 3d6e  oints_in_batch=n
-000129d0: 756d 5f70 6f69 6e74 735f 696e 5f62 6174  um_points_in_bat
-000129e0: 6368 2c0a 2020 2020 2020 2020 2020 2020  ch,.            
-000129f0: 6261 6e64 5f69 6e64 6963 6573 3d73 656c  band_indices=sel
-00012a00: 662e 5f62 616e 645f 696e 6469 6365 732c  f._band_indices,
-00012a10: 0a20 2020 2020 2020 2020 2020 2077 7269  .            wri
-00012a20: 7465 5f74 7874 3d77 7269 7465 5f74 7874  te_txt=write_txt
-00012a30: 2c0a 2020 2020 2020 2020 2020 2020 7772  ,.            wr
-00012a40: 6974 655f 6864 6635 3d77 7269 7465 5f68  ite_hdf5=write_h
-00012a50: 6466 352c 0a20 2020 2020 2020 2020 2020  df5,.           
-00012a60: 206f 7574 7075 745f 6669 6c65 6e61 6d65   output_filename
-00012a70: 3d6f 7574 7075 745f 6669 6c65 6e61 6d65  =output_filename
-00012a80: 2c0a 2020 2020 2020 2020 2020 2020 6c6f  ,.            lo
-00012a90: 675f 6c65 7665 6c3d 7365 6c66 2e5f 6c6f  g_level=self._lo
-00012aa0: 675f 6c65 7665 6c2c 0a20 2020 2020 2020  g_level,.       
-00012ab0: 2029 0a0a 2020 2020 6465 6620 7275 6e5f   )..    def run_
-00012ac0: 7468 6572 6d61 6c5f 636f 6e64 7563 7469  thermal_conducti
-00012ad0: 7669 7479 280a 2020 2020 2020 2020 7365  vity(.        se
-00012ae0: 6c66 2c0a 2020 2020 2020 2020 6973 5f4c  lf,.        is_L
-00012af0: 4254 453d 4661 6c73 652c 0a20 2020 2020  BTE=False,.     
-00012b00: 2020 2074 656d 7065 7261 7475 7265 733d     temperatures=
-00012b10: 4e6f 6e65 2c0a 2020 2020 2020 2020 6973  None,.        is
-00012b20: 5f69 736f 746f 7065 3d46 616c 7365 2c0a  _isotope=False,.
-00012b30: 2020 2020 2020 2020 6d61 7373 5f76 6172          mass_var
-00012b40: 6961 6e63 6573 3d4e 6f6e 652c 0a20 2020  iances=None,.   
-00012b50: 2020 2020 2067 7269 645f 706f 696e 7473       grid_points
-00012b60: 3d4e 6f6e 652c 0a20 2020 2020 2020 2062  =None,.        b
-00012b70: 6f75 6e64 6172 795f 6d66 703d 4e6f 6e65  oundary_mfp=None
-00012b80: 2c20 2023 2069 6e20 6d69 6372 6f6d 6574  ,  # in micromet
-00012b90: 7265 0a20 2020 2020 2020 2073 6f6c 7665  re.        solve
-00012ba0: 5f63 6f6c 6c65 6374 6976 655f 7068 6f6e  _collective_phon
-00012bb0: 6f6e 3d46 616c 7365 2c0a 2020 2020 2020  on=False,.      
-00012bc0: 2020 7573 655f 6176 655f 7070 3d46 616c    use_ave_pp=Fal
-00012bd0: 7365 2c0a 2020 2020 2020 2020 6973 5f72  se,.        is_r
-00012be0: 6564 7563 6962 6c65 5f63 6f6c 6c69 7369  educible_collisi
-00012bf0: 6f6e 5f6d 6174 7269 783d 4661 6c73 652c  on_matrix=False,
-00012c00: 0a20 2020 2020 2020 2069 735f 6b61 7070  .        is_kapp
-00012c10: 615f 7374 6172 3d54 7275 652c 0a20 2020  a_star=True,.   
-00012c20: 2020 2020 2067 765f 6465 6c74 615f 713d       gv_delta_q=
-00012c30: 4e6f 6e65 2c20 2023 2066 6f72 2067 726f  None,  # for gro
-00012c40: 7570 2076 656c 6f63 6974 790a 2020 2020  up velocity.    
-00012c50: 2020 2020 6973 5f66 756c 6c5f 7070 3d46      is_full_pp=F
-00012c60: 616c 7365 2c0a 2020 2020 2020 2020 7069  alse,.        pi
-00012c70: 6e76 5f63 7574 6f66 663d 312e 3065 2d38  nv_cutoff=1.0e-8
-00012c80: 2c20 2023 2066 6f72 2070 7365 7564 6f2d  ,  # for pseudo-
-00012c90: 696e 7665 7273 696f 6e20 6f66 2063 6f6c  inversion of col
-00012ca0: 6c69 7369 6f6e 206d 6174 7269 780a 2020  lision matrix.  
-00012cb0: 2020 2020 2020 7069 6e76 5f6d 6574 686f        pinv_metho
-00012cc0: 643d 302c 2020 2320 666f 7220 7073 6575  d=0,  # for pseu
-00012cd0: 646f 2d69 6e76 6572 7369 6f6e 206f 6620  do-inversion of 
-00012ce0: 636f 6c6c 6973 696f 6e20 6d61 7472 6978  collision matrix
-00012cf0: 0a20 2020 2020 2020 2070 696e 765f 736f  .        pinv_so
-00012d00: 6c76 6572 3d30 2c20 2023 2073 6f6c 7665  lver=0,  # solve
-00012d10: 7220 6f66 2070 7365 7564 6f2d 696e 7665  r of pseudo-inve
-00012d20: 7273 696f 6e20 6f66 2063 6f6c 6c69 7369  rsion of collisi
-00012d30: 6f6e 206d 6174 7269 780a 2020 2020 2020  on matrix.      
-00012d40: 2020 7772 6974 655f 6761 6d6d 613d 4661    write_gamma=Fa
-00012d50: 6c73 652c 0a20 2020 2020 2020 2072 6561  lse,.        rea
-00012d60: 645f 6761 6d6d 613d 4661 6c73 652c 0a20  d_gamma=False,. 
-00012d70: 2020 2020 2020 2069 735f 4e5f 553d 4661         is_N_U=Fa
-00012d80: 6c73 652c 0a20 2020 2020 2020 2063 6f6e  lse,.        con
-00012d90: 6475 6374 6976 6974 795f 7479 7065 3d4e  ductivity_type=N
-00012da0: 6f6e 652c 0a20 2020 2020 2020 2077 7269  one,.        wri
-00012db0: 7465 5f6b 6170 7061 3d46 616c 7365 2c0a  te_kappa=False,.
-00012dc0: 2020 2020 2020 2020 7772 6974 655f 6761          write_ga
-00012dd0: 6d6d 615f 6465 7461 696c 3d46 616c 7365  mma_detail=False
-00012de0: 2c0a 2020 2020 2020 2020 7772 6974 655f  ,.        write_
-00012df0: 636f 6c6c 6973 696f 6e3d 4661 6c73 652c  collision=False,
-00012e00: 0a20 2020 2020 2020 2072 6561 645f 636f  .        read_co
-00012e10: 6c6c 6973 696f 6e3d 4661 6c73 652c 0a20  llision=False,. 
-00012e20: 2020 2020 2020 2077 7269 7465 5f70 703d         write_pp=
-00012e30: 4661 6c73 652c 0a20 2020 2020 2020 2072  False,.        r
-00012e40: 6561 645f 7070 3d46 616c 7365 2c0a 2020  ead_pp=False,.  
-00012e50: 2020 2020 2020 7772 6974 655f 4c42 5445        write_LBTE
-00012e60: 5f73 6f6c 7574 696f 6e3d 4661 6c73 652c  _solution=False,
-00012e70: 0a20 2020 2020 2020 2063 6f6d 7072 6573  .        compres
-00012e80: 7369 6f6e 3d22 677a 6970 222c 0a20 2020  sion="gzip",.   
-00012e90: 2020 2020 2069 6e70 7574 5f66 696c 656e       input_filen
-00012ea0: 616d 653d 4e6f 6e65 2c0a 2020 2020 2020  ame=None,.      
-00012eb0: 2020 6f75 7470 7574 5f66 696c 656e 616d    output_filenam
-00012ec0: 653d 4e6f 6e65 2c0a 2020 2020 293a 0a20  e=None,.    ):. 
-00012ed0: 2020 2020 2020 2022 2222 5275 6e20 7468         """Run th
-00012ee0: 6572 6d61 6c20 636f 6e64 7563 7469 7669  ermal conductivi
-00012ef0: 7479 2063 616c 6375 6c61 7469 6f6e 2e0a  ty calculation..
-00012f00: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00012f10: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-00012f20: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2069  ------.        i
-00012f30: 735f 4c42 5445 203a 2062 6f6f 6c2c 206f  s_LBTE : bool, o
-00012f40: 7074 696f 6e61 6c2c 2064 6566 6175 6c74  ptional, default
-00012f50: 2069 7320 4661 6c73 650a 2020 2020 2020   is False.      
-00012f60: 2020 2020 2020 5254 4120 2846 616c 7365        RTA (False
-00012f70: 2920 6f72 2064 6972 6563 7420 736f 6c75  ) or direct solu
-00012f80: 7469 6f6e 2028 5472 7565 292e 0a20 2020  tion (True)..   
-00012f90: 2020 2020 2074 656d 7065 7261 7475 7265       temperature
-00012fa0: 7320 3a20 6172 7261 795f 6c69 6b65 2c20  s : array_like, 
-00012fb0: 6f70 7469 6f6e 616c 2c20 6465 6661 756c  optional, defaul
-00012fc0: 7420 6973 204e 6f6e 650a 2020 2020 2020  t is None.      
-00012fd0: 2020 2020 2020 5465 6d70 6572 6174 7572        Temperatur
-00012fe0: 6573 2061 7420 7768 6963 6820 7468 6572  es at which ther
-00012ff0: 6d61 6c20 636f 6e64 7563 7469 7669 7479  mal conductivity
-00013000: 2069 7320 6361 6c63 756c 6174 6564 2e0a   is calculated..
-00013010: 2020 2020 2020 2020 2020 2020 7368 6170              shap
-00013020: 653d 2874 656d 7065 7261 7475 7265 5f70  e=(temperature_p
-00013030: 6f69 6e74 732c 2029 2c20 6474 7970 653d  oints, ), dtype=
-00013040: 2764 6f75 626c 6527 2e0a 2020 2020 2020  'double'..      
-00013050: 2020 2020 2020 5769 7468 204e 6f6e 652c        With None,
-00013060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013070: 2060 6973 5f4c 4254 453d 4661 6c73 6560   `is_LBTE=False`
-00013080: 2067 6976 6573 2074 656d 7065 7261 7475   gives temperatu
-00013090: 7265 733d 5b30 2c20 3130 2c20 2e2e 2e2c  res=[0, 10, ...,
-000130a0: 2031 3030 305d 2e0a 2020 2020 2020 2020   1000]..        
-000130b0: 2020 2020 2020 2020 6069 735f 4c42 5445          `is_LBTE
-000130c0: 3d54 7275 6560 2067 6976 6573 2074 656d  =True` gives tem
-000130d0: 7065 7261 7475 7265 733d 5b33 3030 2c20  peratures=[300, 
-000130e0: 5d2e 0a20 2020 2020 2020 2069 735f 6973  ]..        is_is
-000130f0: 6f74 6f70 6520 3a20 626f 6f6c 2c20 6f70  otope : bool, op
-00013100: 7469 6f6e 616c 2c20 6465 6661 756c 7420  tional, default 
-00013110: 6973 2046 616c 7365 0a20 2020 2020 2020  is False.       
-00013120: 2020 2020 2057 6974 6820 6f72 2077 6974       With or wit
-00013130: 686f 7574 2069 736f 746f 7065 2073 6361  hout isotope sca
-00013140: 7474 6572 696e 672e 0a20 2020 2020 2020  ttering..       
-00013150: 206d 6173 735f 7661 7269 616e 6365 7320   mass_variances 
-00013160: 3a20 6172 7261 795f 6c69 6b65 2c20 6f70  : array_like, op
-00013170: 7469 6f6e 616c 2c20 6465 6661 756c 7420  tional, default 
-00013180: 6973 204e 6f6e 650a 2020 2020 2020 2020  is None.        
-00013190: 2020 2020 4d61 7373 2076 6172 6961 6e63      Mass varianc
-000131a0: 6573 2066 6f72 2069 736f 746f 7065 2073  es for isotope s
-000131b0: 6361 7474 6572 696e 6720 6361 6c63 756c  cattering calcul
-000131c0: 6174 696f 6e2e 2057 6865 6e20 4e6f 6e65  ation. When None
-000131d0: 2c0a 2020 2020 2020 2020 2020 2020 7468  ,.            th
-000131e0: 6520 7661 6c75 6573 2073 746f 7265 6420  e values stored 
-000131f0: 696e 2070 686f 6e6f 3370 7920 6172 6520  in phono3py are 
-00013200: 7573 6564 2077 6974 6820 6069 735f 6973  used with `is_is
-00013210: 6f74 6f70 653d 5472 7565 602e 0a20 2020  otope=True`..   
-00013220: 2020 2020 2020 2020 2073 6861 7065 2861           shape(a
-00013230: 746f 6d73 5f69 6e5f 7072 696d 6974 6976  toms_in_primitiv
-00013240: 652c 2029 2c20 6474 7970 653d 2764 6f75  e, ), dtype='dou
-00013250: 626c 6527 2e0a 2020 2020 2020 2020 6772  ble'..        gr
-00013260: 6964 5f70 6f69 6e74 7320 3a20 6172 7261  id_points : arra
-00013270: 795f 6c69 6b65 2c20 6f70 7469 6f6e 616c  y_like, optional
-00013280: 2c20 6465 6661 756c 7420 6973 204e 6f6e  , default is Non
-00013290: 650a 2020 2020 2020 2020 2020 2020 4c69  e.            Li
-000132a0: 7374 206f 6620 6772 6964 2070 6f69 6e74  st of grid point
-000132b0: 2069 6e64 6963 6573 2077 6865 7265 206d   indices where m
-000132c0: 6f64 6520 7468 6572 6d61 6c20 636f 6e64  ode thermal cond
-000132d0: 7563 7469 7669 7469 6573 2061 7265 0a20  uctivities are. 
-000132e0: 2020 2020 2020 2020 2020 2063 616c 6375             calcu
-000132f0: 6c61 7465 642e 2057 6974 6820 4e6f 6e65  lated. With None
-00013300: 2c20 616c 6c20 7468 6520 6772 6964 2070  , all the grid p
-00013310: 6f69 6e74 7320 7468 6174 2061 7265 206e  oints that are n
-00013320: 6563 6573 7361 7279 0a20 2020 2020 2020  ecessary.       
-00013330: 2020 2020 2066 6f72 2074 6865 726d 616c       for thermal
-00013340: 2063 6f6e 6475 6374 6976 6974 7920 6172   conductivity ar
-00013350: 6520 7365 7420 696e 7465 726e 616c 6c79  e set internally
-00013360: 2e0a 2020 2020 2020 2020 2020 2020 7368  ..            sh
-00013370: 6170 6528 6e75 6d5f 6772 6964 5f70 6f69  ape(num_grid_poi
-00013380: 6e74 732c 2029 2c20 6474 7970 653d 2769  nts, ), dtype='i
-00013390: 6e74 5f27 2e0a 2020 2020 2020 2020 626f  nt_'..        bo
-000133a0: 756e 6461 7279 5f6d 6670 203a 2066 6c6f  undary_mfp : flo
-000133b0: 6174 2c20 6f70 7469 6f6e 612c 2064 6566  at, optiona, def
-000133c0: 6175 6c74 2069 7320 4e6f 6e65 0a20 2020  ault is None.   
-000133d0: 2020 2020 2020 2020 204d 6561 6e20 6672           Mean fr
-000133e0: 6565 2070 6174 6820 696e 206d 6963 726f  ee path in micro
-000133f0: 6d65 7472 6520 746f 2063 616c 6375 6c61  metre to calcula
-00013400: 7465 2073 696d 706c 6520 626f 756e 6461  te simple bounda
-00013410: 7279 0a20 2020 2020 2020 2020 2020 2073  ry.            s
-00013420: 6361 7474 6572 696e 6720 636f 6e74 7269  cattering contri
-00013430: 6275 7469 6f6e 2074 6f20 7468 6572 6d61  bution to therma
-00013440: 6c20 636f 6e64 7563 7469 7669 7479 2e0a  l conductivity..
-00013450: 2020 2020 2020 2020 2020 2020 4e6f 6e65              None
-00013460: 2069 676e 6f72 6573 2074 6869 7320 636f   ignores this co
-00013470: 6e74 7269 6275 7469 6f6e 2e0a 2020 2020  ntribution..    
-00013480: 2020 2020 736f 6c76 655f 636f 6c6c 6563      solve_collec
-00013490: 7469 7665 5f70 686f 6e6f 6e20 3a20 626f  tive_phonon : bo
-000134a0: 6f6c 2c20 6f70 7469 6f6e 616c 2c20 6465  ol, optional, de
-000134b0: 6661 756c 7420 6973 2046 616c 7365 0a20  fault is False. 
-000134c0: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-000134d0: 6973 2061 6e20 6f70 7469 6f6e 2066 6f72  is an option for
-000134e0: 2074 6865 2066 6561 7475 7265 2075 6e64   the feature und
-000134f0: 6572 2064 6576 656c 6f70 6d65 6e74 2e0a  er development..
-00013500: 2020 2020 2020 2020 7573 655f 6176 655f          use_ave_
-00013510: 7070 203a 2062 6f6f 6c2c 206f 7074 696f  pp : bool, optio
-00013520: 6e61 6c2c 2064 6566 6175 6c74 2069 7320  nal, default is 
-00013530: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
-00013540: 2020 5254 4120 6f6e 6c79 2028 6069 735f    RTA only (`is_
-00013550: 4c42 5445 3d46 616c 7365 6029 2e20 4176  LBTE=False`). Av
-00013560: 6572 6167 6564 2070 686f 6e6f 6e2d 7068  eraged phonon-ph
-00013570: 6f6e 6f6e 2069 6e74 6572 6163 7469 6f6e  onon interaction
-00013580: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
-00013590: 656e 6774 6820 6973 2075 7365 6420 746f  ength is used to
-000135a0: 2063 616c 6375 6c61 7465 2070 686f 6e6f   calculate phono
-000135b0: 6e20 6c69 6665 7469 6d65 2e20 5468 6973  n lifetime. This
-000135c0: 2064 6f65 7320 6e6f 740a 2020 2020 2020   does not.      
-000135d0: 2020 2020 2020 7265 6475 6365 2063 6f6d        reduce com
-000135e0: 7075 7461 7469 6f6e 616c 2064 656d 616e  putational deman
-000135f0: 642c 2062 7574 206d 6179 2062 6520 7573  d, but may be us
-00013600: 6564 2074 6f20 6d6f 6465 6c20 7468 6572  ed to model ther
-00013610: 6d61 6c0a 2020 2020 2020 2020 2020 2020  mal.            
-00013620: 636f 6e64 7563 7469 7669 7479 2066 6f72  conductivity for
-00013630: 2061 6e61 6c79 7a65 2074 6865 2063 616c   analyze the cal
-00013640: 6375 6c61 7469 6f6e 2072 6573 756c 7473  culation results
-00013650: 2e0a 2020 2020 2020 2020 6973 5f72 6564  ..        is_red
-00013660: 7563 6962 6c65 5f63 6f6c 6c69 7369 6f6e  ucible_collision
-00013670: 5f6d 6174 7269 7820 3a20 626f 6f6c 2c20  _matrix : bool, 
-00013680: 6f70 7469 6f6e 616c 2c20 6465 6661 756c  optional, defaul
-00013690: 7420 6973 2046 616c 7365 0a20 2020 2020  t is False.     
-000136a0: 2020 2020 2020 2044 6972 6563 7420 736f         Direct so
-000136b0: 6c75 7469 6f6e 206f 6e6c 7920 2860 6973  lution only (`is
-000136c0: 5f4c 4254 453d 5472 7565 6029 2e20 5468  _LBTE=True`). Th
-000136d0: 6973 2069 7320 616e 2065 7870 6572 696d  is is an experim
-000136e0: 656e 7461 6c0a 2020 2020 2020 2020 2020  ental.          
-000136f0: 2020 6f70 7469 6f6e 2e20 5769 7468 2054    option. With T
-00013700: 7275 652c 2066 756c 6c20 636f 6c6c 6973  rue, full collis
-00013710: 696f 6e20 6d61 7472 6978 2069 7320 6372  ion matrix is cr
-00013720: 6561 7465 6420 616e 6420 736f 6c76 6564  eated and solved
-00013730: 2e0a 2020 2020 2020 2020 6973 5f6b 6170  ..        is_kap
-00013740: 7061 5f73 7461 7220 3a20 626f 6f6c 2c20  pa_star : bool, 
-00013750: 6f70 7469 6f6e 616c 2c20 6465 6661 756c  optional, defaul
-00013760: 7420 6973 2054 7275 650a 2020 2020 2020  t is True.      
-00013770: 2020 2020 2020 5769 7468 2074 7275 652c        With true,
-00013780: 2073 796d 6d65 7472 7920 6973 2063 6f6e   symmetry is con
-00013790: 7369 6465 7265 6420 7768 656e 2073 616d  sidered when sam
-000137a0: 706c 696e 6720 6772 6964 2070 6f69 6e74  pling grid point
-000137b0: 730a 2020 2020 2020 2020 2020 2020 6174  s.            at
-000137c0: 2077 6869 6368 206d 6f64 6520 7468 6572   which mode ther
-000137d0: 6d61 6c20 636f 6e64 7563 7469 7669 7469  mal conductiviti
-000137e0: 6573 2061 7265 2063 616c 6375 6c61 7465  es are calculate
-000137f0: 642e 0a20 2020 2020 2020 2067 765f 6465  d..        gv_de
-00013800: 6c74 615f 7120 3a20 666c 6f61 742c 206f  lta_q : float, o
-00013810: 7074 696f 6e61 6c2c 2064 6566 6175 6c74  ptional, default
-00013820: 2069 7320 4e6f 6e65 2c20 2023 2066 6f72   is None,  # for
-00013830: 2067 726f 7570 2076 656c 6f63 6974 790a   group velocity.
-00013840: 2020 2020 2020 2020 2020 2020 5769 7468              With
-00013850: 206e 6f6e 2d61 6e61 6c79 7469 6361 6c20   non-analytical 
-00013860: 636f 7272 6563 7469 6f6e 2c20 6772 6f75  correction, grou
-00013870: 7020 7665 6c6f 6369 7479 2069 7320 6361  p velocity is ca
-00013880: 6c63 756c 6174 6564 0a20 2020 2020 2020  lculated.       
-00013890: 2020 2020 2062 7920 6365 6e74 7261 6c20       by central 
-000138a0: 6669 6e69 7465 2064 6966 6665 7265 6e63  finite differenc
-000138b0: 6520 6d65 7468 6f64 2e20 5468 6973 2076  e method. This v
-000138c0: 616c 7565 2067 6976 6573 2074 6865 2064  alue gives the d
-000138d0: 6973 7461 6e63 650a 2020 2020 2020 2020  istance.        
-000138e0: 2020 2020 696e 2062 6f74 6820 6469 7265      in both dire
-000138f0: 6374 696f 6e73 2069 6e20 312f 416e 6773  ctions in 1/Angs
-00013900: 7472 6f6d 2e20 5468 6520 6465 6661 756c  trom. The defaul
-00013910: 7420 7661 6c75 6520 7769 6c6c 2062 6520  t value will be 
-00013920: 3165 2d35 2e0a 2020 2020 2020 2020 6973  1e-5..        is
-00013930: 5f66 756c 6c5f 7070 203a 2062 6f6f 6c2c  _full_pp : bool,
-00013940: 206f 7074 696f 6e61 6c2c 2064 6566 6175   optional, defau
-00013950: 6c74 2069 7320 4661 6c73 650a 2020 2020  lt is False.    
-00013960: 2020 2020 2020 2020 5769 7468 2054 7275          With Tru
-00013970: 652c 2066 756c 6c20 656c 656d 656e 7473  e, full elements
-00013980: 206f 6620 7068 6f6e 6f6e 2d70 686f 6e6f   of phonon-phono
-00013990: 6e20 696e 7465 7261 6374 696f 6e20 7374  n interaction st
-000139a0: 7265 6e67 7468 0a20 2020 2020 2020 2020  rength.         
-000139b0: 2020 2061 7265 2063 6f6d 7075 7465 642e     are computed.
-000139c0: 2048 6f77 6576 6572 2077 6974 6820 7465   However with te
-000139d0: 7472 6168 6564 726f 6e20 6d65 7468 6f64  trahedron method
-000139e0: 2c20 7061 7274 206f 6620 7468 656d 2061  , part of them a
-000139f0: 7265 0a20 2020 2020 2020 2020 2020 206b  re.            k
-00013a00: 6e6f 776e 2074 6f20 6265 207a 6572 6f20  nown to be zero 
-00013a10: 616e 6420 756e 6e65 6365 7373 6172 7920  and unnecessary 
-00013a20: 746f 2063 616c 6375 6c61 7469 6f6e 2e20  to calculation. 
-00013a30: 5769 7468 2046 616c 7365 2c0a 2020 2020  With False,.    
-00013a40: 2020 2020 2020 2020 7468 6f73 6520 656c          those el
-00013a50: 656d 656e 7473 2061 7265 206e 6f74 2063  ements are not c
-00013a60: 616c 6375 6c61 7465 642c 2062 7920 7768  alculated, by wh
-00013a70: 6963 6820 636f 6e73 6964 6572 6162 6c65  ich considerable
-00013a80: 0a20 2020 2020 2020 2020 2020 2069 6d70  .            imp
-00013a90: 726f 7665 206f 6620 6566 6669 6369 656e  rove of efficien
-00013aa0: 6379 2069 7320 6578 7065 6374 6564 2e0a  cy is expected..
-00013ab0: 2020 2020 2020 2020 2020 2020 5769 7468              With
-00013ac0: 2073 6d65 6172 696e 6720 6d65 7468 6f64   smearing method
-00013ad0: 2c20 6576 656e 2069 6620 7468 6973 2069  , even if this i
-00013ae0: 7320 7365 7420 4661 6c73 652c 2066 756c  s set False, ful
-00013af0: 6c20 656c 656d 656e 7473 0a20 2020 2020  l elements.     
-00013b00: 2020 2020 2020 2061 7265 2063 6f6d 7075         are compu
-00013b10: 7465 6420 756e 6c65 7373 2060 7369 676d  ted unless `sigm
-00013b20: 615f 6375 746f 6666 6020 6973 2073 7065  a_cutoff` is spe
-00013b30: 6369 6669 6564 2e0a 2020 2020 2020 2020  cified..        
-00013b40: 7069 6e76 5f63 7574 6f66 6620 3a20 666c  pinv_cutoff : fl
-00013b50: 6f61 742c 206f 7074 696f 6e61 6c2c 2064  oat, optional, d
-00013b60: 6566 6175 6c74 2069 7320 312e 3065 2d38  efault is 1.0e-8
-00013b70: 0a20 2020 2020 2020 2020 2020 2044 6972  .            Dir
-00013b80: 6563 7420 736f 6c75 7469 6f6e 206f 6e6c  ect solution onl
-00013b90: 7920 2860 6973 5f4c 4254 453d 5472 7565  y (`is_LBTE=True
-00013ba0: 6029 2e20 5468 6973 2069 7320 7573 6564  `). This is used
-00013bb0: 2061 7320 6120 6372 6974 6572 696f 6e0a   as a criterion.
-00013bc0: 2020 2020 2020 2020 2020 2020 746f 206a              to j
-00013bd0: 7564 6765 2074 6865 2065 6967 656e 7661  udge the eigenva
-00013be0: 6c75 6573 2061 7265 2063 6f6e 7369 6465  lues are conside
-00013bf0: 7265 6420 6173 207a 6572 6f20 6f72 206e  red as zero or n
-00013c00: 6f74 2069 6e0a 2020 2020 2020 2020 2020  ot in.          
-00013c10: 2020 7073 6575 646f 2d69 6e76 6572 7369    pseudo-inversi
-00013c20: 6f6e 206f 6620 636f 6c6c 6973 696f 6e20  on of collision 
-00013c30: 6d61 7472 6978 2e20 5365 6520 616c 736f  matrix. See also
-00013c40: 2060 7069 6e76 5f6d 6574 686f 6460 2e0a   `pinv_method`..
-00013c50: 2020 2020 2020 2020 7069 6e76 5f6d 6574          pinv_met
-00013c60: 686f 6420 3a20 696e 742c 206f 7074 696f  hod : int, optio
-00013c70: 6e61 6c2c 2064 6566 6175 6c74 2069 7320  nal, default is 
-00013c80: 302e 0a20 2020 2020 2020 2020 2020 2044  0..            D
-00013c90: 6972 6563 7420 736f 6c75 7469 6f6e 206f  irect solution o
-00013ca0: 6e6c 7920 2860 6973 5f4c 4254 453d 5472  nly (`is_LBTE=Tr
-00013cb0: 7565 6029 2e0a 2020 2020 2020 2020 2020  ue`)..          
-00013cc0: 2020 2020 2020 302e 2061 6273 2865 6967        0. abs(eig
-00013cd0: 656e 7661 6c75 6529 203c 2060 7069 6e76  envalue) < `pinv
-00013ce0: 5f63 7574 6f66 6660 0a20 2020 2020 2020  _cutoff`.       
-00013cf0: 2020 2020 2020 2020 2031 2e20 6569 6765           1. eige
-00013d00: 6e76 616c 7565 203c 2060 7069 6e76 5f63  nvalue < `pinv_c
-00013d10: 7574 6f66 6660 0a20 2020 2020 2020 2070  utoff`.        p
-00013d20: 696e 765f 736f 6c76 6572 203a 2069 6e74  inv_solver : int
-00013d30: 2c20 6f70 7469 6f6e 616c 2c20 6465 6661  , optional, defa
-00013d40: 756c 7420 6973 2030 0a20 2020 2020 2020  ult is 0.       
-00013d50: 2020 2020 2044 6972 6563 7420 736f 6c75       Direct solu
-00013d60: 7469 6f6e 206f 6e6c 7920 2860 6973 5f4c  tion only (`is_L
-00013d70: 4254 453d 5472 7565 6029 2e20 4368 6f69  BTE=True`). Choi
-00013d80: 6365 206f 6620 736f 6c76 6572 206f 660a  ce of solver of.
-00013d90: 2020 2020 2020 2020 2020 2020 7073 6575              pseu
-00013da0: 646f 2d69 6e76 6572 7369 6f6e 206f 6620  do-inversion of 
-00013db0: 636f 6c6c 6973 696f 6e20 6d61 7472 6978  collision matrix
-00013dc0: 2e20 3020 6d65 616e 7320 7468 6520 6465  . 0 means the de
-00013dd0: 6661 756c 7420 6368 6f69 6365 2e0a 2020  fault choice..  
-00013de0: 2020 2020 2020 2020 2020 2020 2020 312e                1.
-00013df0: 204c 6170 6163 6b65 2064 7379 6576 3a20   Lapacke dsyev: 
-00013e00: 536d 616c 6c65 7220 6d65 6d6f 7279 2063  Smaller memory c
-00013e10: 6f6e 7375 6d70 7469 6f6e 2074 6861 6e20  onsumption than 
-00013e20: 6473 7965 7664 2c20 6275 740a 2020 2020  dsyevd, but.    
-00013e30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00013e40: 6c6f 7765 722e 2054 6869 7320 6973 2074  lower. This is t
-00013e50: 6865 2064 6566 6175 6c74 2073 6f6c 7665  he default solve
-00013e60: 7220 7768 656e 204d 4b4c 204c 4150 4143  r when MKL LAPAC
-00013e70: 4b45 2069 730a 2020 2020 2020 2020 2020  KE is.          
-00013e80: 2020 2020 2020 2020 2069 6e74 6567 7261           integra
-00013e90: 7465 6420 6f72 2073 6369 7079 2069 7320  ted or scipy is 
-00013ea0: 6e6f 7420 696e 7374 616c 6c65 642e 0a20  not installed.. 
-00013eb0: 2020 2020 2020 2020 2020 2020 2020 2032                 2
-00013ec0: 2e20 4c61 7061 636b 6520 6473 7965 7664  . Lapacke dsyevd
-00013ed0: 3a20 4c61 7267 6572 206d 656d 6f72 7920  : Larger memory 
-00013ee0: 636f 6e73 756d 7074 696f 6e20 7468 616e  consumption than
-00013ef0: 2064 7379 6576 2c20 6275 740a 2020 2020   dsyev, but.    
-00013f00: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00013f10: 6173 7465 722e 2054 6869 7320 6973 206e  aster. This is n
-00013f20: 6f74 2072 6563 6f6d 6d65 6e64 6564 2062  ot recommended b
-00013f30: 6563 6175 7365 2073 6f6d 6574 696d 6573  ecause sometimes
-00013f40: 2061 2077 726f 6e67 0a20 2020 2020 2020   a wrong.       
-00013f50: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00013f60: 6c74 2069 7320 6f62 7461 696e 6564 2e0a  lt is obtained..
-00013f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f80: 332e 204e 756d 7079 e280 9973 2064 7379  3. Numpy...s dsy
-00013f90: 6576 6420 286c 696e 616c 672e 6569 6768  evd (linalg.eigh
-00013fa0: 292e 2054 6869 7320 6973 206e 6f74 2072  ). This is not r
-00013fb0: 6563 6f6d 6d65 6e64 6564 0a20 2020 2020  ecommended.     
-00013fc0: 2020 2020 2020 2020 2020 2020 2020 6265                be
-00013fd0: 6361 7573 6520 736f 6d65 7469 6d65 7320  cause sometimes 
-00013fe0: 6120 7772 6f6e 6720 7265 7375 6c74 2069  a wrong result i
-00013ff0: 7320 6f62 7461 696e 6564 2e0a 2020 2020  s obtained..    
-00014000: 2020 2020 2020 2020 2020 2020 342e 2053              4. S
-00014010: 6369 7079 e280 9973 2064 7379 6576 3a20  cipy...s dsyev: 
-00014020: 5468 6973 2069 7320 7468 6520 6465 6661  This is the defa
-00014030: 756c 7420 736f 6c76 6572 2077 6865 6e20  ult solver when 
-00014040: 7363 6970 7920 6973 0a20 2020 2020 2020  scipy is.       
-00014050: 2020 2020 2020 2020 2020 2020 696e 7374              inst
-00014060: 616c 6c65 6420 616e 6420 4d4b 4c20 4c41  alled and MKL LA
-00014070: 5041 434b 4520 6973 206e 6f74 2069 6e74  PACKE is not int
-00014080: 6567 7261 7465 642e 0a20 2020 2020 2020  egrated..       
-00014090: 2020 2020 2020 2020 2035 2e20 5363 6970           5. Scip
-000140a0: 79e2 8099 7320 6473 7965 7664 2e20 5468  y...s dsyevd. Th
-000140b0: 6973 2069 7320 6e6f 7420 7265 636f 6d6d  is is not recomm
-000140c0: 656e 6465 6420 6265 6361 7573 6520 736f  ended because so
-000140d0: 6d65 7469 6d65 730a 2020 2020 2020 2020  metimes.        
-000140e0: 2020 2020 2020 2020 2020 2061 2077 726f             a wro
-000140f0: 6e67 2072 6573 756c 7420 6973 206f 6274  ng result is obt
-00014100: 6169 6e65 642e 0a20 2020 2020 2020 2020  ained..         
-00014110: 2020 2054 6865 2073 6f6c 7665 7220 6368     The solver ch
-00014120: 6f69 6365 7320 6f74 6865 7220 7468 616e  oices other than
-00014130: 202d 2d70 696e 762d 736f 6c76 6572 3d31   --pinv-solver=1
-00014140: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
-00014150: 202d 2d70 696e 762d 736f 6c76 6572 3d34   --pinv-solver=4
-00014160: 2061 7265 2064 616e 6765 726f 7573 2061   are dangerous a
-00014170: 6e64 206e 6f74 2072 6563 6f6d 6d65 6e64  nd not recommend
-00014180: 2e0a 2020 2020 2020 2020 7772 6974 655f  ..        write_
-00014190: 6761 6d6d 6120 3a20 626f 6f6c 2c20 6f70  gamma : bool, op
-000141a0: 7469 6f6e 616c 2c20 6465 6661 756c 7420  tional, default 
-000141b0: 6973 2046 616c 7365 0a20 2020 2020 2020  is False.       
-000141c0: 2020 2020 2052 5441 206f 6e6c 7920 2860       RTA only (`
-000141d0: 6973 5f4c 4254 453d 4661 6c73 6560 292e  is_LBTE=False`).
-000141e0: 2057 6974 6820 5472 7565 2c20 5772 6974   With True, Writ
-000141f0: 6520 6d6f 6465 2074 6865 726d 616c 0a20  e mode thermal. 
-00014200: 2020 2020 2020 2020 2020 2063 6f6e 6475             condu
-00014210: 6374 6976 6974 7920 7072 6f70 6572 7469  ctivity properti
-00014220: 6573 2069 6e74 6f20 6669 6c65 7320 6174  es into files at
-00014230: 2065 6163 6820 6772 6964 2070 6f69 6e74   each grid point
-00014240: 2e20 5769 7468 0a20 2020 2020 2020 2020  . With.         
-00014250: 2020 2060 6261 6e64 5f69 6e64 6963 6573     `band_indices
-00014260: 6020 6f72 206d 756c 7469 706c 6520 6073  ` or multiple `s
-00014270: 6967 6d61 7360 2069 7320 7370 6563 6966  igmas` is specif
-00014280: 6965 642c 2074 6865 2066 696c 6573 0a20  ied, the files. 
-00014290: 2020 2020 2020 2020 2020 2061 7265 206d             are m
-000142a0: 6164 6520 666f 7220 6561 6368 206f 6620  ade for each of 
-000142b0: 7468 656d 2c20 746f 6f2e 0a20 2020 2020  them, too..     
-000142c0: 2020 2072 6561 645f 6761 6d6d 6120 3a20     read_gamma : 
-000142d0: 626f 6f6c 2c20 6f70 7469 6f6e 616c 2c20  bool, optional, 
-000142e0: 6465 6661 756c 7420 6973 2046 616c 7365  default is False
-000142f0: 0a20 2020 2020 2020 2020 2020 2052 5441  .            RTA
-00014300: 206f 6e6c 7920 2860 6973 5f4c 4254 453d   only (`is_LBTE=
-00014310: 4661 6c73 6560 292e 2057 6974 6820 5472  False`). With Tr
-00014320: 7565 2c20 6465 6164 2066 696c 6573 2063  ue, dead files c
-00014330: 7265 6174 6564 2062 790a 2020 2020 2020  reated by.      
-00014340: 2020 2020 2020 6077 7269 7465 5f67 616d        `write_gam
-00014350: 6d61 3d54 7275 6560 2069 6e73 7465 6164  ma=True` instead
-00014360: 206f 6620 6361 6c63 756c 6174 696e 6720   of calculating 
-00014370: 7068 6f6e 6f6e 2d70 686f 6e6f 6e0a 2020  phonon-phonon.  
-00014380: 2020 2020 2020 2020 2020 696e 7465 7261            intera
-00014390: 6374 696f 6e20 7374 7265 6e67 7468 2061  ction strength a
-000143a0: 6e64 2069 6d61 6769 6e61 7279 2070 6172  nd imaginary par
-000143b0: 7473 206f 6620 7365 6c66 2d65 6e65 7267  ts of self-energ
-000143c0: 792e 0a20 2020 2020 2020 2069 735f 4e5f  y..        is_N_
-000143d0: 5520 3a20 626f 6f6c 2c20 6f70 7469 6f6e  U : bool, option
-000143e0: 616c 2c20 6465 6661 756c 7420 6973 2046  al, default is F
-000143f0: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
-00014400: 2052 5441 206f 6e6c 7920 2860 6973 5f4c   RTA only (`is_L
-00014410: 4254 453d 4661 6c73 6560 292e 2057 6974  BTE=False`). Wit
-00014420: 6820 5472 7565 2c20 6361 7465 676f 7269  h True, categori
-00014430: 7a61 7469 6f6e 206f 6620 6e6f 726d 616c  zation of normal
-00014440: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
-00014450: 2055 6d6b 6c61 7070 2073 6361 7474 6572   Umklapp scatter
-00014460: 696e 6720 6973 206d 6164 6520 616e 6420  ing is made and 
-00014470: 696d 6167 696e 6172 7920 7061 7274 7320  imaginary parts 
-00014480: 6f66 2073 656c 6620 656e 6572 6779 0a20  of self energy. 
-00014490: 2020 2020 2020 2020 2020 2066 6f72 2074             for t
-000144a0: 6865 6d20 6172 6520 7365 7061 7261 7465  hem are separate
-000144b0: 642e 0a20 2020 2020 2020 2063 6f6e 6475  d..        condu
-000144c0: 6374 6976 6974 795f 7479 7065 203a 2073  ctivity_type : s
-000144d0: 7472 2c20 6f70 7469 6f6e 616c 0a20 2020  tr, optional.   
-000144e0: 2020 2020 2020 2020 2022 7769 676e 6572           "wigner
-000144f0: 222c 2022 6b75 626f 222c 206f 7220 4e6f  ", "kubo", or No
-00014500: 6e65 2e20 4465 6661 756c 7420 6973 204e  ne. Default is N
-00014510: 6f6e 652e 0a20 2020 2020 2020 2077 7269  one..        wri
-00014520: 7465 5f6b 6170 7061 203a 2062 6f6f 6c2c  te_kappa : bool,
-00014530: 206f 7074 696f 6e61 6c2c 2064 6566 6175   optional, defau
-00014540: 6c74 2069 7320 4661 6c73 650a 2020 2020  lt is False.    
-00014550: 2020 2020 2020 2020 5769 7468 2054 7275          With Tru
-00014560: 652c 2074 6865 726d 616c 2063 6f6e 6475  e, thermal condu
-00014570: 6374 6976 6974 7920 616e 6420 7265 6c61  ctivity and rela
-00014580: 7465 6420 7072 6f70 6572 7469 6573 2061  ted properties a
-00014590: 7265 0a20 2020 2020 2020 2020 2020 2077  re.            w
-000145a0: 7269 7474 656e 2069 6e74 6f20 6120 6669  ritten into a fi
-000145b0: 6c65 2e20 5769 7468 206d 756c 7469 706c  le. With multipl
-000145c0: 6520 6073 6967 6d61 7360 2c20 7265 7370  e `sigmas`, resp
-000145d0: 6563 7469 7665 2066 696c 6573 0a20 2020  ective files.   
-000145e0: 2020 2020 2020 2020 2061 7265 2063 7265           are cre
-000145f0: 6174 6564 2e0a 2020 2020 2020 2020 7772  ated..        wr
-00014600: 6974 655f 6761 6d6d 615f 6465 7461 696c  ite_gamma_detail
-00014610: 203a 2062 6f6f 6c2c 206f 7074 696f 6e61   : bool, optiona
-00014620: 6c2c 2064 6566 6175 6c74 2069 7320 4661  l, default is Fa
-00014630: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
-00014640: 5254 4120 6f6e 6c79 2028 6069 735f 4c42  RTA only (`is_LB
-00014650: 5445 3d46 616c 7365 6029 2e20 5769 7468  TE=False`). With
-00014660: 2054 7275 652c 2064 6574 6169 6c65 6420   True, detailed 
-00014670: 696e 666f 726d 6174 696f 6e20 6f66 0a20  information of. 
-00014680: 2020 2020 2020 2020 2020 2069 6d61 6769             imagi
-00014690: 6e61 7279 2070 6172 7473 206f 6620 7365  nary parts of se
-000146a0: 6c66 2065 6e65 7267 7920 6973 2073 746f  lf energy is sto
-000146b0: 7265 6420 696e 746f 2066 696c 6573 2073  red into files s
-000146c0: 7563 6820 6173 0a20 2020 2020 2020 2020  uch as.         
-000146d0: 2020 2074 686f 7365 206d 6164 6520 6279     those made by
-000146e0: 2060 7772 6974 655f 6761 6d6d 6160 2e0a   `write_gamma`..
-000146f0: 2020 2020 2020 2020 7772 6974 655f 636f          write_co
-00014700: 6c6c 6973 696f 6e20 3a20 626f 6f6c 2c20  llision : bool, 
-00014710: 6f70 7469 6f6e 616c 2c20 6465 6661 756c  optional, defaul
-00014720: 7420 6973 2046 616c 7365 0a20 2020 2020  t is False.     
-00014730: 2020 2020 2020 2044 6972 6563 7420 736f         Direct so
-00014740: 6c75 7469 6f6e 206f 6e6c 7920 2860 6973  lution only (`is
-00014750: 5f4c 4254 453d 5472 7565 6029 2e20 5769  _LBTE=True`). Wi
-00014760: 7468 2054 7275 652c 2063 6f6c 6c69 7369  th True, collisi
-00014770: 6f6e 206d 6174 7269 780a 2020 2020 2020  on matrix.      
-00014780: 2020 2020 2020 6973 2077 7269 7474 656e        is written
-00014790: 2069 6e74 6f20 6120 6669 6c65 2e20 5769   into a file. Wi
-000147a0: 7468 206d 756c 7469 706c 6520 6073 6967  th multiple `sig
-000147b0: 6d61 7360 2073 7065 6369 6669 6564 2c0a  mas` specified,.
-000147c0: 2020 2020 2020 2020 2020 2020 7265 7370              resp
-000147d0: 6563 7469 7665 2066 696c 6573 2061 7265  ective files are
-000147e0: 2063 7265 6174 6564 2e20 4265 2063 6172   created. Be car
-000147f0: 6566 756c 2074 6861 7420 7468 6973 2066  eful that this f
-00014800: 696c 6520 6361 6e20 6265 0a20 2020 2020  ile can be.     
-00014810: 2020 2020 2020 2068 7567 652e 0a20 2020         huge..   
-00014820: 2020 2020 2072 6561 645f 636f 6c6c 6973       read_collis
-00014830: 696f 6e20 3a20 626f 6f6c 2c20 6f70 7469  ion : bool, opti
-00014840: 6f6e 616c 2c20 6465 6661 756c 7420 6973  onal, default is
-00014850: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
-00014860: 2020 2044 6972 6563 7420 736f 6c75 7469     Direct soluti
-00014870: 6f6e 206f 6e6c 7920 2860 6973 5f4c 4254  on only (`is_LBT
-00014880: 453d 5472 7565 6029 2e20 5769 7468 2054  E=True`). With T
-00014890: 7275 652c 2063 6f6c 6c69 7369 6f6e 206d  rue, collision m
-000148a0: 6174 7269 780a 2020 2020 2020 2020 2020  atrix.          
-000148b0: 2020 6973 2072 6561 6420 6672 6f6d 2061    is read from a
-000148c0: 2066 696c 652e 0a20 2020 2020 2020 2077   file..        w
-000148d0: 7269 7465 5f70 7020 3a20 626f 6f6c 2c20  rite_pp : bool, 
-000148e0: 6f70 7469 6f6e 616c 2c20 6465 6661 756c  optional, defaul
-000148f0: 7420 6973 2046 616c 7365 0a20 2020 2020  t is False.     
-00014900: 2020 2020 2020 2057 6974 6820 5472 7565         With True
-00014910: 2c20 7068 6f6e 6f6e 2d70 686f 6e6f 6e20  , phonon-phonon 
-00014920: 696e 7465 7261 6374 696f 6e20 7374 7265  interaction stre
-00014930: 6e67 7468 2069 7320 7772 6974 7465 6e20  ngth is written 
-00014940: 696e 746f 0a20 2020 2020 2020 2020 2020  into.           
-00014950: 2066 696c 6573 2061 7420 6561 6368 2067   files at each g
-00014960: 7269 6420 706f 696e 742e 2054 6869 7320  rid point. This 
-00014970: 6f70 7469 6f6e 2061 7373 756d 6573 2073  option assumes s
-00014980: 696e 676c 6520 7661 6c75 6520 6973 2069  ingle value is i
-00014990: 6e0a 2020 2020 2020 2020 2020 2020 6073  n.            `s
-000149a0: 6967 6d61 7360 2e0a 2020 2020 2020 2020  igmas`..        
-000149b0: 7265 6164 5f70 7020 3a20 626f 6f6c 2c20  read_pp : bool, 
-000149c0: 6f70 7469 6f6e 616c 2c20 6465 6661 756c  optional, defaul
-000149d0: 7420 6973 2046 616c 7365 0a20 2020 2020  t is False.     
-000149e0: 2020 2020 2020 2057 6974 6820 5472 7565         With True
-000149f0: 2c20 7068 6f6e 6f6e 2d70 686f 6e6f 6e20  , phonon-phonon 
-00014a00: 696e 7465 7261 6374 696f 6e20 7374 7265  interaction stre
-00014a10: 6e67 7468 2069 7320 7265 6164 2066 726f  ngth is read fro
-00014a20: 6d20 6669 6c65 732e 0a20 2020 2020 2020  m files..       
-00014a30: 2077 7269 7465 5f4c 4254 455f 736f 6c75   write_LBTE_solu
-00014a40: 7469 6f6e 203a 2062 6f6f 6c2c 206f 7074  tion : bool, opt
-00014a50: 696f 6e61 6c2c 2064 6566 6175 6c74 2069  ional, default i
-00014a60: 7320 4661 6c73 650a 2020 2020 2020 2020  s False.        
-00014a70: 2020 2020 4469 7265 6374 2073 6f6c 7574      Direct solut
-00014a80: 696f 6e20 6f6e 6c79 2028 6069 735f 4c42  ion only (`is_LB
-00014a90: 5445 3d54 7275 6560 292e 2057 6974 6820  TE=True`). With 
-00014aa0: 5472 7565 2c20 6569 6765 6e76 6563 746f  True, eigenvecto
-00014ab0: 7273 206f 660a 2020 2020 2020 2020 2020  rs of.          
-00014ac0: 2020 636f 6c6c 6973 696f 6e20 6d61 7472    collision matr
-00014ad0: 6978 2069 7320 7772 6974 7465 6e20 696e  ix is written in
-00014ae0: 2061 2066 696c 6520 6173 2074 6865 2072   a file as the r
-00014af0: 6f77 2076 6563 746f 7273 2065 7863 6570  ow vectors excep
-00014b00: 740a 2020 2020 2020 2020 2020 2020 756e  t.            un
-00014b10: 6c65 7373 2060 7069 6e76 5f73 6f6c 7665  less `pinv_solve
-00014b20: 723d 3360 2028 666f 7220 7468 6973 2c20  r=3` (for this, 
-00014b30: 636f 6c75 6d6e 2076 6563 746f 7273 292e  column vectors).
-00014b40: 2057 6974 6820 6d75 6c74 6970 6c65 0a20   With multiple. 
-00014b50: 2020 2020 2020 2020 2020 2060 7369 676d             `sigm
-00014b60: 6173 6020 7370 6563 6966 6965 642c 2072  as` specified, r
-00014b70: 6573 7065 6374 6976 6520 6669 6c65 7320  espective files 
-00014b80: 6172 6520 6372 6561 7465 642e 2042 6520  are created. Be 
-00014b90: 6361 7265 6675 6c20 7468 6174 0a20 2020  careful that.   
-00014ba0: 2020 2020 2020 2020 2074 6869 7320 6669           this fi
-00014bb0: 6c65 2063 616e 2062 6520 6875 6765 2e0a  le can be huge..
-00014bc0: 2020 2020 2020 2020 636f 6d70 7265 7373          compress
-00014bd0: 696f 6e3a 2073 7472 2c20 6f70 7469 6f6e  ion: str, option
-00014be0: 616c 2c20 6465 6661 756c 7420 6973 2022  al, default is "
-00014bf0: 677a 6970 220a 2020 2020 2020 2020 2020  gzip".          
-00014c00: 2020 5768 656e 2077 7269 7469 6e67 2072    When writing r
-00014c10: 6573 756c 7473 2069 6e74 6f20 6669 6c65  esults into file
-00014c20: 7320 696e 2068 6466 352c 206c 6172 6765  s in hdf5, large
-00014c30: 2064 6174 6120 6172 6520 636f 6d70 7265   data are compre
-00014c40: 7373 6564 0a20 2020 2020 2020 2020 2020  ssed.           
-00014c50: 2062 7920 7468 6973 206f 7074 696f 6e73   by this options
-00014c60: 2e20 5365 6520 7468 6520 6465 7461 696c  . See the detail
-00014c70: 2061 7420 6835 7079 2064 6f63 756d 656e   at h5py documen
-00014c80: 7461 7469 6f6e 2e0a 2020 2020 2020 2020  tation..        
-00014c90: 696e 7075 745f 6669 6c65 6e61 6d65 203a  input_filename :
-00014ca0: 2073 7472 2c20 6f70 7469 6f6e 616c 2c20   str, optional, 
-00014cb0: 6465 6661 756c 7420 6973 204e 6f6e 650a  default is None.
-00014cc0: 2020 2020 2020 2020 2020 2020 5768 656e              When
-00014cd0: 2073 7065 6369 6669 6564 2c20 7468 6520   specified, the 
-00014ce0: 7374 7269 6e67 2069 7320 696e 7365 7274  string is insert
-00014cf0: 6564 2062 6566 6f72 6520 6669 6c65 6e61  ed before filena
-00014d00: 6d65 2065 7874 656e 7369 6f6e 0a20 2020  me extension.   
-00014d10: 2020 2020 2020 2020 2069 6e20 7265 6164           in read
-00014d20: 696e 6720 6669 6c65 732e 0a20 2020 2020  ing files..     
-00014d30: 2020 206f 7574 7075 745f 6669 6c65 6e61     output_filena
-00014d40: 6d65 203a 2073 7472 2c20 6f70 7469 6f6e  me : str, option
-00014d50: 616c 2c20 6465 6661 756c 7420 6973 204e  al, default is N
-00014d60: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-00014d70: 5768 656e 2073 7065 6369 6669 6564 2c20  When specified, 
-00014d80: 7468 6520 7374 7269 6e67 2069 7320 696e  the string is in
-00014d90: 7365 7274 6564 2062 6566 6f72 6520 6669  serted before fi
-00014da0: 6c65 6e61 6d65 2065 7874 656e 7369 6f6e  lename extension
-00014db0: 0a20 2020 2020 2020 2020 2020 2069 6e20  .            in 
-00014dc0: 7772 6974 696e 6720 6669 6c65 732e 0a0a  writing files...
-00014dd0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00014de0: 2020 2020 6966 2073 656c 662e 5f69 6e74      if self._int
-00014df0: 6572 6163 7469 6f6e 2069 7320 4e6f 6e65  eraction is None
-00014e00: 3a0a 2020 2020 2020 2020 2020 2020 6d73  :.            ms
-00014e10: 6720 3d20 280a 2020 2020 2020 2020 2020  g = (.          
-00014e20: 2020 2020 2020 2250 686f 6e6f 3370 792e        "Phono3py.
-00014e30: 696e 6974 5f70 6870 685f 696e 7465 7261  init_phph_intera
-00014e40: 6374 696f 6e20 6861 7320 746f 2062 6520  ction has to be 
-00014e50: 6361 6c6c 6564 2022 0a20 2020 2020 2020  called ".       
-00014e60: 2020 2020 2020 2020 2022 6265 666f 7265           "before
-00014e70: 2072 756e 6e69 6e67 2074 6869 7320 6d65   running this me
-00014e80: 7468 6f64 2e22 0a20 2020 2020 2020 2020  thod.".         
-00014e90: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00014ea0: 2072 6169 7365 2052 756e 7469 6d65 4572   raise RuntimeEr
-00014eb0: 726f 7228 6d73 6729 0a0a 2020 2020 2020  ror(msg)..      
-00014ec0: 2020 6966 2069 735f 4c42 5445 3a0a 2020    if is_LBTE:.  
-00014ed0: 2020 2020 2020 2020 2020 6966 2074 656d            if tem
-00014ee0: 7065 7261 7475 7265 7320 6973 204e 6f6e  peratures is Non
-00014ef0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00014f00: 2020 205f 7465 6d70 6572 6174 7572 6573     _temperatures
-00014f10: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
-00014f20: 2020 2020 2020 2020 2033 3030 2c0a 2020           300,.  
-00014f30: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
-00014f40: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00014f50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00014f60: 2020 5f74 656d 7065 7261 7475 7265 7320    _temperatures 
-00014f70: 3d20 7465 6d70 6572 6174 7572 6573 0a20  = temperatures. 
-00014f80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00014f90: 5f74 6865 726d 616c 5f63 6f6e 6475 6374  _thermal_conduct
-00014fa0: 6976 6974 7920 3d20 6765 745f 7468 6572  ivity = get_ther
-00014fb0: 6d61 6c5f 636f 6e64 7563 7469 7669 7479  mal_conductivity
-00014fc0: 5f4c 4254 4528 0a20 2020 2020 2020 2020  _LBTE(.         
-00014fd0: 2020 2020 2020 2073 656c 662e 5f69 6e74         self._int
-00014fe0: 6572 6163 7469 6f6e 2c0a 2020 2020 2020  eraction,.      
-00014ff0: 2020 2020 2020 2020 2020 7465 6d70 6572            temper
-00015000: 6174 7572 6573 3d5f 7465 6d70 6572 6174  atures=_temperat
-00015010: 7572 6573 2c0a 2020 2020 2020 2020 2020  ures,.          
-00015020: 2020 2020 2020 7369 676d 6173 3d73 656c        sigmas=sel
-00015030: 662e 5f73 6967 6d61 732c 0a20 2020 2020  f._sigmas,.     
-00015040: 2020 2020 2020 2020 2020 2073 6967 6d61             sigma
-00015050: 5f63 7574 6f66 663d 7365 6c66 2e5f 7369  _cutoff=self._si
-00015060: 676d 615f 6375 746f 6666 2c0a 2020 2020  gma_cutoff,.    
-00015070: 2020 2020 2020 2020 2020 2020 6973 5f69              is_i
-00015080: 736f 746f 7065 3d69 735f 6973 6f74 6f70  sotope=is_isotop
-00015090: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-000150a0: 2020 206d 6173 735f 7661 7269 616e 6365     mass_variance
-000150b0: 733d 6d61 7373 5f76 6172 6961 6e63 6573  s=mass_variances
-000150c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000150d0: 2020 6772 6964 5f70 6f69 6e74 733d 6772    grid_points=gr
-000150e0: 6964 5f70 6f69 6e74 732c 0a20 2020 2020  id_points,.     
-000150f0: 2020 2020 2020 2020 2020 2062 6f75 6e64             bound
-00015100: 6172 795f 6d66 703d 626f 756e 6461 7279  ary_mfp=boundary
-00015110: 5f6d 6670 2c0a 2020 2020 2020 2020 2020  _mfp,.          
-00015120: 2020 2020 2020 736f 6c76 655f 636f 6c6c        solve_coll
-00015130: 6563 7469 7665 5f70 686f 6e6f 6e3d 736f  ective_phonon=so
-00015140: 6c76 655f 636f 6c6c 6563 7469 7665 5f70  lve_collective_p
-00015150: 686f 6e6f 6e2c 0a20 2020 2020 2020 2020  honon,.         
-00015160: 2020 2020 2020 2069 735f 7265 6475 6369         is_reduci
-00015170: 626c 655f 636f 6c6c 6973 696f 6e5f 6d61  ble_collision_ma
-00015180: 7472 6978 3d69 735f 7265 6475 6369 626c  trix=is_reducibl
-00015190: 655f 636f 6c6c 6973 696f 6e5f 6d61 7472  e_collision_matr
-000151a0: 6978 2c0a 2020 2020 2020 2020 2020 2020  ix,.            
-000151b0: 2020 2020 6973 5f6b 6170 7061 5f73 7461      is_kappa_sta
-000151c0: 723d 6973 5f6b 6170 7061 5f73 7461 722c  r=is_kappa_star,
-000151d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000151e0: 2067 765f 6465 6c74 615f 713d 6776 5f64   gv_delta_q=gv_d
-000151f0: 656c 7461 5f71 2c0a 2020 2020 2020 2020  elta_q,.        
-00015200: 2020 2020 2020 2020 6973 5f66 756c 6c5f          is_full_
-00015210: 7070 3d69 735f 6675 6c6c 5f70 702c 0a20  pp=is_full_pp,. 
-00015220: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00015230: 6f6e 6475 6374 6976 6974 795f 7479 7065  onductivity_type
-00015240: 3d63 6f6e 6475 6374 6976 6974 795f 7479  =conductivity_ty
-00015250: 7065 2c0a 2020 2020 2020 2020 2020 2020  pe,.            
-00015260: 2020 2020 7069 6e76 5f63 7574 6f66 663d      pinv_cutoff=
-00015270: 7069 6e76 5f63 7574 6f66 662c 0a20 2020  pinv_cutoff,.   
-00015280: 2020 2020 2020 2020 2020 2020 2070 696e               pin
-00015290: 765f 736f 6c76 6572 3d70 696e 765f 736f  v_solver=pinv_so
-000152a0: 6c76 6572 2c0a 2020 2020 2020 2020 2020  lver,.          
-000152b0: 2020 2020 2020 7069 6e76 5f6d 6574 686f        pinv_metho
-000152c0: 643d 7069 6e76 5f6d 6574 686f 642c 0a20  d=pinv_method,. 
-000152d0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-000152e0: 7269 7465 5f63 6f6c 6c69 7369 6f6e 3d77  rite_collision=w
-000152f0: 7269 7465 5f63 6f6c 6c69 7369 6f6e 2c0a  rite_collision,.
-00015300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015310: 7265 6164 5f63 6f6c 6c69 7369 6f6e 3d72  read_collision=r
-00015320: 6561 645f 636f 6c6c 6973 696f 6e2c 0a20  ead_collision,. 
-00015330: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00015340: 7269 7465 5f6b 6170 7061 3d77 7269 7465  rite_kappa=write
-00015350: 5f6b 6170 7061 2c0a 2020 2020 2020 2020  _kappa,.        
-00015360: 2020 2020 2020 2020 7772 6974 655f 7070          write_pp
-00015370: 3d77 7269 7465 5f70 702c 0a20 2020 2020  =write_pp,.     
-00015380: 2020 2020 2020 2020 2020 2072 6561 645f             read_
-00015390: 7070 3d72 6561 645f 7070 2c0a 2020 2020  pp=read_pp,.    
-000153a0: 2020 2020 2020 2020 2020 2020 7772 6974              writ
-000153b0: 655f 4c42 5445 5f73 6f6c 7574 696f 6e3d  e_LBTE_solution=
-000153c0: 7772 6974 655f 4c42 5445 5f73 6f6c 7574  write_LBTE_solut
-000153d0: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-000153e0: 2020 2020 2063 6f6d 7072 6573 7369 6f6e       compression
-000153f0: 3d63 6f6d 7072 6573 7369 6f6e 2c0a 2020  =compression,.  
-00015400: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00015410: 7075 745f 6669 6c65 6e61 6d65 3d69 6e70  put_filename=inp
-00015420: 7574 5f66 696c 656e 616d 652c 0a20 2020  ut_filename,.   
-00015430: 2020 2020 2020 2020 2020 2020 206f 7574               out
-00015440: 7075 745f 6669 6c65 6e61 6d65 3d6f 7574  put_filename=out
-00015450: 7075 745f 6669 6c65 6e61 6d65 2c0a 2020  put_filename,.  
-00015460: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00015470: 675f 6c65 7665 6c3d 7365 6c66 2e5f 6c6f  g_level=self._lo
-00015480: 675f 6c65 7665 6c2c 0a20 2020 2020 2020  g_level,.       
-00015490: 2020 2020 2029 0a20 2020 2020 2020 2065       ).        e
-000154a0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-000154b0: 2069 6620 7465 6d70 6572 6174 7572 6573   if temperatures
-000154c0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-000154d0: 2020 2020 2020 2020 2020 5f74 656d 7065            _tempe
-000154e0: 7261 7475 7265 7320 3d20 6e70 2e61 7261  ratures = np.ara
-000154f0: 6e67 6528 302c 2031 3030 312c 2031 302c  nge(0, 1001, 10,
-00015500: 2064 7479 7065 3d22 646f 7562 6c65 2229   dtype="double")
-00015510: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00015520: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00015530: 2020 205f 7465 6d70 6572 6174 7572 6573     _temperatures
-00015540: 203d 2074 656d 7065 7261 7475 7265 730a   = temperatures.
-00015550: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015560: 2e5f 7468 6572 6d61 6c5f 636f 6e64 7563  ._thermal_conduc
-00015570: 7469 7669 7479 203d 2067 6574 5f74 6865  tivity = get_the
-00015580: 726d 616c 5f63 6f6e 6475 6374 6976 6974  rmal_conductivit
-00015590: 795f 5254 4128 0a20 2020 2020 2020 2020  y_RTA(.         
-000155a0: 2020 2020 2020 2073 656c 662e 5f69 6e74         self._int
-000155b0: 6572 6163 7469 6f6e 2c0a 2020 2020 2020  eraction,.      
-000155c0: 2020 2020 2020 2020 2020 7465 6d70 6572            temper
-000155d0: 6174 7572 6573 3d5f 7465 6d70 6572 6174  atures=_temperat
-000155e0: 7572 6573 2c0a 2020 2020 2020 2020 2020  ures,.          
-000155f0: 2020 2020 2020 7369 676d 6173 3d73 656c        sigmas=sel
-00015600: 662e 5f73 6967 6d61 732c 0a20 2020 2020  f._sigmas,.     
-00015610: 2020 2020 2020 2020 2020 2073 6967 6d61             sigma
-00015620: 5f63 7574 6f66 663d 7365 6c66 2e5f 7369  _cutoff=self._si
-00015630: 676d 615f 6375 746f 6666 2c0a 2020 2020  gma_cutoff,.    
-00015640: 2020 2020 2020 2020 2020 2020 6973 5f69              is_i
-00015650: 736f 746f 7065 3d69 735f 6973 6f74 6f70  sotope=is_isotop
-00015660: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00015670: 2020 206d 6173 735f 7661 7269 616e 6365     mass_variance
-00015680: 733d 6d61 7373 5f76 6172 6961 6e63 6573  s=mass_variances
-00015690: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000156a0: 2020 6772 6964 5f70 6f69 6e74 733d 6772    grid_points=gr
-000156b0: 6964 5f70 6f69 6e74 732c 0a20 2020 2020  id_points,.     
-000156c0: 2020 2020 2020 2020 2020 2062 6f75 6e64             bound
-000156d0: 6172 795f 6d66 703d 626f 756e 6461 7279  ary_mfp=boundary
-000156e0: 5f6d 6670 2c0a 2020 2020 2020 2020 2020  _mfp,.          
-000156f0: 2020 2020 2020 7573 655f 6176 655f 7070        use_ave_pp
-00015700: 3d75 7365 5f61 7665 5f70 702c 0a20 2020  =use_ave_pp,.   
-00015710: 2020 2020 2020 2020 2020 2020 2069 735f               is_
-00015720: 6b61 7070 615f 7374 6172 3d69 735f 6b61  kappa_star=is_ka
-00015730: 7070 615f 7374 6172 2c0a 2020 2020 2020  ppa_star,.      
-00015740: 2020 2020 2020 2020 2020 6776 5f64 656c            gv_del
-00015750: 7461 5f71 3d67 765f 6465 6c74 615f 712c  ta_q=gv_delta_q,
-00015760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015770: 2069 735f 6675 6c6c 5f70 703d 6973 5f66   is_full_pp=is_f
-00015780: 756c 6c5f 7070 2c0a 2020 2020 2020 2020  ull_pp,.        
-00015790: 2020 2020 2020 2020 6973 5f4e 5f55 3d69          is_N_U=i
-000157a0: 735f 4e5f 552c 0a20 2020 2020 2020 2020  s_N_U,.         
-000157b0: 2020 2020 2020 2063 6f6e 6475 6374 6976         conductiv
-000157c0: 6974 795f 7479 7065 3d63 6f6e 6475 6374  ity_type=conduct
-000157d0: 6976 6974 795f 7479 7065 2c0a 2020 2020  ivity_type,.    
-000157e0: 2020 2020 2020 2020 2020 2020 7772 6974              writ
-000157f0: 655f 6761 6d6d 613d 7772 6974 655f 6761  e_gamma=write_ga
-00015800: 6d6d 612c 0a20 2020 2020 2020 2020 2020  mma,.           
-00015810: 2020 2020 2072 6561 645f 6761 6d6d 613d       read_gamma=
-00015820: 7265 6164 5f67 616d 6d61 2c0a 2020 2020  read_gamma,.    
-00015830: 2020 2020 2020 2020 2020 2020 7772 6974              writ
-00015840: 655f 6b61 7070 613d 7772 6974 655f 6b61  e_kappa=write_ka
-00015850: 7070 612c 0a20 2020 2020 2020 2020 2020  ppa,.           
-00015860: 2020 2020 2077 7269 7465 5f70 703d 7772       write_pp=wr
-00015870: 6974 655f 7070 2c0a 2020 2020 2020 2020  ite_pp,.        
-00015880: 2020 2020 2020 2020 7265 6164 5f70 703d          read_pp=
-00015890: 7265 6164 5f70 702c 0a20 2020 2020 2020  read_pp,.       
-000158a0: 2020 2020 2020 2020 2077 7269 7465 5f67           write_g
-000158b0: 616d 6d61 5f64 6574 6169 6c3d 7772 6974  amma_detail=writ
-000158c0: 655f 6761 6d6d 615f 6465 7461 696c 2c0a  e_gamma_detail,.
-000158d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000158e0: 636f 6d70 7265 7373 696f 6e3d 636f 6d70  compression=comp
-000158f0: 7265 7373 696f 6e2c 0a20 2020 2020 2020  ression,.       
-00015900: 2020 2020 2020 2020 2069 6e70 7574 5f66           input_f
-00015910: 696c 656e 616d 653d 696e 7075 745f 6669  ilename=input_fi
-00015920: 6c65 6e61 6d65 2c0a 2020 2020 2020 2020  lename,.        
-00015930: 2020 2020 2020 2020 6f75 7470 7574 5f66          output_f
-00015940: 696c 656e 616d 653d 6f75 7470 7574 5f66  ilename=output_f
-00015950: 696c 656e 616d 652c 0a20 2020 2020 2020  ilename,.       
-00015960: 2020 2020 2020 2020 206c 6f67 5f6c 6576           log_lev
-00015970: 656c 3d73 656c 662e 5f6c 6f67 5f6c 6576  el=self._log_lev
-00015980: 656c 2c0a 2020 2020 2020 2020 2020 2020  el,.            
-00015990: 290a 0a20 2020 2064 6566 2073 6176 6528  )..    def save(
-000159a0: 7365 6c66 2c20 6669 6c65 6e61 6d65 3d22  self, filename="
-000159b0: 7068 6f6e 6f33 7079 5f70 6172 616d 732e  phono3py_params.
-000159c0: 7961 6d6c 222c 2073 6574 7469 6e67 733d  yaml", settings=
-000159d0: 4e6f 6e65 293a 0a20 2020 2020 2020 2022  None):.        "
-000159e0: 2222 5361 7665 2070 6172 616d 6574 6572  ""Save parameter
-000159f0: 7320 696e 2050 686f 6e6f 3370 7920 696e  s in Phono3py in
-00015a00: 7374 616e 7473 2069 6e74 6f20 6669 6c65  stants into file
-00015a10: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-00015a20: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-00015a30: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-00015a40: 2066 696c 656e 616d 653a 2073 7472 2c20   filename: str, 
-00015a50: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-00015a60: 2020 2020 2046 696c 6520 6e61 6d65 2e20       File name. 
-00015a70: 4465 6661 756c 7420 6973 2022 7068 6f6e  Default is "phon
-00015a80: 6f33 7079 5f70 6172 616d 732e 7961 6d6c  o3py_params.yaml
-00015a90: 220a 2020 2020 2020 2020 7365 7474 696e  ".        settin
-00015aa0: 6773 3a20 6469 6374 2c20 6f70 7469 6f6e  gs: dict, option
-00015ab0: 616c 0a20 2020 2020 2020 2020 2020 2049  al.            I
-00015ac0: 7420 6973 2064 6573 6372 6962 6564 2077  t is described w
-00015ad0: 6869 6368 2070 6172 616d 6574 6572 7320  hich parameters 
-00015ae0: 6172 6520 7772 6974 7465 6e20 6f75 742e  are written out.
-00015af0: 204f 6e6c 790a 2020 2020 2020 2020 2020   Only.          
-00015b00: 2020 7468 6520 7365 7474 696e 6773 2065    the settings e
-00015b10: 7870 6563 7465 6420 746f 2062 6520 7570  xpected to be up
-00015b20: 6461 7465 6420 6672 6f6d 2074 6865 2066  dated from the f
-00015b30: 6f6c 6c6f 7769 6e67 0a20 2020 2020 2020  ollowing.       
-00015b40: 2020 2020 2064 6566 6175 6c74 2073 6574       default set
-00015b50: 7469 6e67 7320 6172 6520 6e65 6564 6564  tings are needed
-00015b60: 2074 6f20 6265 2073 6574 2069 6e20 7468   to be set in th
-00015b70: 6520 6469 6374 696f 6e61 7279 2e0a 2020  e dictionary..  
-00015b80: 2020 2020 2020 2020 2020 5468 6520 706f            The po
-00015b90: 7373 6962 6c65 2070 6172 616d 6574 6572  ssible parameter
-00015ba0: 7320 616e 6420 7468 6569 7220 6465 6661  s and their defa
-00015bb0: 756c 7420 7365 7474 696e 6773 2061 7265  ult settings are
-00015bc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00015bd0: 2020 7b27 666f 7263 655f 7365 7473 273a    {'force_sets':
-00015be0: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
-00015bf0: 2020 2020 2020 2020 2027 6469 7370 6c61           'displa
-00015c00: 6365 6d65 6e74 7327 3a20 5472 7565 2c0a  cements': True,.
-00015c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015c20: 2027 666f 7263 655f 636f 6e73 7461 6e74   'force_constant
-00015c30: 7327 3a20 4661 6c73 652c 0a20 2020 2020  s': False,.     
-00015c40: 2020 2020 2020 2020 2020 2020 2762 6f72              'bor
-00015c50: 6e5f 6566 6665 6374 6976 655f 6368 6172  n_effective_char
-00015c60: 6765 273a 2054 7275 652c 0a20 2020 2020  ge': True,.     
-00015c70: 2020 2020 2020 2020 2020 2020 2764 6965              'die
-00015c80: 6c65 6374 7269 635f 636f 6e73 7461 6e74  lectric_constant
-00015c90: 273a 2054 7275 657d 0a0a 2020 2020 2020  ': True}..      
-00015ca0: 2020 2222 220a 2020 2020 2020 2020 7068    """.        ph
-00015cb0: 3370 795f 7961 6d6c 203d 2050 686f 6e6f  3py_yaml = Phono
-00015cc0: 3370 7959 616d 6c28 7365 7474 696e 6773  3pyYaml(settings
-00015cd0: 3d73 6574 7469 6e67 7329 0a20 2020 2020  =settings).     
-00015ce0: 2020 2070 6833 7079 5f79 616d 6c2e 7365     ph3py_yaml.se
-00015cf0: 745f 7068 6f6e 6f6e 5f69 6e66 6f28 7365  t_phonon_info(se
-00015d00: 6c66 290a 2020 2020 2020 2020 7769 7468  lf).        with
-00015d10: 206f 7065 6e28 6669 6c65 6e61 6d65 2c20   open(filename, 
-00015d20: 2277 2229 2061 7320 773a 0a20 2020 2020  "w") as w:.     
-00015d30: 2020 2020 2020 2077 2e77 7269 7465 2873         w.write(s
-00015d40: 7472 2870 6833 7079 5f79 616d 6c29 290a  tr(ph3py_yaml)).
-00015d50: 0a20 2020 2023 2323 2323 2323 2323 2323  .    ###########
-00015d60: 2323 2323 2323 2323 0a20 2020 2023 2070  ########.    # p
-00015d70: 7269 7661 7465 206d 6574 686f 6473 2023  rivate methods #
-00015d80: 0a20 2020 2023 2323 2323 2323 2323 2323  .    ###########
-00015d90: 2323 2323 2323 2323 0a20 2020 2064 6566  ########.    def
-00015da0: 205f 7365 6172 6368 5f73 796d 6d65 7472   _search_symmetr
-00015db0: 7928 7365 6c66 293a 0a20 2020 2020 2020  y(self):.       
-00015dc0: 2073 656c 662e 5f73 796d 6d65 7472 7920   self._symmetry 
-00015dd0: 3d20 5379 6d6d 6574 7279 2873 656c 662e  = Symmetry(self.
-00015de0: 5f73 7570 6572 6365 6c6c 2c20 7365 6c66  _supercell, self
-00015df0: 2e5f 7379 6d70 7265 632c 2073 656c 662e  ._symprec, self.
-00015e00: 5f69 735f 7379 6d6d 6574 7279 290a 0a20  _is_symmetry).. 
-00015e10: 2020 2064 6566 205f 7365 6172 6368 5f70     def _search_p
-00015e20: 7269 6d69 7469 7665 5f73 796d 6d65 7472  rimitive_symmetr
-00015e30: 7928 7365 6c66 293a 0a20 2020 2020 2020  y(self):.       
-00015e40: 2073 656c 662e 5f70 7269 6d69 7469 7665   self._primitive
-00015e50: 5f73 796d 6d65 7472 7920 3d20 5379 6d6d  _symmetry = Symm
-00015e60: 6574 7279 280a 2020 2020 2020 2020 2020  etry(.          
-00015e70: 2020 7365 6c66 2e5f 7072 696d 6974 6976    self._primitiv
-00015e80: 652c 2073 656c 662e 5f73 796d 7072 6563  e, self._symprec
-00015e90: 2c20 7365 6c66 2e5f 6973 5f73 796d 6d65  , self._is_symme
-00015ea0: 7472 790a 2020 2020 2020 2020 290a 2020  try.        ).  
-00015eb0: 2020 2020 2020 6966 206c 656e 2873 656c        if len(sel
-00015ec0: 662e 5f73 796d 6d65 7472 792e 706f 696e  f._symmetry.poin
-00015ed0: 7467 726f 7570 5f6f 7065 7261 7469 6f6e  tgroup_operation
-00015ee0: 7329 2021 3d20 6c65 6e28 0a20 2020 2020  s) != len(.     
-00015ef0: 2020 2020 2020 2073 656c 662e 5f70 7269         self._pri
-00015f00: 6d69 7469 7665 5f73 796d 6d65 7472 792e  mitive_symmetry.
-00015f10: 706f 696e 7467 726f 7570 5f6f 7065 7261  pointgroup_opera
-00015f20: 7469 6f6e 730a 2020 2020 2020 2020 293a  tions.        ):
-00015f30: 2020 2320 6e6f 7161 2045 3132 390a 2020    # noqa E129.  
-00015f40: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00015f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015f60: 2022 5761 726e 696e 673a 2070 6f69 6e74   "Warning: point
-00015f70: 2067 726f 7570 2073 796d 6d65 7472 6965   group symmetrie
-00015f80: 7320 6f66 2073 7570 6572 6365 6c6c 2061  s of supercell a
-00015f90: 6e64 2070 7269 6d69 7469 7665 220a 2020  nd primitive".  
-00015fa0: 2020 2020 2020 2020 2020 2020 2020 2263                "c
-00015fb0: 656c 6c20 6172 6520 6469 6666 6572 656e  ell are differen
-00015fc0: 742e 220a 2020 2020 2020 2020 2020 2020  t.".            
-00015fd0: 290a 0a20 2020 2064 6566 205f 7365 6172  )..    def _sear
-00015fe0: 6368 5f70 686f 6e6f 6e5f 7375 7065 7263  ch_phonon_superc
-00015ff0: 656c 6c5f 7379 6d6d 6574 7279 2873 656c  ell_symmetry(sel
-00016000: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
-00016010: 656c 662e 5f70 686f 6e6f 6e5f 7375 7065  elf._phonon_supe
-00016020: 7263 656c 6c5f 6d61 7472 6978 2069 7320  rcell_matrix is 
-00016030: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00016040: 2020 7365 6c66 2e5f 7068 6f6e 6f6e 5f73    self._phonon_s
-00016050: 7570 6572 6365 6c6c 5f73 796d 6d65 7472  upercell_symmetr
-00016060: 7920 3d20 7365 6c66 2e5f 7379 6d6d 6574  y = self._symmet
-00016070: 7279 0a20 2020 2020 2020 2065 6c73 653a  ry.        else:
-00016080: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00016090: 662e 5f70 686f 6e6f 6e5f 7375 7065 7263  f._phonon_superc
-000160a0: 656c 6c5f 7379 6d6d 6574 7279 203d 2053  ell_symmetry = S
-000160b0: 796d 6d65 7472 7928 0a20 2020 2020 2020  ymmetry(.       
-000160c0: 2020 2020 2020 2020 2073 656c 662e 5f70           self._p
-000160d0: 686f 6e6f 6e5f 7375 7065 7263 656c 6c2c  honon_supercell,
-000160e0: 2073 656c 662e 5f73 796d 7072 6563 2c20   self._symprec, 
-000160f0: 7365 6c66 2e5f 6973 5f73 796d 6d65 7472  self._is_symmetr
-00016100: 790a 2020 2020 2020 2020 2020 2020 290a  y.            ).
-00016110: 0a20 2020 2064 6566 205f 6275 696c 645f  .    def _build_
-00016120: 7375 7065 7263 656c 6c28 7365 6c66 293a  supercell(self):
-00016130: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
-00016140: 7570 6572 6365 6c6c 203d 2067 6574 5f73  upercell = get_s
-00016150: 7570 6572 6365 6c6c 280a 2020 2020 2020  upercell(.      
-00016160: 2020 2020 2020 7365 6c66 2e5f 756e 6974        self._unit
-00016170: 6365 6c6c 2c20 7365 6c66 2e5f 7375 7065  cell, self._supe
-00016180: 7263 656c 6c5f 6d61 7472 6978 2c20 7365  rcell_matrix, se
-00016190: 6c66 2e5f 7379 6d70 7265 630a 2020 2020  lf._symprec.    
-000161a0: 2020 2020 290a 0a20 2020 2064 6566 205f      )..    def _
-000161b0: 6275 696c 645f 7072 696d 6974 6976 655f  build_primitive_
-000161c0: 6365 6c6c 2873 656c 6629 3a0a 2020 2020  cell(self):.    
-000161d0: 2020 2020 2222 2243 7265 6174 6520 7072      """Create pr
-000161e0: 696d 6974 6976 6520 6365 6c6c 2e0a 0a20  imitive cell... 
-000161f0: 2020 2020 2020 2070 7269 6d69 7469 7665         primitive
-00016200: 5f6d 6174 7269 783a 0a20 2020 2020 2020  _matrix:.       
-00016210: 2020 2052 656c 6174 6976 6520 6178 6573     Relative axes
-00016220: 206f 6620 7072 696d 6974 6976 6520 6365   of primitive ce
-00016230: 6c6c 2074 6f20 7468 6520 696e 7075 7420  ll to the input 
-00016240: 756e 6974 2063 656c 6c2e 0a20 2020 2020  unit cell..     
-00016250: 2020 2020 2052 656c 6174 6976 6520 6178       Relative ax
-00016260: 6573 2074 6f20 7468 6520 7375 7065 7263  es to the superc
-00016270: 656c 6c20 6973 2063 616c 6375 6c61 7465  ell is calculate
-00016280: 6420 6279 3a0a 2020 2020 2020 2020 2020  d by:.          
-00016290: 2020 2073 7570 6572 6365 6c6c 5f6d 6174     supercell_mat
-000162a0: 7269 785e 2d31 202a 2070 7269 6d69 7469  rix^-1 * primiti
-000162b0: 7665 5f6d 6174 7269 780a 2020 2020 2020  ve_matrix.      
-000162c0: 2020 2020 5468 6572 6566 6f72 6520 7072      Therefore pr
-000162d0: 696d 6974 6976 6520 6365 6c6c 206c 6174  imitive cell lat
-000162e0: 7469 6365 2069 7320 6669 6e61 6c6c 7920  tice is finally 
-000162f0: 6361 6c63 756c 6174 6564 2062 793a 0a20  calculated by:. 
-00016300: 2020 2020 2020 2020 2020 2020 2873 7570              (sup
-00016310: 6572 6365 6c6c 5f6c 6174 7469 6365 202a  ercell_lattice *
-00016320: 2028 7375 7065 7263 656c 6c5f 6d61 7472   (supercell_matr
-00016330: 6978 295e 2d31 202a 2070 7269 6d69 7469  ix)^-1 * primiti
-00016340: 7665 5f6d 6174 7269 7829 5e54 0a0a 2020  ve_matrix)^T..  
-00016350: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00016360: 2020 7365 6c66 2e5f 7072 696d 6974 6976    self._primitiv
-00016370: 6520 3d20 7365 6c66 2e5f 6765 745f 7072  e = self._get_pr
-00016380: 696d 6974 6976 655f 6365 6c6c 280a 2020  imitive_cell(.  
-00016390: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000163a0: 7375 7065 7263 656c 6c2c 2073 656c 662e  supercell, self.
-000163b0: 5f73 7570 6572 6365 6c6c 5f6d 6174 7269  _supercell_matri
-000163c0: 782c 2073 656c 662e 5f70 7269 6d69 7469  x, self._primiti
-000163d0: 7665 5f6d 6174 7269 780a 2020 2020 2020  ve_matrix.      
-000163e0: 2020 290a 0a20 2020 2064 6566 205f 6275    )..    def _bu
-000163f0: 696c 645f 7068 6f6e 6f6e 5f73 7570 6572  ild_phonon_super
-00016400: 6365 6c6c 2873 656c 6629 3a0a 2020 2020  cell(self):.    
-00016410: 2020 2020 2222 2243 7265 6174 6520 7068      """Create ph
-00016420: 6f6e 6f6e 2073 7570 6572 6365 6c6c 2066  onon supercell f
-00016430: 6f72 2066 6332 2e0a 0a20 2020 2020 2020  or fc2...       
-00016440: 2070 686f 6e6f 6e5f 7375 7065 7263 656c   phonon_supercel
-00016450: 6c3a 0a20 2020 2020 2020 2020 2054 6869  l:.          Thi
-00016460: 7320 7375 7065 7263 656c 6c20 6973 2075  s supercell is u
-00016470: 7365 6420 666f 7220 6861 726d 6f6e 6963  sed for harmonic
-00016480: 2070 686f 6e6f 6e73 2028 6672 6571 7565   phonons (freque
-00016490: 6e63 6965 732c 0a20 2020 2020 2020 2020  ncies,.         
-000164a0: 2065 6967 656e 7665 6374 6f72 732c 2067   eigenvectors, g
-000164b0: 726f 7570 2076 656c 6f63 6974 6965 732c  roup velocities,
-000164c0: 202e 2e2e 290a 2020 2020 2020 2020 7068   ...).        ph
-000164d0: 6f6e 6f6e 5f73 7570 6572 6365 6c6c 5f6d  onon_supercell_m
-000164e0: 6174 7269 783a 0a20 2020 2020 2020 2020  atrix:.         
-000164f0: 2044 6966 6665 7265 6e74 2073 7570 6572   Different super
-00016500: 6365 6c6c 2073 697a 6520 6361 6e20 6265  cell size can be
-00016510: 2073 7065 6369 6669 6564 2e0a 0a20 2020   specified...   
-00016520: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00016530: 2069 6620 7365 6c66 2e5f 7068 6f6e 6f6e   if self._phonon
-00016540: 5f73 7570 6572 6365 6c6c 5f6d 6174 7269  _supercell_matri
-00016550: 7820 6973 204e 6f6e 653a 0a20 2020 2020  x is None:.     
-00016560: 2020 2020 2020 2073 656c 662e 5f70 686f         self._pho
-00016570: 6e6f 6e5f 7375 7065 7263 656c 6c20 3d20  non_supercell = 
-00016580: 7365 6c66 2e5f 7375 7065 7263 656c 6c0a  self._supercell.
-00016590: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000165a0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000165b0: 7068 6f6e 6f6e 5f73 7570 6572 6365 6c6c  phonon_supercell
-000165c0: 203d 2067 6574 5f73 7570 6572 6365 6c6c   = get_supercell
-000165d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000165e0: 2020 7365 6c66 2e5f 756e 6974 6365 6c6c    self._unitcell
-000165f0: 2c20 7365 6c66 2e5f 7068 6f6e 6f6e 5f73  , self._phonon_s
-00016600: 7570 6572 6365 6c6c 5f6d 6174 7269 782c  upercell_matrix,
-00016610: 2073 656c 662e 5f73 796d 7072 6563 0a20   self._symprec. 
-00016620: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00016630: 2020 6465 6620 5f62 7569 6c64 5f70 686f    def _build_pho
-00016640: 6e6f 6e5f 7072 696d 6974 6976 655f 6365  non_primitive_ce
-00016650: 6c6c 2873 656c 6629 3a0a 2020 2020 2020  ll(self):.      
-00016660: 2020 6966 2073 656c 662e 5f70 686f 6e6f    if self._phono
-00016670: 6e5f 7375 7065 7263 656c 6c5f 6d61 7472  n_supercell_matr
-00016680: 6978 2069 7320 4e6f 6e65 3a0a 2020 2020  ix is None:.    
-00016690: 2020 2020 2020 2020 7365 6c66 2e5f 7068          self._ph
-000166a0: 6f6e 6f6e 5f70 7269 6d69 7469 7665 203d  onon_primitive =
-000166b0: 2073 656c 662e 5f70 7269 6d69 7469 7665   self._primitive
-000166c0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-000166d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000166e0: 5f70 686f 6e6f 6e5f 7072 696d 6974 6976  _phonon_primitiv
-000166f0: 6520 3d20 7365 6c66 2e5f 6765 745f 7072  e = self._get_pr
-00016700: 696d 6974 6976 655f 6365 6c6c 280a 2020  imitive_cell(.  
-00016710: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00016720: 6c66 2e5f 7068 6f6e 6f6e 5f73 7570 6572  lf._phonon_super
-00016730: 6365 6c6c 2c0a 2020 2020 2020 2020 2020  cell,.          
-00016740: 2020 2020 2020 7365 6c66 2e5f 7068 6f6e        self._phon
-00016750: 6f6e 5f73 7570 6572 6365 6c6c 5f6d 6174  on_supercell_mat
-00016760: 7269 782c 0a20 2020 2020 2020 2020 2020  rix,.           
-00016770: 2020 2020 2073 656c 662e 5f70 7269 6d69       self._primi
-00016780: 7469 7665 5f6d 6174 7269 782c 0a20 2020  tive_matrix,.   
-00016790: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-000167a0: 2020 2020 2020 2069 6620 280a 2020 2020         if (.    
-000167b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000167c0: 2e5f 7072 696d 6974 6976 6520 6973 206e  ._primitive is n
-000167d0: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
-000167e0: 2020 2020 2020 2020 616e 6420 2873 656c          and (sel
-000167f0: 662e 5f70 7269 6d69 7469 7665 2e6e 756d  f._primitive.num
-00016800: 6265 7273 2021 3d20 7365 6c66 2e5f 7068  bers != self._ph
-00016810: 6f6e 6f6e 5f70 7269 6d69 7469 7665 2e6e  onon_primitive.n
-00016820: 756d 6265 7273 292e 616e 7928 290a 2020  umbers).any().  
-00016830: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
-00016840: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00016850: 6e74 2822 2050 7269 6d69 7469 7665 2063  nt(" Primitive c
-00016860: 656c 6c73 2066 6f72 2066 6332 2061 6e64  ells for fc2 and
-00016870: 2066 6333 2063 616e 2062 6520 6469 6666   fc3 can be diff
-00016880: 6572 656e 742e 2229 0a20 2020 2020 2020  erent.").       
-00016890: 2020 2020 2020 2020 2072 6169 7365 2052           raise R
-000168a0: 756e 7469 6d65 4572 726f 720a 0a20 2020  untimeError..   
-000168b0: 2064 6566 205f 6275 696c 645f 7068 6f6e   def _build_phon
-000168c0: 6f6e 5f73 7570 6572 6365 6c6c 735f 7769  on_supercells_wi
-000168d0: 7468 5f64 6973 706c 6163 656d 656e 7473  th_displacements
-000168e0: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
-000168f0: 7375 7065 7263 656c 6c3a 2050 686f 6e6f  supercell: Phono
-00016900: 7079 4174 6f6d 732c 2064 6973 706c 6163  pyAtoms, displac
-00016910: 656d 656e 745f 6461 7461 7365 740a 2020  ement_dataset.  
-00016920: 2020 293a 0a20 2020 2020 2020 2073 7570    ):.        sup
-00016930: 6572 6365 6c6c 7320 3d20 5b5d 0a20 2020  ercells = [].   
-00016940: 2020 2020 206d 6167 6d6f 6d73 203d 2073       magmoms = s
-00016950: 7570 6572 6365 6c6c 2e6d 6167 6e65 7469  upercell.magneti
-00016960: 635f 6d6f 6d65 6e74 730a 2020 2020 2020  c_moments.      
-00016970: 2020 6d61 7373 6573 203d 2073 7570 6572    masses = super
-00016980: 6365 6c6c 2e6d 6173 7365 730a 2020 2020  cell.masses.    
-00016990: 2020 2020 6e75 6d62 6572 7320 3d20 7375      numbers = su
-000169a0: 7065 7263 656c 6c2e 6e75 6d62 6572 730a  percell.numbers.
-000169b0: 2020 2020 2020 2020 6c61 7474 6963 6520          lattice 
-000169c0: 3d20 7375 7065 7263 656c 6c2e 6365 6c6c  = supercell.cell
-000169d0: 0a0a 2020 2020 2020 2020 666f 7220 6469  ..        for di
-000169e0: 7370 3120 696e 2064 6973 706c 6163 656d  sp1 in displacem
-000169f0: 656e 745f 6461 7461 7365 745b 2266 6972  ent_dataset["fir
-00016a00: 7374 5f61 746f 6d73 225d 3a0a 2020 2020  st_atoms"]:.    
-00016a10: 2020 2020 2020 2020 6469 7370 5f63 6172          disp_car
-00016a20: 7431 203d 2064 6973 7031 5b22 6469 7370  t1 = disp1["disp
-00016a30: 6c61 6365 6d65 6e74 225d 0a20 2020 2020  lacement"].     
-00016a40: 2020 2020 2020 2070 6f73 6974 696f 6e73         positions
-00016a50: 203d 2073 7570 6572 6365 6c6c 2e70 6f73   = supercell.pos
-00016a60: 6974 696f 6e73 0a20 2020 2020 2020 2020  itions.         
-00016a70: 2020 2070 6f73 6974 696f 6e73 5b64 6973     positions[dis
-00016a80: 7031 5b22 6e75 6d62 6572 225d 5d20 2b3d  p1["number"]] +=
-00016a90: 2064 6973 705f 6361 7274 310a 2020 2020   disp_cart1.    
-00016aa0: 2020 2020 2020 2020 7375 7065 7263 656c          supercel
-00016ab0: 6c73 2e61 7070 656e 6428 0a20 2020 2020  ls.append(.     
-00016ac0: 2020 2020 2020 2020 2020 2050 686f 6e6f             Phono
-00016ad0: 7079 4174 6f6d 7328 0a20 2020 2020 2020  pyAtoms(.       
-00016ae0: 2020 2020 2020 2020 2020 2020 206e 756d               num
-00016af0: 6265 7273 3d6e 756d 6265 7273 2c0a 2020  bers=numbers,.  
-00016b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b10: 2020 6d61 7373 6573 3d6d 6173 7365 732c    masses=masses,
-00016b20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016b30: 2020 2020 206d 6167 6e65 7469 635f 6d6f       magnetic_mo
-00016b40: 6d65 6e74 733d 6d61 676d 6f6d 732c 0a20  ments=magmoms,. 
-00016b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b60: 2020 2070 6f73 6974 696f 6e73 3d70 6f73     positions=pos
-00016b70: 6974 696f 6e73 2c0a 2020 2020 2020 2020  itions,.        
-00016b80: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
-00016b90: 3d6c 6174 7469 6365 2c0a 2020 2020 2020  =lattice,.      
-00016ba0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00016bb0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00016bc0: 2020 2072 6574 7572 6e20 7375 7065 7263     return superc
-00016bd0: 656c 6c73 0a0a 2020 2020 6465 6620 5f62  ells..    def _b
-00016be0: 7569 6c64 5f73 7570 6572 6365 6c6c 735f  uild_supercells_
-00016bf0: 7769 7468 5f64 6973 706c 6163 656d 656e  with_displacemen
-00016c00: 7473 2873 656c 6629 3a0a 2020 2020 2020  ts(self):.      
-00016c10: 2020 7375 7065 7263 656c 6c73 203d 205b    supercells = [
-00016c20: 5d0a 2020 2020 2020 2020 6d61 676d 6f6d  ].        magmom
-00016c30: 7320 3d20 7365 6c66 2e5f 7375 7065 7263  s = self._superc
-00016c40: 656c 6c2e 6d61 676e 6574 6963 5f6d 6f6d  ell.magnetic_mom
-00016c50: 656e 7473 0a20 2020 2020 2020 206d 6173  ents.        mas
-00016c60: 7365 7320 3d20 7365 6c66 2e5f 7375 7065  ses = self._supe
-00016c70: 7263 656c 6c2e 6d61 7373 6573 0a20 2020  rcell.masses.   
-00016c80: 2020 2020 206e 756d 6265 7273 203d 2073       numbers = s
-00016c90: 656c 662e 5f73 7570 6572 6365 6c6c 2e6e  elf._supercell.n
-00016ca0: 756d 6265 7273 0a20 2020 2020 2020 206c  umbers.        l
-00016cb0: 6174 7469 6365 203d 2073 656c 662e 5f73  attice = self._s
-00016cc0: 7570 6572 6365 6c6c 2e63 656c 6c0a 0a20  upercell.cell.. 
-00016cd0: 2020 2020 2020 2073 7570 6572 6365 6c6c         supercell
-00016ce0: 7320 3d20 7365 6c66 2e5f 6275 696c 645f  s = self._build_
-00016cf0: 7068 6f6e 6f6e 5f73 7570 6572 6365 6c6c  phonon_supercell
-00016d00: 735f 7769 7468 5f64 6973 706c 6163 656d  s_with_displacem
-00016d10: 656e 7473 280a 2020 2020 2020 2020 2020  ents(.          
-00016d20: 2020 7365 6c66 2e5f 7375 7065 7263 656c    self._supercel
-00016d30: 6c2c 2073 656c 662e 5f64 6174 6173 6574  l, self._dataset
-00016d40: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00016d50: 2020 2020 666f 7220 6469 7370 3120 696e      for disp1 in
-00016d60: 2073 656c 662e 5f64 6174 6173 6574 5b22   self._dataset["
-00016d70: 6669 7273 745f 6174 6f6d 7322 5d3a 0a20  first_atoms"]:. 
-00016d80: 2020 2020 2020 2020 2020 2064 6973 705f             disp_
-00016d90: 6361 7274 3120 3d20 6469 7370 315b 2264  cart1 = disp1["d
-00016da0: 6973 706c 6163 656d 656e 7422 5d0a 2020  isplacement"].  
-00016db0: 2020 2020 2020 2020 2020 666f 7220 6469            for di
-00016dc0: 7370 3220 696e 2064 6973 7031 5b22 7365  sp2 in disp1["se
-00016dd0: 636f 6e64 5f61 746f 6d73 225d 3a0a 2020  cond_atoms"]:.  
-00016de0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00016df0: 2022 696e 636c 7564 6564 2220 696e 2064   "included" in d
-00016e00: 6973 7032 3a0a 2020 2020 2020 2020 2020  isp2:.          
-00016e10: 2020 2020 2020 2020 2020 696e 636c 7564            includ
-00016e20: 6564 203d 2064 6973 7032 5b22 696e 636c  ed = disp2["incl
-00016e30: 7564 6564 225d 0a20 2020 2020 2020 2020  uded"].         
-00016e40: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00016e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e60: 2069 6e63 6c75 6465 6420 3d20 5472 7565   included = True
-00016e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016e80: 2069 6620 696e 636c 7564 6564 3a0a 2020   if included:.  
-00016e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ea0: 2020 706f 7369 7469 6f6e 7320 3d20 7365    positions = se
-00016eb0: 6c66 2e5f 7375 7065 7263 656c 6c2e 706f  lf._supercell.po
-00016ec0: 7369 7469 6f6e 730a 2020 2020 2020 2020  sitions.        
-00016ed0: 2020 2020 2020 2020 2020 2020 706f 7369              posi
-00016ee0: 7469 6f6e 735b 6469 7370 315b 226e 756d  tions[disp1["num
-00016ef0: 6265 7222 5d5d 202b 3d20 6469 7370 5f63  ber"]] += disp_c
-00016f00: 6172 7431 0a20 2020 2020 2020 2020 2020  art1.           
-00016f10: 2020 2020 2020 2020 2070 6f73 6974 696f           positio
-00016f20: 6e73 5b64 6973 7032 5b22 6e75 6d62 6572  ns[disp2["number
-00016f30: 225d 5d20 2b3d 2064 6973 7032 5b22 6469  "]] += disp2["di
-00016f40: 7370 6c61 6365 6d65 6e74 225d 0a20 2020  splacement"].   
-00016f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f60: 2073 7570 6572 6365 6c6c 732e 6170 7065   supercells.appe
-00016f70: 6e64 280a 2020 2020 2020 2020 2020 2020  nd(.            
-00016f80: 2020 2020 2020 2020 2020 2020 5068 6f6e              Phon
-00016f90: 6f70 7941 746f 6d73 280a 2020 2020 2020  opyAtoms(.      
-00016fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016fb0: 2020 2020 2020 6e75 6d62 6572 733d 6e75        numbers=nu
-00016fc0: 6d62 6572 732c 0a20 2020 2020 2020 2020  mbers,.         
-00016fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016fe0: 2020 206d 6173 7365 733d 6d61 7373 6573     masses=masses
-00016ff0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00017000: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-00017010: 676e 6574 6963 5f6d 6f6d 656e 7473 3d6d  gnetic_moments=m
-00017020: 6167 6d6f 6d73 2c0a 2020 2020 2020 2020  agmoms,.        
-00017030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017040: 2020 2020 706f 7369 7469 6f6e 733d 706f      positions=po
-00017050: 7369 7469 6f6e 732c 0a20 2020 2020 2020  sitions,.       
-00017060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017070: 2020 2020 2063 656c 6c3d 6c61 7474 6963       cell=lattic
-00017080: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00017090: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-000170a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170b0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-000170c0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000170d0: 2020 2020 2020 2020 2020 2020 2073 7570               sup
-000170e0: 6572 6365 6c6c 732e 6170 7065 6e64 284e  ercells.append(N
-000170f0: 6f6e 6529 0a0a 2020 2020 2020 2020 7365  one)..        se
-00017100: 6c66 2e5f 7375 7065 7263 656c 6c73 5f77  lf._supercells_w
-00017110: 6974 685f 6469 7370 6c61 6365 6d65 6e74  ith_displacement
-00017120: 7320 3d20 7375 7065 7263 656c 6c73 0a0a  s = supercells..
-00017130: 2020 2020 6465 6620 5f67 6574 5f70 7269      def _get_pri
-00017140: 6d69 7469 7665 5f63 656c 6c28 7365 6c66  mitive_cell(self
-00017150: 2c20 7375 7065 7263 656c 6c2c 2073 7570  , supercell, sup
-00017160: 6572 6365 6c6c 5f6d 6174 7269 782c 2070  ercell_matrix, p
-00017170: 7269 6d69 7469 7665 5f6d 6174 7269 7829  rimitive_matrix)
-00017180: 3a0a 2020 2020 2020 2020 696e 765f 7375  :.        inv_su
-00017190: 7065 7263 656c 6c5f 6d61 7472 6978 203d  percell_matrix =
-000171a0: 206e 702e 6c69 6e61 6c67 2e69 6e76 2873   np.linalg.inv(s
-000171b0: 7570 6572 6365 6c6c 5f6d 6174 7269 7829  upercell_matrix)
-000171c0: 0a20 2020 2020 2020 2069 6620 7072 696d  .        if prim
-000171d0: 6974 6976 655f 6d61 7472 6978 2069 7320  itive_matrix is 
-000171e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000171f0: 2020 745f 6d61 7420 3d20 696e 765f 7375    t_mat = inv_su
-00017200: 7065 7263 656c 6c5f 6d61 7472 6978 0a20  percell_matrix. 
-00017210: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00017220: 2020 2020 2020 2020 2074 5f6d 6174 203d           t_mat =
-00017230: 206e 702e 646f 7428 696e 765f 7375 7065   np.dot(inv_supe
-00017240: 7263 656c 6c5f 6d61 7472 6978 2c20 7072  rcell_matrix, pr
-00017250: 696d 6974 6976 655f 6d61 7472 6978 290a  imitive_matrix).
-00017260: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00017270: 6765 745f 7072 696d 6974 6976 6528 7375  get_primitive(su
-00017280: 7065 7263 656c 6c2c 2074 5f6d 6174 2c20  percell, t_mat, 
-00017290: 7365 6c66 2e5f 7379 6d70 7265 632c 2073  self._symprec, s
-000172a0: 746f 7265 5f64 656e 7365 5f73 7665 6373  tore_dense_svecs
-000172b0: 3d54 7275 6529 0a0a 2020 2020 6465 6620  =True)..    def 
-000172c0: 5f64 6574 6572 6d69 6e65 5f70 7269 6d69  _determine_primi
-000172d0: 7469 7665 5f6d 6174 7269 7828 7365 6c66  tive_matrix(self
-000172e0: 2c20 7072 696d 6974 6976 655f 6d61 7472  , primitive_matr
-000172f0: 6978 293a 0a20 2020 2020 2020 2070 6d61  ix):.        pma
-00017300: 7420 3d20 6765 745f 7072 696d 6974 6976  t = get_primitiv
-00017310: 655f 6d61 7472 6978 2870 7269 6d69 7469  e_matrix(primiti
-00017320: 7665 5f6d 6174 7269 782c 2073 796d 7072  ve_matrix, sympr
-00017330: 6563 3d73 656c 662e 5f73 796d 7072 6563  ec=self._symprec
-00017340: 290a 2020 2020 2020 2020 6966 2069 7369  ).        if isi
-00017350: 6e73 7461 6e63 6528 706d 6174 2c20 7374  nstance(pmat, st
-00017360: 7229 2061 6e64 2070 6d61 7420 3d3d 2022  r) and pmat == "
-00017370: 6175 746f 223a 0a20 2020 2020 2020 2020  auto":.         
-00017380: 2020 2072 6574 7572 6e20 6775 6573 735f     return guess_
-00017390: 7072 696d 6974 6976 655f 6d61 7472 6978  primitive_matrix
-000173a0: 2873 656c 662e 5f75 6e69 7463 656c 6c2c  (self._unitcell,
-000173b0: 2073 796d 7072 6563 3d73 656c 662e 5f73   symprec=self._s
-000173c0: 796d 7072 6563 290a 2020 2020 2020 2020  ymprec).        
-000173d0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000173e0: 2020 7265 7475 726e 2070 6d61 740a 0a20    return pmat.. 
-000173f0: 2020 2064 6566 205f 7365 745f 6d65 7368     def _set_mesh
-00017400: 5f6e 756d 6265 7273 280a 2020 2020 2020  _numbers(.      
-00017410: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00017420: 6d65 7368 3a20 556e 696f 6e5b 696e 742c  mesh: Union[int,
-00017430: 2066 6c6f 6174 2c20 5365 7175 656e 6365   float, Sequence
-00017440: 2c20 6e70 2e6e 6461 7272 6179 5d2c 0a20  , np.ndarray],. 
-00017450: 2020 2029 3a0a 2020 2020 2020 2020 2320     ):.        # 
-00017460: 696e 6974 6961 6c69 7a61 7469 6f6e 2072  initialization r
-00017470: 656c 6174 6564 2074 6f20 6d65 7368 0a20  elated to mesh. 
-00017480: 2020 2020 2020 2073 656c 662e 5f69 6e74         self._int
-00017490: 6572 6163 7469 6f6e 203d 204e 6f6e 650a  eraction = None.
-000174a0: 0a20 2020 2020 2020 2073 656c 662e 5f62  .        self._b
-000174b0: 7a5f 6772 6964 203d 2042 5a47 7269 6428  z_grid = BZGrid(
-000174c0: 0a20 2020 2020 2020 2020 2020 206d 6573  .            mes
-000174d0: 682c 0a20 2020 2020 2020 2020 2020 206c  h,.            l
-000174e0: 6174 7469 6365 3d73 656c 662e 5f70 7269  attice=self._pri
-000174f0: 6d69 7469 7665 2e63 656c 6c2c 0a20 2020  mitive.cell,.   
-00017500: 2020 2020 2020 2020 2073 796d 6d65 7472           symmetr
-00017510: 795f 6461 7461 7365 743d 7365 6c66 2e5f  y_dataset=self._
-00017520: 7072 696d 6974 6976 655f 7379 6d6d 6574  primitive_symmet
-00017530: 7279 2e64 6174 6173 6574 2c0a 2020 2020  ry.dataset,.    
-00017540: 2020 2020 2020 2020 6973 5f74 696d 655f          is_time_
-00017550: 7265 7665 7273 616c 3d73 656c 662e 5f69  reversal=self._i
-00017560: 735f 7379 6d6d 6574 7279 2c0a 2020 2020  s_symmetry,.    
-00017570: 2020 2020 2020 2020 7573 655f 6772 673d          use_grg=
-00017580: 7365 6c66 2e5f 7573 655f 6772 672c 0a20  self._use_grg,. 
-00017590: 2020 2020 2020 2020 2020 2066 6f72 6365             force
-000175a0: 5f53 4e46 3d46 616c 7365 2c0a 2020 2020  _SNF=False,.    
-000175b0: 2020 2020 2020 2020 534e 465f 636f 6f72          SNF_coor
-000175c0: 6469 6e61 7465 733d 7365 6c66 2e5f 534e  dinates=self._SN
-000175d0: 465f 636f 6f72 6469 6e61 7465 732c 0a20  F_coordinates,. 
-000175e0: 2020 2020 2020 2020 2020 2073 746f 7265             store
-000175f0: 5f64 656e 7365 5f67 705f 6d61 703d 5472  _dense_gp_map=Tr
-00017600: 7565 2c0a 2020 2020 2020 2020 290a 0a20  ue,.        ).. 
-00017610: 2020 2064 6566 205f 696e 6974 5f64 796e     def _init_dyn
-00017620: 616d 6963 616c 5f6d 6174 7269 7828 7365  amical_matrix(se
-00017630: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
-00017640: 7365 6c66 2e5f 696e 7465 7261 6374 696f  self._interactio
-00017650: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
-00017660: 2020 2020 2020 206d 7367 203d 2028 0a20         msg = (. 
-00017670: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00017680: 5068 6f6e 6f33 7079 2e69 6e69 745f 7068  Phono3py.init_ph
-00017690: 7068 5f69 6e74 6572 6163 7469 6f6e 2068  ph_interaction h
-000176a0: 6173 2074 6f20 6265 2063 616c 6c65 6420  as to be called 
-000176b0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000176c0: 2020 2262 6566 6f72 6520 7275 6e6e 696e    "before runnin
-000176d0: 6720 7468 6973 206d 6574 686f 642e 220a  g this method.".
-000176e0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000176f0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00017700: 5275 6e74 696d 6545 7272 6f72 286d 7367  RuntimeError(msg
-00017710: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00017720: 5f69 6e74 6572 6163 7469 6f6e 2e69 6e69  _interaction.ini
-00017730: 745f 6479 6e61 6d69 6361 6c5f 6d61 7472  t_dynamical_matr
-00017740: 6978 280a 2020 2020 2020 2020 2020 2020  ix(.            
-00017750: 7365 6c66 2e5f 6663 322c 0a20 2020 2020  self._fc2,.     
-00017760: 2020 2020 2020 2073 656c 662e 5f70 686f         self._pho
-00017770: 6e6f 6e5f 7375 7065 7263 656c 6c2c 0a20  non_supercell,. 
-00017780: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00017790: 5f70 686f 6e6f 6e5f 7072 696d 6974 6976  _phonon_primitiv
-000177a0: 652c 0a20 2020 2020 2020 2020 2020 206e  e,.            n
-000177b0: 6163 5f70 6172 616d 733d 7365 6c66 2e5f  ac_params=self._
-000177c0: 6e61 635f 7061 7261 6d73 2c0a 2020 2020  nac_params,.    
-000177d0: 2020 2020 290a 2020 2020 2020 2020 6672      ).        fr
-000177e0: 6571 732c 205f 2c20 5f20 3d20 7365 6c66  eqs, _, _ = self
-000177f0: 2e67 6574 5f70 686f 6e6f 6e5f 6461 7461  .get_phonon_data
-00017800: 2829 0a20 2020 2020 2020 2067 705f 4761  ().        gp_Ga
-00017810: 6d6d 6120 3d20 7365 6c66 2e5f 627a 5f67  mma = self._bz_g
-00017820: 7269 642e 6770 5f47 616d 6d61 0a20 2020  rid.gp_Gamma.   
-00017830: 2020 2020 2069 6620 6e70 2e73 756d 2866       if np.sum(f
-00017840: 7265 7173 5b67 705f 4761 6d6d 615d 203c  reqs[gp_Gamma] <
-00017850: 2073 656c 662e 5f63 7574 6f66 665f 6672   self._cutoff_fr
-00017860: 6571 7565 6e63 7929 203c 2033 3a0a 2020  equency) < 3:.  
-00017870: 2020 2020 2020 2020 2020 666f 7220 692c            for i,
-00017880: 2066 2069 6e20 656e 756d 6572 6174 6528   f in enumerate(
-00017890: 6672 6571 735b 6770 5f47 616d 6d61 2c20  freqs[gp_Gamma, 
-000178a0: 3a33 5d29 3a0a 2020 2020 2020 2020 2020  :3]):.          
-000178b0: 2020 2020 2020 6966 206e 6f74 2028 6620        if not (f 
-000178c0: 3c20 7365 6c66 2e5f 6375 746f 6666 5f66  < self._cutoff_f
-000178d0: 7265 7175 656e 6379 293a 0a20 2020 2020  requency):.     
-000178e0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000178f0: 7265 7173 5b67 705f 4761 6d6d 612c 2069  reqs[gp_Gamma, i
-00017900: 5d20 3d20 300a 2020 2020 2020 2020 2020  ] = 0.          
-00017910: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00017920: 223d 2220 2a20 3236 202b 2022 2057 6172  "=" * 26 + " War
-00017930: 6e69 6e67 2022 202b 2022 3d22 202a 2032  ning " + "=" * 2
-00017940: 3629 0a20 2020 2020 2020 2020 2020 2020  6).             
-00017950: 2020 2020 2020 2070 7269 6e74 280a 2020         print(.  
-00017960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017970: 2020 2020 2020 2220 5068 6f6e 6f6e 2066        " Phonon f
-00017980: 7265 7175 656e 6379 206f 6620 6261 6e64  requency of band
-00017990: 2069 6e64 6578 2025 6420 6174 2047 616d   index %d at Gam
-000179a0: 6d61 2022 0a20 2020 2020 2020 2020 2020  ma ".           
-000179b0: 2020 2020 2020 2020 2020 2020 2022 6973               "is
-000179c0: 2063 616c 6375 6c61 7465 6420 746f 2062   calculated to b
-000179d0: 6520 2566 2e22 2025 2028 6920 2b20 312c  e %f." % (i + 1,
-000179e0: 2066 290a 2020 2020 2020 2020 2020 2020   f).            
-000179f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00017a00: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00017a10: 696e 7428 2220 4275 7420 7468 6973 2066  int(" But this f
-00017a20: 7265 7175 656e 6379 2069 7320 666f 7263  requency is forc
-00017a30: 6564 2074 6f20 6265 207a 6572 6f2e 2229  ed to be zero.")
-00017a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017a50: 2020 2020 2070 7269 6e74 2822 3d22 202a       print("=" *
-00017a60: 2036 3129 0a0a 2020 2020 6465 6620 5f65   61)..    def _e
-00017a70: 7874 7261 6374 5f66 6332 5f66 6333 5f63  xtract_fc2_fc3_c
-00017a80: 616c 6375 6c61 746f 7273 2873 656c 662c  alculators(self,
-00017a90: 2066 635f 6361 6c63 756c 6174 6f72 2c20   fc_calculator, 
-00017aa0: 6663 5f63 616c 6375 6c61 746f 725f 6f70  fc_calculator_op
-00017ab0: 7469 6f6e 732c 206f 7264 6572 293a 0a20  tions, order):. 
-00017ac0: 2020 2020 2020 2022 2222 4578 7472 6163         """Extrac
-00017ad0: 7420 6663 5f63 616c 6375 6c61 746f 7220  t fc_calculator 
-00017ae0: 616e 6420 6663 5f63 616c 6375 6c61 746f  and fc_calculato
-00017af0: 725f 6f70 7469 6f6e 7320 666f 7220 6663  r_options for fc
-00017b00: 3220 616e 6420 6663 332e 0a0a 2020 2020  2 and fc3...    
-00017b10: 2020 2020 6663 5f63 616c 6375 6c61 746f      fc_calculato
-00017b20: 7220 3a20 7374 720a 2020 2020 2020 2020  r : str.        
-00017b30: 2020 2020 4643 2063 616c 6375 6c61 746f      FC calculato
-00017b40: 722e 2022 7c22 2073 6570 6172 6174 6573  r. "|" separates
-00017b50: 2066 6332 2061 6e64 2066 6333 2e20 4669   fc2 and fc3. Fi
-00017b60: 7273 7420 616e 6420 6c61 7374 0a20 2020  rst and last.   
-00017b70: 2020 2020 2020 2020 2070 6172 7473 2073           parts s
-00017b80: 6570 6172 6174 6564 2063 6f72 7265 7370  eparated corresp
-00017b90: 6f6e 6420 746f 2066 6332 2061 6e64 2066  ond to fc2 and f
-00017ba0: 6333 2063 616c 6375 6c61 746f 7273 2c20  c3 calculators, 
-00017bb0: 7265 7370 6563 7469 7665 6c79 2e0a 2020  respectively..  
-00017bc0: 2020 2020 2020 6663 5f63 616c 6375 6c61        fc_calcula
-00017bd0: 746f 725f 6f70 7469 6f6e 7320 3a20 7374  tor_options : st
-00017be0: 720a 2020 2020 2020 2020 2020 2020 4643  r.            FC
-00017bf0: 2063 616c 6375 6c61 746f 7220 6f70 7469   calculator opti
-00017c00: 6f6e 732e 2022 7c22 2073 6570 6172 6174  ons. "|" separat
-00017c10: 6573 2066 6332 2061 6e64 2066 6333 2e20  es fc2 and fc3. 
-00017c20: 4669 7273 7420 616e 6420 6c61 7374 0a20  First and last. 
-00017c30: 2020 2020 2020 2020 2020 2070 6172 7473             parts
-00017c40: 2073 6570 6172 6174 6564 2063 6f72 7265   separated corre
-00017c50: 7370 6f6e 6420 746f 2066 6332 2061 6e64  spond to fc2 and
-00017c60: 2066 6333 206f 7074 696f 6e73 2c20 7265   fc3 options, re
-00017c70: 7370 6563 7469 7665 6c79 2e0a 2020 2020  spectively..    
-00017c80: 2020 2020 6f72 6465 7220 3a20 696e 7420      order : int 
-00017c90: 3d20 3220 6f72 2033 0a20 2020 2020 2020  = 2 or 3.       
-00017ca0: 2020 2020 2032 2061 6e64 2033 2069 6e64       2 and 3 ind
-00017cb0: 6963 6174 6520 6663 3220 616e 6420 6663  icate fc2 and fc
-00017cc0: 332c 2072 6573 7065 6374 6976 656c 792e  3, respectively.
-00017cd0: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00017ce0: 2020 2020 2020 6966 2066 635f 6361 6c63        if fc_calc
-00017cf0: 756c 6174 6f72 2069 7320 6e6f 7420 4e6f  ulator is not No
-00017d00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00017d10: 6966 2022 7c22 2069 6e20 6663 5f63 616c  if "|" in fc_cal
-00017d20: 6375 6c61 746f 723a 0a20 2020 2020 2020  culator:.       
-00017d30: 2020 2020 2020 2020 205f 6663 5f63 616c           _fc_cal
-00017d40: 6375 6c61 746f 7220 3d20 6663 5f63 616c  culator = fc_cal
-00017d50: 6375 6c61 746f 722e 7370 6c69 7428 227c  culator.split("|
-00017d60: 2229 5b6f 7264 6572 202d 2032 5d0a 2020  ")[order - 2].  
-00017d70: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00017d80: 205f 6663 5f63 616c 6375 6c61 746f 7220   _fc_calculator 
-00017d90: 3d3d 2022 223a 0a20 2020 2020 2020 2020  == "":.         
-00017da0: 2020 2020 2020 2020 2020 205f 6663 5f63             _fc_c
-00017db0: 616c 6375 6c61 746f 7220 3d20 4e6f 6e65  alculator = None
-00017dc0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00017dd0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00017de0: 2020 205f 6663 5f63 616c 6375 6c61 746f     _fc_calculato
-00017df0: 7220 3d20 6663 5f63 616c 6375 6c61 746f  r = fc_calculato
-00017e00: 720a 2020 2020 2020 2020 656c 7365 3a0a  r.        else:.
-00017e10: 2020 2020 2020 2020 2020 2020 5f66 635f              _fc_
-00017e20: 6361 6c63 756c 6174 6f72 203d 204e 6f6e  calculator = Non
-00017e30: 650a 0a20 2020 2020 2020 2069 6620 6663  e..        if fc
-00017e40: 5f63 616c 6375 6c61 746f 725f 6f70 7469  _calculator_opti
-00017e50: 6f6e 7320 6973 206e 6f74 204e 6f6e 653a  ons is not None:
-00017e60: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00017e70: 227c 2220 696e 2066 635f 6361 6c63 756c  "|" in fc_calcul
-00017e80: 6174 6f72 5f6f 7074 696f 6e73 3a0a 2020  ator_options:.  
-00017e90: 2020 2020 2020 2020 2020 2020 2020 5f66                _f
-00017ea0: 635f 6361 6c63 756c 6174 6f72 5f6f 7074  c_calculator_opt
-00017eb0: 696f 6e73 203d 2066 635f 6361 6c63 756c  ions = fc_calcul
-00017ec0: 6174 6f72 5f6f 7074 696f 6e73 2e73 706c  ator_options.spl
-00017ed0: 6974 2822 7c22 295b 6f72 6465 7220 2d20  it("|")[order - 
-00017ee0: 325d 0a20 2020 2020 2020 2020 2020 2020  2].             
-00017ef0: 2020 2069 6620 5f66 635f 6361 6c63 756c     if _fc_calcul
-00017f00: 6174 6f72 5f6f 7074 696f 6e73 203d 3d20  ator_options == 
-00017f10: 2222 3a0a 2020 2020 2020 2020 2020 2020  "":.            
-00017f20: 2020 2020 2020 2020 5f66 635f 6361 6c63          _fc_calc
-00017f30: 756c 6174 6f72 5f6f 7074 696f 6e73 203d  ulator_options =
-00017f40: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-00017f50: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00017f60: 2020 2020 2020 2020 5f66 635f 6361 6c63          _fc_calc
-00017f70: 756c 6174 6f72 5f6f 7074 696f 6e73 203d  ulator_options =
-00017f80: 2066 635f 6361 6c63 756c 6174 6f72 5f6f   fc_calculator_o
-00017f90: 7074 696f 6e73 0a20 2020 2020 2020 2065  ptions.        e
-00017fa0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00017fb0: 205f 6663 5f63 616c 6375 6c61 746f 725f   _fc_calculator_
-00017fc0: 6f70 7469 6f6e 7320 3d20 4e6f 6e65 0a0a  options = None..
-00017fd0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00017fe0: 6663 5f63 616c 6375 6c61 746f 722c 205f  fc_calculator, _
-00017ff0: 6663 5f63 616c 6375 6c61 746f 725f 6f70  fc_calculator_op
-00018000: 7469 6f6e 730a                           tions.
+00000640: 4820 4441 4d41 4745 2e0a 0a66 726f 6d20  H DAMAGE...from 
+00000650: 636f 6c6c 6563 7469 6f6e 732e 6162 6320  collections.abc 
+00000660: 696d 706f 7274 2053 6571 7565 6e63 650a  import Sequence.
+00000670: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
+00000680: 7274 204f 7074 696f 6e61 6c2c 2055 6e69  rt Optional, Uni
+00000690: 6f6e 0a0a 696d 706f 7274 206e 756d 7079  on..import numpy
+000006a0: 2061 7320 6e70 0a66 726f 6d20 7068 6f6e   as np.from phon
+000006b0: 6f70 792e 6578 6365 7074 696f 6e20 696d  opy.exception im
+000006c0: 706f 7274 2046 6f72 6365 4361 6c63 756c  port ForceCalcul
+000006d0: 6174 6f72 5265 7175 6972 6564 4572 726f  atorRequiredErro
+000006e0: 720a 6672 6f6d 2070 686f 6e6f 7079 2e68  r.from phonopy.h
+000006f0: 6172 6d6f 6e69 632e 6469 7370 6c61 6365  armonic.displace
+00000700: 6d65 6e74 2069 6d70 6f72 7420 280a 2020  ment import (.  
+00000710: 2020 6469 7265 6374 696f 6e73 5f74 6f5f    directions_to_
+00000720: 6469 7370 6c61 6365 6d65 6e74 5f64 6174  displacement_dat
+00000730: 6173 6574 2c0a 2020 2020 6765 745f 6c65  aset,.    get_le
+00000740: 6173 745f 6469 7370 6c61 6365 6d65 6e74  ast_displacement
+00000750: 732c 0a29 0a66 726f 6d20 7068 6f6e 6f70  s,.).from phonop
+00000760: 792e 6861 726d 6f6e 6963 2e66 6f72 6365  y.harmonic.force
+00000770: 5f63 6f6e 7374 616e 7473 2069 6d70 6f72  _constants impor
+00000780: 7420 6765 745f 6663 3220 6173 2067 6574  t get_fc2 as get
+00000790: 5f70 686f 6e6f 7079 5f66 6332 0a66 726f  _phonopy_fc2.fro
+000007a0: 6d20 7068 6f6e 6f70 792e 6861 726d 6f6e  m phonopy.harmon
+000007b0: 6963 2e66 6f72 6365 5f63 6f6e 7374 616e  ic.force_constan
+000007c0: 7473 2069 6d70 6f72 7420 280a 2020 2020  ts import (.    
+000007d0: 7365 745f 7065 726d 7574 6174 696f 6e5f  set_permutation_
+000007e0: 7379 6d6d 6574 7279 2c0a 2020 2020 7365  symmetry,.    se
+000007f0: 745f 7472 616e 736c 6174 696f 6e61 6c5f  t_translational_
+00000800: 696e 7661 7269 616e 6365 2c0a 2020 2020  invariance,.    
+00000810: 7379 6d6d 6574 7269 7a65 5f63 6f6d 7061  symmetrize_compa
+00000820: 6374 5f66 6f72 6365 5f63 6f6e 7374 616e  ct_force_constan
+00000830: 7473 2c0a 2020 2020 7379 6d6d 6574 7269  ts,.    symmetri
+00000840: 7a65 5f66 6f72 6365 5f63 6f6e 7374 616e  ze_force_constan
+00000850: 7473 2c0a 290a 6672 6f6d 2070 686f 6e6f  ts,.).from phono
+00000860: 7079 2e69 6e74 6572 6661 6365 2e66 635f  py.interface.fc_
+00000870: 6361 6c63 756c 6174 6f72 2069 6d70 6f72  calculator impor
+00000880: 7420 6765 745f 6663 320a 6672 6f6d 2070  t get_fc2.from p
+00000890: 686f 6e6f 7079 2e73 7472 7563 7475 7265  honopy.structure
+000008a0: 2e61 746f 6d73 2069 6d70 6f72 7420 5068  .atoms import Ph
+000008b0: 6f6e 6f70 7941 746f 6d73 0a66 726f 6d20  onopyAtoms.from 
+000008c0: 7068 6f6e 6f70 792e 7374 7275 6374 7572  phonopy.structur
+000008d0: 652e 6365 6c6c 7320 696d 706f 7274 2028  e.cells import (
+000008e0: 0a20 2020 2050 7269 6d69 7469 7665 2c0a  .    Primitive,.
+000008f0: 2020 2020 5375 7065 7263 656c 6c2c 0a20      Supercell,. 
+00000900: 2020 2067 6574 5f70 7269 6d69 7469 7665     get_primitive
+00000910: 2c0a 2020 2020 6765 745f 7072 696d 6974  ,.    get_primit
+00000920: 6976 655f 6d61 7472 6978 2c0a 2020 2020  ive_matrix,.    
+00000930: 6765 745f 7375 7065 7263 656c 6c2c 0a20  get_supercell,. 
+00000940: 2020 2067 7565 7373 5f70 7269 6d69 7469     guess_primiti
+00000950: 7665 5f6d 6174 7269 782c 0a20 2020 2073  ve_matrix,.    s
+00000960: 6861 7065 5f73 7570 6572 6365 6c6c 5f6d  hape_supercell_m
+00000970: 6174 7269 782c 0a29 0a66 726f 6d20 7068  atrix,.).from ph
+00000980: 6f6e 6f70 792e 7374 7275 6374 7572 652e  onopy.structure.
+00000990: 6461 7461 7365 7420 696d 706f 7274 2067  dataset import g
+000009a0: 6574 5f64 6973 706c 6163 656d 656e 7473  et_displacements
+000009b0: 5f61 6e64 5f66 6f72 6365 730a 6672 6f6d  _and_forces.from
+000009c0: 2070 686f 6e6f 7079 2e73 7472 7563 7475   phonopy.structu
+000009d0: 7265 2e73 796d 6d65 7472 7920 696d 706f  re.symmetry impo
+000009e0: 7274 2053 796d 6d65 7472 790a 6672 6f6d  rt Symmetry.from
+000009f0: 2070 686f 6e6f 7079 2e75 6e69 7473 2069   phonopy.units i
+00000a00: 6d70 6f72 7420 5661 7370 546f 5448 7a0a  mport VaspToTHz.
+00000a10: 0a66 726f 6d20 7068 6f6e 6f33 7079 2e63  .from phono3py.c
+00000a20: 6f6e 6475 6374 6976 6974 792e 6469 7265  onductivity.dire
+00000a30: 6374 5f73 6f6c 7574 696f 6e20 696d 706f  ct_solution impo
+00000a40: 7274 2067 6574 5f74 6865 726d 616c 5f63  rt get_thermal_c
+00000a50: 6f6e 6475 6374 6976 6974 795f 4c42 5445  onductivity_LBTE
+00000a60: 0a66 726f 6d20 7068 6f6e 6f33 7079 2e63  .from phono3py.c
+00000a70: 6f6e 6475 6374 6976 6974 792e 7274 6120  onductivity.rta 
+00000a80: 696d 706f 7274 2067 6574 5f74 6865 726d  import get_therm
+00000a90: 616c 5f63 6f6e 6475 6374 6976 6974 795f  al_conductivity_
+00000aa0: 5254 410a 6672 6f6d 2070 686f 6e6f 3370  RTA.from phono3p
+00000ab0: 792e 696e 7465 7266 6163 652e 6663 5f63  y.interface.fc_c
+00000ac0: 616c 6375 6c61 746f 7220 696d 706f 7274  alculator import
+00000ad0: 2067 6574 5f66 6333 0a66 726f 6d20 7068   get_fc3.from ph
+00000ae0: 6f6e 6f33 7079 2e69 6e74 6572 6661 6365  ono3py.interface
+00000af0: 2e70 686f 6e6f 3370 795f 7961 6d6c 2069  .phono3py_yaml i
+00000b00: 6d70 6f72 7420 5068 6f6e 6f33 7079 5961  mport Phono3pyYa
+00000b10: 6d6c 0a66 726f 6d20 7068 6f6e 6f33 7079  ml.from phono3py
+00000b20: 2e70 686f 6e6f 6e33 2e64 6174 6173 6574  .phonon3.dataset
+00000b30: 2069 6d70 6f72 7420 6765 745f 6469 7370   import get_disp
+00000b40: 6c61 6365 6d65 6e74 735f 616e 645f 666f  lacements_and_fo
+00000b50: 7263 6573 5f66 6333 0a66 726f 6d20 7068  rces_fc3.from ph
+00000b60: 6f6e 6f33 7079 2e70 686f 6e6f 6e33 2e64  ono3py.phonon3.d
+00000b70: 6973 706c 6163 656d 656e 745f 6663 3320  isplacement_fc3 
+00000b80: 696d 706f 7274 2028 0a20 2020 2064 6972  import (.    dir
+00000b90: 6563 7469 6f6e 5f74 6f5f 6469 7370 6c61  ection_to_displa
+00000ba0: 6365 6d65 6e74 2c0a 2020 2020 6765 745f  cement,.    get_
+00000bb0: 7468 6972 645f 6f72 6465 725f 6469 7370  third_order_disp
+00000bc0: 6c61 6365 6d65 6e74 732c 0a29 0a66 726f  lacements,.).fro
+00000bd0: 6d20 7068 6f6e 6f33 7079 2e70 686f 6e6f  m phono3py.phono
+00000be0: 6e33 2e66 6333 2069 6d70 6f72 7420 6375  n3.fc3 import cu
+00000bf0: 746f 6666 5f66 6333 5f62 795f 7a65 726f  toff_fc3_by_zero
+00000c00: 0a66 726f 6d20 7068 6f6e 6f33 7079 2e70  .from phono3py.p
+00000c10: 686f 6e6f 6e33 2e66 6333 2069 6d70 6f72  honon3.fc3 impor
+00000c20: 7420 6765 745f 6663 3320 6173 2067 6574  t get_fc3 as get
+00000c30: 5f70 686f 6e6f 3370 795f 6663 330a 6672  _phono3py_fc3.fr
+00000c40: 6f6d 2070 686f 6e6f 3370 792e 7068 6f6e  om phono3py.phon
+00000c50: 6f6e 332e 6663 3320 696d 706f 7274 2028  on3.fc3 import (
+00000c60: 0a20 2020 2073 6574 5f70 6572 6d75 7461  .    set_permuta
+00000c70: 7469 6f6e 5f73 796d 6d65 7472 795f 636f  tion_symmetry_co
+00000c80: 6d70 6163 745f 6663 332c 0a20 2020 2073  mpact_fc3,.    s
+00000c90: 6574 5f70 6572 6d75 7461 7469 6f6e 5f73  et_permutation_s
+00000ca0: 796d 6d65 7472 795f 6663 332c 0a20 2020  ymmetry_fc3,.   
+00000cb0: 2073 6574 5f74 7261 6e73 6c61 7469 6f6e   set_translation
+00000cc0: 616c 5f69 6e76 6172 6961 6e63 655f 636f  al_invariance_co
+00000cd0: 6d70 6163 745f 6663 332c 0a20 2020 2073  mpact_fc3,.    s
+00000ce0: 6574 5f74 7261 6e73 6c61 7469 6f6e 616c  et_translational
+00000cf0: 5f69 6e76 6172 6961 6e63 655f 6663 332c  _invariance_fc3,
+00000d00: 0a29 0a66 726f 6d20 7068 6f6e 6f33 7079  .).from phono3py
+00000d10: 2e70 686f 6e6f 6e33 2e69 6d61 675f 7365  .phonon3.imag_se
+00000d20: 6c66 5f65 6e65 7267 7920 696d 706f 7274  lf_energy import
+00000d30: 2028 0a20 2020 2067 6574 5f69 6d61 675f   (.    get_imag_
+00000d40: 7365 6c66 5f65 6e65 7267 792c 0a20 2020  self_energy,.   
+00000d50: 2077 7269 7465 5f69 6d61 675f 7365 6c66   write_imag_self
+00000d60: 5f65 6e65 7267 792c 0a29 0a66 726f 6d20  _energy,.).from 
+00000d70: 7068 6f6e 6f33 7079 2e70 686f 6e6f 6e33  phono3py.phonon3
+00000d80: 2e69 6e74 6572 6163 7469 6f6e 2069 6d70  .interaction imp
+00000d90: 6f72 7420 496e 7465 7261 6374 696f 6e0a  ort Interaction.
+00000da0: 6672 6f6d 2070 686f 6e6f 3370 792e 7068  from phono3py.ph
+00000db0: 6f6e 6f6e 332e 7265 616c 5f73 656c 665f  onon3.real_self_
+00000dc0: 656e 6572 6779 2069 6d70 6f72 7420 280a  energy import (.
+00000dd0: 2020 2020 6765 745f 7265 616c 5f73 656c      get_real_sel
+00000de0: 665f 656e 6572 6779 2c0a 2020 2020 7772  f_energy,.    wr
+00000df0: 6974 655f 7265 616c 5f73 656c 665f 656e  ite_real_self_en
+00000e00: 6572 6779 2c0a 290a 6672 6f6d 2070 686f  ergy,.).from pho
+00000e10: 6e6f 3370 792e 7068 6f6e 6f6e 332e 7370  no3py.phonon3.sp
+00000e20: 6563 7472 616c 5f66 756e 6374 696f 6e20  ectral_function 
+00000e30: 696d 706f 7274 2072 756e 5f73 7065 6374  import run_spect
+00000e40: 7261 6c5f 6675 6e63 7469 6f6e 0a66 726f  ral_function.fro
+00000e50: 6d20 7068 6f6e 6f33 7079 2e70 686f 6e6f  m phono3py.phono
+00000e60: 6e2e 6772 6964 2069 6d70 6f72 7420 425a  n.grid import BZ
+00000e70: 4772 6964 0a66 726f 6d20 7068 6f6e 6f33  Grid.from phono3
+00000e80: 7079 2e76 6572 7369 6f6e 2069 6d70 6f72  py.version impor
+00000e90: 7420 5f5f 7665 7273 696f 6e5f 5f0a 0a0a  t __version__...
+00000ea0: 636c 6173 7320 5068 6f6e 6f33 7079 3a0a  class Phono3py:.
+00000eb0: 2020 2020 2222 2250 686f 6e6f 3370 7920      """Phono3py 
+00000ec0: 6d61 696e 2063 6c61 7373 2e0a 0a20 2020  main class...   
+00000ed0: 2041 7474 7269 6275 7465 730a 2020 2020   Attributes.    
+00000ee0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2076  ----------.    v
+00000ef0: 6572 7369 6f6e 0a20 2020 2063 616c 6375  ersion.    calcu
+00000f00: 6c61 746f 720a 2020 2020 6663 3320 3a20  lator.    fc3 : 
+00000f10: 6765 7474 6572 2061 6e64 2073 6574 7465  getter and sette
+00000f20: 720a 2020 2020 6663 3220 3a20 6765 7474  r.    fc2 : gett
+00000f30: 6572 2061 6e64 2073 6574 7465 720a 2020  er and setter.  
+00000f40: 2020 666f 7263 655f 636f 6e73 7461 6e74    force_constant
+00000f50: 730a 2020 2020 7369 676d 6120 3a20 6765  s.    sigma : ge
+00000f60: 7474 6572 2061 6e64 2073 6574 7465 720a  tter and setter.
+00000f70: 2020 2020 7369 676d 615f 6375 746f 6666      sigma_cutoff
+00000f80: 203a 2067 6574 7465 7220 616e 6420 7365   : getter and se
+00000f90: 7474 6572 0a20 2020 206e 6163 5f70 6172  tter.    nac_par
+00000fa0: 616d 7320 3a20 6765 7474 6572 2061 6e64  ams : getter and
+00000fb0: 2073 6574 7465 720a 2020 2020 6479 6e61   setter.    dyna
+00000fc0: 6d69 6361 6c5f 6d61 7472 6978 0a20 2020  mical_matrix.   
+00000fd0: 2070 7269 6d69 7469 7665 0a20 2020 2075   primitive.    u
+00000fe0: 6e69 7463 656c 6c0a 2020 2020 7375 7065  nitcell.    supe
+00000ff0: 7263 656c 6c0a 2020 2020 7068 6f6e 6f6e  rcell.    phonon
+00001000: 5f73 7570 6572 6365 6c6c 0a20 2020 2070  _supercell.    p
+00001010: 686f 6e6f 6e5f 7072 696d 6974 6976 650a  honon_primitive.
+00001020: 2020 2020 7379 6d6d 6574 7279 0a20 2020      symmetry.   
+00001030: 2070 7269 6d69 7469 7665 5f73 796d 6d65   primitive_symme
+00001040: 7472 790a 2020 2020 7068 6f6e 6f6e 5f73  try.    phonon_s
+00001050: 7570 6572 6365 6c6c 5f73 796d 6d65 7472  upercell_symmetr
+00001060: 790a 2020 2020 7375 7065 7263 656c 6c5f  y.    supercell_
+00001070: 6d61 7472 6978 0a20 2020 2070 686f 6e6f  matrix.    phono
+00001080: 6e5f 7375 7065 7263 656c 6c5f 6d61 7472  n_supercell_matr
+00001090: 6978 0a20 2020 2070 7269 6d69 7469 7665  ix.    primitive
+000010a0: 5f6d 6174 7269 780a 2020 2020 756e 6974  _matrix.    unit
+000010b0: 5f63 6f6e 7665 7273 696f 6e5f 6661 6374  _conversion_fact
+000010c0: 6f72 0a20 2020 2064 6174 6173 6574 203a  or.    dataset :
+000010d0: 2067 6574 7465 7220 616e 6420 7365 7474   getter and sett
+000010e0: 6572 0a20 2020 2070 686f 6e6f 6e5f 6461  er.    phonon_da
+000010f0: 7461 7365 7420 3a20 6765 7474 6572 2061  taset : getter a
+00001100: 6e64 2073 6574 7465 720a 2020 2020 6261  nd setter.    ba
+00001110: 6e64 5f69 6e64 6963 6573 203a 2067 6574  nd_indices : get
+00001120: 7465 7220 616e 6420 7365 7474 6572 0a20  ter and setter. 
+00001130: 2020 2070 686f 6e6f 6e5f 7375 7065 7263     phonon_superc
+00001140: 656c 6c73 5f77 6974 685f 6469 7370 6c61  ells_with_displa
+00001150: 6365 6d65 6e74 730a 2020 2020 7375 7065  cements.    supe
+00001160: 7263 656c 6c73 5f77 6974 685f 6469 7370  rcells_with_disp
+00001170: 6c61 6365 6d65 6e74 730a 2020 2020 6d65  lacements.    me
+00001180: 7368 5f6e 756d 6265 7273 203a 2067 6574  sh_numbers : get
+00001190: 7465 7220 616e 6420 7365 7474 6572 0a20  ter and setter. 
+000011a0: 2020 2074 6865 726d 616c 5f63 6f6e 6475     thermal_condu
+000011b0: 6374 6976 6974 790a 2020 2020 6469 7370  ctivity.    disp
+000011c0: 6c61 6365 6d65 6e74 7320 3a20 6765 7474  lacements : gett
+000011d0: 6572 2061 6e64 2073 6574 7465 720a 2020  er and setter.  
+000011e0: 2020 666f 7263 6573 203a 2067 6574 7465    forces : gette
+000011f0: 7220 616e 6420 7365 7474 6572 0a20 2020  r and setter.   
+00001200: 2070 686f 6e6f 6e5f 6469 7370 6c61 6365   phonon_displace
+00001210: 6d65 6e74 7320 3a20 6765 7474 6572 2061  ments : getter a
+00001220: 6e64 2073 6574 7465 720a 2020 2020 7068  nd setter.    ph
+00001230: 6f6e 6f6e 5f66 6f72 6365 7320 3a20 6765  onon_forces : ge
+00001240: 7474 6572 2061 6e64 2073 6574 7465 720a  tter and setter.
+00001250: 2020 2020 7068 7068 5f69 6e74 6572 6163      phph_interac
+00001260: 7469 6f6e 0a0a 2020 2020 2222 220a 0a20  tion..    """.. 
+00001270: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00001280: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00001290: 2020 2020 2020 2075 6e69 7463 656c 6c3a         unitcell:
+000012a0: 2050 686f 6e6f 7079 4174 6f6d 732c 0a20   PhonopyAtoms,. 
+000012b0: 2020 2020 2020 2073 7570 6572 6365 6c6c         supercell
+000012c0: 5f6d 6174 7269 783d 4e6f 6e65 2c0a 2020  _matrix=None,.  
+000012d0: 2020 2020 2020 7072 696d 6974 6976 655f        primitive_
+000012e0: 6d61 7472 6978 3d4e 6f6e 652c 0a20 2020  matrix=None,.   
+000012f0: 2020 2020 2070 686f 6e6f 6e5f 7375 7065       phonon_supe
+00001300: 7263 656c 6c5f 6d61 7472 6978 3d4e 6f6e  rcell_matrix=Non
+00001310: 652c 0a20 2020 2020 2020 2063 7574 6f66  e,.        cutof
+00001320: 665f 6672 6571 7565 6e63 793d 3165 2d34  f_frequency=1e-4
+00001330: 2c0a 2020 2020 2020 2020 6672 6571 7565  ,.        freque
+00001340: 6e63 795f 6661 6374 6f72 5f74 6f5f 5448  ncy_factor_to_TH
+00001350: 7a3d 5661 7370 546f 5448 7a2c 0a20 2020  z=VaspToTHz,.   
+00001360: 2020 2020 2069 735f 7379 6d6d 6574 7279       is_symmetry
+00001370: 3d54 7275 652c 0a20 2020 2020 2020 2069  =True,.        i
+00001380: 735f 6d65 7368 5f73 796d 6d65 7472 793d  s_mesh_symmetry=
+00001390: 5472 7565 2c0a 2020 2020 2020 2020 7573  True,.        us
+000013a0: 655f 6772 673d 4661 6c73 652c 0a20 2020  e_grg=False,.   
+000013b0: 2020 2020 2053 4e46 5f63 6f6f 7264 696e       SNF_coordin
+000013c0: 6174 6573 3d22 7265 6369 7072 6f63 616c  ates="reciprocal
+000013d0: 222c 0a20 2020 2020 2020 206d 616b 655f  ",.        make_
+000013e0: 7230 5f61 7665 7261 6765 3a20 626f 6f6c  r0_average: bool
+000013f0: 203d 2054 7275 652c 0a20 2020 2020 2020   = True,.       
+00001400: 2073 796d 7072 6563 3d31 652d 352c 0a20   symprec=1e-5,. 
+00001410: 2020 2020 2020 2063 616c 6375 6c61 746f         calculato
+00001420: 723a 204f 7074 696f 6e61 6c5b 7374 725d  r: Optional[str]
+00001430: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00001440: 206c 6f67 5f6c 6576 656c 3d30 2c0a 2020   log_level=0,.  
+00001450: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
+00001460: 496e 6974 206d 6574 686f 642e 0a0a 2020  Init method...  
+00001470: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00001480: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00001490: 2d2d 2d0a 2020 2020 2020 2020 756e 6974  ---.        unit
+000014a0: 6365 6c6c 203a 2050 686f 6e6f 7079 4174  cell : PhonopyAt
+000014b0: 6f6d 732c 206f 7074 696f 6e61 6c0a 2020  oms, optional.  
+000014c0: 2020 2020 2020 2020 2020 496e 7075 7420            Input 
+000014d0: 756e 6974 2063 656c 6c2e 0a20 2020 2020  unit cell..     
+000014e0: 2020 2073 7570 6572 6365 6c6c 5f6d 6174     supercell_mat
+000014f0: 7269 7820 3a20 6172 7261 795f 6c69 6b65  rix : array_like
+00001500: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+00001510: 2020 2020 2020 2053 7570 6572 6365 6c6c         Supercell
+00001520: 206d 6174 7269 7820 6d75 6c74 6970 6c69   matrix multipli
+00001530: 6564 2074 6f20 696e 7075 7420 6365 6c6c  ed to input cell
+00001540: 2062 6173 6973 2076 6563 746f 7273 2e20   basis vectors. 
+00001550: 7368 6170 653d 2833 2c20 290a 2020 2020  shape=(3, ).    
+00001560: 2020 2020 2020 2020 6f72 2028 332c 2033          or (3, 3
+00001570: 292c 2077 6865 7265 2074 6865 2066 6f72  ), where the for
+00001580: 6d65 7220 6973 2063 6f6e 7369 6465 7265  mer is considere
+00001590: 6420 6120 6469 6167 6f6e 616c 206d 6174  d a diagonal mat
+000015a0: 7269 782e 2054 6865 0a20 2020 2020 2020  rix. The.       
+000015b0: 2020 2020 2065 6c65 6d65 6e74 7320 6861       elements ha
+000015c0: 7665 2074 6f20 6265 2067 6976 656e 2062  ve to be given b
+000015d0: 7920 696e 7465 6765 7273 2e20 416c 7468  y integers. Alth
+000015e0: 6f75 6768 2074 6865 2064 6566 6175 6c74  ough the default
+000015f0: 2069 7320 4e6f 6e65 2c0a 2020 2020 2020   is None,.      
+00001600: 2020 2020 2020 7768 6963 6820 7265 7375        which resu
+00001610: 6c74 7320 696e 2069 6465 6e74 6974 7920  lts in identity 
+00001620: 6d61 7472 6978 2c20 6974 2069 7320 7265  matrix, it is re
+00001630: 636f 6d6d 656e 6465 6420 746f 2067 6976  commended to giv
+00001640: 650a 2020 2020 2020 2020 2020 2020 6073  e.            `s
+00001650: 7570 6572 6365 6c6c 5f6d 6174 7269 7860  upercell_matrix`
+00001660: 2065 7870 6c69 6369 746c 792e 0a20 2020   explicitly..   
+00001670: 2020 2020 2070 7269 6d69 7469 7665 5f6d       primitive_m
+00001680: 6174 7269 7820 3a20 6172 7261 795f 6c69  atrix : array_li
+00001690: 6b65 206f 7220 7374 722c 206f 7074 696f  ke or str, optio
+000016a0: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
+000016b0: 5072 696d 6974 6976 6520 6d61 7472 6978  Primitive matrix
+000016c0: 206d 756c 7469 706c 6965 6420 746f 2069   multiplied to i
+000016d0: 6e70 7574 2063 656c 6c20 6261 7369 7320  nput cell basis 
+000016e0: 7665 6374 6f72 732e 2044 6566 6175 6c74  vectors. Default
+000016f0: 2069 730a 2020 2020 2020 2020 2020 2020   is.            
+00001700: 7468 6520 6964 656e 7469 7479 206d 6174  the identity mat
+00001710: 7269 782e 2057 6865 6e20 6769 7665 6e20  rix. When given 
+00001720: 6173 2061 7272 6179 5f6c 696b 652c 2073  as array_like, s
+00001730: 6861 7065 3d28 332c 2033 292c 0a20 2020  hape=(3, 3),.   
+00001740: 2020 2020 2020 2020 2064 7479 7065 3d66           dtype=f
+00001750: 6c6f 6174 2e20 5768 656e 2027 4627 2c20  loat. When 'F', 
+00001760: 2749 272c 2027 4127 2c20 2743 272c 206f  'I', 'A', 'C', o
+00001770: 7220 2752 2720 6973 2067 6976 656e 2069  r 'R' is given i
+00001780: 6e73 7465 6164 206f 6620 610a 2020 2020  nstead of a.    
+00001790: 2020 2020 2020 2020 3378 3320 6d61 7472          3x3 matr
+000017a0: 6978 2c20 7468 6520 7072 696d 6974 6976  ix, the primitiv
+000017b0: 6520 6d61 7472 6978 2064 6566 696e 6564  e matrix defined
+000017c0: 2061 740a 2020 2020 2020 2020 2020 2020   at.            
+000017d0: 6874 7470 733a 2f2f 7370 676c 6962 2e67  https://spglib.g
+000017e0: 6974 6875 622e 696f 2f73 7067 6c69 622f  ithub.io/spglib/
+000017f0: 6465 6669 6e69 7469 6f6e 2e68 746d 6c20  definition.html 
+00001800: 6973 2075 7365 642e 2057 6865 6e20 2761  is used. When 'a
+00001810: 7574 6f27 0a20 2020 2020 2020 2020 2020  uto'.           
+00001820: 2069 7320 6769 7665 6e2c 2074 6865 2063   is given, the c
+00001830: 656e 7472 696e 6720 7479 7065 2028 2746  entring type ('F
+00001840: 272c 2027 4927 2c20 2741 272c 2027 4327  ', 'I', 'A', 'C'
+00001850: 2c20 2752 272c 206f 7220 7072 696d 6974  , 'R', or primit
+00001860: 6976 650a 2020 2020 2020 2020 2020 2020  ive.            
+00001870: 2750 2729 2069 7320 6175 746f 6d61 7469  'P') is automati
+00001880: 6361 6c6c 7920 6368 6f73 656e 2e0a 2020  cally chosen..  
+00001890: 2020 2020 2020 7068 6f6e 6f6e 5f73 7570        phonon_sup
+000018a0: 6572 6365 6c6c 5f6d 6174 7269 7820 3a20  ercell_matrix : 
+000018b0: 6172 7261 795f 6c69 6b65 2c20 6f70 7469  array_like, opti
+000018c0: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
+000018d0: 2053 7570 6572 6365 6c6c 206d 6174 7269   Supercell matri
+000018e0: 7820 7573 6564 2066 6f72 2066 6332 2e20  x used for fc2. 
+000018f0: 496e 2070 686f 6e6f 3370 792c 2073 7570  In phono3py, sup
+00001900: 6572 6365 6c6c 206d 6174 7269 7820 666f  ercell matrix fo
+00001910: 7220 6663 330a 2020 2020 2020 2020 2020  r fc3.          
+00001920: 2020 616e 6420 6663 3220 6361 6e20 6265    and fc2 can be
+00001930: 2064 6966 6665 7265 6e74 2074 6f20 7375   different to su
+00001940: 7070 6f72 7420 6c6f 6e67 6572 2072 616e  pport longer ran
+00001950: 6765 2069 6e74 6572 6163 7469 6f6e 206f  ge interaction o
+00001960: 6620 6663 320a 2020 2020 2020 2020 2020  f fc2.          
+00001970: 2020 7468 616e 2074 6861 7420 6f66 2066    than that of f
+00001980: 6333 2e20 556e 6c65 7373 2073 6574 7469  c3. Unless setti
+00001990: 6e67 2074 6869 732c 2073 7570 6572 6365  ng this, superce
+000019a0: 6c6c 5f6d 6174 7269 7820 6973 2075 7365  ll_matrix is use
+000019b0: 642e 0a20 2020 2020 2020 2020 2020 2054  d..            T
+000019c0: 6869 7320 6973 206f 6e6c 7920 7661 6c69  his is only vali
+000019d0: 6465 2077 6865 6e20 756e 6974 6365 6c6c  de when unitcell
+000019e0: 206f 7220 756e 6974 6365 6c6c 5f66 696c   or unitcell_fil
+000019f0: 656e 616d 6520 6973 2067 6976 656e 2e0a  ename is given..
+00001a00: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
+00001a10: 756c 7420 6973 204e 6f6e 652e 0a20 2020  ult is None..   
+00001a20: 2020 2020 2063 7574 6f66 665f 6672 6571       cutoff_freq
+00001a30: 7565 6e63 7920 3a20 666c 6f61 742c 206f  uency : float, o
+00001a40: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+00001a50: 2020 2020 5068 6f6e 6f6e 2066 7265 7175      Phonon frequ
+00001a60: 656e 6379 2062 656c 6f77 2074 6869 7320  ency below this 
+00001a70: 7661 6c75 6520 6973 2069 676e 6f72 6564  value is ignored
+00001a80: 2077 6865 6e20 7468 6520 6375 746f 6666   when the cutoff
+00001a90: 2069 730a 2020 2020 2020 2020 2020 2020   is.            
+00001aa0: 6e65 6564 6564 2066 6f72 2074 6865 2063  needed for the c
+00001ab0: 6f6d 7075 7461 7469 6f6e 2e20 4465 6661  omputation. Defa
+00001ac0: 756c 7420 6973 2031 652d 342e 0a20 2020  ult is 1e-4..   
+00001ad0: 2020 2020 2066 7265 7175 656e 6379 5f66       frequency_f
+00001ae0: 6163 746f 725f 746f 5f54 487a 203a 2066  actor_to_THz : f
+00001af0: 6c6f 6174 2c20 6f70 7469 6f6e 616c 0a20  loat, optional. 
+00001b00: 2020 2020 2020 2020 2020 2050 686f 6e6f             Phono
+00001b10: 6e20 6672 6571 7565 6e63 7920 756e 6974  n frequency unit
+00001b20: 2063 6f6e 7665 7273 696f 6e20 6661 6374   conversion fact
+00001b30: 6f72 2e20 556e 6c65 7373 2073 7065 6369  or. Unless speci
+00001b40: 6669 6564 2c20 6465 6661 756c 740a 2020  fied, default.  
+00001b50: 2020 2020 2020 2020 2020 756e 6974 2063            unit c
+00001b60: 6f6e 7665 7273 696f 6e20 6661 6374 6f72  onversion factor
+00001b70: 2066 6f72 2065 6163 6820 6361 6c63 756c   for each calcul
+00001b80: 6174 6f72 2069 7320 7573 6564 2e0a 2020  ator is used..  
+00001b90: 2020 2020 2020 6973 5f73 796d 6d65 7472        is_symmetr
+00001ba0: 7920 3a20 626f 6f6c 2c20 6f70 7469 6f6e  y : bool, option
+00001bb0: 616c 0a20 2020 2020 2020 2020 2020 2055  al.            U
+00001bc0: 7365 2063 7279 7374 616c 2073 796d 6d65  se crystal symme
+00001bd0: 7472 7920 696e 206d 6f73 7420 6361 6c63  try in most calc
+00001be0: 756c 6174 696f 6e73 2077 6865 6e20 5472  ulations when Tr
+00001bf0: 7565 2e20 4465 6661 756c 7420 6973 0a20  ue. Default is. 
+00001c00: 2020 2020 2020 2020 2020 2054 7275 652e             True.
+00001c10: 0a20 2020 2020 2020 2069 735f 6d65 7368  .        is_mesh
+00001c20: 5f73 796d 6d65 7472 7920 3a20 626f 6f6c  _symmetry : bool
+00001c30: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+00001c40: 2020 2020 2020 2055 7365 2063 7279 7374         Use cryst
+00001c50: 616c 2073 796d 6d65 7472 7920 696e 2072  al symmetry in r
+00001c60: 6563 6970 726f 6361 6c20 7370 6163 6520  eciprocal space 
+00001c70: 6772 6964 2068 616e 646c 696e 6720 7768  grid handling wh
+00001c80: 656e 2054 7275 652e 0a20 2020 2020 2020  en True..       
+00001c90: 2020 2020 2044 6566 6175 6c74 2069 7320       Default is 
+00001ca0: 5472 7565 2e0a 2020 2020 2020 2020 7573  True..        us
+00001cb0: 655f 6772 6720 3a20 626f 6f6c 2c20 6f70  e_grg : bool, op
+00001cc0: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
+00001cd0: 2020 2055 7365 2067 656e 6572 616c 697a     Use generaliz
+00001ce0: 6564 2072 6567 756c 6172 2067 7269 6420  ed regular grid 
+00001cf0: 7768 656e 2054 7275 652e 2044 6566 6175  when True. Defau
+00001d00: 6c74 2069 7320 4661 6c73 652e 0a20 2020  lt is False..   
+00001d10: 2020 2020 2053 4e46 5f63 6f6f 7264 696e       SNF_coordin
+00001d20: 6174 6573 203a 2073 7472 2c20 6f70 7469  ates : str, opti
+00001d30: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
+00001d40: 2060 7265 6369 7072 6f63 616c 6020 6f72   `reciprocal` or
+00001d50: 2060 6469 7265 6374 602e 2053 7061 6365   `direct`. Space
+00001d60: 206f 6620 636f 6f72 6469 6e61 7465 7320   of coordinates 
+00001d70: 746f 2067 656e 6572 6174 6520 6772 6964  to generate grid
+00001d80: 0a20 2020 2020 2020 2020 2020 2067 656e  .            gen
+00001d90: 6572 6174 696e 6720 6d61 7472 6978 2065  erating matrix e
+00001da0: 6974 6865 7220 696e 2064 6972 6563 7420  ither in direct 
+00001db0: 6f72 2072 6563 6970 726f 6361 6c20 7370  or reciprocal sp
+00001dc0: 6163 652e 2054 6865 2064 6566 6175 6c74  ace. The default
+00001dd0: 0a20 2020 2020 2020 2020 2020 2069 7320  .            is 
+00001de0: 6072 6563 6970 726f 6361 6c60 2e0a 2020  `reciprocal`..  
+00001df0: 2020 2020 2020 6d61 6b65 5f72 305f 6176        make_r0_av
+00001e00: 6572 6167 6520 3a20 626f 6f6c 2c20 6f70  erage : bool, op
+00001e10: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
+00001e20: 2020 2066 6333 2074 7261 6e73 666f 726d     fc3 transform
+00001e30: 6174 696f 6e20 6672 6f6d 2072 6561 6c20  ation from real 
+00001e40: 746f 2072 6563 6970 726f 6361 6c20 7370  to reciprocal sp
+00001e50: 6163 6520 6973 2064 6f6e 650a 2020 2020  ace is done.    
+00001e60: 2020 2020 2020 2020 6172 6f75 6e64 2074          around t
+00001e70: 6872 6565 2061 746f 6d73 2061 6e64 2061  hree atoms and a
+00001e80: 7665 7261 6765 6420 7768 656e 2054 7275  veraged when Tru
+00001e90: 652e 2044 6566 6175 6c74 2069 7320 4661  e. Default is Fa
+00001ea0: 6c73 652c 2069 2e65 2e2c 0a20 2020 2020  lse, i.e.,.     
+00001eb0: 2020 2020 2020 206f 6e6c 7920 6172 6f75         only arou
+00001ec0: 6e64 2074 6865 2066 6972 7374 2061 746f  nd the first ato
+00001ed0: 6d2e 2053 6574 7469 6e67 2046 616c 7365  m. Setting False
+00001ee0: 2069 7320 666f 7220 726f 7567 6820 636f   is for rough co
+00001ef0: 6d70 6174 6962 696c 6974 790a 2020 2020  mpatibility.    
+00001f00: 2020 2020 2020 2020 7769 7468 2076 322e          with v2.
+00001f10: 782e 2044 6566 6175 6c74 2069 7320 5472  x. Default is Tr
+00001f20: 7565 2e0a 2020 2020 2020 2020 7379 6d70  ue..        symp
+00001f30: 7265 6320 3a20 666c 6f61 742c 206f 7074  rec : float, opt
+00001f40: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+00001f50: 2020 546f 6c65 7261 6e63 6520 7573 6564    Tolerance used
+00001f60: 2074 6f20 6669 6e64 2063 7279 7374 616c   to find crystal
+00001f70: 2073 796d 6d65 7472 792e 2044 6566 6175   symmetry. Defau
+00001f80: 6c74 2069 7320 3165 2d35 2e0a 2020 2020  lt is 1e-5..    
+00001f90: 2020 2020 6361 6c63 756c 6174 6f72 203a      calculator :
+00001fa0: 2073 7472 2c20 6f70 7469 6f6e 616c 2e0a   str, optional..
+00001fb0: 2020 2020 2020 2020 2020 2020 4361 6c63              Calc
+00001fc0: 756c 6174 6f72 2075 7365 6420 666f 7220  ulator used for 
+00001fd0: 636f 6d70 7574 696e 6720 666f 7263 6573  computing forces
+00001fe0: 2e20 5468 6973 2069 7320 7573 6564 2074  . This is used t
+00001ff0: 6f20 7377 6974 6368 2074 6865 2073 6574  o switch the set
+00002000: 0a20 2020 2020 2020 2020 2020 206f 6620  .            of 
+00002010: 7068 7973 6963 616c 2075 6e69 7473 2e20  physical units. 
+00002020: 4465 6661 756c 7420 6973 204e 6f6e 652c  Default is None,
+00002030: 2077 6869 6368 2069 7320 6571 7569 7661   which is equiva
+00002040: 6c65 6e74 2074 6f20 2276 6173 7022 2e0a  lent to "vasp"..
+00002050: 2020 2020 2020 2020 6c6f 675f 6c65 7665          log_leve
+00002060: 6c20 3a20 696e 742c 206f 7074 696f 6e61  l : int, optiona
+00002070: 6c0a 2020 2020 2020 2020 2020 2020 5665  l.            Ve
+00002080: 7262 6f73 6974 7920 636f 6e74 726f 6c2e  rbosity control.
+00002090: 2044 6566 6175 6c74 2069 7320 302e 2054   Default is 0. T
+000020a0: 6869 7320 6361 6e20 6265 2030 2c20 312c  his can be 0, 1,
+000020b0: 206f 7220 322e 0a0a 2020 2020 2020 2020   or 2...        
+000020c0: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
+000020d0: 2e5f 7379 6d70 7265 6320 3d20 7379 6d70  ._symprec = symp
+000020e0: 7265 630a 2020 2020 2020 2020 7365 6c66  rec.        self
+000020f0: 2e5f 6672 6571 7565 6e63 795f 6661 6374  ._frequency_fact
+00002100: 6f72 5f74 6f5f 5448 7a20 3d20 6672 6571  or_to_THz = freq
+00002110: 7565 6e63 795f 6661 6374 6f72 5f74 6f5f  uency_factor_to_
+00002120: 5448 7a0a 2020 2020 2020 2020 7365 6c66  THz.        self
+00002130: 2e5f 6973 5f73 796d 6d65 7472 7920 3d20  ._is_symmetry = 
+00002140: 6973 5f73 796d 6d65 7472 790a 2020 2020  is_symmetry.    
+00002150: 2020 2020 7365 6c66 2e5f 6973 5f6d 6573      self._is_mes
+00002160: 685f 7379 6d6d 6574 7279 203d 2069 735f  h_symmetry = is_
+00002170: 6d65 7368 5f73 796d 6d65 7472 790a 2020  mesh_symmetry.  
+00002180: 2020 2020 2020 7365 6c66 2e5f 7573 655f        self._use_
+00002190: 6772 6720 3d20 7573 655f 6772 670a 2020  grg = use_grg.  
+000021a0: 2020 2020 2020 7365 6c66 2e5f 534e 465f        self._SNF_
+000021b0: 636f 6f72 6469 6e61 7465 7320 3d20 534e  coordinates = SN
+000021c0: 465f 636f 6f72 6469 6e61 7465 730a 0a20  F_coordinates.. 
+000021d0: 2020 2020 2020 2073 656c 662e 5f6d 616b         self._mak
+000021e0: 655f 7230 5f61 7665 7261 6765 203d 206d  e_r0_average = m
+000021f0: 616b 655f 7230 5f61 7665 7261 6765 0a0a  ake_r0_average..
+00002200: 2020 2020 2020 2020 7365 6c66 2e5f 6375          self._cu
+00002210: 746f 6666 5f66 7265 7175 656e 6379 203d  toff_frequency =
+00002220: 2063 7574 6f66 665f 6672 6571 7565 6e63   cutoff_frequenc
+00002230: 790a 2020 2020 2020 2020 7365 6c66 2e5f  y.        self._
+00002240: 6361 6c63 756c 6174 6f72 3a20 4f70 7469  calculator: Opti
+00002250: 6f6e 616c 5b73 7472 5d20 3d20 6361 6c63  onal[str] = calc
+00002260: 756c 6174 6f72 0a20 2020 2020 2020 2073  ulator.        s
+00002270: 656c 662e 5f6c 6f67 5f6c 6576 656c 203d  elf._log_level =
+00002280: 206c 6f67 5f6c 6576 656c 0a0a 2020 2020   log_level..    
+00002290: 2020 2020 2320 4372 6561 7465 2073 7570      # Create sup
+000022a0: 6572 6365 6c6c 2061 6e64 2070 7269 6d69  ercell and primi
+000022b0: 7469 7665 2063 656c 6c0a 2020 2020 2020  tive cell.      
+000022c0: 2020 7365 6c66 2e5f 756e 6974 6365 6c6c    self._unitcell
+000022d0: 203d 2075 6e69 7463 656c 6c0a 2020 2020   = unitcell.    
+000022e0: 2020 2020 7365 6c66 2e5f 7375 7065 7263      self._superc
+000022f0: 656c 6c5f 6d61 7472 6978 203d 206e 702e  ell_matrix = np.
+00002300: 6172 7261 7928 0a20 2020 2020 2020 2020  array(.         
+00002310: 2020 2073 6861 7065 5f73 7570 6572 6365     shape_superce
+00002320: 6c6c 5f6d 6174 7269 7828 7375 7065 7263  ll_matrix(superc
+00002330: 656c 6c5f 6d61 7472 6978 292c 2064 7479  ell_matrix), dty
+00002340: 7065 3d22 696e 745f 222c 206f 7264 6572  pe="int_", order
+00002350: 3d22 4322 0a20 2020 2020 2020 2029 0a20  ="C".        ). 
+00002360: 2020 2020 2020 2070 6d61 7420 3d20 7365         pmat = se
+00002370: 6c66 2e5f 6465 7465 726d 696e 655f 7072  lf._determine_pr
+00002380: 696d 6974 6976 655f 6d61 7472 6978 2870  imitive_matrix(p
+00002390: 7269 6d69 7469 7665 5f6d 6174 7269 7829  rimitive_matrix)
+000023a0: 0a20 2020 2020 2020 2073 656c 662e 5f70  .        self._p
+000023b0: 7269 6d69 7469 7665 5f6d 6174 7269 7820  rimitive_matrix 
+000023c0: 3d20 706d 6174 0a20 2020 2020 2020 2073  = pmat.        s
+000023d0: 656c 662e 5f6e 6163 5f70 6172 616d 7320  elf._nac_params 
+000023e0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2069  = None.        i
+000023f0: 6620 7068 6f6e 6f6e 5f73 7570 6572 6365  f phonon_superce
+00002400: 6c6c 5f6d 6174 7269 7820 6973 206e 6f74  ll_matrix is not
+00002410: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00002420: 2020 2073 656c 662e 5f70 686f 6e6f 6e5f     self._phonon_
+00002430: 7375 7065 7263 656c 6c5f 6d61 7472 6978  supercell_matrix
+00002440: 203d 206e 702e 6172 7261 7928 0a20 2020   = np.array(.   
+00002450: 2020 2020 2020 2020 2020 2020 2073 6861               sha
+00002460: 7065 5f73 7570 6572 6365 6c6c 5f6d 6174  pe_supercell_mat
+00002470: 7269 7828 7068 6f6e 6f6e 5f73 7570 6572  rix(phonon_super
+00002480: 6365 6c6c 5f6d 6174 7269 7829 2c20 6474  cell_matrix), dt
+00002490: 7970 653d 2269 6e74 5f22 2c20 6f72 6465  ype="int_", orde
+000024a0: 723d 2243 220a 2020 2020 2020 2020 2020  r="C".          
+000024b0: 2020 290a 2020 2020 2020 2020 656c 7365    ).        else
+000024c0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000024d0: 6c66 2e5f 7068 6f6e 6f6e 5f73 7570 6572  lf._phonon_super
+000024e0: 6365 6c6c 5f6d 6174 7269 7820 3d20 4e6f  cell_matrix = No
+000024f0: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
+00002500: 5f73 7570 6572 6365 6c6c 203d 204e 6f6e  _supercell = Non
+00002510: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
+00002520: 7072 696d 6974 6976 6520 3d20 4e6f 6e65  primitive = None
+00002530: 0a20 2020 2020 2020 2073 656c 662e 5f70  .        self._p
+00002540: 686f 6e6f 6e5f 7375 7065 7263 656c 6c20  honon_supercell 
+00002550: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
+00002560: 656c 662e 5f70 686f 6e6f 6e5f 7072 696d  elf._phonon_prim
+00002570: 6974 6976 6520 3d20 4e6f 6e65 0a20 2020  itive = None.   
+00002580: 2020 2020 2073 656c 662e 5f62 7569 6c64       self._build
+00002590: 5f73 7570 6572 6365 6c6c 2829 0a20 2020  _supercell().   
+000025a0: 2020 2020 2073 656c 662e 5f62 7569 6c64       self._build
+000025b0: 5f70 7269 6d69 7469 7665 5f63 656c 6c28  _primitive_cell(
+000025c0: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
+000025d0: 6275 696c 645f 7068 6f6e 6f6e 5f73 7570  build_phonon_sup
+000025e0: 6572 6365 6c6c 2829 0a20 2020 2020 2020  ercell().       
+000025f0: 2073 656c 662e 5f62 7569 6c64 5f70 686f   self._build_pho
+00002600: 6e6f 6e5f 7072 696d 6974 6976 655f 6365  non_primitive_ce
+00002610: 6c6c 2829 0a0a 2020 2020 2020 2020 7365  ll()..        se
+00002620: 6c66 2e5f 7369 676d 6173 203d 205b 0a20  lf._sigmas = [. 
+00002630: 2020 2020 2020 2020 2020 204e 6f6e 652c             None,
+00002640: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
+00002650: 2020 2073 656c 662e 5f73 6967 6d61 5f63     self._sigma_c
+00002660: 7574 6f66 6620 3d20 4e6f 6e65 0a0a 2020  utoff = None..  
+00002670: 2020 2020 2020 2320 4772 6964 0a20 2020        # Grid.   
+00002680: 2020 2020 2073 656c 662e 5f62 7a5f 6772       self._bz_gr
+00002690: 6964 203d 204e 6f6e 650a 0a20 2020 2020  id = None..     
+000026a0: 2020 2023 2053 6574 2073 7570 6572 6365     # Set superce
+000026b0: 6c6c 2c20 7072 696d 6974 6976 652c 2061  ll, primitive, a
+000026c0: 6e64 2070 686f 6e6f 6e20 7375 7065 7263  nd phonon superc
+000026d0: 656c 6c20 7379 6d6d 6574 7269 6573 0a20  ell symmetries. 
+000026e0: 2020 2020 2020 2073 656c 662e 5f73 796d         self._sym
+000026f0: 6d65 7472 7920 3d20 4e6f 6e65 0a20 2020  metry = None.   
+00002700: 2020 2020 2073 656c 662e 5f70 7269 6d69       self._primi
+00002710: 7469 7665 5f73 796d 6d65 7472 7920 3d20  tive_symmetry = 
+00002720: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
+00002730: 662e 5f70 686f 6e6f 6e5f 7375 7065 7263  f._phonon_superc
+00002740: 656c 6c5f 7379 6d6d 6574 7279 203d 204e  ell_symmetry = N
+00002750: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+00002760: 2e5f 7365 6172 6368 5f73 796d 6d65 7472  ._search_symmetr
+00002770: 7928 290a 2020 2020 2020 2020 7365 6c66  y().        self
+00002780: 2e5f 7365 6172 6368 5f70 7269 6d69 7469  ._search_primiti
+00002790: 7665 5f73 796d 6d65 7472 7928 290a 2020  ve_symmetry().  
+000027a0: 2020 2020 2020 7365 6c66 2e5f 7365 6172        self._sear
+000027b0: 6368 5f70 686f 6e6f 6e5f 7375 7065 7263  ch_phonon_superc
+000027c0: 656c 6c5f 7379 6d6d 6574 7279 2829 0a0a  ell_symmetry()..
+000027d0: 2020 2020 2020 2020 2320 4469 7370 6c61          # Displa
+000027e0: 6365 6d65 6e74 7320 616e 6420 7375 7065  cements and supe
+000027f0: 7263 656c 6c73 0a20 2020 2020 2020 2073  rcells.        s
+00002800: 656c 662e 5f73 7570 6572 6365 6c6c 735f  elf._supercells_
+00002810: 7769 7468 5f64 6973 706c 6163 656d 656e  with_displacemen
+00002820: 7473 203d 204e 6f6e 650a 2020 2020 2020  ts = None.      
+00002830: 2020 7365 6c66 2e5f 6461 7461 7365 7420    self._dataset 
+00002840: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
+00002850: 656c 662e 5f70 686f 6e6f 6e5f 6461 7461  elf._phonon_data
+00002860: 7365 7420 3d20 4e6f 6e65 0a20 2020 2020  set = None.     
+00002870: 2020 2073 656c 662e 5f70 686f 6e6f 6e5f     self._phonon_
+00002880: 7375 7065 7263 656c 6c73 5f77 6974 685f  supercells_with_
+00002890: 6469 7370 6c61 6365 6d65 6e74 7320 3d20  displacements = 
+000028a0: 4e6f 6e65 0a0a 2020 2020 2020 2020 2320  None..        # 
+000028b0: 5468 6572 6d61 6c20 636f 6e64 7563 7469  Thermal conducti
+000028c0: 7669 7479 0a20 2020 2020 2020 2023 2063  vity.        # c
+000028d0: 6f6e 6475 6374 6976 6974 795f 5254 4120  onductivity_RTA 
+000028e0: 6f72 2063 6f6e 6475 6374 6976 6974 795f  or conductivity_
+000028f0: 4c42 5445 2063 6c61 7373 2069 6e73 7461  LBTE class insta
+00002900: 6e63 650a 2020 2020 2020 2020 7365 6c66  nce.        self
+00002910: 2e5f 7468 6572 6d61 6c5f 636f 6e64 7563  ._thermal_conduc
+00002920: 7469 7669 7479 203d 204e 6f6e 650a 0a20  tivity = None.. 
+00002930: 2020 2020 2020 2023 2049 6d61 6769 6e61         # Imagina
+00002940: 7279 2070 6172 7420 6f66 2073 656c 6620  ry part of self 
+00002950: 656e 6572 6779 2061 7420 6672 6571 7565  energy at freque
+00002960: 6e63 7920 706f 696e 7473 0a20 2020 2020  ncy points.     
+00002970: 2020 2073 656c 662e 5f67 616d 6d61 7320     self._gammas 
+00002980: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
+00002990: 656c 662e 5f73 6361 7474 6572 696e 675f  elf._scattering_
+000029a0: 6576 656e 745f 636c 6173 7320 3d20 4e6f  event_class = No
+000029b0: 6e65 0a0a 2020 2020 2020 2020 2320 4672  ne..        # Fr
+000029c0: 6571 7565 6e63 7920 7368 6966 7420 2872  equency shift (r
+000029d0: 6561 6c20 7061 7274 206f 6620 6275 6262  eal part of bubb
+000029e0: 6c65 2064 6961 6772 616d 290a 2020 2020  le diagram).    
+000029f0: 2020 2020 7365 6c66 2e5f 7265 616c 5f73      self._real_s
+00002a00: 656c 665f 656e 6572 6779 203d 204e 6f6e  elf_energy = Non
+00002a10: 650a 0a20 2020 2020 2020 2073 656c 662e  e..        self.
+00002a20: 5f67 7269 645f 706f 696e 7473 203d 204e  _grid_points = N
+00002a30: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+00002a40: 2e5f 6672 6571 7565 6e63 795f 706f 696e  ._frequency_poin
+00002a50: 7473 203d 204e 6f6e 650a 2020 2020 2020  ts = None.      
+00002a60: 2020 7365 6c66 2e5f 7465 6d70 6572 6174    self._temperat
+00002a70: 7572 6573 203d 204e 6f6e 650a 0a20 2020  ures = None..   
+00002a80: 2020 2020 2023 204f 7468 6572 2076 6172       # Other var
+00002a90: 6961 626c 6573 0a20 2020 2020 2020 2073  iables.        s
+00002aa0: 656c 662e 5f66 6332 203d 204e 6f6e 650a  elf._fc2 = None.
+00002ab0: 2020 2020 2020 2020 7365 6c66 2e5f 6663          self._fc
+00002ac0: 3320 3d20 4e6f 6e65 0a0a 2020 2020 2020  3 = None..      
+00002ad0: 2020 2320 5365 7475 7020 696e 7465 7261    # Setup intera
+00002ae0: 6374 696f 6e0a 2020 2020 2020 2020 7365  ction.        se
+00002af0: 6c66 2e5f 696e 7465 7261 6374 696f 6e20  lf._interaction 
+00002b00: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
+00002b10: 656c 662e 5f62 616e 645f 696e 6469 6365  elf._band_indice
+00002b20: 7320 3d20 4e6f 6e65 0a20 2020 2020 2020  s = None.       
+00002b30: 2073 656c 662e 5f62 616e 645f 696e 6469   self._band_indi
+00002b40: 6365 735f 666c 6174 7465 6e20 3d20 4e6f  ces_flatten = No
+00002b50: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
+00002b60: 5f73 6574 5f62 616e 645f 696e 6469 6365  _set_band_indice
+00002b70: 7328 290a 0a20 2020 2040 7072 6f70 6572  s()..    @proper
+00002b80: 7479 0a20 2020 2064 6566 2076 6572 7369  ty.    def versi
+00002b90: 6f6e 2873 656c 6629 3a0a 2020 2020 2020  on(self):.      
+00002ba0: 2020 2222 2252 6574 7572 6e20 7068 6f6e    """Return phon
+00002bb0: 6f33 7079 2072 656c 6561 7365 2076 6572  o3py release ver
+00002bc0: 7369 6f6e 206e 756d 6265 722e 0a0a 2020  sion number...  
+00002bd0: 2020 2020 2020 7374 720a 2020 2020 2020        str.      
+00002be0: 2020 2020 2020 5068 6f6e 6f33 7079 2072        Phono3py r
+00002bf0: 656c 6561 7365 2076 6572 7369 6f6e 206e  elease version n
+00002c00: 756d 6265 720a 0a20 2020 2020 2020 2022  umber..        "
+00002c10: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+00002c20: 6e20 5f5f 7665 7273 696f 6e5f 5f0a 0a20  n __version__.. 
+00002c30: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00002c40: 2064 6566 2063 616c 6375 6c61 746f 7228   def calculator(
+00002c50: 7365 6c66 2920 2d3e 204f 7074 696f 6e61  self) -> Optiona
+00002c60: 6c5b 7374 725d 3a0a 2020 2020 2020 2020  l[str]:.        
+00002c70: 2222 2252 6574 7572 6e20 6361 6c63 756c  """Return calcul
+00002c80: 6174 6f72 2069 6e74 6572 6661 6365 206e  ator interface n
+00002c90: 616d 652e 0a0a 2020 2020 2020 2020 7374  ame...        st
+00002ca0: 720a 2020 2020 2020 2020 2020 2020 4361  r.            Ca
+00002cb0: 6c63 756c 6174 6f72 206e 616d 6520 7375  lculator name su
+00002cc0: 6368 2061 7320 2776 6173 7027 2c20 2771  ch as 'vasp', 'q
+00002cd0: 6527 2c20 6574 632e 0a0a 2020 2020 2020  e', etc...      
+00002ce0: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+00002cf0: 7475 726e 2073 656c 662e 5f63 616c 6375  turn self._calcu
+00002d00: 6c61 746f 720a 0a20 2020 2040 7072 6f70  lator..    @prop
+00002d10: 6572 7479 0a20 2020 2064 6566 2066 6333  erty.    def fc3
+00002d20: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00002d30: 2222 2253 6574 7465 7220 616e 6420 6765  """Setter and ge
+00002d40: 7474 6572 206f 6620 7468 6972 6420 6f72  tter of third or
+00002d50: 6465 7220 666f 7263 6520 636f 6e73 7461  der force consta
+00002d60: 6e74 7320 2866 6333 292e 0a0a 2020 2020  nts (fc3)...    
+00002d70: 2020 2020 6e64 6172 7261 790a 2020 2020      ndarray.    
+00002d80: 2020 2020 2020 2020 6663 3320 7368 6170          fc3 shap
+00002d90: 6520 6973 2065 6974 6865 7220 2873 7570  e is either (sup
+00002da0: 6572 6365 6c6c 2c20 7375 7065 6365 6c6c  ercell, supecell
+00002db0: 2c20 7375 7065 7263 656c 6c2c 2033 2c20  , supercell, 3, 
+00002dc0: 332c 2033 2920 6f72 0a20 2020 2020 2020  3, 3) or.       
+00002dd0: 2020 2020 2028 7072 696d 6974 6976 652c       (primitive,
+00002de0: 2073 7570 6572 6365 6c6c 2c20 7375 7065   supercell, supe
+00002df0: 6365 6c6c 2c20 332c 2033 2c20 3329 2c0a  cell, 3, 3, 3),.
+00002e00: 2020 2020 2020 2020 2020 2020 7768 6572              wher
+00002e10: 6520 2773 7570 6572 6365 6c6c 2720 616e  e 'supercell' an
+00002e20: 6420 2770 7269 6d69 7469 7665 2720 696e  d 'primitive' in
+00002e30: 6469 6361 7465 206e 756d 6265 7220 6f66  dicate number of
+00002e40: 2061 746f 6d73 2069 6e0a 2020 2020 2020   atoms in.      
+00002e50: 2020 2020 2020 7468 6573 6520 6365 6c6c        these cell
+00002e60: 732e 0a0a 2020 2020 2020 2020 2222 220a  s...        """.
+00002e70: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00002e80: 656c 662e 5f66 6333 0a0a 2020 2020 4066  elf._fc3..    @f
+00002e90: 6333 2e73 6574 7465 720a 2020 2020 6465  c3.setter.    de
+00002ea0: 6620 6663 3328 7365 6c66 2c20 6663 3329  f fc3(self, fc3)
+00002eb0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00002ec0: 6663 3320 3d20 6663 330a 0a20 2020 2040  fc3 = fc3..    @
+00002ed0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00002ee0: 2066 6332 2873 656c 6629 3a0a 2020 2020   fc2(self):.    
+00002ef0: 2020 2020 2222 2253 6574 7465 7220 616e      """Setter an
+00002f00: 6420 6765 7474 6572 206f 6620 7365 636f  d getter of seco
+00002f10: 6e64 206f 7264 6572 2066 6f72 6365 2063  nd order force c
+00002f20: 6f6e 7374 616e 7473 2028 6663 3229 2e0a  onstants (fc2)..
+00002f30: 0a20 2020 2020 2020 206e 6461 7272 6179  .        ndarray
+00002f40: 0a20 2020 2020 2020 2020 2020 2066 6332  .            fc2
+00002f50: 2073 6861 7065 2069 7320 6569 7468 6572   shape is either
+00002f60: 2028 7375 7065 7263 656c 6c2c 2073 7570   (supercell, sup
+00002f70: 6563 656c 6c2c 2033 2c20 3329 206f 720a  ecell, 3, 3) or.
+00002f80: 2020 2020 2020 2020 2020 2020 2870 7269              (pri
+00002f90: 6d69 7469 7665 2c20 7375 7065 6365 6c6c  mitive, supecell
+00002fa0: 2c20 332c 2033 292c 0a20 2020 2020 2020  , 3, 3),.       
+00002fb0: 2020 2020 2077 6865 7265 2027 7375 7065       where 'supe
+00002fc0: 7263 656c 6c27 2061 6e64 2027 7072 696d  rcell' and 'prim
+00002fd0: 6974 6976 6527 2069 6e64 6963 6174 6520  itive' indicate 
+00002fe0: 6e75 6d62 6572 206f 6620 6174 6f6d 7320  number of atoms 
+00002ff0: 696e 0a20 2020 2020 2020 2020 2020 2074  in.            t
+00003000: 6865 7365 2063 656c 6c73 2e0a 0a20 2020  hese cells...   
+00003010: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00003020: 2072 6574 7572 6e20 7365 6c66 2e5f 6663   return self._fc
+00003030: 320a 0a20 2020 2040 6663 322e 7365 7474  2..    @fc2.sett
+00003040: 6572 0a20 2020 2064 6566 2066 6332 2873  er.    def fc2(s
+00003050: 656c 662c 2066 6332 293a 0a20 2020 2020  elf, fc2):.     
+00003060: 2020 2073 656c 662e 5f66 6332 203d 2066     self._fc2 = f
+00003070: 6332 0a0a 2020 2020 4070 726f 7065 7274  c2..    @propert
+00003080: 790a 2020 2020 6465 6620 666f 7263 655f  y.    def force_
+00003090: 636f 6e73 7461 6e74 7328 7365 6c66 293a  constants(self):
+000030a0: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+000030b0: 726e 2066 6332 2e20 5468 6973 2069 7320  rn fc2. This is 
+000030c0: 7361 6d65 2061 7320 7468 6520 6765 7474  same as the gett
+000030d0: 6572 2061 7474 7269 6275 7465 2060 6663  er attribute `fc
+000030e0: 3260 2e22 2222 0a20 2020 2020 2020 2072  2`.""".        r
+000030f0: 6574 7572 6e20 7365 6c66 2e66 6332 0a0a  eturn self.fc2..
+00003100: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00003110: 2020 6465 6620 7369 676d 6173 2873 656c    def sigmas(sel
+00003120: 6629 3a0a 2020 2020 2020 2020 2222 2253  f):.        """S
+00003130: 6574 7465 7220 616e 6420 6765 7474 6572  etter and getter
+00003140: 206f 6620 736d 6561 7269 6e67 2077 6964   of smearing wid
+00003150: 7468 732e 0a0a 2020 2020 2020 2020 6c69  ths...        li
+00003160: 7374 0a20 2020 2020 2020 2020 2020 2054  st.            T
+00003170: 6865 2066 6c6f 6174 2076 616c 7565 7320  he float values 
+00003180: 6172 6520 6769 7665 6e20 6173 2074 6865  are given as the
+00003190: 2073 7461 6e64 6172 6420 6465 7669 6174   standard deviat
+000031a0: 696f 6e73 206f 6620 4761 7573 7369 616e  ions of Gaussian
+000031b0: 0a20 2020 2020 2020 2020 2020 2066 756e  .            fun
+000031c0: 6374 696f 6e2e 2049 6620 4e6f 6e65 2069  ction. If None i
+000031d0: 7320 6769 7665 6e20 6173 2061 6e20 656c  s given as an el
+000031e0: 656d 656e 7420 6f66 2074 6869 7320 6c69  ement of this li
+000031f0: 7374 2c20 6c69 6e65 6172 0a20 2020 2020  st, linear.     
+00003200: 2020 2020 2020 2074 6574 7261 6865 6472         tetrahedr
+00003210: 6f6e 206d 6574 686f 6420 6973 2075 7365  on method is use
+00003220: 6420 696e 7374 6561 6420 6f66 2073 6d65  d instead of sme
+00003230: 6172 696e 6720 6d65 7468 6f64 2e0a 0a20  aring method... 
+00003240: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00003250: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00003260: 7369 676d 6173 0a0a 2020 2020 4073 6967  sigmas..    @sig
+00003270: 6d61 732e 7365 7474 6572 0a20 2020 2064  mas.setter.    d
+00003280: 6566 2073 6967 6d61 7328 7365 6c66 2c20  ef sigmas(self, 
+00003290: 7369 676d 6173 293a 0a20 2020 2020 2020  sigmas):.       
+000032a0: 2069 6620 7369 676d 6173 2069 7320 4e6f   if sigmas is No
+000032b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000032c0: 7365 6c66 2e5f 7369 676d 6173 203d 205b  self._sigmas = [
+000032d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000032e0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+000032f0: 2020 205d 0a20 2020 2020 2020 2065 6c69     ].        eli
+00003300: 6620 6973 696e 7374 616e 6365 2873 6967  f isinstance(sig
+00003310: 6d61 732c 2066 6c6f 6174 2920 6f72 2069  mas, float) or i
+00003320: 7369 6e73 7461 6e63 6528 7369 676d 6173  sinstance(sigmas
+00003330: 2c20 696e 7429 3a0a 2020 2020 2020 2020  , int):.        
+00003340: 2020 2020 7365 6c66 2e5f 7369 676d 6173      self._sigmas
+00003350: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+00003360: 2020 2020 2066 6c6f 6174 2873 6967 6d61       float(sigma
+00003370: 7329 2c0a 2020 2020 2020 2020 2020 2020  s),.            
+00003380: 5d0a 2020 2020 2020 2020 656c 7365 3a0a  ].        else:.
+00003390: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000033a0: 2e5f 7369 676d 6173 203d 205b 5d0a 2020  ._sigmas = [].  
+000033b0: 2020 2020 2020 2020 2020 666f 7220 7320            for s 
+000033c0: 696e 2073 6967 6d61 733a 0a20 2020 2020  in sigmas:.     
+000033d0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+000033e0: 696e 7374 616e 6365 2873 2c20 666c 6f61  instance(s, floa
+000033f0: 7429 206f 7220 6973 696e 7374 616e 6365  t) or isinstance
+00003400: 2873 2c20 696e 7429 3a0a 2020 2020 2020  (s, int):.      
+00003410: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003420: 6c66 2e5f 7369 676d 6173 2e61 7070 656e  lf._sigmas.appen
+00003430: 6428 666c 6f61 7428 7329 290a 2020 2020  d(float(s)).    
+00003440: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00003450: 2073 2069 7320 4e6f 6e65 3a0a 2020 2020   s is None:.    
+00003460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003470: 7365 6c66 2e5f 7369 676d 6173 2e61 7070  self._sigmas.app
+00003480: 656e 6428 4e6f 6e65 290a 0a20 2020 2040  end(None)..    @
+00003490: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+000034a0: 2073 6967 6d61 5f63 7574 6f66 6628 7365   sigma_cutoff(se
+000034b0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+000034c0: 5365 7474 6572 2061 6e64 2067 6574 7465  Setter and gette
+000034d0: 7220 6f66 2053 6d65 6172 696e 6720 6375  r of Smearing cu
+000034e0: 746f 6666 2077 6964 7468 2e0a 0a20 2020  toff width...   
+000034f0: 2020 2020 2054 6869 7320 6973 2067 6976       This is giv
+00003500: 656e 2061 7320 6120 6d75 6c74 6970 6c65  en as a multiple
+00003510: 206f 6620 7468 6520 7374 616e 6461 7264   of the standard
+00003520: 2064 6576 6961 7469 6f6e 2e0a 0a20 2020   deviation...   
+00003530: 2020 2020 2066 6c6f 6174 0a20 2020 2020       float.     
+00003540: 2020 2020 2020 2046 6f72 2065 7861 6d70         For examp
+00003550: 6c65 2c20 6966 2074 6869 7320 7661 6c75  le, if this valu
+00003560: 6520 6973 2035 2c20 7468 6520 7461 696c  e is 5, the tail
+00003570: 206f 6620 7468 6520 4761 7573 7369 616e   of the Gaussian
+00003580: 2066 756e 6374 696f 6e0a 2020 2020 2020   function.      
+00003590: 2020 2020 2020 6973 2063 7574 2061 7420        is cut at 
+000035a0: 3520 7369 676d 612e 0a0a 2020 2020 2020  5 sigma...      
+000035b0: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+000035c0: 7475 726e 2073 656c 662e 5f73 6967 6d61  turn self._sigma
+000035d0: 5f63 7574 6f66 660a 0a20 2020 2040 7369  _cutoff..    @si
+000035e0: 676d 615f 6375 746f 6666 2e73 6574 7465  gma_cutoff.sette
+000035f0: 720a 2020 2020 6465 6620 7369 676d 615f  r.    def sigma_
+00003600: 6375 746f 6666 2873 656c 662c 2073 6967  cutoff(self, sig
+00003610: 6d61 5f63 7574 6f66 6629 3a0a 2020 2020  ma_cutoff):.    
+00003620: 2020 2020 7365 6c66 2e5f 7369 676d 615f      self._sigma_
+00003630: 6375 746f 6666 203d 2073 6967 6d61 5f63  cutoff = sigma_c
+00003640: 7574 6f66 660a 0a20 2020 2040 7072 6f70  utoff..    @prop
+00003650: 6572 7479 0a20 2020 2064 6566 206e 6163  erty.    def nac
+00003660: 5f70 6172 616d 7328 7365 6c66 293a 0a20  _params(self):. 
+00003670: 2020 2020 2020 2022 2222 5365 7474 6572         """Setter
+00003680: 2061 6e64 2067 6574 7465 7220 6f66 2070   and getter of p
+00003690: 6172 616d 6574 6572 7320 666f 7220 6e6f  arameters for no
+000036a0: 6e2d 616e 616c 7974 6963 616c 2074 6572  n-analytical ter
+000036b0: 6d20 636f 7272 6563 7469 6f6e 2e0a 0a20  m correction... 
+000036c0: 2020 2020 2020 2064 6963 740a 2020 2020         dict.    
+000036d0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+000036e0: 7273 2075 7365 6420 666f 7220 6e6f 6e2d  rs used for non-
+000036f0: 616e 616c 7974 6963 616c 2074 6572 6d20  analytical term 
+00003700: 636f 7272 6563 7469 6f6e 0a20 2020 2020  correction.     
+00003710: 2020 2020 2020 2027 626f 726e 273a 206e         'born': n
+00003720: 6461 7272 6179 0a20 2020 2020 2020 2020  darray.         
+00003730: 2020 2020 2020 2042 6f72 6e20 6566 6665         Born effe
+00003740: 6374 6976 6520 6368 6172 6765 730a 2020  ctive charges.  
+00003750: 2020 2020 2020 2020 2020 2020 2020 7368                sh
+00003760: 6170 653d 2870 7269 6d69 7469 7665 2063  ape=(primitive c
+00003770: 656c 6c20 6174 6f6d 732c 2033 2c20 3329  ell atoms, 3, 3)
+00003780: 2c20 6474 7970 653d 2764 6f75 626c 6527  , dtype='double'
+00003790: 2c20 6f72 6465 723d 2743 270a 2020 2020  , order='C'.    
+000037a0: 2020 2020 2020 2020 2766 6163 746f 7227          'factor'
+000037b0: 3a20 666c 6f61 740a 2020 2020 2020 2020  : float.        
+000037c0: 2020 2020 2020 2020 556e 6974 2063 6f6e          Unit con
+000037d0: 7665 7273 696f 6e20 6661 6374 6f72 0a20  version factor. 
+000037e0: 2020 2020 2020 2020 2020 2027 6469 656c             'diel
+000037f0: 6563 7472 6963 273a 206e 6461 7272 6179  ectric': ndarray
+00003800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003810: 2044 6965 6c65 6374 7269 6320 636f 6e73   Dielectric cons
+00003820: 7461 6e74 2074 656e 736f 720a 2020 2020  tant tensor.    
+00003830: 2020 2020 2020 2020 2020 2020 7368 6170              shap
+00003840: 653d 2833 2c20 3329 2c20 6474 7970 653d  e=(3, 3), dtype=
+00003850: 2764 6f75 626c 6527 2c20 6f72 6465 723d  'double', order=
+00003860: 2743 270a 0a20 2020 2020 2020 2022 2222  'C'..        """
+00003870: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00003880: 7365 6c66 2e5f 6e61 635f 7061 7261 6d73  self._nac_params
+00003890: 0a0a 2020 2020 406e 6163 5f70 6172 616d  ..    @nac_param
+000038a0: 732e 7365 7474 6572 0a20 2020 2064 6566  s.setter.    def
+000038b0: 206e 6163 5f70 6172 616d 7328 7365 6c66   nac_params(self
+000038c0: 2c20 6e61 635f 7061 7261 6d73 293a 0a20  , nac_params):. 
+000038d0: 2020 2020 2020 2073 656c 662e 5f6e 6163         self._nac
+000038e0: 5f70 6172 616d 7320 3d20 6e61 635f 7061  _params = nac_pa
+000038f0: 7261 6d73 0a20 2020 2020 2020 2069 6620  rams.        if 
+00003900: 7365 6c66 2e5f 696e 7465 7261 6374 696f  self._interactio
+00003910: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
+00003920: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003930: 5f69 6e69 745f 6479 6e61 6d69 6361 6c5f  _init_dynamical_
+00003940: 6d61 7472 6978 2829 0a0a 2020 2020 4070  matrix()..    @p
+00003950: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00003960: 6479 6e61 6d69 6361 6c5f 6d61 7472 6978  dynamical_matrix
+00003970: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00003980: 2222 2252 6574 7572 6e20 4479 6e61 6d69  """Return Dynami
+00003990: 6361 6c4d 6174 7269 7820 696e 7374 616e  calMatrix instan
+000039a0: 6365 2e0a 0a20 2020 2020 2020 2054 6869  ce...        Thi
+000039b0: 7320 6973 206e 6f74 2064 796e 616d 6963  s is not dynamic
+000039c0: 616c 206d 6174 7269 6365 7320 6275 7420  al matrices but 
+000039d0: 7468 6520 696e 7374 616e 6365 206f 6620  the instance of 
+000039e0: 4479 6e61 6d69 6361 6c4d 6174 7269 780a  DynamicalMatrix.
+000039f0: 2020 2020 2020 2020 636c 6173 732e 0a0a          class...
+00003a00: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00003a10: 2020 2020 6966 2073 656c 662e 5f69 6e74      if self._int
+00003a20: 6572 6163 7469 6f6e 2069 7320 4e6f 6e65  eraction is None
+00003a30: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00003a40: 7475 726e 204e 6f6e 650a 2020 2020 2020  turn None.      
+00003a50: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00003a60: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00003a70: 5f69 6e74 6572 6163 7469 6f6e 2e64 796e  _interaction.dyn
+00003a80: 616d 6963 616c 5f6d 6174 7269 780a 0a20  amical_matrix.. 
+00003a90: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00003aa0: 2064 6566 2070 7269 6d69 7469 7665 2873   def primitive(s
+00003ab0: 656c 6629 202d 3e20 5072 696d 6974 6976  elf) -> Primitiv
+00003ac0: 653a 0a20 2020 2020 2020 2022 2222 5265  e:.        """Re
+00003ad0: 7475 726e 2070 7269 6d69 7469 7665 2063  turn primitive c
+00003ae0: 656c 6c2e 0a0a 2020 2020 2020 2020 5072  ell...        Pr
+00003af0: 696d 6974 6976 650a 2020 2020 2020 2020  imitive.        
+00003b00: 2020 2020 5072 696d 6974 6976 6520 6365      Primitive ce
+00003b10: 6c6c 2e0a 0a20 2020 2020 2020 2022 2222  ll...        """
+00003b20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00003b30: 7365 6c66 2e5f 7072 696d 6974 6976 650a  self._primitive.
+00003b40: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+00003b50: 2020 2064 6566 2075 6e69 7463 656c 6c28     def unitcell(
+00003b60: 7365 6c66 2920 2d3e 2050 686f 6e6f 7079  self) -> Phonopy
+00003b70: 4174 6f6d 733a 0a20 2020 2020 2020 2022  Atoms:.        "
+00003b80: 2222 5265 7475 726e 2055 6e69 7420 6365  ""Return Unit ce
+00003b90: 6c6c 2e0a 0a20 2020 2020 2020 2050 686f  ll...        Pho
+00003ba0: 6e6f 7079 4174 6f6d 730a 2020 2020 2020  nopyAtoms.      
+00003bb0: 2020 2020 2020 556e 6974 2063 656c 6c2e        Unit cell.
+00003bc0: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00003bd0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00003be0: 662e 5f75 6e69 7463 656c 6c0a 0a20 2020  f._unitcell..   
+00003bf0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+00003c00: 6566 2073 7570 6572 6365 6c6c 2873 656c  ef supercell(sel
+00003c10: 6629 202d 3e20 5375 7065 7263 656c 6c3a  f) -> Supercell:
+00003c20: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+00003c30: 726e 2073 7570 6572 6365 6c6c 2e0a 0a20  rn supercell... 
+00003c40: 2020 2020 2020 2053 7570 6572 6365 6c6c         Supercell
+00003c50: 0a20 2020 2020 2020 2020 2020 2053 7570  .            Sup
+00003c60: 6572 6365 6c6c 2e0a 0a20 2020 2020 2020  ercell...       
+00003c70: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
+00003c80: 7572 6e20 7365 6c66 2e5f 7375 7065 7263  urn self._superc
+00003c90: 656c 6c0a 0a20 2020 2040 7072 6f70 6572  ell..    @proper
+00003ca0: 7479 0a20 2020 2064 6566 2070 686f 6e6f  ty.    def phono
+00003cb0: 6e5f 7375 7065 7263 656c 6c28 7365 6c66  n_supercell(self
+00003cc0: 2920 2d3e 2053 7570 6572 6365 6c6c 3a0a  ) -> Supercell:.
+00003cd0: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
+00003ce0: 6e20 7375 7065 7263 656c 6c20 666f 7220  n supercell for 
+00003cf0: 6663 322e 0a0a 2020 2020 2020 2020 5375  fc2...        Su
+00003d00: 7065 7263 656c 6c0a 2020 2020 2020 2020  percell.        
+00003d10: 2020 2020 5375 7065 7263 656c 6c20 666f      Supercell fo
+00003d20: 7220 6663 322e 0a0a 2020 2020 2020 2020  r fc2...        
+00003d30: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+00003d40: 726e 2073 656c 662e 5f70 686f 6e6f 6e5f  rn self._phonon_
+00003d50: 7375 7065 7263 656c 6c0a 0a20 2020 2040  supercell..    @
+00003d60: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00003d70: 2070 686f 6e6f 6e5f 7072 696d 6974 6976   phonon_primitiv
+00003d80: 6528 7365 6c66 2920 2d3e 2050 7269 6d69  e(self) -> Primi
+00003d90: 7469 7665 3a0a 2020 2020 2020 2020 2222  tive:.        ""
+00003da0: 2252 6574 7572 6e20 7072 696d 6974 6976  "Return primitiv
+00003db0: 6520 6365 6c6c 2066 6f72 2066 6332 2e0a  e cell for fc2..
+00003dc0: 0a20 2020 2020 2020 2050 7269 6d69 7469  .        Primiti
+00003dd0: 7665 0a20 2020 2020 2020 2020 2020 2050  ve.            P
+00003de0: 7269 6d69 7469 7665 2063 656c 6c20 666f  rimitive cell fo
+00003df0: 7220 6663 322e 2054 6869 7320 7368 6f75  r fc2. This shou
+00003e00: 6c64 2062 6520 7468 6520 7361 6d65 2061  ld be the same a
+00003e10: 7320 7468 6520 7072 696d 6974 6976 650a  s the primitive.
+00003e20: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
+00003e30: 2066 6f72 2066 6333 2c20 6275 7420 7468   for fc3, but th
+00003e40: 6973 2069 7320 6372 6561 7465 6420 6672  is is created fr
+00003e50: 6f6d 2073 7570 6572 6365 6c6c 2066 6f72  om supercell for
+00003e60: 2066 6332 2061 6e64 0a20 2020 2020 2020   fc2 and.       
+00003e70: 2020 2020 2063 616e 2062 6520 6e6f 7420       can be not 
+00003e80: 6e75 6d65 7269 6361 6c6c 7920 7065 7266  numerically perf
+00003e90: 6563 746c 7920 6964 656e 7469 6361 6c2e  ectly identical.
+00003ea0: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00003eb0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00003ec0: 662e 5f70 686f 6e6f 6e5f 7072 696d 6974  f._phonon_primit
+00003ed0: 6976 650a 0a20 2020 2040 7072 6f70 6572  ive..    @proper
+00003ee0: 7479 0a20 2020 2064 6566 2073 796d 6d65  ty.    def symme
+00003ef0: 7472 7928 7365 6c66 2920 2d3e 2053 796d  try(self) -> Sym
+00003f00: 6d65 7472 793a 0a20 2020 2020 2020 2022  metry:.        "
+00003f10: 2222 5265 7475 726e 2073 796d 6d65 7472  ""Return symmetr
+00003f20: 7920 6f66 2073 7570 6572 6365 6c6c 2e0a  y of supercell..
+00003f30: 0a20 2020 2020 2020 2053 796d 6d65 7472  .        Symmetr
+00003f40: 790a 2020 2020 2020 2020 2020 2020 5379  y.            Sy
+00003f50: 6d6d 6574 7279 206f 6620 7375 7065 7263  mmetry of superc
+00003f60: 656c 6c0a 0a20 2020 2020 2020 2022 2222  ell..        """
+00003f70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00003f80: 7365 6c66 2e5f 7379 6d6d 6574 7279 0a0a  self._symmetry..
+00003f90: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00003fa0: 2020 6465 6620 7072 696d 6974 6976 655f    def primitive_
+00003fb0: 7379 6d6d 6574 7279 2873 656c 6629 202d  symmetry(self) -
+00003fc0: 3e20 5379 6d6d 6574 7279 3a0a 2020 2020  > Symmetry:.    
+00003fd0: 2020 2020 2222 2252 6574 7572 6e20 7379      """Return sy
+00003fe0: 6d6d 6574 7279 206f 6620 7072 696d 6974  mmetry of primit
+00003ff0: 6976 6520 6365 6c6c 2e0a 0a20 2020 2020  ive cell...     
+00004000: 2020 2053 796d 6d65 7472 790a 2020 2020     Symmetry.    
+00004010: 2020 2020 2020 2020 5379 6d6d 6574 7279          Symmetry
+00004020: 206f 6620 7072 696d 6974 6976 6520 6365   of primitive ce
+00004030: 6c6c 2e0a 0a20 2020 2020 2020 2022 2222  ll...        """
+00004040: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00004050: 7365 6c66 2e5f 7072 696d 6974 6976 655f  self._primitive_
+00004060: 7379 6d6d 6574 7279 0a0a 2020 2020 4070  symmetry..    @p
+00004070: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00004080: 7068 6f6e 6f6e 5f73 7570 6572 6365 6c6c  phonon_supercell
+00004090: 5f73 796d 6d65 7472 7928 7365 6c66 2920  _symmetry(self) 
+000040a0: 2d3e 2053 796d 6d65 7472 793a 0a20 2020  -> Symmetry:.   
+000040b0: 2020 2020 2022 2222 5265 7475 726e 2073       """Return s
+000040c0: 796d 6d65 7472 7920 6f66 2073 7570 6572  ymmetry of super
+000040d0: 6365 6c6c 2066 6f72 2066 6332 2e0a 0a20  cell for fc2... 
+000040e0: 2020 2020 2020 2053 796d 6d65 7472 790a         Symmetry.
+000040f0: 2020 2020 2020 2020 2020 2020 5379 6d6d              Symm
+00004100: 6574 7279 206f 6620 7375 7065 7263 656c  etry of supercel
+00004110: 6c20 666f 7220 6663 3220 2870 686f 6e6f  l for fc2 (phono
+00004120: 6e5f 7375 7065 7263 656c 6c29 2e0a 0a20  n_supercell)... 
+00004130: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00004140: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00004150: 7068 6f6e 6f6e 5f73 7570 6572 6365 6c6c  phonon_supercell
+00004160: 5f73 796d 6d65 7472 790a 0a20 2020 2040  _symmetry..    @
+00004170: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00004180: 2073 7570 6572 6365 6c6c 5f6d 6174 7269   supercell_matri
+00004190: 7828 7365 6c66 293a 0a20 2020 2020 2020  x(self):.       
+000041a0: 2022 2222 5265 7475 726e 2074 7261 6e73   """Return trans
+000041b0: 666f 726d 6174 696f 6e20 6d61 7472 6978  formation matrix
+000041c0: 2074 6f20 7375 7065 7263 656c 6c20 6365   to supercell ce
+000041d0: 6c6c 2066 726f 6d20 756e 6974 2063 656c  ll from unit cel
+000041e0: 6c2e 0a0a 2020 2020 2020 2020 6e64 6172  l...        ndar
+000041f0: 7261 790a 2020 2020 2020 2020 2020 2020  ray.            
+00004200: 5375 7065 7263 656c 6c20 6d61 7472 6978  Supercell matrix
+00004210: 2077 6974 6820 7265 7370 6563 7420 746f   with respect to
+00004220: 2075 6e69 7420 6365 6c6c 2e0a 2020 2020   unit cell..    
+00004230: 2020 2020 2020 2020 7368 6170 653d 2833          shape=(3
+00004240: 2c20 3329 2c20 6474 7970 653d 2769 6e74  , 3), dtype='int
+00004250: 5f27 2c20 6f72 6465 723d 2743 270a 0a20  _', order='C'.. 
+00004260: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00004270: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00004280: 7375 7065 7263 656c 6c5f 6d61 7472 6978  supercell_matrix
+00004290: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+000042a0: 2020 2020 6465 6620 7068 6f6e 6f6e 5f73      def phonon_s
+000042b0: 7570 6572 6365 6c6c 5f6d 6174 7269 7828  upercell_matrix(
+000042c0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+000042d0: 2222 5265 7475 726e 2074 7261 6e73 666f  ""Return transfo
+000042e0: 726d 6174 696f 6e20 6d61 7472 6978 2074  rmation matrix t
+000042f0: 6f20 7068 6f6e 6f6e 2073 7570 6572 6365  o phonon superce
+00004300: 6c6c 2066 726f 6d20 756e 6974 2063 656c  ll from unit cel
+00004310: 6c2e 0a0a 2020 2020 2020 2020 6e64 6172  l...        ndar
+00004320: 7261 790a 2020 2020 2020 2020 2020 2020  ray.            
+00004330: 5375 7065 7263 656c 6c20 6d61 7472 6978  Supercell matrix
+00004340: 2077 6974 6820 7265 7370 6563 7420 746f   with respect to
+00004350: 2075 6e69 7420 6365 6c6c 2e0a 2020 2020   unit cell..    
+00004360: 2020 2020 2020 2020 7368 6170 653d 2833          shape=(3
+00004370: 2c20 3329 2c20 6474 7970 653d 2769 6e74  , 3), dtype='int
+00004380: 5f27 2c20 6f72 6465 723d 2743 270a 0a20  _', order='C'.. 
+00004390: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000043a0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+000043b0: 7068 6f6e 6f6e 5f73 7570 6572 6365 6c6c  phonon_supercell
+000043c0: 5f6d 6174 7269 780a 0a20 2020 2040 7072  _matrix..    @pr
+000043d0: 6f70 6572 7479 0a20 2020 2064 6566 2070  operty.    def p
+000043e0: 7269 6d69 7469 7665 5f6d 6174 7269 7828  rimitive_matrix(
+000043f0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00004400: 2222 5265 7475 726e 2074 7261 6e73 666f  ""Return transfo
+00004410: 726d 6174 696f 6e20 6d61 7472 6978 2074  rmation matrix t
+00004420: 6f20 7072 696d 6974 6976 6520 6365 6c6c  o primitive cell
+00004430: 2066 726f 6d20 756e 6974 2063 656c 6c2e   from unit cell.
+00004440: 0a0a 2020 2020 2020 2020 6e64 6172 7261  ..        ndarra
+00004450: 790a 2020 2020 2020 2020 2020 2020 5072  y.            Pr
+00004460: 696d 6974 6976 6520 6d61 7472 6978 2077  imitive matrix w
+00004470: 6974 6820 7265 7370 6563 7420 746f 2075  ith respect to u
+00004480: 6e69 7420 6365 6c6c 2e0a 2020 2020 2020  nit cell..      
+00004490: 2020 2020 2020 7368 6170 653d 2833 2c20        shape=(3, 
+000044a0: 3329 2c20 6474 7970 653d 2764 6f75 626c  3), dtype='doubl
+000044b0: 6527 2c20 6f72 6465 723d 2743 270a 0a20  e', order='C'.. 
+000044c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000044d0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+000044e0: 7072 696d 6974 6976 655f 6d61 7472 6978  primitive_matrix
+000044f0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00004500: 2020 2020 6465 6620 756e 6974 5f63 6f6e      def unit_con
+00004510: 7665 7273 696f 6e5f 6661 6374 6f72 2873  version_factor(s
+00004520: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00004530: 2252 6574 7572 6e20 7068 6f6e 6f6e 2066  "Return phonon f
+00004540: 7265 7175 656e 6379 2075 6e69 7420 636f  requency unit co
+00004550: 6e76 6572 7369 6f6e 2066 6163 746f 722e  nversion factor.
+00004560: 0a0a 2020 2020 2020 2020 666c 6f61 740a  ..        float.
+00004570: 2020 2020 2020 2020 2020 2020 5068 6f6e              Phon
+00004580: 6f6e 2066 7265 7175 656e 6379 2075 6e69  on frequency uni
+00004590: 7420 636f 6e76 6572 7369 6f6e 2066 6163  t conversion fac
+000045a0: 746f 722e 2054 6869 7320 6661 6374 6f72  tor. This factor
+000045b0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+000045c0: 7665 7274 7320 7371 7274 283c 666f 7263  verts sqrt(<forc
+000045d0: 653e 2f3c 6469 7374 616e 6365 3e2f 3c41  e>/<distance>/<A
+000045e0: 4d55 3e29 2f32 7069 2f31 6531 3220 746f  MU>)/2pi/1e12 to
+000045f0: 2054 487a 0a20 2020 2020 2020 2020 2020   THz.           
+00004600: 2028 6f72 6469 6e61 7279 2066 7265 7175   (ordinary frequ
+00004610: 656e 6379 292e 0a0a 2020 2020 2020 2020  ency)...        
+00004620: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+00004630: 726e 2073 656c 662e 5f66 7265 7175 656e  rn self._frequen
+00004640: 6379 5f66 6163 746f 725f 746f 5f54 487a  cy_factor_to_THz
+00004650: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00004660: 2020 2020 6465 6620 6461 7461 7365 7428      def dataset(
+00004670: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00004680: 2222 5365 7474 6572 2061 6e64 2067 6574  ""Setter and get
+00004690: 7465 7220 6f66 2064 6973 706c 6163 656d  ter of displacem
+000046a0: 656e 742d 666f 7263 6520 6461 7461 7365  ent-force datase
+000046b0: 742e 0a0a 2020 2020 2020 2020 6469 6374  t...        dict
+000046c0: 0a20 2020 2020 2020 2020 2020 2044 6973  .            Dis
+000046d0: 706c 6163 656d 656e 7473 2069 6e20 7375  placements in su
+000046e0: 7065 7263 656c 6c73 2e20 5468 6572 6520  percells. There 
+000046f0: 6172 6520 7477 6f20 7479 7065 7320 6f66  are two types of
+00004700: 2066 6f72 6d61 7473 2e0a 2020 2020 2020   formats..      
+00004710: 2020 2020 2020 5479 7065 2031 2e20 5477        Type 1. Tw
+00004720: 6f20 6174 6f6d 6963 2064 6973 706c 6163  o atomic displac
+00004730: 656d 656e 7420 696e 2065 6163 6820 7375  ement in each su
+00004740: 7065 7263 656c 6c3a 0a20 2020 2020 2020  percell:.       
+00004750: 2020 2020 2020 2020 207b 276e 6174 6f6d           {'natom
+00004760: 273a 206e 756d 6265 7220 6f66 2061 746f  ': number of ato
+00004770: 6d73 2069 6e20 7375 7065 7263 656c 6c2c  ms in supercell,
+00004780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004790: 2020 2766 6972 7374 5f61 746f 6d73 273a    'first_atoms':
+000047a0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+000047b0: 2020 2020 2020 7b27 6e75 6d62 6572 273a        {'number':
+000047c0: 2061 746f 6d20 696e 6465 7820 6f66 2066   atom index of f
+000047d0: 6972 7374 2064 6973 706c 6163 6564 2061  irst displaced a
+000047e0: 746f 6d2c 0a20 2020 2020 2020 2020 2020  tom,.           
+000047f0: 2020 2020 2020 2020 2027 6469 7370 6c61           'displa
+00004800: 6365 6d65 6e74 273a 2064 6973 706c 6163  cement': displac
+00004810: 656d 656e 7420 696e 2043 6172 7465 7369  ement in Cartesi
+00004820: 616e 2063 6f6f 7264 696e 6174 6573 2c0a  an coordinates,.
+00004830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004840: 2020 2020 2766 6f72 6365 7327 3a20 666f      'forces': fo
+00004850: 7263 6573 206f 6e20 6174 6f6d 7320 696e  rces on atoms in
+00004860: 2073 7570 6572 6365 6c6c 2c0a 2020 2020   supercell,.    
+00004870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004880: 2769 6427 3a20 6469 7370 6c61 6365 6d65  'id': displaceme
+00004890: 6e74 2069 6420 2831 2c20 322c 2e2e 2e2c  nt id (1, 2,...,
+000048a0: 6e5f 6669 7273 745f 6174 6f6d 7329 0a20  n_first_atoms). 
+000048b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048c0: 2020 2027 7365 636f 6e64 5f61 746f 6d73     'second_atoms
+000048d0: 273a 205b 0a20 2020 2020 2020 2020 2020  ': [.           
+000048e0: 2020 2020 2020 2020 2020 207b 276e 756d             {'num
+000048f0: 6265 7227 3a20 6174 6f6d 2069 6e64 6578  ber': atom index
+00004900: 206f 6620 7365 636f 6e64 2064 6973 706c   of second displ
+00004910: 6163 6564 2061 746f 6d2c 0a20 2020 2020  aced atom,.     
+00004920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004930: 2020 2764 6973 706c 6163 656d 656e 7427    'displacement'
+00004940: 3a20 6469 7370 6c61 6365 6d65 6e74 2069  : displacement i
+00004950: 6e20 4361 7274 6573 6961 6e20 636f 6f72  n Cartesian coor
+00004960: 6469 6e61 7465 737d 2c0a 2020 2020 2020  dinates},.      
+00004970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004980: 2027 666f 7263 6573 273a 2066 6f72 6365   'forces': force
+00004990: 7320 6f6e 2061 746f 6d73 2069 6e20 7375  s on atoms in su
+000049a0: 7065 7263 656c 6c2c 0a20 2020 2020 2020  percell,.       
+000049b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049c0: 2770 6169 725f 6469 7374 616e 6365 273a  'pair_distance':
+000049d0: 2064 6973 7461 6e63 6520 6265 7477 6565   distance betwee
+000049e0: 6e20 7061 6972 6564 2061 746f 6d73 2c0a  n paired atoms,.
+000049f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a00: 2020 2020 2020 2027 696e 636c 7564 6564         'included
+00004a10: 273a 2077 6974 6820 6375 746f 6666 2070  ': with cutoff p
+00004a20: 6169 7220 6469 7374 616e 6365 2069 6e20  air distance in 
+00004a30: 6469 7370 6c61 6365 6d65 6e74 0a20 2020  displacement.   
+00004a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a60: 7061 6972 2067 656e 6572 6174 696f 6e2c  pair generation,
+00004a70: 2074 6869 7320 696e 6469 6361 7465 7320   this indicates 
+00004a80: 6966 2074 6869 730a 2020 2020 2020 2020  if this.        
+00004a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004aa0: 2020 2020 2020 2020 2020 2070 6169 7220             pair 
+00004ab0: 6469 7370 6c61 6365 6d65 6e74 7320 6973  displacements is
+00004ac0: 2069 6e63 6c75 6465 6420 746f 2063 6f6d   included to com
+00004ad0: 7075 7465 0a20 2020 2020 2020 2020 2020  pute.           
+00004ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004af0: 2020 2020 2020 2020 6663 3320 6f72 206e          fc3 or n
+00004b00: 6f74 2c0a 2020 2020 2020 2020 2020 2020  ot,.            
+00004b10: 2020 2020 2020 2020 2020 2027 6964 273a             'id':
+00004b20: 2064 6973 706c 6163 656d 656e 7420 6964   displacement id
+00004b30: 2e20 286e 5f66 6972 7374 5f61 746f 6d73  . (n_first_atoms
+00004b40: 202b 2031 2c20 2e2e 2e29 0a20 2020 2020   + 1, ...).     
+00004b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b60: 202e 2e2e 205d 207d 2c20 2e2e 2e20 5d20   ... ] }, ... ] 
+00004b70: 7d0a 2020 2020 2020 2020 2020 2020 5479  }.            Ty
+00004b80: 7065 2032 2e20 416c 6c20 6174 6f6d 6963  pe 2. All atomic
+00004b90: 2064 6973 706c 6163 656d 656e 7473 2069   displacements i
+00004ba0: 6e20 6561 6368 2073 7570 6572 6365 6c6c  n each supercell
+00004bb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004bc0: 2020 7b27 6469 7370 6c61 6365 6d65 6e74    {'displacement
+00004bd0: 7327 3a20 6e64 6172 7261 792c 2064 7479  s': ndarray, dty
+00004be0: 7065 3d27 646f 7562 6c65 272c 206f 7264  pe='double', ord
+00004bf0: 6572 3d27 4327 2c0a 2020 2020 2020 2020  er='C',.        
+00004c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c10: 2020 2020 2020 2020 2020 7368 6170 653d            shape=
+00004c20: 2873 7570 6572 6365 6c6c 732c 2061 746f  (supercells, ato
+00004c30: 6d73 2069 6e20 7375 7065 7263 656c 6c2c  ms in supercell,
+00004c40: 2033 290a 2020 2020 2020 2020 2020 2020   3).            
+00004c50: 2020 2020 2027 666f 7263 6573 273a 206e       'forces': n
+00004c60: 6461 7272 6179 2c20 6474 7970 653d 2764  darray, dtype='d
+00004c70: 6f75 626c 6527 2c2c 206f 7264 6572 3d27  ouble',, order='
+00004c80: 4327 2c0a 2020 2020 2020 2020 2020 2020  C',.            
+00004c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ca0: 2020 2020 2020 7368 6170 653d 2873 7570        shape=(sup
+00004cb0: 6572 6365 6c6c 732c 2061 746f 6d73 2069  ercells, atoms i
+00004cc0: 6e20 7375 7065 7263 656c 6c2c 2033 297d  n supercell, 3)}
+00004cd0: 0a20 2020 2020 2020 2020 2020 2049 6e20  .            In 
+00004ce0: 7479 7065 2032 2c20 6469 7370 6c61 6365  type 2, displace
+00004cf0: 6d65 6e74 7320 616e 6420 666f 7263 6573  ments and forces
+00004d00: 2063 616e 2062 6520 6769 7665 6e20 6279   can be given by
+00004d10: 206e 756d 7079 2061 7272 6179 0a20 2020   numpy array.   
+00004d20: 2020 2020 2020 2020 2077 6974 6820 6469           with di
+00004d30: 6666 6572 656e 7420 7368 6170 6520 6275  fferent shape bu
+00004d40: 7420 7468 6174 2063 616e 2062 6520 7265  t that can be re
+00004d50: 7368 6170 6564 2074 6f0a 2020 2020 2020  shaped to.      
+00004d60: 2020 2020 2020 2873 7570 6572 6365 6c6c        (supercell
+00004d70: 732c 206e 6174 6f6d 2c20 3329 2e0a 0a20  s, natom, 3)... 
+00004d80: 2020 2020 2020 2020 2020 2049 6e20 6164             In ad
+00004d90: 6469 7469 6f6e 2c20 2764 7570 6c69 6361  dition, 'duplica
+00004da0: 7465 7327 2061 6e64 2027 6375 746f 6666  tes' and 'cutoff
+00004db0: 5f64 6973 7461 6e63 6527 2063 616e 2065  _distance' can e
+00004dc0: 7869 7374 2069 6e20 7468 6973 0a20 2020  xist in this.   
+00004dd0: 2020 2020 2020 2020 2064 6174 6173 6574           dataset
+00004de0: 2069 6e20 6469 7370 6c61 6365 6d65 6e74   in displacement
+00004df0: 2070 6169 7220 6765 6e65 7261 7469 6f6e   pair generation
+00004e00: 2e20 2764 7570 6c69 6361 7465 7327 2067  . 'duplicates' g
+00004e10: 6976 6573 0a20 2020 2020 2020 2020 2020  ives.           
+00004e20: 2064 7570 6c69 6361 7465 6420 7375 7065   duplicated supe
+00004e30: 7263 656c 6c20 6964 7320 6173 2070 6169  rcell ids as pai
+00004e40: 7273 2e0a 0a20 2020 2020 2020 2022 2222  rs...        """
+00004e50: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00004e60: 7365 6c66 2e5f 6461 7461 7365 740a 0a20  self._dataset.. 
+00004e70: 2020 2040 6461 7461 7365 742e 7365 7474     @dataset.sett
+00004e80: 6572 0a20 2020 2064 6566 2064 6174 6173  er.    def datas
+00004e90: 6574 2873 656c 662c 2064 6174 6173 6574  et(self, dataset
+00004ea0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00004eb0: 5f64 6174 6173 6574 203d 2064 6174 6173  _dataset = datas
+00004ec0: 6574 0a20 2020 2020 2020 2073 656c 662e  et.        self.
+00004ed0: 5f73 7570 6572 6365 6c6c 735f 7769 7468  _supercells_with
+00004ee0: 5f64 6973 706c 6163 656d 656e 7473 203d  _displacements =
+00004ef0: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
+00004f00: 6c66 2e5f 7068 6f6e 6f6e 5f73 7570 6572  lf._phonon_super
+00004f10: 6365 6c6c 735f 7769 7468 5f64 6973 706c  cells_with_displ
+00004f20: 6163 656d 656e 7473 203d 204e 6f6e 650a  acements = None.
+00004f30: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+00004f40: 2020 2064 6566 2070 686f 6e6f 6e5f 6461     def phonon_da
+00004f50: 7461 7365 7428 7365 6c66 293a 0a20 2020  taset(self):.   
+00004f60: 2020 2020 2022 2222 5365 7474 6572 2061       """Setter a
+00004f70: 6e64 2067 6574 7465 7220 6f66 2064 6973  nd getter of dis
+00004f80: 706c 6163 656d 656e 742d 666f 7263 6520  placement-force 
+00004f90: 6461 7461 7365 7420 666f 7220 6663 322e  dataset for fc2.
+00004fa0: 0a0a 2020 2020 2020 2020 6469 6374 0a20  ..        dict. 
+00004fb0: 2020 2020 2020 2020 2020 2044 6973 706c             Displ
+00004fc0: 6163 656d 656e 7473 2069 6e20 7375 7065  acements in supe
+00004fd0: 7263 656c 6c73 2e20 5468 6572 6520 6172  rcells. There ar
+00004fe0: 6520 7477 6f20 7479 7065 7320 6f66 2066  e two types of f
+00004ff0: 6f72 6d61 7473 2e0a 2020 2020 2020 2020  ormats..        
+00005000: 2020 2020 5479 7065 2031 2e20 5477 6f20      Type 1. Two 
+00005010: 6174 6f6d 6963 2064 6973 706c 6163 656d  atomic displacem
+00005020: 656e 7420 696e 2065 6163 6820 7375 7065  ent in each supe
+00005030: 7263 656c 6c3a 0a20 2020 2020 2020 2020  rcell:.         
+00005040: 2020 2020 2020 207b 276e 6174 6f6d 273a         {'natom':
+00005050: 206e 756d 6265 7220 6f66 2061 746f 6d73   number of atoms
+00005060: 2069 6e20 7375 7065 7263 656c 6c2c 0a20   in supercell,. 
+00005070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005080: 2766 6972 7374 5f61 746f 6d73 273a 205b  'first_atoms': [
+00005090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000050a0: 2020 2020 7b27 6e75 6d62 6572 273a 2061      {'number': a
+000050b0: 746f 6d20 696e 6465 7820 6f66 2066 6972  tom index of fir
+000050c0: 7374 2064 6973 706c 6163 6564 2061 746f  st displaced ato
+000050d0: 6d2c 0a20 2020 2020 2020 2020 2020 2020  m,.             
+000050e0: 2020 2020 2020 2027 6469 7370 6c61 6365         'displace
+000050f0: 6d65 6e74 273a 2064 6973 706c 6163 656d  ment': displacem
+00005100: 656e 7420 696e 2043 6172 7465 7369 616e  ent in Cartesian
+00005110: 2063 6f6f 7264 696e 6174 6573 2c0a 2020   coordinates,.  
+00005120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005130: 2020 2766 6f72 6365 7327 3a20 666f 7263    'forces': forc
+00005140: 6573 206f 6e20 6174 6f6d 7320 696e 2073  es on atoms in s
+00005150: 7570 6572 6365 6c6c 7d20 2e2e 2e20 5d7d  upercell} ... ]}
+00005160: 0a20 2020 2020 2020 2020 2020 2054 7970  .            Typ
+00005170: 6520 322e 2041 6c6c 2061 746f 6d69 6320  e 2. All atomic 
+00005180: 6469 7370 6c61 6365 6d65 6e74 7320 696e  displacements in
+00005190: 2065 6163 6820 7375 7065 7263 656c 6c3a   each supercell:
+000051a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000051b0: 207b 2764 6973 706c 6163 656d 656e 7473   {'displacements
+000051c0: 273a 206e 6461 7272 6179 2c20 6474 7970  ': ndarray, dtyp
+000051d0: 653d 2764 6f75 626c 6527 2c20 6f72 6465  e='double', orde
+000051e0: 723d 2743 272c 0a20 2020 2020 2020 2020  r='C',.         
+000051f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005200: 2020 2020 2020 2020 2073 6861 7065 3d28           shape=(
+00005210: 7375 7065 7263 656c 6c73 2c20 6174 6f6d  supercells, atom
+00005220: 7320 696e 2073 7570 6572 6365 6c6c 2c20  s in supercell, 
+00005230: 3329 0a20 2020 2020 2020 2020 2020 2020  3).             
+00005240: 2020 2020 2766 6f72 6365 7327 3a20 6e64      'forces': nd
+00005250: 6172 7261 792c 2064 7479 7065 3d27 646f  array, dtype='do
+00005260: 7562 6c65 272c 2c20 6f72 6465 723d 2743  uble',, order='C
+00005270: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00005280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005290: 2020 2020 2073 6861 7065 3d28 7375 7065       shape=(supe
+000052a0: 7263 656c 6c73 2c20 6174 6f6d 7320 696e  rcells, atoms in
+000052b0: 2073 7570 6572 6365 6c6c 2c20 3329 7d0a   supercell, 3)}.
+000052c0: 2020 2020 2020 2020 2020 2020 496e 2074              In t
+000052d0: 7970 6520 322c 2064 6973 706c 6163 656d  ype 2, displacem
+000052e0: 656e 7473 2061 6e64 2066 6f72 6365 7320  ents and forces 
+000052f0: 6361 6e20 6265 2067 6976 656e 2062 7920  can be given by 
+00005300: 6e75 6d70 7920 6172 7261 790a 2020 2020  numpy array.    
+00005310: 2020 2020 2020 2020 7769 7468 2064 6966          with dif
+00005320: 6665 7265 6e74 2073 6861 7065 2062 7574  ferent shape but
+00005330: 2074 6861 7420 6361 6e20 6265 2072 6573   that can be res
+00005340: 6861 7065 6420 746f 0a20 2020 2020 2020  haped to.       
+00005350: 2020 2020 2028 7375 7065 7263 656c 6c73       (supercells
+00005360: 2c20 6e61 746f 6d2c 2033 292e 0a0a 2020  , natom, 3)...  
+00005370: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00005380: 2020 7265 7475 726e 2073 656c 662e 5f70    return self._p
+00005390: 686f 6e6f 6e5f 6461 7461 7365 740a 0a20  honon_dataset.. 
+000053a0: 2020 2040 7068 6f6e 6f6e 5f64 6174 6173     @phonon_datas
+000053b0: 6574 2e73 6574 7465 720a 2020 2020 6465  et.setter.    de
+000053c0: 6620 7068 6f6e 6f6e 5f64 6174 6173 6574  f phonon_dataset
+000053d0: 2873 656c 662c 2064 6174 6173 6574 293a  (self, dataset):
+000053e0: 0a20 2020 2020 2020 2073 656c 662e 5f70  .        self._p
+000053f0: 686f 6e6f 6e5f 6461 7461 7365 7420 3d20  honon_dataset = 
+00005400: 6461 7461 7365 740a 0a20 2020 2040 7072  dataset..    @pr
+00005410: 6f70 6572 7479 0a20 2020 2064 6566 2062  operty.    def b
+00005420: 616e 645f 696e 6469 6365 7328 7365 6c66  and_indices(self
+00005430: 293a 0a20 2020 2020 2020 2022 2222 5365  ):.        """Se
+00005440: 7474 6572 2061 6e64 2067 6574 7465 7220  tter and getter 
+00005450: 6f66 2062 616e 6420 696e 6469 6365 732e  of band indices.
+00005460: 0a0a 2020 2020 2020 2020 6172 7261 795f  ..        array_
+00005470: 6c69 6b65 0a20 2020 2020 2020 2020 2020  like.           
+00005480: 204c 6973 7420 6f66 2062 616e 6420 696e   List of band in
+00005490: 6469 6365 7320 7370 6563 6966 6965 6420  dices specified 
+000054a0: 746f 2073 656c 6563 7420 7370 6563 6966  to select specif
+000054b0: 6963 2062 616e 6473 0a20 2020 2020 2020  ic bands.       
+000054c0: 2020 2020 2074 6f20 636f 6d70 7574 6572       to computer
+000054d0: 2070 682d 7068 2069 6e74 6572 6163 7469   ph-ph interacti
+000054e0: 6f6e 2072 656c 6174 6564 2070 726f 7065  on related prope
+000054f0: 7274 6965 732e 0a0a 2020 2020 2020 2020  rties...        
+00005500: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+00005510: 726e 2073 656c 662e 5f62 616e 645f 696e  rn self._band_in
+00005520: 6469 6365 730a 0a20 2020 2040 6261 6e64  dices..    @band
+00005530: 5f69 6e64 6963 6573 2e73 6574 7465 720a  _indices.setter.
+00005540: 2020 2020 6465 6620 6261 6e64 5f69 6e64      def band_ind
+00005550: 6963 6573 2873 656c 662c 2062 616e 645f  ices(self, band_
+00005560: 696e 6469 6365 7329 3a0a 2020 2020 2020  indices):.      
+00005570: 2020 7365 6c66 2e5f 7365 745f 6261 6e64    self._set_band
+00005580: 5f69 6e64 6963 6573 2862 616e 645f 696e  _indices(band_in
+00005590: 6469 6365 733d 6261 6e64 5f69 6e64 6963  dices=band_indic
+000055a0: 6573 290a 0a20 2020 2064 6566 205f 7365  es)..    def _se
+000055b0: 745f 6261 6e64 5f69 6e64 6963 6573 2873  t_band_indices(s
+000055c0: 656c 662c 2062 616e 645f 696e 6469 6365  elf, band_indice
+000055d0: 733d 4e6f 6e65 293a 0a20 2020 2020 2020  s=None):.       
+000055e0: 2069 6620 6261 6e64 5f69 6e64 6963 6573   if band_indices
+000055f0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00005600: 2020 2020 2020 6e75 6d5f 6261 6e64 203d        num_band =
+00005610: 206c 656e 2873 656c 662e 5f70 7269 6d69   len(self._primi
+00005620: 7469 7665 2920 2a20 330a 2020 2020 2020  tive) * 3.      
+00005630: 2020 2020 2020 7365 6c66 2e5f 6261 6e64        self._band
+00005640: 5f69 6e64 6963 6573 203d 205b 6e70 2e61  _indices = [np.a
+00005650: 7261 6e67 6528 6e75 6d5f 6261 6e64 2c20  range(num_band, 
+00005660: 6474 7970 653d 2269 6e74 5f22 295d 0a20  dtype="int_")]. 
+00005670: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00005680: 2020 2020 2020 2020 2073 656c 662e 5f62           self._b
+00005690: 616e 645f 696e 6469 6365 7320 3d20 6261  and_indices = ba
+000056a0: 6e64 5f69 6e64 6963 6573 0a20 2020 2020  nd_indices.     
+000056b0: 2020 2073 656c 662e 5f62 616e 645f 696e     self._band_in
+000056c0: 6469 6365 735f 666c 6174 7465 6e20 3d20  dices_flatten = 
+000056d0: 6e70 2e68 7374 6163 6b28 7365 6c66 2e5f  np.hstack(self._
+000056e0: 6261 6e64 5f69 6e64 6963 6573 292e 6173  band_indices).as
+000056f0: 7479 7065 2822 696e 745f 2229 0a0a 2020  type("int_")..  
+00005700: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+00005710: 6465 6620 6d61 7373 6573 2873 656c 6629  def masses(self)
+00005720: 3a0a 2020 2020 2020 2020 2222 2253 6574  :.        """Set
+00005730: 7465 7220 616e 6420 6765 7474 6572 206f  ter and getter o
+00005740: 6620 6174 6f6d 6963 206d 6173 7365 7320  f atomic masses 
+00005750: 6f66 2070 7269 6d69 7469 7665 2063 656c  of primitive cel
+00005760: 6c2e 2222 220a 2020 2020 2020 2020 7265  l.""".        re
+00005770: 7475 726e 2073 656c 662e 5f70 7269 6d69  turn self._primi
+00005780: 7469 7665 2e6d 6173 7365 730a 0a20 2020  tive.masses..   
+00005790: 2040 6d61 7373 6573 2e73 6574 7465 720a   @masses.setter.
+000057a0: 2020 2020 6465 6620 6d61 7373 6573 2873      def masses(s
+000057b0: 656c 662c 206d 6173 7365 7329 3a0a 2020  elf, masses):.  
+000057c0: 2020 2020 2020 6966 206d 6173 7365 7320        if masses 
+000057d0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+000057e0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+000057f0: 2020 2020 705f 6d61 7373 6573 203d 206e      p_masses = n
+00005800: 702e 6172 7261 7928 6d61 7373 6573 290a  p.array(masses).
+00005810: 2020 2020 2020 2020 7365 6c66 2e5f 7072          self._pr
+00005820: 696d 6974 6976 652e 6d61 7373 6573 203d  imitive.masses =
+00005830: 2070 5f6d 6173 7365 730a 2020 2020 2020   p_masses.      
+00005840: 2020 7032 705f 6d61 7020 3d20 7365 6c66    p2p_map = self
+00005850: 2e5f 7072 696d 6974 6976 652e 7032 705f  ._primitive.p2p_
+00005860: 6d61 700a 2020 2020 2020 2020 735f 6d61  map.        s_ma
+00005870: 7373 6573 203d 2070 5f6d 6173 7365 735b  sses = p_masses[
+00005880: 5b70 3270 5f6d 6170 5b78 5d20 666f 7220  [p2p_map[x] for 
+00005890: 7820 696e 2073 656c 662e 5f70 7269 6d69  x in self._primi
+000058a0: 7469 7665 2e73 3270 5f6d 6170 5d5d 0a20  tive.s2p_map]]. 
+000058b0: 2020 2020 2020 2073 656c 662e 5f73 7570         self._sup
+000058c0: 6572 6365 6c6c 2e6d 6173 7365 7320 3d20  ercell.masses = 
+000058d0: 735f 6d61 7373 6573 0a20 2020 2020 2020  s_masses.       
+000058e0: 2075 3273 5f6d 6170 203d 2073 656c 662e   u2s_map = self.
+000058f0: 5f73 7570 6572 6365 6c6c 2e75 3273 5f6d  _supercell.u2s_m
+00005900: 6170 0a20 2020 2020 2020 2075 5f6d 6173  ap.        u_mas
+00005910: 7365 7320 3d20 735f 6d61 7373 6573 5b75  ses = s_masses[u
+00005920: 3273 5f6d 6170 5d0a 2020 2020 2020 2020  2s_map].        
+00005930: 7365 6c66 2e5f 756e 6974 6365 6c6c 2e6d  self._unitcell.m
+00005940: 6173 7365 7320 3d20 755f 6d61 7373 6573  asses = u_masses
+00005950: 0a20 2020 2020 2020 2073 656c 662e 5f70  .        self._p
+00005960: 686f 6e6f 6e5f 7072 696d 6974 6976 652e  honon_primitive.
+00005970: 6d61 7373 6573 203d 2070 5f6d 6173 7365  masses = p_masse
+00005980: 730a 2020 2020 2020 2020 7032 705f 6d61  s.        p2p_ma
+00005990: 7020 3d20 7365 6c66 2e5f 7068 6f6e 6f6e  p = self._phonon
+000059a0: 5f70 7269 6d69 7469 7665 2e70 3270 5f6d  _primitive.p2p_m
+000059b0: 6170 0a20 2020 2020 2020 2073 5f6d 6173  ap.        s_mas
+000059c0: 7365 7320 3d20 705f 6d61 7373 6573 5b5b  ses = p_masses[[
+000059d0: 7032 705f 6d61 705b 785d 2066 6f72 2078  p2p_map[x] for x
+000059e0: 2069 6e20 7365 6c66 2e5f 7068 6f6e 6f6e   in self._phonon
+000059f0: 5f70 7269 6d69 7469 7665 2e73 3270 5f6d  _primitive.s2p_m
+00005a00: 6170 5d5d 0a20 2020 2020 2020 2073 656c  ap]].        sel
+00005a10: 662e 5f70 686f 6e6f 6e5f 7375 7065 7263  f._phonon_superc
+00005a20: 656c 6c2e 6d61 7373 6573 203d 2073 5f6d  ell.masses = s_m
+00005a30: 6173 7365 730a 0a20 2020 2040 7072 6f70  asses..    @prop
+00005a40: 6572 7479 0a20 2020 2064 6566 2073 7570  erty.    def sup
+00005a50: 6572 6365 6c6c 735f 7769 7468 5f64 6973  ercells_with_dis
+00005a60: 706c 6163 656d 656e 7473 2873 656c 6629  placements(self)
+00005a70: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
+00005a80: 7572 6e20 7375 7065 7263 656c 6c73 2077  urn supercells w
+00005a90: 6974 6820 6469 7370 6c61 6365 6d65 6e74  ith displacement
+00005aa0: 732e 0a0a 2020 2020 2020 2020 6c69 7374  s...        list
+00005ab0: 206f 6620 5068 6f6e 6f70 7941 746f 6d73   of PhonopyAtoms
+00005ac0: 0a20 2020 2020 2020 2020 2020 2053 7570  .            Sup
+00005ad0: 6572 6365 6c6c 7320 7769 7468 2064 6973  ercells with dis
+00005ae0: 706c 6163 656d 656e 7473 2067 656e 6572  placements gener
+00005af0: 6174 6564 2062 790a 2020 2020 2020 2020  ated by.        
+00005b00: 2020 2020 5068 6f6e 6f33 7079 2e67 656e      Phono3py.gen
+00005b10: 6572 6174 655f 6469 7370 6c61 6365 6d65  erate_displaceme
+00005b20: 6e74 732e 0a0a 2020 2020 2020 2020 2222  nts...        ""
+00005b30: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
+00005b40: 662e 5f73 7570 6572 6365 6c6c 735f 7769  f._supercells_wi
+00005b50: 7468 5f64 6973 706c 6163 656d 656e 7473  th_displacements
+00005b60: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00005b70: 2020 2020 2020 7365 6c66 2e5f 6275 696c        self._buil
+00005b80: 645f 7375 7065 7263 656c 6c73 5f77 6974  d_supercells_wit
+00005b90: 685f 6469 7370 6c61 6365 6d65 6e74 7328  h_displacements(
+00005ba0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00005bb0: 2073 656c 662e 5f73 7570 6572 6365 6c6c   self._supercell
+00005bc0: 735f 7769 7468 5f64 6973 706c 6163 656d  s_with_displacem
+00005bd0: 656e 7473 0a0a 2020 2020 4070 726f 7065  ents..    @prope
+00005be0: 7274 790a 2020 2020 6465 6620 7068 6f6e  rty.    def phon
+00005bf0: 6f6e 5f73 7570 6572 6365 6c6c 735f 7769  on_supercells_wi
+00005c00: 7468 5f64 6973 706c 6163 656d 656e 7473  th_displacements
+00005c10: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00005c20: 2222 2252 6574 7572 6e20 7375 7065 7263  """Return superc
+00005c30: 656c 6c73 2077 6974 6820 6469 7370 6c61  ells with displa
+00005c40: 6365 6d65 6e74 7320 666f 7220 6663 322e  cements for fc2.
+00005c50: 0a0a 2020 2020 2020 2020 6c69 7374 206f  ..        list o
+00005c60: 6620 5068 6f6e 6f70 7941 746f 6d73 0a20  f PhonopyAtoms. 
+00005c70: 2020 2020 2020 2020 2020 2053 7570 6572             Super
+00005c80: 6365 6c6c 7320 7769 7468 2064 6973 706c  cells with displ
+00005c90: 6163 656d 656e 7473 2067 656e 6572 6174  acements generat
+00005ca0: 6564 2062 790a 2020 2020 2020 2020 2020  ed by.          
+00005cb0: 2020 5068 6f6e 6f33 7079 2e67 656e 6572    Phono3py.gener
+00005cc0: 6174 655f 6469 7370 6c61 6365 6d65 6e74  ate_displacement
+00005cd0: 732e 0a0a 2020 2020 2020 2020 2222 220a  s...        """.
+00005ce0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00005cf0: 5f70 686f 6e6f 6e5f 7375 7065 7263 656c  _phonon_supercel
+00005d00: 6c73 5f77 6974 685f 6469 7370 6c61 6365  ls_with_displace
+00005d10: 6d65 6e74 7320 6973 204e 6f6e 653a 0a20  ments is None:. 
+00005d20: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00005d30: 6c66 2e5f 7068 6f6e 6f6e 5f64 6174 6173  lf._phonon_datas
+00005d40: 6574 2069 7320 6e6f 7420 4e6f 6e65 3a0a  et is not None:.
+00005d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d60: 7365 6c66 2e5f 7068 6f6e 6f6e 5f73 7570  self._phonon_sup
+00005d70: 6572 6365 6c6c 735f 7769 7468 5f64 6973  ercells_with_dis
+00005d80: 706c 6163 656d 656e 7473 203d 2028 0a20  placements = (. 
+00005d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005da0: 2020 2073 656c 662e 5f62 7569 6c64 5f70     self._build_p
+00005db0: 686f 6e6f 6e5f 7375 7065 7263 656c 6c73  honon_supercells
+00005dc0: 5f77 6974 685f 6469 7370 6c61 6365 6d65  _with_displaceme
+00005dd0: 6e74 7328 0a20 2020 2020 2020 2020 2020  nts(.           
+00005de0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00005df0: 662e 5f70 686f 6e6f 6e5f 7375 7065 7263  f._phonon_superc
+00005e00: 656c 6c2c 2073 656c 662e 5f70 686f 6e6f  ell, self._phono
+00005e10: 6e5f 6461 7461 7365 740a 2020 2020 2020  n_dataset.      
+00005e20: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00005e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e40: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00005e50: 2073 656c 662e 5f70 686f 6e6f 6e5f 7375   self._phonon_su
+00005e60: 7065 7263 656c 6c73 5f77 6974 685f 6469  percells_with_di
+00005e70: 7370 6c61 6365 6d65 6e74 730a 0a20 2020  splacements..   
+00005e80: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+00005e90: 6566 206d 6573 685f 6e75 6d62 6572 7328  ef mesh_numbers(
+00005ea0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00005eb0: 2222 5365 7474 6572 2061 6e64 2067 6574  ""Setter and get
+00005ec0: 7465 7220 6f66 2073 616d 706c 696e 6720  ter of sampling 
+00005ed0: 6d65 7368 206e 756d 6265 7273 2069 6e20  mesh numbers in 
+00005ee0: 7265 6369 7072 6f63 616c 2073 7061 6365  reciprocal space
+00005ef0: 2e22 2222 0a20 2020 2020 2020 2069 6620  .""".        if 
+00005f00: 7365 6c66 2e5f 627a 5f67 7269 6420 6973  self._bz_grid is
+00005f10: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00005f20: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
+00005f30: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00005f40: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00005f50: 7365 6c66 2e5f 627a 5f67 7269 642e 445f  self._bz_grid.D_
+00005f60: 6469 6167 0a0a 2020 2020 406d 6573 685f  diag..    @mesh_
+00005f70: 6e75 6d62 6572 732e 7365 7474 6572 0a20  numbers.setter. 
+00005f80: 2020 2064 6566 206d 6573 685f 6e75 6d62     def mesh_numb
+00005f90: 6572 7328 7365 6c66 2c20 6d65 7368 5f6e  ers(self, mesh_n
+00005fa0: 756d 6265 7273 3a20 556e 696f 6e5b 696e  umbers: Union[in
+00005fb0: 742c 2066 6c6f 6174 2c20 5365 7175 656e  t, float, Sequen
+00005fc0: 6365 2c20 6e70 2e6e 6461 7272 6179 5d29  ce, np.ndarray])
+00005fd0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00005fe0: 7365 745f 6d65 7368 5f6e 756d 6265 7273  set_mesh_numbers
+00005ff0: 286d 6573 685f 6e75 6d62 6572 7329 0a0a  (mesh_numbers)..
+00006000: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00006010: 2020 6465 6620 7468 6572 6d61 6c5f 636f    def thermal_co
+00006020: 6e64 7563 7469 7669 7479 2873 656c 6629  nductivity(self)
+00006030: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
+00006040: 7572 6e20 7468 6572 6d61 6c20 636f 6e64  urn thermal cond
+00006050: 7563 7469 7669 7479 2063 6c61 7373 2069  uctivity class i
+00006060: 6e73 7461 6e63 652e 2222 220a 2020 2020  nstance.""".    
+00006070: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00006080: 5f74 6865 726d 616c 5f63 6f6e 6475 6374  _thermal_conduct
+00006090: 6976 6974 790a 0a20 2020 2040 7072 6f70  ivity..    @prop
+000060a0: 6572 7479 0a20 2020 2064 6566 2064 6973  erty.    def dis
+000060b0: 706c 6163 656d 656e 7473 2873 656c 6629  placements(self)
+000060c0: 3a0a 2020 2020 2020 2020 2222 2253 6574  :.        """Set
+000060d0: 7465 7220 616e 6420 6765 7474 6572 2064  ter and getter d
+000060e0: 6973 706c 6163 656d 656e 7473 2069 6e20  isplacements in 
+000060f0: 7375 7065 7263 656c 6c73 2e0a 0a20 2020  supercells...   
+00006100: 2020 2020 2054 6865 7265 2061 7265 2074       There are t
+00006110: 776f 2074 7970 6573 206f 6620 6469 7370  wo types of disp
+00006120: 6c61 6365 6d65 6e74 2064 6174 6173 6574  lacement dataset
+00006130: 2e20 5365 6520 7468 6520 646f 6373 7472  . See the docstr
+00006140: 696e 670a 2020 2020 2020 2020 6f66 2064  ing.        of d
+00006150: 6174 6173 6574 2061 626f 7574 2074 7970  ataset about typ
+00006160: 6573 2031 2061 6e64 2032 2066 6f72 2074  es 1 and 2 for t
+00006170: 6865 2064 6973 706c 6163 656d 656e 7420  he displacement 
+00006180: 6461 7461 7365 7420 666f 726d 6174 732e  dataset formats.
+00006190: 0a20 2020 2020 2020 2044 6973 706c 6163  .        Displac
+000061a0: 656d 656e 7473 2073 6574 2072 6574 7572  ements set retur
+000061b0: 6e65 6420 6465 7065 6e64 7320 6f6e 2065  ned depends on e
+000061c0: 6974 6865 7220 7479 7065 2d31 206f 7220  ither type-1 or 
+000061d0: 7479 7065 2d32 2061 730a 2020 2020 2020  type-2 as.      
+000061e0: 2020 666f 6c6c 6f77 733a 0a0a 2020 2020    follows:..    
+000061f0: 2020 2020 5479 7065 2d31 2c20 4c69 7374      Type-1, List
+00006200: 206f 6620 6c69 7374 0a20 2020 2020 2020   of list.       
+00006210: 2020 2020 2054 6865 2069 6e74 6572 6e61       The interna
+00006220: 6c20 6c69 7374 2068 6173 2034 2065 6c65  l list has 4 ele
+00006230: 6d65 6e74 7320 7375 6368 2061 7320 5b33  ments such as [3
+00006240: 322c 2030 2e30 312c 2030 2e30 2c20 302e  2, 0.01, 0.0, 0.
+00006250: 305d 5d2e 0a20 2020 2020 2020 2020 2020  0]]..           
+00006260: 2054 6865 2066 6972 7374 2065 6c65 6d65   The first eleme
+00006270: 6e74 2069 7320 7468 6520 7375 7065 7263  nt is the superc
+00006280: 656c 6c20 6174 6f6d 2069 6e64 6578 2073  ell atom index s
+00006290: 7461 7274 696e 6720 7769 7468 2030 2e0a  tarting with 0..
+000062a0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+000062b0: 7265 6d61 696e 696e 6720 7468 7265 6520  remaining three 
+000062c0: 656c 656d 656e 7473 2067 6976 6520 7468  elements give th
+000062d0: 6520 6469 7370 6c61 6365 6d65 6e74 2069  e displacement i
+000062e0: 6e20 4361 7274 6573 6961 6e0a 2020 2020  n Cartesian.    
+000062f0: 2020 2020 2020 2020 636f 6f72 6469 6e61          coordina
+00006300: 7465 732e 0a20 2020 2020 2020 2054 7970  tes..        Typ
+00006310: 652d 322c 2061 7272 6179 5f6c 696b 650a  e-2, array_like.
+00006320: 2020 2020 2020 2020 2020 2020 4469 7370              Disp
+00006330: 6c61 6365 6d65 6e74 7320 6f66 2061 6c6c  lacements of all
+00006340: 2061 746f 6d73 206f 6620 616c 6c20 7375   atoms of all su
+00006350: 7065 7263 656c 6c73 2069 6e20 4361 7274  percells in Cart
+00006360: 6573 6961 6e0a 2020 2020 2020 2020 2020  esian.          
+00006370: 2020 636f 6f72 6469 6e61 7465 732e 0a20    coordinates.. 
+00006380: 2020 2020 2020 2020 2020 2073 6861 7065             shape
+00006390: 3d28 7375 7065 7263 656c 6c73 2c20 6e61  =(supercells, na
+000063a0: 746f 6d2c 2033 290a 2020 2020 2020 2020  tom, 3).        
+000063b0: 2020 2020 6474 7970 653d 2764 6f75 626c      dtype='doubl
+000063c0: 6527 0a0a 0a20 2020 2020 2020 2046 6f72  e'...        For
+000063d0: 2073 6574 7465 722c 206f 6e6c 7920 7479   setter, only ty
+000063e0: 7065 2d32 2064 6174 6173 6574 2066 6f72  pe-2 dataset for
+000063f0: 6d61 7420 6973 2061 6c6c 6f77 6564 2e0a  mat is allowed..
+00006400: 0a20 2020 2020 2020 2064 6973 706c 6163  .        displac
+00006410: 656d 656e 7473 203a 2061 7272 6179 5f6c  ements : array_l
+00006420: 696b 650a 2020 2020 2020 2020 2020 2020  ike.            
+00006430: 4174 6f6d 6963 2064 6973 706c 6163 656d  Atomic displacem
+00006440: 656e 7473 206f 6620 616c 6c20 6174 6f6d  ents of all atom
+00006450: 7320 6f66 2061 6c6c 2073 7570 6572 6365  s of all superce
+00006460: 6c6c 732e 0a20 2020 2020 2020 2020 2020  lls..           
+00006470: 204f 6e6c 7920 616c 6c20 6469 7370 6c61   Only all displa
+00006480: 6365 6d65 6e74 7320 696e 2065 6163 6820  cements in each 
+00006490: 7375 7065 7263 656c 6c20 6361 7365 2028  supercell case (
+000064a0: 7479 7065 2d32 2920 6973 0a20 2020 2020  type-2) is.     
+000064b0: 2020 2020 2020 2073 7570 706f 7274 6564         supported
+000064c0: 2e0a 2020 2020 2020 2020 2020 2020 7368  ..            sh
+000064d0: 6170 653d 2873 7570 6572 6365 6c6c 732c  ape=(supercells,
+000064e0: 206e 6174 6f6d 2c20 3329 2c20 6474 7970   natom, 3), dtyp
+000064f0: 653d 2764 6f75 626c 6527 2c20 6f72 6465  e='double', orde
+00006500: 723d 2743 270a 0a20 2020 2020 2020 2022  r='C'..        "
+00006510: 2222 0a20 2020 2020 2020 2064 6174 6173  "".        datas
+00006520: 6574 203d 2073 656c 662e 5f64 6174 6173  et = self._datas
+00006530: 6574 0a0a 2020 2020 2020 2020 6966 2022  et..        if "
+00006540: 6669 7273 745f 6174 6f6d 7322 2069 6e20  first_atoms" in 
+00006550: 6461 7461 7365 743a 0a20 2020 2020 2020  dataset:.       
+00006560: 2020 2020 206e 756d 5f73 6365 6c6c 7320       num_scells 
+00006570: 3d20 6c65 6e28 6461 7461 7365 745b 2266  = len(dataset["f
+00006580: 6972 7374 5f61 746f 6d73 225d 290a 2020  irst_atoms"]).  
+00006590: 2020 2020 2020 2020 2020 666f 7220 6469            for di
+000065a0: 7370 3120 696e 2064 6174 6173 6574 5b22  sp1 in dataset["
+000065b0: 6669 7273 745f 6174 6f6d 7322 5d3a 0a20  first_atoms"]:. 
+000065c0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000065d0: 756d 5f73 6365 6c6c 7320 2b3d 206c 656e  um_scells += len
+000065e0: 2864 6973 7031 5b22 7365 636f 6e64 5f61  (disp1["second_a
+000065f0: 746f 6d73 225d 290a 2020 2020 2020 2020  toms"]).        
+00006600: 2020 2020 6469 7370 6c61 6365 6d65 6e74      displacement
+00006610: 7320 3d20 6e70 2e7a 6572 6f73 280a 2020  s = np.zeros(.  
+00006620: 2020 2020 2020 2020 2020 2020 2020 286e                (n
+00006630: 756d 5f73 6365 6c6c 732c 2073 656c 662e  um_scells, self.
+00006640: 5f73 7570 6572 6365 6c6c 2e67 6574 5f6e  _supercell.get_n
+00006650: 756d 6265 725f 6f66 5f61 746f 6d73 2829  umber_of_atoms()
+00006660: 2c20 3329 2c0a 2020 2020 2020 2020 2020  , 3),.          
+00006670: 2020 2020 2020 6474 7970 653d 2264 6f75        dtype="dou
+00006680: 626c 6522 2c0a 2020 2020 2020 2020 2020  ble",.          
+00006690: 2020 2020 2020 6f72 6465 723d 2243 222c        order="C",
+000066a0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+000066b0: 2020 2020 2020 2020 2020 2069 203d 2030             i = 0
+000066c0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+000066d0: 2064 6973 7031 2069 6e20 6461 7461 7365   disp1 in datase
+000066e0: 745b 2266 6972 7374 5f61 746f 6d73 225d  t["first_atoms"]
+000066f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00006700: 2020 6469 7370 6c61 6365 6d65 6e74 735b    displacements[
+00006710: 692c 2064 6973 7031 5b22 6e75 6d62 6572  i, disp1["number
+00006720: 225d 5d20 3d20 6469 7370 315b 2264 6973  "]] = disp1["dis
+00006730: 706c 6163 656d 656e 7422 5d0a 2020 2020  placement"].    
+00006740: 2020 2020 2020 2020 2020 2020 6920 2b3d              i +=
+00006750: 2031 0a20 2020 2020 2020 2020 2020 2066   1.            f
+00006760: 6f72 2064 6973 7031 2069 6e20 6461 7461  or disp1 in data
+00006770: 7365 745b 2266 6972 7374 5f61 746f 6d73  set["first_atoms
+00006780: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
+00006790: 2020 2020 666f 7220 6469 7370 3220 696e      for disp2 in
+000067a0: 2064 6973 7031 5b22 7365 636f 6e64 5f61   disp1["second_a
+000067b0: 746f 6d73 225d 3a0a 2020 2020 2020 2020  toms"]:.        
+000067c0: 2020 2020 2020 2020 2020 2020 6469 7370              disp
+000067d0: 6c61 6365 6d65 6e74 735b 692c 2064 6973  lacements[i, dis
+000067e0: 7032 5b22 6e75 6d62 6572 225d 5d20 3d20  p2["number"]] = 
+000067f0: 6469 7370 325b 2264 6973 706c 6163 656d  disp2["displacem
+00006800: 656e 7422 5d0a 2020 2020 2020 2020 2020  ent"].          
+00006810: 2020 2020 2020 2020 2020 6920 2b3d 2031            i += 1
+00006820: 0a20 2020 2020 2020 2065 6c69 6620 2266  .        elif "f
+00006830: 6f72 6365 7322 2069 6e20 6461 7461 7365  orces" in datase
+00006840: 7420 6f72 2022 6469 7370 6c61 6365 6d65  t or "displaceme
+00006850: 6e74 7322 2069 6e20 6461 7461 7365 743a  nts" in dataset:
+00006860: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
+00006870: 706c 6163 656d 656e 7473 203d 2064 6174  placements = dat
+00006880: 6173 6574 5b22 6469 7370 6c61 6365 6d65  aset["displaceme
+00006890: 6e74 7322 5d0a 2020 2020 2020 2020 656c  nts"].        el
+000068a0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000068b0: 7261 6973 6520 5275 6e74 696d 6545 7272  raise RuntimeErr
+000068c0: 6f72 2822 6469 7370 6c61 6365 6d65 6e74  or("displacement
+000068d0: 2064 6174 6173 6574 2068 6173 2077 726f   dataset has wro
+000068e0: 6e67 2066 6f72 6d61 742e 2229 0a0a 2020  ng format.")..  
+000068f0: 2020 2020 2020 7265 7475 726e 2064 6973        return dis
+00006900: 706c 6163 656d 656e 7473 0a0a 2020 2020  placements..    
+00006910: 4064 6973 706c 6163 656d 656e 7473 2e73  @displacements.s
+00006920: 6574 7465 720a 2020 2020 6465 6620 6469  etter.    def di
+00006930: 7370 6c61 6365 6d65 6e74 7328 7365 6c66  splacements(self
+00006940: 2c20 6469 7370 6c61 6365 6d65 6e74 7329  , displacements)
+00006950: 3a0a 2020 2020 2020 2020 6469 7370 7320  :.        disps 
+00006960: 3d20 6e70 2e61 7272 6179 2864 6973 706c  = np.array(displ
+00006970: 6163 656d 656e 7473 2c20 6474 7970 653d  acements, dtype=
+00006980: 2264 6f75 626c 6522 2c20 6f72 6465 723d  "double", order=
+00006990: 2243 2229 0a20 2020 2020 2020 206e 6174  "C").        nat
+000069a0: 6f6d 203d 206c 656e 2873 656c 662e 5f73  om = len(self._s
+000069b0: 7570 6572 6365 6c6c 290a 2020 2020 2020  upercell).      
+000069c0: 2020 6966 2064 6973 7073 2e6e 6469 6d20    if disps.ndim 
+000069d0: 213d 2033 206f 7220 6469 7370 732e 7368  != 3 or disps.sh
+000069e0: 6170 655b 313a 5d20 213d 2028 6e61 746f  ape[1:] != (nato
+000069f0: 6d2c 2033 293a 0a20 2020 2020 2020 2020  m, 3):.         
+00006a00: 2020 2072 6169 7365 2052 756e 7469 6d65     raise Runtime
+00006a10: 4572 726f 7228 2241 7272 6179 2073 6861  Error("Array sha
+00006a20: 7065 206f 6620 6469 7370 6c61 6365 6d65  pe of displaceme
+00006a30: 6e74 7320 6973 2069 6e63 6f72 7265 6374  nts is incorrect
+00006a40: 2e22 290a 2020 2020 2020 2020 6966 2073  .").        if s
+00006a50: 656c 662e 5f64 6174 6173 6574 2069 7320  elf._dataset is 
+00006a60: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00006a70: 2020 7365 6c66 2e5f 6461 7461 7365 7420    self._dataset 
+00006a80: 3d20 7b7d 0a20 2020 2020 2020 2065 6c69  = {}.        eli
+00006a90: 6620 2266 6972 7374 5f61 746f 6d73 2220  f "first_atoms" 
+00006aa0: 696e 2073 656c 662e 5f64 6174 6173 6574  in self._dataset
+00006ab0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00006ac0: 6973 6520 5275 6e74 696d 6545 7272 6f72  ise RuntimeError
+00006ad0: 2822 4469 7370 6c61 6365 6d65 6e74 7320  ("Displacements 
+00006ae0: 6172 6520 696e 636f 6d70 6174 6962 6c65  are incompatible
+00006af0: 2077 6974 6820 6461 7461 7365 742e 2229   with dataset.")
+00006b00: 0a20 2020 2020 2020 2073 656c 662e 5f64  .        self._d
+00006b10: 6174 6173 6574 5b22 6469 7370 6c61 6365  ataset["displace
+00006b20: 6d65 6e74 7322 5d20 3d20 6469 7370 730a  ments"] = disps.
+00006b30: 2020 2020 2020 2020 7365 6c66 2e5f 7375          self._su
+00006b40: 7065 7263 656c 6c73 5f77 6974 685f 6469  percells_with_di
+00006b50: 7370 6c61 6365 6d65 6e74 7320 3d20 4e6f  splacements = No
+00006b60: 6e65 0a0a 2020 2020 4070 726f 7065 7274  ne..    @propert
+00006b70: 790a 2020 2020 6465 6620 666f 7263 6573  y.    def forces
+00006b80: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00006b90: 2222 2253 6574 7465 7220 616e 6420 6765  """Setter and ge
+00006ba0: 7474 6572 206f 6620 666f 7263 6573 2069  tter of forces i
+00006bb0: 6e20 6469 7370 6c61 6365 6d65 6e74 2064  n displacement d
+00006bc0: 6174 6173 6574 2e0a 0a20 2020 2020 2020  ataset...       
+00006bd0: 2041 2073 6574 206f 6620 6174 6f6d 6963   A set of atomic
+00006be0: 2066 6f72 6365 7320 696e 2064 6973 706c   forces in displ
+00006bf0: 6163 6564 2073 7570 6572 6365 6c6c 732e  aced supercells.
+00006c00: 2054 6865 206f 7264 6572 206f 660a 2020   The order of.  
+00006c10: 2020 2020 2020 6469 7370 6c61 6365 6420        displaced 
+00006c20: 7375 7065 7263 656c 6c73 2068 6173 2074  supercells has t
+00006c30: 6f20 6d61 7463 6820 7769 7468 2074 6861  o match with tha
+00006c40: 7420 696e 2064 6973 706c 6163 656d 656e  t in displacemen
+00006c50: 7420 6461 7461 7365 742e 0a20 2020 2020  t dataset..     
+00006c60: 2020 2073 6861 7065 3d28 6469 7370 6c61     shape=(displa
+00006c70: 6365 6420 7375 7065 7263 656c 6c73 2c20  ced supercells, 
+00006c80: 6174 6f6d 7320 696e 2073 7570 6572 6365  atoms in superce
+00006c90: 6c6c 2c20 3329 0a0a 2020 2020 2020 2020  ll, 3)..        
+00006ca0: 6765 7474 6572 203a 206e 6461 7272 6179  getter : ndarray
+00006cb0: 0a0a 2020 2020 2020 2020 7365 7474 6572  ..        setter
+00006cc0: 203a 2061 7272 6179 5f6c 696b 650a 2020   : array_like.  
+00006cd0: 2020 2020 2020 2020 2020 5468 6520 6f72            The or
+00006ce0: 6465 7220 6f66 2073 7570 6572 6365 6c6c  der of supercell
+00006cf0: 7320 7573 6564 2066 6f72 2063 616c 6375  s used for calcu
+00006d00: 6c61 7469 6e67 2066 6f72 6365 7320 6861  lating forces ha
+00006d10: 7320 746f 0a20 2020 2020 2020 2020 2020  s to.           
+00006d20: 2062 6520 7468 6520 7361 6d65 206f 7264   be the same ord
+00006d30: 6572 206f 6620 7375 7065 7263 656c 6c73  er of supercells
+00006d40: 5f77 6974 685f 6469 7370 6c61 6365 6d65  _with_displaceme
+00006d50: 6e74 732e 0a0a 2020 2020 2020 2020 2222  nts...        ""
+00006d60: 220a 2020 2020 2020 2020 6461 7461 7365  ".        datase
+00006d70: 7420 3d20 7365 6c66 2e5f 6461 7461 7365  t = self._datase
+00006d80: 740a 2020 2020 2020 2020 6966 2022 666f  t.        if "fo
+00006d90: 7263 6573 2220 696e 2064 6174 6173 6574  rces" in dataset
+00006da0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00006db0: 7475 726e 2064 6174 6173 6574 5b22 666f  turn dataset["fo
+00006dc0: 7263 6573 225d 0a20 2020 2020 2020 2065  rces"].        e
+00006dd0: 6c69 6620 2266 6972 7374 5f61 746f 6d73  lif "first_atoms
+00006de0: 2220 696e 2064 6174 6173 6574 3a0a 2020  " in dataset:.  
+00006df0: 2020 2020 2020 2020 2020 6e75 6d5f 7363            num_sc
+00006e00: 656c 6c73 203d 206c 656e 2864 6174 6173  ells = len(datas
+00006e10: 6574 5b22 6669 7273 745f 6174 6f6d 7322  et["first_atoms"
+00006e20: 5d29 0a20 2020 2020 2020 2020 2020 2066  ]).            f
+00006e30: 6f72 2064 6973 7031 2069 6e20 6461 7461  or disp1 in data
+00006e40: 7365 745b 2266 6972 7374 5f61 746f 6d73  set["first_atoms
+00006e50: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
+00006e60: 2020 2020 6e75 6d5f 7363 656c 6c73 202b      num_scells +
+00006e70: 3d20 6c65 6e28 6469 7370 315b 2273 6563  = len(disp1["sec
+00006e80: 6f6e 645f 6174 6f6d 7322 5d29 0a20 2020  ond_atoms"]).   
+00006e90: 2020 2020 2020 2020 2066 6f72 6365 7320           forces 
+00006ea0: 3d20 6e70 2e7a 6572 6f73 280a 2020 2020  = np.zeros(.    
+00006eb0: 2020 2020 2020 2020 2020 2020 286e 756d              (num
+00006ec0: 5f73 6365 6c6c 732c 2073 656c 662e 5f73  _scells, self._s
+00006ed0: 7570 6572 6365 6c6c 2e67 6574 5f6e 756d  upercell.get_num
+00006ee0: 6265 725f 6f66 5f61 746f 6d73 2829 2c20  ber_of_atoms(), 
+00006ef0: 3329 2c0a 2020 2020 2020 2020 2020 2020  3),.            
+00006f00: 2020 2020 6474 7970 653d 2264 6f75 626c      dtype="doubl
+00006f10: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00006f20: 2020 2020 6f72 6465 723d 2243 222c 0a20      order="C",. 
+00006f30: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00006f40: 2020 2020 2020 2020 2069 203d 2030 0a20           i = 0. 
+00006f50: 2020 2020 2020 2020 2020 2066 6f72 2064             for d
+00006f60: 6973 7031 2069 6e20 6461 7461 7365 745b  isp1 in dataset[
+00006f70: 2266 6972 7374 5f61 746f 6d73 225d 3a0a  "first_atoms"]:.
+00006f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f90: 666f 7263 6573 5b69 5d20 3d20 6469 7370  forces[i] = disp
+00006fa0: 315b 2266 6f72 6365 7322 5d0a 2020 2020  1["forces"].    
+00006fb0: 2020 2020 2020 2020 2020 2020 6920 2b3d              i +=
+00006fc0: 2031 0a20 2020 2020 2020 2020 2020 2066   1.            f
+00006fd0: 6f72 2064 6973 7031 2069 6e20 6461 7461  or disp1 in data
+00006fe0: 7365 745b 2266 6972 7374 5f61 746f 6d73  set["first_atoms
+00006ff0: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
+00007000: 2020 2020 666f 7220 6469 7370 3220 696e      for disp2 in
+00007010: 2064 6973 7031 5b22 7365 636f 6e64 5f61   disp1["second_a
+00007020: 746f 6d73 225d 3a0a 2020 2020 2020 2020  toms"]:.        
+00007030: 2020 2020 2020 2020 2020 2020 666f 7263              forc
+00007040: 6573 5b69 5d20 3d20 6469 7370 325b 2266  es[i] = disp2["f
+00007050: 6f72 6365 7322 5d0a 2020 2020 2020 2020  orces"].        
+00007060: 2020 2020 2020 2020 2020 2020 6920 2b3d              i +=
+00007070: 2031 0a20 2020 2020 2020 2020 2020 2072   1.            r
+00007080: 6574 7572 6e20 666f 7263 6573 0a20 2020  eturn forces.   
+00007090: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000070a0: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
+000070b0: 7469 6d65 4572 726f 7228 2264 6973 706c  timeError("displ
+000070c0: 6163 656d 656e 7420 6461 7461 7365 7420  acement dataset 
+000070d0: 6861 7320 7772 6f6e 6720 666f 726d 6174  has wrong format
+000070e0: 2e22 290a 0a20 2020 2040 666f 7263 6573  .")..    @forces
+000070f0: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
+00007100: 666f 7263 6573 2873 656c 662c 2066 6f72  forces(self, for
+00007110: 6365 735f 6663 3329 3a0a 2020 2020 2020  ces_fc3):.      
+00007120: 2020 666f 7263 6573 203d 206e 702e 6172    forces = np.ar
+00007130: 7261 7928 666f 7263 6573 5f66 6333 2c20  ray(forces_fc3, 
+00007140: 6474 7970 653d 2264 6f75 626c 6522 2c20  dtype="double", 
+00007150: 6f72 6465 723d 2243 2229 0a20 2020 2020  order="C").     
+00007160: 2020 2064 6174 6173 6574 203d 2073 656c     dataset = sel
+00007170: 662e 5f64 6174 6173 6574 0a20 2020 2020  f._dataset.     
+00007180: 2020 2069 6620 2266 6972 7374 5f61 746f     if "first_ato
+00007190: 6d73 2220 696e 2064 6174 6173 6574 3a0a  ms" in dataset:.
+000071a0: 2020 2020 2020 2020 2020 2020 6920 3d20              i = 
+000071b0: 300a 2020 2020 2020 2020 2020 2020 666f  0.            fo
+000071c0: 7220 6469 7370 3120 696e 2064 6174 6173  r disp1 in datas
+000071d0: 6574 5b22 6669 7273 745f 6174 6f6d 7322  et["first_atoms"
+000071e0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+000071f0: 2020 2064 6973 7031 5b22 666f 7263 6573     disp1["forces
+00007200: 225d 203d 2066 6f72 6365 735b 695d 0a20  "] = forces[i]. 
+00007210: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00007220: 202b 3d20 310a 2020 2020 2020 2020 2020   += 1.          
+00007230: 2020 666f 7220 6469 7370 3120 696e 2064    for disp1 in d
+00007240: 6174 6173 6574 5b22 6669 7273 745f 6174  ataset["first_at
+00007250: 6f6d 7322 5d3a 0a20 2020 2020 2020 2020  oms"]:.         
+00007260: 2020 2020 2020 2066 6f72 2064 6973 7032         for disp2
+00007270: 2069 6e20 6469 7370 315b 2273 6563 6f6e   in disp1["secon
+00007280: 645f 6174 6f6d 7322 5d3a 0a20 2020 2020  d_atoms"]:.     
+00007290: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000072a0: 6973 7032 5b22 666f 7263 6573 225d 203d  isp2["forces"] =
+000072b0: 2066 6f72 6365 735b 695d 0a20 2020 2020   forces[i].     
+000072c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000072d0: 202b 3d20 310a 2020 2020 2020 2020 656c   += 1.        el
+000072e0: 6966 2022 6469 7370 6c61 6365 6d65 6e74  if "displacement
+000072f0: 7322 2069 6e20 6461 7461 7365 7420 6f72  s" in dataset or
+00007300: 2022 666f 7263 6573 2220 696e 2064 6174   "forces" in dat
+00007310: 6173 6574 3a0a 2020 2020 2020 2020 2020  aset:.          
+00007320: 2020 6461 7461 7365 745b 2266 6f72 6365    dataset["force
+00007330: 7322 5d20 3d20 666f 7263 6573 0a0a 2020  s"] = forces..  
+00007340: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+00007350: 6465 6620 7068 6f6e 6f6e 5f64 6973 706c  def phonon_displ
+00007360: 6163 656d 656e 7473 2873 656c 6629 3a0a  acements(self):.
+00007370: 2020 2020 2020 2020 2222 2253 6574 7465          """Sette
+00007380: 7220 616e 6420 6765 7474 6572 206f 6620  r and getter of 
+00007390: 6469 7370 6c61 6365 6d65 6e74 7320 696e  displacements in
+000073a0: 2073 7570 6572 6365 6c6c 7320 666f 7220   supercells for 
+000073b0: 6663 322e 0a0a 2020 2020 2020 2020 5468  fc2...        Th
+000073c0: 6572 6520 6172 6520 7477 6f20 7479 7065  ere are two type
+000073d0: 7320 6f66 2064 6973 706c 6163 656d 656e  s of displacemen
+000073e0: 7420 6461 7461 7365 742e 2053 6565 2074  t dataset. See t
+000073f0: 6865 2064 6f63 7374 7269 6e67 0a20 2020  he docstring.   
+00007400: 2020 2020 206f 6620 6461 7461 7365 7420       of dataset 
+00007410: 6162 6f75 7420 7479 7065 7320 3120 616e  about types 1 an
+00007420: 6420 3220 666f 7220 7468 6520 6469 7370  d 2 for the disp
+00007430: 6c61 6365 6d65 6e74 2064 6174 6173 6574  lacement dataset
+00007440: 2066 6f72 6d61 7473 2e0a 2020 2020 2020   formats..      
+00007450: 2020 4469 7370 6c61 6365 6d65 6e74 7320    Displacements 
+00007460: 7365 7420 7265 7475 726e 6564 2064 6570  set returned dep
+00007470: 656e 6473 206f 6e20 6569 7468 6572 2074  ends on either t
+00007480: 7970 652d 3120 6f72 2074 7970 652d 3220  ype-1 or type-2 
+00007490: 6173 0a20 2020 2020 2020 2066 6f6c 6c6f  as.        follo
+000074a0: 7773 3a0a 0a20 2020 2020 2020 2054 7970  ws:..        Typ
+000074b0: 652d 312c 204c 6973 7420 6f66 206c 6973  e-1, List of lis
+000074c0: 740a 2020 2020 2020 2020 2020 2020 5468  t.            Th
+000074d0: 6520 696e 7465 726e 616c 206c 6973 7420  e internal list 
+000074e0: 6861 7320 3420 656c 656d 656e 7473 2073  has 4 elements s
+000074f0: 7563 6820 6173 205b 3332 2c20 302e 3031  uch as [32, 0.01
+00007500: 2c20 302e 302c 2030 2e30 5d5d 2e0a 2020  , 0.0, 0.0]]..  
+00007510: 2020 2020 2020 2020 2020 5468 6520 6669            The fi
+00007520: 7273 7420 656c 656d 656e 7420 6973 2074  rst element is t
+00007530: 6865 2073 7570 6572 6365 6c6c 2061 746f  he supercell ato
+00007540: 6d20 696e 6465 7820 7374 6172 7469 6e67  m index starting
+00007550: 2077 6974 6820 302e 0a20 2020 2020 2020   with 0..       
+00007560: 2020 2020 2054 6865 2072 656d 6169 6e69       The remaini
+00007570: 6e67 2074 6872 6565 2065 6c65 6d65 6e74  ng three element
+00007580: 7320 6769 7665 2074 6865 2064 6973 706c  s give the displ
+00007590: 6163 656d 656e 7420 696e 2043 6172 7465  acement in Carte
+000075a0: 7369 616e 0a20 2020 2020 2020 2020 2020  sian.           
+000075b0: 2063 6f6f 7264 696e 6174 6573 2e0a 2020   coordinates..  
+000075c0: 2020 2020 2020 5479 7065 2d32 2c20 6172        Type-2, ar
+000075d0: 7261 795f 6c69 6b65 0a20 2020 2020 2020  ray_like.       
+000075e0: 2020 2020 2044 6973 706c 6163 656d 656e       Displacemen
+000075f0: 7473 206f 6620 616c 6c20 6174 6f6d 7320  ts of all atoms 
+00007600: 6f66 2061 6c6c 2073 7570 6572 6365 6c6c  of all supercell
+00007610: 7320 696e 2043 6172 7465 7369 616e 0a20  s in Cartesian. 
+00007620: 2020 2020 2020 2020 2020 2063 6f6f 7264             coord
+00007630: 696e 6174 6573 2e0a 2020 2020 2020 2020  inates..        
+00007640: 2020 2020 7368 6170 653d 2873 7570 6572      shape=(super
+00007650: 6365 6c6c 732c 206e 6174 6f6d 2c20 3329  cells, natom, 3)
+00007660: 0a20 2020 2020 2020 2020 2020 2064 7479  .            dty
+00007670: 7065 3d27 646f 7562 6c65 270a 0a0a 2020  pe='double'...  
+00007680: 2020 2020 2020 466f 7220 7365 7474 6572        For setter
+00007690: 2c20 6f6e 6c79 2074 7970 652d 3220 6461  , only type-2 da
+000076a0: 7461 7365 7420 666f 726d 6174 2069 7320  taset format is 
+000076b0: 616c 6c6f 7765 642e 0a0a 2020 2020 2020  allowed...      
+000076c0: 2020 6469 7370 6c61 6365 6d65 6e74 7320    displacements 
+000076d0: 3a20 6172 7261 795f 6c69 6b65 0a20 2020  : array_like.   
+000076e0: 2020 2020 2020 2020 2041 746f 6d69 6320           Atomic 
+000076f0: 6469 7370 6c61 6365 6d65 6e74 7320 6f66  displacements of
+00007700: 2061 6c6c 2061 746f 6d73 206f 6620 616c   all atoms of al
+00007710: 6c20 7375 7065 7263 656c 6c73 2e0a 2020  l supercells..  
+00007720: 2020 2020 2020 2020 2020 4f6e 6c79 2061            Only a
+00007730: 6c6c 2064 6973 706c 6163 656d 656e 7473  ll displacements
+00007740: 2069 6e20 6561 6368 2073 7570 6572 6365   in each superce
+00007750: 6c6c 2063 6173 6520 2874 7970 652d 3229  ll case (type-2)
+00007760: 2069 730a 2020 2020 2020 2020 2020 2020   is.            
+00007770: 7375 7070 6f72 7465 642e 0a20 2020 2020  supported..     
+00007780: 2020 2020 2020 2073 6861 7065 3d28 7375         shape=(su
+00007790: 7065 7263 656c 6c73 2c20 6e61 746f 6d2c  percells, natom,
+000077a0: 2033 292c 2064 7479 7065 3d27 646f 7562   3), dtype='doub
+000077b0: 6c65 272c 206f 7264 6572 3d27 4327 0a0a  le', order='C'..
+000077c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000077d0: 2020 2020 6966 2073 656c 662e 5f70 686f      if self._pho
+000077e0: 6e6f 6e5f 7375 7065 7263 656c 6c5f 6d61  non_supercell_ma
+000077f0: 7472 6978 2069 7320 4e6f 6e65 3a0a 2020  trix is None:.  
+00007800: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00007810: 5275 6e74 696d 6545 7272 6f72 2822 7068  RuntimeError("ph
+00007820: 6f6e 6f6e 5f73 7570 6572 6365 6c6c 5f6d  onon_supercell_m
+00007830: 6174 7269 7820 6973 206e 6f74 2073 6574  atrix is not set
+00007840: 2e22 290a 0a20 2020 2020 2020 2064 6174  .")..        dat
+00007850: 6173 6574 203d 2073 656c 662e 5f70 686f  aset = self._pho
+00007860: 6e6f 6e5f 6461 7461 7365 740a 2020 2020  non_dataset.    
+00007870: 2020 2020 6966 2022 6669 7273 745f 6174      if "first_at
+00007880: 6f6d 7322 2069 6e20 6461 7461 7365 743a  oms" in dataset:
+00007890: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
+000078a0: 5f73 6365 6c6c 7320 3d20 6c65 6e28 6461  _scells = len(da
+000078b0: 7461 7365 745b 2266 6972 7374 5f61 746f  taset["first_ato
+000078c0: 6d73 225d 290a 2020 2020 2020 2020 2020  ms"]).          
+000078d0: 2020 6e61 746f 6d20 3d20 6c65 6e28 7365    natom = len(se
+000078e0: 6c66 2e5f 7068 6f6e 6f6e 5f73 7570 6572  lf._phonon_super
+000078f0: 6365 6c6c 290a 2020 2020 2020 2020 2020  cell).          
+00007900: 2020 6469 7370 6c61 6365 6d65 6e74 7320    displacements 
+00007910: 3d20 6e70 2e7a 6572 6f73 2828 6e75 6d5f  = np.zeros((num_
+00007920: 7363 656c 6c73 2c20 6e61 746f 6d2c 2033  scells, natom, 3
+00007930: 292c 2064 7479 7065 3d22 646f 7562 6c65  ), dtype="double
+00007940: 222c 206f 7264 6572 3d22 4322 290a 2020  ", order="C").  
+00007950: 2020 2020 2020 2020 2020 666f 7220 692c            for i,
+00007960: 2064 6973 7031 2069 6e20 656e 756d 6572   disp1 in enumer
+00007970: 6174 6528 6461 7461 7365 745b 2266 6972  ate(dataset["fir
+00007980: 7374 5f61 746f 6d73 225d 293a 0a20 2020  st_atoms"]):.   
+00007990: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+000079a0: 706c 6163 656d 656e 7473 5b69 2c20 6469  placements[i, di
+000079b0: 7370 315b 226e 756d 6265 7222 5d5d 203d  sp1["number"]] =
+000079c0: 2064 6973 7031 5b22 6469 7370 6c61 6365   disp1["displace
+000079d0: 6d65 6e74 225d 0a20 2020 2020 2020 2065  ment"].        e
+000079e0: 6c69 6620 2266 6f72 6365 7322 2069 6e20  lif "forces" in 
+000079f0: 6461 7461 7365 7420 6f72 2022 6469 7370  dataset or "disp
+00007a00: 6c61 6365 6d65 6e74 7322 2069 6e20 6461  lacements" in da
+00007a10: 7461 7365 743a 0a20 2020 2020 2020 2020  taset:.         
+00007a20: 2020 2064 6973 706c 6163 656d 656e 7473     displacements
+00007a30: 203d 2064 6174 6173 6574 5b22 6469 7370   = dataset["disp
+00007a40: 6c61 6365 6d65 6e74 7322 5d0a 2020 2020  lacements"].    
+00007a50: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00007a60: 2020 2020 2020 7261 6973 6520 5275 6e74        raise Runt
+00007a70: 696d 6545 7272 6f72 2822 6469 7370 6c61  imeError("displa
+00007a80: 6365 6d65 6e74 2064 6174 6173 6574 2068  cement dataset h
+00007a90: 6173 2077 726f 6e67 2066 6f72 6d61 742e  as wrong format.
+00007aa0: 2229 0a0a 2020 2020 2020 2020 7265 7475  ")..        retu
+00007ab0: 726e 2064 6973 706c 6163 656d 656e 7473  rn displacements
+00007ac0: 0a0a 2020 2020 4070 686f 6e6f 6e5f 6469  ..    @phonon_di
+00007ad0: 7370 6c61 6365 6d65 6e74 732e 7365 7474  splacements.sett
+00007ae0: 6572 0a20 2020 2064 6566 2070 686f 6e6f  er.    def phono
+00007af0: 6e5f 6469 7370 6c61 6365 6d65 6e74 7328  n_displacements(
+00007b00: 7365 6c66 2c20 6469 7370 6c61 6365 6d65  self, displaceme
+00007b10: 6e74 7329 3a0a 2020 2020 2020 2020 6966  nts):.        if
+00007b20: 2073 656c 662e 5f70 686f 6e6f 6e5f 7375   self._phonon_su
+00007b30: 7065 7263 656c 6c5f 6d61 7472 6978 2069  percell_matrix i
+00007b40: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00007b50: 2020 2020 7261 6973 6520 5275 6e74 696d      raise Runtim
+00007b60: 6545 7272 6f72 2822 7068 6f6e 6f6e 5f73  eError("phonon_s
+00007b70: 7570 6572 6365 6c6c 5f6d 6174 7269 7820  upercell_matrix 
+00007b80: 6973 206e 6f74 2073 6574 2e22 290a 0a20  is not set.").. 
+00007b90: 2020 2020 2020 2064 6973 7073 203d 206e         disps = n
+00007ba0: 702e 6172 7261 7928 6469 7370 6c61 6365  p.array(displace
+00007bb0: 6d65 6e74 732c 2064 7479 7065 3d22 646f  ments, dtype="do
+00007bc0: 7562 6c65 222c 206f 7264 6572 3d22 4322  uble", order="C"
+00007bd0: 290a 2020 2020 2020 2020 6e61 746f 6d20  ).        natom 
+00007be0: 3d20 6c65 6e28 7365 6c66 2e5f 7068 6f6e  = len(self._phon
+00007bf0: 6f6e 5f73 7570 6572 6365 6c6c 290a 2020  on_supercell).  
+00007c00: 2020 2020 2020 6966 2064 6973 7073 2e6e        if disps.n
+00007c10: 6469 6d20 213d 2033 206f 7220 6469 7370  dim != 3 or disp
+00007c20: 732e 7368 6170 655b 313a 5d20 213d 2028  s.shape[1:] != (
+00007c30: 6e61 746f 6d2c 2033 293a 0a20 2020 2020  natom, 3):.     
+00007c40: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
+00007c50: 7469 6d65 4572 726f 7228 2241 7272 6179  timeError("Array
+00007c60: 2073 6861 7065 206f 6620 6469 7370 6c61   shape of displa
+00007c70: 6365 6d65 6e74 7320 6973 2069 6e63 6f72  cements is incor
+00007c80: 7265 6374 2e22 290a 2020 2020 2020 2020  rect.").        
+00007c90: 6966 2073 656c 662e 5f70 686f 6e6f 6e5f  if self._phonon_
+00007ca0: 6461 7461 7365 7420 6973 204e 6f6e 653a  dataset is None:
+00007cb0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00007cc0: 662e 5f70 686f 6e6f 6e5f 6461 7461 7365  f._phonon_datase
+00007cd0: 7420 3d20 7b7d 0a20 2020 2020 2020 2065  t = {}.        e
+00007ce0: 6c69 6620 2266 6972 7374 5f61 746f 6d73  lif "first_atoms
+00007cf0: 2220 696e 2073 656c 662e 5f70 686f 6e6f  " in self._phono
+00007d00: 6e5f 6461 7461 7365 743a 0a20 2020 2020  n_dataset:.     
+00007d10: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
+00007d20: 7469 6d65 4572 726f 7228 2244 6973 706c  timeError("Displ
+00007d30: 6163 656d 656e 7473 2061 7265 2069 6e63  acements are inc
+00007d40: 6f6d 7061 7469 626c 6520 7769 7468 2064  ompatible with d
+00007d50: 6174 6173 6574 2e22 290a 0a20 2020 2020  ataset.")..     
+00007d60: 2020 2073 656c 662e 5f70 686f 6e6f 6e5f     self._phonon_
+00007d70: 6461 7461 7365 745b 2264 6973 706c 6163  dataset["displac
+00007d80: 656d 656e 7473 225d 203d 2064 6973 7073  ements"] = disps
+00007d90: 0a20 2020 2020 2020 2073 656c 662e 5f70  .        self._p
+00007da0: 686f 6e6f 6e5f 7375 7065 7263 656c 6c73  honon_supercells
+00007db0: 5f77 6974 685f 6469 7370 6c61 6365 6d65  _with_displaceme
+00007dc0: 6e74 7320 3d20 4e6f 6e65 0a0a 2020 2020  nts = None..    
+00007dd0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00007de0: 6620 7068 6f6e 6f6e 5f66 6f72 6365 7328  f phonon_forces(
+00007df0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00007e00: 2222 5365 7474 6572 2061 6e64 2067 6574  ""Setter and get
+00007e10: 7465 7220 6f66 2066 6f72 6365 7320 696e  ter of forces in
+00007e20: 2064 6973 706c 6163 656d 656e 7420 6461   displacement da
+00007e30: 7461 7365 7420 666f 7220 6663 322e 0a0a  taset for fc2...
+00007e40: 2020 2020 2020 2020 4120 7365 7420 6f66          A set of
+00007e50: 2061 746f 6d69 6320 666f 7263 6573 2069   atomic forces i
+00007e60: 6e20 6469 7370 6c61 6365 6420 7375 7065  n displaced supe
+00007e70: 7263 656c 6c73 2e20 5468 6520 6f72 6465  rcells. The orde
+00007e80: 7220 6f66 0a20 2020 2020 2020 2064 6973  r of.        dis
+00007e90: 706c 6163 6564 2073 7570 6572 6365 6c6c  placed supercell
+00007ea0: 7320 6861 7320 746f 206d 6174 6368 2077  s has to match w
+00007eb0: 6974 6820 7468 6174 2069 6e20 7068 6f6e  ith that in phon
+00007ec0: 6f6e 2064 6973 706c 6163 656d 656e 740a  on displacement.
+00007ed0: 2020 2020 2020 2020 6461 7461 7365 742e          dataset.
+00007ee0: 0a20 2020 2020 2020 2073 6861 7065 3d28  .        shape=(
+00007ef0: 6469 7370 6c61 6365 6420 7375 7065 7263  displaced superc
+00007f00: 656c 6c73 2c20 6174 6f6d 7320 696e 2073  ells, atoms in s
+00007f10: 7570 6572 6365 6c6c 2c20 3329 0a0a 2020  upercell, 3)..  
+00007f20: 2020 2020 2020 6765 7474 6572 203a 206e        getter : n
+00007f30: 6461 7272 6179 0a0a 2020 2020 2020 2020  darray..        
+00007f40: 7365 7474 6572 203a 2061 7272 6179 5f6c  setter : array_l
+00007f50: 696b 650a 2020 2020 2020 2020 2020 2020  ike.            
+00007f60: 5468 6520 6f72 6465 7220 6f66 2073 7570  The order of sup
+00007f70: 6572 6365 6c6c 7320 7573 6564 2066 6f72  ercells used for
+00007f80: 2063 616c 6375 6c61 7469 6e67 2066 6f72   calculating for
+00007f90: 6365 7320 6861 7320 746f 0a20 2020 2020  ces has to.     
+00007fa0: 2020 2020 2020 2062 6520 7468 6520 7361         be the sa
+00007fb0: 6d65 206f 7264 6572 206f 6620 7068 6f6e  me order of phon
+00007fc0: 6f6e 5f73 7570 6572 6365 6c6c 735f 7769  on_supercells_wi
+00007fd0: 7468 5f64 6973 706c 6163 656d 656e 7473  th_displacements
+00007fe0: 2e0a 0a20 2020 2020 2020 2022 2222 0a20  ...        """. 
+00007ff0: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+00008000: 7068 6f6e 6f6e 5f64 6174 6173 6574 2069  phonon_dataset i
+00008010: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00008020: 2020 2020 7261 6973 6520 5275 6e74 696d      raise Runtim
+00008030: 6545 7272 6f72 2822 7068 6f6e 6f6e 5f64  eError("phonon_d
+00008040: 6973 706c 6163 656d 656e 745f 6461 7461  isplacement_data
+00008050: 7365 7420 646f 6573 206e 6f74 2065 7869  set does not exi
+00008060: 7374 2e22 290a 0a20 2020 2020 2020 2064  st.")..        d
+00008070: 6174 6173 6574 203d 2073 656c 662e 5f70  ataset = self._p
+00008080: 686f 6e6f 6e5f 6461 7461 7365 740a 2020  honon_dataset.  
+00008090: 2020 2020 2020 6966 2022 666f 7263 6573        if "forces
+000080a0: 2220 696e 2064 6174 6173 6574 3a0a 2020  " in dataset:.  
+000080b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000080c0: 2064 6174 6173 6574 5b22 666f 7263 6573   dataset["forces
+000080d0: 225d 0a20 2020 2020 2020 2065 6c69 6620  "].        elif 
+000080e0: 2266 6972 7374 5f61 746f 6d73 2220 696e  "first_atoms" in
+000080f0: 2064 6174 6173 6574 3a0a 2020 2020 2020   dataset:.      
+00008100: 2020 2020 2020 6e75 6d5f 7363 656c 6c73        num_scells
+00008110: 203d 206c 656e 2864 6174 6173 6574 5b22   = len(dataset["
+00008120: 6669 7273 745f 6174 6f6d 7322 5d29 0a20  first_atoms"]). 
+00008130: 2020 2020 2020 2020 2020 2066 6f72 6365             force
+00008140: 7320 3d20 6e70 2e7a 6572 6f73 280a 2020  s = np.zeros(.  
+00008150: 2020 2020 2020 2020 2020 2020 2020 286e                (n
+00008160: 756d 5f73 6365 6c6c 732c 2073 656c 662e  um_scells, self.
+00008170: 5f70 686f 6e6f 6e5f 7375 7065 7263 656c  _phonon_supercel
+00008180: 6c2e 6765 745f 6e75 6d62 6572 5f6f 665f  l.get_number_of_
+00008190: 6174 6f6d 7328 292c 2033 292c 0a20 2020  atoms(), 3),.   
+000081a0: 2020 2020 2020 2020 2020 2020 2064 7479               dty
+000081b0: 7065 3d22 646f 7562 6c65 222c 0a20 2020  pe="double",.   
+000081c0: 2020 2020 2020 2020 2020 2020 206f 7264               ord
+000081d0: 6572 3d22 4322 2c0a 2020 2020 2020 2020  er="C",.        
+000081e0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+000081f0: 2020 666f 7220 692c 2064 6973 7031 2069    for i, disp1 i
+00008200: 6e20 656e 756d 6572 6174 6528 6461 7461  n enumerate(data
+00008210: 7365 745b 2266 6972 7374 5f61 746f 6d73  set["first_atoms
+00008220: 225d 293a 0a20 2020 2020 2020 2020 2020  "]):.           
+00008230: 2020 2020 2066 6f72 6365 735b 695d 203d       forces[i] =
+00008240: 2064 6973 7031 5b22 666f 7263 6573 225d   disp1["forces"]
+00008250: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00008260: 7572 6e20 666f 7263 6573 0a20 2020 2020  urn forces.     
+00008270: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00008280: 2020 2020 2072 6169 7365 2052 756e 7469       raise Runti
+00008290: 6d65 4572 726f 7228 2264 6973 706c 6163  meError("displac
+000082a0: 656d 656e 7420 6461 7461 7365 7420 6861  ement dataset ha
+000082b0: 7320 7772 6f6e 6720 666f 726d 6174 2e22  s wrong format."
+000082c0: 290a 0a20 2020 2040 7068 6f6e 6f6e 5f66  )..    @phonon_f
+000082d0: 6f72 6365 732e 7365 7474 6572 0a20 2020  orces.setter.   
+000082e0: 2064 6566 2070 686f 6e6f 6e5f 666f 7263   def phonon_forc
+000082f0: 6573 2873 656c 662c 2066 6f72 6365 735f  es(self, forces_
+00008300: 6663 3229 3a0a 2020 2020 2020 2020 6966  fc2):.        if
+00008310: 2073 656c 662e 5f70 686f 6e6f 6e5f 6461   self._phonon_da
+00008320: 7461 7365 7420 6973 204e 6f6e 653a 0a20  taset is None:. 
+00008330: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00008340: 2052 756e 7469 6d65 4572 726f 7228 2270   RuntimeError("p
+00008350: 686f 6e6f 6e5f 6469 7370 6c61 6365 6d65  honon_displaceme
+00008360: 6e74 5f64 6174 6173 6574 2064 6f65 7320  nt_dataset does 
+00008370: 6e6f 7420 6578 6973 742e 2229 0a0a 2020  not exist.")..  
+00008380: 2020 2020 2020 666f 7263 6573 203d 206e        forces = n
+00008390: 702e 6172 7261 7928 666f 7263 6573 5f66  p.array(forces_f
+000083a0: 6332 2c20 6474 7970 653d 2264 6f75 626c  c2, dtype="doubl
+000083b0: 6522 2c20 6f72 6465 723d 2243 2229 0a20  e", order="C"). 
+000083c0: 2020 2020 2020 2064 6174 6173 6574 203d         dataset =
+000083d0: 2073 656c 662e 5f70 686f 6e6f 6e5f 6461   self._phonon_da
+000083e0: 7461 7365 740a 2020 2020 2020 2020 6966  taset.        if
+000083f0: 2022 6669 7273 745f 6174 6f6d 7322 2069   "first_atoms" i
+00008400: 6e20 6461 7461 7365 743a 0a20 2020 2020  n dataset:.     
+00008410: 2020 2020 2020 2069 203d 2030 0a20 2020         i = 0.   
+00008420: 2020 2020 2020 2020 2066 6f72 2069 2c20           for i, 
+00008430: 6469 7370 3120 696e 2065 6e75 6d65 7261  disp1 in enumera
+00008440: 7465 2864 6174 6173 6574 5b22 6669 7273  te(dataset["firs
+00008450: 745f 6174 6f6d 7322 5d29 3a0a 2020 2020  t_atoms"]):.    
+00008460: 2020 2020 2020 2020 2020 2020 6469 7370              disp
+00008470: 315b 2266 6f72 6365 7322 5d20 3d20 666f  1["forces"] = fo
+00008480: 7263 6573 5b69 5d0a 2020 2020 2020 2020  rces[i].        
+00008490: 2020 2020 2020 2020 6920 2b3d 2031 0a20          i += 1. 
+000084a0: 2020 2020 2020 2065 6c69 6620 2264 6973         elif "dis
+000084b0: 706c 6163 656d 656e 7473 2220 696e 2064  placements" in d
+000084c0: 6174 6173 6574 206f 7220 2266 6f72 6365  ataset or "force
+000084d0: 7322 2069 6e20 6461 7461 7365 743a 0a20  s" in dataset:. 
+000084e0: 2020 2020 2020 2020 2020 2064 6174 6173             datas
+000084f0: 6574 5b22 666f 7263 6573 225d 203d 2066  et["forces"] = f
+00008500: 6f72 6365 730a 0a20 2020 2040 7072 6f70  orces..    @prop
+00008510: 6572 7479 0a20 2020 2064 6566 2070 6870  erty.    def php
+00008520: 685f 696e 7465 7261 6374 696f 6e28 7365  h_interaction(se
+00008530: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00008540: 5265 7475 726e 2049 6e74 6572 6163 7469  Return Interacti
+00008550: 6f6e 2069 6e73 7461 6e63 652e 2222 220a  on instance.""".
+00008560: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00008570: 656c 662e 5f69 6e74 6572 6163 7469 6f6e  elf._interaction
+00008580: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00008590: 2020 2020 6465 6620 6465 7461 696c 6564      def detailed
+000085a0: 5f67 616d 6d61 7328 7365 6c66 293a 0a20  _gammas(self):. 
+000085b0: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
+000085c0: 2064 6574 6169 6c65 6420 6761 6d6d 612e   detailed gamma.
+000085d0: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+000085e0: 726e 2073 656c 662e 5f64 6574 6169 6c65  rn self._detaile
+000085f0: 645f 6761 6d6d 6173 0a0a 2020 2020 4070  d_gammas..    @p
+00008600: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00008610: 6772 6964 2873 656c 6629 3a0a 2020 2020  grid(self):.    
+00008620: 2020 2020 2222 2252 6574 7572 6e20 4272      """Return Br
+00008630: 696c 6c6f 7569 6e20 7a6f 6e65 2067 7269  illouin zone gri
+00008640: 6420 696e 666f 726d 6174 696f 6e2e 0a0a  d information...
+00008650: 2020 2020 2020 2020 425a 4772 6964 0a20          BZGrid. 
+00008660: 2020 2020 2020 2020 2020 2041 6e20 696e             An in
+00008670: 7374 616e 6365 206f 6620 425a 4772 6964  stance of BZGrid
+00008680: 2075 7365 6420 666f 7220 656e 7469 7265   used for entire
+00008690: 2070 686f 6e6f 3370 7920 6361 6c63 756c   phono3py calcul
+000086a0: 6174 696f 6e2e 0a0a 2020 2020 2020 2020  ation...        
+000086b0: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+000086c0: 726e 2073 656c 662e 5f62 7a5f 6772 6964  rn self._bz_grid
+000086d0: 0a0a 2020 2020 6465 6620 696e 6974 5f70  ..    def init_p
+000086e0: 6870 685f 696e 7465 7261 6374 696f 6e28  hph_interaction(
+000086f0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00008700: 2020 2020 2020 206e 6163 5f71 5f64 6972         nac_q_dir
+00008710: 6563 7469 6f6e 3d4e 6f6e 652c 0a20 2020  ection=None,.   
+00008720: 2020 2020 2063 6f6e 7374 616e 745f 6176       constant_av
+00008730: 6572 6167 6564 5f69 6e74 6572 6163 7469  eraged_interacti
+00008740: 6f6e 3d4e 6f6e 652c 0a20 2020 2020 2020  on=None,.       
+00008750: 2066 7265 7175 656e 6379 5f73 6361 6c65   frequency_scale
+00008760: 5f66 6163 746f 723d 4e6f 6e65 2c0a 2020  _factor=None,.  
+00008770: 2020 2020 2020 7379 6d6d 6574 7269 7a65        symmetrize
+00008780: 5f66 6333 713a 2062 6f6f 6c20 3d20 4661  _fc3q: bool = Fa
+00008790: 6c73 652c 0a20 2020 2020 2020 206c 6170  lse,.        lap
+000087a0: 6163 6b5f 7a68 6565 765f 7570 6c6f 3d22  ack_zheev_uplo="
+000087b0: 4c22 2c0a 2020 2020 2020 2020 6f70 656e  L",.        open
+000087c0: 6d70 5f70 6572 5f74 7269 706c 6574 733d  mp_per_triplets=
+000087d0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+000087e0: 2020 2020 2022 2222 496e 6974 6961 6c69       """Initiali
+000087f0: 7a65 2070 682d 7068 2069 6e74 6572 6163  ze ph-ph interac
+00008800: 7469 6f6e 2063 616c 6375 6c61 7469 6f6e  tion calculation
+00008810: 2e0a 0a20 2020 2020 2020 2054 6869 7320  ...        This 
+00008820: 6d65 7468 6f64 2063 7265 6174 6573 2061  method creates a
+00008830: 6e20 696e 7374 616e 6365 206f 6620 496e  n instance of In
+00008840: 7465 7261 6374 696f 6e20 636c 6173 732c  teraction class,
+00008850: 2077 6869 6368 0a20 2020 2020 2020 2069   which.        i
+00008860: 7320 6e65 6365 7373 6172 7920 746f 2072  s necessary to r
+00008870: 756e 2070 682d 7068 2069 6e74 6572 6163  un ph-ph interac
+00008880: 7469 6f6e 2063 616c 6375 6c61 7469 6f6e  tion calculation
+00008890: 2e0a 2020 2020 2020 2020 5468 6520 696e  ..        The in
+000088a0: 7075 7420 6461 7461 2073 7563 6820 6173  put data such as
+000088b0: 2067 7269 6473 2c20 666f 7263 6520 636f   grids, force co
+000088c0: 6e73 7461 6e74 732c 2065 7463 2c20 6172  nstants, etc, ar
+000088d0: 650a 2020 2020 2020 2020 7374 6f72 6564  e.        stored
+000088e0: 2074 6f20 6265 2072 6561 6479 2066 6f72   to be ready for
+000088f0: 2074 6865 2063 616c 6375 6c61 7469 6f6e   the calculation
+00008900: 2e0a 0a20 2020 2020 2020 204e 6f74 650a  ...        Note.
+00008910: 2020 2020 2020 2020 2d2d 2d2d 0a20 2020          ----.   
+00008920: 2020 2020 2066 6333 2061 6e64 2066 6332       fc3 and fc2
+00008930: 2c20 616e 6420 6f70 7469 6f6e 616c 6c79  , and optionally
+00008940: 206e 6163 5f70 6172 616d 7320 6861 7665   nac_params have
+00008950: 2074 6f20 6265 2073 6574 2062 6566 6f72   to be set befor
+00008960: 6520 6361 6c6c 696e 670a 2020 2020 2020  e calling.      
+00008970: 2020 7468 6973 206d 6574 686f 642e 2066    this method. f
+00008980: 6333 2061 6e64 2066 6332 2063 616e 2062  c3 and fc2 can b
+00008990: 6520 6d61 6465 2065 6974 6865 7220 6672  e made either fr
+000089a0: 6f6d 2073 6574 7320 6f66 2066 6f72 6365  om sets of force
+000089b0: 730a 2020 2020 2020 2020 616e 6420 6469  s.        and di
+000089c0: 7370 6c61 6365 6d65 6e74 7320 6f66 2073  splacements of s
+000089d0: 7570 6572 6365 6c6c 7320 6f72 2062 6520  upercells or be 
+000089e0: 7365 7420 7369 6d70 6c79 2076 6961 2061  set simply via a
+000089f0: 7474 7269 6275 7465 732e 0a0a 2020 2020  ttributes...    
+00008a00: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00008a10: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00008a20: 2d0a 2020 2020 2020 2020 6e61 635f 715f  -.        nac_q_
+00008a30: 6469 7265 6374 696f 6e20 3a20 6172 7261  direction : arra
+00008a40: 795f 6c69 6b65 2c20 6f70 7469 6f6e 616c  y_like, optional
+00008a50: 0a20 2020 2020 2020 2020 2020 2044 6972  .            Dir
+00008a60: 6563 7469 6f6e 206f 6620 712d 7665 6374  ection of q-vect
+00008a70: 6f72 2077 6174 6368 696e 6720 6672 6f6d  or watching from
+00008a80: 2047 616d 6d61 2070 6f69 6e74 2075 7365   Gamma point use
+00008a90: 6420 666f 720a 2020 2020 2020 2020 2020  d for.          
+00008aa0: 2020 6e6f 6e2d 616e 616c 7974 6963 616c    non-analytical
+00008ab0: 2074 6572 6d20 636f 7272 6563 7469 6f6e   term correction
+00008ac0: 2e20 5468 6973 2069 7320 6566 6665 6374  . This is effect
+00008ad0: 6976 6520 6f6e 6c79 2061 7420 713d 300a  ive only at q=0.
+00008ae0: 2020 2020 2020 2020 2020 2020 2870 6879              (phy
+00008af0: 7369 6361 6c6c 7920 712d 3e30 292e 2054  sically q->0). T
+00008b00: 6865 2064 6972 6563 7469 6f6e 2069 7320  he direction is 
+00008b10: 6769 7665 6e20 696e 2063 7279 7374 616c  given in crystal
+00008b20: 6c6f 6772 6170 6869 630a 2020 2020 2020  lographic.      
+00008b30: 2020 2020 2020 2866 7261 6374 696f 6e61        (fractiona
+00008b40: 6c29 2063 6f6f 7264 696e 6174 6573 2e0a  l) coordinates..
+00008b50: 2020 2020 2020 2020 2020 2020 7368 6170              shap
+00008b60: 653d 2833 2c29 2c20 6474 7970 653d 2764  e=(3,), dtype='d
+00008b70: 6f75 626c 6527 2e0a 2020 2020 2020 2020  ouble'..        
+00008b80: 2020 2020 4465 6661 756c 7420 7661 6c75      Default valu
+00008b90: 6520 6973 204e 6f6e 652c 2077 6869 6368  e is None, which
+00008ba0: 206d 6561 6e73 2074 6869 7320 6665 6174   means this feat
+00008bb0: 7572 6520 6973 206e 6f74 2075 7365 642e  ure is not used.
+00008bc0: 0a20 2020 2020 2020 2063 6f6e 7374 616e  .        constan
+00008bd0: 745f 6176 6572 6167 6564 5f69 6e74 6572  t_averaged_inter
+00008be0: 6163 7469 6f6e 203a 2066 6c6f 6174 2c20  action : float, 
+00008bf0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+00008c00: 2020 2020 2050 682d 7068 2069 6e74 6572       Ph-ph inter
+00008c10: 6163 7469 6f6e 2073 7472 656e 6774 6820  action strength 
+00008c20: 6172 7261 7920 6973 2072 6570 6c61 6365  array is replace
+00008c30: 6420 6279 2061 2073 6361 6c61 7220 7661  d by a scalar va
+00008c40: 6c75 652e 0a20 2020 2020 2020 2020 2020  lue..           
+00008c50: 2044 6566 6175 6c74 2069 7320 4e6f 6e65   Default is None
+00008c60: 2c20 7768 6963 6820 6d65 616e 7320 7468  , which means th
+00008c70: 6973 2066 6561 7475 7265 2069 7320 6e6f  is feature is no
+00008c80: 7420 7573 6564 2e0a 2020 2020 2020 2020  t used..        
+00008c90: 6672 6571 7565 6e63 795f 7363 616c 655f  frequency_scale_
+00008ca0: 6661 6374 6f72 203a 2066 6c6f 6174 2c20  factor : float, 
+00008cb0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+00008cc0: 2020 2020 2041 6c6c 2070 686f 6e6f 6e20       All phonon 
+00008cd0: 6672 6571 7565 6e63 6573 2061 7265 2073  frequences are s
+00008ce0: 6361 6c65 6420 6279 2074 6869 7320 7661  caled by this va
+00008cf0: 6c75 652e 2044 6566 6175 6c74 2069 7320  lue. Default is 
+00008d00: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00008d10: 2020 7768 6963 6820 6d65 616e 7320 7068    which means ph
+00008d20: 6f6e 6f6e 2066 7265 7175 656e 6369 6573  onon frequencies
+00008d30: 2061 7265 206e 6f74 2073 6361 6c65 642e   are not scaled.
+00008d40: 0a20 2020 2020 2020 2073 796d 6d65 7472  .        symmetr
+00008d50: 697a 655f 6663 3371 203a 2062 6f6f 6c2c  ize_fc3q : bool,
+00008d60: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+00008d70: 2020 2020 2020 6663 3320 696e 2070 686f        fc3 in pho
+00008d80: 6e6f 6e20 7370 6163 6520 6973 2073 796d  non space is sym
+00008d90: 6d65 7472 697a 6564 2062 7920 7065 726d  metrized by perm
+00008da0: 7574 6174 696f 6e20 7379 6d6d 6574 7279  utation symmetry
+00008db0: 2e0a 2020 2020 2020 2020 2020 2020 4465  ..            De
+00008dc0: 6661 756c 7420 6973 2046 616c 7365 2e0a  fault is False..
+00008dd0: 2020 2020 2020 2020 6c61 7061 636b 5f7a          lapack_z
+00008de0: 6865 6576 5f75 706c 6f20 3a20 7374 722c  heev_uplo : str,
+00008df0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+00008e00: 2020 2020 2020 274c 2720 6f72 2027 5527        'L' or 'U'
+00008e10: 2e20 4465 6661 756c 7420 6973 2027 4c27  . Default is 'L'
+00008e20: 2e20 5468 6973 2069 7320 7061 7373 6564  . This is passed
+00008e30: 2074 6f20 4c41 5041 434b 207a 6865 6576   to LAPACK zheev
+00008e40: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
+00008e50: 6420 666f 7220 7068 6f6e 6f6e 2073 6f6c  d for phonon sol
+00008e60: 7665 722e 0a20 2020 2020 2020 206f 7065  ver..        ope
+00008e70: 6e6d 705f 7065 725f 7472 6970 6c65 7473  nmp_per_triplets
+00008e80: 203a 2062 6f6f 6c20 6f72 204e 6f6e 652c   : bool or None,
+00008e90: 206f 7074 696f 6e61 6c2c 2064 6566 6175   optional, defau
+00008ea0: 6c74 2069 7320 4e6f 6e65 0a20 2020 2020  lt is None.     
+00008eb0: 2020 2020 2020 204e 6f72 6d61 6c6c 7920         Normally 
+00008ec0: 7468 6973 2070 6172 616d 6574 6572 2073  this parameter s
+00008ed0: 686f 756c 6420 6e6f 7420 6265 2074 6f75  hould not be tou
+00008ee0: 6368 6564 2e0a 2020 2020 2020 2020 2020  ched..          
+00008ef0: 2020 5768 656e 2060 5472 7565 602c 2070    When `True`, p
+00008f00: 682d 7068 2069 6e74 6572 6163 7469 6f6e  h-ph interaction
+00008f10: 2073 7472 656e 6774 6820 6361 6c63 756c   strength calcul
+00008f20: 6174 696f 6e20 7275 6e73 2077 6974 680a  ation runs with.
+00008f30: 2020 2020 2020 2020 2020 2020 4f70 656e              Open
+00008f40: 4d50 2064 6973 7472 6962 7574 696f 6e20  MP distribution 
+00008f50: 6f76 6572 2074 7269 706c 6574 732c 2061  over triplets, a
+00008f60: 6e64 206f 7665 7220 6261 6e64 7320 7768  nd over bands wh
+00008f70: 656e 2060 4661 6c73 6560 2e0a 2020 2020  en `False`..    
+00008f80: 2020 2020 2020 2020 604e 6f6e 6560 2077          `None` w
+00008f90: 696c 6c20 6368 6f6f 7365 206f 6e65 206f  ill choose one o
+00008fa0: 6620 7468 656d 2061 7574 6f6d 6174 6963  f them automatic
+00008fb0: 616c 6c79 2e0a 0a20 2020 2020 2020 2022  ally...        "
+00008fc0: 2222 0a20 2020 2020 2020 2069 6620 7365  "".        if se
+00008fd0: 6c66 2e6d 6573 685f 6e75 6d62 6572 7320  lf.mesh_numbers 
+00008fe0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00008ff0: 2020 2020 206d 7367 203d 2022 5068 6f6e       msg = "Phon
+00009000: 6f33 7079 2e6d 6573 685f 6e75 6d62 6572  o3py.mesh_number
+00009010: 7320 6f66 2069 6e73 7461 6e63 6520 6861  s of instance ha
+00009020: 7320 746f 2062 6520 7365 742e 220a 2020  s to be set.".  
+00009030: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00009040: 5275 6e74 696d 6545 7272 6f72 286d 7367  RuntimeError(msg
+00009050: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
+00009060: 6c66 2e5f 6663 3220 6973 204e 6f6e 653a  lf._fc2 is None:
+00009070: 0a20 2020 2020 2020 2020 2020 206d 7367  .            msg
+00009080: 203d 2022 5068 6f6e 6f33 7079 2e66 6332   = "Phono3py.fc2
+00009090: 206f 6620 696e 7374 616e 6365 2069 7320   of instance is 
+000090a0: 6e6f 7420 666f 756e 642e 220a 2020 2020  not found.".    
+000090b0: 2020 2020 2020 2020 7261 6973 6520 5275          raise Ru
+000090c0: 6e74 696d 6545 7272 6f72 286d 7367 290a  ntimeError(msg).
+000090d0: 0a20 2020 2020 2020 2073 656c 662e 5f69  .        self._i
+000090e0: 6e74 6572 6163 7469 6f6e 203d 2049 6e74  nteraction = Int
+000090f0: 6572 6163 7469 6f6e 280a 2020 2020 2020  eraction(.      
+00009100: 2020 2020 2020 7365 6c66 2e5f 7072 696d        self._prim
+00009110: 6974 6976 652c 0a20 2020 2020 2020 2020  itive,.         
+00009120: 2020 2073 656c 662e 5f62 7a5f 6772 6964     self._bz_grid
+00009130: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
+00009140: 6c66 2e5f 7072 696d 6974 6976 655f 7379  lf._primitive_sy
+00009150: 6d6d 6574 7279 2c0a 2020 2020 2020 2020  mmetry,.        
+00009160: 2020 2020 6663 333d 7365 6c66 2e5f 6663      fc3=self._fc
+00009170: 332c 0a20 2020 2020 2020 2020 2020 2062  3,.            b
+00009180: 616e 645f 696e 6469 6365 733d 7365 6c66  and_indices=self
+00009190: 2e5f 6261 6e64 5f69 6e64 6963 6573 5f66  ._band_indices_f
+000091a0: 6c61 7474 656e 2c0a 2020 2020 2020 2020  latten,.        
+000091b0: 2020 2020 636f 6e73 7461 6e74 5f61 7665      constant_ave
+000091c0: 7261 6765 645f 696e 7465 7261 6374 696f  raged_interactio
+000091d0: 6e3d 636f 6e73 7461 6e74 5f61 7665 7261  n=constant_avera
+000091e0: 6765 645f 696e 7465 7261 6374 696f 6e2c  ged_interaction,
+000091f0: 0a20 2020 2020 2020 2020 2020 2066 7265  .            fre
+00009200: 7175 656e 6379 5f66 6163 746f 725f 746f  quency_factor_to
+00009210: 5f54 487a 3d73 656c 662e 5f66 7265 7175  _THz=self._frequ
+00009220: 656e 6379 5f66 6163 746f 725f 746f 5f54  ency_factor_to_T
+00009230: 487a 2c0a 2020 2020 2020 2020 2020 2020  Hz,.            
+00009240: 6672 6571 7565 6e63 795f 7363 616c 655f  frequency_scale_
+00009250: 6661 6374 6f72 3d66 7265 7175 656e 6379  factor=frequency
+00009260: 5f73 6361 6c65 5f66 6163 746f 722c 0a20  _scale_factor,. 
+00009270: 2020 2020 2020 2020 2020 2063 7574 6f66             cutof
+00009280: 665f 6672 6571 7565 6e63 793d 7365 6c66  f_frequency=self
+00009290: 2e5f 6375 746f 6666 5f66 7265 7175 656e  ._cutoff_frequen
+000092a0: 6379 2c0a 2020 2020 2020 2020 2020 2020  cy,.            
+000092b0: 6973 5f6d 6573 685f 7379 6d6d 6574 7279  is_mesh_symmetry
+000092c0: 3d73 656c 662e 5f69 735f 6d65 7368 5f73  =self._is_mesh_s
+000092d0: 796d 6d65 7472 792c 0a20 2020 2020 2020  ymmetry,.       
+000092e0: 2020 2020 2073 796d 6d65 7472 697a 655f       symmetrize_
+000092f0: 6663 3371 3d73 796d 6d65 7472 697a 655f  fc3q=symmetrize_
+00009300: 6663 3371 2c0a 2020 2020 2020 2020 2020  fc3q,.          
+00009310: 2020 6d61 6b65 5f72 305f 6176 6572 6167    make_r0_averag
+00009320: 653d 7365 6c66 2e5f 6d61 6b65 5f72 305f  e=self._make_r0_
+00009330: 6176 6572 6167 652c 0a20 2020 2020 2020  average,.       
+00009340: 2020 2020 206c 6170 6163 6b5f 7a68 6565       lapack_zhee
+00009350: 765f 7570 6c6f 3d6c 6170 6163 6b5f 7a68  v_uplo=lapack_zh
+00009360: 6565 765f 7570 6c6f 2c0a 2020 2020 2020  eev_uplo,.      
+00009370: 2020 2020 2020 6f70 656e 6d70 5f70 6572        openmp_per
+00009380: 5f74 7269 706c 6574 733d 6f70 656e 6d70  _triplets=openmp
+00009390: 5f70 6572 5f74 7269 706c 6574 732c 0a20  _per_triplets,. 
+000093a0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000093b0: 2073 656c 662e 5f69 6e74 6572 6163 7469   self._interacti
+000093c0: 6f6e 2e6e 6163 5f71 5f64 6972 6563 7469  on.nac_q_directi
+000093d0: 6f6e 203d 206e 6163 5f71 5f64 6972 6563  on = nac_q_direc
+000093e0: 7469 6f6e 0a20 2020 2020 2020 2073 656c  tion.        sel
+000093f0: 662e 5f69 6e69 745f 6479 6e61 6d69 6361  f._init_dynamica
+00009400: 6c5f 6d61 7472 6978 2829 0a0a 2020 2020  l_matrix()..    
+00009410: 6465 6620 7365 745f 7068 6f6e 6f6e 5f64  def set_phonon_d
+00009420: 6174 6128 7365 6c66 2c20 6672 6571 7565  ata(self, freque
+00009430: 6e63 6965 732c 2065 6967 656e 7665 6374  ncies, eigenvect
+00009440: 6f72 732c 2067 7269 645f 6164 6472 6573  ors, grid_addres
+00009450: 7329 3a0a 2020 2020 2020 2020 2222 2253  s):.        """S
+00009460: 6574 2070 686f 6e6f 6e20 6672 6571 7565  et phonon freque
+00009470: 6e63 6965 7320 616e 6420 6569 6765 6e76  ncies and eigenv
+00009480: 6563 746f 7273 2069 6e20 496e 7465 7261  ectors in Intera
+00009490: 6374 696f 6e20 696e 7374 616e 6365 2e0a  ction instance..
+000094a0: 0a20 2020 2020 2020 2048 6172 6d6f 6e69  .        Harmoni
+000094b0: 6320 7068 6f6e 6f6e 2069 6e66 6f72 6d61  c phonon informa
+000094c0: 7469 6f6e 2069 7320 7374 6f72 6564 2069  tion is stored i
+000094d0: 6e20 496e 7465 7261 6374 696f 6e20 696e  n Interaction in
+000094e0: 7374 616e 6365 2e20 466f 720a 2020 2020  stance. For.    
+000094f0: 2020 2020 6578 616d 706c 652c 2074 6869      example, thi
+00009500: 7320 696e 666f 726d 6174 696f 6e20 7374  s information st
+00009510: 6f72 6520 696e 2061 2066 696c 6520 6973  ore in a file is
+00009520: 2072 6561 6420 616e 6420 7061 7373 6564   read and passed
+00009530: 2074 6f0a 2020 2020 2020 2020 5068 6f6e   to.        Phon
+00009540: 6f33 7079 2069 6e73 7461 6e63 6520 6279  o3py instance by
+00009550: 2075 7369 6e67 2074 6869 7320 6d65 7468   using this meth
+00009560: 6f64 2e20 5468 6520 6772 6964 5f61 6464  od. The grid_add
+00009570: 7265 7373 2069 7320 7573 6564 0a20 2020  ress is used.   
+00009580: 2020 2020 2066 6f72 2074 6865 2063 6f6e       for the con
+00009590: 7369 7374 656e 6379 2063 6865 636b 2e0a  sistency check..
+000095a0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+000095b0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+000095c0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2066  ------.        f
+000095d0: 7265 7175 656e 6369 6573 203a 2061 7272  requencies : arr
+000095e0: 6179 5f6c 696b 650a 2020 2020 2020 2020  ay_like.        
+000095f0: 2020 2020 5068 6f6e 6f6e 2066 7265 7175      Phonon frequ
+00009600: 656e 6369 6573 2e0a 2020 2020 2020 2020  encies..        
+00009610: 2020 2020 7368 6170 653d 286e 756d 5f67      shape=(num_g
+00009620: 7269 645f 706f 696e 7473 2c20 6e75 6d5f  rid_points, num_
+00009630: 6261 6e64 292c 2064 7479 7065 3d27 646f  band), dtype='do
+00009640: 7562 6c65 272c 206f 7264 6572 3d27 4327  uble', order='C'
+00009650: 0a20 2020 2020 2020 2065 6967 656e 7665  .        eigenve
+00009660: 6374 6f72 7320 3a20 6172 7261 795f 6c69  ctors : array_li
+00009670: 6b65 0a20 2020 2020 2020 2020 2020 2050  ke.            P
+00009680: 686f 6e6f 6e20 6569 6765 6e76 6563 746f  honon eigenvecto
+00009690: 7273 0a20 2020 2020 2020 2020 2020 2073  rs.            s
+000096a0: 6861 7065 3d28 6e75 6d5f 6772 6964 5f70  hape=(num_grid_p
+000096b0: 6f69 6e74 732c 206e 756d 5f62 616e 642c  oints, num_band,
+000096c0: 206e 756d 5f62 616e 6429 0a20 2020 2020   num_band).     
+000096d0: 2020 2020 2020 2064 7479 7065 3d27 636f         dtype='co
+000096e0: 6d70 6c65 7831 3238 272c 206f 7264 6572  mplex128', order
+000096f0: 3d27 4327 0a20 2020 2020 2020 2067 7269  ='C'.        gri
+00009700: 645f 6164 6472 6573 7320 3a20 6172 7261  d_address : arra
+00009710: 795f 6c69 6b65 0a20 2020 2020 2020 2020  y_like.         
+00009720: 2020 2047 7269 6420 706f 696e 7420 6164     Grid point ad
+00009730: 6472 6573 7365 7320 6279 2069 6e74 6567  dresses by integ
+00009740: 6572 732e 2054 6865 2066 6972 7374 2064  ers. The first d
+00009750: 696d 656e 7369 6f6e 206d 6179 206e 6f74  imension may not
+00009760: 2062 650a 2020 2020 2020 2020 2020 2020   be.            
+00009770: 7072 6f64 286d 6573 6829 2062 6563 6175  prod(mesh) becau
+00009780: 7365 2069 7420 696e 636c 7564 6573 2042  se it includes B
+00009790: 7269 6c6c 6f75 696e 207a 6f6e 6520 626f  rillouin zone bo
+000097a0: 756e 6461 7279 2e20 5468 6520 6465 7461  undary. The deta
+000097b0: 696c 0a20 2020 2020 2020 2020 2020 2069  il.            i
+000097c0: 7320 666f 756e 6420 696e 2074 6865 2064  s found in the d
+000097d0: 6f63 7374 7269 6e67 206f 660a 2020 2020  ocstring of.    
+000097e0: 2020 2020 2020 2020 7068 6f6e 6f33 7079          phono3py
+000097f0: 2e70 686f 6e6f 6e33 2e74 7269 706c 6574  .phonon3.triplet
+00009800: 732e 6765 745f 7472 6970 6c65 7473 5f61  s.get_triplets_a
+00009810: 745f 712e 0a20 2020 2020 2020 2020 2020  t_q..           
+00009820: 2073 6861 7065 3d28 6e75 6d5f 6772 6964   shape=(num_grid
+00009830: 5f70 6f69 6e74 732c 2033 292c 2064 7479  _points, 3), dty
+00009840: 7065 3d69 6e74 0a0a 2020 2020 2020 2020  pe=int..        
+00009850: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
+00009860: 656c 662e 5f69 6e74 6572 6163 7469 6f6e  elf._interaction
+00009870: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00009880: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00009890: 696e 7465 7261 6374 696f 6e2e 7365 745f  interaction.set_
+000098a0: 7068 6f6e 6f6e 5f64 6174 6128 6672 6571  phonon_data(freq
+000098b0: 7565 6e63 6965 732c 2065 6967 656e 7665  uencies, eigenve
+000098c0: 6374 6f72 732c 2067 7269 645f 6164 6472  ctors, grid_addr
+000098d0: 6573 7329 0a0a 2020 2020 6465 6620 6765  ess)..    def ge
+000098e0: 745f 7068 6f6e 6f6e 5f64 6174 6128 7365  t_phonon_data(se
+000098f0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00009900: 4765 7420 7068 6f6e 6f6e 2066 7265 7175  Get phonon frequ
+00009910: 656e 6369 6573 2061 6e64 2065 6967 656e  encies and eigen
+00009920: 7665 6374 6f72 7320 696e 2049 6e74 6572  vectors in Inter
+00009930: 6163 7469 6f6e 2069 6e73 7461 6e63 652e  action instance.
+00009940: 0a0a 2020 2020 2020 2020 4861 726d 6f6e  ..        Harmon
+00009950: 6963 2070 686f 6e6f 6e20 696e 666f 726d  ic phonon inform
+00009960: 6174 696f 6e20 6973 2073 746f 7265 6420  ation is stored 
+00009970: 696e 2049 6e74 6572 6163 7469 6f6e 2069  in Interaction i
+00009980: 6e73 7461 6e63 652e 2054 6869 730a 2020  nstance. This.  
+00009990: 2020 2020 2020 696e 666f 726d 6174 696f        informatio
+000099a0: 6e20 6361 6e20 6265 206f 6274 6169 6e65  n can be obtaine
+000099b0: 642e 2054 6865 2067 7269 645f 6164 6472  d. The grid_addr
+000099c0: 6573 7320 7265 7475 726e 6564 2067 6976  ess returned giv
+000099d0: 6520 7468 650a 2020 2020 2020 2020 712d  e the.        q-
+000099e0: 706f 696e 7473 206c 6f63 6174 696f 6e73  points locations
+000099f0: 2077 6974 6820 7265 7370 6563 7420 746f   with respect to
+00009a00: 2072 6563 6970 726f 6361 6c20 6261 7369   reciprocal basi
+00009a10: 7320 7665 6374 6f72 7320 6279 0a20 2020  s vectors by.   
+00009a20: 2020 2020 2069 6e74 6567 6572 7320 696e       integers in
+00009a30: 2074 6865 2077 6179 2074 6861 740a 2020   the way that.  
+00009a40: 2020 2020 2020 2020 2020 715f 706f 696e            q_poin
+00009a50: 7473 203d 2067 7269 645f 6164 6472 6573  ts = grid_addres
+00009a60: 7320 2f20 6e70 2e61 7272 6179 286d 6573  s / np.array(mes
+00009a70: 682c 2064 7479 7065 3d27 646f 7562 6c65  h, dtype='double
+00009a80: 2729 2e0a 0a20 2020 2020 2020 2052 6574  ')...        Ret
+00009a90: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+00009aa0: 2d2d 2d2d 0a20 2020 2020 2020 2074 7570  ----.        tup
+00009ab0: 6c65 0a20 2020 2020 2020 2020 2020 2028  le.            (
+00009ac0: 6672 6571 7565 6e63 6965 732c 2065 6967  frequencies, eig
+00009ad0: 656e 7665 6374 6f72 732c 2067 7269 645f  envectors, grid_
+00009ae0: 6164 6472 6573 7329 0a20 2020 2020 2020  address).       
+00009af0: 2020 2020 2053 6565 206d 6f72 6520 6465       See more de
+00009b00: 7461 696c 7320 6174 2074 6865 2064 6f63  tails at the doc
+00009b10: 7374 7269 6e67 206f 6620 7365 745f 7068  string of set_ph
+00009b20: 6f6e 6f6e 5f64 6174 612e 0a0a 2020 2020  onon_data...    
+00009b30: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00009b40: 6966 2073 656c 662e 5f69 6e74 6572 6163  if self._interac
+00009b50: 7469 6f6e 2069 7320 6e6f 7420 4e6f 6e65  tion is not None
+00009b60: 3a0a 2020 2020 2020 2020 2020 2020 6672  :.            fr
+00009b70: 6571 732c 2065 6967 7665 6373 2c20 5f20  eqs, eigvecs, _ 
+00009b80: 3d20 7365 6c66 2e5f 696e 7465 7261 6374  = self._interact
+00009b90: 696f 6e2e 6765 745f 7068 6f6e 6f6e 7328  ion.get_phonons(
+00009ba0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00009bb0: 7475 726e 2066 7265 7173 2c20 6569 6776  turn freqs, eigv
+00009bc0: 6563 732c 2073 656c 662e 5f69 6e74 6572  ecs, self._inter
+00009bd0: 6163 7469 6f6e 2e62 7a5f 6772 6964 2e61  action.bz_grid.a
+00009be0: 6464 7265 7373 6573 0a20 2020 2020 2020  ddresses.       
+00009bf0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00009c00: 2020 206d 7367 203d 2028 0a20 2020 2020     msg = (.     
+00009c10: 2020 2020 2020 2020 2020 2022 5068 6f6e             "Phon
+00009c20: 6f33 7079 2e69 6e69 745f 7068 7068 5f69  o3py.init_phph_i
+00009c30: 6e74 6572 6163 7469 6f6e 2068 6173 2074  nteraction has t
+00009c40: 6f20 6265 2063 616c 6c65 6420 220a 2020  o be called ".  
+00009c50: 2020 2020 2020 2020 2020 2020 2020 2262                "b
+00009c60: 6566 6f72 6520 7275 6e6e 696e 6720 7468  efore running th
+00009c70: 6973 206d 6574 686f 642e 220a 2020 2020  is method.".    
+00009c80: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00009c90: 2020 2020 2020 7261 6973 6520 5275 6e74        raise Runt
+00009ca0: 696d 6545 7272 6f72 286d 7367 290a 0a20  imeError(msg).. 
+00009cb0: 2020 2064 6566 2072 756e 5f70 686f 6e6f     def run_phono
+00009cc0: 6e5f 736f 6c76 6572 2873 656c 662c 2067  n_solver(self, g
+00009cd0: 7269 645f 706f 696e 7473 3d4e 6f6e 6529  rid_points=None)
+00009ce0: 3a0a 2020 2020 2020 2020 2222 2252 756e  :.        """Run
+00009cf0: 2068 6172 6d6f 6e69 6320 7068 6f6e 6f6e   harmonic phonon
+00009d00: 2063 616c 6375 6c61 7469 6f6e 206f 6e20   calculation on 
+00009d10: 6772 6964 2070 6f69 6e74 732e 0a0a 2020  grid points...  
+00009d20: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00009d30: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00009d40: 2d2d 2d0a 2020 2020 2020 2020 6772 6964  ---.        grid
+00009d50: 5f70 6f69 6e74 7320 3a20 6172 7261 795f  _points : array_
+00009d60: 6c69 6b65 206f 7220 4e6f 6e65 2c20 6f70  like or None, op
+00009d70: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
+00009d80: 2020 2041 206c 6973 7420 6f66 2067 7269     A list of gri
+00009d90: 6420 706f 696e 7420 696e 6469 6365 7320  d point indices 
+00009da0: 6f66 2050 686f 6e6f 3370 792e 6772 6964  of Phono3py.grid
+00009db0: 2e61 6464 7265 7373 6573 2e0a 2020 2020  .addresses..    
+00009dc0: 2020 2020 2020 2020 5370 6563 6966 7969          Specifyi
+00009dd0: 6e67 204e 6f6e 6520 7275 6e73 2061 6c6c  ng None runs all
+00009de0: 2070 686f 6e6f 6e73 206f 6e20 7468 6520   phonons on the 
+00009df0: 6772 6964 2070 6f69 6e74 7320 756e 6c65  grid points unle
+00009e00: 7373 0a20 2020 2020 2020 2020 2020 2074  ss.            t
+00009e10: 686f 7365 2070 686f 6e6f 6e73 2077 6572  hose phonons wer
+00009e20: 6520 616c 7265 6164 7920 6361 6c63 756c  e already calcul
+00009e30: 6174 6564 2e20 4e6f 726d 616c 6c79 2070  ated. Normally p
+00009e40: 686f 6e6f 6e73 2061 740a 2020 2020 2020  honons at.      
+00009e50: 2020 2020 2020 5b30 2c20 302c 2030 5d20        [0, 0, 0] 
+00009e60: 706f 696e 7420 6973 2061 6c72 6561 6479  point is already
+00009e70: 2063 616c 6375 6c61 7465 6420 6265 666f   calculated befo
+00009e80: 7265 2063 616c 6c69 6e67 2074 6869 7320  re calling this 
+00009e90: 6d65 7468 6f64 2e0a 2020 2020 2020 2020  method..        
+00009ea0: 2020 2020 5068 6f6e 6f6e 2063 616c 6375      Phonon calcu
+00009eb0: 6c61 7469 6f6e 7320 6172 6520 7065 7266  lations are perf
+00009ec0: 6f72 6d65 6420 6175 746f 6d61 7469 6361  ormed automatica
+00009ed0: 6c6c 7920 7768 656e 206e 6565 6465 640a  lly when needed.
+00009ee0: 2020 2020 2020 2020 2020 2020 696e 7465              inte
+00009ef0: 726e 616c 6c79 2066 6f72 2070 682d 7068  rnally for ph-ph
+00009f00: 2063 616c 6375 6c61 7469 6f6e 2e20 5468   calculation. Th
+00009f10: 6572 6566 6f72 6520 6361 6c6c 696e 6720  erefore calling 
+00009f20: 7468 6973 206d 6574 686f 640a 2020 2020  this method.    
+00009f30: 2020 2020 2020 2020 6973 206e 6f74 206e          is not n
+00009f40: 6563 6573 7361 7279 2069 6e20 6d6f 7374  ecessary in most
+00009f50: 2063 6173 6573 2e0a 2020 2020 2020 2020   cases..        
+00009f60: 2020 2020 5468 6520 7068 6f6e 6f6e 2072      The phonon r
+00009f70: 6573 756c 7473 2061 7265 206f 6274 6169  esults are obtai
+00009f80: 6e65 6420 6279 2050 686f 6e6f 3370 792e  ned by Phono3py.
+00009f90: 6765 745f 7068 6f6e 6f6e 5f64 6174 6128  get_phonon_data(
+00009fa0: 292e 0a0a 2020 2020 2020 2020 2222 220a  )...        """.
+00009fb0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00009fc0: 5f69 6e74 6572 6163 7469 6f6e 2069 7320  _interaction is 
+00009fd0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00009fe0: 2020 2020 2020 7365 6c66 2e5f 696e 7465        self._inte
+00009ff0: 7261 6374 696f 6e2e 7275 6e5f 7068 6f6e  raction.run_phon
+0000a000: 6f6e 5f73 6f6c 7665 7228 6772 6964 5f70  on_solver(grid_p
+0000a010: 6f69 6e74 733d 6772 6964 5f70 6f69 6e74  oints=grid_point
+0000a020: 7329 0a20 2020 2020 2020 2065 6c73 653a  s).        else:
+0000a030: 0a20 2020 2020 2020 2020 2020 206d 7367  .            msg
+0000a040: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+0000a050: 2020 2020 2022 5068 6f6e 6f33 7079 2e69       "Phono3py.i
+0000a060: 6e69 745f 7068 7068 5f69 6e74 6572 6163  nit_phph_interac
+0000a070: 7469 6f6e 2068 6173 2074 6f20 6265 2063  tion has to be c
+0000a080: 616c 6c65 6420 220a 2020 2020 2020 2020  alled ".        
+0000a090: 2020 2020 2020 2020 2262 6566 6f72 6520          "before 
+0000a0a0: 7275 6e6e 696e 6720 7468 6973 206d 6574  running this met
+0000a0b0: 686f 642e 220a 2020 2020 2020 2020 2020  hod.".          
+0000a0c0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000a0d0: 7261 6973 6520 5275 6e74 696d 6545 7272  raise RuntimeErr
+0000a0e0: 6f72 286d 7367 290a 0a20 2020 2064 6566  or(msg)..    def
+0000a0f0: 2067 656e 6572 6174 655f 6469 7370 6c61   generate_displa
+0000a100: 6365 6d65 6e74 7328 0a20 2020 2020 2020  cements(.       
+0000a110: 2073 656c 662c 0a20 2020 2020 2020 2064   self,.        d
+0000a120: 6973 7461 6e63 653d 302e 3033 2c0a 2020  istance=0.03,.  
+0000a130: 2020 2020 2020 6375 746f 6666 5f70 6169        cutoff_pai
+0000a140: 725f 6469 7374 616e 6365 3d4e 6f6e 652c  r_distance=None,
+0000a150: 0a20 2020 2020 2020 2069 735f 706c 7573  .        is_plus
+0000a160: 6d69 6e75 733d 2261 7574 6f22 2c0a 2020  minus="auto",.  
+0000a170: 2020 2020 2020 6973 5f64 6961 676f 6e61        is_diagona
+0000a180: 6c3d 5472 7565 2c0a 2020 2020 293a 0a20  l=True,.    ):. 
+0000a190: 2020 2020 2020 2022 2222 4765 6e65 7261         """Genera
+0000a1a0: 7465 2064 6973 706c 6163 656d 656e 7420  te displacement 
+0000a1b0: 6461 7461 7365 7420 696e 2073 7570 6572  dataset in super
+0000a1c0: 6365 6c6c 2066 6f72 2066 6333 2e0a 0a20  cell for fc3... 
+0000a1d0: 2020 2020 2020 2054 6869 7320 7379 7374         This syst
+0000a1e0: 656d 6174 6963 616c 6c79 2067 656e 6572  ematically gener
+0000a1f0: 6174 6573 2073 696e 676c 6520 616e 6420  ates single and 
+0000a200: 7061 6972 2061 746f 6d69 6320 6469 7370  pair atomic disp
+0000a210: 6c61 6365 6d65 6e74 730a 2020 2020 2020  lacements.      
+0000a220: 2020 696e 2073 7570 6572 6365 6c6c 7320    in supercells 
+0000a230: 746f 2063 616c 6375 6c61 7465 2066 6333  to calculate fc3
+0000a240: 2063 6f6e 7369 6465 7269 6e67 2063 7279   considering cry
+0000a250: 7374 616c 2073 796d 6d65 7472 792e 0a20  stal symmetry.. 
+0000a260: 2020 2020 2020 2057 6865 6e20 7468 6973         When this
+0000a270: 206d 6574 686f 6420 6973 2063 616c 6c65   method is calle
+0000a280: 642c 2065 7869 7374 696e 6720 6361 6368  d, existing cach
+0000a290: 6520 6f66 2073 7570 6572 6365 6c6c 7320  e of supercells 
+0000a2a0: 7769 7468 0a20 2020 2020 2020 2064 6973  with.        dis
+0000a2b0: 706c 6163 656d 656e 7473 2066 6f72 2066  placements for f
+0000a2c0: 6333 2061 7265 2072 656d 6f76 6564 2e0a  c3 are removed..
+0000a2d0: 0a20 2020 2020 2020 2046 6f72 2066 6333  .        For fc3
+0000a2e0: 2c20 7477 6f20 6174 6f6d 7320 6172 6520  , two atoms are 
+0000a2f0: 6469 7370 6c61 6365 6420 666f 7220 6561  displaced for ea
+0000a300: 6368 2063 6f6e 6669 6775 7261 7469 6f6e  ch configuration
+0000a310: 0a20 2020 2020 2020 2063 6f6e 7369 6465  .        conside
+0000a320: 7269 6e67 2063 7279 7374 616c 2073 796d  ring crystal sym
+0000a330: 6d65 7472 792e 2054 6865 2066 6972 7374  metry. The first
+0000a340: 2064 6973 706c 6163 656d 656e 7420 6973   displacement is
+0000a350: 2063 686f 7365 6e0a 2020 2020 2020 2020   chosen.        
+0000a360: 696e 2074 6865 2070 6572 6665 6374 2073  in the perfect s
+0000a370: 7570 6572 6365 6c6c 2c20 616e 6420 7468  upercell, and th
+0000a380: 6520 7365 636f 6e64 2064 6973 706c 6163  e second displac
+0000a390: 656d 656e 7420 696e 2074 6865 0a20 2020  ement in the.   
+0000a3a0: 2020 2020 2064 6973 706c 6163 6564 2073       displaced s
+0000a3b0: 7570 6572 6365 6c6c 2e20 5468 6520 6669  upercell. The fi
+0000a3c0: 7273 7420 6469 7370 6c61 6365 6d65 6e74  rst displacement
+0000a3d0: 7320 6172 6520 7461 6b65 6e20 616c 6f6e  s are taken alon
+0000a3e0: 670a 2020 2020 2020 2020 7468 6520 6261  g.        the ba
+0000a3f0: 7369 7320 7665 6374 6f72 7320 6f66 2074  sis vectors of t
+0000a400: 6865 2073 7570 6572 6365 6c6c 2e20 5468  he supercell. Th
+0000a410: 6973 2069 7320 6265 6361 7573 6520 7468  is is because th
+0000a420: 650a 2020 2020 2020 2020 7379 6d6d 6574  e.        symmet
+0000a430: 7279 2069 7320 6578 7065 6374 6564 2074  ry is expected t
+0000a440: 6f20 6265 206c 6573 7320 6272 6f6b 656e  o be less broken
+0000a450: 2062 7920 7468 6520 696e 7472 6f64 7563   by the introduc
+0000a460: 6564 2066 6972 7374 0a20 2020 2020 2020  ed first.       
+0000a470: 2064 6973 706c 6163 656d 656e 742c 2061   displacement, a
+0000a480: 6e64 2061 7320 7468 6520 7265 7375 6c74  nd as the result
+0000a490: 2c20 7468 6520 6e75 6d62 6572 206f 6620  , the number of 
+0000a4a0: 7365 636f 6e64 0a20 2020 2020 2020 2064  second.        d
+0000a4b0: 6973 706c 6163 656d 656e 7473 206d 6179  isplacements may
+0000a4c0: 2062 6563 6f6d 6520 736d 616c 6c65 7220   become smaller 
+0000a4d0: 7468 616e 2074 6865 2063 6173 6520 7468  than the case th
+0000a4e0: 6174 2074 6865 2066 6972 7374 0a20 2020  at the first.   
+0000a4f0: 2020 2020 2061 746f 6d20 6973 2064 6973       atom is dis
+0000a500: 706c 6163 6564 206e 6f74 2061 6c6f 6e67  placed not along
+0000a510: 2074 6865 2062 6173 6973 2076 6563 746f   the basis vecto
+0000a520: 7273 2e0a 0a20 2020 2020 2020 204e 6f74  rs...        Not
+0000a530: 650a 2020 2020 2020 2020 2d2d 2d2d 0a20  e.        ----. 
+0000a540: 2020 2020 2020 2057 6865 6e20 7068 6f6e         When phon
+0000a550: 6f6e 5f73 7570 6572 6365 6c6c 5f6d 6174  on_supercell_mat
+0000a560: 7269 7820 6973 206e 6f74 2067 6976 656e  rix is not given
+0000a570: 2c20 6663 3220 6973 2061 6c73 6f0a 2020  , fc2 is also.  
+0000a580: 2020 2020 2020 636f 6d70 7574 6564 2066        computed f
+0000a590: 726f 6d20 7468 6520 7361 6d65 2073 6574  rom the same set
+0000a5a0: 206f 6620 7468 6520 6469 7370 6c61 6365   of the displace
+0000a5b0: 6d65 6e74 7320 666f 7220 6663 3320 616e  ments for fc3 an
+0000a5c0: 640a 2020 2020 2020 2020 7265 7370 6563  d.        respec
+0000a5d0: 7469 7665 2073 7570 6572 6365 6c6c 2066  tive supercell f
+0000a5e0: 6f72 6365 732e 2057 6865 6e20 7068 6f6e  orces. When phon
+0000a5f0: 6f6e 5f73 7570 6572 6365 6c6c 5f6d 6174  on_supercell_mat
+0000a600: 7269 7820 6973 0a20 2020 2020 2020 2073  rix is.        s
+0000a610: 6574 2c20 7468 6520 6469 7370 6c61 6365  et, the displace
+0000a620: 6d65 6e74 7320 696e 2070 686f 6e6f 6e5f  ments in phonon_
+0000a630: 7375 7065 7263 656c 6c20 6172 6520 6765  supercell are ge
+0000a640: 6e65 7261 7465 6420 756e 6c65 7373 0a20  nerated unless. 
+0000a650: 2020 2020 2020 2074 686f 7365 2061 6c72         those alr
+0000a660: 6561 6479 2065 7869 7374 2e0a 0a20 2020  eady exist...   
+0000a670: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+0000a680: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+0000a690: 2d2d 0a20 2020 2020 2020 2064 6973 7461  --.        dista
+0000a6a0: 6e63 6520 3a20 666c 6f61 742c 206f 7074  nce : float, opt
+0000a6b0: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+0000a6c0: 2020 436f 6e73 7461 6e74 2064 6973 706c    Constant displ
+0000a6d0: 6163 656d 656e 7420 4575 636c 6964 6561  acement Euclidea
+0000a6e0: 6e20 6469 7374 616e 6365 2e20 4465 6661  n distance. Defa
+0000a6f0: 756c 7420 6973 2030 2e30 332e 0a20 2020  ult is 0.03..   
+0000a700: 2020 2020 2063 7574 6f66 665f 7061 6972       cutoff_pair
+0000a710: 5f64 6973 7461 6e63 6520 3a20 666c 6f61  _distance : floa
+0000a720: 742c 206f 7074 696f 6e61 6c0a 2020 2020  t, optional.    
+0000a730: 2020 2020 2020 2020 5468 6973 2069 7320          This is 
+0000a740: 7573 6564 2061 7320 6120 6375 746f 6666  used as a cutoff
+0000a750: 2045 7563 6c69 6465 616e 2064 6973 7461   Euclidean dista
+0000a760: 6e63 6520 746f 2064 6574 6572 6d69 6e65  nce to determine
+0000a770: 2069 660a 2020 2020 2020 2020 2020 2020   if.            
+0000a780: 6561 6368 2070 6169 7220 6f66 2064 6973  each pair of dis
+0000a790: 706c 6163 656d 656e 7473 2069 7320 636f  placements is co
+0000a7a0: 6e73 6964 6572 6564 2074 6f20 6361 6c63  nsidered to calc
+0000a7b0: 756c 6174 6520 6663 3320 6f72 206e 6f74  ulate fc3 or not
+0000a7c0: 2e0a 2020 2020 2020 2020 2020 2020 4465  ..            De
+0000a7d0: 6661 756c 7420 6973 204e 6f6e 652c 2077  fault is None, w
+0000a7e0: 6869 6368 206d 6561 6e73 2063 7574 6f66  hich means cutof
+0000a7f0: 6620 6973 206e 6f74 2075 7365 642e 0a20  f is not used.. 
+0000a800: 2020 2020 2020 2069 735f 706c 7573 6d69         is_plusmi
+0000a810: 6e75 7320 3a20 5472 7565 2c20 4661 6c73  nus : True, Fals
+0000a820: 652c 206f 7220 2761 7574 6f27 2c20 6f70  e, or 'auto', op
+0000a830: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
+0000a840: 2020 2057 6974 6820 5472 7565 2c20 6174     With True, at
+0000a850: 6f6d 6973 2061 7265 2064 6973 706c 6163  omis are displac
+0000a860: 6564 2069 6e20 626f 7468 2070 6f73 6974  ed in both posit
+0000a870: 6976 6520 616e 6420 6e65 6761 7469 7665  ive and negative
+0000a880: 0a20 2020 2020 2020 2020 2020 2064 6972  .            dir
+0000a890: 6563 7469 6f6e 732e 2057 6974 6820 4661  ections. With Fa
+0000a8a0: 6c73 652c 206f 6e6c 7920 6f6e 6520 6469  lse, only one di
+0000a8b0: 7265 6374 696f 6e2e 2057 6974 6820 2761  rection. With 'a
+0000a8c0: 7574 6f27 2c0a 2020 2020 2020 2020 2020  uto',.          
+0000a8d0: 2020 6d6f 7374 6c79 2065 7175 6976 616c    mostly equival
+0000a8e0: 656e 7420 746f 2069 735f 706c 7573 6d69  ent to is_plusmi
+0000a8f0: 6e75 733d 5472 7565 2c20 6275 7420 6f6e  nus=True, but on
+0000a900: 6c79 206f 6e65 2064 6972 6563 7469 6f6e  ly one direction
+0000a910: 0a20 2020 2020 2020 2020 2020 2069 7320  .            is 
+0000a920: 6368 6f73 656e 2077 6865 6e20 7468 6520  chosen when the 
+0000a930: 6469 7370 6c61 6365 6d65 6e74 7320 696e  displacements in
+0000a940: 2062 6f74 6820 6469 7265 6374 696f 6e73   both directions
+0000a950: 2061 7265 0a20 2020 2020 2020 2020 2020   are.           
+0000a960: 2073 796d 6d65 7472 6963 616c 6c79 2065   symmetrically e
+0000a970: 7175 6976 616c 656e 742e 2044 6566 6175  quivalent. Defau
+0000a980: 6c74 2069 7320 2761 7574 6f27 2e0a 2020  lt is 'auto'..  
+0000a990: 2020 2020 2020 6973 5f64 6961 676f 6e61        is_diagona
+0000a9a0: 6c20 3a20 426f 6f6c 2c20 6f70 7469 6f6e  l : Bool, option
+0000a9b0: 616c 0a20 2020 2020 2020 2020 2020 2057  al.            W
+0000a9c0: 6974 6820 4661 6c73 652c 2074 6865 2073  ith False, the s
+0000a9d0: 6563 6f6e 6420 6469 7370 6c61 6365 6d65  econd displaceme
+0000a9e0: 6e74 7320 6172 6520 6d61 6465 2061 6c6f  nts are made alo
+0000a9f0: 6e67 2074 6865 2062 6173 6973 0a20 2020  ng the basis.   
+0000aa00: 2020 2020 2020 2020 2076 6563 746f 7273           vectors
+0000aa10: 206f 6620 7468 6520 7375 7065 7263 656c   of the supercel
+0000aa20: 6c2e 2057 6974 6820 5472 7565 2c20 6469  l. With True, di
+0000aa30: 7265 6374 696f 6e20 6e6f 7420 616c 6f6e  rection not alon
+0000aa40: 6720 7468 6520 6261 7369 730a 2020 2020  g the basis.    
+0000aa50: 2020 2020 2020 2020 7665 6374 6f72 7320          vectors 
+0000aa60: 6361 6e20 6265 2063 686f 7365 6e20 7768  can be chosen wh
+0000aa70: 656e 2074 6865 206e 756d 6265 7220 6f66  en the number of
+0000aa80: 2074 6865 2064 6973 706c 6163 656d 656e   the displacemen
+0000aa90: 7473 0a20 2020 2020 2020 2020 2020 206d  ts.            m
+0000aaa0: 6179 2062 6520 7265 6475 6365 642e 0a0a  ay be reduced...
+0000aab0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000aac0: 2020 2020 6469 7265 6374 696f 6e5f 6461      direction_da
+0000aad0: 7461 7365 7420 3d20 6765 745f 7468 6972  taset = get_thir
+0000aae0: 645f 6f72 6465 725f 6469 7370 6c61 6365  d_order_displace
+0000aaf0: 6d65 6e74 7328 0a20 2020 2020 2020 2020  ments(.         
+0000ab00: 2020 2073 656c 662e 5f73 7570 6572 6365     self._superce
+0000ab10: 6c6c 2c0a 2020 2020 2020 2020 2020 2020  ll,.            
+0000ab20: 7365 6c66 2e5f 7379 6d6d 6574 7279 2c0a  self._symmetry,.
+0000ab30: 2020 2020 2020 2020 2020 2020 6973 5f70              is_p
+0000ab40: 6c75 736d 696e 7573 3d69 735f 706c 7573  lusminus=is_plus
+0000ab50: 6d69 6e75 732c 0a20 2020 2020 2020 2020  minus,.         
+0000ab60: 2020 2069 735f 6469 6167 6f6e 616c 3d69     is_diagonal=i
+0000ab70: 735f 6469 6167 6f6e 616c 2c0a 2020 2020  s_diagonal,.    
+0000ab80: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
+0000ab90: 6c66 2e5f 6461 7461 7365 7420 3d20 6469  lf._dataset = di
+0000aba0: 7265 6374 696f 6e5f 746f 5f64 6973 706c  rection_to_displ
+0000abb0: 6163 656d 656e 7428 0a20 2020 2020 2020  acement(.       
+0000abc0: 2020 2020 2064 6972 6563 7469 6f6e 5f64       direction_d
+0000abd0: 6174 6173 6574 2c0a 2020 2020 2020 2020  ataset,.        
+0000abe0: 2020 2020 6469 7374 616e 6365 2c0a 2020      distance,.  
+0000abf0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000ac00: 7375 7065 7263 656c 6c2c 0a20 2020 2020  supercell,.     
+0000ac10: 2020 2020 2020 2063 7574 6f66 665f 6469         cutoff_di
+0000ac20: 7374 616e 6365 3d63 7574 6f66 665f 7061  stance=cutoff_pa
+0000ac30: 6972 5f64 6973 7461 6e63 652c 0a20 2020  ir_distance,.   
+0000ac40: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
+0000ac50: 656c 662e 5f73 7570 6572 6365 6c6c 735f  elf._supercells_
+0000ac60: 7769 7468 5f64 6973 706c 6163 656d 656e  with_displacemen
+0000ac70: 7473 203d 204e 6f6e 650a 0a20 2020 2020  ts = None..     
+0000ac80: 2020 2069 6620 7365 6c66 2e5f 7068 6f6e     if self._phon
+0000ac90: 6f6e 5f73 7570 6572 6365 6c6c 5f6d 6174  on_supercell_mat
+0000aca0: 7269 7820 6973 206e 6f74 204e 6f6e 6520  rix is not None 
+0000acb0: 616e 6420 7365 6c66 2e5f 7068 6f6e 6f6e  and self._phonon
+0000acc0: 5f64 6174 6173 6574 2069 7320 4e6f 6e65  _dataset is None
+0000acd0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000ace0: 6c66 2e67 656e 6572 6174 655f 6663 325f  lf.generate_fc2_
+0000acf0: 6469 7370 6c61 6365 6d65 6e74 7328 0a20  displacements(. 
+0000ad00: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000ad10: 6973 7461 6e63 653d 6469 7374 616e 6365  istance=distance
+0000ad20: 2c20 6973 5f70 6c75 736d 696e 7573 3d69  , is_plusminus=i
+0000ad30: 735f 706c 7573 6d69 6e75 732c 2069 735f  s_plusminus, is_
+0000ad40: 6469 6167 6f6e 616c 3d46 616c 7365 0a20  diagonal=False. 
+0000ad50: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0000ad60: 2020 6465 6620 6765 6e65 7261 7465 5f66    def generate_f
+0000ad70: 6332 5f64 6973 706c 6163 656d 656e 7473  c2_displacements
+0000ad80: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
+0000ad90: 6469 7374 616e 6365 3d30 2e30 332c 2069  distance=0.03, i
+0000ada0: 735f 706c 7573 6d69 6e75 733d 2261 7574  s_plusminus="aut
+0000adb0: 6f22 2c20 6973 5f64 6961 676f 6e61 6c3d  o", is_diagonal=
+0000adc0: 4661 6c73 650a 2020 2020 293a 0a20 2020  False.    ):.   
+0000add0: 2020 2020 2022 2222 4765 6e65 7261 7465       """Generate
+0000ade0: 2064 6973 706c 6163 656d 656e 7420 6461   displacement da
+0000adf0: 7461 7365 7420 696e 2070 686f 6e6f 6e20  taset in phonon 
+0000ae00: 7375 7065 7263 656c 6c20 666f 7220 6663  supercell for fc
+0000ae10: 322e 0a0a 2020 2020 2020 2020 5468 6973  2...        This
+0000ae20: 2073 7973 7465 6d61 7469 6361 6c6c 7920   systematically 
+0000ae30: 6765 6e65 7261 7465 7320 7369 6e67 6c65  generates single
+0000ae40: 2061 746f 6d69 6320 6469 7370 6c61 6365   atomic displace
+0000ae50: 6d65 6e74 730a 2020 2020 2020 2020 696e  ments.        in
+0000ae60: 2073 7570 6572 6365 6c6c 7320 746f 2063   supercells to c
+0000ae70: 616c 6375 6c61 7465 2070 686f 6e6f 6e5f  alculate phonon_
+0000ae80: 6663 3220 636f 6e73 6964 6572 696e 6720  fc2 considering 
+0000ae90: 6372 7973 7461 6c20 7379 6d6d 6574 7279  crystal symmetry
+0000aea0: 2e0a 2020 2020 2020 2020 5768 656e 2074  ..        When t
+0000aeb0: 6869 7320 6d65 7468 6f64 2069 7320 6361  his method is ca
+0000aec0: 6c6c 6564 2c20 6578 6973 7469 6e67 2063  lled, existing c
+0000aed0: 6163 6865 206f 6620 7375 7065 7263 656c  ache of supercel
+0000aee0: 6c73 2077 6974 680a 2020 2020 2020 2020  ls with.        
+0000aef0: 6469 7370 6c61 6365 6d65 6e74 7320 666f  displacements fo
+0000af00: 7220 6663 3220 6172 6520 7265 6d6f 7665  r fc2 are remove
+0000af10: 642e 0a0a 2020 2020 2020 2020 4e6f 7465  d...        Note
+0000af20: 0a20 2020 2020 2020 202d 2d2d 2d0a 2020  .        ----.  
+0000af30: 2020 2020 2020 6973 5f64 6961 676f 6e61        is_diagona
+0000af40: 6c3d 4661 6c73 6520 6973 2063 686f 7365  l=False is chose
+0000af50: 6e20 6173 2074 6865 2064 6566 6175 6c74  n as the default
+0000af60: 2073 6574 7469 6e67 2069 6e74 656e 7469   setting intenti
+0000af70: 6f6e 616c 6c79 0a20 2020 2020 2020 2074  onally.        t
+0000af80: 6f20 6265 2063 6f6e 7369 7374 656e 7420  o be consistent 
+0000af90: 746f 2074 6865 2066 6972 7374 2064 6973  to the first dis
+0000afa0: 706c 6163 656d 656e 7473 206f 6620 7468  placements of th
+0000afb0: 6520 6663 3320 7061 6972 0a20 2020 2020  e fc3 pair.     
+0000afc0: 2020 2064 6973 706c 6163 656d 6574 7320     displacemets 
+0000afd0: 696e 2073 7570 6572 6365 6c6c 2e0a 0a20  in supercell... 
+0000afe0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+0000aff0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0000b000: 2d2d 2d2d 0a20 2020 2020 2020 2064 6973  ----.        dis
+0000b010: 7461 6e63 6520 3a20 666c 6f61 742c 206f  tance : float, o
+0000b020: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+0000b030: 2020 2020 436f 6e73 7461 6e74 2064 6973      Constant dis
+0000b040: 706c 6163 656d 656e 7420 4575 636c 6964  placement Euclid
+0000b050: 6561 6e20 6469 7374 616e 6365 2e20 4465  ean distance. De
+0000b060: 6661 756c 7420 6973 2030 2e30 332e 0a20  fault is 0.03.. 
+0000b070: 2020 2020 2020 2069 735f 706c 7573 6d69         is_plusmi
+0000b080: 6e75 7320 3a20 5472 7565 2c20 4661 6c73  nus : True, Fals
+0000b090: 652c 206f 7220 2761 7574 6f27 2c20 6f70  e, or 'auto', op
+0000b0a0: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
+0000b0b0: 2020 2057 6974 6820 5472 7565 2c20 6174     With True, at
+0000b0c0: 6f6d 6973 2061 7265 2064 6973 706c 6163  omis are displac
+0000b0d0: 6564 2069 6e20 626f 7468 2070 6f73 6974  ed in both posit
+0000b0e0: 6976 6520 616e 6420 6e65 6761 7469 7665  ive and negative
+0000b0f0: 0a20 2020 2020 2020 2020 2020 2064 6972  .            dir
+0000b100: 6563 7469 6f6e 732e 2057 6974 6820 4661  ections. With Fa
+0000b110: 6c73 652c 206f 6e6c 7920 6f6e 6520 6469  lse, only one di
+0000b120: 7265 6374 696f 6e2e 2057 6974 6820 2761  rection. With 'a
+0000b130: 7574 6f27 2c0a 2020 2020 2020 2020 2020  uto',.          
+0000b140: 2020 6d6f 7374 6c79 2065 7175 6976 616c    mostly equival
+0000b150: 656e 7420 746f 2069 735f 706c 7573 6d69  ent to is_plusmi
+0000b160: 6e75 733d 5472 7565 2c20 6275 7420 6f6e  nus=True, but on
+0000b170: 6c79 206f 6e65 2064 6972 6563 7469 6f6e  ly one direction
+0000b180: 0a20 2020 2020 2020 2020 2020 2069 7320  .            is 
+0000b190: 6368 6f73 656e 2077 6865 6e20 7468 6520  chosen when the 
+0000b1a0: 6469 7370 6c61 6365 6d65 6e74 7320 696e  displacements in
+0000b1b0: 2062 6f74 6820 6469 7265 6374 696f 6e73   both directions
+0000b1c0: 2061 7265 0a20 2020 2020 2020 2020 2020   are.           
+0000b1d0: 2073 796d 6d65 7472 6963 616c 6c79 2065   symmetrically e
+0000b1e0: 7175 6976 616c 656e 742e 2044 6566 6175  quivalent. Defau
+0000b1f0: 6c74 2069 7320 2761 7574 6f27 2e0a 2020  lt is 'auto'..  
+0000b200: 2020 2020 2020 6973 5f64 6961 676f 6e61        is_diagona
+0000b210: 6c20 3a20 426f 6f6c 2c20 6f70 7469 6f6e  l : Bool, option
+0000b220: 616c 0a20 2020 2020 2020 2020 2020 2057  al.            W
+0000b230: 6974 6820 4661 6c73 652c 2074 6865 2064  ith False, the d
+0000b240: 6973 706c 6163 656d 656e 7473 2061 7265  isplacements are
+0000b250: 206d 6164 6520 616c 6f6e 6720 7468 6520   made along the 
+0000b260: 6261 7369 730a 2020 2020 2020 2020 2020  basis.          
+0000b270: 2020 7665 6374 6f72 7320 6f66 2074 6865    vectors of the
+0000b280: 2073 7570 6572 6365 6c6c 2e20 5769 7468   supercell. With
+0000b290: 2054 7275 652c 2064 6972 6563 7469 6f6e   True, direction
+0000b2a0: 206e 6f74 2061 6c6f 6e67 2074 6865 2062   not along the b
+0000b2b0: 6173 6973 0a20 2020 2020 2020 2020 2020  asis.           
+0000b2c0: 2076 6563 746f 7273 2063 616e 2062 6520   vectors can be 
+0000b2d0: 6368 6f73 656e 2077 6865 6e20 7468 6520  chosen when the 
+0000b2e0: 6e75 6d62 6572 206f 6620 7468 6520 6469  number of the di
+0000b2f0: 7370 6c61 6365 6d65 6e74 730a 2020 2020  splacements.    
+0000b300: 2020 2020 2020 2020 6d61 7920 6265 2072          may be r
+0000b310: 6564 7563 6564 2e20 4465 6661 756c 7420  educed. Default 
+0000b320: 6973 2046 616c 7365 2e0a 0a20 2020 2020  is False...     
+0000b330: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+0000b340: 6620 7365 6c66 2e5f 7068 6f6e 6f6e 5f73  f self._phonon_s
+0000b350: 7570 6572 6365 6c6c 5f6d 6174 7269 7820  upercell_matrix 
+0000b360: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+0000b370: 2020 2020 206d 7367 203d 2028 0a20 2020       msg = (.   
+0000b380: 2020 2020 2020 2020 2020 2020 2022 7068               "ph
+0000b390: 6f6e 6f6e 5f73 7570 6572 6365 6c6c 5f6d  onon_supercell_m
+0000b3a0: 6174 7269 7820 6973 206e 6f74 2073 6574  atrix is not set
+0000b3b0: 2e20 220a 2020 2020 2020 2020 2020 2020  . ".            
+0000b3c0: 2020 2020 2254 6869 7320 6d65 7468 6f64      "This method
+0000b3d0: 2069 7320 7573 6564 2074 6f20 6765 6e65   is used to gene
+0000b3e0: 7261 7465 2064 6973 706c 6163 656d 656e  rate displacemen
+0000b3f0: 7473 2074 6f20 220a 2020 2020 2020 2020  ts to ".        
+0000b400: 2020 2020 2020 2020 2263 616c 6375 6c61          "calcula
+0000b410: 7465 2070 686f 6e6f 6e5f 6663 322e 220a  te phonon_fc2.".
+0000b420: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000b430: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000b440: 5275 6e74 696d 6545 7272 6f72 286d 7367  RuntimeError(msg
+0000b450: 290a 0a20 2020 2020 2020 2070 686f 6e6f  )..        phono
+0000b460: 6e5f 6469 7370 6c61 6365 6d65 6e74 5f64  n_displacement_d
+0000b470: 6972 6563 7469 6f6e 7320 3d20 6765 745f  irections = get_
+0000b480: 6c65 6173 745f 6469 7370 6c61 6365 6d65  least_displaceme
+0000b490: 6e74 7328 0a20 2020 2020 2020 2020 2020  nts(.           
+0000b4a0: 2073 656c 662e 5f70 686f 6e6f 6e5f 7375   self._phonon_su
+0000b4b0: 7065 7263 656c 6c5f 7379 6d6d 6574 7279  percell_symmetry
+0000b4c0: 2c0a 2020 2020 2020 2020 2020 2020 6973  ,.            is
+0000b4d0: 5f70 6c75 736d 696e 7573 3d69 735f 706c  _plusminus=is_pl
+0000b4e0: 7573 6d69 6e75 732c 0a20 2020 2020 2020  usminus,.       
+0000b4f0: 2020 2020 2069 735f 6469 6167 6f6e 616c       is_diagonal
+0000b500: 3d69 735f 6469 6167 6f6e 616c 2c0a 2020  =is_diagonal,.  
+0000b510: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000b520: 7365 6c66 2e5f 7068 6f6e 6f6e 5f64 6174  self._phonon_dat
+0000b530: 6173 6574 203d 2064 6972 6563 7469 6f6e  aset = direction
+0000b540: 735f 746f 5f64 6973 706c 6163 656d 656e  s_to_displacemen
+0000b550: 745f 6461 7461 7365 7428 0a20 2020 2020  t_dataset(.     
+0000b560: 2020 2020 2020 2070 686f 6e6f 6e5f 6469         phonon_di
+0000b570: 7370 6c61 6365 6d65 6e74 5f64 6972 6563  splacement_direc
+0000b580: 7469 6f6e 732c 2064 6973 7461 6e63 652c  tions, distance,
+0000b590: 2073 656c 662e 5f70 686f 6e6f 6e5f 7375   self._phonon_su
+0000b5a0: 7065 7263 656c 6c0a 2020 2020 2020 2020  percell.        
+0000b5b0: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
+0000b5c0: 7068 6f6e 6f6e 5f73 7570 6572 6365 6c6c  phonon_supercell
+0000b5d0: 735f 7769 7468 5f64 6973 706c 6163 656d  s_with_displacem
+0000b5e0: 656e 7473 203d 204e 6f6e 650a 0a20 2020  ents = None..   
+0000b5f0: 2064 6566 2070 726f 6475 6365 5f66 6333   def produce_fc3
+0000b600: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0000b610: 2020 2020 2020 2020 7379 6d6d 6574 7269          symmetri
+0000b620: 7a65 5f66 6333 723d 4661 6c73 652c 0a20  ze_fc3r=False,. 
+0000b630: 2020 2020 2020 2069 735f 636f 6d70 6163         is_compac
+0000b640: 745f 6663 3d46 616c 7365 2c0a 2020 2020  t_fc=False,.    
+0000b650: 2020 2020 6663 5f63 616c 6375 6c61 746f      fc_calculato
+0000b660: 723d 4e6f 6e65 2c0a 2020 2020 2020 2020  r=None,.        
+0000b670: 6663 5f63 616c 6375 6c61 746f 725f 6f70  fc_calculator_op
+0000b680: 7469 6f6e 733d 4e6f 6e65 2c0a 2020 2020  tions=None,.    
+0000b690: 293a 0a20 2020 2020 2020 2022 2222 4361  ):.        """Ca
+0000b6a0: 6c63 756c 6174 6520 6663 3320 6672 6f6d  lculate fc3 from
+0000b6b0: 2064 6973 706c 6163 656d 656e 7473 2061   displacements a
+0000b6c0: 6e64 2066 6f72 6365 732e 0a0a 2020 2020  nd forces...    
+0000b6d0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+0000b6e0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+0000b6f0: 2d0a 2020 2020 2020 2020 7379 6d6d 6574  -.        symmet
+0000b700: 7269 7a65 5f66 6333 7220 3a20 626f 6f6c  rize_fc3r : bool
+0000b710: 0a20 2020 2020 2020 2020 2020 204f 6e6c  .            Onl
+0000b720: 7920 666f 7220 7479 7065 2031 2064 6973  y for type 1 dis
+0000b730: 706c 6163 656d 656e 745f 6461 7461 7365  placement_datase
+0000b740: 742c 2074 7261 6e73 6c61 7469 6f6e 616c  t, translational
+0000b750: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
+0000b760: 2070 6572 6d75 7461 7469 6f6e 2073 796d   permutation sym
+0000b770: 6d65 7472 6965 7320 6172 6520 6170 706c  metries are appl
+0000b780: 6965 6420 6166 7465 7220 6372 6561 7469  ied after creati
+0000b790: 6e67 2066 6333 2e20 5468 6973 0a20 2020  ng fc3. This.   
+0000b7a0: 2020 2020 2020 2020 2073 796d 6d65 7472           symmetr
+0000b7b0: 697a 6174 696f 6e20 6973 206e 6f74 2076  ization is not v
+0000b7c0: 6572 7920 736f 7068 6973 7469 6361 7465  ery sophisticate
+0000b7d0: 6420 616e 6420 6361 6e20 6272 6561 6b20  d and can break 
+0000b7e0: 7370 6163 650a 2020 2020 2020 2020 2020  space.          
+0000b7f0: 2020 6772 6f75 7020 7379 6d6d 6574 7279    group symmetry
+0000b800: 2c20 6275 7420 6f66 7465 6e20 7573 6566  , but often usef
+0000b810: 756c 2e20 4966 2062 6574 7465 7220 7379  ul. If better sy
+0000b820: 6d6d 6574 7269 7a61 7469 6f6e 2069 730a  mmetrization is.
+0000b830: 2020 2020 2020 2020 2020 2020 6578 7065              expe
+0000b840: 6374 6564 2c20 6974 2069 7320 7265 636f  cted, it is reco
+0000b850: 6d6d 656e 6465 6420 746f 2075 7365 2065  mmended to use e
+0000b860: 7874 6572 6e61 6c20 666f 7263 6520 636f  xternal force co
+0000b870: 6e73 7461 6e74 730a 2020 2020 2020 2020  nstants.        
+0000b880: 2020 2020 6361 6c63 756c 6174 6f72 2073      calculator s
+0000b890: 7563 6820 6173 2041 4c4d 2e20 4465 6661  uch as ALM. Defa
+0000b8a0: 756c 7420 6973 2046 616c 7365 2e0a 2020  ult is False..  
+0000b8b0: 2020 2020 2020 6973 5f63 6f6d 7061 6374        is_compact
+0000b8c0: 5f66 6320 3a20 626f 6f6c 0a20 2020 2020  _fc : bool.     
+0000b8d0: 2020 2020 2020 2066 6333 2073 6861 7065         fc3 shape
+0000b8e0: 2069 730a 2020 2020 2020 2020 2020 2020   is.            
+0000b8f0: 2020 2020 4661 6c73 653a 2028 7375 7065      False: (supe
+0000b900: 7263 656c 6c2c 2073 7570 6572 6365 6c6c  rcell, supercell
+0000b910: 2c20 7375 7065 6365 6c6c 2c20 332c 2033  , supecell, 3, 3
+0000b920: 2c20 3329 0a20 2020 2020 2020 2020 2020  , 3).           
+0000b930: 2020 2020 2054 7275 653a 2028 7072 696d       True: (prim
+0000b940: 6974 6976 652c 2073 7570 6572 6365 6c6c  itive, supercell
+0000b950: 2c20 7375 7065 6365 6c6c 2c20 332c 2033  , supecell, 3, 3
+0000b960: 2c20 3329 0a20 2020 2020 2020 2020 2020  , 3).           
+0000b970: 2077 6865 7265 2027 7375 7065 7263 656c   where 'supercel
+0000b980: 6c27 2061 6e64 2027 7072 696d 6974 6976  l' and 'primitiv
+0000b990: 6527 2069 6e64 6963 6174 6520 6e75 6d62  e' indicate numb
+0000b9a0: 6572 206f 6620 6174 6f6d 7320 696e 2074  er of atoms in t
+0000b9b0: 6865 7365 0a20 2020 2020 2020 2020 2020  hese.           
+0000b9c0: 2063 656c 6c73 2e20 4465 6661 756c 7420   cells. Default 
+0000b9d0: 6973 2046 616c 7365 2e0a 2020 2020 2020  is False..      
+0000b9e0: 2020 6663 5f63 616c 6375 6c61 746f 7220    fc_calculator 
+0000b9f0: 3a20 7374 7220 6f72 204e 6f6e 650a 2020  : str or None.  
+0000ba00: 2020 2020 2020 2020 2020 466f 7263 6520            Force 
+0000ba10: 636f 6e73 7461 6e74 7320 6361 6c63 756c  constants calcul
+0000ba20: 6174 6f72 2067 6976 656e 2062 7920 7374  ator given by st
+0000ba30: 722e 0a20 2020 2020 2020 2066 635f 6361  r..        fc_ca
+0000ba40: 6c63 756c 6174 6f72 5f6f 7074 696f 6e73  lculator_options
+0000ba50: 203a 2064 6963 740a 2020 2020 2020 2020   : dict.        
+0000ba60: 2020 2020 4f70 7469 6f6e 7320 666f 7220      Options for 
+0000ba70: 6578 7465 726e 616c 2066 6f72 6365 2063  external force c
+0000ba80: 6f6e 7374 616e 7473 2063 616c 6375 6c61  onstants calcula
+0000ba90: 746f 722e 0a0a 2020 2020 2020 2020 2222  tor...        ""
+0000baa0: 220a 2020 2020 2020 2020 6469 7370 5f64  ".        disp_d
+0000bab0: 6174 6173 6574 203d 2073 656c 662e 5f64  ataset = self._d
+0000bac0: 6174 6173 6574 0a0a 2020 2020 2020 2020  ataset..        
+0000bad0: 6663 335f 6361 6c63 756c 6174 6f72 2c20  fc3_calculator, 
+0000bae0: 6663 335f 6361 6c63 756c 6174 6f72 5f6f  fc3_calculator_o
+0000baf0: 7074 696f 6e73 203d 2073 656c 662e 5f65  ptions = self._e
+0000bb00: 7874 7261 6374 5f66 6332 5f66 6333 5f63  xtract_fc2_fc3_c
+0000bb10: 616c 6375 6c61 746f 7273 280a 2020 2020  alculators(.    
+0000bb20: 2020 2020 2020 2020 6663 5f63 616c 6375          fc_calcu
+0000bb30: 6c61 746f 722c 2066 635f 6361 6c63 756c  lator, fc_calcul
+0000bb40: 6174 6f72 5f6f 7074 696f 6e73 2c20 330a  ator_options, 3.
+0000bb50: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000bb60: 2020 2069 6620 6663 335f 6361 6c63 756c     if fc3_calcul
+0000bb70: 6174 6f72 2069 7320 6e6f 7420 4e6f 6e65  ator is not None
+0000bb80: 3a0a 2020 2020 2020 2020 2020 2020 6469  :.            di
+0000bb90: 7370 732c 2066 6f72 6365 7320 3d20 6765  sps, forces = ge
+0000bba0: 745f 6469 7370 6c61 6365 6d65 6e74 735f  t_displacements_
+0000bbb0: 616e 645f 666f 7263 6573 5f66 6333 2864  and_forces_fc3(d
+0000bbc0: 6973 705f 6461 7461 7365 7429 0a20 2020  isp_dataset).   
+0000bbd0: 2020 2020 2020 2020 2066 6332 2c20 6663           fc2, fc
+0000bbe0: 3320 3d20 6765 745f 6663 3328 0a20 2020  3 = get_fc3(.   
+0000bbf0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000bc00: 662e 5f73 7570 6572 6365 6c6c 2c0a 2020  f._supercell,.  
+0000bc10: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000bc20: 6c66 2e5f 7072 696d 6974 6976 652c 0a20  lf._primitive,. 
+0000bc30: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000bc40: 6973 7073 2c0a 2020 2020 2020 2020 2020  isps,.          
+0000bc50: 2020 2020 2020 666f 7263 6573 2c0a 2020        forces,.  
+0000bc60: 2020 2020 2020 2020 2020 2020 2020 6663                fc
+0000bc70: 5f63 616c 6375 6c61 746f 723d 6663 335f  _calculator=fc3_
+0000bc80: 6361 6c63 756c 6174 6f72 2c0a 2020 2020  calculator,.    
+0000bc90: 2020 2020 2020 2020 2020 2020 6663 5f63              fc_c
+0000bca0: 616c 6375 6c61 746f 725f 6f70 7469 6f6e  alculator_option
+0000bcb0: 733d 6663 335f 6361 6c63 756c 6174 6f72  s=fc3_calculator
+0000bcc0: 5f6f 7074 696f 6e73 2c0a 2020 2020 2020  _options,.      
+0000bcd0: 2020 2020 2020 2020 2020 6973 5f63 6f6d            is_com
+0000bce0: 7061 6374 5f66 633d 6973 5f63 6f6d 7061  pact_fc=is_compa
+0000bcf0: 6374 5f66 632c 0a20 2020 2020 2020 2020  ct_fc,.         
+0000bd00: 2020 2020 2020 206c 6f67 5f6c 6576 656c         log_level
+0000bd10: 3d73 656c 662e 5f6c 6f67 5f6c 6576 656c  =self._log_level
+0000bd20: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+0000bd30: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000bd40: 2020 2020 2020 2020 2020 6966 2022 6469            if "di
+0000bd50: 7370 6c61 6365 6d65 6e74 7322 2069 6e20  splacements" in 
+0000bd60: 6469 7370 5f64 6174 6173 6574 3a0a 2020  disp_dataset:.  
+0000bd70: 2020 2020 2020 2020 2020 2020 2020 6d73                ms
+0000bd80: 6720 3d20 280a 2020 2020 2020 2020 2020  g = (.          
+0000bd90: 2020 2020 2020 2020 2020 2266 635f 6361            "fc_ca
+0000bda0: 6c63 756c 6174 6f72 2068 6173 2074 6f20  lculator has to 
+0000bdb0: 6265 2073 6574 2074 6f20 7072 6f64 7563  be set to produc
+0000bdc0: 6520 666f 7263 6520 220a 2020 2020 2020  e force ".      
+0000bdd0: 2020 2020 2020 2020 2020 2020 2020 2263                "c
+0000bde0: 6f6e 7374 616e 7320 6672 6f6d 2074 6869  onstans from thi
+0000bdf0: 7320 6461 7461 7365 742e 220a 2020 2020  s dataset.".    
+0000be00: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000be10: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+0000be20: 6973 6520 466f 7263 6543 616c 6375 6c61  ise ForceCalcula
+0000be30: 746f 7252 6571 7569 7265 6445 7272 6f72  torRequiredError
+0000be40: 286d 7367 290a 2020 2020 2020 2020 2020  (msg).          
+0000be50: 2020 6663 322c 2066 6333 203d 2067 6574    fc2, fc3 = get
+0000be60: 5f70 686f 6e6f 3370 795f 6663 3328 0a20  _phono3py_fc3(. 
+0000be70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000be80: 656c 662e 5f73 7570 6572 6365 6c6c 2c0a  elf._supercell,.
+0000be90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bea0: 7365 6c66 2e5f 7072 696d 6974 6976 652c  self._primitive,
+0000beb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bec0: 2064 6973 705f 6461 7461 7365 742c 0a20   disp_dataset,. 
+0000bed0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000bee0: 656c 662e 5f73 796d 6d65 7472 792c 0a20  elf._symmetry,. 
+0000bef0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000bf00: 735f 636f 6d70 6163 745f 6663 3d69 735f  s_compact_fc=is_
+0000bf10: 636f 6d70 6163 745f 6663 2c0a 2020 2020  compact_fc,.    
+0000bf20: 2020 2020 2020 2020 2020 2020 7665 7262              verb
+0000bf30: 6f73 653d 7365 6c66 2e5f 6c6f 675f 6c65  ose=self._log_le
+0000bf40: 7665 6c2c 0a20 2020 2020 2020 2020 2020  vel,.           
+0000bf50: 2029 0a20 2020 2020 2020 2020 2020 2069   ).            i
+0000bf60: 6620 7379 6d6d 6574 7269 7a65 5f66 6333  f symmetrize_fc3
+0000bf70: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
+0000bf80: 2020 2069 6620 6973 5f63 6f6d 7061 6374     if is_compact
+0000bf90: 5f66 633a 0a20 2020 2020 2020 2020 2020  _fc:.           
+0000bfa0: 2020 2020 2020 2020 2073 6574 5f74 7261           set_tra
+0000bfb0: 6e73 6c61 7469 6f6e 616c 5f69 6e76 6172  nslational_invar
+0000bfc0: 6961 6e63 655f 636f 6d70 6163 745f 6663  iance_compact_fc
+0000bfd0: 3328 6663 332c 2073 656c 662e 5f70 7269  3(fc3, self._pri
+0000bfe0: 6d69 7469 7665 290a 2020 2020 2020 2020  mitive).        
+0000bff0: 2020 2020 2020 2020 2020 2020 7365 745f              set_
+0000c000: 7065 726d 7574 6174 696f 6e5f 7379 6d6d  permutation_symm
+0000c010: 6574 7279 5f63 6f6d 7061 6374 5f66 6333  etry_compact_fc3
+0000c020: 2866 6333 2c20 7365 6c66 2e5f 7072 696d  (fc3, self._prim
+0000c030: 6974 6976 6529 0a20 2020 2020 2020 2020  itive).         
+0000c040: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000c050: 6c66 2e5f 6663 3220 6973 204e 6f6e 653a  lf._fc2 is None:
+0000c060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c070: 2020 2020 2020 2020 2073 796d 6d65 7472           symmetr
+0000c080: 697a 655f 636f 6d70 6163 745f 666f 7263  ize_compact_forc
+0000c090: 655f 636f 6e73 7461 6e74 7328 6663 322c  e_constants(fc2,
+0000c0a0: 2073 656c 662e 5f70 7269 6d69 7469 7665   self._primitive
+0000c0b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000c0c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000c0d0: 2020 2020 2020 2020 2020 2020 7365 745f              set_
+0000c0e0: 7472 616e 736c 6174 696f 6e61 6c5f 696e  translational_in
+0000c0f0: 7661 7269 616e 6365 5f66 6333 2866 6333  variance_fc3(fc3
+0000c100: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000c110: 2020 2020 2020 7365 745f 7065 726d 7574        set_permut
+0000c120: 6174 696f 6e5f 7379 6d6d 6574 7279 5f66  ation_symmetry_f
+0000c130: 6333 2866 6333 290a 2020 2020 2020 2020  c3(fc3).        
+0000c140: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000c150: 656c 662e 5f66 6332 2069 7320 4e6f 6e65  elf._fc2 is None
+0000c160: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000c170: 2020 2020 2020 2020 2020 7379 6d6d 6574            symmet
+0000c180: 7269 7a65 5f66 6f72 6365 5f63 6f6e 7374  rize_force_const
+0000c190: 616e 7473 2866 6332 290a 0a20 2020 2020  ants(fc2)..     
+0000c1a0: 2020 2023 2053 6574 2066 6332 2061 6e64     # Set fc2 and
+0000c1b0: 2066 6333 0a20 2020 2020 2020 2073 656c   fc3.        sel
+0000c1c0: 662e 5f66 6333 203d 2066 6333 0a0a 2020  f._fc3 = fc3..  
+0000c1d0: 2020 2020 2020 2320 6663 3220 6173 206f        # fc2 as o
+0000c1e0: 6274 6169 6e65 6420 6162 6f76 6520 7769  btained above wi
+0000c1f0: 6c6c 206e 6f74 2062 6520 7365 7420 7768  ll not be set wh
+0000c200: 656e 2022 7c22 2069 6e20 6663 2d63 616c  en "|" in fc-cal
+0000c210: 6375 6c61 746f 7220 7365 7474 696e 672e  culator setting.
+0000c220: 0a20 2020 2020 2020 2069 6620 6663 5f63  .        if fc_c
+0000c230: 616c 6375 6c61 746f 7220 6973 206e 6f74  alculator is not
+0000c240: 204e 6f6e 6520 616e 6420 227c 2220 696e   None and "|" in
+0000c250: 2066 635f 6361 6c63 756c 6174 6f72 3a0a   fc_calculator:.
+0000c260: 2020 2020 2020 2020 2020 2020 6663 3220              fc2 
+0000c270: 3d20 4e6f 6e65 0a20 2020 2020 2020 2069  = None.        i
+0000c280: 6620 6663 5f63 616c 6375 6c61 746f 725f  f fc_calculator_
+0000c290: 6f70 7469 6f6e 7320 6973 206e 6f74 204e  options is not N
+0000c2a0: 6f6e 6520 616e 6420 227c 2220 696e 2066  one and "|" in f
+0000c2b0: 635f 6361 6c63 756c 6174 6f72 5f6f 7074  c_calculator_opt
+0000c2c0: 696f 6e73 3a0a 2020 2020 2020 2020 2020  ions:.          
+0000c2d0: 2020 6663 3220 3d20 4e6f 6e65 0a0a 2020    fc2 = None..  
+0000c2e0: 2020 2020 2020 2320 4e6f 726d 616c 6c79        # Normally
+0000c2f0: 2073 656c 662e 5f66 6332 2069 7320 6f76   self._fc2 is ov
+0000c300: 6572 7772 6974 7465 6e20 696e 2070 726f  erwritten in pro
+0000c310: 6475 6365 5f66 6332 0a20 2020 2020 2020  duce_fc2.       
+0000c320: 2069 6620 7365 6c66 2e5f 6663 3220 6973   if self._fc2 is
+0000c330: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000c340: 2020 2073 656c 662e 5f66 6332 203d 2066     self._fc2 = f
+0000c350: 6332 0a0a 2020 2020 6465 6620 7072 6f64  c2..    def prod
+0000c360: 7563 655f 6663 3228 0a20 2020 2020 2020  uce_fc2(.       
+0000c370: 2073 656c 662c 0a20 2020 2020 2020 2073   self,.        s
+0000c380: 796d 6d65 7472 697a 655f 6663 323d 4661  ymmetrize_fc2=Fa
+0000c390: 6c73 652c 0a20 2020 2020 2020 2069 735f  lse,.        is_
+0000c3a0: 636f 6d70 6163 745f 6663 3d46 616c 7365  compact_fc=False
+0000c3b0: 2c0a 2020 2020 2020 2020 6663 5f63 616c  ,.        fc_cal
+0000c3c0: 6375 6c61 746f 723d 4e6f 6e65 2c0a 2020  culator=None,.  
+0000c3d0: 2020 2020 2020 6663 5f63 616c 6375 6c61        fc_calcula
+0000c3e0: 746f 725f 6f70 7469 6f6e 733d 4e6f 6e65  tor_options=None
+0000c3f0: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+0000c400: 2022 2222 4361 6c63 756c 6174 6520 6663   """Calculate fc
+0000c410: 3220 6672 6f6d 2064 6973 706c 6163 656d  2 from displacem
+0000c420: 656e 7473 2061 6e64 2066 6f72 6365 732e  ents and forces.
+0000c430: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+0000c440: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+0000c450: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+0000c460: 7379 6d6d 6574 7269 7a65 5f66 6332 203a  symmetrize_fc2 :
+0000c470: 2062 6f6f 6c0a 2020 2020 2020 2020 2020   bool.          
+0000c480: 2020 4f6e 6c79 2066 6f72 2074 7970 6520    Only for type 
+0000c490: 3120 6469 7370 6c61 6365 6d65 6e74 5f64  1 displacement_d
+0000c4a0: 6174 6173 6574 2c20 7472 616e 736c 6174  ataset, translat
+0000c4b0: 696f 6e61 6c20 616e 640a 2020 2020 2020  ional and.      
+0000c4c0: 2020 2020 2020 7065 726d 7574 6174 696f        permutatio
+0000c4d0: 6e20 7379 6d6d 6574 7269 6573 2061 7265  n symmetries are
+0000c4e0: 2061 7070 6c69 6564 2061 6674 6572 2063   applied after c
+0000c4f0: 7265 6174 696e 6720 6663 332e 2054 6869  reating fc3. Thi
+0000c500: 730a 2020 2020 2020 2020 2020 2020 7379  s.            sy
+0000c510: 6d6d 6574 7269 7a61 7469 6f6e 2069 7320  mmetrization is 
+0000c520: 6e6f 7420 7665 7279 2073 6f70 6869 7374  not very sophist
+0000c530: 6963 6174 6564 2061 6e64 2063 616e 2062  icated and can b
+0000c540: 7265 616b 2073 7061 6365 0a20 2020 2020  reak space.     
+0000c550: 2020 2020 2020 2067 726f 7570 2073 796d         group sym
+0000c560: 6d65 7472 792c 2062 7574 206f 6674 656e  metry, but often
+0000c570: 2075 7365 6675 6c2e 2049 6620 6265 7474   useful. If bett
+0000c580: 6572 2073 796d 6d65 7472 697a 6174 696f  er symmetrizatio
+0000c590: 6e20 6973 0a20 2020 2020 2020 2020 2020  n is.           
+0000c5a0: 2065 7870 6563 7465 642c 2069 7420 6973   expected, it is
+0000c5b0: 2072 6563 6f6d 6d65 6e64 6564 2074 6f20   recommended to 
+0000c5c0: 7573 6520 6578 7465 726e 616c 2066 6f72  use external for
+0000c5d0: 6365 2063 6f6e 7374 616e 7473 0a20 2020  ce constants.   
+0000c5e0: 2020 2020 2020 2020 2063 616c 6375 6c61           calcula
+0000c5f0: 746f 7220 7375 6368 2061 7320 414c 4d2e  tor such as ALM.
+0000c600: 2044 6566 6175 6c74 2069 7320 4661 6c73   Default is Fals
+0000c610: 652e 0a20 2020 2020 2020 2069 735f 636f  e..        is_co
+0000c620: 6d70 6163 745f 6663 203a 2062 6f6f 6c0a  mpact_fc : bool.
+0000c630: 2020 2020 2020 2020 2020 2020 6663 3220              fc2 
+0000c640: 7368 6170 6520 6973 0a20 2020 2020 2020  shape is.       
+0000c650: 2020 2020 2020 2020 2046 616c 7365 3a20           False: 
+0000c660: 2873 7570 6572 6365 6c6c 2c20 7375 7065  (supercell, supe
+0000c670: 6365 6c6c 2c20 332c 2033 290a 2020 2020  cell, 3, 3).    
+0000c680: 2020 2020 2020 2020 2020 2020 5472 7565              True
+0000c690: 3a20 2870 7269 6d69 7469 7665 2c20 7375  : (primitive, su
+0000c6a0: 7065 6365 6c6c 2c20 332c 2033 290a 2020  pecell, 3, 3).  
+0000c6b0: 2020 2020 2020 2020 2020 7768 6572 6520            where 
+0000c6c0: 2773 7570 6572 6365 6c6c 2720 616e 6420  'supercell' and 
+0000c6d0: 2770 7269 6d69 7469 7665 2720 696e 6469  'primitive' indi
+0000c6e0: 6361 7465 206e 756d 6265 7220 6f66 2061  cate number of a
+0000c6f0: 746f 6d73 2069 6e20 7468 6573 650a 2020  toms in these.  
+0000c700: 2020 2020 2020 2020 2020 6365 6c6c 732e            cells.
+0000c710: 2044 6566 6175 6c74 2069 7320 4661 6c73   Default is Fals
+0000c720: 652e 0a20 2020 2020 2020 2066 635f 6361  e..        fc_ca
+0000c730: 6c63 756c 6174 6f72 203a 2073 7472 206f  lculator : str o
+0000c740: 7220 4e6f 6e65 0a20 2020 2020 2020 2020  r None.         
+0000c750: 2020 2046 6f72 6365 2063 6f6e 7374 616e     Force constan
+0000c760: 7473 2063 616c 6375 6c61 746f 7220 6769  ts calculator gi
+0000c770: 7665 6e20 6279 2073 7472 2e0a 2020 2020  ven by str..    
+0000c780: 2020 2020 6663 5f63 616c 6375 6c61 746f      fc_calculato
+0000c790: 725f 6f70 7469 6f6e 7320 3a20 6469 6374  r_options : dict
+0000c7a0: 0a20 2020 2020 2020 2020 2020 204f 7074  .            Opt
+0000c7b0: 696f 6e73 2066 6f72 2065 7874 6572 6e61  ions for externa
+0000c7c0: 6c20 666f 7263 6520 636f 6e73 7461 6e74  l force constant
+0000c7d0: 7320 6361 6c63 756c 6174 6f72 2e0a 0a20  s calculator... 
+0000c7e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000c7f0: 2020 2069 6620 7365 6c66 2e5f 7068 6f6e     if self._phon
+0000c800: 6f6e 5f64 6174 6173 6574 2069 7320 4e6f  on_dataset is No
+0000c810: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000c820: 6469 7370 5f64 6174 6173 6574 203d 2073  disp_dataset = s
+0000c830: 656c 662e 5f64 6174 6173 6574 0a20 2020  elf._dataset.   
+0000c840: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000c850: 2020 2020 2020 2064 6973 705f 6461 7461         disp_data
+0000c860: 7365 7420 3d20 7365 6c66 2e5f 7068 6f6e  set = self._phon
+0000c870: 6f6e 5f64 6174 6173 6574 0a0a 2020 2020  on_dataset..    
+0000c880: 2020 2020 6966 2069 735f 636f 6d70 6163      if is_compac
+0000c890: 745f 6663 3a0a 2020 2020 2020 2020 2020  t_fc:.          
+0000c8a0: 2020 7032 735f 6d61 7020 3d20 7365 6c66    p2s_map = self
+0000c8b0: 2e5f 7068 6f6e 6f6e 5f70 7269 6d69 7469  ._phonon_primiti
+0000c8c0: 7665 2e70 3273 5f6d 6170 0a20 2020 2020  ve.p2s_map.     
+0000c8d0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000c8e0: 2020 2020 2070 3273 5f6d 6170 203d 204e       p2s_map = N
+0000c8f0: 6f6e 650a 0a20 2020 2020 2020 2066 6332  one..        fc2
+0000c900: 5f63 616c 6375 6c61 746f 722c 2066 6332  _calculator, fc2
+0000c910: 5f63 616c 6375 6c61 746f 725f 6f70 7469  _calculator_opti
+0000c920: 6f6e 7320 3d20 7365 6c66 2e5f 6578 7472  ons = self._extr
+0000c930: 6163 745f 6663 325f 6663 335f 6361 6c63  act_fc2_fc3_calc
+0000c940: 756c 6174 6f72 7328 0a20 2020 2020 2020  ulators(.       
+0000c950: 2020 2020 2066 635f 6361 6c63 756c 6174       fc_calculat
+0000c960: 6f72 2c20 6663 5f63 616c 6375 6c61 746f  or, fc_calculato
+0000c970: 725f 6f70 7469 6f6e 732c 2032 0a20 2020  r_options, 2.   
+0000c980: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0000c990: 6966 2066 6332 5f63 616c 6375 6c61 746f  if fc2_calculato
+0000c9a0: 7220 6973 206e 6f74 204e 6f6e 653a 0a20  r is not None:. 
+0000c9b0: 2020 2020 2020 2020 2020 2064 6973 7073             disps
+0000c9c0: 2c20 666f 7263 6573 203d 2067 6574 5f64  , forces = get_d
+0000c9d0: 6973 706c 6163 656d 656e 7473 5f61 6e64  isplacements_and
+0000c9e0: 5f66 6f72 6365 7328 6469 7370 5f64 6174  _forces(disp_dat
+0000c9f0: 6173 6574 290a 2020 2020 2020 2020 2020  aset).          
+0000ca00: 2020 7365 6c66 2e5f 6663 3220 3d20 6765    self._fc2 = ge
+0000ca10: 745f 6663 3228 0a20 2020 2020 2020 2020  t_fc2(.         
+0000ca20: 2020 2020 2020 2073 656c 662e 5f70 686f         self._pho
+0000ca30: 6e6f 6e5f 7375 7065 7263 656c 6c2c 0a20  non_supercell,. 
+0000ca40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000ca50: 656c 662e 5f70 686f 6e6f 6e5f 7072 696d  elf._phonon_prim
+0000ca60: 6974 6976 652c 0a20 2020 2020 2020 2020  itive,.         
+0000ca70: 2020 2020 2020 2064 6973 7073 2c0a 2020         disps,.  
+0000ca80: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0000ca90: 7263 6573 2c0a 2020 2020 2020 2020 2020  rces,.          
+0000caa0: 2020 2020 2020 6663 5f63 616c 6375 6c61        fc_calcula
+0000cab0: 746f 723d 6663 325f 6361 6c63 756c 6174  tor=fc2_calculat
+0000cac0: 6f72 2c0a 2020 2020 2020 2020 2020 2020  or,.            
+0000cad0: 2020 2020 6663 5f63 616c 6375 6c61 746f      fc_calculato
+0000cae0: 725f 6f70 7469 6f6e 733d 6663 325f 6361  r_options=fc2_ca
+0000caf0: 6c63 756c 6174 6f72 5f6f 7074 696f 6e73  lculator_options
+0000cb00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000cb10: 2020 6174 6f6d 5f6c 6973 743d 7032 735f    atom_list=p2s_
+0000cb20: 6d61 702c 0a20 2020 2020 2020 2020 2020  map,.           
+0000cb30: 2020 2020 206c 6f67 5f6c 6576 656c 3d73       log_level=s
+0000cb40: 656c 662e 5f6c 6f67 5f6c 6576 656c 2c0a  elf._log_level,.
+0000cb50: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000cb60: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000cb70: 2020 2020 2020 2020 6966 2022 6469 7370          if "disp
+0000cb80: 6c61 6365 6d65 6e74 7322 2069 6e20 6469  lacements" in di
+0000cb90: 7370 5f64 6174 6173 6574 3a0a 2020 2020  sp_dataset:.    
+0000cba0: 2020 2020 2020 2020 2020 2020 6d73 6720              msg 
+0000cbb0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+0000cbc0: 2020 2020 2020 2020 2266 635f 6361 6c63          "fc_calc
+0000cbd0: 756c 6174 6f72 2068 6173 2074 6f20 6265  ulator has to be
+0000cbe0: 2073 6574 2074 6f20 7072 6f64 7563 6520   set to produce 
+0000cbf0: 666f 7263 6520 220a 2020 2020 2020 2020  force ".        
+0000cc00: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
+0000cc10: 7374 616e 7320 6672 6f6d 2074 6869 7320  stans from this 
+0000cc20: 6461 7461 7365 7420 666f 7220 6663 322e  dataset for fc2.
+0000cc30: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000cc40: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000cc50: 2020 2020 7261 6973 6520 5275 6e74 696d      raise Runtim
+0000cc60: 6545 7272 6f72 286d 7367 290a 2020 2020  eError(msg).    
+0000cc70: 2020 2020 2020 2020 7365 6c66 2e5f 6663          self._fc
+0000cc80: 3220 3d20 6765 745f 7068 6f6e 6f70 795f  2 = get_phonopy_
+0000cc90: 6663 3228 0a20 2020 2020 2020 2020 2020  fc2(.           
+0000cca0: 2020 2020 2073 656c 662e 5f70 686f 6e6f       self._phono
+0000ccb0: 6e5f 7375 7065 7263 656c 6c2c 0a20 2020  n_supercell,.   
+0000ccc0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000ccd0: 662e 5f70 686f 6e6f 6e5f 7375 7065 7263  f._phonon_superc
+0000cce0: 656c 6c5f 7379 6d6d 6574 7279 2c0a 2020  ell_symmetry,.  
+0000ccf0: 2020 2020 2020 2020 2020 2020 2020 6469                di
+0000cd00: 7370 5f64 6174 6173 6574 2c0a 2020 2020  sp_dataset,.    
+0000cd10: 2020 2020 2020 2020 2020 2020 6174 6f6d              atom
+0000cd20: 5f6c 6973 743d 7032 735f 6d61 702c 0a20  _list=p2s_map,. 
+0000cd30: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000cd40: 2020 2020 2020 2020 2069 6620 7379 6d6d           if symm
+0000cd50: 6574 7269 7a65 5f66 6332 3a0a 2020 2020  etrize_fc2:.    
+0000cd60: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+0000cd70: 735f 636f 6d70 6163 745f 6663 3a0a 2020  s_compact_fc:.  
+0000cd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd90: 2020 7379 6d6d 6574 7269 7a65 5f63 6f6d    symmetrize_com
+0000cda0: 7061 6374 5f66 6f72 6365 5f63 6f6e 7374  pact_force_const
+0000cdb0: 616e 7473 280a 2020 2020 2020 2020 2020  ants(.          
+0000cdc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000cdd0: 6c66 2e5f 6663 322c 2073 656c 662e 5f70  lf._fc2, self._p
+0000cde0: 686f 6e6f 6e5f 7072 696d 6974 6976 650a  honon_primitive.
+0000cdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce00: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000ce10: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000ce20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce30: 7379 6d6d 6574 7269 7a65 5f66 6f72 6365  symmetrize_force
+0000ce40: 5f63 6f6e 7374 616e 7473 2873 656c 662e  _constants(self.
+0000ce50: 5f66 6332 290a 0a20 2020 2064 6566 2063  _fc2)..    def c
+0000ce60: 7574 6f66 665f 6663 335f 6279 5f7a 6572  utoff_fc3_by_zer
+0000ce70: 6f28 7365 6c66 2c20 6375 746f 6666 5f64  o(self, cutoff_d
+0000ce80: 6973 7461 6e63 652c 2066 6333 3d4e 6f6e  istance, fc3=Non
+0000ce90: 6529 3a0a 2020 2020 2020 2020 2222 2253  e):.        """S
+0000cea0: 6574 207a 6572 6f20 746f 2066 6333 2065  et zero to fc3 e
+0000ceb0: 6c65 6d65 6e74 7320 6f75 7420 6f66 2063  lements out of c
+0000cec0: 7574 6f66 6620 6469 7374 616e 6365 2e0a  utoff distance..
+0000ced0: 0a20 2020 2020 2020 204e 6f74 650a 2020  .        Note.  
+0000cee0: 2020 2020 2020 2d2d 2d2d 0a20 2020 2020        ----.     
+0000cef0: 2020 2066 6333 2069 7320 6f76 6572 7772     fc3 is overwr
+0000cf00: 6974 7465 6e2e 0a0a 2020 2020 2020 2020  itten...        
+0000cf10: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+0000cf20: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+0000cf30: 2020 2020 2020 6375 746f 6666 5f64 6973        cutoff_dis
+0000cf40: 7461 6e63 6520 3a20 666c 6f61 740a 2020  tance : float.  
+0000cf50: 2020 2020 2020 2020 2020 4166 7465 7220            After 
+0000cf60: 6372 6561 7469 6e67 2066 6f72 6365 2063  creating force c
+0000cf70: 6f6e 7374 616e 7473 2c20 6663 2065 6c65  onstants, fc ele
+0000cf80: 6d65 6e74 7320 7768 6572 6520 616e 7920  ments where any 
+0000cf90: 7061 6972 0a20 2020 2020 2020 2020 2020  pair.           
+0000cfa0: 2064 6973 7461 6e63 6520 696e 2061 746f   distance in ato
+0000cfb0: 6d20 7472 6970 6c65 7473 206c 6172 6765  m triplets large
+0000cfc0: 7220 7468 616e 2063 7574 6f66 665f 6469  r than cutoff_di
+0000cfd0: 7374 616e 6365 2061 7265 2073 6574 207a  stance are set z
+0000cfe0: 6572 6f2e 0a0a 2020 2020 2020 2020 2222  ero...        ""
+0000cff0: 220a 2020 2020 2020 2020 6966 2066 6333  ".        if fc3
+0000d000: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0000d010: 2020 2020 2020 5f66 6333 203d 2073 656c        _fc3 = sel
+0000d020: 662e 5f66 6333 0a20 2020 2020 2020 2065  f._fc3.        e
+0000d030: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000d040: 205f 6663 3320 3d20 6663 330a 2020 2020   _fc3 = fc3.    
+0000d050: 2020 2020 6375 746f 6666 5f66 6333 5f62      cutoff_fc3_b
+0000d060: 795f 7a65 726f 280a 2020 2020 2020 2020  y_zero(.        
+0000d070: 2020 2020 5f66 6333 2c0a 2020 2020 2020      _fc3,.      
+0000d080: 2020 2020 2020 7365 6c66 2e5f 7375 7065        self._supe
+0000d090: 7263 656c 6c2c 0a20 2020 2020 2020 2020  rcell,.         
+0000d0a0: 2020 2063 7574 6f66 665f 6469 7374 616e     cutoff_distan
+0000d0b0: 6365 2c0a 2020 2020 2020 2020 2020 2020  ce,.            
+0000d0c0: 7032 735f 6d61 703d 7365 6c66 2e5f 7072  p2s_map=self._pr
+0000d0d0: 696d 6974 6976 652e 7032 735f 6d61 702c  imitive.p2s_map,
+0000d0e0: 0a20 2020 2020 2020 2020 2020 2073 796d  .            sym
+0000d0f0: 7072 6563 3d73 656c 662e 5f73 796d 7072  prec=self._sympr
+0000d100: 6563 2c0a 2020 2020 2020 2020 290a 0a20  ec,.        ).. 
+0000d110: 2020 2064 6566 2073 6574 5f70 6572 6d75     def set_permu
+0000d120: 7461 7469 6f6e 5f73 796d 6d65 7472 7928  tation_symmetry(
+0000d130: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000d140: 2222 456e 666f 7263 6520 7065 726d 7574  ""Enforce permut
+0000d150: 6174 696f 6e20 7379 6d6d 6574 7279 2074  ation symmetry t
+0000d160: 6f20 6663 3220 616e 6420 6663 332e 2222  o fc2 and fc3.""
+0000d170: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
+0000d180: 662e 5f66 6332 2069 7320 6e6f 7420 4e6f  f._fc2 is not No
+0000d190: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000d1a0: 7365 745f 7065 726d 7574 6174 696f 6e5f  set_permutation_
+0000d1b0: 7379 6d6d 6574 7279 2873 656c 662e 5f66  symmetry(self._f
+0000d1c0: 6332 290a 2020 2020 2020 2020 6966 2073  c2).        if s
+0000d1d0: 656c 662e 5f66 6333 2069 7320 6e6f 7420  elf._fc3 is not 
+0000d1e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000d1f0: 2020 7365 745f 7065 726d 7574 6174 696f    set_permutatio
+0000d200: 6e5f 7379 6d6d 6574 7279 5f66 6333 2873  n_symmetry_fc3(s
+0000d210: 656c 662e 5f66 6333 290a 0a20 2020 2064  elf._fc3)..    d
+0000d220: 6566 2073 6574 5f74 7261 6e73 6c61 7469  ef set_translati
+0000d230: 6f6e 616c 5f69 6e76 6172 6961 6e63 6528  onal_invariance(
+0000d240: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000d250: 2222 456e 666f 7263 6520 7472 616e 736c  ""Enforce transl
+0000d260: 6174 696f 6e20 696e 7661 7269 616e 6365  ation invariance
+0000d270: 2e0a 0a20 2020 2020 2020 2054 6869 7320  ...        This 
+0000d280: 7375 6274 7261 6374 7320 6472 6966 7420  subtracts drift 
+0000d290: 6469 7669 6465 6420 6279 206e 756d 6265  divided by numbe
+0000d2a0: 7220 6f66 2065 6c65 6d65 6e74 7320 696e  r of elements in
+0000d2b0: 2065 6163 6820 726f 7720 616e 640a 2020   each row and.  
+0000d2c0: 2020 2020 2020 636f 6c75 6d6e 2e0a 0a20        column... 
+0000d2d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000d2e0: 2020 2069 6620 7365 6c66 2e5f 6663 3220     if self._fc2 
+0000d2f0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000d300: 2020 2020 2020 2020 2073 6574 5f74 7261           set_tra
+0000d310: 6e73 6c61 7469 6f6e 616c 5f69 6e76 6172  nslational_invar
+0000d320: 6961 6e63 6528 7365 6c66 2e5f 6663 3229  iance(self._fc2)
+0000d330: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000d340: 2e5f 6663 3320 6973 206e 6f74 204e 6f6e  ._fc3 is not Non
+0000d350: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0000d360: 6574 5f74 7261 6e73 6c61 7469 6f6e 616c  et_translational
+0000d370: 5f69 6e76 6172 6961 6e63 655f 6663 3328  _invariance_fc3(
+0000d380: 7365 6c66 2e5f 6663 3329 0a0a 2020 2020  self._fc3)..    
+0000d390: 6465 6620 7275 6e5f 696d 6167 5f73 656c  def run_imag_sel
+0000d3a0: 665f 656e 6572 6779 280a 2020 2020 2020  f_energy(.      
+0000d3b0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+0000d3c0: 6772 6964 5f70 6f69 6e74 732c 0a20 2020  grid_points,.   
+0000d3d0: 2020 2020 2074 656d 7065 7261 7475 7265       temperature
+0000d3e0: 732c 0a20 2020 2020 2020 2066 7265 7175  s,.        frequ
+0000d3f0: 656e 6379 5f70 6f69 6e74 733d 4e6f 6e65  ency_points=None
+0000d400: 2c0a 2020 2020 2020 2020 6672 6571 7565  ,.        freque
+0000d410: 6e63 795f 7374 6570 3d4e 6f6e 652c 0a20  ncy_step=None,. 
+0000d420: 2020 2020 2020 206e 756d 5f66 7265 7175         num_frequ
+0000d430: 656e 6379 5f70 6f69 6e74 733d 4e6f 6e65  ency_points=None
+0000d440: 2c0a 2020 2020 2020 2020 6e75 6d5f 706f  ,.        num_po
+0000d450: 696e 7473 5f69 6e5f 6261 7463 683d 4e6f  ints_in_batch=No
+0000d460: 6e65 2c0a 2020 2020 2020 2020 6672 6571  ne,.        freq
+0000d470: 7565 6e63 795f 706f 696e 7473 5f61 745f  uency_points_at_
+0000d480: 6261 6e64 733d 4661 6c73 652c 0a20 2020  bands=False,.   
+0000d490: 2020 2020 2073 6361 7474 6572 696e 675f       scattering_
+0000d4a0: 6576 656e 745f 636c 6173 733d 4e6f 6e65  event_class=None
+0000d4b0: 2c0a 2020 2020 2020 2020 7772 6974 655f  ,.        write_
+0000d4c0: 7478 743d 4661 6c73 652c 0a20 2020 2020  txt=False,.     
+0000d4d0: 2020 2077 7269 7465 5f67 616d 6d61 5f64     write_gamma_d
+0000d4e0: 6574 6169 6c3d 4661 6c73 652c 0a20 2020  etail=False,.   
+0000d4f0: 2020 2020 206b 6565 705f 6761 6d6d 615f       keep_gamma_
+0000d500: 6465 7461 696c 3d46 616c 7365 2c0a 2020  detail=False,.  
+0000d510: 2020 2020 2020 6f75 7470 7574 5f66 696c        output_fil
+0000d520: 656e 616d 653d 4e6f 6e65 2c0a 2020 2020  ename=None,.    
+0000d530: 293a 0a20 2020 2020 2020 2022 2222 4361  ):.        """Ca
+0000d540: 6c63 756c 6174 6520 696d 6167 696e 6172  lculate imaginar
+0000d550: 7920 7061 7274 206f 6620 7365 6c66 2d65  y part of self-e
+0000d560: 6e65 7267 7920 6f66 2062 7562 626c 6520  nergy of bubble 
+0000d570: 6469 6167 7261 6d20 2847 616d 6d61 292e  diagram (Gamma).
+0000d580: 0a0a 2020 2020 2020 2020 5069 203d 2044  ..        Pi = D
+0000d590: 656c 7461 202d 2069 2047 616d 6d61 2e0a  elta - i Gamma..
+0000d5a0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+0000d5b0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+0000d5c0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2067  ------.        g
+0000d5d0: 7269 645f 706f 696e 7473 203a 2061 7272  rid_points : arr
+0000d5e0: 6179 5f6c 696b 650a 2020 2020 2020 2020  ay_like.        
+0000d5f0: 2020 2020 4772 6964 2d70 6f69 6e74 2069      Grid-point i
+0000d600: 6e64 6963 6573 2077 6865 7265 2069 6d61  ndices where ima
+0000d610: 6769 6e61 7279 2070 6172 7420 6f66 2073  ginary part of s
+0000d620: 656c 662d 656e 6572 6769 6573 2061 7265  elf-energies are
+0000d630: 0a20 2020 2020 2020 2020 2020 2063 6163  .            cac
+0000d640: 6c63 756c 6174 6564 2e0a 2020 2020 2020  lculated..      
+0000d650: 2020 2020 2020 6474 7970 653d 696e 742c        dtype=int,
+0000d660: 2073 6861 7065 3d28 6772 6964 5f70 6f69   shape=(grid_poi
+0000d670: 6e74 732c 290a 2020 2020 2020 2020 7465  nts,).        te
+0000d680: 6d70 6572 6174 7572 6573 203a 2061 7272  mperatures : arr
+0000d690: 6179 5f6c 696b 650a 2020 2020 2020 2020  ay_like.        
+0000d6a0: 2020 2020 5465 6d70 6572 6174 7572 6573      Temperatures
+0000d6b0: 2077 6865 7265 2069 6d61 6769 6e61 7279   where imaginary
+0000d6c0: 2070 6172 7420 6f66 2073 656c 662d 656e   part of self-en
+0000d6d0: 6572 6769 6573 2061 7265 2063 616c 6375  ergies are calcu
+0000d6e0: 6c61 7465 642e 0a20 2020 2020 2020 2020  lated..         
+0000d6f0: 2020 2064 7479 7065 3d66 6c6f 6174 2c20     dtype=float, 
+0000d700: 7368 6170 653d 2874 656d 7065 7261 7475  shape=(temperatu
+0000d710: 7265 732c 290a 2020 2020 2020 2020 6672  res,).        fr
+0000d720: 6571 7565 6e63 795f 706f 696e 7473 203a  equency_points :
+0000d730: 2061 7272 6179 5f6c 696b 652c 206f 7074   array_like, opt
+0000d740: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+0000d750: 2020 4672 6571 7565 6e63 7920 7361 6d70    Frequency samp
+0000d760: 6c69 6e67 2070 6f69 6e74 732e 2044 6566  ling points. Def
+0000d770: 6175 6c74 2069 7320 4e6f 6e65 2e20 5769  ault is None. Wi
+0000d780: 7468 0a20 2020 2020 2020 2020 2020 2066  th.            f
+0000d790: 7265 7175 656e 6379 5f70 6f69 6e74 735f  requency_points_
+0000d7a0: 6174 5f62 616e 6473 3d46 616c 7365 2061  at_bands=False a
+0000d7b0: 6e64 2066 7265 7175 656e 6379 5f70 6f69  nd frequency_poi
+0000d7c0: 6e74 7320 6973 204e 6f6e 652c 0a20 2020  nts is None,.   
+0000d7d0: 2020 2020 2020 2020 206e 756d 5f66 7265           num_fre
+0000d7e0: 7175 656e 6379 5f70 6f69 6e74 7320 6f72  quency_points or
+0000d7f0: 2066 7265 7175 656e 6379 5f73 7465 7020   frequency_step 
+0000d800: 6973 2075 7365 6420 746f 2067 656e 6572  is used to gener
+0000d810: 6174 6520 756e 6966 6f72 6d0a 2020 2020  ate uniform.    
+0000d820: 2020 2020 2020 2020 6672 6571 7565 6e63          frequenc
+0000d830: 7920 7361 6d70 6c69 6e67 2070 6f69 6e74  y sampling point
+0000d840: 732e 0a20 2020 2020 2020 2020 2020 2064  s..            d
+0000d850: 7479 7065 3d66 6c6f 6174 2c20 7368 6170  type=float, shap
+0000d860: 653d 2866 7265 7175 656e 6379 5f70 6f69  e=(frequency_poi
+0000d870: 6e74 732c 290a 2020 2020 2020 2020 6672  nts,).        fr
+0000d880: 6571 7565 6e63 795f 7374 6570 203a 2066  equency_step : f
+0000d890: 6c6f 6174 2c20 6f70 7469 6f6e 616c 0a20  loat, optional. 
+0000d8a0: 2020 2020 2020 2020 2020 2055 6e69 666f             Unifo
+0000d8b0: 726d 2070 6974 6368 206f 6620 6672 6571  rm pitch of freq
+0000d8c0: 7565 6e63 7920 7361 6d70 6c69 6e67 2070  uency sampling p
+0000d8d0: 6f69 6e74 732e 2044 6566 6175 6c74 2069  oints. Default i
+0000d8e0: 7320 4e6f 6e65 2e20 5468 6973 0a20 2020  s None. This.   
+0000d8f0: 2020 2020 2020 2020 2072 6573 756c 7473           results
+0000d900: 2069 6e20 7573 696e 6720 6e75 6d5f 6672   in using num_fr
+0000d910: 6571 7565 6e63 795f 706f 696e 7473 2e0a  equency_points..
+0000d920: 2020 2020 2020 2020 6e75 6d5f 6672 6571          num_freq
+0000d930: 7565 6e63 795f 706f 696e 7473 3a20 496e  uency_points: In
+0000d940: 742c 206f 7074 696f 6e61 6c0a 2020 2020  t, optional.    
+0000d950: 2020 2020 2020 2020 4e75 6d62 6572 206f          Number o
+0000d960: 6620 7361 6d70 6c69 6e67 2073 616d 706c  f sampling sampl
+0000d970: 696e 6720 706f 696e 7473 2074 6f20 6265  ing points to be
+0000d980: 2075 7365 6420 696e 7374 6561 6420 6f66   used instead of
+0000d990: 0a20 2020 2020 2020 2020 2020 2066 7265  .            fre
+0000d9a0: 7175 656e 6379 5f73 7465 702e 2054 6869  quency_step. Thi
+0000d9b0: 7320 6e75 6d62 6572 2069 6e63 6c75 6465  s number include
+0000d9c0: 7320 656e 6420 706f 696e 7473 2e20 4465  s end points. De
+0000d9d0: 6661 756c 7420 6973 204e 6f6e 652c 0a20  fault is None,. 
+0000d9e0: 2020 2020 2020 2020 2020 2077 6869 6368             which
+0000d9f0: 2067 6976 6573 2032 3031 2e0a 2020 2020   gives 201..    
+0000da00: 2020 2020 6e75 6d5f 706f 696e 7473 5f69      num_points_i
+0000da10: 6e5f 6261 7463 683a 2069 6e74 2c20 6f70  n_batch: int, op
+0000da20: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
+0000da30: 2020 204e 756d 6265 7220 6f66 2073 616d     Number of sam
+0000da40: 706c 696e 6720 706f 696e 7473 2069 6e20  pling points in 
+0000da50: 6f6e 6520 6261 7463 682e 2054 6869 7320  one batch. This 
+0000da60: 6973 2066 6f72 2074 6865 2066 7265 7175  is for the frequ
+0000da70: 656e 6379 0a20 2020 2020 2020 2020 2020  ency.           
+0000da80: 2073 616d 706c 696e 6720 6d6f 6465 2061   sampling mode a
+0000da90: 6e64 2074 6865 2073 616d 706c 696e 6720  nd the sampling 
+0000daa0: 706f 696e 7473 2061 7265 2064 6976 6964  points are divid
+0000dab0: 6564 2069 6e74 6f20 6261 7463 6865 732e  ed into batches.
+0000dac0: 0a20 2020 2020 2020 2020 2020 204c 6167  .            Lag
+0000dad0: 6572 206e 756d 6265 7220 7072 6f76 6964  er number provid
+0000dae0: 6573 2065 6666 6963 6965 6e74 2075 7365  es efficient use
+0000daf0: 206f 6620 6d75 6c74 692d 636f 7265 7320   of multi-cores 
+0000db00: 6275 7420 6d6f 7265 0a20 2020 2020 2020  but more.       
+0000db10: 2020 2020 206d 656d 6f72 7920 6465 6d61       memory dema
+0000db20: 6e64 696e 672e 2044 6566 6175 6c74 2069  nding. Default i
+0000db30: 7320 4e6f 6e65 2c20 7768 6963 6820 6769  s None, which gi
+0000db40: 7665 2074 6865 206e 756d 6265 7220 6f66  ve the number of
+0000db50: 2031 302e 0a20 2020 2020 2020 2066 7265   10..        fre
+0000db60: 7175 656e 6379 5f70 6f69 6e74 735f 6174  quency_points_at
+0000db70: 5f62 616e 6473 203a 2062 6f6f 6c2c 206f  _bands : bool, o
+0000db80: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+0000db90: 2020 2020 5068 6f6e 6f6e 2062 616e 6420      Phonon band 
+0000dba0: 6672 6571 7565 6e63 6965 7320 6172 6520  frequencies are 
+0000dbb0: 7573 6564 2061 7320 6672 6571 7565 6e63  used as frequenc
+0000dbc0: 7920 706f 696e 7473 2077 6865 6e20 5472  y points when Tr
+0000dbd0: 7565 2e0a 2020 2020 2020 2020 2020 2020  ue..            
+0000dbe0: 4465 6661 756c 7420 6973 2046 616c 7365  Default is False
+0000dbf0: 2e0a 2020 2020 2020 2020 7363 6174 7465  ..        scatte
+0000dc00: 7269 6e67 5f65 7665 6e74 5f63 6c61 7373  ring_event_class
+0000dc10: 203a 2069 6e74 2c20 6f70 7469 6f6e 616c   : int, optional
+0000dc20: 0a20 2020 2020 2020 2020 2020 2053 7065  .            Spe
+0000dc30: 6369 6669 6320 6368 6f69 6365 206f 6620  cific choice of 
+0000dc40: 7363 6174 7465 7269 6e67 2065 7665 6e74  scattering event
+0000dc50: 2063 6c61 7373 2c20 3120 6f72 2032 2074   class, 1 or 2 t
+0000dc60: 6861 7420 6973 2073 7065 6369 6669 6564  hat is specified
+0000dc70: 0a20 2020 2020 2020 2020 2020 2031 206f  .            1 o
+0000dc80: 7220 322c 2072 6573 7065 6374 6976 656c  r 2, respectivel
+0000dc90: 792e 2054 6865 2072 6573 756c 7420 6973  y. The result is
+0000dca0: 2073 746f 7265 6420 696e 2067 616d 6d61   stored in gamma
+0000dcb0: 732e 2054 6865 7265 666f 7265 0a20 2020  s. Therefore.   
+0000dcc0: 2020 2020 2020 2020 2075 7375 616c 2067           usual g
+0000dcd0: 616d 6d61 7320 6172 6520 6e6f 7420 7374  ammas are not st
+0000dce0: 6f72 6564 2069 6e20 7468 6520 7661 7269  ored in the vari
+0000dcf0: 6162 6c65 2e20 4465 6661 756c 7420 6973  able. Default is
+0000dd00: 204e 6f6e 652c 2077 6869 6368 0a20 2020   None, which.   
+0000dd10: 2020 2020 2020 2020 2064 6f65 736e 2774           doesn't
+0000dd20: 2073 7065 6369 6679 2073 6361 7474 6572   specify scatter
+0000dd30: 696e 675f 6576 656e 745f 636c 6173 732e  ing_event_class.
+0000dd40: 0a20 2020 2020 2020 2077 7269 7465 5f74  .        write_t
+0000dd50: 7874 203a 2062 6f6f 6c2c 206f 7074 696f  xt : bool, optio
+0000dd60: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
+0000dd70: 4672 6571 7565 6e63 7920 706f 696e 7473  Frequency points
+0000dd80: 2061 6e64 2069 6d61 6769 6e61 7279 2070   and imaginary p
+0000dd90: 6172 7420 6f66 2073 656c 662d 656e 6572  art of self-ener
+0000dda0: 6769 6573 2061 7265 2077 7269 7474 656e  gies are written
+0000ddb0: 0a20 2020 2020 2020 2020 2020 2069 6e74  .            int
+0000ddc0: 6f20 7465 7874 2066 696c 6573 2e0a 2020  o text files..  
+0000ddd0: 2020 2020 2020 7772 6974 655f 6761 6d6d        write_gamm
+0000dde0: 615f 6465 7461 696c 203a 2062 6f6f 6c2c  a_detail : bool,
+0000ddf0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+0000de00: 2020 2020 2020 4465 7461 696c 6564 2067        Detailed g
+0000de10: 616d 6d61 7320 6172 6520 7772 6974 7465  ammas are writte
+0000de20: 6e20 696e 746f 2061 2066 696c 6520 696e  n into a file in
+0000de30: 2068 6466 352e 2044 6566 6175 6c74 2069   hdf5. Default i
+0000de40: 7320 4661 6c73 652e 0a20 2020 2020 2020  s False..       
+0000de50: 206b 6565 705f 6761 6d6d 615f 6465 7461   keep_gamma_deta
+0000de60: 696c 203a 2062 6f6f 6c2c 206f 7074 696f  il : bool, optio
+0000de70: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
+0000de80: 5769 7468 2054 7275 652c 2064 6574 6169  With True, detai
+0000de90: 6c65 6420 6761 6d6d 6173 2061 7265 2073  led gammas are s
+0000dea0: 746f 7265 642e 2044 6566 6175 6c74 2069  tored. Default i
+0000deb0: 7320 4661 6c73 652e 0a20 2020 2020 2020  s False..       
+0000dec0: 206f 7574 7075 745f 6669 6c65 6e61 6d65   output_filename
+0000ded0: 203a 2073 7472 0a20 2020 2020 2020 2020   : str.         
+0000dee0: 2020 2054 6869 7320 7374 7269 6e67 2069     This string i
+0000def0: 7320 696e 7365 7274 6564 2069 6e20 7468  s inserted in th
+0000df00: 6520 6f75 7470 7574 2066 696c 6520 6e61  e output file na
+0000df10: 6d65 732e 0a0a 2020 2020 2020 2020 2222  mes...        ""
+0000df20: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
+0000df30: 662e 5f69 6e74 6572 6163 7469 6f6e 2069  f._interaction i
+0000df40: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+0000df50: 2020 2020 6d73 6720 3d20 280a 2020 2020      msg = (.    
+0000df60: 2020 2020 2020 2020 2020 2020 2250 686f              "Pho
+0000df70: 6e6f 3370 792e 696e 6974 5f70 6870 685f  no3py.init_phph_
+0000df80: 696e 7465 7261 6374 696f 6e20 6861 7320  interaction has 
+0000df90: 746f 2062 6520 6361 6c6c 6564 2022 0a20  to be called ". 
+0000dfa0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000dfb0: 6265 666f 7265 2072 756e 6e69 6e67 2074  before running t
+0000dfc0: 6869 7320 6d65 7468 6f64 2e22 0a20 2020  his method.".   
+0000dfd0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000dfe0: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
+0000dff0: 7469 6d65 4572 726f 7228 6d73 6729 0a0a  timeError(msg)..
+0000e000: 2020 2020 2020 2020 6966 2074 656d 7065          if tempe
+0000e010: 7261 7475 7265 7320 6973 204e 6f6e 653a  ratures is None:
+0000e020: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000e030: 662e 5f74 656d 7065 7261 7475 7265 7320  f._temperatures 
+0000e040: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+0000e050: 2020 2020 3330 302e 302c 0a20 2020 2020      300.0,.     
+0000e060: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+0000e070: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000e080: 2020 2073 656c 662e 5f74 656d 7065 7261     self._tempera
+0000e090: 7475 7265 7320 3d20 7465 6d70 6572 6174  tures = temperat
+0000e0a0: 7572 6573 0a20 2020 2020 2020 2073 656c  ures.        sel
+0000e0b0: 662e 5f67 7269 645f 706f 696e 7473 203d  f._grid_points =
+0000e0c0: 2067 7269 645f 706f 696e 7473 0a20 2020   grid_points.   
+0000e0d0: 2020 2020 2073 656c 662e 5f73 6361 7474       self._scatt
+0000e0e0: 6572 696e 675f 6576 656e 745f 636c 6173  ering_event_clas
+0000e0f0: 7320 3d20 7363 6174 7465 7269 6e67 5f65  s = scattering_e
+0000e100: 7665 6e74 5f63 6c61 7373 0a20 2020 2020  vent_class.     
+0000e110: 2020 2076 616c 7320 3d20 6765 745f 696d     vals = get_im
+0000e120: 6167 5f73 656c 665f 656e 6572 6779 280a  ag_self_energy(.
+0000e130: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e140: 2e5f 696e 7465 7261 6374 696f 6e2c 0a20  ._interaction,. 
+0000e150: 2020 2020 2020 2020 2020 2067 7269 645f             grid_
+0000e160: 706f 696e 7473 2c0a 2020 2020 2020 2020  points,.        
+0000e170: 2020 2020 7465 6d70 6572 6174 7572 6573      temperatures
+0000e180: 2c0a 2020 2020 2020 2020 2020 2020 7369  ,.            si
+0000e190: 676d 6173 3d73 656c 662e 5f73 6967 6d61  gmas=self._sigma
+0000e1a0: 732c 0a20 2020 2020 2020 2020 2020 2066  s,.            f
+0000e1b0: 7265 7175 656e 6379 5f70 6f69 6e74 733d  requency_points=
+0000e1c0: 6672 6571 7565 6e63 795f 706f 696e 7473  frequency_points
+0000e1d0: 2c0a 2020 2020 2020 2020 2020 2020 6672  ,.            fr
+0000e1e0: 6571 7565 6e63 795f 7374 6570 3d66 7265  equency_step=fre
+0000e1f0: 7175 656e 6379 5f73 7465 702c 0a20 2020  quency_step,.   
+0000e200: 2020 2020 2020 2020 2066 7265 7175 656e           frequen
+0000e210: 6379 5f70 6f69 6e74 735f 6174 5f62 616e  cy_points_at_ban
+0000e220: 6473 3d66 7265 7175 656e 6379 5f70 6f69  ds=frequency_poi
+0000e230: 6e74 735f 6174 5f62 616e 6473 2c0a 2020  nts_at_bands,.  
+0000e240: 2020 2020 2020 2020 2020 6e75 6d5f 6672            num_fr
+0000e250: 6571 7565 6e63 795f 706f 696e 7473 3d6e  equency_points=n
+0000e260: 756d 5f66 7265 7175 656e 6379 5f70 6f69  um_frequency_poi
+0000e270: 6e74 732c 0a20 2020 2020 2020 2020 2020  nts,.           
+0000e280: 206e 756d 5f70 6f69 6e74 735f 696e 5f62   num_points_in_b
+0000e290: 6174 6368 3d6e 756d 5f70 6f69 6e74 735f  atch=num_points_
+0000e2a0: 696e 5f62 6174 6368 2c0a 2020 2020 2020  in_batch,.      
+0000e2b0: 2020 2020 2020 7363 6174 7465 7269 6e67        scattering
+0000e2c0: 5f65 7665 6e74 5f63 6c61 7373 3d73 6361  _event_class=sca
+0000e2d0: 7474 6572 696e 675f 6576 656e 745f 636c  ttering_event_cl
+0000e2e0: 6173 732c 0a20 2020 2020 2020 2020 2020  ass,.           
+0000e2f0: 2077 7269 7465 5f67 616d 6d61 5f64 6574   write_gamma_det
+0000e300: 6169 6c3d 7772 6974 655f 6761 6d6d 615f  ail=write_gamma_
+0000e310: 6465 7461 696c 2c0a 2020 2020 2020 2020  detail,.        
+0000e320: 2020 2020 7265 7475 726e 5f67 616d 6d61      return_gamma
+0000e330: 5f64 6574 6169 6c3d 6b65 6570 5f67 616d  _detail=keep_gam
+0000e340: 6d61 5f64 6574 6169 6c2c 0a20 2020 2020  ma_detail,.     
+0000e350: 2020 2020 2020 206f 7574 7075 745f 6669         output_fi
+0000e360: 6c65 6e61 6d65 3d6f 7574 7075 745f 6669  lename=output_fi
+0000e370: 6c65 6e61 6d65 2c0a 2020 2020 2020 2020  lename,.        
+0000e380: 2020 2020 6c6f 675f 6c65 7665 6c3d 7365      log_level=se
+0000e390: 6c66 2e5f 6c6f 675f 6c65 7665 6c2c 0a20  lf._log_level,. 
+0000e3a0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000e3b0: 2069 6620 6b65 6570 5f67 616d 6d61 5f64   if keep_gamma_d
+0000e3c0: 6574 6169 6c3a 0a20 2020 2020 2020 2020  etail:.         
+0000e3d0: 2020 2028 7365 6c66 2e5f 6672 6571 7565     (self._freque
+0000e3e0: 6e63 795f 706f 696e 7473 2c20 7365 6c66  ncy_points, self
+0000e3f0: 2e5f 6761 6d6d 6173 2c20 7365 6c66 2e5f  ._gammas, self._
+0000e400: 6465 7461 696c 6564 5f67 616d 6d61 7329  detailed_gammas)
+0000e410: 203d 2076 616c 730a 2020 2020 2020 2020   = vals.        
+0000e420: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000e430: 2020 7365 6c66 2e5f 6672 6571 7565 6e63    self._frequenc
+0000e440: 795f 706f 696e 7473 2c20 7365 6c66 2e5f  y_points, self._
+0000e450: 6761 6d6d 6173 203d 2076 616c 730a 0a20  gammas = vals.. 
+0000e460: 2020 2020 2020 2069 6620 7772 6974 655f         if write_
+0000e470: 7478 743a 0a20 2020 2020 2020 2020 2020  txt:.           
+0000e480: 2073 656c 662e 5f77 7269 7465 5f69 6d61   self._write_ima
+0000e490: 675f 7365 6c66 5f65 6e65 7267 7928 6f75  g_self_energy(ou
+0000e4a0: 7470 7574 5f66 696c 656e 616d 653d 6f75  tput_filename=ou
+0000e4b0: 7470 7574 5f66 696c 656e 616d 6529 0a0a  tput_filename)..
+0000e4c0: 2020 2020 2020 2020 7265 7475 726e 2076          return v
+0000e4d0: 616c 730a 0a20 2020 2064 6566 205f 7772  als..    def _wr
+0000e4e0: 6974 655f 696d 6167 5f73 656c 665f 656e  ite_imag_self_en
+0000e4f0: 6572 6779 2873 656c 662c 206f 7574 7075  ergy(self, outpu
+0000e500: 745f 6669 6c65 6e61 6d65 3d4e 6f6e 6529  t_filename=None)
+0000e510: 3a0a 2020 2020 2020 2020 7772 6974 655f  :.        write_
+0000e520: 696d 6167 5f73 656c 665f 656e 6572 6779  imag_self_energy
+0000e530: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
+0000e540: 6c66 2e5f 6761 6d6d 6173 2c0a 2020 2020  lf._gammas,.    
+0000e550: 2020 2020 2020 2020 7365 6c66 2e6d 6573          self.mes
+0000e560: 685f 6e75 6d62 6572 732c 0a20 2020 2020  h_numbers,.     
+0000e570: 2020 2020 2020 2073 656c 662e 5f67 7269         self._gri
+0000e580: 645f 706f 696e 7473 2c0a 2020 2020 2020  d_points,.      
+0000e590: 2020 2020 2020 7365 6c66 2e5f 6261 6e64        self._band
+0000e5a0: 5f69 6e64 6963 6573 2c0a 2020 2020 2020  _indices,.      
+0000e5b0: 2020 2020 2020 7365 6c66 2e5f 6672 6571        self._freq
+0000e5c0: 7565 6e63 795f 706f 696e 7473 2c0a 2020  uency_points,.  
+0000e5d0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000e5e0: 7465 6d70 6572 6174 7572 6573 2c0a 2020  temperatures,.  
+0000e5f0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000e600: 7369 676d 6173 2c0a 2020 2020 2020 2020  sigmas,.        
+0000e610: 2020 2020 7363 6174 7465 7269 6e67 5f65      scattering_e
+0000e620: 7665 6e74 5f63 6c61 7373 3d73 656c 662e  vent_class=self.
+0000e630: 5f73 6361 7474 6572 696e 675f 6576 656e  _scattering_even
+0000e640: 745f 636c 6173 732c 0a20 2020 2020 2020  t_class,.       
+0000e650: 2020 2020 206f 7574 7075 745f 6669 6c65       output_file
+0000e660: 6e61 6d65 3d6f 7574 7075 745f 6669 6c65  name=output_file
+0000e670: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+0000e680: 2020 6973 5f6d 6573 685f 7379 6d6d 6574    is_mesh_symmet
+0000e690: 7279 3d73 656c 662e 5f69 735f 6d65 7368  ry=self._is_mesh
+0000e6a0: 5f73 796d 6d65 7472 792c 0a20 2020 2020  _symmetry,.     
+0000e6b0: 2020 2020 2020 206c 6f67 5f6c 6576 656c         log_level
+0000e6c0: 3d73 656c 662e 5f6c 6f67 5f6c 6576 656c  =self._log_level
+0000e6d0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+0000e6e0: 2064 6566 2072 756e 5f72 6561 6c5f 7365   def run_real_se
+0000e6f0: 6c66 5f65 6e65 7267 7928 0a20 2020 2020  lf_energy(.     
+0000e700: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0000e710: 2067 7269 645f 706f 696e 7473 2c0a 2020   grid_points,.  
+0000e720: 2020 2020 2020 7465 6d70 6572 6174 7572        temperatur
+0000e730: 6573 2c0a 2020 2020 2020 2020 6672 6571  es,.        freq
+0000e740: 7565 6e63 795f 706f 696e 7473 5f61 745f  uency_points_at_
+0000e750: 6261 6e64 733d 4661 6c73 652c 0a20 2020  bands=False,.   
+0000e760: 2020 2020 2066 7265 7175 656e 6379 5f70       frequency_p
+0000e770: 6f69 6e74 733d 4e6f 6e65 2c0a 2020 2020  oints=None,.    
+0000e780: 2020 2020 6672 6571 7565 6e63 795f 7374      frequency_st
+0000e790: 6570 3d4e 6f6e 652c 0a20 2020 2020 2020  ep=None,.       
+0000e7a0: 206e 756d 5f66 7265 7175 656e 6379 5f70   num_frequency_p
+0000e7b0: 6f69 6e74 733d 4e6f 6e65 2c0a 2020 2020  oints=None,.    
+0000e7c0: 2020 2020 6570 7369 6c6f 6e73 3d4e 6f6e      epsilons=Non
+0000e7d0: 652c 0a20 2020 2020 2020 2077 7269 7465  e,.        write
+0000e7e0: 5f74 7874 3d46 616c 7365 2c0a 2020 2020  _txt=False,.    
+0000e7f0: 2020 2020 7772 6974 655f 6864 6635 3d46      write_hdf5=F
+0000e800: 616c 7365 2c0a 2020 2020 2020 2020 6f75  alse,.        ou
+0000e810: 7470 7574 5f66 696c 656e 616d 653d 4e6f  tput_filename=No
+0000e820: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+0000e830: 2020 2022 2222 4361 6c63 756c 6174 6520     """Calculate 
+0000e840: 7265 616c 2d70 6172 7420 6f66 2073 656c  real-part of sel
+0000e850: 662d 656e 6572 6779 206f 6620 6275 6262  f-energy of bubb
+0000e860: 6c65 2064 6961 6772 616d 2028 4465 6c74  le diagram (Delt
+0000e870: 6129 2e0a 0a20 2020 2020 2020 2050 6920  a)...        Pi 
+0000e880: 3d20 4465 6c74 6120 2d20 6920 4761 6d6d  = Delta - i Gamm
+0000e890: 612e 0a0a 2020 2020 2020 2020 5061 7261  a...        Para
+0000e8a0: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+0000e8b0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+0000e8c0: 2020 6772 6964 5f70 6f69 6e74 7320 3a20    grid_points : 
+0000e8d0: 6172 7261 795f 6c69 6b65 0a20 2020 2020  array_like.     
+0000e8e0: 2020 2020 2020 2047 7269 642d 706f 696e         Grid-poin
+0000e8f0: 7420 696e 6469 6365 7320 7768 6572 6520  t indices where 
+0000e900: 7265 616c 2070 6172 7420 6f66 2073 656c  real part of sel
+0000e910: 662d 656e 6572 6769 6573 2061 7265 0a20  f-energies are. 
+0000e920: 2020 2020 2020 2020 2020 2063 6163 6c63             caclc
+0000e930: 756c 6174 6564 2e0a 2020 2020 2020 2020  ulated..        
+0000e940: 2020 2020 6474 7970 653d 696e 742c 2073      dtype=int, s
+0000e950: 6861 7065 3d28 6772 6964 5f70 6f69 6e74  hape=(grid_point
+0000e960: 732c 290a 2020 2020 2020 2020 7465 6d70  s,).        temp
+0000e970: 6572 6174 7572 6573 203a 2061 7272 6179  eratures : array
+0000e980: 5f6c 696b 650a 2020 2020 2020 2020 2020  _like.          
+0000e990: 2020 5465 6d70 6572 6174 7572 6573 2077    Temperatures w
+0000e9a0: 6865 7265 2072 6561 6c20 7061 7274 206f  here real part o
+0000e9b0: 6620 7365 6c66 2d65 6e65 7267 6965 7320  f self-energies 
+0000e9c0: 2061 7265 2063 616c 6375 6c61 7465 642e   are calculated.
+0000e9d0: 0a20 2020 2020 2020 2020 2020 2064 7479  .            dty
+0000e9e0: 7065 3d66 6c6f 6174 2c20 7368 6170 653d  pe=float, shape=
+0000e9f0: 2874 656d 7065 7261 7475 7265 732c 290a  (temperatures,).
+0000ea00: 2020 2020 2020 2020 6672 6571 7565 6e63          frequenc
+0000ea10: 795f 706f 696e 7473 5f61 745f 6261 6e64  y_points_at_band
+0000ea20: 7320 3a20 626f 6f6c 2c20 6f70 7469 6f6e  s : bool, option
+0000ea30: 616c 0a20 2020 2020 2020 2020 2020 2057  al.            W
+0000ea40: 6974 6820 4661 6c73 652c 2066 7265 7175  ith False, frequ
+0000ea50: 656e 6379 2073 6869 6674 7320 6172 6520  ency shifts are 
+0000ea60: 6361 6c63 756c 6174 6564 2061 7420 6672  calculated at fr
+0000ea70: 7175 656e 6379 2073 616d 706c 696e 670a  quency sampling.
+0000ea80: 2020 2020 2020 2020 2020 2020 706f 696e              poin
+0000ea90: 7473 2e20 5768 656e 2054 7275 652c 2074  ts. When True, t
+0000eaa0: 6865 7920 6172 6520 646f 6e65 2061 7420  hey are done at 
+0000eab0: 7468 6520 7068 6f6e 6f6e 2066 7265 7175  the phonon frequ
+0000eac0: 656e 6369 6573 2e0a 2020 2020 2020 2020  encies..        
+0000ead0: 2020 2020 4465 6661 756c 7420 6973 2046      Default is F
+0000eae0: 616c 7365 2e0a 2020 2020 2020 2020 6672  alse..        fr
+0000eaf0: 6571 7565 6e63 795f 706f 696e 7473 203a  equency_points :
+0000eb00: 2061 7272 6179 5f6c 696b 652c 206f 7074   array_like, opt
+0000eb10: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+0000eb20: 2020 4672 6571 7565 6e63 7920 7361 6d70    Frequency samp
+0000eb30: 6c69 6e67 2070 6f69 6e74 732e 2044 6566  ling points. Def
+0000eb40: 6175 6c74 2069 7320 4e6f 6e65 2e20 496e  ault is None. In
+0000eb50: 2074 6869 7320 6361 7365 2c0a 2020 2020   this case,.    
+0000eb60: 2020 2020 2020 2020 6e75 6d5f 6672 6571          num_freq
+0000eb70: 7565 6e63 795f 706f 696e 7473 206f 7220  uency_points or 
+0000eb80: 6672 6571 7565 6e63 795f 7374 6570 2069  frequency_step i
+0000eb90: 7320 7573 6564 2074 6f20 6765 6e65 7261  s used to genera
+0000eba0: 7465 2075 6e69 666f 726d 0a20 2020 2020  te uniform.     
+0000ebb0: 2020 2020 2020 2066 7265 7175 656e 6379         frequency
+0000ebc0: 2073 616d 706c 696e 6720 706f 696e 7473   sampling points
+0000ebd0: 2e0a 2020 2020 2020 2020 2020 2020 6474  ..            dt
+0000ebe0: 7970 653d 666c 6f61 742c 2073 6861 7065  ype=float, shape
+0000ebf0: 3d28 6672 6571 7565 6e63 795f 706f 696e  =(frequency_poin
+0000ec00: 7473 2c29 0a20 2020 2020 2020 2066 7265  ts,).        fre
+0000ec10: 7175 656e 6379 5f73 7465 7020 3a20 666c  quency_step : fl
+0000ec20: 6f61 742c 206f 7074 696f 6e61 6c0a 2020  oat, optional.  
+0000ec30: 2020 2020 2020 2020 2020 556e 6966 6f72            Unifor
+0000ec40: 6d20 7069 7463 6820 6f66 2066 7265 7175  m pitch of frequ
+0000ec50: 656e 6379 2073 616d 706c 696e 6720 706f  ency sampling po
+0000ec60: 696e 7473 2e20 4465 6661 756c 7420 6973  ints. Default is
+0000ec70: 204e 6f6e 652e 2054 6869 730a 2020 2020   None. This.    
+0000ec80: 2020 2020 2020 2020 7265 7375 6c74 7320          results 
+0000ec90: 696e 2075 7369 6e67 206e 756d 5f66 7265  in using num_fre
+0000eca0: 7175 656e 6379 5f70 6f69 6e74 732e 0a20  quency_points.. 
+0000ecb0: 2020 2020 2020 206e 756d 5f66 7265 7175         num_frequ
+0000ecc0: 656e 6379 5f70 6f69 6e74 733a 2049 6e74  ency_points: Int
+0000ecd0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+0000ece0: 2020 2020 2020 204e 756d 6265 7220 6f66         Number of
+0000ecf0: 2073 616d 706c 696e 6720 7361 6d70 6c69   sampling sampli
+0000ed00: 6e67 2070 6f69 6e74 7320 746f 2062 6520  ng points to be 
+0000ed10: 7573 6564 2069 6e73 7465 6164 206f 660a  used instead of.
+0000ed20: 2020 2020 2020 2020 2020 2020 6672 6571              freq
+0000ed30: 7565 6e63 795f 7374 6570 2e20 5468 6973  uency_step. This
+0000ed40: 206e 756d 6265 7220 696e 636c 7564 6573   number includes
+0000ed50: 2065 6e64 2070 6f69 6e74 732e 2044 6566   end points. Def
+0000ed60: 6175 6c74 2069 7320 4e6f 6e65 2c0a 2020  ault is None,.  
+0000ed70: 2020 2020 2020 2020 2020 7768 6963 6820            which 
+0000ed80: 6769 7665 7320 3230 312e 0a20 2020 2020  gives 201..     
+0000ed90: 2020 2065 7073 696c 6f6e 7320 3a20 6172     epsilons : ar
+0000eda0: 7261 795f 6c69 6b65 0a20 2020 2020 2020  ray_like.       
+0000edb0: 2020 2020 2053 6d65 6172 696e 6720 7769       Smearing wi
+0000edc0: 6474 6873 2074 6f20 636f 6d70 7574 6572  dths to computer
+0000edd0: 2070 7269 6e63 6970 616c 2070 6172 742e   principal part.
+0000ede0: 2057 6865 6e20 6d75 6c74 6970 6c65 2076   When multiple v
+0000edf0: 616c 7565 730a 2020 2020 2020 2020 2020  alues.          
+0000ee00: 2020 6172 6520 6769 7665 6e20 6672 6571    are given freq
+0000ee10: 7565 6e63 7920 7368 6966 7473 2066 6f72  uency shifts for
+0000ee20: 2074 686f 7365 2076 616c 7565 7320 6172   those values ar
+0000ee30: 6520 7265 7475 726e 6564 2e0a 2020 2020  e returned..    
+0000ee40: 2020 2020 2020 2020 6474 7970 653d 666c          dtype=fl
+0000ee50: 6f61 742c 2073 6861 7065 3d28 6570 7369  oat, shape=(epsi
+0000ee60: 6c6f 6e73 2c29 0a20 2020 2020 2020 2077  lons,).        w
+0000ee70: 7269 7465 5f74 7874 203a 2062 6f6f 6c2c  rite_txt : bool,
+0000ee80: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+0000ee90: 2020 2020 2020 4672 6571 7565 6e63 7920        Frequency 
+0000eea0: 706f 696e 7473 2061 6e64 2072 6561 6c20  points and real 
+0000eeb0: 7061 7274 206f 6620 7365 6c66 2d65 6e65  part of self-ene
+0000eec0: 7267 6965 7320 6172 6520 7772 6974 7465  rgies are writte
+0000eed0: 6e0a 2020 2020 2020 2020 2020 2020 696e  n.            in
+0000eee0: 746f 2074 6578 7420 6669 6c65 732e 0a20  to text files.. 
+0000eef0: 2020 2020 2020 2077 7269 7465 5f68 6466         write_hdf
+0000ef00: 3520 3a20 626f 6f6c 0a20 2020 2020 2020  5 : bool.       
+0000ef10: 2020 2020 2052 6573 756c 7473 2061 7265       Results are
+0000ef20: 2073 746f 7265 6420 696e 2068 6466 3520   stored in hdf5 
+0000ef30: 6669 6c65 7320 696e 6465 7065 6e64 656e  files independen
+0000ef40: 746c 7920 6174 2067 7269 6420 706f 696e  tly at grid poin
+0000ef50: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
+0000ef60: 6570 7369 6c6f 6e73 2c20 616e 6420 7465  epsilons, and te
+0000ef70: 6d70 6572 6174 7572 6573 2e0a 2020 2020  mperatures..    
+0000ef80: 2020 2020 6f75 7470 7574 5f66 696c 656e      output_filen
+0000ef90: 616d 6520 3a20 7374 720a 2020 2020 2020  ame : str.      
+0000efa0: 2020 2020 2020 5468 6973 2073 7472 696e        This strin
+0000efb0: 6720 6973 2069 6e73 6572 7465 6420 696e  g is inserted in
+0000efc0: 2074 6865 206f 7574 7075 7420 6669 6c65   the output file
+0000efd0: 206e 616d 6573 2e0a 0a20 2020 2020 2020   names...       
+0000efe0: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+0000eff0: 7365 6c66 2e5f 696e 7465 7261 6374 696f  self._interactio
+0000f000: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
+0000f010: 2020 2020 2020 206d 7367 203d 2028 0a20         msg = (. 
+0000f020: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000f030: 5068 6f6e 6f33 7079 2e69 6e69 745f 7068  Phono3py.init_ph
+0000f040: 7068 5f69 6e74 6572 6163 7469 6f6e 2068  ph_interaction h
+0000f050: 6173 2074 6f20 6265 2063 616c 6c65 6420  as to be called 
+0000f060: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000f070: 2020 2262 6566 6f72 6520 7275 6e6e 696e    "before runnin
+0000f080: 6720 7468 6973 206d 6574 686f 642e 220a  g this method.".
+0000f090: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000f0a0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000f0b0: 5275 6e74 696d 6545 7272 6f72 286d 7367  RuntimeError(msg
+0000f0c0: 290a 0a20 2020 2020 2020 2069 6620 6570  )..        if ep
+0000f0d0: 7369 6c6f 6e73 2069 7320 6e6f 7420 4e6f  silons is not No
+0000f0e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000f0f0: 5f65 7073 696c 6f6e 7320 3d20 6570 7369  _epsilons = epsi
+0000f100: 6c6f 6e73 0a20 2020 2020 2020 2065 6c73  lons.        els
+0000f110: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+0000f120: 6620 6c65 6e28 7365 6c66 2e5f 7369 676d  f len(self._sigm
+0000f130: 6173 2920 3d3d 2031 2061 6e64 2073 656c  as) == 1 and sel
+0000f140: 662e 5f73 6967 6d61 735b 305d 2069 7320  f._sigmas[0] is 
+0000f150: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000f160: 2020 2020 2020 5f65 7073 696c 6f6e 7320        _epsilons 
+0000f170: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+0000f180: 2020 2065 6c69 6620 7365 6c66 2e5f 7369     elif self._si
+0000f190: 676d 6173 5b30 5d20 6973 204e 6f6e 653a  gmas[0] is None:
+0000f1a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f1b0: 205f 6570 7369 6c6f 6e73 203d 2073 656c   _epsilons = sel
+0000f1c0: 662e 5f73 6967 6d61 735b 313a 5d0a 2020  f._sigmas[1:].  
+0000f1d0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0000f1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f1f0: 5f65 7073 696c 6f6e 7320 3d20 7365 6c66  _epsilons = self
+0000f200: 2e5f 7369 676d 6173 0a0a 2020 2020 2020  ._sigmas..      
+0000f210: 2020 2320 2865 7073 696c 6f6e 2c20 6772    # (epsilon, gr
+0000f220: 6964 5f70 6f69 6e74 2c20 7465 6d70 6572  id_point, temper
+0000f230: 6174 7572 652c 2062 616e 6429 0a20 2020  ature, band).   
+0000f240: 2020 2020 2066 7265 7175 656e 6379 5f70       frequency_p
+0000f250: 6f69 6e74 732c 2064 656c 7461 7320 3d20  oints, deltas = 
+0000f260: 6765 745f 7265 616c 5f73 656c 665f 656e  get_real_self_en
+0000f270: 6572 6779 280a 2020 2020 2020 2020 2020  ergy(.          
+0000f280: 2020 7365 6c66 2e5f 696e 7465 7261 6374    self._interact
+0000f290: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+0000f2a0: 2067 7269 645f 706f 696e 7473 2c0a 2020   grid_points,.  
+0000f2b0: 2020 2020 2020 2020 2020 7465 6d70 6572            temper
+0000f2c0: 6174 7572 6573 2c0a 2020 2020 2020 2020  atures,.        
+0000f2d0: 2020 2020 6570 7369 6c6f 6e73 3d5f 6570      epsilons=_ep
+0000f2e0: 7369 6c6f 6e73 2c0a 2020 2020 2020 2020  silons,.        
+0000f2f0: 2020 2020 6672 6571 7565 6e63 795f 706f      frequency_po
+0000f300: 696e 7473 3d66 7265 7175 656e 6379 5f70  ints=frequency_p
+0000f310: 6f69 6e74 732c 0a20 2020 2020 2020 2020  oints,.         
+0000f320: 2020 2066 7265 7175 656e 6379 5f73 7465     frequency_ste
+0000f330: 703d 6672 6571 7565 6e63 795f 7374 6570  p=frequency_step
+0000f340: 2c0a 2020 2020 2020 2020 2020 2020 6e75  ,.            nu
+0000f350: 6d5f 6672 6571 7565 6e63 795f 706f 696e  m_frequency_poin
+0000f360: 7473 3d6e 756d 5f66 7265 7175 656e 6379  ts=num_frequency
+0000f370: 5f70 6f69 6e74 732c 0a20 2020 2020 2020  _points,.       
+0000f380: 2020 2020 2066 7265 7175 656e 6379 5f70       frequency_p
+0000f390: 6f69 6e74 735f 6174 5f62 616e 6473 3d66  oints_at_bands=f
+0000f3a0: 7265 7175 656e 6379 5f70 6f69 6e74 735f  requency_points_
+0000f3b0: 6174 5f62 616e 6473 2c0a 2020 2020 2020  at_bands,.      
+0000f3c0: 2020 2020 2020 7772 6974 655f 6864 6635        write_hdf5
+0000f3d0: 3d77 7269 7465 5f68 6466 352c 0a20 2020  =write_hdf5,.   
+0000f3e0: 2020 2020 2020 2020 206f 7574 7075 745f           output_
+0000f3f0: 6669 6c65 6e61 6d65 3d6f 7574 7075 745f  filename=output_
+0000f400: 6669 6c65 6e61 6d65 2c0a 2020 2020 2020  filename,.      
+0000f410: 2020 2020 2020 6c6f 675f 6c65 7665 6c3d        log_level=
+0000f420: 7365 6c66 2e5f 6c6f 675f 6c65 7665 6c2c  self._log_level,
+0000f430: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+0000f440: 2020 2020 6966 2077 7269 7465 5f74 7874      if write_txt
+0000f450: 3a0a 2020 2020 2020 2020 2020 2020 7772  :.            wr
+0000f460: 6974 655f 7265 616c 5f73 656c 665f 656e  ite_real_self_en
+0000f470: 6572 6779 280a 2020 2020 2020 2020 2020  ergy(.          
+0000f480: 2020 2020 2020 6465 6c74 6173 2c0a 2020        deltas,.  
+0000f490: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000f4a0: 6c66 2e6d 6573 685f 6e75 6d62 6572 732c  lf.mesh_numbers,
+0000f4b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f4c0: 2067 7269 645f 706f 696e 7473 2c0a 2020   grid_points,.  
+0000f4d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000f4e0: 6c66 2e5f 6261 6e64 5f69 6e64 6963 6573  lf._band_indices
+0000f4f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000f500: 2020 6672 6571 7565 6e63 795f 706f 696e    frequency_poin
+0000f510: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
+0000f520: 2020 2020 7465 6d70 6572 6174 7572 6573      temperatures
+0000f530: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000f540: 2020 5f65 7073 696c 6f6e 732c 0a20 2020    _epsilons,.   
+0000f550: 2020 2020 2020 2020 2020 2020 206f 7574               out
+0000f560: 7075 745f 6669 6c65 6e61 6d65 3d6f 7574  put_filename=out
+0000f570: 7075 745f 6669 6c65 6e61 6d65 2c0a 2020  put_filename,.  
+0000f580: 2020 2020 2020 2020 2020 2020 2020 6973                is
+0000f590: 5f6d 6573 685f 7379 6d6d 6574 7279 3d73  _mesh_symmetry=s
+0000f5a0: 656c 662e 5f69 735f 6d65 7368 5f73 796d  elf._is_mesh_sym
+0000f5b0: 6d65 7472 792c 0a20 2020 2020 2020 2020  metry,.         
+0000f5c0: 2020 2020 2020 206c 6f67 5f6c 6576 656c         log_level
+0000f5d0: 3d73 656c 662e 5f6c 6f67 5f6c 6576 656c  =self._log_level
+0000f5e0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+0000f5f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000f600: 6672 6571 7565 6e63 795f 706f 696e 7473  frequency_points
+0000f610: 2c20 6465 6c74 6173 0a0a 2020 2020 6465  , deltas..    de
+0000f620: 6620 7275 6e5f 7370 6563 7472 616c 5f66  f run_spectral_f
+0000f630: 756e 6374 696f 6e28 0a20 2020 2020 2020  unction(.       
+0000f640: 2073 656c 662c 0a20 2020 2020 2020 2067   self,.        g
+0000f650: 7269 645f 706f 696e 7473 2c0a 2020 2020  rid_points,.    
+0000f660: 2020 2020 7465 6d70 6572 6174 7572 6573      temperatures
+0000f670: 2c0a 2020 2020 2020 2020 6672 6571 7565  ,.        freque
+0000f680: 6e63 795f 706f 696e 7473 3d4e 6f6e 652c  ncy_points=None,
+0000f690: 0a20 2020 2020 2020 2066 7265 7175 656e  .        frequen
+0000f6a0: 6379 5f73 7465 703d 4e6f 6e65 2c0a 2020  cy_step=None,.  
+0000f6b0: 2020 2020 2020 6e75 6d5f 6672 6571 7565        num_freque
+0000f6c0: 6e63 795f 706f 696e 7473 3d4e 6f6e 652c  ncy_points=None,
+0000f6d0: 0a20 2020 2020 2020 206e 756d 5f70 6f69  .        num_poi
+0000f6e0: 6e74 735f 696e 5f62 6174 6368 3d4e 6f6e  nts_in_batch=Non
+0000f6f0: 652c 0a20 2020 2020 2020 2077 7269 7465  e,.        write
+0000f700: 5f74 7874 3d46 616c 7365 2c0a 2020 2020  _txt=False,.    
+0000f710: 2020 2020 7772 6974 655f 6864 6635 3d46      write_hdf5=F
+0000f720: 616c 7365 2c0a 2020 2020 2020 2020 6f75  alse,.        ou
+0000f730: 7470 7574 5f66 696c 656e 616d 653d 4e6f  tput_filename=No
+0000f740: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+0000f750: 2020 2022 2222 4672 6571 7565 6e63 7920     """Frequency 
+0000f760: 7368 6966 7420 6672 6f6d 206c 6f77 6573  shift from lowes
+0000f770: 7420 6f72 6465 7220 6469 6167 7261 6d20  t order diagram 
+0000f780: 6973 2063 616c 6375 6c61 7465 642e 0a0a  is calculated...
+0000f790: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+0000f7a0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+0000f7b0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6772  -----.        gr
+0000f7c0: 6964 5f70 6f69 6e74 7320 3a20 6172 7261  id_points : arra
+0000f7d0: 795f 6c69 6b65 0a20 2020 2020 2020 2020  y_like.         
+0000f7e0: 2020 2047 7269 642d 706f 696e 7420 696e     Grid-point in
+0000f7f0: 6469 6365 7320 7768 6572 6520 696d 6167  dices where imag
+0000f800: 2d73 656c 662d 656e 6572 6765 6973 2061  -self-energeis a
+0000f810: 7265 2063 6163 6c63 756c 6174 6564 2e0a  re caclculated..
+0000f820: 2020 2020 2020 2020 2020 2020 6474 7970              dtyp
+0000f830: 653d 696e 742c 2073 6861 7065 3d28 6772  e=int, shape=(gr
+0000f840: 6964 5f70 6f69 6e74 732c 290a 2020 2020  id_points,).    
+0000f850: 2020 2020 7465 6d70 6572 6174 7572 6573      temperatures
+0000f860: 203a 2061 7272 6179 5f6c 696b 650a 2020   : array_like.  
+0000f870: 2020 2020 2020 2020 2020 5465 6d70 6572            Temper
+0000f880: 6174 7572 6573 2077 6865 7265 2069 6d61  atures where ima
+0000f890: 672d 7365 6c66 2d65 6e65 7267 6965 7320  g-self-energies 
+0000f8a0: 6172 6520 6361 6c63 756c 6174 6564 2e0a  are calculated..
+0000f8b0: 2020 2020 2020 2020 2020 2020 6474 7970              dtyp
+0000f8c0: 653d 666c 6f61 742c 2073 6861 7065 3d28  e=float, shape=(
+0000f8d0: 7465 6d70 6572 6174 7572 6573 2c29 0a20  temperatures,). 
+0000f8e0: 2020 2020 2020 2066 7265 7175 656e 6379         frequency
+0000f8f0: 5f70 6f69 6e74 7320 3a20 6172 7261 795f  _points : array_
+0000f900: 6c69 6b65 2c20 6f70 7469 6f6e 616c 0a20  like, optional. 
+0000f910: 2020 2020 2020 2020 2020 2046 7265 7175             Frequ
+0000f920: 656e 6379 2073 616d 706c 696e 6720 706f  ency sampling po
+0000f930: 696e 7473 2e20 4465 6661 756c 7420 6973  ints. Default is
+0000f940: 204e 6f6e 652e 2049 6e20 7468 6973 2063   None. In this c
+0000f950: 6173 652c 0a20 2020 2020 2020 2020 2020  ase,.           
+0000f960: 206e 756d 5f66 7265 7175 656e 6379 5f70   num_frequency_p
+0000f970: 6f69 6e74 7320 6f72 2066 7265 7175 656e  oints or frequen
+0000f980: 6379 5f73 7465 7020 6973 2075 7365 6420  cy_step is used 
+0000f990: 746f 2067 656e 6572 6174 6520 756e 6966  to generate unif
+0000f9a0: 6f72 6d0a 2020 2020 2020 2020 2020 2020  orm.            
+0000f9b0: 6672 6571 7565 6e63 7920 7361 6d70 6c69  frequency sampli
+0000f9c0: 6e67 2070 6f69 6e74 732e 0a20 2020 2020  ng points..     
+0000f9d0: 2020 2020 2020 2064 7479 7065 3d66 6c6f         dtype=flo
+0000f9e0: 6174 2c20 7368 6170 653d 2866 7265 7175  at, shape=(frequ
+0000f9f0: 656e 6379 5f70 6f69 6e74 732c 290a 2020  ency_points,).  
+0000fa00: 2020 2020 2020 6672 6571 7565 6e63 795f        frequency_
+0000fa10: 7374 6570 203a 2066 6c6f 6174 2c20 6f70  step : float, op
+0000fa20: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
+0000fa30: 2020 2055 6e69 666f 726d 2070 6974 6368     Uniform pitch
+0000fa40: 206f 6620 6672 6571 7565 6e63 7920 7361   of frequency sa
+0000fa50: 6d70 6c69 6e67 2070 6f69 6e74 732e 2044  mpling points. D
+0000fa60: 6566 6175 6c74 2069 7320 4e6f 6e65 2e20  efault is None. 
+0000fa70: 5468 6973 0a20 2020 2020 2020 2020 2020  This.           
+0000fa80: 2072 6573 756c 7473 2069 6e20 7573 696e   results in usin
+0000fa90: 6720 6e75 6d5f 6672 6571 7565 6e63 795f  g num_frequency_
+0000faa0: 706f 696e 7473 2e0a 2020 2020 2020 2020  points..        
+0000fab0: 6e75 6d5f 6672 6571 7565 6e63 795f 706f  num_frequency_po
+0000fac0: 696e 7473 3a20 496e 742c 206f 7074 696f  ints: Int, optio
+0000fad0: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
+0000fae0: 4e75 6d62 6572 206f 6620 7361 6d70 6c69  Number of sampli
+0000faf0: 6e67 2073 616d 706c 696e 6720 706f 696e  ng sampling poin
+0000fb00: 7473 2074 6f20 6265 2075 7365 6420 696e  ts to be used in
+0000fb10: 7374 6561 6420 6f66 0a20 2020 2020 2020  stead of.       
+0000fb20: 2020 2020 2066 7265 7175 656e 6379 5f73       frequency_s
+0000fb30: 7465 702e 2054 6869 7320 6e75 6d62 6572  tep. This number
+0000fb40: 2069 6e63 6c75 6465 7320 656e 6420 706f   includes end po
+0000fb50: 696e 7473 2e20 4465 6661 756c 7420 6973  ints. Default is
+0000fb60: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+0000fb70: 2020 2077 6869 6368 2067 6976 6573 2032     which gives 2
+0000fb80: 3031 2e0a 2020 2020 2020 2020 6e75 6d5f  01..        num_
+0000fb90: 706f 696e 7473 5f69 6e5f 6261 7463 683a  points_in_batch:
+0000fba0: 2069 6e74 2c20 6f70 7469 6f6e 616c 0a20   int, optional. 
+0000fbb0: 2020 2020 2020 2020 2020 204e 756d 6265             Numbe
+0000fbc0: 7220 6f66 2073 616d 706c 696e 6720 706f  r of sampling po
+0000fbd0: 696e 7473 2069 6e20 6f6e 6520 6261 7463  ints in one batc
+0000fbe0: 682e 2054 6869 7320 6973 2066 6f72 2074  h. This is for t
+0000fbf0: 6865 2066 7265 7175 656e 6379 0a20 2020  he frequency.   
+0000fc00: 2020 2020 2020 2020 2073 616d 706c 696e           samplin
+0000fc10: 6720 6d6f 6465 2061 6e64 2074 6865 2073  g mode and the s
+0000fc20: 616d 706c 696e 6720 706f 696e 7473 2061  ampling points a
+0000fc30: 7265 2064 6976 6964 6564 2069 6e74 6f20  re divided into 
+0000fc40: 6261 7463 6865 732e 0a20 2020 2020 2020  batches..       
+0000fc50: 2020 2020 204c 6167 6572 206e 756d 6265       Lager numbe
+0000fc60: 7220 7072 6f76 6964 6573 2065 6666 6963  r provides effic
+0000fc70: 6965 6e74 2075 7365 206f 6620 6d75 6c74  ient use of mult
+0000fc80: 692d 636f 7265 7320 6275 7420 6d6f 7265  i-cores but more
+0000fc90: 0a20 2020 2020 2020 2020 2020 206d 656d  .            mem
+0000fca0: 6f72 7920 6465 6d61 6e64 696e 672e 2044  ory demanding. D
+0000fcb0: 6566 6175 6c74 2069 7320 4e6f 6e65 2c20  efault is None, 
+0000fcc0: 7768 6963 6820 6769 7665 2074 6865 206e  which give the n
+0000fcd0: 756d 6265 7220 6f66 2031 302e 0a20 2020  umber of 10..   
+0000fce0: 2020 2020 2077 7269 7465 5f74 7874 203a       write_txt :
+0000fcf0: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0a   bool, optional.
+0000fd00: 2020 2020 2020 2020 2020 2020 4672 6571              Freq
+0000fd10: 7565 6e63 7920 706f 696e 7473 2061 6e64  uency points and
+0000fd20: 2073 7065 6374 7261 6c20 6675 6e63 7469   spectral functi
+0000fd30: 6f6e 7320 6172 6520 7772 6974 7465 6e0a  ons are written.
+0000fd40: 2020 2020 2020 2020 2020 2020 696e 746f              into
+0000fd50: 2074 6578 7420 6669 6c65 732e 2044 6566   text files. Def
+0000fd60: 6175 6c74 2069 7320 4661 6c73 652e 0a20  ault is False.. 
+0000fd70: 2020 2020 2020 2077 7269 7465 5f68 6466         write_hdf
+0000fd80: 3520 3a20 626f 6f6c 0a20 2020 2020 2020  5 : bool.       
+0000fd90: 2020 2020 2052 6573 756c 7473 2061 7265       Results are
+0000fda0: 2073 746f 7265 6420 696e 2068 6466 3520   stored in hdf5 
+0000fdb0: 6669 6c65 7320 696e 6465 7065 6e64 656e  files independen
+0000fdc0: 746c 7920 6174 2067 7269 6420 706f 696e  tly at grid poin
+0000fdd0: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
+0000fde0: 6570 7369 6c6f 6e73 2e20 4465 6661 756c  epsilons. Defaul
+0000fdf0: 7420 6973 2046 616c 7365 2e0a 2020 2020  t is False..    
+0000fe00: 2020 2020 6f75 7470 7574 5f66 696c 656e      output_filen
+0000fe10: 616d 6520 3a20 7374 720a 2020 2020 2020  ame : str.      
+0000fe20: 2020 2020 2020 5468 6973 2073 7472 696e        This strin
+0000fe30: 6720 6973 2069 6e73 6572 7465 6420 696e  g is inserted in
+0000fe40: 2074 6865 206f 7574 7075 7420 6669 6c65   the output file
+0000fe50: 206e 616d 6573 2e0a 0a20 2020 2020 2020   names...       
+0000fe60: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+0000fe70: 7365 6c66 2e5f 696e 7465 7261 6374 696f  self._interactio
+0000fe80: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
+0000fe90: 2020 2020 2020 206d 7367 203d 2028 0a20         msg = (. 
+0000fea0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000feb0: 5068 6f6e 6f33 7079 2e69 6e69 745f 7068  Phono3py.init_ph
+0000fec0: 7068 5f69 6e74 6572 6163 7469 6f6e 2068  ph_interaction h
+0000fed0: 6173 2074 6f20 6265 2063 616c 6c65 6420  as to be called 
+0000fee0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000fef0: 2020 2262 6566 6f72 6520 7275 6e6e 696e    "before runnin
+0000ff00: 6720 7468 6973 206d 6574 686f 642e 220a  g this method.".
+0000ff10: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000ff20: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000ff30: 5275 6e74 696d 6545 7272 6f72 286d 7367  RuntimeError(msg
+0000ff40: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0000ff50: 5f73 7065 6374 7261 6c5f 6675 6e63 7469  _spectral_functi
+0000ff60: 6f6e 203d 2072 756e 5f73 7065 6374 7261  on = run_spectra
+0000ff70: 6c5f 6675 6e63 7469 6f6e 280a 2020 2020  l_function(.    
+0000ff80: 2020 2020 2020 2020 7365 6c66 2e5f 696e          self._in
+0000ff90: 7465 7261 6374 696f 6e2c 0a20 2020 2020  teraction,.     
+0000ffa0: 2020 2020 2020 2067 7269 645f 706f 696e         grid_poin
+0000ffb0: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
+0000ffc0: 7465 6d70 6572 6174 7572 6573 3d74 656d  temperatures=tem
+0000ffd0: 7065 7261 7475 7265 732c 0a20 2020 2020  peratures,.     
+0000ffe0: 2020 2020 2020 2073 6967 6d61 733d 7365         sigmas=se
+0000fff0: 6c66 2e5f 7369 676d 6173 2c0a 2020 2020  lf._sigmas,.    
+00010000: 2020 2020 2020 2020 6672 6571 7565 6e63          frequenc
+00010010: 795f 706f 696e 7473 3d66 7265 7175 656e  y_points=frequen
+00010020: 6379 5f70 6f69 6e74 732c 0a20 2020 2020  cy_points,.     
+00010030: 2020 2020 2020 2066 7265 7175 656e 6379         frequency
+00010040: 5f73 7465 703d 6672 6571 7565 6e63 795f  _step=frequency_
+00010050: 7374 6570 2c0a 2020 2020 2020 2020 2020  step,.          
+00010060: 2020 6e75 6d5f 6672 6571 7565 6e63 795f    num_frequency_
+00010070: 706f 696e 7473 3d6e 756d 5f66 7265 7175  points=num_frequ
+00010080: 656e 6379 5f70 6f69 6e74 732c 0a20 2020  ency_points,.   
+00010090: 2020 2020 2020 2020 206e 756d 5f70 6f69           num_poi
+000100a0: 6e74 735f 696e 5f62 6174 6368 3d6e 756d  nts_in_batch=num
+000100b0: 5f70 6f69 6e74 735f 696e 5f62 6174 6368  _points_in_batch
+000100c0: 2c0a 2020 2020 2020 2020 2020 2020 6261  ,.            ba
+000100d0: 6e64 5f69 6e64 6963 6573 3d73 656c 662e  nd_indices=self.
+000100e0: 5f62 616e 645f 696e 6469 6365 732c 0a20  _band_indices,. 
+000100f0: 2020 2020 2020 2020 2020 2077 7269 7465             write
+00010100: 5f74 7874 3d77 7269 7465 5f74 7874 2c0a  _txt=write_txt,.
+00010110: 2020 2020 2020 2020 2020 2020 7772 6974              writ
+00010120: 655f 6864 6635 3d77 7269 7465 5f68 6466  e_hdf5=write_hdf
+00010130: 352c 0a20 2020 2020 2020 2020 2020 206f  5,.            o
+00010140: 7574 7075 745f 6669 6c65 6e61 6d65 3d6f  utput_filename=o
+00010150: 7574 7075 745f 6669 6c65 6e61 6d65 2c0a  utput_filename,.
+00010160: 2020 2020 2020 2020 2020 2020 6c6f 675f              log_
+00010170: 6c65 7665 6c3d 7365 6c66 2e5f 6c6f 675f  level=self._log_
+00010180: 6c65 7665 6c2c 0a20 2020 2020 2020 2029  level,.        )
+00010190: 0a0a 2020 2020 6465 6620 7275 6e5f 7468  ..    def run_th
+000101a0: 6572 6d61 6c5f 636f 6e64 7563 7469 7669  ermal_conductivi
+000101b0: 7479 280a 2020 2020 2020 2020 7365 6c66  ty(.        self
+000101c0: 2c0a 2020 2020 2020 2020 6973 5f4c 4254  ,.        is_LBT
+000101d0: 453d 4661 6c73 652c 0a20 2020 2020 2020  E=False,.       
+000101e0: 2074 656d 7065 7261 7475 7265 733d 4e6f   temperatures=No
+000101f0: 6e65 2c0a 2020 2020 2020 2020 6973 5f69  ne,.        is_i
+00010200: 736f 746f 7065 3d46 616c 7365 2c0a 2020  sotope=False,.  
+00010210: 2020 2020 2020 6d61 7373 5f76 6172 6961        mass_varia
+00010220: 6e63 6573 3d4e 6f6e 652c 0a20 2020 2020  nces=None,.     
+00010230: 2020 2067 7269 645f 706f 696e 7473 3d4e     grid_points=N
+00010240: 6f6e 652c 0a20 2020 2020 2020 2062 6f75  one,.        bou
+00010250: 6e64 6172 795f 6d66 703d 4e6f 6e65 2c20  ndary_mfp=None, 
+00010260: 2023 2069 6e20 6d69 6372 6f6d 6574 7265   # in micrometre
+00010270: 0a20 2020 2020 2020 2073 6f6c 7665 5f63  .        solve_c
+00010280: 6f6c 6c65 6374 6976 655f 7068 6f6e 6f6e  ollective_phonon
+00010290: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
+000102a0: 7573 655f 6176 655f 7070 3d46 616c 7365  use_ave_pp=False
+000102b0: 2c0a 2020 2020 2020 2020 6973 5f72 6564  ,.        is_red
+000102c0: 7563 6962 6c65 5f63 6f6c 6c69 7369 6f6e  ucible_collision
+000102d0: 5f6d 6174 7269 783d 4661 6c73 652c 0a20  _matrix=False,. 
+000102e0: 2020 2020 2020 2069 735f 6b61 7070 615f         is_kappa_
+000102f0: 7374 6172 3d54 7275 652c 0a20 2020 2020  star=True,.     
+00010300: 2020 2067 765f 6465 6c74 615f 713d 4e6f     gv_delta_q=No
+00010310: 6e65 2c20 2023 2066 6f72 2067 726f 7570  ne,  # for group
+00010320: 2076 656c 6f63 6974 790a 2020 2020 2020   velocity.      
+00010330: 2020 6973 5f66 756c 6c5f 7070 3d46 616c    is_full_pp=Fal
+00010340: 7365 2c0a 2020 2020 2020 2020 7069 6e76  se,.        pinv
+00010350: 5f63 7574 6f66 663d 312e 3065 2d38 2c20  _cutoff=1.0e-8, 
+00010360: 2023 2066 6f72 2070 7365 7564 6f2d 696e   # for pseudo-in
+00010370: 7665 7273 696f 6e20 6f66 2063 6f6c 6c69  version of colli
+00010380: 7369 6f6e 206d 6174 7269 780a 2020 2020  sion matrix.    
+00010390: 2020 2020 7069 6e76 5f6d 6574 686f 643d      pinv_method=
+000103a0: 302c 2020 2320 666f 7220 7073 6575 646f  0,  # for pseudo
+000103b0: 2d69 6e76 6572 7369 6f6e 206f 6620 636f  -inversion of co
+000103c0: 6c6c 6973 696f 6e20 6d61 7472 6978 0a20  llision matrix. 
+000103d0: 2020 2020 2020 2070 696e 765f 736f 6c76         pinv_solv
+000103e0: 6572 3d30 2c20 2023 2073 6f6c 7665 7220  er=0,  # solver 
+000103f0: 6f66 2070 7365 7564 6f2d 696e 7665 7273  of pseudo-invers
+00010400: 696f 6e20 6f66 2063 6f6c 6c69 7369 6f6e  ion of collision
+00010410: 206d 6174 7269 780a 2020 2020 2020 2020   matrix.        
+00010420: 7772 6974 655f 6761 6d6d 613d 4661 6c73  write_gamma=Fals
+00010430: 652c 0a20 2020 2020 2020 2072 6561 645f  e,.        read_
+00010440: 6761 6d6d 613d 4661 6c73 652c 0a20 2020  gamma=False,.   
+00010450: 2020 2020 2069 735f 4e5f 553d 4661 6c73       is_N_U=Fals
+00010460: 652c 0a20 2020 2020 2020 2063 6f6e 6475  e,.        condu
+00010470: 6374 6976 6974 795f 7479 7065 3d4e 6f6e  ctivity_type=Non
+00010480: 652c 0a20 2020 2020 2020 2077 7269 7465  e,.        write
+00010490: 5f6b 6170 7061 3d46 616c 7365 2c0a 2020  _kappa=False,.  
+000104a0: 2020 2020 2020 7772 6974 655f 6761 6d6d        write_gamm
+000104b0: 615f 6465 7461 696c 3d46 616c 7365 2c0a  a_detail=False,.
+000104c0: 2020 2020 2020 2020 7772 6974 655f 636f          write_co
+000104d0: 6c6c 6973 696f 6e3d 4661 6c73 652c 0a20  llision=False,. 
+000104e0: 2020 2020 2020 2072 6561 645f 636f 6c6c         read_coll
+000104f0: 6973 696f 6e3d 4661 6c73 652c 0a20 2020  ision=False,.   
+00010500: 2020 2020 2077 7269 7465 5f70 703d 4661       write_pp=Fa
+00010510: 6c73 652c 0a20 2020 2020 2020 2072 6561  lse,.        rea
+00010520: 645f 7070 3d46 616c 7365 2c0a 2020 2020  d_pp=False,.    
+00010530: 2020 2020 7772 6974 655f 4c42 5445 5f73      write_LBTE_s
+00010540: 6f6c 7574 696f 6e3d 4661 6c73 652c 0a20  olution=False,. 
+00010550: 2020 2020 2020 2063 6f6d 7072 6573 7369         compressi
+00010560: 6f6e 3d22 677a 6970 222c 0a20 2020 2020  on="gzip",.     
+00010570: 2020 2069 6e70 7574 5f66 696c 656e 616d     input_filenam
+00010580: 653d 4e6f 6e65 2c0a 2020 2020 2020 2020  e=None,.        
+00010590: 6f75 7470 7574 5f66 696c 656e 616d 653d  output_filename=
+000105a0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+000105b0: 2020 2020 2022 2222 5275 6e20 7468 6572       """Run ther
+000105c0: 6d61 6c20 636f 6e64 7563 7469 7669 7479  mal conductivity
+000105d0: 2063 616c 6375 6c61 7469 6f6e 2e0a 0a20   calculation... 
+000105e0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+000105f0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00010600: 2d2d 2d2d 0a20 2020 2020 2020 2069 735f  ----.        is_
+00010610: 4c42 5445 203a 2062 6f6f 6c2c 206f 7074  LBTE : bool, opt
+00010620: 696f 6e61 6c2c 2064 6566 6175 6c74 2069  ional, default i
+00010630: 7320 4661 6c73 650a 2020 2020 2020 2020  s False.        
+00010640: 2020 2020 5254 4120 2846 616c 7365 2920      RTA (False) 
+00010650: 6f72 2064 6972 6563 7420 736f 6c75 7469  or direct soluti
+00010660: 6f6e 2028 5472 7565 292e 0a20 2020 2020  on (True)..     
+00010670: 2020 2074 656d 7065 7261 7475 7265 7320     temperatures 
+00010680: 3a20 6172 7261 795f 6c69 6b65 2c20 6f70  : array_like, op
+00010690: 7469 6f6e 616c 2c20 6465 6661 756c 7420  tional, default 
+000106a0: 6973 204e 6f6e 650a 2020 2020 2020 2020  is None.        
+000106b0: 2020 2020 5465 6d70 6572 6174 7572 6573      Temperatures
+000106c0: 2061 7420 7768 6963 6820 7468 6572 6d61   at which therma
+000106d0: 6c20 636f 6e64 7563 7469 7669 7479 2069  l conductivity i
+000106e0: 7320 6361 6c63 756c 6174 6564 2e0a 2020  s calculated..  
+000106f0: 2020 2020 2020 2020 2020 7368 6170 653d            shape=
+00010700: 2874 656d 7065 7261 7475 7265 5f70 6f69  (temperature_poi
+00010710: 6e74 732c 2029 2c20 6474 7970 653d 2764  nts, ), dtype='d
+00010720: 6f75 626c 6527 2e0a 2020 2020 2020 2020  ouble'..        
+00010730: 2020 2020 5769 7468 204e 6f6e 652c 0a20      With None,. 
+00010740: 2020 2020 2020 2020 2020 2020 2020 2060                 `
+00010750: 6973 5f4c 4254 453d 4661 6c73 6560 2067  is_LBTE=False` g
+00010760: 6976 6573 2074 656d 7065 7261 7475 7265  ives temperature
+00010770: 733d 5b30 2c20 3130 2c20 2e2e 2e2c 2031  s=[0, 10, ..., 1
+00010780: 3030 305d 2e0a 2020 2020 2020 2020 2020  000]..          
+00010790: 2020 2020 2020 6069 735f 4c42 5445 3d54        `is_LBTE=T
+000107a0: 7275 6560 2067 6976 6573 2074 656d 7065  rue` gives tempe
+000107b0: 7261 7475 7265 733d 5b33 3030 2c20 5d2e  ratures=[300, ].
+000107c0: 0a20 2020 2020 2020 2069 735f 6973 6f74  .        is_isot
+000107d0: 6f70 6520 3a20 626f 6f6c 2c20 6f70 7469  ope : bool, opti
+000107e0: 6f6e 616c 2c20 6465 6661 756c 7420 6973  onal, default is
+000107f0: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
+00010800: 2020 2057 6974 6820 6f72 2077 6974 686f     With or witho
+00010810: 7574 2069 736f 746f 7065 2073 6361 7474  ut isotope scatt
+00010820: 6572 696e 672e 0a20 2020 2020 2020 206d  ering..        m
+00010830: 6173 735f 7661 7269 616e 6365 7320 3a20  ass_variances : 
+00010840: 6172 7261 795f 6c69 6b65 2c20 6f70 7469  array_like, opti
+00010850: 6f6e 616c 2c20 6465 6661 756c 7420 6973  onal, default is
+00010860: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+00010870: 2020 4d61 7373 2076 6172 6961 6e63 6573    Mass variances
+00010880: 2066 6f72 2069 736f 746f 7065 2073 6361   for isotope sca
+00010890: 7474 6572 696e 6720 6361 6c63 756c 6174  ttering calculat
+000108a0: 696f 6e2e 2057 6865 6e20 4e6f 6e65 2c0a  ion. When None,.
+000108b0: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+000108c0: 7661 6c75 6573 2073 746f 7265 6420 696e  values stored in
+000108d0: 2070 686f 6e6f 3370 7920 6172 6520 7573   phono3py are us
+000108e0: 6564 2077 6974 6820 6069 735f 6973 6f74  ed with `is_isot
+000108f0: 6f70 653d 5472 7565 602e 0a20 2020 2020  ope=True`..     
+00010900: 2020 2020 2020 2073 6861 7065 2861 746f         shape(ato
+00010910: 6d73 5f69 6e5f 7072 696d 6974 6976 652c  ms_in_primitive,
+00010920: 2029 2c20 6474 7970 653d 2764 6f75 626c   ), dtype='doubl
+00010930: 6527 2e0a 2020 2020 2020 2020 6772 6964  e'..        grid
+00010940: 5f70 6f69 6e74 7320 3a20 6172 7261 795f  _points : array_
+00010950: 6c69 6b65 2c20 6f70 7469 6f6e 616c 2c20  like, optional, 
+00010960: 6465 6661 756c 7420 6973 204e 6f6e 650a  default is None.
+00010970: 2020 2020 2020 2020 2020 2020 4c69 7374              List
+00010980: 206f 6620 6772 6964 2070 6f69 6e74 2069   of grid point i
+00010990: 6e64 6963 6573 2077 6865 7265 206d 6f64  ndices where mod
+000109a0: 6520 7468 6572 6d61 6c20 636f 6e64 7563  e thermal conduc
+000109b0: 7469 7669 7469 6573 2061 7265 0a20 2020  tivities are.   
+000109c0: 2020 2020 2020 2020 2063 616c 6375 6c61           calcula
+000109d0: 7465 642e 2057 6974 6820 4e6f 6e65 2c20  ted. With None, 
+000109e0: 616c 6c20 7468 6520 6772 6964 2070 6f69  all the grid poi
+000109f0: 6e74 7320 7468 6174 2061 7265 206e 6563  nts that are nec
+00010a00: 6573 7361 7279 0a20 2020 2020 2020 2020  essary.         
+00010a10: 2020 2066 6f72 2074 6865 726d 616c 2063     for thermal c
+00010a20: 6f6e 6475 6374 6976 6974 7920 6172 6520  onductivity are 
+00010a30: 7365 7420 696e 7465 726e 616c 6c79 2e0a  set internally..
+00010a40: 2020 2020 2020 2020 2020 2020 7368 6170              shap
+00010a50: 6528 6e75 6d5f 6772 6964 5f70 6f69 6e74  e(num_grid_point
+00010a60: 732c 2029 2c20 6474 7970 653d 2769 6e74  s, ), dtype='int
+00010a70: 5f27 2e0a 2020 2020 2020 2020 626f 756e  _'..        boun
+00010a80: 6461 7279 5f6d 6670 203a 2066 6c6f 6174  dary_mfp : float
+00010a90: 2c20 6f70 7469 6f6e 612c 2064 6566 6175  , optiona, defau
+00010aa0: 6c74 2069 7320 4e6f 6e65 0a20 2020 2020  lt is None.     
+00010ab0: 2020 2020 2020 204d 6561 6e20 6672 6565         Mean free
+00010ac0: 2070 6174 6820 696e 206d 6963 726f 6d65   path in microme
+00010ad0: 7472 6520 746f 2063 616c 6375 6c61 7465  tre to calculate
+00010ae0: 2073 696d 706c 6520 626f 756e 6461 7279   simple boundary
+00010af0: 0a20 2020 2020 2020 2020 2020 2073 6361  .            sca
+00010b00: 7474 6572 696e 6720 636f 6e74 7269 6275  ttering contribu
+00010b10: 7469 6f6e 2074 6f20 7468 6572 6d61 6c20  tion to thermal 
+00010b20: 636f 6e64 7563 7469 7669 7479 2e0a 2020  conductivity..  
+00010b30: 2020 2020 2020 2020 2020 4e6f 6e65 2069            None i
+00010b40: 676e 6f72 6573 2074 6869 7320 636f 6e74  gnores this cont
+00010b50: 7269 6275 7469 6f6e 2e0a 2020 2020 2020  ribution..      
+00010b60: 2020 736f 6c76 655f 636f 6c6c 6563 7469    solve_collecti
+00010b70: 7665 5f70 686f 6e6f 6e20 3a20 626f 6f6c  ve_phonon : bool
+00010b80: 2c20 6f70 7469 6f6e 616c 2c20 6465 6661  , optional, defa
+00010b90: 756c 7420 6973 2046 616c 7365 0a20 2020  ult is False.   
+00010ba0: 2020 2020 2020 2020 2054 6869 7320 6973           This is
+00010bb0: 2061 6e20 6f70 7469 6f6e 2066 6f72 2074   an option for t
+00010bc0: 6865 2066 6561 7475 7265 2075 6e64 6572  he feature under
+00010bd0: 2064 6576 656c 6f70 6d65 6e74 2e0a 2020   development..  
+00010be0: 2020 2020 2020 7573 655f 6176 655f 7070        use_ave_pp
+00010bf0: 203a 2062 6f6f 6c2c 206f 7074 696f 6e61   : bool, optiona
+00010c00: 6c2c 2064 6566 6175 6c74 2069 7320 4661  l, default is Fa
+00010c10: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
+00010c20: 5254 4120 6f6e 6c79 2028 6069 735f 4c42  RTA only (`is_LB
+00010c30: 5445 3d46 616c 7365 6029 2e20 4176 6572  TE=False`). Aver
+00010c40: 6167 6564 2070 686f 6e6f 6e2d 7068 6f6e  aged phonon-phon
+00010c50: 6f6e 2069 6e74 6572 6163 7469 6f6e 0a20  on interaction. 
+00010c60: 2020 2020 2020 2020 2020 2073 7472 656e             stren
+00010c70: 6774 6820 6973 2075 7365 6420 746f 2063  gth is used to c
+00010c80: 616c 6375 6c61 7465 2070 686f 6e6f 6e20  alculate phonon 
+00010c90: 6c69 6665 7469 6d65 2e20 5468 6973 2064  lifetime. This d
+00010ca0: 6f65 7320 6e6f 740a 2020 2020 2020 2020  oes not.        
+00010cb0: 2020 2020 7265 6475 6365 2063 6f6d 7075      reduce compu
+00010cc0: 7461 7469 6f6e 616c 2064 656d 616e 642c  tational demand,
+00010cd0: 2062 7574 206d 6179 2062 6520 7573 6564   but may be used
+00010ce0: 2074 6f20 6d6f 6465 6c20 7468 6572 6d61   to model therma
+00010cf0: 6c0a 2020 2020 2020 2020 2020 2020 636f  l.            co
+00010d00: 6e64 7563 7469 7669 7479 2066 6f72 2061  nductivity for a
+00010d10: 6e61 6c79 7a65 2074 6865 2063 616c 6375  nalyze the calcu
+00010d20: 6c61 7469 6f6e 2072 6573 756c 7473 2e0a  lation results..
+00010d30: 2020 2020 2020 2020 6973 5f72 6564 7563          is_reduc
+00010d40: 6962 6c65 5f63 6f6c 6c69 7369 6f6e 5f6d  ible_collision_m
+00010d50: 6174 7269 7820 3a20 626f 6f6c 2c20 6f70  atrix : bool, op
+00010d60: 7469 6f6e 616c 2c20 6465 6661 756c 7420  tional, default 
+00010d70: 6973 2046 616c 7365 0a20 2020 2020 2020  is False.       
+00010d80: 2020 2020 2044 6972 6563 7420 736f 6c75       Direct solu
+00010d90: 7469 6f6e 206f 6e6c 7920 2860 6973 5f4c  tion only (`is_L
+00010da0: 4254 453d 5472 7565 6029 2e20 5468 6973  BTE=True`). This
+00010db0: 2069 7320 616e 2065 7870 6572 696d 656e   is an experimen
+00010dc0: 7461 6c0a 2020 2020 2020 2020 2020 2020  tal.            
+00010dd0: 6f70 7469 6f6e 2e20 5769 7468 2054 7275  option. With Tru
+00010de0: 652c 2066 756c 6c20 636f 6c6c 6973 696f  e, full collisio
+00010df0: 6e20 6d61 7472 6978 2069 7320 6372 6561  n matrix is crea
+00010e00: 7465 6420 616e 6420 736f 6c76 6564 2e0a  ted and solved..
+00010e10: 2020 2020 2020 2020 6973 5f6b 6170 7061          is_kappa
+00010e20: 5f73 7461 7220 3a20 626f 6f6c 2c20 6f70  _star : bool, op
+00010e30: 7469 6f6e 616c 2c20 6465 6661 756c 7420  tional, default 
+00010e40: 6973 2054 7275 650a 2020 2020 2020 2020  is True.        
+00010e50: 2020 2020 5769 7468 2074 7275 652c 2073      With true, s
+00010e60: 796d 6d65 7472 7920 6973 2063 6f6e 7369  ymmetry is consi
+00010e70: 6465 7265 6420 7768 656e 2073 616d 706c  dered when sampl
+00010e80: 696e 6720 6772 6964 2070 6f69 6e74 730a  ing grid points.
+00010e90: 2020 2020 2020 2020 2020 2020 6174 2077              at w
+00010ea0: 6869 6368 206d 6f64 6520 7468 6572 6d61  hich mode therma
+00010eb0: 6c20 636f 6e64 7563 7469 7669 7469 6573  l conductivities
+00010ec0: 2061 7265 2063 616c 6375 6c61 7465 642e   are calculated.
+00010ed0: 0a20 2020 2020 2020 2067 765f 6465 6c74  .        gv_delt
+00010ee0: 615f 7120 3a20 666c 6f61 742c 206f 7074  a_q : float, opt
+00010ef0: 696f 6e61 6c2c 2064 6566 6175 6c74 2069  ional, default i
+00010f00: 7320 4e6f 6e65 2c20 2023 2066 6f72 2067  s None,  # for g
+00010f10: 726f 7570 2076 656c 6f63 6974 790a 2020  roup velocity.  
+00010f20: 2020 2020 2020 2020 2020 5769 7468 206e            With n
+00010f30: 6f6e 2d61 6e61 6c79 7469 6361 6c20 636f  on-analytical co
+00010f40: 7272 6563 7469 6f6e 2c20 6772 6f75 7020  rrection, group 
+00010f50: 7665 6c6f 6369 7479 2069 7320 6361 6c63  velocity is calc
+00010f60: 756c 6174 6564 0a20 2020 2020 2020 2020  ulated.         
+00010f70: 2020 2062 7920 6365 6e74 7261 6c20 6669     by central fi
+00010f80: 6e69 7465 2064 6966 6665 7265 6e63 6520  nite difference 
+00010f90: 6d65 7468 6f64 2e20 5468 6973 2076 616c  method. This val
+00010fa0: 7565 2067 6976 6573 2074 6865 2064 6973  ue gives the dis
+00010fb0: 7461 6e63 650a 2020 2020 2020 2020 2020  tance.          
+00010fc0: 2020 696e 2062 6f74 6820 6469 7265 6374    in both direct
+00010fd0: 696f 6e73 2069 6e20 312f 416e 6773 7472  ions in 1/Angstr
+00010fe0: 6f6d 2e20 5468 6520 6465 6661 756c 7420  om. The default 
+00010ff0: 7661 6c75 6520 7769 6c6c 2062 6520 3165  value will be 1e
+00011000: 2d35 2e0a 2020 2020 2020 2020 6973 5f66  -5..        is_f
+00011010: 756c 6c5f 7070 203a 2062 6f6f 6c2c 206f  ull_pp : bool, o
+00011020: 7074 696f 6e61 6c2c 2064 6566 6175 6c74  ptional, default
+00011030: 2069 7320 4661 6c73 650a 2020 2020 2020   is False.      
+00011040: 2020 2020 2020 5769 7468 2054 7275 652c        With True,
+00011050: 2066 756c 6c20 656c 656d 656e 7473 206f   full elements o
+00011060: 6620 7068 6f6e 6f6e 2d70 686f 6e6f 6e20  f phonon-phonon 
+00011070: 696e 7465 7261 6374 696f 6e20 7374 7265  interaction stre
+00011080: 6e67 7468 0a20 2020 2020 2020 2020 2020  ngth.           
+00011090: 2061 7265 2063 6f6d 7075 7465 642e 2048   are computed. H
+000110a0: 6f77 6576 6572 2077 6974 6820 7465 7472  owever with tetr
+000110b0: 6168 6564 726f 6e20 6d65 7468 6f64 2c20  ahedron method, 
+000110c0: 7061 7274 206f 6620 7468 656d 2061 7265  part of them are
+000110d0: 0a20 2020 2020 2020 2020 2020 206b 6e6f  .            kno
+000110e0: 776e 2074 6f20 6265 207a 6572 6f20 616e  wn to be zero an
+000110f0: 6420 756e 6e65 6365 7373 6172 7920 746f  d unnecessary to
+00011100: 2063 616c 6375 6c61 7469 6f6e 2e20 5769   calculation. Wi
+00011110: 7468 2046 616c 7365 2c0a 2020 2020 2020  th False,.      
+00011120: 2020 2020 2020 7468 6f73 6520 656c 656d        those elem
+00011130: 656e 7473 2061 7265 206e 6f74 2063 616c  ents are not cal
+00011140: 6375 6c61 7465 642c 2062 7920 7768 6963  culated, by whic
+00011150: 6820 636f 6e73 6964 6572 6162 6c65 0a20  h considerable. 
+00011160: 2020 2020 2020 2020 2020 2069 6d70 726f             impro
+00011170: 7665 206f 6620 6566 6669 6369 656e 6379  ve of efficiency
+00011180: 2069 7320 6578 7065 6374 6564 2e0a 2020   is expected..  
+00011190: 2020 2020 2020 2020 2020 5769 7468 2073            With s
+000111a0: 6d65 6172 696e 6720 6d65 7468 6f64 2c20  mearing method, 
+000111b0: 6576 656e 2069 6620 7468 6973 2069 7320  even if this is 
+000111c0: 7365 7420 4661 6c73 652c 2066 756c 6c20  set False, full 
+000111d0: 656c 656d 656e 7473 0a20 2020 2020 2020  elements.       
+000111e0: 2020 2020 2061 7265 2063 6f6d 7075 7465       are compute
+000111f0: 6420 756e 6c65 7373 2060 7369 676d 615f  d unless `sigma_
+00011200: 6375 746f 6666 6020 6973 2073 7065 6369  cutoff` is speci
+00011210: 6669 6564 2e0a 2020 2020 2020 2020 7069  fied..        pi
+00011220: 6e76 5f63 7574 6f66 6620 3a20 666c 6f61  nv_cutoff : floa
+00011230: 742c 206f 7074 696f 6e61 6c2c 2064 6566  t, optional, def
+00011240: 6175 6c74 2069 7320 312e 3065 2d38 0a20  ault is 1.0e-8. 
+00011250: 2020 2020 2020 2020 2020 2044 6972 6563             Direc
+00011260: 7420 736f 6c75 7469 6f6e 206f 6e6c 7920  t solution only 
+00011270: 2860 6973 5f4c 4254 453d 5472 7565 6029  (`is_LBTE=True`)
+00011280: 2e20 5468 6973 2069 7320 7573 6564 2061  . This is used a
+00011290: 7320 6120 6372 6974 6572 696f 6e0a 2020  s a criterion.  
+000112a0: 2020 2020 2020 2020 2020 746f 206a 7564            to jud
+000112b0: 6765 2074 6865 2065 6967 656e 7661 6c75  ge the eigenvalu
+000112c0: 6573 2061 7265 2063 6f6e 7369 6465 7265  es are considere
+000112d0: 6420 6173 207a 6572 6f20 6f72 206e 6f74  d as zero or not
+000112e0: 2069 6e0a 2020 2020 2020 2020 2020 2020   in.            
+000112f0: 7073 6575 646f 2d69 6e76 6572 7369 6f6e  pseudo-inversion
+00011300: 206f 6620 636f 6c6c 6973 696f 6e20 6d61   of collision ma
+00011310: 7472 6978 2e20 5365 6520 616c 736f 2060  trix. See also `
+00011320: 7069 6e76 5f6d 6574 686f 6460 2e0a 2020  pinv_method`..  
+00011330: 2020 2020 2020 7069 6e76 5f6d 6574 686f        pinv_metho
+00011340: 6420 3a20 696e 742c 206f 7074 696f 6e61  d : int, optiona
+00011350: 6c2c 2064 6566 6175 6c74 2069 7320 302e  l, default is 0.
+00011360: 0a20 2020 2020 2020 2020 2020 2044 6972  .            Dir
+00011370: 6563 7420 736f 6c75 7469 6f6e 206f 6e6c  ect solution onl
+00011380: 7920 2860 6973 5f4c 4254 453d 5472 7565  y (`is_LBTE=True
+00011390: 6029 2e0a 2020 2020 2020 2020 2020 2020  `)..            
+000113a0: 2020 2020 302e 2061 6273 2865 6967 656e      0. abs(eigen
+000113b0: 7661 6c75 6529 203c 2060 7069 6e76 5f63  value) < `pinv_c
+000113c0: 7574 6f66 6660 0a20 2020 2020 2020 2020  utoff`.         
+000113d0: 2020 2020 2020 2031 2e20 6569 6765 6e76         1. eigenv
+000113e0: 616c 7565 203c 2060 7069 6e76 5f63 7574  alue < `pinv_cut
+000113f0: 6f66 6660 0a20 2020 2020 2020 2070 696e  off`.        pin
+00011400: 765f 736f 6c76 6572 203a 2069 6e74 2c20  v_solver : int, 
+00011410: 6f70 7469 6f6e 616c 2c20 6465 6661 756c  optional, defaul
+00011420: 7420 6973 2030 0a20 2020 2020 2020 2020  t is 0.         
+00011430: 2020 2044 6972 6563 7420 736f 6c75 7469     Direct soluti
+00011440: 6f6e 206f 6e6c 7920 2860 6973 5f4c 4254  on only (`is_LBT
+00011450: 453d 5472 7565 6029 2e20 4368 6f69 6365  E=True`). Choice
+00011460: 206f 6620 736f 6c76 6572 206f 660a 2020   of solver of.  
+00011470: 2020 2020 2020 2020 2020 7073 6575 646f            pseudo
+00011480: 2d69 6e76 6572 7369 6f6e 206f 6620 636f  -inversion of co
+00011490: 6c6c 6973 696f 6e20 6d61 7472 6978 2e20  llision matrix. 
+000114a0: 3020 6d65 616e 7320 7468 6520 6465 6661  0 means the defa
+000114b0: 756c 7420 6368 6f69 6365 2e0a 2020 2020  ult choice..    
+000114c0: 2020 2020 2020 2020 2020 2020 312e 204c              1. L
+000114d0: 6170 6163 6b65 2064 7379 6576 3a20 536d  apacke dsyev: Sm
+000114e0: 616c 6c65 7220 6d65 6d6f 7279 2063 6f6e  aller memory con
+000114f0: 7375 6d70 7469 6f6e 2074 6861 6e20 6473  sumption than ds
+00011500: 7965 7664 2c20 6275 740a 2020 2020 2020  yevd, but.      
+00011510: 2020 2020 2020 2020 2020 2020 2073 6c6f               slo
+00011520: 7765 722e 2054 6869 7320 6973 2074 6865  wer. This is the
+00011530: 2064 6566 6175 6c74 2073 6f6c 7665 7220   default solver 
+00011540: 7768 656e 204d 4b4c 204c 4150 4143 4b45  when MKL LAPACKE
+00011550: 2069 730a 2020 2020 2020 2020 2020 2020   is.            
+00011560: 2020 2020 2020 2069 6e74 6567 7261 7465         integrate
+00011570: 6420 6f72 2073 6369 7079 2069 7320 6e6f  d or scipy is no
+00011580: 7420 696e 7374 616c 6c65 642e 0a20 2020  t installed..   
+00011590: 2020 2020 2020 2020 2020 2020 2032 2e20               2. 
+000115a0: 4c61 7061 636b 6520 6473 7965 7664 3a20  Lapacke dsyevd: 
+000115b0: 4c61 7267 6572 206d 656d 6f72 7920 636f  Larger memory co
+000115c0: 6e73 756d 7074 696f 6e20 7468 616e 2064  nsumption than d
+000115d0: 7379 6576 2c20 6275 740a 2020 2020 2020  syev, but.      
+000115e0: 2020 2020 2020 2020 2020 2020 2066 6173               fas
+000115f0: 7465 722e 2054 6869 7320 6973 206e 6f74  ter. This is not
+00011600: 2072 6563 6f6d 6d65 6e64 6564 2062 6563   recommended bec
+00011610: 6175 7365 2073 6f6d 6574 696d 6573 2061  ause sometimes a
+00011620: 2077 726f 6e67 0a20 2020 2020 2020 2020   wrong.         
+00011630: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00011640: 2069 7320 6f62 7461 696e 6564 2e0a 2020   is obtained..  
+00011650: 2020 2020 2020 2020 2020 2020 2020 332e                3.
+00011660: 204e 756d 7079 e280 9973 2064 7379 6576   Numpy...s dsyev
+00011670: 6420 286c 696e 616c 672e 6569 6768 292e  d (linalg.eigh).
+00011680: 2054 6869 7320 6973 206e 6f74 2072 6563   This is not rec
+00011690: 6f6d 6d65 6e64 6564 0a20 2020 2020 2020  ommended.       
+000116a0: 2020 2020 2020 2020 2020 2020 6265 6361              beca
+000116b0: 7573 6520 736f 6d65 7469 6d65 7320 6120  use sometimes a 
+000116c0: 7772 6f6e 6720 7265 7375 6c74 2069 7320  wrong result is 
+000116d0: 6f62 7461 696e 6564 2e0a 2020 2020 2020  obtained..      
+000116e0: 2020 2020 2020 2020 2020 342e 2053 6369            4. Sci
+000116f0: 7079 e280 9973 2064 7379 6576 3a20 5468  py...s dsyev: Th
+00011700: 6973 2069 7320 7468 6520 6465 6661 756c  is is the defaul
+00011710: 7420 736f 6c76 6572 2077 6865 6e20 7363  t solver when sc
+00011720: 6970 7920 6973 0a20 2020 2020 2020 2020  ipy is.         
+00011730: 2020 2020 2020 2020 2020 696e 7374 616c            instal
+00011740: 6c65 6420 616e 6420 4d4b 4c20 4c41 5041  led and MKL LAPA
+00011750: 434b 4520 6973 206e 6f74 2069 6e74 6567  CKE is not integ
+00011760: 7261 7465 642e 0a20 2020 2020 2020 2020  rated..         
+00011770: 2020 2020 2020 2035 2e20 5363 6970 79e2         5. Scipy.
+00011780: 8099 7320 6473 7965 7664 2e20 5468 6973  ..s dsyevd. This
+00011790: 2069 7320 6e6f 7420 7265 636f 6d6d 656e   is not recommen
+000117a0: 6465 6420 6265 6361 7573 6520 736f 6d65  ded because some
+000117b0: 7469 6d65 730a 2020 2020 2020 2020 2020  times.          
+000117c0: 2020 2020 2020 2020 2061 2077 726f 6e67           a wrong
+000117d0: 2072 6573 756c 7420 6973 206f 6274 6169   result is obtai
+000117e0: 6e65 642e 0a20 2020 2020 2020 2020 2020  ned..           
+000117f0: 2054 6865 2073 6f6c 7665 7220 6368 6f69   The solver choi
+00011800: 6365 7320 6f74 6865 7220 7468 616e 202d  ces other than -
+00011810: 2d70 696e 762d 736f 6c76 6572 3d31 2061  -pinv-solver=1 a
+00011820: 6e64 0a20 2020 2020 2020 2020 2020 202d  nd.            -
+00011830: 2d70 696e 762d 736f 6c76 6572 3d34 2061  -pinv-solver=4 a
+00011840: 7265 2064 616e 6765 726f 7573 2061 6e64  re dangerous and
+00011850: 206e 6f74 2072 6563 6f6d 6d65 6e64 2e0a   not recommend..
+00011860: 2020 2020 2020 2020 7772 6974 655f 6761          write_ga
+00011870: 6d6d 6120 3a20 626f 6f6c 2c20 6f70 7469  mma : bool, opti
+00011880: 6f6e 616c 2c20 6465 6661 756c 7420 6973  onal, default is
+00011890: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
+000118a0: 2020 2052 5441 206f 6e6c 7920 2860 6973     RTA only (`is
+000118b0: 5f4c 4254 453d 4661 6c73 6560 292e 2057  _LBTE=False`). W
+000118c0: 6974 6820 5472 7565 2c20 5772 6974 6520  ith True, Write 
+000118d0: 6d6f 6465 2074 6865 726d 616c 0a20 2020  mode thermal.   
+000118e0: 2020 2020 2020 2020 2063 6f6e 6475 6374           conduct
+000118f0: 6976 6974 7920 7072 6f70 6572 7469 6573  ivity properties
+00011900: 2069 6e74 6f20 6669 6c65 7320 6174 2065   into files at e
+00011910: 6163 6820 6772 6964 2070 6f69 6e74 2e20  ach grid point. 
+00011920: 5769 7468 0a20 2020 2020 2020 2020 2020  With.           
+00011930: 2060 6261 6e64 5f69 6e64 6963 6573 6020   `band_indices` 
+00011940: 6f72 206d 756c 7469 706c 6520 6073 6967  or multiple `sig
+00011950: 6d61 7360 2069 7320 7370 6563 6966 6965  mas` is specifie
+00011960: 642c 2074 6865 2066 696c 6573 0a20 2020  d, the files.   
+00011970: 2020 2020 2020 2020 2061 7265 206d 6164           are mad
+00011980: 6520 666f 7220 6561 6368 206f 6620 7468  e for each of th
+00011990: 656d 2c20 746f 6f2e 0a20 2020 2020 2020  em, too..       
+000119a0: 2072 6561 645f 6761 6d6d 6120 3a20 626f   read_gamma : bo
+000119b0: 6f6c 2c20 6f70 7469 6f6e 616c 2c20 6465  ol, optional, de
+000119c0: 6661 756c 7420 6973 2046 616c 7365 0a20  fault is False. 
+000119d0: 2020 2020 2020 2020 2020 2052 5441 206f             RTA o
+000119e0: 6e6c 7920 2860 6973 5f4c 4254 453d 4661  nly (`is_LBTE=Fa
+000119f0: 6c73 6560 292e 2057 6974 6820 5472 7565  lse`). With True
+00011a00: 2c20 6465 6164 2066 696c 6573 2063 7265  , dead files cre
+00011a10: 6174 6564 2062 790a 2020 2020 2020 2020  ated by.        
+00011a20: 2020 2020 6077 7269 7465 5f67 616d 6d61      `write_gamma
+00011a30: 3d54 7275 6560 2069 6e73 7465 6164 206f  =True` instead o
+00011a40: 6620 6361 6c63 756c 6174 696e 6720 7068  f calculating ph
+00011a50: 6f6e 6f6e 2d70 686f 6e6f 6e0a 2020 2020  onon-phonon.    
+00011a60: 2020 2020 2020 2020 696e 7465 7261 6374          interact
+00011a70: 696f 6e20 7374 7265 6e67 7468 2061 6e64  ion strength and
+00011a80: 2069 6d61 6769 6e61 7279 2070 6172 7473   imaginary parts
+00011a90: 206f 6620 7365 6c66 2d65 6e65 7267 792e   of self-energy.
+00011aa0: 0a20 2020 2020 2020 2069 735f 4e5f 5520  .        is_N_U 
+00011ab0: 3a20 626f 6f6c 2c20 6f70 7469 6f6e 616c  : bool, optional
+00011ac0: 2c20 6465 6661 756c 7420 6973 2046 616c  , default is Fal
+00011ad0: 7365 0a20 2020 2020 2020 2020 2020 2052  se.            R
+00011ae0: 5441 206f 6e6c 7920 2860 6973 5f4c 4254  TA only (`is_LBT
+00011af0: 453d 4661 6c73 6560 292e 2057 6974 6820  E=False`). With 
+00011b00: 5472 7565 2c20 6361 7465 676f 7269 7a61  True, categoriza
+00011b10: 7469 6f6e 206f 6620 6e6f 726d 616c 0a20  tion of normal. 
+00011b20: 2020 2020 2020 2020 2020 2061 6e64 2055             and U
+00011b30: 6d6b 6c61 7070 2073 6361 7474 6572 696e  mklapp scatterin
+00011b40: 6720 6973 206d 6164 6520 616e 6420 696d  g is made and im
+00011b50: 6167 696e 6172 7920 7061 7274 7320 6f66  aginary parts of
+00011b60: 2073 656c 6620 656e 6572 6779 0a20 2020   self energy.   
+00011b70: 2020 2020 2020 2020 2066 6f72 2074 6865           for the
+00011b80: 6d20 6172 6520 7365 7061 7261 7465 642e  m are separated.
+00011b90: 0a20 2020 2020 2020 2063 6f6e 6475 6374  .        conduct
+00011ba0: 6976 6974 795f 7479 7065 203a 2073 7472  ivity_type : str
+00011bb0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+00011bc0: 2020 2020 2020 2022 7769 676e 6572 222c         "wigner",
+00011bd0: 2022 6b75 626f 222c 206f 7220 4e6f 6e65   "kubo", or None
+00011be0: 2e20 4465 6661 756c 7420 6973 204e 6f6e  . Default is Non
+00011bf0: 652e 0a20 2020 2020 2020 2077 7269 7465  e..        write
+00011c00: 5f6b 6170 7061 203a 2062 6f6f 6c2c 206f  _kappa : bool, o
+00011c10: 7074 696f 6e61 6c2c 2064 6566 6175 6c74  ptional, default
+00011c20: 2069 7320 4661 6c73 650a 2020 2020 2020   is False.      
+00011c30: 2020 2020 2020 5769 7468 2054 7275 652c        With True,
+00011c40: 2074 6865 726d 616c 2063 6f6e 6475 6374   thermal conduct
+00011c50: 6976 6974 7920 616e 6420 7265 6c61 7465  ivity and relate
+00011c60: 6420 7072 6f70 6572 7469 6573 2061 7265  d properties are
+00011c70: 0a20 2020 2020 2020 2020 2020 2077 7269  .            wri
+00011c80: 7474 656e 2069 6e74 6f20 6120 6669 6c65  tten into a file
+00011c90: 2e20 5769 7468 206d 756c 7469 706c 6520  . With multiple 
+00011ca0: 6073 6967 6d61 7360 2c20 7265 7370 6563  `sigmas`, respec
+00011cb0: 7469 7665 2066 696c 6573 0a20 2020 2020  tive files.     
+00011cc0: 2020 2020 2020 2061 7265 2063 7265 6174         are creat
+00011cd0: 6564 2e0a 2020 2020 2020 2020 7772 6974  ed..        writ
+00011ce0: 655f 6761 6d6d 615f 6465 7461 696c 203a  e_gamma_detail :
+00011cf0: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c2c   bool, optional,
+00011d00: 2064 6566 6175 6c74 2069 7320 4661 6c73   default is Fals
+00011d10: 650a 2020 2020 2020 2020 2020 2020 5254  e.            RT
+00011d20: 4120 6f6e 6c79 2028 6069 735f 4c42 5445  A only (`is_LBTE
+00011d30: 3d46 616c 7365 6029 2e20 5769 7468 2054  =False`). With T
+00011d40: 7275 652c 2064 6574 6169 6c65 6420 696e  rue, detailed in
+00011d50: 666f 726d 6174 696f 6e20 6f66 0a20 2020  formation of.   
+00011d60: 2020 2020 2020 2020 2069 6d61 6769 6e61           imagina
+00011d70: 7279 2070 6172 7473 206f 6620 7365 6c66  ry parts of self
+00011d80: 2065 6e65 7267 7920 6973 2073 746f 7265   energy is store
+00011d90: 6420 696e 746f 2066 696c 6573 2073 7563  d into files suc
+00011da0: 6820 6173 0a20 2020 2020 2020 2020 2020  h as.           
+00011db0: 2074 686f 7365 206d 6164 6520 6279 2060   those made by `
+00011dc0: 7772 6974 655f 6761 6d6d 6160 2e0a 2020  write_gamma`..  
+00011dd0: 2020 2020 2020 7772 6974 655f 636f 6c6c        write_coll
+00011de0: 6973 696f 6e20 3a20 626f 6f6c 2c20 6f70  ision : bool, op
+00011df0: 7469 6f6e 616c 2c20 6465 6661 756c 7420  tional, default 
+00011e00: 6973 2046 616c 7365 0a20 2020 2020 2020  is False.       
+00011e10: 2020 2020 2044 6972 6563 7420 736f 6c75       Direct solu
+00011e20: 7469 6f6e 206f 6e6c 7920 2860 6973 5f4c  tion only (`is_L
+00011e30: 4254 453d 5472 7565 6029 2e20 5769 7468  BTE=True`). With
+00011e40: 2054 7275 652c 2063 6f6c 6c69 7369 6f6e   True, collision
+00011e50: 206d 6174 7269 780a 2020 2020 2020 2020   matrix.        
+00011e60: 2020 2020 6973 2077 7269 7474 656e 2069      is written i
+00011e70: 6e74 6f20 6120 6669 6c65 2e20 5769 7468  nto a file. With
+00011e80: 206d 756c 7469 706c 6520 6073 6967 6d61   multiple `sigma
+00011e90: 7360 2073 7065 6369 6669 6564 2c0a 2020  s` specified,.  
+00011ea0: 2020 2020 2020 2020 2020 7265 7370 6563            respec
+00011eb0: 7469 7665 2066 696c 6573 2061 7265 2063  tive files are c
+00011ec0: 7265 6174 6564 2e20 4265 2063 6172 6566  reated. Be caref
+00011ed0: 756c 2074 6861 7420 7468 6973 2066 696c  ul that this fil
+00011ee0: 6520 6361 6e20 6265 0a20 2020 2020 2020  e can be.       
+00011ef0: 2020 2020 2068 7567 652e 0a20 2020 2020       huge..     
+00011f00: 2020 2072 6561 645f 636f 6c6c 6973 696f     read_collisio
+00011f10: 6e20 3a20 626f 6f6c 2c20 6f70 7469 6f6e  n : bool, option
+00011f20: 616c 2c20 6465 6661 756c 7420 6973 2046  al, default is F
+00011f30: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
+00011f40: 2044 6972 6563 7420 736f 6c75 7469 6f6e   Direct solution
+00011f50: 206f 6e6c 7920 2860 6973 5f4c 4254 453d   only (`is_LBTE=
+00011f60: 5472 7565 6029 2e20 5769 7468 2054 7275  True`). With Tru
+00011f70: 652c 2063 6f6c 6c69 7369 6f6e 206d 6174  e, collision mat
+00011f80: 7269 780a 2020 2020 2020 2020 2020 2020  rix.            
+00011f90: 6973 2072 6561 6420 6672 6f6d 2061 2066  is read from a f
+00011fa0: 696c 652e 0a20 2020 2020 2020 2077 7269  ile..        wri
+00011fb0: 7465 5f70 7020 3a20 626f 6f6c 2c20 6f70  te_pp : bool, op
+00011fc0: 7469 6f6e 616c 2c20 6465 6661 756c 7420  tional, default 
+00011fd0: 6973 2046 616c 7365 0a20 2020 2020 2020  is False.       
+00011fe0: 2020 2020 2057 6974 6820 5472 7565 2c20       With True, 
+00011ff0: 7068 6f6e 6f6e 2d70 686f 6e6f 6e20 696e  phonon-phonon in
+00012000: 7465 7261 6374 696f 6e20 7374 7265 6e67  teraction streng
+00012010: 7468 2069 7320 7772 6974 7465 6e20 696e  th is written in
+00012020: 746f 0a20 2020 2020 2020 2020 2020 2066  to.            f
+00012030: 696c 6573 2061 7420 6561 6368 2067 7269  iles at each gri
+00012040: 6420 706f 696e 742e 2054 6869 7320 6f70  d point. This op
+00012050: 7469 6f6e 2061 7373 756d 6573 2073 696e  tion assumes sin
+00012060: 676c 6520 7661 6c75 6520 6973 2069 6e0a  gle value is in.
+00012070: 2020 2020 2020 2020 2020 2020 6073 6967              `sig
+00012080: 6d61 7360 2e0a 2020 2020 2020 2020 7265  mas`..        re
+00012090: 6164 5f70 7020 3a20 626f 6f6c 2c20 6f70  ad_pp : bool, op
+000120a0: 7469 6f6e 616c 2c20 6465 6661 756c 7420  tional, default 
+000120b0: 6973 2046 616c 7365 0a20 2020 2020 2020  is False.       
+000120c0: 2020 2020 2057 6974 6820 5472 7565 2c20       With True, 
+000120d0: 7068 6f6e 6f6e 2d70 686f 6e6f 6e20 696e  phonon-phonon in
+000120e0: 7465 7261 6374 696f 6e20 7374 7265 6e67  teraction streng
+000120f0: 7468 2069 7320 7265 6164 2066 726f 6d20  th is read from 
+00012100: 6669 6c65 732e 0a20 2020 2020 2020 2077  files..        w
+00012110: 7269 7465 5f4c 4254 455f 736f 6c75 7469  rite_LBTE_soluti
+00012120: 6f6e 203a 2062 6f6f 6c2c 206f 7074 696f  on : bool, optio
+00012130: 6e61 6c2c 2064 6566 6175 6c74 2069 7320  nal, default is 
+00012140: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
+00012150: 2020 4469 7265 6374 2073 6f6c 7574 696f    Direct solutio
+00012160: 6e20 6f6e 6c79 2028 6069 735f 4c42 5445  n only (`is_LBTE
+00012170: 3d54 7275 6560 292e 2057 6974 6820 5472  =True`). With Tr
+00012180: 7565 2c20 6569 6765 6e76 6563 746f 7273  ue, eigenvectors
+00012190: 206f 660a 2020 2020 2020 2020 2020 2020   of.            
+000121a0: 636f 6c6c 6973 696f 6e20 6d61 7472 6978  collision matrix
+000121b0: 2069 7320 7772 6974 7465 6e20 696e 2061   is written in a
+000121c0: 2066 696c 6520 6173 2074 6865 2072 6f77   file as the row
+000121d0: 2076 6563 746f 7273 2065 7863 6570 740a   vectors except.
+000121e0: 2020 2020 2020 2020 2020 2020 756e 6c65              unle
+000121f0: 7373 2060 7069 6e76 5f73 6f6c 7665 723d  ss `pinv_solver=
+00012200: 3360 2028 666f 7220 7468 6973 2c20 636f  3` (for this, co
+00012210: 6c75 6d6e 2076 6563 746f 7273 292e 2057  lumn vectors). W
+00012220: 6974 6820 6d75 6c74 6970 6c65 0a20 2020  ith multiple.   
+00012230: 2020 2020 2020 2020 2060 7369 676d 6173           `sigmas
+00012240: 6020 7370 6563 6966 6965 642c 2072 6573  ` specified, res
+00012250: 7065 6374 6976 6520 6669 6c65 7320 6172  pective files ar
+00012260: 6520 6372 6561 7465 642e 2042 6520 6361  e created. Be ca
+00012270: 7265 6675 6c20 7468 6174 0a20 2020 2020  reful that.     
+00012280: 2020 2020 2020 2074 6869 7320 6669 6c65         this file
+00012290: 2063 616e 2062 6520 6875 6765 2e0a 2020   can be huge..  
+000122a0: 2020 2020 2020 636f 6d70 7265 7373 696f        compressio
+000122b0: 6e3a 2073 7472 2c20 6f70 7469 6f6e 616c  n: str, optional
+000122c0: 2c20 6465 6661 756c 7420 6973 2022 677a  , default is "gz
+000122d0: 6970 220a 2020 2020 2020 2020 2020 2020  ip".            
+000122e0: 5768 656e 2077 7269 7469 6e67 2072 6573  When writing res
+000122f0: 756c 7473 2069 6e74 6f20 6669 6c65 7320  ults into files 
+00012300: 696e 2068 6466 352c 206c 6172 6765 2064  in hdf5, large d
+00012310: 6174 6120 6172 6520 636f 6d70 7265 7373  ata are compress
+00012320: 6564 0a20 2020 2020 2020 2020 2020 2062  ed.            b
+00012330: 7920 7468 6973 206f 7074 696f 6e73 2e20  y this options. 
+00012340: 5365 6520 7468 6520 6465 7461 696c 2061  See the detail a
+00012350: 7420 6835 7079 2064 6f63 756d 656e 7461  t h5py documenta
+00012360: 7469 6f6e 2e0a 2020 2020 2020 2020 696e  tion..        in
+00012370: 7075 745f 6669 6c65 6e61 6d65 203a 2073  put_filename : s
+00012380: 7472 2c20 6f70 7469 6f6e 616c 2c20 6465  tr, optional, de
+00012390: 6661 756c 7420 6973 204e 6f6e 650a 2020  fault is None.  
+000123a0: 2020 2020 2020 2020 2020 5768 656e 2073            When s
+000123b0: 7065 6369 6669 6564 2c20 7468 6520 7374  pecified, the st
+000123c0: 7269 6e67 2069 7320 696e 7365 7274 6564  ring is inserted
+000123d0: 2062 6566 6f72 6520 6669 6c65 6e61 6d65   before filename
+000123e0: 2065 7874 656e 7369 6f6e 0a20 2020 2020   extension.     
+000123f0: 2020 2020 2020 2069 6e20 7265 6164 696e         in readin
+00012400: 6720 6669 6c65 732e 0a20 2020 2020 2020  g files..       
+00012410: 206f 7574 7075 745f 6669 6c65 6e61 6d65   output_filename
+00012420: 203a 2073 7472 2c20 6f70 7469 6f6e 616c   : str, optional
+00012430: 2c20 6465 6661 756c 7420 6973 204e 6f6e  , default is Non
+00012440: 650a 2020 2020 2020 2020 2020 2020 5768  e.            Wh
+00012450: 656e 2073 7065 6369 6669 6564 2c20 7468  en specified, th
+00012460: 6520 7374 7269 6e67 2069 7320 696e 7365  e string is inse
+00012470: 7274 6564 2062 6566 6f72 6520 6669 6c65  rted before file
+00012480: 6e61 6d65 2065 7874 656e 7369 6f6e 0a20  name extension. 
+00012490: 2020 2020 2020 2020 2020 2069 6e20 7772             in wr
+000124a0: 6974 696e 6720 6669 6c65 732e 0a0a 2020  iting files...  
+000124b0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000124c0: 2020 6966 2073 656c 662e 5f69 6e74 6572    if self._inter
+000124d0: 6163 7469 6f6e 2069 7320 4e6f 6e65 3a0a  action is None:.
+000124e0: 2020 2020 2020 2020 2020 2020 6d73 6720              msg 
+000124f0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+00012500: 2020 2020 2250 686f 6e6f 3370 792e 696e      "Phono3py.in
+00012510: 6974 5f70 6870 685f 696e 7465 7261 6374  it_phph_interact
+00012520: 696f 6e20 6861 7320 746f 2062 6520 6361  ion has to be ca
+00012530: 6c6c 6564 2022 0a20 2020 2020 2020 2020  lled ".         
+00012540: 2020 2020 2020 2022 6265 666f 7265 2072         "before r
+00012550: 756e 6e69 6e67 2074 6869 7320 6d65 7468  unning this meth
+00012560: 6f64 2e22 0a20 2020 2020 2020 2020 2020  od.".           
+00012570: 2029 0a20 2020 2020 2020 2020 2020 2072   ).            r
+00012580: 6169 7365 2052 756e 7469 6d65 4572 726f  aise RuntimeErro
+00012590: 7228 6d73 6729 0a0a 2020 2020 2020 2020  r(msg)..        
+000125a0: 6966 2069 735f 4c42 5445 3a0a 2020 2020  if is_LBTE:.    
+000125b0: 2020 2020 2020 2020 6966 2074 656d 7065          if tempe
+000125c0: 7261 7475 7265 7320 6973 204e 6f6e 653a  ratures is None:
+000125d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000125e0: 205f 7465 6d70 6572 6174 7572 6573 203d   _temperatures =
+000125f0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00012600: 2020 2020 2020 2033 3030 2c0a 2020 2020         300,.    
+00012610: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
+00012620: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00012630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012640: 5f74 656d 7065 7261 7475 7265 7320 3d20  _temperatures = 
+00012650: 7465 6d70 6572 6174 7572 6573 0a20 2020  temperatures.   
+00012660: 2020 2020 2020 2020 2073 656c 662e 5f74           self._t
+00012670: 6865 726d 616c 5f63 6f6e 6475 6374 6976  hermal_conductiv
+00012680: 6974 7920 3d20 6765 745f 7468 6572 6d61  ity = get_therma
+00012690: 6c5f 636f 6e64 7563 7469 7669 7479 5f4c  l_conductivity_L
+000126a0: 4254 4528 0a20 2020 2020 2020 2020 2020  BTE(.           
+000126b0: 2020 2020 2073 656c 662e 5f69 6e74 6572       self._inter
+000126c0: 6163 7469 6f6e 2c0a 2020 2020 2020 2020  action,.        
+000126d0: 2020 2020 2020 2020 7465 6d70 6572 6174          temperat
+000126e0: 7572 6573 3d5f 7465 6d70 6572 6174 7572  ures=_temperatur
+000126f0: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+00012700: 2020 2020 7369 676d 6173 3d73 656c 662e      sigmas=self.
+00012710: 5f73 6967 6d61 732c 0a20 2020 2020 2020  _sigmas,.       
+00012720: 2020 2020 2020 2020 2073 6967 6d61 5f63           sigma_c
+00012730: 7574 6f66 663d 7365 6c66 2e5f 7369 676d  utoff=self._sigm
+00012740: 615f 6375 746f 6666 2c0a 2020 2020 2020  a_cutoff,.      
+00012750: 2020 2020 2020 2020 2020 6973 5f69 736f            is_iso
+00012760: 746f 7065 3d69 735f 6973 6f74 6f70 652c  tope=is_isotope,
+00012770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012780: 206d 6173 735f 7661 7269 616e 6365 733d   mass_variances=
+00012790: 6d61 7373 5f76 6172 6961 6e63 6573 2c0a  mass_variances,.
+000127a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000127b0: 6772 6964 5f70 6f69 6e74 733d 6772 6964  grid_points=grid
+000127c0: 5f70 6f69 6e74 732c 0a20 2020 2020 2020  _points,.       
+000127d0: 2020 2020 2020 2020 2062 6f75 6e64 6172           boundar
+000127e0: 795f 6d66 703d 626f 756e 6461 7279 5f6d  y_mfp=boundary_m
+000127f0: 6670 2c0a 2020 2020 2020 2020 2020 2020  fp,.            
+00012800: 2020 2020 736f 6c76 655f 636f 6c6c 6563      solve_collec
+00012810: 7469 7665 5f70 686f 6e6f 6e3d 736f 6c76  tive_phonon=solv
+00012820: 655f 636f 6c6c 6563 7469 7665 5f70 686f  e_collective_pho
+00012830: 6e6f 6e2c 0a20 2020 2020 2020 2020 2020  non,.           
+00012840: 2020 2020 2069 735f 7265 6475 6369 626c       is_reducibl
+00012850: 655f 636f 6c6c 6973 696f 6e5f 6d61 7472  e_collision_matr
+00012860: 6978 3d69 735f 7265 6475 6369 626c 655f  ix=is_reducible_
+00012870: 636f 6c6c 6973 696f 6e5f 6d61 7472 6978  collision_matrix
+00012880: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00012890: 2020 6973 5f6b 6170 7061 5f73 7461 723d    is_kappa_star=
+000128a0: 6973 5f6b 6170 7061 5f73 7461 722c 0a20  is_kappa_star,. 
+000128b0: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+000128c0: 765f 6465 6c74 615f 713d 6776 5f64 656c  v_delta_q=gv_del
+000128d0: 7461 5f71 2c0a 2020 2020 2020 2020 2020  ta_q,.          
+000128e0: 2020 2020 2020 6973 5f66 756c 6c5f 7070        is_full_pp
+000128f0: 3d69 735f 6675 6c6c 5f70 702c 0a20 2020  =is_full_pp,.   
+00012900: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00012910: 6475 6374 6976 6974 795f 7479 7065 3d63  ductivity_type=c
+00012920: 6f6e 6475 6374 6976 6974 795f 7479 7065  onductivity_type
+00012930: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00012940: 2020 7069 6e76 5f63 7574 6f66 663d 7069    pinv_cutoff=pi
+00012950: 6e76 5f63 7574 6f66 662c 0a20 2020 2020  nv_cutoff,.     
+00012960: 2020 2020 2020 2020 2020 2070 696e 765f             pinv_
+00012970: 736f 6c76 6572 3d70 696e 765f 736f 6c76  solver=pinv_solv
+00012980: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+00012990: 2020 2020 7069 6e76 5f6d 6574 686f 643d      pinv_method=
+000129a0: 7069 6e76 5f6d 6574 686f 642c 0a20 2020  pinv_method,.   
+000129b0: 2020 2020 2020 2020 2020 2020 2077 7269               wri
+000129c0: 7465 5f63 6f6c 6c69 7369 6f6e 3d77 7269  te_collision=wri
+000129d0: 7465 5f63 6f6c 6c69 7369 6f6e 2c0a 2020  te_collision,.  
+000129e0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000129f0: 6164 5f63 6f6c 6c69 7369 6f6e 3d72 6561  ad_collision=rea
+00012a00: 645f 636f 6c6c 6973 696f 6e2c 0a20 2020  d_collision,.   
+00012a10: 2020 2020 2020 2020 2020 2020 2077 7269               wri
+00012a20: 7465 5f6b 6170 7061 3d77 7269 7465 5f6b  te_kappa=write_k
+00012a30: 6170 7061 2c0a 2020 2020 2020 2020 2020  appa,.          
+00012a40: 2020 2020 2020 7772 6974 655f 7070 3d77        write_pp=w
+00012a50: 7269 7465 5f70 702c 0a20 2020 2020 2020  rite_pp,.       
+00012a60: 2020 2020 2020 2020 2072 6561 645f 7070           read_pp
+00012a70: 3d72 6561 645f 7070 2c0a 2020 2020 2020  =read_pp,.      
+00012a80: 2020 2020 2020 2020 2020 7772 6974 655f            write_
+00012a90: 4c42 5445 5f73 6f6c 7574 696f 6e3d 7772  LBTE_solution=wr
+00012aa0: 6974 655f 4c42 5445 5f73 6f6c 7574 696f  ite_LBTE_solutio
+00012ab0: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
+00012ac0: 2020 2063 6f6d 7072 6573 7369 6f6e 3d63     compression=c
+00012ad0: 6f6d 7072 6573 7369 6f6e 2c0a 2020 2020  ompression,.    
+00012ae0: 2020 2020 2020 2020 2020 2020 696e 7075              inpu
+00012af0: 745f 6669 6c65 6e61 6d65 3d69 6e70 7574  t_filename=input
+00012b00: 5f66 696c 656e 616d 652c 0a20 2020 2020  _filename,.     
+00012b10: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+00012b20: 745f 6669 6c65 6e61 6d65 3d6f 7574 7075  t_filename=outpu
+00012b30: 745f 6669 6c65 6e61 6d65 2c0a 2020 2020  t_filename,.    
+00012b40: 2020 2020 2020 2020 2020 2020 6c6f 675f              log_
+00012b50: 6c65 7665 6c3d 7365 6c66 2e5f 6c6f 675f  level=self._log_
+00012b60: 6c65 7665 6c2c 0a20 2020 2020 2020 2020  level,.         
+00012b70: 2020 2029 0a20 2020 2020 2020 2065 6c73     ).        els
+00012b80: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+00012b90: 6620 7465 6d70 6572 6174 7572 6573 2069  f temperatures i
+00012ba0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00012bb0: 2020 2020 2020 2020 5f74 656d 7065 7261          _tempera
+00012bc0: 7475 7265 7320 3d20 6e70 2e61 7261 6e67  tures = np.arang
+00012bd0: 6528 302c 2031 3030 312c 2031 302c 2064  e(0, 1001, 10, d
+00012be0: 7479 7065 3d22 646f 7562 6c65 2229 0a20  type="double"). 
+00012bf0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00012c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012c10: 205f 7465 6d70 6572 6174 7572 6573 203d   _temperatures =
+00012c20: 2074 656d 7065 7261 7475 7265 730a 2020   temperatures.  
+00012c30: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00012c40: 7468 6572 6d61 6c5f 636f 6e64 7563 7469  thermal_conducti
+00012c50: 7669 7479 203d 2067 6574 5f74 6865 726d  vity = get_therm
+00012c60: 616c 5f63 6f6e 6475 6374 6976 6974 795f  al_conductivity_
+00012c70: 5254 4128 0a20 2020 2020 2020 2020 2020  RTA(.           
+00012c80: 2020 2020 2073 656c 662e 5f69 6e74 6572       self._inter
+00012c90: 6163 7469 6f6e 2c0a 2020 2020 2020 2020  action,.        
+00012ca0: 2020 2020 2020 2020 7465 6d70 6572 6174          temperat
+00012cb0: 7572 6573 3d5f 7465 6d70 6572 6174 7572  ures=_temperatur
+00012cc0: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+00012cd0: 2020 2020 7369 676d 6173 3d73 656c 662e      sigmas=self.
+00012ce0: 5f73 6967 6d61 732c 0a20 2020 2020 2020  _sigmas,.       
+00012cf0: 2020 2020 2020 2020 2073 6967 6d61 5f63           sigma_c
+00012d00: 7574 6f66 663d 7365 6c66 2e5f 7369 676d  utoff=self._sigm
+00012d10: 615f 6375 746f 6666 2c0a 2020 2020 2020  a_cutoff,.      
+00012d20: 2020 2020 2020 2020 2020 6973 5f69 736f            is_iso
+00012d30: 746f 7065 3d69 735f 6973 6f74 6f70 652c  tope=is_isotope,
+00012d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012d50: 206d 6173 735f 7661 7269 616e 6365 733d   mass_variances=
+00012d60: 6d61 7373 5f76 6172 6961 6e63 6573 2c0a  mass_variances,.
+00012d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d80: 6772 6964 5f70 6f69 6e74 733d 6772 6964  grid_points=grid
+00012d90: 5f70 6f69 6e74 732c 0a20 2020 2020 2020  _points,.       
+00012da0: 2020 2020 2020 2020 2062 6f75 6e64 6172           boundar
+00012db0: 795f 6d66 703d 626f 756e 6461 7279 5f6d  y_mfp=boundary_m
+00012dc0: 6670 2c0a 2020 2020 2020 2020 2020 2020  fp,.            
+00012dd0: 2020 2020 7573 655f 6176 655f 7070 3d75      use_ave_pp=u
+00012de0: 7365 5f61 7665 5f70 702c 0a20 2020 2020  se_ave_pp,.     
+00012df0: 2020 2020 2020 2020 2020 2069 735f 6b61             is_ka
+00012e00: 7070 615f 7374 6172 3d69 735f 6b61 7070  ppa_star=is_kapp
+00012e10: 615f 7374 6172 2c0a 2020 2020 2020 2020  a_star,.        
+00012e20: 2020 2020 2020 2020 6776 5f64 656c 7461          gv_delta
+00012e30: 5f71 3d67 765f 6465 6c74 615f 712c 0a20  _q=gv_delta_q,. 
+00012e40: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00012e50: 735f 6675 6c6c 5f70 703d 6973 5f66 756c  s_full_pp=is_ful
+00012e60: 6c5f 7070 2c0a 2020 2020 2020 2020 2020  l_pp,.          
+00012e70: 2020 2020 2020 6973 5f4e 5f55 3d69 735f        is_N_U=is_
+00012e80: 4e5f 552c 0a20 2020 2020 2020 2020 2020  N_U,.           
+00012e90: 2020 2020 2063 6f6e 6475 6374 6976 6974       conductivit
+00012ea0: 795f 7479 7065 3d63 6f6e 6475 6374 6976  y_type=conductiv
+00012eb0: 6974 795f 7479 7065 2c0a 2020 2020 2020  ity_type,.      
+00012ec0: 2020 2020 2020 2020 2020 7772 6974 655f            write_
+00012ed0: 6761 6d6d 613d 7772 6974 655f 6761 6d6d  gamma=write_gamm
+00012ee0: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
+00012ef0: 2020 2072 6561 645f 6761 6d6d 613d 7265     read_gamma=re
+00012f00: 6164 5f67 616d 6d61 2c0a 2020 2020 2020  ad_gamma,.      
+00012f10: 2020 2020 2020 2020 2020 7772 6974 655f            write_
+00012f20: 6b61 7070 613d 7772 6974 655f 6b61 7070  kappa=write_kapp
+00012f30: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
+00012f40: 2020 2077 7269 7465 5f70 703d 7772 6974     write_pp=writ
+00012f50: 655f 7070 2c0a 2020 2020 2020 2020 2020  e_pp,.          
+00012f60: 2020 2020 2020 7265 6164 5f70 703d 7265        read_pp=re
+00012f70: 6164 5f70 702c 0a20 2020 2020 2020 2020  ad_pp,.         
+00012f80: 2020 2020 2020 2077 7269 7465 5f67 616d         write_gam
+00012f90: 6d61 5f64 6574 6169 6c3d 7772 6974 655f  ma_detail=write_
+00012fa0: 6761 6d6d 615f 6465 7461 696c 2c0a 2020  gamma_detail,.  
+00012fb0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00012fc0: 6d70 7265 7373 696f 6e3d 636f 6d70 7265  mpression=compre
+00012fd0: 7373 696f 6e2c 0a20 2020 2020 2020 2020  ssion,.         
+00012fe0: 2020 2020 2020 2069 6e70 7574 5f66 696c         input_fil
+00012ff0: 656e 616d 653d 696e 7075 745f 6669 6c65  ename=input_file
+00013000: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+00013010: 2020 2020 2020 6f75 7470 7574 5f66 696c        output_fil
+00013020: 656e 616d 653d 6f75 7470 7574 5f66 696c  ename=output_fil
+00013030: 656e 616d 652c 0a20 2020 2020 2020 2020  ename,.         
+00013040: 2020 2020 2020 206c 6f67 5f6c 6576 656c         log_level
+00013050: 3d73 656c 662e 5f6c 6f67 5f6c 6576 656c  =self._log_level
+00013060: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00013070: 0a20 2020 2064 6566 2073 6176 6528 7365  .    def save(se
+00013080: 6c66 2c20 6669 6c65 6e61 6d65 3d22 7068  lf, filename="ph
+00013090: 6f6e 6f33 7079 5f70 6172 616d 732e 7961  ono3py_params.ya
+000130a0: 6d6c 222c 2073 6574 7469 6e67 733d 4e6f  ml", settings=No
+000130b0: 6e65 293a 0a20 2020 2020 2020 2022 2222  ne):.        """
+000130c0: 5361 7665 2070 6172 616d 6574 6572 7320  Save parameters 
+000130d0: 696e 2050 686f 6e6f 3370 7920 696e 7374  in Phono3py inst
+000130e0: 616e 7473 2069 6e74 6f20 6669 6c65 2e0a  ants into file..
+000130f0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00013100: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+00013110: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2066  ------.        f
+00013120: 696c 656e 616d 653a 2073 7472 2c20 6f70  ilename: str, op
+00013130: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
+00013140: 2020 2046 696c 6520 6e61 6d65 2e20 4465     File name. De
+00013150: 6661 756c 7420 6973 2022 7068 6f6e 6f33  fault is "phono3
+00013160: 7079 5f70 6172 616d 732e 7961 6d6c 220a  py_params.yaml".
+00013170: 2020 2020 2020 2020 7365 7474 696e 6773          settings
+00013180: 3a20 6469 6374 2c20 6f70 7469 6f6e 616c  : dict, optional
+00013190: 0a20 2020 2020 2020 2020 2020 2049 7420  .            It 
+000131a0: 6973 2064 6573 6372 6962 6564 2077 6869  is described whi
+000131b0: 6368 2070 6172 616d 6574 6572 7320 6172  ch parameters ar
+000131c0: 6520 7772 6974 7465 6e20 6f75 742e 204f  e written out. O
+000131d0: 6e6c 790a 2020 2020 2020 2020 2020 2020  nly.            
+000131e0: 7468 6520 7365 7474 696e 6773 2065 7870  the settings exp
+000131f0: 6563 7465 6420 746f 2062 6520 7570 6461  ected to be upda
+00013200: 7465 6420 6672 6f6d 2074 6865 2066 6f6c  ted from the fol
+00013210: 6c6f 7769 6e67 0a20 2020 2020 2020 2020  lowing.         
+00013220: 2020 2064 6566 6175 6c74 2073 6574 7469     default setti
+00013230: 6e67 7320 6172 6520 6e65 6564 6564 2074  ngs are needed t
+00013240: 6f20 6265 2073 6574 2069 6e20 7468 6520  o be set in the 
+00013250: 6469 6374 696f 6e61 7279 2e0a 2020 2020  dictionary..    
+00013260: 2020 2020 2020 2020 5468 6520 706f 7373          The poss
+00013270: 6962 6c65 2070 6172 616d 6574 6572 7320  ible parameters 
+00013280: 616e 6420 7468 6569 7220 6465 6661 756c  and their defaul
+00013290: 7420 7365 7474 696e 6773 2061 7265 3a0a  t settings are:.
+000132a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132b0: 7b27 666f 7263 655f 7365 7473 273a 2046  {'force_sets': F
+000132c0: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+000132d0: 2020 2020 2020 2027 6469 7370 6c61 6365         'displace
+000132e0: 6d65 6e74 7327 3a20 5472 7565 2c0a 2020  ments': True,.  
+000132f0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00013300: 666f 7263 655f 636f 6e73 7461 6e74 7327  force_constants'
+00013310: 3a20 4661 6c73 652c 0a20 2020 2020 2020  : False,.       
+00013320: 2020 2020 2020 2020 2020 2762 6f72 6e5f            'born_
+00013330: 6566 6665 6374 6976 655f 6368 6172 6765  effective_charge
+00013340: 273a 2054 7275 652c 0a20 2020 2020 2020  ': True,.       
+00013350: 2020 2020 2020 2020 2020 2764 6965 6c65            'diele
+00013360: 6374 7269 635f 636f 6e73 7461 6e74 273a  ctric_constant':
+00013370: 2054 7275 657d 0a0a 2020 2020 2020 2020   True}..        
+00013380: 2222 220a 2020 2020 2020 2020 7068 3370  """.        ph3p
+00013390: 795f 7961 6d6c 203d 2050 686f 6e6f 3370  y_yaml = Phono3p
+000133a0: 7959 616d 6c28 7365 7474 696e 6773 3d73  yYaml(settings=s
+000133b0: 6574 7469 6e67 7329 0a20 2020 2020 2020  ettings).       
+000133c0: 2070 6833 7079 5f79 616d 6c2e 7365 745f   ph3py_yaml.set_
+000133d0: 7068 6f6e 6f6e 5f69 6e66 6f28 7365 6c66  phonon_info(self
+000133e0: 290a 2020 2020 2020 2020 7769 7468 206f  ).        with o
+000133f0: 7065 6e28 6669 6c65 6e61 6d65 2c20 2277  pen(filename, "w
+00013400: 2229 2061 7320 773a 0a20 2020 2020 2020  ") as w:.       
+00013410: 2020 2020 2077 2e77 7269 7465 2873 7472       w.write(str
+00013420: 2870 6833 7079 5f79 616d 6c29 290a 0a20  (ph3py_yaml)).. 
+00013430: 2020 2023 2323 2323 2323 2323 2323 2323     #############
+00013440: 2323 2323 2323 0a20 2020 2023 2070 7269  ######.    # pri
+00013450: 7661 7465 206d 6574 686f 6473 2023 0a20  vate methods #. 
+00013460: 2020 2023 2323 2323 2323 2323 2323 2323     #############
+00013470: 2323 2323 2323 0a20 2020 2064 6566 205f  ######.    def _
+00013480: 7365 6172 6368 5f73 796d 6d65 7472 7928  search_symmetry(
+00013490: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+000134a0: 656c 662e 5f73 796d 6d65 7472 7920 3d20  elf._symmetry = 
+000134b0: 5379 6d6d 6574 7279 2873 656c 662e 5f73  Symmetry(self._s
+000134c0: 7570 6572 6365 6c6c 2c20 7365 6c66 2e5f  upercell, self._
+000134d0: 7379 6d70 7265 632c 2073 656c 662e 5f69  symprec, self._i
+000134e0: 735f 7379 6d6d 6574 7279 290a 0a20 2020  s_symmetry)..   
+000134f0: 2064 6566 205f 7365 6172 6368 5f70 7269   def _search_pri
+00013500: 6d69 7469 7665 5f73 796d 6d65 7472 7928  mitive_symmetry(
+00013510: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+00013520: 656c 662e 5f70 7269 6d69 7469 7665 5f73  elf._primitive_s
+00013530: 796d 6d65 7472 7920 3d20 5379 6d6d 6574  ymmetry = Symmet
+00013540: 7279 280a 2020 2020 2020 2020 2020 2020  ry(.            
+00013550: 7365 6c66 2e5f 7072 696d 6974 6976 652c  self._primitive,
+00013560: 2073 656c 662e 5f73 796d 7072 6563 2c20   self._symprec, 
+00013570: 7365 6c66 2e5f 6973 5f73 796d 6d65 7472  self._is_symmetr
+00013580: 790a 2020 2020 2020 2020 290a 2020 2020  y.        ).    
+00013590: 2020 2020 6966 206c 656e 2873 656c 662e      if len(self.
+000135a0: 5f73 796d 6d65 7472 792e 706f 696e 7467  _symmetry.pointg
+000135b0: 726f 7570 5f6f 7065 7261 7469 6f6e 7329  roup_operations)
+000135c0: 2021 3d20 6c65 6e28 0a20 2020 2020 2020   != len(.       
+000135d0: 2020 2020 2073 656c 662e 5f70 7269 6d69       self._primi
+000135e0: 7469 7665 5f73 796d 6d65 7472 792e 706f  tive_symmetry.po
+000135f0: 696e 7467 726f 7570 5f6f 7065 7261 7469  intgroup_operati
+00013600: 6f6e 730a 2020 2020 2020 2020 293a 2020  ons.        ):  
+00013610: 2320 6e6f 7161 2045 3132 390a 2020 2020  # noqa E129.    
+00013620: 2020 2020 2020 2020 7072 696e 7428 0a20          print(. 
+00013630: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00013640: 5761 726e 696e 673a 2070 6f69 6e74 2067  Warning: point g
+00013650: 726f 7570 2073 796d 6d65 7472 6965 7320  roup symmetries 
+00013660: 6f66 2073 7570 6572 6365 6c6c 2061 6e64  of supercell and
+00013670: 2070 7269 6d69 7469 7665 220a 2020 2020   primitive".    
+00013680: 2020 2020 2020 2020 2020 2020 2263 656c              "cel
+00013690: 6c20 6172 6520 6469 6666 6572 656e 742e  l are different.
+000136a0: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
+000136b0: 0a20 2020 2064 6566 205f 7365 6172 6368  .    def _search
+000136c0: 5f70 686f 6e6f 6e5f 7375 7065 7263 656c  _phonon_supercel
+000136d0: 6c5f 7379 6d6d 6574 7279 2873 656c 6629  l_symmetry(self)
+000136e0: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
+000136f0: 662e 5f70 686f 6e6f 6e5f 7375 7065 7263  f._phonon_superc
+00013700: 656c 6c5f 6d61 7472 6978 2069 7320 4e6f  ell_matrix is No
+00013710: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00013720: 7365 6c66 2e5f 7068 6f6e 6f6e 5f73 7570  self._phonon_sup
+00013730: 6572 6365 6c6c 5f73 796d 6d65 7472 7920  ercell_symmetry 
+00013740: 3d20 7365 6c66 2e5f 7379 6d6d 6574 7279  = self._symmetry
+00013750: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00013760: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013770: 5f70 686f 6e6f 6e5f 7375 7065 7263 656c  _phonon_supercel
+00013780: 6c5f 7379 6d6d 6574 7279 203d 2053 796d  l_symmetry = Sym
+00013790: 6d65 7472 7928 0a20 2020 2020 2020 2020  metry(.         
+000137a0: 2020 2020 2020 2073 656c 662e 5f70 686f         self._pho
+000137b0: 6e6f 6e5f 7375 7065 7263 656c 6c2c 2073  non_supercell, s
+000137c0: 656c 662e 5f73 796d 7072 6563 2c20 7365  elf._symprec, se
+000137d0: 6c66 2e5f 6973 5f73 796d 6d65 7472 790a  lf._is_symmetry.
+000137e0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+000137f0: 2020 2064 6566 205f 6275 696c 645f 7375     def _build_su
+00013800: 7065 7263 656c 6c28 7365 6c66 293a 0a20  percell(self):. 
+00013810: 2020 2020 2020 2073 656c 662e 5f73 7570         self._sup
+00013820: 6572 6365 6c6c 203d 2067 6574 5f73 7570  ercell = get_sup
+00013830: 6572 6365 6c6c 280a 2020 2020 2020 2020  ercell(.        
+00013840: 2020 2020 7365 6c66 2e5f 756e 6974 6365      self._unitce
+00013850: 6c6c 2c20 7365 6c66 2e5f 7375 7065 7263  ll, self._superc
+00013860: 656c 6c5f 6d61 7472 6978 2c20 7365 6c66  ell_matrix, self
+00013870: 2e5f 7379 6d70 7265 630a 2020 2020 2020  ._symprec.      
+00013880: 2020 290a 0a20 2020 2064 6566 205f 6275    )..    def _bu
+00013890: 696c 645f 7072 696d 6974 6976 655f 6365  ild_primitive_ce
+000138a0: 6c6c 2873 656c 6629 3a0a 2020 2020 2020  ll(self):.      
+000138b0: 2020 2222 2243 7265 6174 6520 7072 696d    """Create prim
+000138c0: 6974 6976 6520 6365 6c6c 2e0a 0a20 2020  itive cell...   
+000138d0: 2020 2020 2070 7269 6d69 7469 7665 5f6d       primitive_m
+000138e0: 6174 7269 783a 0a20 2020 2020 2020 2020  atrix:.         
+000138f0: 2052 656c 6174 6976 6520 6178 6573 206f   Relative axes o
+00013900: 6620 7072 696d 6974 6976 6520 6365 6c6c  f primitive cell
+00013910: 2074 6f20 7468 6520 696e 7075 7420 756e   to the input un
+00013920: 6974 2063 656c 6c2e 0a20 2020 2020 2020  it cell..       
+00013930: 2020 2052 656c 6174 6976 6520 6178 6573     Relative axes
+00013940: 2074 6f20 7468 6520 7375 7065 7263 656c   to the supercel
+00013950: 6c20 6973 2063 616c 6375 6c61 7465 6420  l is calculated 
+00013960: 6279 3a0a 2020 2020 2020 2020 2020 2020  by:.            
+00013970: 2073 7570 6572 6365 6c6c 5f6d 6174 7269   supercell_matri
+00013980: 785e 2d31 202a 2070 7269 6d69 7469 7665  x^-1 * primitive
+00013990: 5f6d 6174 7269 780a 2020 2020 2020 2020  _matrix.        
+000139a0: 2020 5468 6572 6566 6f72 6520 7072 696d    Therefore prim
+000139b0: 6974 6976 6520 6365 6c6c 206c 6174 7469  itive cell latti
+000139c0: 6365 2069 7320 6669 6e61 6c6c 7920 6361  ce is finally ca
+000139d0: 6c63 756c 6174 6564 2062 793a 0a20 2020  lculated by:.   
+000139e0: 2020 2020 2020 2020 2020 2873 7570 6572            (super
+000139f0: 6365 6c6c 5f6c 6174 7469 6365 202a 2028  cell_lattice * (
+00013a00: 7375 7065 7263 656c 6c5f 6d61 7472 6978  supercell_matrix
+00013a10: 295e 2d31 202a 2070 7269 6d69 7469 7665  )^-1 * primitive
+00013a20: 5f6d 6174 7269 7829 5e54 0a0a 2020 2020  _matrix)^T..    
+00013a30: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00013a40: 7365 6c66 2e5f 7072 696d 6974 6976 6520  self._primitive 
+00013a50: 3d20 7365 6c66 2e5f 6765 745f 7072 696d  = self._get_prim
+00013a60: 6974 6976 655f 6365 6c6c 280a 2020 2020  itive_cell(.    
+00013a70: 2020 2020 2020 2020 7365 6c66 2e5f 7375          self._su
+00013a80: 7065 7263 656c 6c2c 2073 656c 662e 5f73  percell, self._s
+00013a90: 7570 6572 6365 6c6c 5f6d 6174 7269 782c  upercell_matrix,
+00013aa0: 2073 656c 662e 5f70 7269 6d69 7469 7665   self._primitive
+00013ab0: 5f6d 6174 7269 780a 2020 2020 2020 2020  _matrix.        
+00013ac0: 290a 0a20 2020 2064 6566 205f 6275 696c  )..    def _buil
+00013ad0: 645f 7068 6f6e 6f6e 5f73 7570 6572 6365  d_phonon_superce
+00013ae0: 6c6c 2873 656c 6629 3a0a 2020 2020 2020  ll(self):.      
+00013af0: 2020 2222 2243 7265 6174 6520 7068 6f6e    """Create phon
+00013b00: 6f6e 2073 7570 6572 6365 6c6c 2066 6f72  on supercell for
+00013b10: 2066 6332 2e0a 0a20 2020 2020 2020 2070   fc2...        p
+00013b20: 686f 6e6f 6e5f 7375 7065 7263 656c 6c3a  honon_supercell:
+00013b30: 0a20 2020 2020 2020 2020 2054 6869 7320  .          This 
+00013b40: 7375 7065 7263 656c 6c20 6973 2075 7365  supercell is use
+00013b50: 6420 666f 7220 6861 726d 6f6e 6963 2070  d for harmonic p
+00013b60: 686f 6e6f 6e73 2028 6672 6571 7565 6e63  honons (frequenc
+00013b70: 6965 732c 0a20 2020 2020 2020 2020 2065  ies,.          e
+00013b80: 6967 656e 7665 6374 6f72 732c 2067 726f  igenvectors, gro
+00013b90: 7570 2076 656c 6f63 6974 6965 732c 202e  up velocities, .
+00013ba0: 2e2e 290a 2020 2020 2020 2020 7068 6f6e  ..).        phon
+00013bb0: 6f6e 5f73 7570 6572 6365 6c6c 5f6d 6174  on_supercell_mat
+00013bc0: 7269 783a 0a20 2020 2020 2020 2020 2044  rix:.          D
+00013bd0: 6966 6665 7265 6e74 2073 7570 6572 6365  ifferent superce
+00013be0: 6c6c 2073 697a 6520 6361 6e20 6265 2073  ll size can be s
+00013bf0: 7065 6369 6669 6564 2e0a 0a20 2020 2020  pecified...     
+00013c00: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00013c10: 6620 7365 6c66 2e5f 7068 6f6e 6f6e 5f73  f self._phonon_s
+00013c20: 7570 6572 6365 6c6c 5f6d 6174 7269 7820  upercell_matrix 
+00013c30: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00013c40: 2020 2020 2073 656c 662e 5f70 686f 6e6f       self._phono
+00013c50: 6e5f 7375 7065 7263 656c 6c20 3d20 7365  n_supercell = se
+00013c60: 6c66 2e5f 7375 7065 7263 656c 6c0a 2020  lf._supercell.  
+00013c70: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00013c80: 2020 2020 2020 2020 7365 6c66 2e5f 7068          self._ph
+00013c90: 6f6e 6f6e 5f73 7570 6572 6365 6c6c 203d  onon_supercell =
+00013ca0: 2067 6574 5f73 7570 6572 6365 6c6c 280a   get_supercell(.
+00013cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013cc0: 7365 6c66 2e5f 756e 6974 6365 6c6c 2c20  self._unitcell, 
+00013cd0: 7365 6c66 2e5f 7068 6f6e 6f6e 5f73 7570  self._phonon_sup
+00013ce0: 6572 6365 6c6c 5f6d 6174 7269 782c 2073  ercell_matrix, s
+00013cf0: 656c 662e 5f73 796d 7072 6563 0a20 2020  elf._symprec.   
+00013d00: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00013d10: 6465 6620 5f62 7569 6c64 5f70 686f 6e6f  def _build_phono
+00013d20: 6e5f 7072 696d 6974 6976 655f 6365 6c6c  n_primitive_cell
+00013d30: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00013d40: 6966 2073 656c 662e 5f70 686f 6e6f 6e5f  if self._phonon_
+00013d50: 7375 7065 7263 656c 6c5f 6d61 7472 6978  supercell_matrix
+00013d60: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00013d70: 2020 2020 2020 7365 6c66 2e5f 7068 6f6e        self._phon
+00013d80: 6f6e 5f70 7269 6d69 7469 7665 203d 2073  on_primitive = s
+00013d90: 656c 662e 5f70 7269 6d69 7469 7665 0a20  elf._primitive. 
+00013da0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00013db0: 2020 2020 2020 2020 2073 656c 662e 5f70           self._p
+00013dc0: 686f 6e6f 6e5f 7072 696d 6974 6976 6520  honon_primitive 
+00013dd0: 3d20 7365 6c66 2e5f 6765 745f 7072 696d  = self._get_prim
+00013de0: 6974 6976 655f 6365 6c6c 280a 2020 2020  itive_cell(.    
+00013df0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013e00: 2e5f 7068 6f6e 6f6e 5f73 7570 6572 6365  ._phonon_superce
+00013e10: 6c6c 2c0a 2020 2020 2020 2020 2020 2020  ll,.            
+00013e20: 2020 2020 7365 6c66 2e5f 7068 6f6e 6f6e      self._phonon
+00013e30: 5f73 7570 6572 6365 6c6c 5f6d 6174 7269  _supercell_matri
+00013e40: 782c 0a20 2020 2020 2020 2020 2020 2020  x,.             
+00013e50: 2020 2073 656c 662e 5f70 7269 6d69 7469     self._primiti
+00013e60: 7665 5f6d 6174 7269 782c 0a20 2020 2020  ve_matrix,.     
+00013e70: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00013e80: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
+00013e90: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00013ea0: 7072 696d 6974 6976 6520 6973 206e 6f74  primitive is not
+00013eb0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+00013ec0: 2020 2020 2020 616e 6420 2873 656c 662e        and (self.
+00013ed0: 5f70 7269 6d69 7469 7665 2e6e 756d 6265  _primitive.numbe
+00013ee0: 7273 2021 3d20 7365 6c66 2e5f 7068 6f6e  rs != self._phon
+00013ef0: 6f6e 5f70 7269 6d69 7469 7665 2e6e 756d  on_primitive.num
+00013f00: 6265 7273 292e 616e 7928 290a 2020 2020  bers).any().    
+00013f10: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
+00013f20: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00013f30: 2822 2050 7269 6d69 7469 7665 2063 656c  (" Primitive cel
+00013f40: 6c73 2066 6f72 2066 6332 2061 6e64 2066  ls for fc2 and f
+00013f50: 6333 2063 616e 2062 6520 6469 6666 6572  c3 can be differ
+00013f60: 656e 742e 2229 0a20 2020 2020 2020 2020  ent.").         
+00013f70: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
+00013f80: 7469 6d65 4572 726f 720a 0a20 2020 2064  timeError..    d
+00013f90: 6566 205f 6275 696c 645f 7068 6f6e 6f6e  ef _build_phonon
+00013fa0: 5f73 7570 6572 6365 6c6c 735f 7769 7468  _supercells_with
+00013fb0: 5f64 6973 706c 6163 656d 656e 7473 280a  _displacements(.
+00013fc0: 2020 2020 2020 2020 7365 6c66 2c20 7375          self, su
+00013fd0: 7065 7263 656c 6c3a 2050 686f 6e6f 7079  percell: Phonopy
+00013fe0: 4174 6f6d 732c 2064 6973 706c 6163 656d  Atoms, displacem
+00013ff0: 656e 745f 6461 7461 7365 740a 2020 2020  ent_dataset.    
+00014000: 293a 0a20 2020 2020 2020 2073 7570 6572  ):.        super
+00014010: 6365 6c6c 7320 3d20 5b5d 0a20 2020 2020  cells = [].     
+00014020: 2020 206d 6167 6d6f 6d73 203d 2073 7570     magmoms = sup
+00014030: 6572 6365 6c6c 2e6d 6167 6e65 7469 635f  ercell.magnetic_
+00014040: 6d6f 6d65 6e74 730a 2020 2020 2020 2020  moments.        
+00014050: 6d61 7373 6573 203d 2073 7570 6572 6365  masses = superce
+00014060: 6c6c 2e6d 6173 7365 730a 2020 2020 2020  ll.masses.      
+00014070: 2020 6e75 6d62 6572 7320 3d20 7375 7065    numbers = supe
+00014080: 7263 656c 6c2e 6e75 6d62 6572 730a 2020  rcell.numbers.  
+00014090: 2020 2020 2020 6c61 7474 6963 6520 3d20        lattice = 
+000140a0: 7375 7065 7263 656c 6c2e 6365 6c6c 0a0a  supercell.cell..
+000140b0: 2020 2020 2020 2020 666f 7220 6469 7370          for disp
+000140c0: 3120 696e 2064 6973 706c 6163 656d 656e  1 in displacemen
+000140d0: 745f 6461 7461 7365 745b 2266 6972 7374  t_dataset["first
+000140e0: 5f61 746f 6d73 225d 3a0a 2020 2020 2020  _atoms"]:.      
+000140f0: 2020 2020 2020 6469 7370 5f63 6172 7431        disp_cart1
+00014100: 203d 2064 6973 7031 5b22 6469 7370 6c61   = disp1["displa
+00014110: 6365 6d65 6e74 225d 0a20 2020 2020 2020  cement"].       
+00014120: 2020 2020 2070 6f73 6974 696f 6e73 203d       positions =
+00014130: 2073 7570 6572 6365 6c6c 2e70 6f73 6974   supercell.posit
+00014140: 696f 6e73 0a20 2020 2020 2020 2020 2020  ions.           
+00014150: 2070 6f73 6974 696f 6e73 5b64 6973 7031   positions[disp1
+00014160: 5b22 6e75 6d62 6572 225d 5d20 2b3d 2064  ["number"]] += d
+00014170: 6973 705f 6361 7274 310a 2020 2020 2020  isp_cart1.      
+00014180: 2020 2020 2020 7375 7065 7263 656c 6c73        supercells
+00014190: 2e61 7070 656e 6428 0a20 2020 2020 2020  .append(.       
+000141a0: 2020 2020 2020 2020 2050 686f 6e6f 7079           Phonopy
+000141b0: 4174 6f6d 7328 0a20 2020 2020 2020 2020  Atoms(.         
+000141c0: 2020 2020 2020 2020 2020 206e 756d 6265             numbe
+000141d0: 7273 3d6e 756d 6265 7273 2c0a 2020 2020  rs=numbers,.    
+000141e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000141f0: 6d61 7373 6573 3d6d 6173 7365 732c 0a20  masses=masses,. 
+00014200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014210: 2020 206d 6167 6e65 7469 635f 6d6f 6d65     magnetic_mome
+00014220: 6e74 733d 6d61 676d 6f6d 732c 0a20 2020  nts=magmoms,.   
+00014230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014240: 2070 6f73 6974 696f 6e73 3d70 6f73 6974   positions=posit
+00014250: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
+00014260: 2020 2020 2020 2020 2020 6365 6c6c 3d6c            cell=l
+00014270: 6174 7469 6365 2c0a 2020 2020 2020 2020  attice,.        
+00014280: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00014290: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+000142a0: 2072 6574 7572 6e20 7375 7065 7263 656c   return supercel
+000142b0: 6c73 0a0a 2020 2020 6465 6620 5f62 7569  ls..    def _bui
+000142c0: 6c64 5f73 7570 6572 6365 6c6c 735f 7769  ld_supercells_wi
+000142d0: 7468 5f64 6973 706c 6163 656d 656e 7473  th_displacements
+000142e0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000142f0: 7375 7065 7263 656c 6c73 203d 205b 5d0a  supercells = [].
+00014300: 2020 2020 2020 2020 6d61 676d 6f6d 7320          magmoms 
+00014310: 3d20 7365 6c66 2e5f 7375 7065 7263 656c  = self._supercel
+00014320: 6c2e 6d61 676e 6574 6963 5f6d 6f6d 656e  l.magnetic_momen
+00014330: 7473 0a20 2020 2020 2020 206d 6173 7365  ts.        masse
+00014340: 7320 3d20 7365 6c66 2e5f 7375 7065 7263  s = self._superc
+00014350: 656c 6c2e 6d61 7373 6573 0a20 2020 2020  ell.masses.     
+00014360: 2020 206e 756d 6265 7273 203d 2073 656c     numbers = sel
+00014370: 662e 5f73 7570 6572 6365 6c6c 2e6e 756d  f._supercell.num
+00014380: 6265 7273 0a20 2020 2020 2020 206c 6174  bers.        lat
+00014390: 7469 6365 203d 2073 656c 662e 5f73 7570  tice = self._sup
+000143a0: 6572 6365 6c6c 2e63 656c 6c0a 0a20 2020  ercell.cell..   
+000143b0: 2020 2020 2073 7570 6572 6365 6c6c 7320       supercells 
+000143c0: 3d20 7365 6c66 2e5f 6275 696c 645f 7068  = self._build_ph
+000143d0: 6f6e 6f6e 5f73 7570 6572 6365 6c6c 735f  onon_supercells_
+000143e0: 7769 7468 5f64 6973 706c 6163 656d 656e  with_displacemen
+000143f0: 7473 280a 2020 2020 2020 2020 2020 2020  ts(.            
+00014400: 7365 6c66 2e5f 7375 7065 7263 656c 6c2c  self._supercell,
+00014410: 2073 656c 662e 5f64 6174 6173 6574 0a20   self._dataset. 
+00014420: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00014430: 2020 666f 7220 6469 7370 3120 696e 2073    for disp1 in s
+00014440: 656c 662e 5f64 6174 6173 6574 5b22 6669  elf._dataset["fi
+00014450: 7273 745f 6174 6f6d 7322 5d3a 0a20 2020  rst_atoms"]:.   
+00014460: 2020 2020 2020 2020 2064 6973 705f 6361           disp_ca
+00014470: 7274 3120 3d20 6469 7370 315b 2264 6973  rt1 = disp1["dis
+00014480: 706c 6163 656d 656e 7422 5d0a 2020 2020  placement"].    
+00014490: 2020 2020 2020 2020 666f 7220 6469 7370          for disp
+000144a0: 3220 696e 2064 6973 7031 5b22 7365 636f  2 in disp1["seco
+000144b0: 6e64 5f61 746f 6d73 225d 3a0a 2020 2020  nd_atoms"]:.    
+000144c0: 2020 2020 2020 2020 2020 2020 6966 2022              if "
+000144d0: 696e 636c 7564 6564 2220 696e 2064 6973  included" in dis
+000144e0: 7032 3a0a 2020 2020 2020 2020 2020 2020  p2:.            
+000144f0: 2020 2020 2020 2020 696e 636c 7564 6564          included
+00014500: 203d 2064 6973 7032 5b22 696e 636c 7564   = disp2["includ
+00014510: 6564 225d 0a20 2020 2020 2020 2020 2020  ed"].           
+00014520: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00014530: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00014540: 6e63 6c75 6465 6420 3d20 5472 7565 0a20  ncluded = True. 
+00014550: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00014560: 6620 696e 636c 7564 6564 3a0a 2020 2020  f included:.    
+00014570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014580: 706f 7369 7469 6f6e 7320 3d20 7365 6c66  positions = self
+00014590: 2e5f 7375 7065 7263 656c 6c2e 706f 7369  ._supercell.posi
+000145a0: 7469 6f6e 730a 2020 2020 2020 2020 2020  tions.          
+000145b0: 2020 2020 2020 2020 2020 706f 7369 7469            positi
+000145c0: 6f6e 735b 6469 7370 315b 226e 756d 6265  ons[disp1["numbe
+000145d0: 7222 5d5d 202b 3d20 6469 7370 5f63 6172  r"]] += disp_car
+000145e0: 7431 0a20 2020 2020 2020 2020 2020 2020  t1.             
+000145f0: 2020 2020 2020 2070 6f73 6974 696f 6e73         positions
+00014600: 5b64 6973 7032 5b22 6e75 6d62 6572 225d  [disp2["number"]
+00014610: 5d20 2b3d 2064 6973 7032 5b22 6469 7370  ] += disp2["disp
+00014620: 6c61 6365 6d65 6e74 225d 0a20 2020 2020  lacement"].     
+00014630: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014640: 7570 6572 6365 6c6c 732e 6170 7065 6e64  upercells.append
+00014650: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00014660: 2020 2020 2020 2020 2020 5068 6f6e 6f70            Phonop
+00014670: 7941 746f 6d73 280a 2020 2020 2020 2020  yAtoms(.        
+00014680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014690: 2020 2020 6e75 6d62 6572 733d 6e75 6d62      numbers=numb
+000146a0: 6572 732c 0a20 2020 2020 2020 2020 2020  ers,.           
+000146b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000146c0: 206d 6173 7365 733d 6d61 7373 6573 2c0a   masses=masses,.
+000146d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000146e0: 2020 2020 2020 2020 2020 2020 6d61 676e              magn
+000146f0: 6574 6963 5f6d 6f6d 656e 7473 3d6d 6167  etic_moments=mag
+00014700: 6d6f 6d73 2c0a 2020 2020 2020 2020 2020  moms,.          
+00014710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014720: 2020 706f 7369 7469 6f6e 733d 706f 7369    positions=posi
+00014730: 7469 6f6e 732c 0a20 2020 2020 2020 2020  tions,.         
+00014740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014750: 2020 2063 656c 6c3d 6c61 7474 6963 652c     cell=lattice,
+00014760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014770: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00014780: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00014790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000147a0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000147b0: 2020 2020 2020 2020 2020 2073 7570 6572             super
+000147c0: 6365 6c6c 732e 6170 7065 6e64 284e 6f6e  cells.append(Non
+000147d0: 6529 0a0a 2020 2020 2020 2020 7365 6c66  e)..        self
+000147e0: 2e5f 7375 7065 7263 656c 6c73 5f77 6974  ._supercells_wit
+000147f0: 685f 6469 7370 6c61 6365 6d65 6e74 7320  h_displacements 
+00014800: 3d20 7375 7065 7263 656c 6c73 0a0a 2020  = supercells..  
+00014810: 2020 6465 6620 5f67 6574 5f70 7269 6d69    def _get_primi
+00014820: 7469 7665 5f63 656c 6c28 7365 6c66 2c20  tive_cell(self, 
+00014830: 7375 7065 7263 656c 6c2c 2073 7570 6572  supercell, super
+00014840: 6365 6c6c 5f6d 6174 7269 782c 2070 7269  cell_matrix, pri
+00014850: 6d69 7469 7665 5f6d 6174 7269 7829 3a0a  mitive_matrix):.
+00014860: 2020 2020 2020 2020 696e 765f 7375 7065          inv_supe
+00014870: 7263 656c 6c5f 6d61 7472 6978 203d 206e  rcell_matrix = n
+00014880: 702e 6c69 6e61 6c67 2e69 6e76 2873 7570  p.linalg.inv(sup
+00014890: 6572 6365 6c6c 5f6d 6174 7269 7829 0a20  ercell_matrix). 
+000148a0: 2020 2020 2020 2069 6620 7072 696d 6974         if primit
+000148b0: 6976 655f 6d61 7472 6978 2069 7320 4e6f  ive_matrix is No
+000148c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000148d0: 745f 6d61 7420 3d20 696e 765f 7375 7065  t_mat = inv_supe
+000148e0: 7263 656c 6c5f 6d61 7472 6978 0a20 2020  rcell_matrix.   
+000148f0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00014900: 2020 2020 2020 2074 5f6d 6174 203d 206e         t_mat = n
+00014910: 702e 646f 7428 696e 765f 7375 7065 7263  p.dot(inv_superc
+00014920: 656c 6c5f 6d61 7472 6978 2c20 7072 696d  ell_matrix, prim
+00014930: 6974 6976 655f 6d61 7472 6978 290a 0a20  itive_matrix).. 
+00014940: 2020 2020 2020 2072 6574 7572 6e20 6765         return ge
+00014950: 745f 7072 696d 6974 6976 6528 7375 7065  t_primitive(supe
+00014960: 7263 656c 6c2c 2074 5f6d 6174 2c20 7365  rcell, t_mat, se
+00014970: 6c66 2e5f 7379 6d70 7265 632c 2073 746f  lf._symprec, sto
+00014980: 7265 5f64 656e 7365 5f73 7665 6373 3d54  re_dense_svecs=T
+00014990: 7275 6529 0a0a 2020 2020 6465 6620 5f64  rue)..    def _d
+000149a0: 6574 6572 6d69 6e65 5f70 7269 6d69 7469  etermine_primiti
+000149b0: 7665 5f6d 6174 7269 7828 7365 6c66 2c20  ve_matrix(self, 
+000149c0: 7072 696d 6974 6976 655f 6d61 7472 6978  primitive_matrix
+000149d0: 293a 0a20 2020 2020 2020 2070 6d61 7420  ):.        pmat 
+000149e0: 3d20 6765 745f 7072 696d 6974 6976 655f  = get_primitive_
+000149f0: 6d61 7472 6978 2870 7269 6d69 7469 7665  matrix(primitive
+00014a00: 5f6d 6174 7269 782c 2073 796d 7072 6563  _matrix, symprec
+00014a10: 3d73 656c 662e 5f73 796d 7072 6563 290a  =self._symprec).
+00014a20: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00014a30: 7461 6e63 6528 706d 6174 2c20 7374 7229  tance(pmat, str)
+00014a40: 2061 6e64 2070 6d61 7420 3d3d 2022 6175   and pmat == "au
+00014a50: 746f 223a 0a20 2020 2020 2020 2020 2020  to":.           
+00014a60: 2072 6574 7572 6e20 6775 6573 735f 7072   return guess_pr
+00014a70: 696d 6974 6976 655f 6d61 7472 6978 2873  imitive_matrix(s
+00014a80: 656c 662e 5f75 6e69 7463 656c 6c2c 2073  elf._unitcell, s
+00014a90: 796d 7072 6563 3d73 656c 662e 5f73 796d  ymprec=self._sym
+00014aa0: 7072 6563 290a 2020 2020 2020 2020 656c  prec).        el
+00014ab0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00014ac0: 7265 7475 726e 2070 6d61 740a 0a20 2020  return pmat..   
+00014ad0: 2064 6566 205f 7365 745f 6d65 7368 5f6e   def _set_mesh_n
+00014ae0: 756d 6265 7273 280a 2020 2020 2020 2020  umbers(.        
+00014af0: 7365 6c66 2c0a 2020 2020 2020 2020 6d65  self,.        me
+00014b00: 7368 3a20 556e 696f 6e5b 696e 742c 2066  sh: Union[int, f
+00014b10: 6c6f 6174 2c20 5365 7175 656e 6365 2c20  loat, Sequence, 
+00014b20: 6e70 2e6e 6461 7272 6179 5d2c 0a20 2020  np.ndarray],.   
+00014b30: 2029 3a0a 2020 2020 2020 2020 2320 696e   ):.        # in
+00014b40: 6974 6961 6c69 7a61 7469 6f6e 2072 656c  itialization rel
+00014b50: 6174 6564 2074 6f20 6d65 7368 0a20 2020  ated to mesh.   
+00014b60: 2020 2020 2073 656c 662e 5f69 6e74 6572       self._inter
+00014b70: 6163 7469 6f6e 203d 204e 6f6e 650a 0a20  action = None.. 
+00014b80: 2020 2020 2020 2073 656c 662e 5f62 7a5f         self._bz_
+00014b90: 6772 6964 203d 2042 5a47 7269 6428 0a20  grid = BZGrid(. 
+00014ba0: 2020 2020 2020 2020 2020 206d 6573 682c             mesh,
+00014bb0: 0a20 2020 2020 2020 2020 2020 206c 6174  .            lat
+00014bc0: 7469 6365 3d73 656c 662e 5f70 7269 6d69  tice=self._primi
+00014bd0: 7469 7665 2e63 656c 6c2c 0a20 2020 2020  tive.cell,.     
+00014be0: 2020 2020 2020 2073 796d 6d65 7472 795f         symmetry_
+00014bf0: 6461 7461 7365 743d 7365 6c66 2e5f 7072  dataset=self._pr
+00014c00: 696d 6974 6976 655f 7379 6d6d 6574 7279  imitive_symmetry
+00014c10: 2e64 6174 6173 6574 2c0a 2020 2020 2020  .dataset,.      
+00014c20: 2020 2020 2020 6973 5f74 696d 655f 7265        is_time_re
+00014c30: 7665 7273 616c 3d73 656c 662e 5f69 735f  versal=self._is_
+00014c40: 7379 6d6d 6574 7279 2c0a 2020 2020 2020  symmetry,.      
+00014c50: 2020 2020 2020 7573 655f 6772 673d 7365        use_grg=se
+00014c60: 6c66 2e5f 7573 655f 6772 672c 0a20 2020  lf._use_grg,.   
+00014c70: 2020 2020 2020 2020 2066 6f72 6365 5f53           force_S
+00014c80: 4e46 3d46 616c 7365 2c0a 2020 2020 2020  NF=False,.      
+00014c90: 2020 2020 2020 534e 465f 636f 6f72 6469        SNF_coordi
+00014ca0: 6e61 7465 733d 7365 6c66 2e5f 534e 465f  nates=self._SNF_
+00014cb0: 636f 6f72 6469 6e61 7465 732c 0a20 2020  coordinates,.   
+00014cc0: 2020 2020 2020 2020 2073 746f 7265 5f64           store_d
+00014cd0: 656e 7365 5f67 705f 6d61 703d 5472 7565  ense_gp_map=True
+00014ce0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+00014cf0: 2064 6566 205f 696e 6974 5f64 796e 616d   def _init_dynam
+00014d00: 6963 616c 5f6d 6174 7269 7828 7365 6c66  ical_matrix(self
+00014d10: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
+00014d20: 6c66 2e5f 696e 7465 7261 6374 696f 6e20  lf._interaction 
+00014d30: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00014d40: 2020 2020 206d 7367 203d 2028 0a20 2020       msg = (.   
+00014d50: 2020 2020 2020 2020 2020 2020 2022 5068               "Ph
+00014d60: 6f6e 6f33 7079 2e69 6e69 745f 7068 7068  ono3py.init_phph
+00014d70: 5f69 6e74 6572 6163 7469 6f6e 2068 6173  _interaction has
+00014d80: 2074 6f20 6265 2063 616c 6c65 6420 220a   to be called ".
+00014d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014da0: 2262 6566 6f72 6520 7275 6e6e 696e 6720  "before running 
+00014db0: 7468 6973 206d 6574 686f 642e 220a 2020  this method.".  
+00014dc0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00014dd0: 2020 2020 2020 2020 7261 6973 6520 5275          raise Ru
+00014de0: 6e74 696d 6545 7272 6f72 286d 7367 290a  ntimeError(msg).
+00014df0: 0a20 2020 2020 2020 2073 656c 662e 5f69  .        self._i
+00014e00: 6e74 6572 6163 7469 6f6e 2e69 6e69 745f  nteraction.init_
+00014e10: 6479 6e61 6d69 6361 6c5f 6d61 7472 6978  dynamical_matrix
+00014e20: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
+00014e30: 6c66 2e5f 6663 322c 0a20 2020 2020 2020  lf._fc2,.       
+00014e40: 2020 2020 2073 656c 662e 5f70 686f 6e6f       self._phono
+00014e50: 6e5f 7375 7065 7263 656c 6c2c 0a20 2020  n_supercell,.   
+00014e60: 2020 2020 2020 2020 2073 656c 662e 5f70           self._p
+00014e70: 686f 6e6f 6e5f 7072 696d 6974 6976 652c  honon_primitive,
+00014e80: 0a20 2020 2020 2020 2020 2020 206e 6163  .            nac
+00014e90: 5f70 6172 616d 733d 7365 6c66 2e5f 6e61  _params=self._na
+00014ea0: 635f 7061 7261 6d73 2c0a 2020 2020 2020  c_params,.      
+00014eb0: 2020 290a 2020 2020 2020 2020 6672 6571    ).        freq
+00014ec0: 732c 205f 2c20 5f20 3d20 7365 6c66 2e67  s, _, _ = self.g
+00014ed0: 6574 5f70 686f 6e6f 6e5f 6461 7461 2829  et_phonon_data()
+00014ee0: 0a20 2020 2020 2020 2067 705f 4761 6d6d  .        gp_Gamm
+00014ef0: 6120 3d20 7365 6c66 2e5f 627a 5f67 7269  a = self._bz_gri
+00014f00: 642e 6770 5f47 616d 6d61 0a20 2020 2020  d.gp_Gamma.     
+00014f10: 2020 2069 6620 6e70 2e73 756d 2866 7265     if np.sum(fre
+00014f20: 7173 5b67 705f 4761 6d6d 615d 203c 2073  qs[gp_Gamma] < s
+00014f30: 656c 662e 5f63 7574 6f66 665f 6672 6571  elf._cutoff_freq
+00014f40: 7565 6e63 7929 203c 2033 3a0a 2020 2020  uency) < 3:.    
+00014f50: 2020 2020 2020 2020 666f 7220 692c 2066          for i, f
+00014f60: 2069 6e20 656e 756d 6572 6174 6528 6672   in enumerate(fr
+00014f70: 6571 735b 6770 5f47 616d 6d61 2c20 3a33  eqs[gp_Gamma, :3
+00014f80: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
+00014f90: 2020 2020 6966 206e 6f74 2028 6620 3c20      if not (f < 
+00014fa0: 7365 6c66 2e5f 6375 746f 6666 5f66 7265  self._cutoff_fre
+00014fb0: 7175 656e 6379 293a 0a20 2020 2020 2020  quency):.       
+00014fc0: 2020 2020 2020 2020 2020 2020 2066 7265               fre
+00014fd0: 7173 5b67 705f 4761 6d6d 612c 2069 5d20  qs[gp_Gamma, i] 
+00014fe0: 3d20 300a 2020 2020 2020 2020 2020 2020  = 0.            
+00014ff0: 2020 2020 2020 2020 7072 696e 7428 223d          print("=
+00015000: 2220 2a20 3236 202b 2022 2057 6172 6e69  " * 26 + " Warni
+00015010: 6e67 2022 202b 2022 3d22 202a 2032 3629  ng " + "=" * 26)
+00015020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015030: 2020 2020 2070 7269 6e74 280a 2020 2020       print(.    
+00015040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015050: 2020 2020 2220 5068 6f6e 6f6e 2066 7265      " Phonon fre
+00015060: 7175 656e 6379 206f 6620 6261 6e64 2069  quency of band i
+00015070: 6e64 6578 2025 6420 6174 2047 616d 6d61  ndex %d at Gamma
+00015080: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+00015090: 2020 2020 2020 2020 2020 2022 6973 2063             "is c
+000150a0: 616c 6375 6c61 7465 6420 746f 2062 6520  alculated to be 
+000150b0: 2566 2e22 2025 2028 6920 2b20 312c 2066  %f." % (i + 1, f
+000150c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000150d0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000150e0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+000150f0: 7428 2220 4275 7420 7468 6973 2066 7265  t(" But this fre
+00015100: 7175 656e 6379 2069 7320 666f 7263 6564  quency is forced
+00015110: 2074 6f20 6265 207a 6572 6f2e 2229 0a20   to be zero."). 
+00015120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015130: 2020 2070 7269 6e74 2822 3d22 202a 2036     print("=" * 6
+00015140: 3129 0a0a 2020 2020 6465 6620 5f65 7874  1)..    def _ext
+00015150: 7261 6374 5f66 6332 5f66 6333 5f63 616c  ract_fc2_fc3_cal
+00015160: 6375 6c61 746f 7273 2873 656c 662c 2066  culators(self, f
+00015170: 635f 6361 6c63 756c 6174 6f72 2c20 6663  c_calculator, fc
+00015180: 5f63 616c 6375 6c61 746f 725f 6f70 7469  _calculator_opti
+00015190: 6f6e 732c 206f 7264 6572 293a 0a20 2020  ons, order):.   
+000151a0: 2020 2020 2022 2222 4578 7472 6163 7420       """Extract 
+000151b0: 6663 5f63 616c 6375 6c61 746f 7220 616e  fc_calculator an
+000151c0: 6420 6663 5f63 616c 6375 6c61 746f 725f  d fc_calculator_
+000151d0: 6f70 7469 6f6e 7320 666f 7220 6663 3220  options for fc2 
+000151e0: 616e 6420 6663 332e 0a0a 2020 2020 2020  and fc3...      
+000151f0: 2020 6663 5f63 616c 6375 6c61 746f 7220    fc_calculator 
+00015200: 3a20 7374 720a 2020 2020 2020 2020 2020  : str.          
+00015210: 2020 4643 2063 616c 6375 6c61 746f 722e    FC calculator.
+00015220: 2022 7c22 2073 6570 6172 6174 6573 2066   "|" separates f
+00015230: 6332 2061 6e64 2066 6333 2e20 4669 7273  c2 and fc3. Firs
+00015240: 7420 616e 6420 6c61 7374 0a20 2020 2020  t and last.     
+00015250: 2020 2020 2020 2070 6172 7473 2073 6570         parts sep
+00015260: 6172 6174 6564 2063 6f72 7265 7370 6f6e  arated correspon
+00015270: 6420 746f 2066 6332 2061 6e64 2066 6333  d to fc2 and fc3
+00015280: 2063 616c 6375 6c61 746f 7273 2c20 7265   calculators, re
+00015290: 7370 6563 7469 7665 6c79 2e0a 2020 2020  spectively..    
+000152a0: 2020 2020 6663 5f63 616c 6375 6c61 746f      fc_calculato
+000152b0: 725f 6f70 7469 6f6e 7320 3a20 7374 720a  r_options : str.
+000152c0: 2020 2020 2020 2020 2020 2020 4643 2063              FC c
+000152d0: 616c 6375 6c61 746f 7220 6f70 7469 6f6e  alculator option
+000152e0: 732e 2022 7c22 2073 6570 6172 6174 6573  s. "|" separates
+000152f0: 2066 6332 2061 6e64 2066 6333 2e20 4669   fc2 and fc3. Fi
+00015300: 7273 7420 616e 6420 6c61 7374 0a20 2020  rst and last.   
+00015310: 2020 2020 2020 2020 2070 6172 7473 2073           parts s
+00015320: 6570 6172 6174 6564 2063 6f72 7265 7370  eparated corresp
+00015330: 6f6e 6420 746f 2066 6332 2061 6e64 2066  ond to fc2 and f
+00015340: 6333 206f 7074 696f 6e73 2c20 7265 7370  c3 options, resp
+00015350: 6563 7469 7665 6c79 2e0a 2020 2020 2020  ectively..      
+00015360: 2020 6f72 6465 7220 3a20 696e 7420 3d20    order : int = 
+00015370: 3220 6f72 2033 0a20 2020 2020 2020 2020  2 or 3.         
+00015380: 2020 2032 2061 6e64 2033 2069 6e64 6963     2 and 3 indic
+00015390: 6174 6520 6663 3220 616e 6420 6663 332c  ate fc2 and fc3,
+000153a0: 2072 6573 7065 6374 6976 656c 792e 0a0a   respectively...
+000153b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000153c0: 2020 2020 6966 2066 635f 6361 6c63 756c      if fc_calcul
+000153d0: 6174 6f72 2069 7320 6e6f 7420 4e6f 6e65  ator is not None
+000153e0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+000153f0: 2022 7c22 2069 6e20 6663 5f63 616c 6375   "|" in fc_calcu
+00015400: 6c61 746f 723a 0a20 2020 2020 2020 2020  lator:.         
+00015410: 2020 2020 2020 205f 6663 5f63 616c 6375         _fc_calcu
+00015420: 6c61 746f 7220 3d20 6663 5f63 616c 6375  lator = fc_calcu
+00015430: 6c61 746f 722e 7370 6c69 7428 227c 2229  lator.split("|")
+00015440: 5b6f 7264 6572 202d 2032 5d0a 2020 2020  [order - 2].    
+00015450: 2020 2020 2020 2020 2020 2020 6966 205f              if _
+00015460: 6663 5f63 616c 6375 6c61 746f 7220 3d3d  fc_calculator ==
+00015470: 2022 223a 0a20 2020 2020 2020 2020 2020   "":.           
+00015480: 2020 2020 2020 2020 205f 6663 5f63 616c           _fc_cal
+00015490: 6375 6c61 746f 7220 3d20 4e6f 6e65 0a20  culator = None. 
+000154a0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000154b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000154c0: 205f 6663 5f63 616c 6375 6c61 746f 7220   _fc_calculator 
+000154d0: 3d20 6663 5f63 616c 6375 6c61 746f 720a  = fc_calculator.
+000154e0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000154f0: 2020 2020 2020 2020 2020 5f66 635f 6361            _fc_ca
+00015500: 6c63 756c 6174 6f72 203d 204e 6f6e 650a  lculator = None.
+00015510: 0a20 2020 2020 2020 2069 6620 6663 5f63  .        if fc_c
+00015520: 616c 6375 6c61 746f 725f 6f70 7469 6f6e  alculator_option
+00015530: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+00015540: 2020 2020 2020 2020 2020 2069 6620 227c             if "|
+00015550: 2220 696e 2066 635f 6361 6c63 756c 6174  " in fc_calculat
+00015560: 6f72 5f6f 7074 696f 6e73 3a0a 2020 2020  or_options:.    
+00015570: 2020 2020 2020 2020 2020 2020 5f66 635f              _fc_
+00015580: 6361 6c63 756c 6174 6f72 5f6f 7074 696f  calculator_optio
+00015590: 6e73 203d 2066 635f 6361 6c63 756c 6174  ns = fc_calculat
+000155a0: 6f72 5f6f 7074 696f 6e73 2e73 706c 6974  or_options.split
+000155b0: 2822 7c22 295b 6f72 6465 7220 2d20 325d  ("|")[order - 2]
+000155c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000155d0: 2069 6620 5f66 635f 6361 6c63 756c 6174   if _fc_calculat
+000155e0: 6f72 5f6f 7074 696f 6e73 203d 3d20 2222  or_options == ""
+000155f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015600: 2020 2020 2020 5f66 635f 6361 6c63 756c        _fc_calcul
+00015610: 6174 6f72 5f6f 7074 696f 6e73 203d 204e  ator_options = N
+00015620: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+00015630: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00015640: 2020 2020 2020 5f66 635f 6361 6c63 756c        _fc_calcul
+00015650: 6174 6f72 5f6f 7074 696f 6e73 203d 2066  ator_options = f
+00015660: 635f 6361 6c63 756c 6174 6f72 5f6f 7074  c_calculator_opt
+00015670: 696f 6e73 0a20 2020 2020 2020 2065 6c73  ions.        els
+00015680: 653a 0a20 2020 2020 2020 2020 2020 205f  e:.            _
+00015690: 6663 5f63 616c 6375 6c61 746f 725f 6f70  fc_calculator_op
+000156a0: 7469 6f6e 7320 3d20 4e6f 6e65 0a0a 2020  tions = None..  
+000156b0: 2020 2020 2020 7265 7475 726e 205f 6663        return _fc
+000156c0: 5f63 616c 6375 6c61 746f 722c 205f 6663  _calculator, _fc
+000156d0: 5f63 616c 6375 6c61 746f 725f 6f70 7469  _calculator_opti
+000156e0: 6f6e 730a                                ons.
```

### Comparing `phono3py-2.9.2/phono3py/conductivity/base.py` & `phono3py-3.0.0/phono3py/conductivity/base.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/conductivity/direct_solution.py` & `phono3py-3.0.0/phono3py/conductivity/direct_solution.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/conductivity/kubo.py` & `phono3py-3.0.0/phono3py/conductivity/kubo.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/conductivity/rta.py` & `phono3py-3.0.0/phono3py/conductivity/rta.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/conductivity/utils.py` & `phono3py-3.0.0/phono3py/conductivity/utils.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/conductivity/wigner.py` & `phono3py-3.0.0/phono3py/conductivity/wigner.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/cui/create_force_constants.py` & `phono3py-3.0.0/phono3py/cui/create_force_constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,16 +50,14 @@
 from phonopy.interface.calculator import get_default_physical_units
 from phonopy.interface.fc_calculator import fc_calculator_names
 
 from phono3py import Phono3py
 from phono3py.cui.show_log import show_phono3py_force_constants_settings
 from phono3py.file_IO import (
     get_length_of_first_line,
-    parse_disp_fc2_yaml,
-    parse_disp_fc3_yaml,
     parse_FORCES_FC2,
     parse_FORCES_FC3,
     read_fc2_from_hdf5,
     read_fc3_from_hdf5,
     write_fc2_to_hdf5,
     write_fc3_to_hdf5,
 )
@@ -113,15 +111,14 @@
             _read_phono3py_fc3(phono3py, symmetrize_fc3r, input_filename, log_level)
         else:  # fc3 from FORCES_FC3 or ph3py_yaml
             _create_phono3py_fc3(
                 phono3py,
                 ph3py_yaml,
                 phono3py_yaml_filename,
                 symmetrize_fc3r,
-                input_filename,
                 settings.is_compact_fc,
                 settings.cutoff_pair_distance,
                 fc_calculator,
                 fc_calculator_options,
                 log_level,
             )
 
@@ -163,26 +160,24 @@
                 if log_level:
                     print("fc2 that was fit simultaneously with fc3 " "by ALM is used.")
             else:
                 _create_phono3py_fc2(
                     phono3py,
                     ph3py_yaml,
                     symmetrize_fc2,
-                    input_filename,
                     settings.is_compact_fc,
                     fc_calculator,
                     fc_calculator_options,
                     log_level,
                 )
         else:
             _create_phono3py_phonon_fc2(
                 phono3py,
                 ph3py_yaml,
                 symmetrize_fc2,
-                input_filename,
                 settings.is_compact_fc,
                 fc_calculator,
                 fc_calculator_options,
                 log_level,
             )
         if output_filename is None:
             filename = "fc2.hdf5"
@@ -203,15 +198,14 @@
 
 
 def parse_forces(
     phono3py: Phono3py,
     ph3py_yaml: Optional[Phono3pyYaml] = None,
     cutoff_pair_distance=None,
     force_filename: str = "FORCES_FC3",
-    disp_filename: Optional[str] = None,
     phono3py_yaml_filename: Optional[str] = None,
     fc_type=None,
     log_level=0,
 ):
     """Read displacements and forces.
 
     Physical units of displacements and forces are converted following the
@@ -265,40 +259,15 @@
             if calculator is not None:
                 _convert_unit_in_dataset(
                     dataset,
                     distance_to_A=physical_units["distance_to_A"],
                     force_to_eVperA=physical_units["force_to_eVperA"],
                 )
 
-    # No dataset is found. "disp_fc*.yaml" is read. But this is deprecated.
-    if dataset is None:
-        if disp_filename is None:
-            msg = (
-                "Displacement dataset corresponding to "
-                f'"{force_filename}" not found.'
-            )
-            raise RuntimeError(msg)
-        # Displacement dataset is obtained from disp_filename.
-        # can emit FileNotFoundError.
-        dataset = _read_disp_fc_yaml(disp_filename, fc_type)
-        filename_read_from = disp_filename
-
-        # No forces should exist. Therefore only unit of displacements is
-        # converted.
-        if calculator is None:
-            if log_level:
-                print(
-                    f'Displacements are read from "{disp_filename}", but '
-                    " the unit has not converted."
-                )
-        else:
-            _convert_unit_in_dataset(
-                dataset,
-                distance_to_A=physical_units["distance_to_A"],
-            )
+    assert dataset is not None
 
     if "natom" in dataset and dataset["natom"] != natom:
         msg = (
             "Number of atoms in supercell is not consistent with "
             '"%s".' % filename_read_from
         )
         raise RuntimeError(msg)
@@ -365,23 +334,14 @@
     fc_calculator_options = None
     if settings.fc_calculator_options is not None:
         fc_calculator_options = settings.fc_calculator_options
 
     return fc_calculator, fc_calculator_options
 
 
-def _read_disp_fc_yaml(disp_filename, fc_type):
-    if fc_type == "phonon_fc2":
-        dataset = parse_disp_fc2_yaml(filename=disp_filename)
-    else:
-        dataset = parse_disp_fc3_yaml(filename=disp_filename)
-
-    return dataset
-
-
 def _read_phono3py_fc3(phono3py, symmetrize_fc3r, input_filename, log_level):
     if input_filename is None:
         filename = "fc3.hdf5"
     else:
         filename = "fc3." + input_filename + ".hdf5"
     file_exists(filename, log_level)
     if log_level:
@@ -465,21 +425,20 @@
     return dataset
 
 
 def _create_phono3py_fc3(
     phono3py: Phono3py,
     ph3py_yaml: Optional[Phono3pyYaml],
     phono3py_yaml_filename: Optional[str],
-    symmetrize_fc3r,
-    input_filename,
-    is_compact_fc,
-    cutoff_pair_distance,
-    fc_calculator,
-    fc_calculator_options,
-    log_level,
+    symmetrize_fc3r: bool,
+    is_compact_fc: bool,
+    cutoff_pair_distance: Optional[float],
+    fc_calculator: Optional[str],
+    fc_calculator_options: Optional[str],
+    log_level: int,
 ):
     """Read or calculate fc3.
 
     Note
     ----
     cutoff_pair_distance is the parameter to determine each displaced
     supercell is included to the computation of fc3. It is assumed that
@@ -487,30 +446,22 @@
     displacements and the value is stored n the displacement dataset and
     also as the parameter 'included': True or False for each displacement.
     The parameter cutoff_pair_distance here can be used in the step to
     create fc3 by overwriting original cutoff_pair_distance value only
     when the former value is smaller than the later.
 
     """
-    # disp_fc3.yaml is obsolete.
-    if input_filename is None:
-        disp_filename = "disp_fc3.yaml"
-    else:
-        disp_filename = "disp_fc3." + input_filename + ".yaml"
-
-    # If disp_fc3.yaml is not found, default phono3py.yaml file is
-    _ph3py_yaml = _get_ph3py_yaml(disp_filename, ph3py_yaml)
+    _ph3py_yaml = _get_default_ph3py_yaml(ph3py_yaml)
 
     try:
         dataset = parse_forces(
             phono3py,
             ph3py_yaml=_ph3py_yaml,
             cutoff_pair_distance=cutoff_pair_distance,
             force_filename="FORCES_FC3",
-            disp_filename=disp_filename,
             phono3py_yaml_filename=phono3py_yaml_filename,
             fc_type="fc3",
             log_level=log_level,
         )
     except RuntimeError as e:
         # from _parse_forces_type1
         if log_level:
@@ -530,33 +481,26 @@
     )
 
 
 def _create_phono3py_fc2(
     phono3py: Phono3py,
     ph3py_yaml: Optional[Phono3pyYaml],
     symmetrize_fc2,
-    input_filename,
     is_compact_fc,
     fc_calculator,
     fc_calculator_options,
     log_level,
 ):
-    if input_filename is None:
-        disp_filename = "disp_fc3.yaml"
-    else:
-        disp_filename = "disp_fc3." + input_filename + ".yaml"
-
-    _ph3py_yaml = _get_ph3py_yaml(disp_filename, ph3py_yaml)
+    _ph3py_yaml = _get_default_ph3py_yaml(ph3py_yaml)
 
     try:
         dataset = parse_forces(
             phono3py,
             ph3py_yaml=_ph3py_yaml,
             force_filename="FORCES_FC3",
-            disp_filename=disp_filename,
             fc_type="fc2",
             log_level=log_level,
         )
     except RuntimeError as e:
         if log_level:
             print(str(e))
             print_error()
@@ -569,48 +513,38 @@
         symmetrize_fc2=symmetrize_fc2,
         is_compact_fc=is_compact_fc,
         fc_calculator=fc_calculator,
         fc_calculator_options=fc_calculator_options,
     )
 
 
-def _get_ph3py_yaml(disp_filename, ph3py_yaml: Optional[Phono3pyYaml]):
+def _get_default_ph3py_yaml(ph3py_yaml: Optional[Phono3pyYaml]):
     _ph3py_yaml = ph3py_yaml
-    # Try to use phono3py.phonon_dataset when the disp file not found
-    if not os.path.isfile(disp_filename):
-        disp_filename = None
-        if _ph3py_yaml is None and os.path.isfile("phono3py_disp.yaml"):
-            _ph3py_yaml = Phono3pyYaml()
-            _ph3py_yaml.read("phono3py_disp.yaml")
+    if _ph3py_yaml is None and os.path.isfile("phono3py_disp.yaml"):
+        _ph3py_yaml = Phono3pyYaml()
+        _ph3py_yaml.read("phono3py_disp.yaml")
     return _ph3py_yaml
 
 
 def _create_phono3py_phonon_fc2(
     phono3py: Phono3py,
     ph3py_yaml: Optional[Phono3pyYaml],
-    symmetrize_fc2,
-    input_filename,
-    is_compact_fc,
-    fc_calculator,
-    fc_calculator_options,
-    log_level,
+    symmetrize_fc2: bool,
+    is_compact_fc: bool,
+    fc_calculator: Optional[str],
+    fc_calculator_options: Optional[str],
+    log_level: int,
 ):
-    if input_filename is None:
-        disp_filename = "disp_fc2.yaml"
-    else:
-        disp_filename = "disp_fc2." + input_filename + ".yaml"
-
-    _ph3py_yaml = _get_ph3py_yaml(disp_filename, ph3py_yaml)
+    _ph3py_yaml = _get_default_ph3py_yaml(ph3py_yaml)
 
     try:
         dataset = parse_forces(
             phono3py,
             ph3py_yaml=_ph3py_yaml,
             force_filename="FORCES_FC2",
-            disp_filename=disp_filename,
             fc_type="phonon_fc2",
             log_level=log_level,
         )
     except RuntimeError as e:
         if log_level:
             print(str(e))
             print_error()
```

### Comparing `phono3py-2.9.2/phono3py/cui/create_supercells.py` & `phono3py-3.0.0/phono3py/cui/create_supercells.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,41 +33,34 @@
 # LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
 # ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 from phonopy.interface.calculator import write_supercells_with_displacements
 
 from phono3py import Phono3py
-from phono3py.file_IO import write_disp_fc2_yaml, write_disp_fc3_yaml
 from phono3py.interface.calculator import (
     get_additional_info_to_write_fc2_supercells,
     get_additional_info_to_write_supercells,
     get_default_displacement_distance,
 )
 
 
 def create_phono3py_supercells(
     cell_info,
     settings,
     symprec,
     output_filename=None,
     interface_mode="vasp",
     log_level=1,
-    write_disp_yaml=False,
 ):
     """Create displacements and supercells.
 
     Distance unit used is that for the calculator interface.
     The default unit is Angstron.
 
-    Parameters
-    ----------
-    write_disp_yaml : bool
-        Write old-style files of disp_fc3.yaml and disp_fc2.yaml. Default is False.
-
     """
     optional_structure_info = cell_info["optional_structure_info"]
 
     if settings.displacement_distance is None:
         distance = get_default_displacement_distance(interface_mode)
     else:
         distance = settings.displacement_distance
@@ -88,23 +81,14 @@
     )
 
     if log_level:
         print("")
         print('Unit cell was read from "%s".' % optional_structure_info[0])
         print("Displacement distance: %s" % distance)
 
-    if write_disp_yaml:
-        if output_filename is None:
-            filename = "disp_fc3.yaml"
-        else:
-            filename = "disp_fc3." + output_filename + ".yaml"
-        num_disps, num_disp_files = write_disp_fc3_yaml(
-            phono3py.dataset, phono3py.supercell, filename=filename
-        )
-
     ids = []
     disp_cells = []
     for i, cell in enumerate(phono3py.supercells_with_displacements):
         if cell is not None:
             ids.append(i + 1)
             disp_cells.append(cell)
 
@@ -128,23 +112,14 @@
         if settings.cutoff_pair_distance is not None:
             print(
                 "Cutoff distance for displacements: %s" % settings.cutoff_pair_distance
             )
             print("Number of displacement supercell files created: %d" % num_disp_files)
 
     if phono3py.phonon_supercell_matrix is not None:
-        if write_disp_yaml:
-            if output_filename is None:
-                filename = "disp_fc2.yaml"
-            else:
-                filename = "disp_fc2." + output_filename + ".yaml"
-            num_disps = write_disp_fc2_yaml(
-                phono3py.phonon_dataset, phono3py.phonon_supercell, filename=filename
-            )
-
         additional_info = get_additional_info_to_write_fc2_supercells(
             interface_mode, phono3py.phonon_supercell_matrix
         )
         write_supercells_with_displacements(
             interface_mode,
             phono3py.supercell,
             phono3py.phonon_supercells_with_displacements,
```

### Comparing `phono3py-2.9.2/phono3py/cui/kaccum_script.py` & `phono3py-3.0.0/phono3py/cui/kaccum_script.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,21 +2,15 @@
 
 import argparse
 import sys
 
 import h5py
 import numpy as np
 from phonopy.cui.collect_cell_info import collect_cell_info
-from phonopy.cui.settings import fracval
 from phonopy.interface.calculator import read_crystal_structure
-from phonopy.structure.cells import (
-    get_primitive,
-    get_primitive_matrix,
-    guess_primitive_matrix,
-)
 from phonopy.structure.symmetry import Symmetry
 
 from phono3py.interface.phono3py_yaml import Phono3pyYaml
 from phono3py.other.kaccum import GammaDOSsmearing, get_mfp, run_mfp_dos, run_prop_dos
 from phono3py.phonon.grid import BZGrid, get_ir_grid_points
 
 epsilon = 1.0e-8
@@ -125,22 +119,22 @@
         diff_q = qpoints - qpoints_for_check
         np.testing.assert_almost_equal(diff_q, np.rint(diff_q))
 
 
 def _get_calculator(args):
     """Return calculator name."""
     interface_mode = None
-    if args.qe_mode:
-        interface_mode = "qe"
-    elif args.crystal_mode:
-        interface_mode = "crystal"
-    elif args.abinit_mode:
-        interface_mode = "abinit"
-    elif args.turbomole_mode:
-        interface_mode = "turbomole"
+    # if args.qe_mode:
+    #     interface_mode = "qe"
+    # elif args.crystal_mode:
+    #     interface_mode = "crystal"
+    # elif args.abinit_mode:
+    #     interface_mode = "abinit"
+    # elif args.turbomole_mode:
+    #     interface_mode = "turbomole"
     return interface_mode
 
 
 def _read_files(args):
     """Read crystal structure and kappa.hdf5 files."""
     interface_mode = _get_calculator(args)
     if len(args.filenames) > 1:
@@ -153,24 +147,14 @@
             args.cell_filename, interface_mode=interface_mode
         )
         f = h5py.File(args.filenames[0], "r")
 
     return cell, f
 
 
-def _read_files_by_collect_cell_info(cell_filename, interface_mode):
-    cell_info = collect_cell_info(
-        interface_mode=interface_mode,
-        cell_filename=cell_filename,
-        supercell_matrix=np.eye(3, dtype=int),
-        phonopy_yaml_cls=Phono3pyYaml,
-    )
-    return cell_info
-
-
 def _get_mode_property(args, f_kappa):
     """Read property data from hdf5 file object."""
     if args.pqj:
         mode_prop = f_kappa["ave_pp"][:].reshape((1,) + f_kappa["ave_pp"].shape)
     elif args.cv:
         mode_prop = f_kappa["heat_capacity"][:]
     elif args.tau:
@@ -194,31 +178,14 @@
     return mode_prop
 
 
 def _get_parser():
     """Return args of ArgumentParser."""
     parser = argparse.ArgumentParser(description="Show unit cell volume")
     parser.add_argument(
-        "--pa",
-        "--primitive-axis",
-        "--primitive-axes",
-        nargs="+",
-        dest="primitive_matrix",
-        default=None,
-        help="Same as PRIMITIVE_AXES tags",
-    )
-    parser.add_argument(
-        "-c",
-        "--cell",
-        dest="cell_filename",
-        metavar="FILE",
-        default=None,
-        help="Read unit cell",
-    )
-    parser.add_argument(
         "--gv", action="store_true", help="Calculate for gv_x_gv (tensor)"
     )
     parser.add_argument("--pqj", action="store_true", help="Calculate for Pqj (scalar)")
     parser.add_argument("--cv", action="store_true", help="Calculate for Cv (scalar)")
     parser.add_argument(
         "--tau", action="store_true", help="Calculate for lifetimes (scalar)"
     )
@@ -268,120 +235,63 @@
     )
     parser.add_argument(
         "--smearing",
         action="store_true",
         help="Use smearing method (only for scalar density)",
     )
     parser.add_argument(
-        "--qe", "--pwscf", dest="qe_mode", action="store_true", help="Invoke Pwscf mode"
-    )
-    parser.add_argument(
-        "--crystal",
-        dest="crystal_mode",
-        action="store_true",
-        help="Invoke CRYSTAL mode",
-    )
-    parser.add_argument(
-        "--abinit", dest="abinit_mode", action="store_true", help="Invoke Abinit mode"
-    )
-    parser.add_argument(
-        "--turbomole",
-        dest="turbomole_mode",
-        action="store_true",
-        help="Invoke TURBOMOLE mode",
-    )
-    parser.add_argument(
         "--no-gridsym",
         dest="no_gridsym",
         action="store_true",
         help="Grid symmetry is unused for phonon-xxx.hdf5 inputs.",
     )
     parser.add_argument("filenames", nargs="*")
     args = parser.parse_args()
     return args
 
 
-def _analyze_primitive_matrix_option(args, unitcell=None):
-    """Analyze --pa option argument."""
-    if args.primitive_matrix is not None:
-        if type(args.primitive_matrix) is list:
-            _primitive_matrix = " ".join(args.primitive_matrix)
-        else:
-            _primitive_matrix = args.primitive_matrix.strip()
-
-        if _primitive_matrix.lower() == "auto":
-            primitive_matrix = "auto"
-        elif _primitive_matrix.upper() in ("P", "F", "I", "A", "C", "R"):
-            primitive_matrix = _primitive_matrix.upper()
-        elif len(_primitive_matrix.split()) != 9:
-            raise SyntaxError("Number of elements in --pa option argument has to be 9.")
-        else:
-            primitive_matrix = np.reshape(
-                [fracval(x) for x in _primitive_matrix.split()], (3, 3)
-            )
-            if np.linalg.det(primitive_matrix) < 1e-8:
-                raise SyntaxError("Primitive matrix has to have positive determinant.")
-
-    pmat = get_primitive_matrix(primitive_matrix)
-    if unitcell is not None and isinstance(pmat, str) and pmat == "auto":
-        return guess_primitive_matrix(unitcell)
-    else:
-        return pmat
-
-
 def main():
     """Calculate kappa spectrum.
 
     Usage
     -----
     If `phono3py_disp.yaml` or `phono3py.yaml` exists in current directory,
     ```
     % phono3py-kaccum kappa-m111111.hdf5
     ```
 
-    Old style usage
-    ---------------
-    ```
-    % phono3py-kaccum --pa="F" -c POSCAR-unitcell kappa-m111111.hdf5 |tee kaccum.dat
-    ```
-
     Plot by gnuplot
     ---------------
     ```
     % gnuplot
     ...
     gnuplot> p "kaccum.dat" i 30 u 1:2 w l, "kaccum.dat" i 30 u 1:8 w l
     ```
 
-    With phono3py.yaml type file as crystal structure, primitive matrix is
-    unnecessary to set.
-
     """
     args = _get_parser()
     primitive = None
-    if len(args.filenames) > 1:  # deprecated
-        cell, f_kappa = _read_files(args)
-        primitive_matrix = _analyze_primitive_matrix_option(args, unitcell=cell)
+    if len(args.filenames) > 1:
+        raise RuntimeError(
+            'Use of "phono3py-kaccum CRYSTAL_STRUCTURE_FILE" is not supported.'
+        )
     else:
-        interface_mode = _get_calculator(args)
-        cell_info = _read_files_by_collect_cell_info(args.cell_filename, interface_mode)
+        cell_info = collect_cell_info(
+            supercell_matrix=np.eye(3, dtype=int),
+            phonopy_yaml_cls=Phono3pyYaml,
+        )
+        cell_filename = cell_info["optional_structure_info"][0]
+        print(f'# Crystal structure was read from "{cell_filename}".')
         cell = cell_info["unitcell"]
         phpy_yaml = cell_info.get("phonopy_yaml", None)
         if phpy_yaml is not None:
             primitive = cell_info["phonopy_yaml"].primitive
             if primitive is None:
                 primitive = cell
-        else:
-            primitive_matrix = _analyze_primitive_matrix_option(args, unitcell=cell)
         f_kappa = h5py.File(args.filenames[0], "r")
-    if primitive is None:
-        if primitive_matrix is None:
-            primitive = cell
-        else:
-            primitive = get_primitive(cell, primitive_matrix)
 
     if "grid_matrix" in f_kappa:
         mesh = np.array(f_kappa["grid_matrix"][:], dtype="int_")
     else:
         mesh = np.array(f_kappa["mesh"][:], dtype="int_")
     if "temperature" in f_kappa:
         temperatures = f_kappa["temperature"][:]
```

### Comparing `phono3py-2.9.2/phono3py/cui/load.py` & `phono3py-3.0.0/phono3py/cui/load.py`

 * *Files 12% similar despite different names*

```diff
@@ -90,25 +90,25 @@
     "phono3py_yaml"-like file is parsed unless crystal structure information is
     given by unitcell_filename, supercell_filename, unitcell
     (PhonopyAtoms-like), or supercell (PhonopyAtoms-like). Even when
     "phono3py_yaml"-like file is parse, parameters except for crystal structure
     can be overwritten.
 
     'fc3.hdf5' is read if found in current directory. Unless 'fc3.hdf5' is found
-    and if 'FORCES_FC3' and 'disp_fc3.yaml" are found, these are read and fc3
-    and fc2 are produced.
+    and if 'FORCES_FC3' and 'phono3py_disp.yaml" are found, these are read and
+    fc3 and fc2 are produced.
 
     if 'fc2.hdf5' is found, this is read. Unless 'fc2.hdf5' is found and if
-    'FORCES_FC2' and 'disp_fc2.yaml" are found, these are read and fc2 is
+    'FORCES_FC2' and 'phono3py_disp.yaml" are found, these are read and fc2 is
     produced.
 
     When force_sets_filename and force_constants_filename are not given,
     'FORCES_FC3' and 'FORCES_FC2' are looked for in the current directory as the
     default behaviour. When 'FORCES_FC3' ('FORCES_FC2') is given in the type-1
-    format, 'disp_fc3.yaml' ('disp_fc2.yaml') is also necessary and read.
+    format, 'phono3py_disp.yaml' is also necessary and read.
 
     Crystal structure
     -----------------
     Means to provide crystal structure(s) and their priority:
         1. unitcell_filename (with supercell_matrix)
         2. supercell_filename
         3. unitcell (with supercell_matrix)
@@ -117,20 +117,20 @@
 
     Force sets or force constants
     -----------------------------
     Optional. Means to provide information to generate force constants and their
     priority:
         1. fc3_filename (fc2_filename)
         2. forces_fc3_filename (forces_fc2_filename). Do not forget that for
-           type-1 format, disp_fc3.yaml (disp_fc2.yaml) has to be given, too.
+           type-1 format, phono3py_disp.yaml has to be given, too.
         3. 'fc3.hdf5' and 'fc2.hdf5' are searched in current directory.
         4. 'FORCES_FC3' and 'FORCES_FC2' are searched in current directory.
-           'FORCES_FC2' is optional. For type-1 format, 'disp_fc3.yaml' and
-           optionally 'disp_fc2.yaml' are also searched in current directory.
-           When 'FORCES_FC2' is not found, 'FORCES_FC3' is used to create fc2.
+           'FORCES_FC2' is optional. For type-1 format, 'phono3py_disp.yaml' is
+           also searched in current directory. When 'FORCES_FC2' is not found,
+           'FORCES_FC3' is used to create fc2.
 
     Parameters for non-analytical term correctiion (NAC)
     ----------------------------------------------------
     Optional. Means to provide NAC parameters and their priority:
         1. born_filename
         2. nac_params
         3. phono3py_yaml_like.nac_params if existed and is_nac=True.
@@ -184,19 +184,19 @@
         Input supercell filename. When this is specified, supercell_matrix is
         ignored. Default is None.
     born_filename : os.PathLike, optional
         Filename corresponding to 'BORN', a file contains non-analytical term
         correction parameters.
     forces_fc3_filename : sequence or os.PathLike, optional
         A two-elemental sequence of filenames corresponding to ('FORCES_FC3',
-        'disp_fc3.yaml') in the type-1 format or a filename (os.PathLike)
+        'phono3py_disp.yaml') in the type-1 format or a filename (os.PathLike)
         corresponding to 'FORCES_FC3' in the type-2 format. Default is None.
     forces_fc2_filename : os.PathLike or sequence, optional
         A two-elemental sequence of filenames corresponding to ('FORCES_FC2',
-        'disp_fc2.yaml') in the type-1 format or a filename (os.PathLike)
+        'phono3py_disp.yaml') in the type-1 format or a filename (os.PathLike)
         corresponding to 'FORCES_FC2' in the type-2 format. Default is None.
     fc3_filename : os.PathLike, optional
         Filename of a file corresponding to 'fc3.hdf5', a file contains
         third-order force constants. Default is None.
     fc2_filename : os.PathLike, optional
         Filename of a file corresponding to 'fc2.hdf5', a file contains
         second-order force constants. Default is None.
@@ -229,18 +229,18 @@
         and for fc2
             True: (primitive, supecell, 3, 3) False: (supercell, supecell, 3, 3)
         where 'supercell' and 'primitive' indicate number of atoms in these
         cells. Default is False.
     use_grg : bool, optional
         Use generalized regular grid when True. Default is False.
     make_r0_average : bool, optional
-        fc3 transformation from real to reciprocal space is done
-        around three atoms and averaged when True. Default is False, i.e.,
-        only around the first atom. Setting False is for rough compatibility
-        with v2.x. Default is True.
+        fc3 transformation from real to reciprocal space is done around three
+        atoms and averaged when True. Default is False, i.e., only around the
+        first atom. Setting False is for rough compatibility with v2.x. Default
+        is True.
     symprec : float, optional
         Tolerance used to find crystal symmetry. Default is 1e-5.
     log_level : int, optional
         Verbosity control. Default is 0.
 
     """
     if (
@@ -473,61 +473,48 @@
         fc3 = read_fc3_from_hdf5(filename=fc3_filename, p2s_map=p2s_map)
         _check_fc3_shape(ph3py, fc3, filename=fc3_filename)
         ph3py.fc3 = fc3
         read_fc3 = True
         if log_level:
             print('fc3 was read from "%s".' % fc3_filename)
     elif forces_fc3_filename is not None:
-        if isinstance(forces_fc3_filename, os.PathLike):
-            force_filename = forces_fc3_filename
-            disp_filename = None
-        else:
-            force_filename, disp_filename = forces_fc3_filename
+        force_filename = forces_fc3_filename
         _set_dataset_for_fc3(
             ph3py,
             ph3py_yaml,
             force_filename,
-            disp_filename,
             phono3py_yaml_filename,
             cutoff_pair_distance,
             log_level,
         )
     elif os.path.isfile("fc3.hdf5"):
         fc3 = read_fc3_from_hdf5(filename="fc3.hdf5", p2s_map=p2s_map)
         _check_fc3_shape(ph3py, fc3)
         ph3py.fc3 = fc3
         read_fc3 = True
         if log_level:
             print('fc3 was read from "fc3.hdf5".')
     elif os.path.isfile("FORCES_FC3"):
-        disp_filename = None
-        if os.path.isfile("disp_fc3.yaml"):
-            if ph3py_yaml is None:
-                disp_filename = "disp_fc3.yaml"
-            elif ph3py_yaml.dataset is None:
-                disp_filename = "disp_fc3.yaml"
         _set_dataset_for_fc3(
             ph3py,
             ph3py_yaml,
             "FORCES_FC3",
-            disp_filename,
             phono3py_yaml_filename,
             cutoff_pair_distance,
             log_level,
         )
     elif (
         ph3py_yaml is not None
         and ph3py_yaml.dataset is not None
         and forces_in_dataset(ph3py_yaml.dataset)
     ):
         _set_dataset_for_fc3(
             ph3py,
             ph3py_yaml,
             None,
-            None,
             phono3py_yaml_filename,
             cutoff_pair_distance,
             log_level,
         )
     return read_fc3
 
 
@@ -544,128 +531,103 @@
         fc2 = read_fc2_from_hdf5(filename=fc2_filename, p2s_map=phonon_p2s_map)
         _check_fc2_shape(ph3py, fc2, filename=fc2_filename)
         ph3py.fc2 = fc2
         read_fc2 = True
         if log_level:
             print('fc2 was read from "%s".' % fc2_filename)
     elif forces_fc2_filename is not None:
-        if isinstance(forces_fc2_filename, os.PathLike):
-            force_filename = forces_fc2_filename
-            disp_filename = None
-        else:
-            force_filename, disp_filename = forces_fc2_filename
+        force_filename = forces_fc2_filename
         _set_dataset_for_fc2(
             ph3py,
             ph3py_yaml,
             force_filename,
-            disp_filename,
             "phonon_fc2",
             log_level,
         )
     elif os.path.isfile("fc2.hdf5"):
         fc2 = read_fc2_from_hdf5(filename="fc2.hdf5", p2s_map=phonon_p2s_map)
         _check_fc2_shape(ph3py, fc2)
         ph3py.fc2 = fc2
         read_fc2 = True
         if log_level:
             print('fc2 was read from "fc2.hdf5".')
     elif os.path.isfile("FORCES_FC2"):
-        disp_filename = None
-        if os.path.isfile("disp_fc2.yaml"):
-            if ph3py_yaml is None:
-                disp_filename = "disp_fc2.yaml"
-            elif ph3py_yaml.phonon_dataset is None:
-                disp_filename = "disp_fc2.yaml"
         _set_dataset_for_fc2(
             ph3py,
             ph3py_yaml,
             "FORCES_FC2",
-            disp_filename,
             "phonon_fc2",
             log_level,
         )
     elif (
         ph3py_yaml is not None
         and ph3py_yaml.phonon_dataset is not None
         and forces_in_dataset(ph3py_yaml.phonon_dataset)
     ):
         _set_dataset_for_fc2(
             ph3py,
             ph3py_yaml,
             None,
-            None,
             "phonon_fc2",
             log_level,
         )
     elif (
         ph3py_yaml is not None
         and ph3py_yaml.dataset is not None
         and forces_in_dataset(ph3py_yaml.dataset)
     ):
         _set_dataset_for_fc2(
             ph3py,
             ph3py_yaml,
             None,
-            None,
             "fc2",
             log_level,
         )
     elif os.path.isfile("FORCES_FC3"):
         # suppose fc3.hdf5 is read but fc2.hdf5 doesn't exist.
-        disp_filename = None
-        if os.path.isfile("disp_fc3.yaml"):
-            if ph3py_yaml is None:
-                disp_filename = "disp_fc3.yaml"
-            elif ph3py_yaml.dataset is None:
-                disp_filename = "disp_fc3.yaml"
         _set_dataset_for_fc2(
             ph3py,
             ph3py_yaml,
             "FORCES_FC3",
-            disp_filename,
             "fc2",
             log_level,
         )
     return read_fc2
 
 
 def _set_dataset_for_fc3(
     ph3py: Phono3py,
     ph3py_yaml: Optional[Phono3pyYaml],
     force_filename,
-    disp_filename,
     phono3py_yaml_filename,
     cutoff_pair_distance,
     log_level,
 ):
     ph3py.dataset = parse_forces(
         ph3py,
         ph3py_yaml=ph3py_yaml,
         cutoff_pair_distance=cutoff_pair_distance,
         force_filename=force_filename,
-        disp_filename=disp_filename,
         phono3py_yaml_filename=phono3py_yaml_filename,
         fc_type="fc3",
         log_level=log_level,
     )
 
 
 def _set_dataset_for_fc2(
     ph3py: Phono3py,
     ph3py_yaml: Optional[Phono3pyYaml],
     force_filename,
-    disp_filename,
     fc_type,
     log_level,
 ):
     dataset = parse_forces(
         ph3py,
         ph3py_yaml=ph3py_yaml,
         force_filename=force_filename,
-        disp_filename=disp_filename,
         fc_type=fc_type,
         log_level=log_level,
     )
     if fc_type == "phonon_fc2":
         ph3py.phonon_dataset = dataset
     else:
         ph3py.dataset = dataset
```

### Comparing `phono3py-2.9.2/phono3py/cui/phono3py_argparse.py` & `phono3py-3.0.0/phono3py/cui/phono3py_argparse.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,15 +278,15 @@
             "--fc3",
             dest="read_fc3",
             action="store_true",
             default=False,
             help="Read third order force constants",
         )
     parser.add_argument(
-        "--v3",
+        "--v2",
         dest="is_fc3_r0_average",
         action="store_true",
         default=False,
         help="Take average in fc3-r2q transformation around three atoms",
     )
     parser.add_argument(
         "--fc-calc",
```

### Comparing `phono3py-2.9.2/phono3py/cui/phono3py_script.py` & `phono3py-3.0.0/phono3py/cui/phono3py_script.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,16 +79,14 @@
     show_general_settings,
     show_phono3py_cells,
     show_phono3py_settings,
 )
 from phono3py.cui.triplets_info import show_num_triplets, write_grid_points
 from phono3py.file_IO import (
     get_length_of_first_line,
-    parse_disp_fc2_yaml,
-    parse_disp_fc3_yaml,
     parse_FORCES_FC2,
     read_phonon_from_hdf5,
     write_fc2_to_hdf5,
     write_fc3_to_hdf5,
     write_FORCES_FC2,
     write_FORCES_FC3,
     write_phonon_to_hdf5,
@@ -381,44 +379,37 @@
             )
             print_end_phono3py()
     sys.exit(0)
 
 
 def create_FORCES_FC3_and_FORCES_FC2_then_exit(
     settings,
-    input_filename: Optional[str],
     cell_filename: Optional[str],
     log_level: Union[bool, int],
 ):
     """Create FORCES_FC3 and FORCES_FC2 from files."""
     interface_mode = settings.calculator
     ph3py_yaml = None
 
     #####################
     # Create FORCES_FC3 #
     #####################
     if settings.create_forces_fc3 or settings.create_forces_fc3_file:
-        if input_filename is None:
-            disp_fc3_filename = "disp_fc3.yaml"
-        else:
-            disp_fc3_filename = "disp_fc3." + input_filename + ".yaml"
-        disp_filename_candidates = ["phono3py_disp.yaml", disp_fc3_filename]
+        disp_filename_candidates = [
+            "phono3py_disp.yaml",
+        ]
         if cell_filename is not None:
             disp_filename_candidates.insert(0, cell_filename)
         disp_filenames = files_exist(disp_filename_candidates, log_level, is_any=True)
         disp_filename = disp_filenames[0]
-        if disp_filename == disp_fc3_filename:
-            file_exists(disp_filename, log_level)
-            disp_dataset = parse_disp_fc3_yaml(filename=disp_filename)
-        else:
-            ph3py_yaml = Phono3pyYaml()
-            ph3py_yaml.read(disp_filename)
-            if ph3py_yaml.calculator is not None:
-                interface_mode = ph3py_yaml.calculator  # overwrite
-            disp_dataset = ph3py_yaml.dataset
+        ph3py_yaml = Phono3pyYaml()
+        ph3py_yaml.read(disp_filename)
+        if ph3py_yaml.calculator is not None:
+            interface_mode = ph3py_yaml.calculator  # overwrite
+        disp_dataset = ph3py_yaml.dataset
 
         if log_level:
             print("")
             print('Displacement dataset was read from "%s".' % disp_filename)
 
         num_atoms = disp_dataset["natom"]
         num_disps = len(disp_dataset["first_atoms"])
@@ -484,35 +475,29 @@
                 print_error()
             sys.exit(1)
 
     #####################
     # Create FORCES_FC2 #
     #####################
     if settings.create_forces_fc2:
-        if input_filename is None:
-            disp_fc2_filename = "disp_fc2.yaml"
-        else:
-            disp_fc2_filename = "disp_fc2." + input_filename + ".yaml"
-        disp_filename_candidates = ["phono3py_disp.yaml", disp_fc2_filename]
+        disp_filename_candidates = [
+            "phono3py_disp.yaml",
+        ]
         if cell_filename is not None:
             disp_filename_candidates.insert(0, cell_filename)
         disp_filenames = files_exist(disp_filename_candidates, log_level, is_any=True)
         disp_filename = disp_filenames[0]
 
-        if disp_filename == disp_fc2_filename:
-            file_exists(disp_filename, log_level)
-            disp_dataset = parse_disp_fc2_yaml(filename=disp_filename)
-        else:
-            # ph3py_yaml is not None, phono3py_disp.yaml is already read.
-            if ph3py_yaml is None:
-                ph3py_yaml = Phono3pyYaml()
-                ph3py_yaml.read(disp_filename)
-                if ph3py_yaml.calculator is not None:
-                    interface_mode = ph3py_yaml.calculator  # overwrite
-            disp_dataset = ph3py_yaml.phonon_dataset
+        # ph3py_yaml is not None, phono3py_disp.yaml is already read.
+        if ph3py_yaml is None:
+            ph3py_yaml = Phono3pyYaml()
+            ph3py_yaml.read(disp_filename)
+            if ph3py_yaml.calculator is not None:
+                interface_mode = ph3py_yaml.calculator  # overwrite
+        disp_dataset = ph3py_yaml.phonon_dataset
 
         if log_level:
             print('Displacement dataset was read from "%s".' % disp_filename)
         num_atoms = disp_dataset["natom"]
         num_disps = len(disp_dataset["first_atoms"])
         force_filenames = settings.create_forces_fc2
         for filename in force_filenames:
@@ -1134,17 +1119,15 @@
     # -----------------------------------------------------------------------
     # ----------------- 'args' should not be used below. --------------------
     # -----------------------------------------------------------------------
 
     ####################################
     # Create FORCES_FC3 and FORCES_FC2 #
     ####################################
-    create_FORCES_FC3_and_FORCES_FC2_then_exit(
-        settings, input_filename, cell_filename, log_level
-    )
+    create_FORCES_FC3_and_FORCES_FC2_then_exit(settings, cell_filename, log_level)
 
     ###########################################################
     # Symmetry tolerance. Distance unit depends on interface. #
     ###########################################################
     if settings.symmetry_tolerance is None:
         symprec = 1e-5
     else:
```

### Comparing `phono3py-2.9.2/phono3py/cui/settings.py` & `phono3py-3.0.0/phono3py/cui/settings.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/cui/show_log.py` & `phono3py-3.0.0/phono3py/cui/show_log.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/cui/triplets_info.py` & `phono3py-3.0.0/phono3py/cui/triplets_info.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/file_IO.py` & `phono3py-3.0.0/phono3py/file_IO.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,36 +47,20 @@
 # This import is deactivated for a while.
 # from phonopy.file_IO import write_force_constants_to_hdf5
 from phonopy.file_IO import check_force_constants_indices, get_cell_from_disp_yaml
 
 from phono3py.version import __version__
 
 
-def write_cell_yaml(w, supercell):
-    """Write cell info.
+def write_disp_fc3_yaml(dataset, supercell, filename="disp_fc3.yaml"):
+    """Write disp_fc3.yaml.
 
-    This is only used from write_disp_fc3_yaml and write_disp_fc2_yaml.
-    These methods are also deprecated.
+    This function should not be called from phono3py script from version 3.
 
     """
-    warnings.warn("write_cell_yaml() is deprecated.", DeprecationWarning)
-
-    w.write("lattice:\n")
-    for axis in supercell.get_cell():
-        w.write("- [ %20.15f,%20.15f,%20.15f ]\n" % tuple(axis))
-    symbols = supercell.get_chemical_symbols()
-    positions = supercell.get_scaled_positions()
-    w.write("atoms:\n")
-    for i, (s, v) in enumerate(zip(symbols, positions)):
-        w.write("- symbol: %-2s # %d\n" % (s, i + 1))
-        w.write("  position: [ %18.14f,%18.14f,%18.14f ]\n" % tuple(v))
-
-
-def write_disp_fc3_yaml(dataset, supercell, filename="disp_fc3.yaml"):
-    """Write disp_fc3.yaml."""
     warnings.warn("write_disp_fc3_yaml() is deprecated.", DeprecationWarning)
 
     w = open(filename, "w")
     w.write("natom: %d\n" % dataset["natom"])
 
     num_first = len(dataset["first_atoms"])
     w.write("num_first_displacements: %d\n" % num_first)
@@ -154,23 +138,27 @@
                     "    - [%20.16f,%20.16f,%20.16f ] # %05d\n"
                     % (disp_cart2[0], disp_cart2[1], disp_cart2[2], count2)
                 )
 
             ids = ["%d" % disp2["id"] for disp2 in disp2_list]
             w.write("    displacement_ids: [ %s ]\n" % ", ".join(ids))
 
-    write_cell_yaml(w, supercell)
+    _write_cell_yaml(w, supercell)
 
     w.close()
 
     return num_first + num_second, num_disp_files
 
 
 def write_disp_fc2_yaml(dataset, supercell, filename="disp_fc2.yaml"):
-    """Write disp_fc2.yaml."""
+    """Write disp_fc2.yaml.
+
+    This function should not be called from phono3py script from version 3.
+
+    """
     warnings.warn("write_disp_fc2_yaml() is deprecated.", DeprecationWarning)
 
     w = open(filename, "w")
     w.write("natom: %d\n" % dataset["natom"])
 
     num_first = len(dataset["first_atoms"])
     w.write("num_first_displacements: %d\n" % num_first)
@@ -181,15 +169,15 @@
         w.write("  displacement:\n")
         w.write(
             "    [%20.16f,%20.16f,%20.16f ] # %05d\n"
             % (disp_cart1[0], disp_cart1[1], disp_cart1[2], i + 1)
         )
 
     if supercell is not None:
-        write_cell_yaml(w, supercell)
+        _write_cell_yaml(w, supercell)
 
     w.close()
 
     return num_first
 
 
 def write_FORCES_FC2(disp_dataset, forces_fc2=None, fp=None, filename="FORCES_FC2"):
@@ -267,33 +255,14 @@
                     w.write("%15.10f %15.10f %15.10f\n" % (0, 0, 0))
             count += 1
 
     if fp is None:
         w.close()
 
 
-def write_fc3_dat(force_constants_third, filename="fc3.dat"):
-    """Write fc3.dat."""
-    warnings.warn("write_fc3_dat() is deprecated.", DeprecationWarning)
-
-    w = open(filename, "w")
-    for i in range(force_constants_third.shape[0]):
-        for j in range(force_constants_third.shape[1]):
-            for k in range(force_constants_third.shape[2]):
-                tensor3 = force_constants_third[i, j, k]
-                w.write(
-                    " %d - %d - %d  (%f)\n"
-                    % (i + 1, j + 1, k + 1, np.abs(tensor3).sum())
-                )
-                for tensor2 in tensor3:
-                    for vec in tensor2:
-                        w.write("%20.14f %20.14f %20.14f\n" % tuple(vec))
-                    w.write("\n")
-
-
 def write_fc3_to_hdf5(fc3, filename="fc3.hdf5", p2s_map=None, compression="gzip"):
     """Write fc3 in fc3.hdf5.
 
     Parameters
     ----------
     force_constants : ndarray
         Force constants
@@ -400,72 +369,14 @@
 def read_fc2_from_hdf5(filename="fc2.hdf5", p2s_map=None):
     """Read fc2 from fc2.hdf5."""
     return read_force_constants_from_hdf5(
         filename=filename, p2s_map=p2s_map, calculator="vasp"
     )
 
 
-def write_triplets(
-    triplets, weights, mesh, grid_address, grid_point=None, filename=None
-):
-    """Write triplets in triplets.dat."""
-    warnings.warn("write_triplets() is deprecated.", DeprecationWarning)
-
-    triplets_filename = "triplets"
-    suffix = "-m%d%d%d" % tuple(mesh)
-    if grid_point is not None:
-        suffix += "-g%d" % grid_point
-    if filename is not None:
-        suffix += "." + filename
-    suffix += ".dat"
-    triplets_filename += suffix
-    w = open(triplets_filename, "w")
-    for weight, g3 in zip(weights, triplets):
-        w.write("%4d    " % weight)
-        for q3 in grid_address[g3]:
-            w.write("%4d %4d %4d    " % tuple(q3))
-        w.write("\n")
-    w.close()
-
-
-def write_grid_address(grid_address, mesh, filename=None):
-    """Write grid addresses in grid_address.dat."""
-    warnings.warn("write_grid_address() is deprecated.", DeprecationWarning)
-
-    grid_address_filename = "grid_address"
-    suffix = "-m%d%d%d" % tuple(mesh)
-    if filename is not None:
-        suffix += "." + filename
-    suffix += ".dat"
-    grid_address_filename += suffix
-
-    w = open(grid_address_filename, "w")
-    w.write("# Grid addresses for %dx%dx%d mesh\n" % tuple(mesh))
-    w.write(
-        "#%9s    %8s %8s %8s     %8s %8s %8s\n"
-        % (
-            "index",
-            "a",
-            "b",
-            "c",
-            ("a%%%d" % mesh[0]),
-            ("b%%%d" % mesh[1]),
-            ("c%%%d" % mesh[2]),
-        )
-    )
-    for i, bz_q in enumerate(grid_address):
-        if i == np.prod(mesh):
-            w.write("#" + "-" * 78 + "\n")
-        q = bz_q % mesh
-        w.write("%10d    %8d %8d %8d     " % (i, bz_q[0], bz_q[1], bz_q[2]))
-        w.write("%8d %8d %8d\n" % tuple(q))
-
-    return grid_address_filename
-
-
 def write_grid_address_to_hdf5(
     grid_address,
     mesh,
     grid_mapping_table,
     bz_grid=None,
     compression="gzip",
     filename=None,
@@ -1562,15 +1473,15 @@
     with open("ir_grid_points.yaml", "w") as w:
         w.write("\n".join(lines))
 
 
 def parse_disp_fc2_yaml(filename="disp_fc2.yaml", return_cell=False):
     """Parse disp_fc2.yaml file.
 
-    This is obsolete at v2 and later versions.
+    This function should not be called from phono3py script from version 3.
 
     """
     warnings.warn("parse_disp_fc2_yaml() is deprecated.", DeprecationWarning)
 
     dataset = _parse_yaml(filename)
     natom = dataset["natom"]
     new_dataset = {}
@@ -1589,15 +1500,15 @@
     else:
         return new_dataset
 
 
 def parse_disp_fc3_yaml(filename="disp_fc3.yaml", return_cell=False):
     """Parse disp_fc3.yaml file.
 
-    This is obsolete at v2 and later versions.
+    This function should not be called from phono3py script from version 3.
 
     """
     warnings.warn("parse_disp_fc3_yaml() is deprecated.", DeprecationWarning)
 
     dataset = _parse_yaml(filename)
     natom = dataset["natom"]
     new_dataset = {}
@@ -1796,7 +1707,27 @@
         if len(forces) == num_atom:
             break
 
     if not len(forces) == num_atom:
         return None
     else:
         return np.array(forces)
+
+
+def _write_cell_yaml(w, supercell):
+    """Write cell info.
+
+    This is only used from write_disp_fc3_yaml and write_disp_fc2_yaml.
+    These methods are also deprecated.
+
+    """
+    warnings.warn("write_cell_yaml() is deprecated.", DeprecationWarning)
+
+    w.write("lattice:\n")
+    for axis in supercell.get_cell():
+        w.write("- [ %20.15f,%20.15f,%20.15f ]\n" % tuple(axis))
+    symbols = supercell.get_chemical_symbols()
+    positions = supercell.get_scaled_positions()
+    w.write("atoms:\n")
+    for i, (s, v) in enumerate(zip(symbols, positions)):
+        w.write("- symbol: %-2s # %d\n" % (s, i + 1))
+        w.write("  position: [ %18.14f,%18.14f,%18.14f ]\n" % tuple(v))
```

### Comparing `phono3py-2.9.2/phono3py/interface/alm.py` & `phono3py-3.0.0/phono3py/interface/alm.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/interface/calculator.py` & `phono3py-3.0.0/phono3py/interface/calculator.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/interface/fc_calculator.py` & `phono3py-3.0.0/phono3py/interface/fc_calculator.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/interface/phono3py_yaml.py` & `phono3py-3.0.0/phono3py/interface/phono3py_yaml.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/other/isotope.py` & `phono3py-3.0.0/phono3py/other/isotope.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,16 +30,17 @@
 # BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
 # LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
 # ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-import warnings
-from typing import Dict, List, Optional, Tuple, Union
+from __future__ import annotations
+
+from typing import Optional, Union
 
 import numpy as np
 from phonopy.harmonic.dynamical_matrix import get_dynamical_matrix
 from phonopy.phonon.tetrahedron_mesh import get_tetrahedra_frequencies
 from phonopy.structure.atoms import PhonopyAtoms
 from phonopy.structure.atoms import isotope_data as phonopy_isotope_data
 from phonopy.structure.cells import Primitive
@@ -54,16 +55,16 @@
 from phono3py.phonon.func import gaussian
 from phono3py.phonon.grid import BZGrid
 from phono3py.phonon.solver import run_phonon_solver_c, run_phonon_solver_py
 
 
 def get_mass_variances(
     primitive: Optional[PhonopyAtoms] = None,
-    symbols: Optional[Union[List[str], Tuple[str]]] = None,
-    isotope_data: Optional[Dict] = None,
+    symbols: Optional[Union[list[str], tuple[str]]] = None,
+    isotope_data: Optional[dict] = None,
 ):
     """Calculate mass variances."""
     if primitive is not None:
         _symbols = primitive.symbols
     elif symbols is not None:
         _symbols = symbols
     else:
@@ -172,22 +173,14 @@
     @sigma.setter
     def sigma(self, sigma):
         if sigma is None:
             self._sigma = None
         else:
             self._sigma = float(sigma)
 
-    def set_sigma(self, sigma):
-        """Set smearing width."""
-        warnings.warn(
-            "Isotope.set_sigma() is deprecated." "Use Isotope.sigma attribute.",
-            DeprecationWarning,
-        )
-        self.sigma = sigma
-
     @property
     def dynamical_matrix(self):
         """Return DynamicalMatrix* class instance."""
         return self._dm
 
     @property
     def band_indices(self):
@@ -195,41 +188,24 @@
         return self._band_indices
 
     @property
     def gamma(self):
         """Return scattering strength."""
         return self._gamma
 
-    def get_gamma(self):
-        """Return scattering strength."""
-        warnings.warn(
-            "Isotope.get_gamma() is deprecated." "Use Isotope.gamma attribute.",
-            DeprecationWarning,
-        )
-        return self.gamma
-
     @property
     def bz_grid(self):
         """Return BZgrid class instance."""
         return self._bz_grid
 
     @property
     def mass_variances(self):
         """Return mass variances."""
         return self._mass_variances
 
-    def get_mass_variances(self):
-        """Return mass variances."""
-        warnings.warn(
-            "Isotope.get_mass_variances() is deprecated."
-            "Use Isotope.mass_variances attribute.",
-            DeprecationWarning,
-        )
-        return self.mass_variances
-
     def get_phonons(self):
         """Return phonons on grid."""
         return self._frequencies, self._eigenvectors, self._phonon_done
 
     def set_phonons(self, frequencies, eigenvectors, phonon_done, dm=None):
         """Set phonons on grid."""
         self._frequencies = frequencies
@@ -252,15 +228,14 @@
         self._dm = get_dynamical_matrix(
             fc2,
             supercell,
             primitive,
             nac_params=nac_params,
             frequency_scale_factor=frequency_scale_factor,
             decimals=decimals,
-            symprec=self._symprec,
         )
 
     def set_nac_q_direction(self, nac_q_direction=None):
         """Set q-direction at q->0 used for NAC."""
         if nac_q_direction is not None:
             self._nac_q_direction = np.array(nac_q_direction, dtype="double")
```

### Comparing `phono3py-2.9.2/phono3py/other/kaccum.py` & `phono3py-3.0.0/phono3py/other/kaccum.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,74 @@
 """Calculated accumulated property with respect to other property."""
 
-from typing import Optional
+from __future__ import annotations
+
+from collections.abc import Sequence
+from typing import Optional, Union
 
 import numpy as np
 from phonopy.phonon.dos import NormalDistribution
 
 from phono3py.other.tetrahedron_method import get_integration_weights
 from phono3py.phonon.grid import BZGrid
 
 epsilon = 1.0e-8
 
 
-class KappaDOS:
-    """Class to calculate thermal conductivity spectram."""
+class KappaDOSTHM:
+    """Class to calculate DOS like spectram with tetrahedron method.
+
+    To compute usual DOS,
+
+    kappados = KappaDOSTHM(
+        np.ones(freqs.shape)[None, :, :, None],
+        freqs,
+        bzgrid,
+        ir_grid_points,
+        ir_grid_weights=ir_weights,
+        ir_grid_map=ir_grid_map,
+        num_sampling_points=201
+    )
+
+    """
 
     def __init__(
         self,
-        mode_kappa,
-        frequencies,
+        mode_kappa: np.ndarray,
+        frequencies: np.ndarray,
         bz_grid: BZGrid,
-        ir_grid_points,
-        ir_grid_map=None,
-        frequency_points=None,
-        num_sampling_points=100,
+        ir_grid_points: np.ndarray,
+        ir_grid_weights: Optional[np.ndarray] = None,
+        ir_grid_map: Optional[np.ndarray] = None,
+        frequency_points: Optional[Union[np.ndarray, Sequence]] = None,
+        num_sampling_points: int = 100,
     ):
         """Init method.
 
+        Parameters
+        ----------
         mode_kappa : ndarray
             Target value.
             shape=(temperatures, ir_grid_points, num_band, num_elem),
             dtype='double'
         frequencies : ndarray
+            Frequencies at ir-grid points.
             shape=(ir_grid_points, num_band), dtype='double'
         bz_grid : BZGrid
         ir_grid_points : ndarray
-            Ir-grid point indices in BZ-grid.
-            shape=(ir_grid_points, ), dtype='int_'
-        ir_grid_map : ndarray, optional, default=None
-            Mapping table to ir-grid point indices in GR-grid.
-            None gives `np.arange(len(frequencies), 'int_')`.
+            Irreducible grid point indices in GR-grid.
+            shape=(num_ir_grid_points, ), dtype='int_'
+        ir_grid_weights : ndarray
+            Weights of irreducible grid points. Its sum is the number of
+            grid points in GR-grid (prod(D_diag)).
+            shape=(num_ir_grid_points, ), dtype='int_'
+        ir_grid_map : ndarray
+            Index mapping table to irreducible grid points from all grid points
+            such as, [0, 0, 2, 3, 3, ...].
+            shape=(prod(D_diag), ), dtype='int_'
         frequency_points : array_like, optional, default=None
             This is used as the frequency points. When None,
             frequency points are created from `num_sampling_points`.
         num_sampling_points : int, optional, default=100
             Number of uniform sampling points.
 
         """
@@ -60,26 +86,30 @@
             (n_temp, len(self._frequency_points), 2, n_elem), dtype="double"
         )
 
         if ir_grid_map is None:
             bzgp2irgp_map = None
         else:
             bzgp2irgp_map = self._get_bzgp2irgp_map(bz_grid, ir_grid_map)
+        if ir_grid_weights is None:
+            grid_weights = np.ones(mode_kappa.shape[1])
+        else:
+            grid_weights = ir_grid_weights
         for j, function in enumerate(("J", "I")):
             iweights = get_integration_weights(
                 self._frequency_points,
                 frequencies,
                 bz_grid,
-                grid_points=ir_grid_points,
+                grid_points=bz_grid.grg2bzg[ir_grid_points],
                 bzgp2irgp_map=bzgp2irgp_map,
                 function=function,
             )
             for i, iw in enumerate(iweights):
                 self._kdos[:, :, j] += np.transpose(
-                    np.dot(iw, mode_kappa[:, i]), axes=(1, 0, 2)
+                    np.dot(iw, mode_kappa[:, i] * grid_weights[i]), axes=(1, 0, 2)
                 )
         self._kdos /= np.prod(bz_grid.D_diag)
 
     def get_kdos(self):
         """Return thermal conductivity spectram.
 
         Returns
@@ -175,48 +205,72 @@
 
 
 def run_prop_dos(
     frequencies,
     mode_prop,
     ir_grid_map,
     ir_grid_points,
-    num_sampling_points,
+    num_sampling_points: int,
     bz_grid: BZGrid,
 ):
-    """Run DOS-like calculation."""
-    kappa_dos = KappaDOS(
+    """Run DOS-like calculation.
+
+    This is a simple wrapper of KappsDOSTHM.
+
+    Parameters
+    ----------
+    frequencies:
+        Frequencies at ir-grid points.
+    mode_prop:
+        Properties at  ir-grid points.
+    ir_grid_map:
+        Obtained by get_ir_grid_points(bz_grid)[2].
+    ir_grid_points:
+        Obtained by get_ir_grid_points(bz_grid)[0].
+    num_sampling_points:
+        Number of sampling points in horizontal axis.
+    bz_grid:
+        BZ grid.
+
+    """
+    kappa_dos = KappaDOSTHM(
         mode_prop,
         frequencies,
         bz_grid,
-        ir_grid_points,
+        bz_grid.bzg2grg[ir_grid_points],
         ir_grid_map=ir_grid_map,
         num_sampling_points=num_sampling_points,
     )
     freq_points, kdos = kappa_dos.get_kdos()
     sampling_points = np.tile(freq_points, (len(kdos), 1))
     return kdos, sampling_points
 
 
 def run_mfp_dos(
-    mean_freepath, mode_prop, ir_grid_map, ir_grid_points, num_sampling_points, bz_grid
+    mean_freepath,
+    mode_prop,
+    ir_grid_map,
+    ir_grid_points,
+    num_sampling_points: int,
+    bz_grid: BZGrid,
 ):
     """Run DOS-like calculation for mean free path.
 
     mean_freepath : shape=(temperatures, ir_grid_points, 6)
     mode_prop : shape=(temperatures, ir_grid_points, 6, 6)
 
     """
     kdos = []
     sampling_points = []
     for i, _ in enumerate(mean_freepath):
-        kappa_dos = KappaDOS(
+        kappa_dos = KappaDOSTHM(
             mode_prop[i : i + 1, :, :],
             mean_freepath[i],
             bz_grid,
-            ir_grid_points,
+            bz_grid.bzg2grg[ir_grid_points],
             ir_grid_map=ir_grid_map,
             num_sampling_points=num_sampling_points,
         )
         sampling_points_at_T, kdos_at_T = kappa_dos.get_kdos()
         kdos.append(kdos_at_T[0])
         sampling_points.append(sampling_points_at_T)
     kdos = np.array(kdos)
```

### Comparing `phono3py-2.9.2/phono3py/other/tetrahedron_method.py` & `phono3py-3.0.0/phono3py/other/tetrahedron_method.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/phonon/func.py` & `phono3py-3.0.0/phono3py/phonon/func.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/phonon/grid.py` & `phono3py-3.0.0/phono3py/phonon/grid.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/phonon/group_velocity_matrix.py` & `phono3py-3.0.0/phono3py/phonon/group_velocity_matrix.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/phonon/heat_capacity_matrix.py` & `phono3py-3.0.0/phono3py/phonon/heat_capacity_matrix.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/phonon/solver.py` & `phono3py-3.0.0/phono3py/phonon/solver.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/phonon/velocity_operator.py` & `phono3py-3.0.0/phono3py/phonon/velocity_operator.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/phonon3/collision_matrix.py` & `phono3py-3.0.0/phono3py/phonon3/collision_matrix.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/phonon3/dataset.py` & `phono3py-3.0.0/phono3py/phonon3/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,16 +43,15 @@
     Note
     ----
     Dipslacements and forces of all atoms in supercells are returned.
 
     Parameters
     ----------
     disp_dataset : dict
-        Displacement dataset that may be obtained by
-        file_IO.parse_disp_fc3_yaml.
+        Displacement dataset.
 
     Returns
     -------
     displacements : ndarray
         Displacements of all atoms in all supercells.
         shape=(snapshots, supercell atoms, 3), dtype='double', order='C'
     forces : ndarray or None
```

### Comparing `phono3py-2.9.2/phono3py/phonon3/displacement_fc3.py` & `phono3py-3.0.0/phono3py/phonon3/displacement_fc3.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/phonon3/fc3.py` & `phono3py-3.0.0/phono3py/phonon3/fc3.py`

 * *Files 1% similar despite different names*

```diff
@@ -688,15 +688,15 @@
     if is_compact_fc:
         num_patom = len(primitive)
         s2p_map = primitive.s2p_map
         p2p_map = primitive.p2p_map
         first_atom_nums = []
         for i in unique_first_atom_nums:
             if i != s2p_map[i]:
-                print("Something wrong in disp_fc3.yaml")
+                print("Something wrong in displacement dataset.")
                 raise RuntimeError
             else:
                 first_atom_nums.append(i)
         fc3 = np.zeros(
             (num_patom, num_satom, num_satom, 3, 3, 3), dtype="double", order="C"
         )
     else:
```

### Comparing `phono3py-2.9.2/phono3py/phonon3/gruneisen.py` & `phono3py-3.0.0/phono3py/phonon3/gruneisen.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,14 @@
         self._factor = factor
         self._symprec = symprec
         self._dm = get_dynamical_matrix(
             self._fc2,
             self._scell,
             self._pcell,
             nac_params=nac_params,
-            symprec=self._symprec,
         )
         self._nac_q_direction = nac_q_direction
 
         self._svecs, self._multi = self._pcell.get_smallest_vectors()
 
         if self._ion_clamped:
             num_atom_prim = len(self._pcell)
```

### Comparing `phono3py-2.9.2/phono3py/phonon3/imag_self_energy.py` & `phono3py-3.0.0/phono3py/phonon3/imag_self_energy.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/phonon3/interaction.py` & `phono3py-3.0.0/phono3py/phonon3/interaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -667,15 +667,14 @@
         self._dm = get_dynamical_matrix(
             fc2,
             supercell,
             primitive,
             nac_params=nac_params,
             frequency_scale_factor=self._frequency_scale_factor,
             decimals=decimals,
-            symprec=self._symprec,
         )
         self._allocate_phonon()
 
     def set_phonon_data(self, frequencies, eigenvectors, bz_grid_addresses):
         """Set phonons on grid."""
         if bz_grid_addresses.shape != self._bz_grid.addresses.shape:
             raise RuntimeError(
```

### Comparing `phono3py-2.9.2/phono3py/phonon3/joint_dos.py` & `phono3py-3.0.0/phono3py/phonon3/joint_dos.py`

 * *Files 1% similar despite different names*

```diff
@@ -413,15 +413,14 @@
     def _init_dynamical_matrix(self):
         self._dm = get_dynamical_matrix(
             self._fc2,
             self._supercell,
             self._primitive,
             nac_params=self._nac_params,
             frequency_scale_factor=self._frequency_scale_factor,
-            symprec=self._symprec,
         )
         self._allocate_phonons()
 
     def _set_triplets(self):
         if not self._is_mesh_symmetry:
             if self._log_level:
                 print("Triplets at q without considering symmetry")
```

### Comparing `phono3py-2.9.2/phono3py/phonon3/real_self_energy.py` & `phono3py-3.0.0/phono3py/phonon3/real_self_energy.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/phonon3/real_to_reciprocal.py` & `phono3py-3.0.0/phono3py/phonon3/real_to_reciprocal.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/phonon3/reciprocal_to_normal.py` & `phono3py-3.0.0/phono3py/phonon3/reciprocal_to_normal.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/phonon3/spectral_function.py` & `phono3py-3.0.0/phono3py/phonon3/spectral_function.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/phonon3/triplets.py` & `phono3py-3.0.0/phono3py/phonon3/triplets.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/sscha/sscha.py` & `phono3py-3.0.0/phono3py/sscha/sscha.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/phono3py/version.py` & `phono3py-3.0.0/phono3py/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,8 +30,8 @@
 # BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
 # LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
 # ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "2.9.2"
+__version__ = "3.0.0"
```

### Comparing `phono3py-2.9.2/phono3py.egg-info/SOURCES.txt` & `phono3py-3.0.0/phono3py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/scripts/phono3py` & `phono3py-3.0.0/scripts/phono3py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/scripts/phono3py-coleigplot` & `phono3py-3.0.0/scripts/phono3py-coleigplot`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/scripts/phono3py-kaccum` & `phono3py-3.0.0/scripts/phono3py-kaccum`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/scripts/phono3py-kdeplot` & `phono3py-3.0.0/scripts/phono3py-kdeplot`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/scripts/phono3py-load` & `phono3py-3.0.0/scripts/phono3py-load`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/setup.py` & `phono3py-3.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,15 +316,15 @@
         install_requires=[
             "numpy>=1.17.0",
             "scipy",
             "PyYAML>=5.3",
             "matplotlib>=2.2.2",
             "h5py>=3.0",
             "spglib>=2.0",
-            "phonopy>=2.21,<2.22",
+            "phonopy>=2.22,<2.23",
         ],
         provides=["phono3py"],
         scripts=scripts_phono3py,
         ext_modules=_get_extensions(build_dir),
     )
     _clean_cmake(build_dir)
```

### Comparing `phono3py-2.9.2/test/AgNO2_cell.yaml` & `phono3py-3.0.0/test/AgNO2_cell.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/FORCES_FC3_si_pbesol` & `phono3py-3.0.0/test/FORCES_FC3_si_pbesol`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/FORCE_SETS_NaCl` & `phono3py-3.0.0/test/FORCE_SETS_NaCl`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/api/test_api_phono3py.py` & `phono3py-3.0.0/test/api/test_api_phono3py.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/conductivity/test_kappa_LBTE.py` & `phono3py-3.0.0/test/conductivity/test_kappa_LBTE.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/conductivity/test_kappa_LBTE_Wigner.py` & `phono3py-3.0.0/test/conductivity/test_kappa_LBTE_Wigner.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/conductivity/test_kappa_RTA.py` & `phono3py-3.0.0/test/conductivity/test_kappa_RTA.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/conductivity/test_kappa_RTA_Wigner.py` & `phono3py-3.0.0/test/conductivity/test_kappa_RTA_Wigner.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/conftest.py` & `phono3py-3.0.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/cui/phono3py_params-qe-Si222.yaml.xz` & `phono3py-3.0.0/test/cui/phono3py_params-qe-Si222.yaml.xz`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/cui/test_phono3py_load_script.py` & `phono3py-3.0.0/test/cui/test_phono3py_load_script.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/file_IO/test_file_IO.py` & `phono3py-3.0.0/test/file_IO/test_file_IO.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/interface/test_phono3py_yaml.py` & `phono3py-3.0.0/test/interface/test_phono3py_yaml.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/other/test_isotope.py` & `phono3py-3.0.0/test/other/test_isotope.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/other/test_kaccum.py` & `phono3py-3.0.0/test/other/test_kaccum.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 """Test for kaccum.py."""
 
+from __future__ import annotations
+
+from typing import Optional
+
 import numpy as np
 
 from phono3py import Phono3py
-from phono3py.other.kaccum import GammaDOSsmearing, KappaDOS, get_mfp
+from phono3py.other.kaccum import (
+    GammaDOSsmearing,
+    KappaDOSTHM,
+    get_mfp,
+    run_mfp_dos,
+    run_prop_dos,
+)
 from phono3py.phonon.grid import get_ir_grid_points
 
 
 def test_kappados_si(si_pbesol: Phono3py):
     """Test KappaDOS class with Si.
 
     * 3x3 tensor vs frequency
@@ -97,24 +107,28 @@
         temperatures=[
             300,
         ]
     )
     tc = ph3.thermal_conductivity
     freq_points_in = np.array(kappados_si).reshape(-1, 3)[:, 0]
     freq_points, kdos = _calculate_kappados(
-        ph3, tc.mode_kappa[0], freq_points=freq_points_in
+        ph3,
+        tc.mode_kappa[0],
+        freq_points=freq_points_in,
     )
     # for f, (jval, ival) in zip(freq_points, kdos):
     #     print("[%.7f, %.7f, %.7f]," % (f, jval, ival))
     np.testing.assert_allclose(
         kappados_si, np.vstack((freq_points, kdos.T)).T, rtol=0, atol=0.5
     )
 
     freq_points, kdos = _calculate_kappados(
-        ph3, tc.gamma[0, :, :, :, None], freq_points=freq_points_in
+        ph3,
+        tc.gamma[0, :, :, :, None],
+        freq_points=freq_points_in,
     )
     # for f, (jval, ival) in zip(freq_points, kdos):
     #     print("[%.7f, %.7f, %.7f]," % (f, jval, ival))
     np.testing.assert_allclose(
         gammados_si, np.vstack((freq_points, kdos.T)).T, rtol=0, atol=1e-4
     )
 
@@ -226,15 +240,17 @@
     # for f, (jval, ival) in zip(freq_points, kdos):
     #     print("[%.7f, %.7f, %.7f]," % (f, jval, ival))
     np.testing.assert_allclose(
         kappados_nacl, np.vstack((freq_points, kdos.T)).T, rtol=0, atol=0.5
     )
 
     freq_points, kdos = _calculate_kappados(
-        ph3, tc.gamma[0, :, :, :, None], freq_points=freq_points_in
+        ph3,
+        tc.gamma[0, :, :, :, None],
+        freq_points=freq_points_in,
     )
     for f, (jval, ival) in zip(freq_points, kdos):
         print("[%.7f, %.7f, %.7f]," % (f, jval, ival))
     np.testing.assert_allclose(
         gammados_nacl, np.vstack((freq_points, kdos.T)).T, rtol=0, atol=1e-4
     )
 
@@ -277,50 +293,149 @@
     ]
 
     np.testing.assert_allclose(
         np.c_[fpoints, gdos_vals[0, :, 1]], gdos_ref, rtol=0, atol=1e-5
     )
 
 
-def _calculate_kappados(ph3: Phono3py, mode_prop, freq_points=None):
-    tc = ph3.thermal_conductivity
+def test_run_prop_dos(si_pbesol: Phono3py):
+    ph3 = si_pbesol
+    ph3.mesh_numbers = [7, 7, 7]
+    ph3.init_phph_interaction()
+    ph3.run_thermal_conductivity(
+        temperatures=[
+            300,
+        ]
+    )
     bz_grid = ph3.grid
-    frequencies, _, _ = ph3.get_phonon_data()
-    kappados = KappaDOS(
-        mode_prop, frequencies, bz_grid, tc.grid_points, frequency_points=freq_points
+    ir_grid_points, _, ir_grid_map = get_ir_grid_points(bz_grid)
+    tc = ph3.thermal_conductivity
+
+    kdos, sampling_points = run_prop_dos(
+        tc.frequencies, tc.mode_kappa[0], ir_grid_map, ir_grid_points, 10, bz_grid
     )
-    freq_points, kdos = kappados.get_kdos()
+    mean_freepath = get_mfp(tc.gamma[0], tc.group_velocities)
+    mfp, sampling_points_mfp = run_mfp_dos(
+        mean_freepath, tc.mode_kappa[0], ir_grid_map, ir_grid_points, 10, bz_grid
+    )
+
+    # print(",".join([f"{v:10.5f}" for v in kdos[0, :, :, 0].ravel()]))
+    ref_kdos = [
+        0.00000,
+        0.00000,
+        2.19162,
+        5.16697,
+        28.22125,
+        18.97280,
+        58.56343,
+        12.19206,
+        69.05896,
+        3.47035,
+        73.17626,
+        1.48915,
+        74.74544,
+        0.43485,
+        75.87064,
+        1.74135,
+        79.08179,
+        2.30428,
+        81.21678,
+        0.00000,
+    ]
+    # print(",".join([f"{v:10.5f}" for v in mfp[0, :, :, 0].ravel()]))
+    ref_mfp = [
+        0.00000,
+        0.00000,
+        29.19150,
+        0.02604,
+        42.80717,
+        0.01202,
+        52.09457,
+        0.01158,
+        61.79908,
+        0.01140,
+        69.49177,
+        0.00784,
+        74.57499,
+        0.00501,
+        77.99145,
+        0.00364,
+        80.33477,
+        0.00210,
+        81.21678,
+        0.00000,
+    ]
+    # print(",".join([f"{v:10.5f}" for v in sampling_points[0]]))
+    ref_sampling_points = [
+        -0.00000,
+        1.69664,
+        3.39328,
+        5.08992,
+        6.78656,
+        8.48320,
+        10.17984,
+        11.87648,
+        13.57312,
+        15.26976,
+    ]
+    # print(",".join([f"{v:10.5f}" for v in sampling_points_mfp[0]]))
+    ref_sampling_points_mfp = [
+        0.00000,
+        803.91710,
+        1607.83420,
+        2411.75130,
+        3215.66841,
+        4019.58551,
+        4823.50261,
+        5627.41971,
+        6431.33681,
+        7235.25391,
+    ]
+    np.testing.assert_allclose(ref_kdos, kdos[0, :, :, 0].ravel(), atol=0.5)
+    np.testing.assert_allclose(ref_mfp, mfp[0, :, :, 0].ravel(), atol=0.5)
+    np.testing.assert_allclose(ref_sampling_points, sampling_points[0], atol=1e-4)
+    np.testing.assert_allclose(ref_sampling_points_mfp, sampling_points_mfp[0], rtol=10)
+
 
+def _calculate_kappados(
+    ph3: Phono3py,
+    mode_prop: np.ndarray,
+    freq_points: Optional[np.ndarray] = None,
+):
+    tc = ph3.thermal_conductivity
+    bz_grid = ph3.grid
     ir_grid_points, _, ir_grid_map = get_ir_grid_points(bz_grid)
-    kappados = KappaDOS(
+    kappados = KappaDOSTHM(
         mode_prop,
         tc.frequencies,
         bz_grid,
-        tc.grid_points,
+        bz_grid.bzg2grg[tc.grid_points],
         ir_grid_map=ir_grid_map,
         frequency_points=freq_points,
     )
     ir_freq_points, ir_kdos = kappados.get_kdos()
     np.testing.assert_equal(bz_grid.bzg2grg[tc.grid_points], ir_grid_points)
     np.testing.assert_allclose(ir_freq_points, freq_points, rtol=0, atol=1e-5)
-    np.testing.assert_allclose(ir_kdos, kdos, rtol=0, atol=1e-5)
 
-    return freq_points, kdos[0, :, :, 0]
+    return freq_points, ir_kdos[0, :, :, 0]
 
 
-def _calculate_mfpdos(ph3: Phono3py, mfp_points=None):
+def _calculate_mfpdos(
+    ph3: Phono3py,
+    mfp_points=None,
+):
     tc = ph3.thermal_conductivity
     bz_grid = ph3.grid
     mean_freepath = get_mfp(tc.gamma[0], tc.group_velocities)
     _, _, ir_grid_map = get_ir_grid_points(bz_grid)
-    mfpdos = KappaDOS(
+    mfpdos = KappaDOSTHM(
         tc.mode_kappa[0],
         mean_freepath[0],
         bz_grid,
-        tc.grid_points,
+        bz_grid.bzg2grg[tc.grid_points],
         ir_grid_map=ir_grid_map,
         frequency_points=mfp_points,
         num_sampling_points=10,
     )
     freq_points, kdos = mfpdos.get_kdos()
 
     return freq_points, kdos[0, :, :, 0]
```

### Comparing `phono3py-2.9.2/test/phono3py_params-Si111-rd.yaml.xz` & `phono3py-3.0.0/test/phono3py_params-Si111-rd.yaml.xz`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/phono3py_params_AlN332.yaml.xz` & `phono3py-3.0.0/test/phono3py_params_AlN332.yaml.xz`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/phono3py_params_NaCl111.yaml` & `phono3py-3.0.0/test/phono3py_params_NaCl111.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/phono3py_params_NaCl222.yaml.xz` & `phono3py-3.0.0/test/phono3py_params_NaCl222.yaml.xz`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/phono3py_params_Si-111-222.yaml` & `phono3py-3.0.0/test/phono3py_params_Si-111-222.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/phono3py_params_Si111.yaml` & `phono3py-3.0.0/test/phono3py_params_Si111.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/phono3py_si_pbesol.yaml` & `phono3py-3.0.0/test/phono3py_si_pbesol.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/phonon/test_grid.py` & `phono3py-3.0.0/test/phonon/test_grid.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/phonon/test_velocity_operator.py` & `phono3py-3.0.0/test/phonon/test_velocity_operator.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
     )
 
     gv_operator = VelocityOperator(
         ph_nacl.dynamical_matrix, symmetry=ph_nacl.primitive_symmetry
     )
 
     # we chose an 'ugly' q-point because we want to avoid degeneracies.
-    ph_nacl.dynamical_matrix.run([[0.1, 0.22, 0.33]])
+    ph_nacl.dynamical_matrix.run([0.1, 0.22, 0.33])
     dm = ph_nacl.dynamical_matrix.dynamical_matrix
     eigvals, eigvecs = np.linalg.eigh(dm)
 
     np.testing.assert_allclose(
         eigvals * VaspToTHz * THzToCm,
         eigvals_NaCl_Ref,
         atol=0.00001,
```

### Comparing `phono3py-2.9.2/test/phonon3/test_displacements.py` & `phono3py-3.0.0/test/phonon3/test_displacements.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/phonon3/test_fc3.py` & `phono3py-3.0.0/test/phonon3/test_fc3.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/phonon3/test_imag_self_energy.py` & `phono3py-3.0.0/test/phonon3/test_imag_self_energy.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/phonon3/test_interaction.py` & `phono3py-3.0.0/test/phonon3/test_interaction.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/phonon3/test_joint_dos.py` & `phono3py-3.0.0/test/phonon3/test_joint_dos.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/phonon3/test_real_self_energy.py` & `phono3py-3.0.0/test/phonon3/test_real_self_energy.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/phonon3/test_spectral_function.py` & `phono3py-3.0.0/test/phonon3/test_spectral_function.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/phonon3/test_triplets.py` & `phono3py-3.0.0/test/phonon3/test_triplets.py`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/phonopy_disp_NaCl.yaml` & `phono3py-3.0.0/test/phonopy_disp_NaCl.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/phonopy_params-Si111-iterha.yaml.gz` & `phono3py-3.0.0/test/phonopy_params-Si111-iterha.yaml.gz`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/phonopy_params_Si.yaml` & `phono3py-3.0.0/test/phonopy_params_Si.yaml`

 * *Files identical despite different names*

### Comparing `phono3py-2.9.2/test/sscha/test_sscha.py` & `phono3py-3.0.0/test/sscha/test_sscha.py`

 * *Files identical despite different names*

