# Comparing `tmp/corecon-1.3.tar.gz` & `tmp/corecon-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/corecon-1.3.tar", last modified: Wed Feb 21 15:40:57 2024, max compression
+gzip compressed data, was "dist/corecon-1.4.tar", last modified: Sat Apr 20 17:34:28 2024, max compression
```

## Comparing `corecon-1.3.tar` & `corecon-1.4.tar`

### file list

```diff
@@ -1,246 +1,278 @@
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/
--rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)    34444 2020-05-11 19:32:45.000000 corecon-1.3/LICENSE.txt
--rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)      116 2020-05-11 19:32:45.000000 corecon-1.3/MANIFEST.in
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1940 2024-02-21 15:40:57.000000 corecon-1.3/PKG-INFO
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      900 2023-07-07 14:08:22.000000 corecon-1.3/README.md
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/corecon/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     9015 2023-06-19 16:03:09.000000 corecon-1.3/corecon/DataEntryClass.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     8225 2023-07-05 12:35:41.000000 corecon-1.3/corecon/FieldClass.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1802 2023-06-19 16:03:09.000000 corecon-1.3/corecon/InternalFunctions.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     6010 2023-06-19 16:03:09.000000 corecon-1.3/corecon/__init__.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2176 2023-06-19 16:03:09.000000 corecon-1.3/corecon/check_updates.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/corecon/data/
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/corecon/data/HeII_to_HI_column_density_ratio/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    19889 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/HeII_to_HI_column_density_ratio/Syphers_and_Shull_2014.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.3/corecon/data/HeII_to_HI_column_density_ratio/__init__.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/corecon/data/IGM_temperature_mean_density/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1104 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/IGM_temperature_mean_density/Becker_et_al_2011.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      964 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/IGM_temperature_mean_density/Boera_et_al_2014.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      830 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/IGM_temperature_mean_density/Boera_et_al_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      754 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/IGM_temperature_mean_density/Bolton_et_al_2010.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      792 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/IGM_temperature_mean_density/Bolton_et_al_2012.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      885 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/IGM_temperature_mean_density/Bolton_et_al_2014.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      918 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/IGM_temperature_mean_density/Gaikwad_et_al_2020.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1332 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/IGM_temperature_mean_density/Gaikwad_et_al_2021.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      885 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/IGM_temperature_mean_density/Garzilli_et_al_2012.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1145 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/IGM_temperature_mean_density/Hiss_et_al_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      970 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/IGM_temperature_mean_density/Lidz_et_al_2010.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1081 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/IGM_temperature_mean_density/Rorai_et_al_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1551 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/IGM_temperature_mean_density/Schaye_et_al_2010.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1579 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/IGM_temperature_mean_density/Walther_et_al_2019.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.3/corecon/data/IGM_temperature_mean_density/__init__.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/corecon/data/Lya_flux_power_spectrum/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     5003 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/Lya_flux_power_spectrum/Croft_et_al_2002.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2674 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/Lya_flux_power_spectrum/DAloisio_et_al_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     9025 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/Lya_flux_power_spectrum/McDonald_et_al_2006.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    26999 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/Lya_flux_power_spectrum/Palanque-Delabrouille_et_al_2013_fourier.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    25486 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/Lya_flux_power_spectrum/Palanque-Delabrouille_et_al_2013_likelihood.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.3/corecon/data/Lya_flux_power_spectrum/__init__.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/corecon/data/Lya_spike_galaxy_correlation/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2219 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/Lya_spike_galaxy_correlation/Kakiichi_et_al_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     6447 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/Lya_spike_galaxy_correlation/Kashino_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1530 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/Lya_spike_galaxy_correlation/Meyer_et_al_2019.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     3433 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/Lya_spike_galaxy_correlation/Meyer_et_al_2020.py
--rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)        0 2020-06-27 13:38:09.000000 corecon-1.3/corecon/data/Lya_spike_galaxy_correlation/__init__.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/corecon/data/UV_luminosity_density/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      599 2024-02-21 14:56:31.000000 corecon-1.3/corecon/data/UV_luminosity_density/Adams_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      694 2024-02-21 14:57:29.000000 corecon-1.3/corecon/data/UV_luminosity_density/Bouwens_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      505 2024-02-21 14:57:29.000000 corecon-1.3/corecon/data/UV_luminosity_density/Donnan_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      566 2024-02-21 14:57:29.000000 corecon-1.3/corecon/data/UV_luminosity_density/Finkelstein_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      640 2024-02-21 14:57:29.000000 corecon-1.3/corecon/data/UV_luminosity_density/Harikane_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      505 2024-02-21 14:57:29.000000 corecon-1.3/corecon/data/UV_luminosity_density/McLeod_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      675 2024-02-21 14:57:29.000000 corecon-1.3/corecon/data/UV_luminosity_density/Perez-Gonzales_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      626 2024-02-21 14:57:29.000000 corecon-1.3/corecon/data/UV_luminosity_density/Willot_et_al_2023.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/corecon/data/UV_luminosity_function/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1828 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_luminosity_function/Atek_et_al_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1785 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_luminosity_function/Atek_et_al_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     5909 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_luminosity_function/Bouwens_et_al_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1229 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_luminosity_function/Bouwens_et_al_2016.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1813 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_luminosity_function/Bouwens_et_al_2017.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1038 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_luminosity_function/Bouwens_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1129 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_luminosity_function/Bowler_et_al_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1070 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_luminosity_function/Bowler_et_al_2020.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      898 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_luminosity_function/Castellano_et_al_2016.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1970 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_luminosity_function/Donnan_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     5256 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_luminosity_function/Finkelstein_et_al_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      848 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_luminosity_function/Finkelstein_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1976 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_luminosity_function/Harikane_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     4562 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_luminosity_function/Ishigaki_et_al_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1170 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_luminosity_function/Kauffmann_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     4335 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_luminosity_function/Livermore_et_al_2017.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1075 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_luminosity_function/McLeod_et_al_2016.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1984 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_luminosity_function/McLure_et_al_2013.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      889 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_luminosity_function/Morishita_et_al_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      888 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_luminosity_function/Naidu_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1235 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_luminosity_function/Oesch_et_al_2014.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1283 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_luminosity_function/Rojas-Ruiz_et_al_2020.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1217 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_luminosity_function/Stefanon_et_al_2019.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.3/corecon/data/UV_luminosity_function/__init__.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/corecon/data/UV_slope/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1511 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_slope/Atek_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     3110 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_slope/Austin_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2565 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_slope/Bouwens_et_al_2009.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     4278 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_slope/Cullen_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1106 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_slope/Curtis-Lake_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     8626 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_slope/Endsley_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)   243506 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_slope/Finkelstein_et_al_2012.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2525 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_slope/Franco_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2242 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_slope/Simmonds_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1950 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_slope/Tacchella_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      922 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_slope/Topping_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1210 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_slope/Whitler_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     3277 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/UV_slope/Whitler_et_al_2023.py
--rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)        0 2020-05-11 19:32:45.000000 corecon-1.3/corecon/data/__init__.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      507 2023-06-19 16:03:09.000000 corecon-1.3/corecon/data/data_entry_template.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/corecon/data/dust_mass/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      843 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/dust_mass/Laporte_et_al_2017.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/corecon/data/effective_optical_depth_HI_Lya/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     5850 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/effective_optical_depth_HI_Lya/Becker_et_al_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    16176 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/effective_optical_depth_HI_Lya/Bosman_et_al_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    29333 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/effective_optical_depth_HI_Lya/Bosman_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     7910 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/effective_optical_depth_HI_Lya/Eilers+18.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     6987 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/effective_optical_depth_HI_Lya/Fan_et_al_2006.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     4116 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/effective_optical_depth_HI_Lya/Liu_Bordoloi_2021.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    11861 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/effective_optical_depth_HI_Lya/Yang_et_al_2020.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.3/corecon/data/effective_optical_depth_HI_Lya/__init__.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/corecon/data/effective_optical_depth_HeII_Lya/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     6007 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/effective_optical_depth_HeII_Lya/Worseck_et_al_2016.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.3/corecon/data/effective_optical_depth_HeII_Lya/__init__.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/corecon/data/galaxy_main_sequence/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2019 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/galaxy_main_sequence/Chen_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      867 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/galaxy_main_sequence/Finkelstein_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1642 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/galaxy_main_sequence/Leethochawali_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2885 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/galaxy_main_sequence/Roberts-Borsani_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1538 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/galaxy_main_sequence/Stefanon_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1863 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/galaxy_main_sequence/Tacchella_et_al_2022.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/corecon/data/ionized_fraction/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      689 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Bolton_et_al_2011.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1129 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Bosman_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      710 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Chornock_et_al_2013.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      729 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Choudhury_et_al_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      910 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Choudhury_et_al_2021.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1247 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Davies_et_al_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      632 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Dijkstra_et_al_2011.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1105 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Fan_et_al_2006.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1401 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Gaikwad_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      661 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Greig_et_al_2017.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      664 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Greig_et_al_2019.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      695 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Hoag_et_al_2019.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      730 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Jensen_et_al_2013.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      868 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Jung_et_al_2020.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1391 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Lu_et_al_2020.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      635 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Mason_et_al_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      760 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Mason_et_al_2019.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      658 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/McGreer_et_al_2011.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      674 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/McGreer_et_al_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      731 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Mesinger_et_al_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      657 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Mortlock_et_al_2011.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      684 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Ono_et_al_2012.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      699 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Ota_et_al_2008.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      927 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Ouchi_et_al_2010.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      957 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Pentericci_et_al_2014.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      922 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Robertson_et_al_2013.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      688 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Schenker_et_al_2014.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      678 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Schroeder_et_al_2013.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      661 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Sobacchi_Mesinger_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      936 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Tilvi_et_al_2014.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1094 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Totani_et_al_2006.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      872 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Wang_et_al_2020.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      791 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Yang_et_al_2020.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1126 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Yang_et_al_2020b.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      716 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionized_fraction/Zhu_et_al_2022.py
--rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)        0 2020-05-11 19:32:45.000000 corecon-1.3/corecon/data/ionized_fraction/__init__.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/corecon/data/ionizing_photons_emission_rate/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      643 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionizing_photons_emission_rate/Becker_et_al_2013.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      789 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionizing_photons_emission_rate/Becker_et_al_2021.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1746 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionizing_photons_emission_rate/Bouwens_et_al_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1311 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionizing_photons_emission_rate/Gaikwad_et_al_2023.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/corecon/data/ionizing_photons_production_efficiency/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1023 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionizing_photons_production_efficiency/Bouwens_et_al_2016.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      788 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionizing_photons_production_efficiency/Bunker_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1380 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionizing_photons_production_efficiency/Endsley_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      912 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionizing_photons_production_efficiency/Harikane_et_al_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      878 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionizing_photons_production_efficiency/Jung_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1124 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionizing_photons_production_efficiency/Lam_et_al_2019.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      788 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionizing_photons_production_efficiency/Maseda_et_al_2020.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    67827 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionizing_photons_production_efficiency/Prieto-Lyon_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1160 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionizing_photons_production_efficiency/Saxena_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2242 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/ionizing_photons_production_efficiency/Simmonds_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      724 2023-06-19 16:03:09.000000 corecon-1.3/corecon/data/make_data_archive.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/corecon/data/mass_gas_metallicity_relation/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      925 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/mass_gas_metallicity_relation/Boyett_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      900 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/mass_gas_metallicity_relation/Bunker_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      868 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/mass_gas_metallicity_relation/Curti_et_al_2023a.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1357 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/mass_gas_metallicity_relation/Faisst_et_al_2016.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1463 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/mass_gas_metallicity_relation/Fujimoto_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1793 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/mass_gas_metallicity_relation/Langeroodi_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    37184 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/mass_gas_metallicity_relation/Nakajima_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2834 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/mass_gas_metallicity_relation/Roberts-Borsani_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1076 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/mass_gas_metallicity_relation/Schaerer_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1097 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/mass_gas_metallicity_relation/Trump_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1038 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/mass_gas_metallicity_relation/Williams_et_al_2023.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/corecon/data/mass_stellar_metallicity_relation/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1948 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/mass_stellar_metallicity_relation/Furtak_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1690 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/mass_stellar_metallicity_relation/Tacchella_et_al_2022.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/corecon/data/mean_free_path/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      697 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/mean_free_path/Becker_et_al_2021.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      568 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/mean_free_path/Bosman_et_al_2021.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      643 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/mean_free_path/DAloisio_et_al_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      791 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/mean_free_path/Fumagalli_et_al_2013.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1192 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/mean_free_path/Gaikwad_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      783 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/mean_free_path/OMeara_et_al_2013.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      931 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/mean_free_path/Prochaska_et_al_2009.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      852 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/mean_free_path/Worseck_et_al_2014.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.3/corecon/data/mean_free_path/__init__.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/corecon/data/optical_depth_CMB/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1017 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/optical_depth_CMB/Pagani_et_al_2020.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      845 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/optical_depth_CMB/Paoletti_et_al_2020.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      850 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/optical_depth_CMB/Planck_2013.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      997 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/optical_depth_CMB/Planck_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1058 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/optical_depth_CMB/Planck_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      848 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/optical_depth_CMB/WMAP_5yr.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      840 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/optical_depth_CMB/WMAP_7yr.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      849 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/optical_depth_CMB/WMAP_9yr.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.3/corecon/data/optical_depth_CMB/__init__.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      860 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/optical_depth_CMB/deBelsunce_et_al_2021.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/corecon/data/photoionization_rate/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      608 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/photoionization_rate/Bolton_et_al_2007.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      796 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/photoionization_rate/Calverley_et_al_2011.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      807 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/photoionization_rate/DAloisio_et_al_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1311 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/photoionization_rate/Gaikwad_et_al_2023.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      678 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/photoionization_rate/Wyithe_et_al_2011.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/corecon/data/quasar_luminosity_function/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1348 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/quasar_luminosity_function/Giallongo_et_al_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1337 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/quasar_luminosity_function/Giallongo_et_al_2019.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1040 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/quasar_luminosity_function/Glikman_et_al_2011.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1147 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/quasar_luminosity_function/Jiang_et_al_2016.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      897 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/quasar_luminosity_function/Kashikawa_et_al_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    28572 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/quasar_luminosity_function/Kulkarni_et_al_2019.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1266 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/quasar_luminosity_function/McGreer_et_al_2013.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     4498 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/quasar_luminosity_function/Ross_et_al_2013.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1078 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/quasar_luminosity_function/Willott_et_al_2010.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1027 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/quasar_luminosity_function/Yang_et_al_2016.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.3/corecon/data/quasar_luminosity_function/__init__.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/corecon/data/reionization_midpoint/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      490 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/reionization_midpoint/Pagano_et_al_2020.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      500 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/reionization_midpoint/Paoletti_et_al_2020.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      472 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/reionization_midpoint/Planck_2013.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      477 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/reionization_midpoint/Planck_2015.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      477 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/reionization_midpoint/Planck_2018.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      499 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/reionization_midpoint/deBelsunce_et_al_2021.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/corecon/data/sfrd/
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      980 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/sfrd/Donnan_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      982 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/sfrd/Harikane_et_al_2022.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     4720 2024-02-21 14:34:54.000000 corecon-1.3/corecon/data/sfrd/Madau_and_Dickinson_2014.py
--rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)        0 2020-06-23 15:25:46.000000 corecon-1.3/corecon/data/sfrd/__init__.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     9559 2024-02-21 14:55:47.000000 corecon-1.3/corecon/fields_info.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     8799 2023-06-20 08:06:03.000000 corecon-1.3/corecon/loaders.py
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)       20 2024-02-21 14:57:57.000000 corecon-1.3/corecon/version.py
-drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-02-21 15:40:57.000000 corecon-1.3/corecon.egg-info/
--rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)     1940 2024-02-21 15:40:57.000000 corecon-1.3/corecon.egg-info/PKG-INFO
--rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)    11734 2024-02-21 15:40:57.000000 corecon-1.3/corecon.egg-info/SOURCES.txt
--rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)        1 2024-02-21 15:40:57.000000 corecon-1.3/corecon.egg-info/dependency_links.txt
--rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)        6 2024-02-21 15:40:57.000000 corecon-1.3/corecon.egg-info/requires.txt
--rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)        8 2024-02-21 15:40:57.000000 corecon-1.3/corecon.egg-info/top_level.txt
--rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)       79 2024-02-21 15:40:57.000000 corecon-1.3/setup.cfg
--rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1358 2023-06-19 16:03:09.000000 corecon-1.3/setup.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/
+-rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)    34444 2020-05-11 19:32:45.000000 corecon-1.4/LICENSE.txt
+-rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)      116 2020-05-11 19:32:45.000000 corecon-1.4/MANIFEST.in
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1991 2024-04-20 17:34:28.000000 corecon-1.4/PKG-INFO
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      900 2023-07-07 14:08:22.000000 corecon-1.4/README.md
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     9015 2024-04-19 11:08:32.000000 corecon-1.4/corecon/DataEntryClass.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     8225 2023-07-05 12:35:41.000000 corecon-1.4/corecon/FieldClass.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1802 2024-04-19 11:08:32.000000 corecon-1.4/corecon/InternalFunctions.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     6010 2024-04-19 11:08:32.000000 corecon-1.4/corecon/__init__.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2176 2023-06-19 16:03:09.000000 corecon-1.4/corecon/check_updates.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon/data/
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon/data/HII_fraction/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      689 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Bolton_et_al_2011.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1129 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Bosman_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      710 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Chornock_et_al_2013.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      729 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Choudhury_et_al_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      910 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Choudhury_et_al_2021.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1247 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Davies_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      632 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Dijkstra_et_al_2011.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1147 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Durovcikova_et_al_2024.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1105 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Fan_et_al_2006.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1401 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Gaikwad_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      661 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Greig_et_al_2017.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      664 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Greig_et_al_2019.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      695 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Hoag_et_al_2019.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      730 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Jensen_et_al_2013.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      868 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Jung_et_al_2020.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1391 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Lu_et_al_2020.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      635 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Mason_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      760 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Mason_et_al_2019.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      658 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/McGreer_et_al_2011.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      674 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/McGreer_et_al_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      731 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Mesinger_et_al_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      657 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Mortlock_et_al_2011.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      795 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Nakane_et_al_2024.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      684 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Ono_et_al_2012.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      699 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Ota_et_al_2008.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      927 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Ouchi_et_al_2010.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      957 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Pentericci_et_al_2014.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      922 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Robertson_et_al_2013.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      688 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Schenker_et_al_2014.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      678 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Schroeder_et_al_2013.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      661 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Sobacchi_Mesinger_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      936 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Tilvi_et_al_2014.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1094 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Totani_et_al_2006.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      783 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Umeda_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      872 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Wang_et_al_2020.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      791 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Yang_et_al_2020.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1126 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Yang_et_al_2020b.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      716 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HII_fraction/Zhu_et_al_2022.py
+-rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)        0 2020-05-11 19:32:45.000000 corecon-1.4/corecon/data/HII_fraction/__init__.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon/data/HI_photoionization_rate/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      823 2024-04-20 17:01:29.000000 corecon-1.4/corecon/data/HI_photoionization_rate/Becker_et_al_2013.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      608 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HI_photoionization_rate/Bolton_et_al_2007.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      796 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HI_photoionization_rate/Calverley_et_al_2011.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      807 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HI_photoionization_rate/DAloisio_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      922 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HI_photoionization_rate/Davies_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      857 2024-04-20 17:19:20.000000 corecon-1.4/corecon/data/HI_photoionization_rate/Gaikwad_et_al_2017a.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      835 2024-04-20 17:19:12.000000 corecon-1.4/corecon/data/HI_photoionization_rate/Gaikwad_et_al_2017b.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1311 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HI_photoionization_rate/Gaikwad_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      574 2024-04-20 17:18:19.000000 corecon-1.4/corecon/data/HI_photoionization_rate/Kollmeier_et_al_2014.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      651 2024-04-20 17:22:07.000000 corecon-1.4/corecon/data/HI_photoionization_rate/Viel_et_al_2017.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      678 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HI_photoionization_rate/Wyithe_et_al_2011.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon/data/HeIII_fraction/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      753 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HeIII_fraction/Makan_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      796 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HeIII_fraction/Worseck_et_al_2016.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1091 2024-04-20 12:34:18.000000 corecon-1.4/corecon/data/HeIII_fraction/Worseck_et_al_2019.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 10:20:15.000000 corecon-1.4/corecon/data/HeIII_fraction/__init__.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon/data/HeII_to_HI_column_density_ratio/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    19889 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/HeII_to_HI_column_density_ratio/Syphers_and_Shull_2014.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.4/corecon/data/HeII_to_HI_column_density_ratio/__init__.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon/data/IGM_temperature_mean_density/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1104 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/IGM_temperature_mean_density/Becker_et_al_2011.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      964 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/IGM_temperature_mean_density/Boera_et_al_2014.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      830 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/IGM_temperature_mean_density/Boera_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      754 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/IGM_temperature_mean_density/Bolton_et_al_2010.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      792 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/IGM_temperature_mean_density/Bolton_et_al_2012.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      885 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/IGM_temperature_mean_density/Bolton_et_al_2014.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      918 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/IGM_temperature_mean_density/Gaikwad_et_al_2020.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1332 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/IGM_temperature_mean_density/Gaikwad_et_al_2021.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      885 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/IGM_temperature_mean_density/Garzilli_et_al_2012.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1145 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/IGM_temperature_mean_density/Hiss_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      970 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/IGM_temperature_mean_density/Lidz_et_al_2010.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1081 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/IGM_temperature_mean_density/Rorai_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1551 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/IGM_temperature_mean_density/Schaye_et_al_2010.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1579 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/IGM_temperature_mean_density/Walther_et_al_2019.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.4/corecon/data/IGM_temperature_mean_density/__init__.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon/data/Lya_flux_power_spectrum/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     5003 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/Lya_flux_power_spectrum/Croft_et_al_2002.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2674 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/Lya_flux_power_spectrum/DAloisio_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     9025 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/Lya_flux_power_spectrum/McDonald_et_al_2006.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    26999 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/Lya_flux_power_spectrum/Palanque-Delabrouille_et_al_2013_fourier.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    25486 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/Lya_flux_power_spectrum/Palanque-Delabrouille_et_al_2013_likelihood.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.4/corecon/data/Lya_flux_power_spectrum/__init__.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon/data/Lya_spike_galaxy_correlation/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2219 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/Lya_spike_galaxy_correlation/Kakiichi_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     6447 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/Lya_spike_galaxy_correlation/Kashino_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1530 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/Lya_spike_galaxy_correlation/Meyer_et_al_2019.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     3433 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/Lya_spike_galaxy_correlation/Meyer_et_al_2020.py
+-rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)        0 2020-06-27 13:38:09.000000 corecon-1.4/corecon/data/Lya_spike_galaxy_correlation/__init__.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon/data/UV_luminosity_density/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      599 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_density/Adams_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      694 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_density/Bouwens_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      505 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_density/Donnan_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      566 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_density/Finkelstein_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      640 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_density/Harikane_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      505 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_density/McLeod_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      675 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_density/Perez-Gonzales_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      626 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_density/Willot_et_al_2023.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon/data/UV_luminosity_function/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2245 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Adams_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1828 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Atek_et_al_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1785 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Atek_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     5909 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Bouwens_et_al_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1229 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Bouwens_et_al_2016.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1813 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Bouwens_et_al_2017.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     6608 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Bouwens_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1173 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Bouwens_et_al_2023a.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1039 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Bouwens_et_al_2023b.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1129 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Bowler_et_al_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1070 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Bowler_et_al_2020.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      979 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Casey_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      898 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Castellano_et_al_2016.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1773 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Donnan_et_al_2023a.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      845 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Donnan_et_al_2023b.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2694 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Donnan_et_al_2024.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     5256 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Finkelstein_et_al_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      848 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Finkelstein_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1953 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Finkelstein_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2004 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Harikane_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     4562 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Ishigaki_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1170 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Kauffmann_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1870 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Leung_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     4335 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Livermore_et_al_2017.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1075 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/McLeod_et_al_2016.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1354 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/McLeod_et_al_2024.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1984 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/McLure_et_al_2013.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      889 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Morishita_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      888 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Naidu_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1235 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Oesch_et_al_2014.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      978 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Oesch_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1020 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Perez-Gonzalez_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1216 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Robertson_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1283 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Rojas-Ruiz_et_al_2020.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1217 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Stefanon_et_al_2019.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2626 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_luminosity_function/Willott_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.4/corecon/data/UV_luminosity_function/__init__.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon/data/UV_slope/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1511 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_slope/Atek_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     3110 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_slope/Austin_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2565 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_slope/Bouwens_et_al_2009.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     4278 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_slope/Cullen_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1106 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_slope/Curtis-Lake_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1384 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_slope/Donnan_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     8626 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_slope/Endsley_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)   243506 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_slope/Finkelstein_et_al_2012.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2525 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_slope/Franco_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2242 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_slope/Simmonds_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1950 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_slope/Tacchella_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      922 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_slope/Topping_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1210 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_slope/Whitler_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     3277 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/UV_slope/Whitler_et_al_2023.py
+-rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)        0 2020-05-11 19:32:45.000000 corecon-1.4/corecon/data/__init__.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      507 2023-06-19 16:03:09.000000 corecon-1.4/corecon/data/data_entry_template.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon/data/dust_mass/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      843 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/dust_mass/Laporte_et_al_2017.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon/data/effective_optical_depth_HI_Lya/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     5850 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/effective_optical_depth_HI_Lya/Becker_et_al_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    16176 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/effective_optical_depth_HI_Lya/Bosman_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    29333 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/effective_optical_depth_HI_Lya/Bosman_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     7910 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/effective_optical_depth_HI_Lya/Eilers+18.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     6987 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/effective_optical_depth_HI_Lya/Fan_et_al_2006.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     4116 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/effective_optical_depth_HI_Lya/Liu_Bordoloi_2021.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    11861 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/effective_optical_depth_HI_Lya/Yang_et_al_2020.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.4/corecon/data/effective_optical_depth_HI_Lya/__init__.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon/data/effective_optical_depth_HeII_Lya/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1956 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/effective_optical_depth_HeII_Lya/Makan_et_al_2021.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2932 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/effective_optical_depth_HeII_Lya/Makan_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     6007 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/effective_optical_depth_HeII_Lya/Worseck_et_al_2016.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     6533 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/effective_optical_depth_HeII_Lya/Worseck_et_al_2019.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.4/corecon/data/effective_optical_depth_HeII_Lya/__init__.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon/data/galaxy_main_sequence/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2019 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/galaxy_main_sequence/Chen_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      867 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/galaxy_main_sequence/Finkelstein_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1642 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/galaxy_main_sequence/Leethochawali_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2885 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/galaxy_main_sequence/Roberts-Borsani_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1538 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/galaxy_main_sequence/Stefanon_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1863 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/galaxy_main_sequence/Tacchella_et_al_2022.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon/data/ionizing_photons_emission_rate/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      643 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/ionizing_photons_emission_rate/Becker_et_al_2013.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      789 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/ionizing_photons_emission_rate/Becker_et_al_2021.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1746 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/ionizing_photons_emission_rate/Bouwens_et_al_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1311 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/ionizing_photons_emission_rate/Gaikwad_et_al_2023.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon/data/ionizing_photons_production_efficiency/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1023 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/ionizing_photons_production_efficiency/Bouwens_et_al_2016.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      788 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/ionizing_photons_production_efficiency/Bunker_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1380 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/ionizing_photons_production_efficiency/Endsley_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      912 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/ionizing_photons_production_efficiency/Harikane_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      878 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/ionizing_photons_production_efficiency/Jung_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1124 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/ionizing_photons_production_efficiency/Lam_et_al_2019.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      788 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/ionizing_photons_production_efficiency/Maseda_et_al_2020.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    67827 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/ionizing_photons_production_efficiency/Prieto-Lyon_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1160 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/ionizing_photons_production_efficiency/Saxena_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2242 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/ionizing_photons_production_efficiency/Simmonds_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      724 2023-06-19 16:03:09.000000 corecon-1.4/corecon/data/make_data_archive.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon/data/mass_gas_metallicity_relation/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      925 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/mass_gas_metallicity_relation/Boyett_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      900 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/mass_gas_metallicity_relation/Bunker_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      868 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/mass_gas_metallicity_relation/Curti_et_al_2023a.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1357 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/mass_gas_metallicity_relation/Faisst_et_al_2016.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1463 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/mass_gas_metallicity_relation/Fujimoto_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1793 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/mass_gas_metallicity_relation/Langeroodi_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    37184 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/mass_gas_metallicity_relation/Nakajima_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2834 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/mass_gas_metallicity_relation/Roberts-Borsani_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1076 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/mass_gas_metallicity_relation/Schaerer_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1097 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/mass_gas_metallicity_relation/Trump_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     2462 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/mass_gas_metallicity_relation/Venturi_et_al_2024.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1038 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/mass_gas_metallicity_relation/Williams_et_al_2023.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon/data/mass_stellar_metallicity_relation/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1948 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/mass_stellar_metallicity_relation/Furtak_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1690 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/mass_stellar_metallicity_relation/Tacchella_et_al_2022.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon/data/mean_free_path/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      697 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/mean_free_path/Becker_et_al_2021.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      568 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/mean_free_path/Bosman_et_al_2021.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      643 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/mean_free_path/DAloisio_et_al_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      791 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/mean_free_path/Fumagalli_et_al_2013.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1192 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/mean_free_path/Gaikwad_et_al_2023.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      783 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/mean_free_path/OMeara_et_al_2013.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      931 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/mean_free_path/Prochaska_et_al_2009.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      852 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/mean_free_path/Worseck_et_al_2014.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.4/corecon/data/mean_free_path/__init__.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon/data/optical_depth_CMB/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1017 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/optical_depth_CMB/Pagani_et_al_2020.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      845 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/optical_depth_CMB/Paoletti_et_al_2020.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      850 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/optical_depth_CMB/Planck_2013.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      997 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/optical_depth_CMB/Planck_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1058 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/optical_depth_CMB/Planck_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      848 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/optical_depth_CMB/WMAP_5yr.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      840 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/optical_depth_CMB/WMAP_7yr.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      849 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/optical_depth_CMB/WMAP_9yr.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.4/corecon/data/optical_depth_CMB/__init__.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      860 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/optical_depth_CMB/deBelsunce_et_al_2021.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon/data/quasar_luminosity_function/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1348 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/quasar_luminosity_function/Giallongo_et_al_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1337 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/quasar_luminosity_function/Giallongo_et_al_2019.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1040 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/quasar_luminosity_function/Glikman_et_al_2011.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1147 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/quasar_luminosity_function/Jiang_et_al_2016.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      897 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/quasar_luminosity_function/Kashikawa_et_al_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    28572 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/quasar_luminosity_function/Kulkarni_et_al_2019.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1266 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/quasar_luminosity_function/McGreer_et_al_2013.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     4498 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/quasar_luminosity_function/Ross_et_al_2013.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1078 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/quasar_luminosity_function/Willott_et_al_2010.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1027 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/quasar_luminosity_function/Yang_et_al_2016.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)        0 2023-06-19 16:03:09.000000 corecon-1.4/corecon/data/quasar_luminosity_function/__init__.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon/data/reionization_midpoint/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      490 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/reionization_midpoint/Pagano_et_al_2020.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      500 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/reionization_midpoint/Paoletti_et_al_2020.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      472 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/reionization_midpoint/Planck_2013.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      477 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/reionization_midpoint/Planck_2015.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      477 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/reionization_midpoint/Planck_2018.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      499 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/reionization_midpoint/deBelsunce_et_al_2021.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon/data/sfrd/
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      980 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/sfrd/Donnan_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)      982 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/sfrd/Harikane_et_al_2022.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     4720 2024-04-20 12:22:32.000000 corecon-1.4/corecon/data/sfrd/Madau_and_Dickinson_2014.py
+-rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)        0 2020-06-23 15:25:46.000000 corecon-1.4/corecon/data/sfrd/__init__.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)    10032 2024-04-20 10:48:13.000000 corecon-1.4/corecon/fields_info.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     8799 2024-04-19 11:08:32.000000 corecon-1.4/corecon/loaders.py
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)       20 2024-04-20 17:30:54.000000 corecon-1.4/corecon/version.py
+drwxrwxr-x   0 egaraldi  (1001) egaraldi  (1001)        0 2024-04-20 17:34:28.000000 corecon-1.4/corecon.egg-info/
+-rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)     1991 2024-04-20 17:34:28.000000 corecon-1.4/corecon.egg-info/PKG-INFO
+-rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)    13359 2024-04-20 17:34:28.000000 corecon-1.4/corecon.egg-info/SOURCES.txt
+-rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)        1 2024-04-20 17:34:28.000000 corecon-1.4/corecon.egg-info/dependency_links.txt
+-rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)        6 2024-04-20 17:34:28.000000 corecon-1.4/corecon.egg-info/requires.txt
+-rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)        8 2024-04-20 17:34:28.000000 corecon-1.4/corecon.egg-info/top_level.txt
+-rw-r--r--   0 egaraldi  (1001) egaraldi  (1001)       79 2024-04-20 17:34:28.000000 corecon-1.4/setup.cfg
+-rw-rw-r--   0 egaraldi  (1001) egaraldi  (1001)     1404 2024-04-20 17:32:31.000000 corecon-1.4/setup.py
```

### Comparing `corecon-1.3/LICENSE.txt` & `corecon-1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `corecon-1.3/PKG-INFO` & `corecon-1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: corecon
-Version: 1.3
+Version: 1.4
 Summary: an open collection of constraints on the Epoch of Reionization
 Home-page: https://github.com/EGaraldi/corecon
-Download-URL: https://github.com/EGaraldi/corecon/archive/v1.3.tar.gz
+Download-URL: https://github.com/EGaraldi/corecon/archive/v1.4.tar.gz
 Author: Enrico Garaldi
 Author-email: enrico.garaldi@gmail.com
 License: gpl-3.0
 Keywords: constraints,reionization,cosmic,observations,data
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Build Tools
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE.txt
 
 ![](logo.png)
 
 [![DOI](https://zenodo.org/badge/224433919.svg)](https://zenodo.org/badge/latestdoi/224433919)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.05407/status.svg)](https://doi.org/10.21105/joss.05407)
```

### Comparing `corecon-1.3/README.md` & `corecon-1.4/README.md`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/DataEntryClass.py` & `corecon-1.4/corecon/DataEntryClass.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/FieldClass.py` & `corecon-1.4/corecon/FieldClass.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/InternalFunctions.py` & `corecon-1.4/corecon/InternalFunctions.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/__init__.py` & `corecon-1.4/corecon/__init__.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/check_updates.py` & `corecon-1.4/corecon/check_updates.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/HeII_to_HI_column_density_ratio/Syphers_and_Shull_2014.py` & `corecon-1.4/corecon/data/HeII_to_HI_column_density_ratio/Syphers_and_Shull_2014.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/IGM_temperature_mean_density/Becker_et_al_2011.py` & `corecon-1.4/corecon/data/IGM_temperature_mean_density/Becker_et_al_2011.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/IGM_temperature_mean_density/Boera_et_al_2014.py` & `corecon-1.4/corecon/data/IGM_temperature_mean_density/Boera_et_al_2014.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/IGM_temperature_mean_density/Boera_et_al_2018.py` & `corecon-1.4/corecon/data/IGM_temperature_mean_density/Boera_et_al_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/IGM_temperature_mean_density/Bolton_et_al_2010.py` & `corecon-1.4/corecon/data/IGM_temperature_mean_density/Bolton_et_al_2010.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/IGM_temperature_mean_density/Bolton_et_al_2012.py` & `corecon-1.4/corecon/data/IGM_temperature_mean_density/Bolton_et_al_2012.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/IGM_temperature_mean_density/Bolton_et_al_2014.py` & `corecon-1.4/corecon/data/IGM_temperature_mean_density/Bolton_et_al_2014.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/IGM_temperature_mean_density/Gaikwad_et_al_2020.py` & `corecon-1.4/corecon/data/IGM_temperature_mean_density/Gaikwad_et_al_2020.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/IGM_temperature_mean_density/Gaikwad_et_al_2021.py` & `corecon-1.4/corecon/data/IGM_temperature_mean_density/Gaikwad_et_al_2021.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/IGM_temperature_mean_density/Garzilli_et_al_2012.py` & `corecon-1.4/corecon/data/IGM_temperature_mean_density/Garzilli_et_al_2012.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/IGM_temperature_mean_density/Hiss_et_al_2018.py` & `corecon-1.4/corecon/data/IGM_temperature_mean_density/Hiss_et_al_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/IGM_temperature_mean_density/Lidz_et_al_2010.py` & `corecon-1.4/corecon/data/IGM_temperature_mean_density/Lidz_et_al_2010.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/IGM_temperature_mean_density/Rorai_et_al_2018.py` & `corecon-1.4/corecon/data/IGM_temperature_mean_density/Rorai_et_al_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/IGM_temperature_mean_density/Schaye_et_al_2010.py` & `corecon-1.4/corecon/data/IGM_temperature_mean_density/Schaye_et_al_2010.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/IGM_temperature_mean_density/Walther_et_al_2019.py` & `corecon-1.4/corecon/data/IGM_temperature_mean_density/Walther_et_al_2019.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/Lya_flux_power_spectrum/Croft_et_al_2002.py` & `corecon-1.4/corecon/data/Lya_flux_power_spectrum/Croft_et_al_2002.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/Lya_flux_power_spectrum/DAloisio_et_al_2018.py` & `corecon-1.4/corecon/data/Lya_flux_power_spectrum/DAloisio_et_al_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/Lya_flux_power_spectrum/McDonald_et_al_2006.py` & `corecon-1.4/corecon/data/Lya_flux_power_spectrum/McDonald_et_al_2006.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/Lya_flux_power_spectrum/Palanque-Delabrouille_et_al_2013_fourier.py` & `corecon-1.4/corecon/data/Lya_flux_power_spectrum/Palanque-Delabrouille_et_al_2013_fourier.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/Lya_flux_power_spectrum/Palanque-Delabrouille_et_al_2013_likelihood.py` & `corecon-1.4/corecon/data/Lya_flux_power_spectrum/Palanque-Delabrouille_et_al_2013_likelihood.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/Lya_spike_galaxy_correlation/Kakiichi_et_al_2018.py` & `corecon-1.4/corecon/data/Lya_spike_galaxy_correlation/Kakiichi_et_al_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/Lya_spike_galaxy_correlation/Kashino_et_al_2023.py` & `corecon-1.4/corecon/data/Lya_spike_galaxy_correlation/Kashino_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/Lya_spike_galaxy_correlation/Meyer_et_al_2019.py` & `corecon-1.4/corecon/data/Lya_spike_galaxy_correlation/Meyer_et_al_2019.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/Lya_spike_galaxy_correlation/Meyer_et_al_2020.py` & `corecon-1.4/corecon/data/Lya_spike_galaxy_correlation/Meyer_et_al_2020.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_density/Adams_et_al_2023.py` & `corecon-1.4/corecon/data/UV_luminosity_density/Adams_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_density/Bouwens_et_al_2022.py` & `corecon-1.4/corecon/data/UV_luminosity_density/Bouwens_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_density/Finkelstein_et_al_2023.py` & `corecon-1.4/corecon/data/UV_luminosity_density/Finkelstein_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_density/Harikane_et_al_2023.py` & `corecon-1.4/corecon/data/UV_luminosity_density/Harikane_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_density/Perez-Gonzales_et_al_2023.py` & `corecon-1.4/corecon/data/UV_luminosity_density/Perez-Gonzales_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_density/Willot_et_al_2023.py` & `corecon-1.4/corecon/data/UV_luminosity_density/Willot_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_function/Atek_et_al_2015.py` & `corecon-1.4/corecon/data/UV_luminosity_function/Atek_et_al_2015.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_function/Atek_et_al_2018.py` & `corecon-1.4/corecon/data/UV_luminosity_function/Atek_et_al_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_function/Bouwens_et_al_2015.py` & `corecon-1.4/corecon/data/UV_luminosity_function/Bouwens_et_al_2015.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_function/Bouwens_et_al_2016.py` & `corecon-1.4/corecon/data/UV_luminosity_function/Bouwens_et_al_2016.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_function/Bouwens_et_al_2017.py` & `corecon-1.4/corecon/data/UV_luminosity_function/Bouwens_et_al_2017.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_function/Bouwens_et_al_2022.py` & `corecon-1.4/corecon/data/UV_luminosity_function/Bouwens_et_al_2023b.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-dictionary_tag         = "Bouwens et al. 2023"
+dictionary_tag         = "Bouwens et al. 2023b"
 
 reference              = "Bouwens, Stefanon, Brammer, Oesch, Herard-Demanche, Illingworth, et al., MNRAS 523, 1936 (2023)"
 
 url                    = "https://ui.adsabs.harvard.edu/abs/2023MNRAS.523.1036B/abstract"
 
 description            = \
 """
```

### Comparing `corecon-1.3/corecon/data/UV_luminosity_function/Bowler_et_al_2015.py` & `corecon-1.4/corecon/data/UV_luminosity_function/Bowler_et_al_2015.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_function/Bowler_et_al_2020.py` & `corecon-1.4/corecon/data/UV_luminosity_function/Bowler_et_al_2020.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_function/Castellano_et_al_2016.py` & `corecon-1.4/corecon/data/UV_luminosity_function/Castellano_et_al_2016.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_function/Donnan_et_al_2022.py` & `corecon-1.4/corecon/data/UV_luminosity_function/Harikane_et_al_2022.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,45 @@
-dictionary_tag         = "Donnan et al. 2022"
+dictionary_tag         = "Harikane et al. 2023"
 
-reference              = "Donnan, McLeod, Dunlop, McLure, Carnall, Begley, Cullen, et al.; arXiv (2022)"
+reference              = "Harikane, Ouchi, Oguri, Ono, Nakajima, Isobe, Umeda, Mawatari, Zhang; ApJS 265, 5 (2023)"
 
-url                    = "https://arxiv.org/pdf/2207.12356.pdf"
+url                    = "https://iopscience.iop.org/article/10.3847/1538-4365/acaaa9"
 
 description            = \
 """
-Based on a combination of COSMOS and JWST's SMACS0723, GLASS and CEERS data, resulting in 55 galaxy candidates at
-8 < z < 15 (6 at z>12). 
+Based on 25 dropout galaxy candidates at 9 < z < 17 identified in 90 arcmin2 JWST/NIRCam images taken by the early release 
+observations (ERO) and early release science (ERS) programs.
 """
 
 data_structure         = "points" #grid or points
 
 extracted              = False
 
 ndim                   = 2
 
 dimensions_descriptors = ["redshift", "M_UV"]
 
-axes                   = [[8, -22.17], [8, -21.42], [9, -22.30], [9, -21.30], [9, -19.33], [9, -18.70], \
-                          [10, -22.57], [10, -19.35], [10, -18.85], [11, -20.60], [11, -19.75], [11, -19.25], \
-                          [12, -20.70], [12, -18.85], [13.75, -19.10]]
-
-values                 = [-6.20065945, -5.40671393, -6.76955108, -5.51999306, -3.85294233,
-                          -3.31060234, -6.74472749, -3.88706002, -3.79344396, -4.76955108,
-                          -3.98505965, -3.85480359, -4.73282827, -4.22694531, -4.7721133
-                         ]
-
-err_up                 = [0.17838306, 0.15100692, 0.30103   , 0.28041554, 0.1764007 ,
-                          0.39162542, 0.30103   , 0.17620286, 0.16061344, 0.30103   ,
-                          0.19804583, 0.17619487, 0.30103   , 0.19822116, 0.23301114
-                         ]
-
-err_down               = [0.30797886,  0.23345058, 100,  1.03284891,  0.30195963,
-                          100, 93.25527251,  0.30136497,  0.25765428, 100,
-                          0.37445891,  0.30134098, 100,  0.37511468,  0.53769062
-                         ]
+axes                   = [[9, -23.03], [9, -22.03], [9, -21.03], [9, -20.03], [9, -19.03], [9, -18.03], 
+                          [12, -23.21], [12, -22.21], [12, -21.21], [12, -20.21], [12, -19.21], [12, -18.21],
+                          [16, -23.59], [16, -20.59]]
 
-err_left               = [0.5, 0.25, 0.5, 0.5, 0.5, 0.25, 0.5, 0.25, 0.25, 0.5, 0.25, 0.25, 0.5, 0.5, 0.5]
+values                 = [-4.1580152 , -4.11520464, -4.39794001, -4.38933984, -3.64975198, -2.95078198, 
+                          -5.23284413, -5.19382003, -5.30103   , -4.8827287 , -4.61978876, -3.84771166, 
+                          -5.61618463, -5.17914201]
 
-err_right              = [0.5, 0.25, 0.5, 0.5, 0.5, 0.25, 0.5, 0.25, 0.25, 0.5, 0.25, 0.25, 0.5, 0.5, 0.5]
+err_up                 = [None, None, 0.52569252, 0.52542593, 0.03482176, 0.0039757,
+                          None, None, 0.52009033, 0.36845013, 0.29921665, 0.37791135,        
+                          None, 0.3683515]
 
-upper_lim              = False
+err_down               = [None, None, 1.42596873, 1.40654018, 0.02927134, 0.00350396,
+                          None, None, 0.83564714, 0.49402201, 0.38021124, 0.64713837,
+                          None, 0.49247839]
+
+err_right              = [0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 1.5, 1.5]
+
+err_left               = [0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 1.5, 1.5]
+
+upper_lim              = [True, True, False, False, False, False, 
+                          True, True, False, False, False, False,
+                          True, False]
 
 lower_lim              = False
```

### Comparing `corecon-1.3/corecon/data/UV_luminosity_function/Finkelstein_et_al_2015.py` & `corecon-1.4/corecon/data/UV_luminosity_function/Finkelstein_et_al_2015.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_function/Finkelstein_et_al_2022.py` & `corecon-1.4/corecon/data/UV_luminosity_function/Finkelstein_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_function/Harikane_et_al_2022.py` & `corecon-1.4/corecon/data/UV_luminosity_function/Donnan_et_al_2023a.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,43 @@
-dictionary_tag         = "Harikane et al. 2022"
+dictionary_tag         = "Donnan et al. 2023a"
 
-reference              = "Harikane, Ouchi, Oguri, Ono, Nakajima, Isobe, Umeda, Mawatari, Zhang; arXiv (2022)"
+reference              = "Donnan, McLeod, Dunlop, McLure, Carnall, Begley, Cullen, et al.; MNRAS 518, 6011 (2023)"
 
-url                    = "https://arxiv.org/pdf/2208.01612.pdf"
+url                    = "https://academic.oup.com/mnras/article/518/4/6011/6849970"
 
 description            = \
 """
-Based on 25 dropout galaxy candidates at 9 < z < 17 identified in 90 arcmin2 JWST/NIRCam images taken by the early release 
-observations (ERO) and early release science (ERS) programs.
+Based on a combination of COSMOS and JWST's SMACS0723, GLASS and CEERS data, resulting in 55 galaxy candidates at
+8 < z < 15 (6 at z>12). 
 """
 
 data_structure         = "points" #grid or points
 
 extracted              = False
 
 ndim                   = 2
 
 dimensions_descriptors = ["redshift", "M_UV"]
 
-axes                   = [[9, -23.03], [9, -22.03], [9, -21.03], [9, -20.03], [9, -19.03], [9, -18.03], 
-                          [12, -23.21], [12, -22.21], [12, -21.21], [12, -20.21], [12, -19.21], [12, -18.21],
-                          [17, -23.59], [17, -20.59]]
+axes                   = [[8, -22.17], [8, -21.42], [9, -22.30], [9, -21.30], [9, -18.50], 
+                          [10.5, -22.57], [10.5, -20.10], [10.5, -19.35], [10.5, -18.85], [10.5, -18.23], 
+                          [13.25, -20.35], [13.25, -19]]
 
-values                 = [-4.1580152 , -4.11350927, -4.38933984, -4.38933984, -3.5214335, -3.27083521, 
-                          -5.22841252, -5.18641901, -5.34872199, -4.88941029, -4.83564714, -3.98716278, 
-                          -5.66756154, -5.26841123]
+values                 = [-6.20065945, -5.40671393, -6.76955108, -5.51999306, -2.92081875,
+                          -6.74472749, -4.79048499, -3.86646109, -3.62911698, 
+                          -3.20010832, -4.98716278, -4.56224944]
 
-err_up                 = [None, None, 0.52510835, 0.52510835, 0.23743685, 0.25983983,
-                          None, None, 0.51957019, 0.36797679, 0.36840152, 0.30730906,        
-                          None, 0.36705496]
+err_up                 = [0.25373789, 0.20328827, 0.52542593, 0.3650911 , 0.20344087,
+                          0.52287875, 0.36567283, 0.1743848 , 0.16301608, 
+                          0.18723808, 0.29423073, 0.25333093]
 
-err_down               = [None, None, 1.40654018, 1.40654018, 0.41038063, 0.50385551,
-                          None, None, 0.83173408, 0.48734042, 0.492255  , 0.45653472,
-                          None, 0.47151738]
+err_down               = [0.28082661, 0.22037406, 0.75332767, 0.45062317, 0.21944268,
+                          0.77815125, 0.45364016, 0.18463715, 0.17195115, 
+                          0.20022691, 0.33981632, 0.28241453]
 
-err_right              = [0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 1.5, 1.5]
+err_left               = [0.5, 0.25, 0.5, 0.5, 0.5, 0.5, 0.5, 0.25, 0.25, 0.375, 0.85, 0.5]
 
-err_left               = [0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 1.5, 1.5]
+err_right              = [0.5, 0.25, 0.5, 0.5, 0.5, 0.5, 0.5, 0.25, 0.25, 0.375, 0.85, 0.5]
 
-upper_lim              = [True, True, False, False, False, False, 
-                          True, True, False, False, False, False,
-                          True, False]
+upper_lim              = False
 
 lower_lim              = False
```

### Comparing `corecon-1.3/corecon/data/UV_luminosity_function/Ishigaki_et_al_2018.py` & `corecon-1.4/corecon/data/UV_luminosity_function/Ishigaki_et_al_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_function/Kauffmann_et_al_2022.py` & `corecon-1.4/corecon/data/UV_luminosity_function/Kauffmann_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_function/Livermore_et_al_2017.py` & `corecon-1.4/corecon/data/UV_luminosity_function/Livermore_et_al_2017.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_function/McLeod_et_al_2016.py` & `corecon-1.4/corecon/data/UV_luminosity_function/McLeod_et_al_2016.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_function/McLure_et_al_2013.py` & `corecon-1.4/corecon/data/UV_luminosity_function/McLure_et_al_2013.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_function/Morishita_et_al_2018.py` & `corecon-1.4/corecon/data/UV_luminosity_function/Morishita_et_al_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_function/Naidu_et_al_2022.py` & `corecon-1.4/corecon/data/UV_luminosity_function/Naidu_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_function/Oesch_et_al_2014.py` & `corecon-1.4/corecon/data/UV_luminosity_function/Oesch_et_al_2014.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_function/Rojas-Ruiz_et_al_2020.py` & `corecon-1.4/corecon/data/UV_luminosity_function/Rojas-Ruiz_et_al_2020.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_luminosity_function/Stefanon_et_al_2019.py` & `corecon-1.4/corecon/data/UV_luminosity_function/Stefanon_et_al_2019.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_slope/Atek_et_al_2023.py` & `corecon-1.4/corecon/data/UV_slope/Atek_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_slope/Austin_et_al_2023.py` & `corecon-1.4/corecon/data/UV_slope/Austin_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_slope/Bouwens_et_al_2009.py` & `corecon-1.4/corecon/data/UV_slope/Bouwens_et_al_2009.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_slope/Cullen_et_al_2023.py` & `corecon-1.4/corecon/data/UV_slope/Cullen_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_slope/Curtis-Lake_et_al_2022.py` & `corecon-1.4/corecon/data/UV_slope/Curtis-Lake_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_slope/Endsley_et_al_2022.py` & `corecon-1.4/corecon/data/UV_slope/Endsley_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_slope/Finkelstein_et_al_2012.py` & `corecon-1.4/corecon/data/UV_slope/Finkelstein_et_al_2012.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_slope/Franco_et_al_2023.py` & `corecon-1.4/corecon/data/UV_slope/Franco_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_slope/Simmonds_et_al_2023.py` & `corecon-1.4/corecon/data/UV_slope/Simmonds_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_slope/Tacchella_et_al_2022.py` & `corecon-1.4/corecon/data/UV_slope/Tacchella_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_slope/Topping_et_al_2022.py` & `corecon-1.4/corecon/data/UV_slope/Topping_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_slope/Whitler_et_al_2022.py` & `corecon-1.4/corecon/data/UV_slope/Whitler_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/UV_slope/Whitler_et_al_2023.py` & `corecon-1.4/corecon/data/UV_slope/Whitler_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/dust_mass/Laporte_et_al_2017.py` & `corecon-1.4/corecon/data/dust_mass/Laporte_et_al_2017.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/effective_optical_depth_HI_Lya/Becker_et_al_2015.py` & `corecon-1.4/corecon/data/effective_optical_depth_HI_Lya/Becker_et_al_2015.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/effective_optical_depth_HI_Lya/Bosman_et_al_2018.py` & `corecon-1.4/corecon/data/effective_optical_depth_HI_Lya/Bosman_et_al_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/effective_optical_depth_HI_Lya/Bosman_et_al_2022.py` & `corecon-1.4/corecon/data/effective_optical_depth_HI_Lya/Bosman_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/effective_optical_depth_HI_Lya/Eilers+18.py` & `corecon-1.4/corecon/data/effective_optical_depth_HI_Lya/Eilers+18.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/effective_optical_depth_HI_Lya/Fan_et_al_2006.py` & `corecon-1.4/corecon/data/effective_optical_depth_HI_Lya/Fan_et_al_2006.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/effective_optical_depth_HI_Lya/Liu_Bordoloi_2021.py` & `corecon-1.4/corecon/data/effective_optical_depth_HI_Lya/Liu_Bordoloi_2021.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/effective_optical_depth_HI_Lya/Yang_et_al_2020.py` & `corecon-1.4/corecon/data/effective_optical_depth_HI_Lya/Yang_et_al_2020.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/effective_optical_depth_HeII_Lya/Worseck_et_al_2016.py` & `corecon-1.4/corecon/data/effective_optical_depth_HeII_Lya/Worseck_et_al_2016.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/galaxy_main_sequence/Chen_et_al_2022.py` & `corecon-1.4/corecon/data/galaxy_main_sequence/Chen_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/galaxy_main_sequence/Finkelstein_et_al_2022.py` & `corecon-1.4/corecon/data/galaxy_main_sequence/Finkelstein_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/galaxy_main_sequence/Leethochawali_et_al_2022.py` & `corecon-1.4/corecon/data/galaxy_main_sequence/Leethochawali_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/galaxy_main_sequence/Roberts-Borsani_et_al_2022.py` & `corecon-1.4/corecon/data/galaxy_main_sequence/Roberts-Borsani_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/galaxy_main_sequence/Stefanon_et_al_2022.py` & `corecon-1.4/corecon/data/galaxy_main_sequence/Stefanon_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/galaxy_main_sequence/Tacchella_et_al_2022.py` & `corecon-1.4/corecon/data/galaxy_main_sequence/Tacchella_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Bolton_et_al_2011.py` & `corecon-1.4/corecon/data/HII_fraction/Bolton_et_al_2011.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Bosman_et_al_2022.py` & `corecon-1.4/corecon/data/HII_fraction/Bosman_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Chornock_et_al_2013.py` & `corecon-1.4/corecon/data/HII_fraction/Chornock_et_al_2013.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Choudhury_et_al_2015.py` & `corecon-1.4/corecon/data/HII_fraction/Choudhury_et_al_2015.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Choudhury_et_al_2021.py` & `corecon-1.4/corecon/data/HII_fraction/Choudhury_et_al_2021.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Davies_et_al_2018.py` & `corecon-1.4/corecon/data/HII_fraction/Davies_et_al_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Dijkstra_et_al_2011.py` & `corecon-1.4/corecon/data/HII_fraction/Dijkstra_et_al_2011.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Fan_et_al_2006.py` & `corecon-1.4/corecon/data/HII_fraction/Fan_et_al_2006.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Gaikwad_et_al_2023.py` & `corecon-1.4/corecon/data/HII_fraction/Gaikwad_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Greig_et_al_2017.py` & `corecon-1.4/corecon/data/HII_fraction/Greig_et_al_2017.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Greig_et_al_2019.py` & `corecon-1.4/corecon/data/HII_fraction/Greig_et_al_2019.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Hoag_et_al_2019.py` & `corecon-1.4/corecon/data/HII_fraction/Hoag_et_al_2019.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Jensen_et_al_2013.py` & `corecon-1.4/corecon/data/HII_fraction/Jensen_et_al_2013.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Jung_et_al_2020.py` & `corecon-1.4/corecon/data/HII_fraction/Jung_et_al_2020.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Lu_et_al_2020.py` & `corecon-1.4/corecon/data/HII_fraction/Lu_et_al_2020.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Mason_et_al_2018.py` & `corecon-1.4/corecon/data/HII_fraction/Mason_et_al_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Mason_et_al_2019.py` & `corecon-1.4/corecon/data/HII_fraction/Mason_et_al_2019.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/McGreer_et_al_2011.py` & `corecon-1.4/corecon/data/HII_fraction/McGreer_et_al_2011.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/McGreer_et_al_2015.py` & `corecon-1.4/corecon/data/HII_fraction/McGreer_et_al_2015.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Mesinger_et_al_2015.py` & `corecon-1.4/corecon/data/HII_fraction/Mesinger_et_al_2015.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Mortlock_et_al_2011.py` & `corecon-1.4/corecon/data/HII_fraction/Mortlock_et_al_2011.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Ono_et_al_2012.py` & `corecon-1.4/corecon/data/HII_fraction/Ono_et_al_2012.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Ota_et_al_2008.py` & `corecon-1.4/corecon/data/HII_fraction/Ota_et_al_2008.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Ouchi_et_al_2010.py` & `corecon-1.4/corecon/data/HII_fraction/Ouchi_et_al_2010.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Pentericci_et_al_2014.py` & `corecon-1.4/corecon/data/HII_fraction/Pentericci_et_al_2014.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Robertson_et_al_2013.py` & `corecon-1.4/corecon/data/HII_fraction/Robertson_et_al_2013.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Schenker_et_al_2014.py` & `corecon-1.4/corecon/data/HII_fraction/Schenker_et_al_2014.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Schroeder_et_al_2013.py` & `corecon-1.4/corecon/data/HII_fraction/Schroeder_et_al_2013.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Sobacchi_Mesinger_2015.py` & `corecon-1.4/corecon/data/HII_fraction/Sobacchi_Mesinger_2015.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Tilvi_et_al_2014.py` & `corecon-1.4/corecon/data/HII_fraction/Tilvi_et_al_2014.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Totani_et_al_2006.py` & `corecon-1.4/corecon/data/HII_fraction/Totani_et_al_2006.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Wang_et_al_2020.py` & `corecon-1.4/corecon/data/HII_fraction/Wang_et_al_2020.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Yang_et_al_2020.py` & `corecon-1.4/corecon/data/HII_fraction/Yang_et_al_2020.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Yang_et_al_2020b.py` & `corecon-1.4/corecon/data/HII_fraction/Yang_et_al_2020b.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionized_fraction/Zhu_et_al_2022.py` & `corecon-1.4/corecon/data/HII_fraction/Zhu_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionizing_photons_emission_rate/Becker_et_al_2013.py` & `corecon-1.4/corecon/data/ionizing_photons_emission_rate/Becker_et_al_2013.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionizing_photons_emission_rate/Becker_et_al_2021.py` & `corecon-1.4/corecon/data/ionizing_photons_emission_rate/Becker_et_al_2021.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionizing_photons_emission_rate/Bouwens_et_al_2015.py` & `corecon-1.4/corecon/data/ionizing_photons_emission_rate/Bouwens_et_al_2015.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionizing_photons_emission_rate/Gaikwad_et_al_2023.py` & `corecon-1.4/corecon/data/ionizing_photons_emission_rate/Gaikwad_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionizing_photons_production_efficiency/Bouwens_et_al_2016.py` & `corecon-1.4/corecon/data/ionizing_photons_production_efficiency/Bouwens_et_al_2016.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionizing_photons_production_efficiency/Bunker_et_al_2023.py` & `corecon-1.4/corecon/data/ionizing_photons_production_efficiency/Bunker_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionizing_photons_production_efficiency/Endsley_et_al_2022.py` & `corecon-1.4/corecon/data/ionizing_photons_production_efficiency/Endsley_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionizing_photons_production_efficiency/Harikane_et_al_2018.py` & `corecon-1.4/corecon/data/ionizing_photons_production_efficiency/Harikane_et_al_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionizing_photons_production_efficiency/Jung_et_al_2023.py` & `corecon-1.4/corecon/data/ionizing_photons_production_efficiency/Jung_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionizing_photons_production_efficiency/Lam_et_al_2019.py` & `corecon-1.4/corecon/data/ionizing_photons_production_efficiency/Lam_et_al_2019.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionizing_photons_production_efficiency/Maseda_et_al_2020.py` & `corecon-1.4/corecon/data/ionizing_photons_production_efficiency/Maseda_et_al_2020.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionizing_photons_production_efficiency/Prieto-Lyon_et_al_2023.py` & `corecon-1.4/corecon/data/ionizing_photons_production_efficiency/Prieto-Lyon_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionizing_photons_production_efficiency/Saxena_et_al_2023.py` & `corecon-1.4/corecon/data/ionizing_photons_production_efficiency/Saxena_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/ionizing_photons_production_efficiency/Simmonds_et_al_2023.py` & `corecon-1.4/corecon/data/ionizing_photons_production_efficiency/Simmonds_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/make_data_archive.py` & `corecon-1.4/corecon/data/make_data_archive.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/mass_gas_metallicity_relation/Boyett_et_al_2023.py` & `corecon-1.4/corecon/data/mass_gas_metallicity_relation/Boyett_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/mass_gas_metallicity_relation/Bunker_et_al_2023.py` & `corecon-1.4/corecon/data/mass_gas_metallicity_relation/Bunker_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/mass_gas_metallicity_relation/Curti_et_al_2023a.py` & `corecon-1.4/corecon/data/mass_gas_metallicity_relation/Curti_et_al_2023a.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/mass_gas_metallicity_relation/Faisst_et_al_2016.py` & `corecon-1.4/corecon/data/mass_gas_metallicity_relation/Faisst_et_al_2016.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/mass_gas_metallicity_relation/Fujimoto_et_al_2023.py` & `corecon-1.4/corecon/data/mass_gas_metallicity_relation/Fujimoto_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/mass_gas_metallicity_relation/Langeroodi_et_al_2022.py` & `corecon-1.4/corecon/data/mass_gas_metallicity_relation/Langeroodi_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/mass_gas_metallicity_relation/Nakajima_et_al_2023.py` & `corecon-1.4/corecon/data/mass_gas_metallicity_relation/Nakajima_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/mass_gas_metallicity_relation/Roberts-Borsani_et_al_2022.py` & `corecon-1.4/corecon/data/mass_gas_metallicity_relation/Roberts-Borsani_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/mass_gas_metallicity_relation/Schaerer_et_al_2022.py` & `corecon-1.4/corecon/data/mass_gas_metallicity_relation/Schaerer_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/mass_gas_metallicity_relation/Trump_et_al_2023.py` & `corecon-1.4/corecon/data/mass_gas_metallicity_relation/Trump_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/mass_gas_metallicity_relation/Williams_et_al_2023.py` & `corecon-1.4/corecon/data/mass_gas_metallicity_relation/Williams_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/mass_stellar_metallicity_relation/Furtak_et_al_2022.py` & `corecon-1.4/corecon/data/mass_stellar_metallicity_relation/Furtak_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/mass_stellar_metallicity_relation/Tacchella_et_al_2022.py` & `corecon-1.4/corecon/data/mass_stellar_metallicity_relation/Tacchella_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/mean_free_path/Becker_et_al_2021.py` & `corecon-1.4/corecon/data/mean_free_path/Becker_et_al_2021.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/mean_free_path/Bosman_et_al_2021.py` & `corecon-1.4/corecon/data/mean_free_path/Bosman_et_al_2021.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/mean_free_path/DAloisio_et_al_2018.py` & `corecon-1.4/corecon/data/mean_free_path/DAloisio_et_al_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/mean_free_path/Fumagalli_et_al_2013.py` & `corecon-1.4/corecon/data/mean_free_path/Fumagalli_et_al_2013.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/mean_free_path/Gaikwad_et_al_2023.py` & `corecon-1.4/corecon/data/mean_free_path/Gaikwad_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/mean_free_path/OMeara_et_al_2013.py` & `corecon-1.4/corecon/data/mean_free_path/OMeara_et_al_2013.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/mean_free_path/Prochaska_et_al_2009.py` & `corecon-1.4/corecon/data/mean_free_path/Prochaska_et_al_2009.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/mean_free_path/Worseck_et_al_2014.py` & `corecon-1.4/corecon/data/mean_free_path/Worseck_et_al_2014.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/optical_depth_CMB/Pagani_et_al_2020.py` & `corecon-1.4/corecon/data/optical_depth_CMB/Pagani_et_al_2020.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/optical_depth_CMB/Paoletti_et_al_2020.py` & `corecon-1.4/corecon/data/optical_depth_CMB/Paoletti_et_al_2020.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/optical_depth_CMB/Planck_2013.py` & `corecon-1.4/corecon/data/optical_depth_CMB/Planck_2013.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/optical_depth_CMB/Planck_2015.py` & `corecon-1.4/corecon/data/optical_depth_CMB/Planck_2015.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/optical_depth_CMB/Planck_2018.py` & `corecon-1.4/corecon/data/optical_depth_CMB/Planck_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/optical_depth_CMB/WMAP_5yr.py` & `corecon-1.4/corecon/data/optical_depth_CMB/WMAP_5yr.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/optical_depth_CMB/WMAP_7yr.py` & `corecon-1.4/corecon/data/optical_depth_CMB/WMAP_7yr.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/optical_depth_CMB/WMAP_9yr.py` & `corecon-1.4/corecon/data/optical_depth_CMB/WMAP_9yr.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/optical_depth_CMB/deBelsunce_et_al_2021.py` & `corecon-1.4/corecon/data/optical_depth_CMB/deBelsunce_et_al_2021.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/photoionization_rate/Bolton_et_al_2007.py` & `corecon-1.4/corecon/data/HI_photoionization_rate/Bolton_et_al_2007.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/photoionization_rate/Calverley_et_al_2011.py` & `corecon-1.4/corecon/data/HI_photoionization_rate/Calverley_et_al_2011.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/photoionization_rate/DAloisio_et_al_2018.py` & `corecon-1.4/corecon/data/HI_photoionization_rate/DAloisio_et_al_2018.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/photoionization_rate/Gaikwad_et_al_2023.py` & `corecon-1.4/corecon/data/HI_photoionization_rate/Gaikwad_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/photoionization_rate/Wyithe_et_al_2011.py` & `corecon-1.4/corecon/data/HI_photoionization_rate/Wyithe_et_al_2011.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/quasar_luminosity_function/Giallongo_et_al_2015.py` & `corecon-1.4/corecon/data/quasar_luminosity_function/Giallongo_et_al_2015.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/quasar_luminosity_function/Giallongo_et_al_2019.py` & `corecon-1.4/corecon/data/quasar_luminosity_function/Giallongo_et_al_2019.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/quasar_luminosity_function/Glikman_et_al_2011.py` & `corecon-1.4/corecon/data/quasar_luminosity_function/Glikman_et_al_2011.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/quasar_luminosity_function/Jiang_et_al_2016.py` & `corecon-1.4/corecon/data/quasar_luminosity_function/Jiang_et_al_2016.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/quasar_luminosity_function/Kashikawa_et_al_2015.py` & `corecon-1.4/corecon/data/quasar_luminosity_function/Kashikawa_et_al_2015.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/quasar_luminosity_function/Kulkarni_et_al_2019.py` & `corecon-1.4/corecon/data/quasar_luminosity_function/Kulkarni_et_al_2019.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/quasar_luminosity_function/McGreer_et_al_2013.py` & `corecon-1.4/corecon/data/quasar_luminosity_function/McGreer_et_al_2013.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/quasar_luminosity_function/Ross_et_al_2013.py` & `corecon-1.4/corecon/data/quasar_luminosity_function/Ross_et_al_2013.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/quasar_luminosity_function/Willott_et_al_2010.py` & `corecon-1.4/corecon/data/quasar_luminosity_function/Willott_et_al_2010.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/quasar_luminosity_function/Yang_et_al_2016.py` & `corecon-1.4/corecon/data/quasar_luminosity_function/Yang_et_al_2016.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/sfrd/Donnan_et_al_2022.py` & `corecon-1.4/corecon/data/sfrd/Donnan_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/sfrd/Harikane_et_al_2022.py` & `corecon-1.4/corecon/data/sfrd/Harikane_et_al_2022.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/data/sfrd/Madau_and_Dickinson_2014.py` & `corecon-1.4/corecon/data/sfrd/Madau_and_Dickinson_2014.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon/fields_info.py` & `corecon-1.4/corecon/fields_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
-__fields_info__ = {  "ionized_fraction"                      : { "synonyms" : ['x_HII', 'f_HII', 'x_ion', 'f_ion', 'ion_frac']                                                         , "description" : "Ionized fraction"                                            , "symbol" : r"$x_\mathrm{HII}$"                                                          , "units" : ""             , "remarks": "volume-averaged", "required_fields" : ["redshift"]}  ,
+__fields_info__ = {  "HII_fraction"                          : { "synonyms" : ['ionized_fraction', 'x_HII', 'f_HII', 'x_ion', 'f_ion', 'ion_frac']                                     , "description" : "Hydrogen ionized fraction"                                   , "symbol" : r"$x_\mathrm{HII}$"                                                          , "units" : ""             , "remarks": "volume-averaged", "required_fields" : ["redshift"]}  ,
+                     "HeIII_fraction"                        : { "synonyms" : ['helium_ionized_fraction', 'ionized_fraction_helium', 'He_ion_frac', 'ion_frac_He']                     , "description" : "Helium doubly-ionized fraction"                              , "symbol" : r"$x_\mathrm{HeIII}$"                                                        , "units" : ""             , "remarks": "volume-averaged", "required_fields" : ["redshift"]}  ,
                      "Lya_flux_power_spectrum"               : { "synonyms" : ['Lya_flux_PS']                                                                                          , "description" : "Ly-alpha flux power spectrum"                                , "symbol" : r"$P\, [\mathrm{km/s}]$"                                                     , "units" : "km/s"         , "remarks": ""               , "required_fields" : ["redshift"]}  , 
                      "mean_free_path"                        : { "synonyms" : ['mfp', 'lambda_mfp', 'lambda_ion', 'lambda_912', 'mfp_912', 'mfp_ion']                                  , "description" : "Mean free path of ionising photons"                          , "symbol" : r"$\lambda_\mathrm{mfp} \, [h^{-1} \, \mathrm{Mpc}]$"                        , "units" : "Mpc/h"        , "remarks": ""               , "required_fields" : ["redshift"]}  , 
                      "effective_optical_depth_HI_Lya"        : { "synonyms" : ['tau_HI', 'tau_eff_HI']                                                                                 , "description" : "HI Ly-alpha effective optical depth"                         , "symbol" : r"$\tau_\mathrm{eff, HI}$"                                                   , "units" : ""             , "remarks": ""               , "required_fields" : ["redshift"]}  , 
                      "effective_optical_depth_HeII_Lya"      : { "synonyms" : ['tau_HeII', 'tau_eff_HeII']                                                                             , "description" : "HeII Ly-alpha effective optical depth"                       , "symbol" : r"$\tau_\mathrm{eff, HeII}$"                                                 , "units" : ""             , "remarks": ""               , "required_fields" : ["redshift"]}  , 
                      "HeII_to_HI_column_density_ratio"       : { "synonyms" : ['eta']                                                                                                  , "description" : "HeII-to-HI column density ratio"                             , "symbol" : r"$\eta$"                                                                    , "units" : ""             , "remarks": ""               , "required_fields" : ["redshift"]}  , 
                      "quasar_luminosity_function"            : { "synonyms" : ['QLF', 'QSOLF']                                                                                         , "description" : "Quasar luminosity function"                                  , "symbol" : r"$\log_{10} (phi_\mathrm{QSO}) \, [\mathrm{Mpc}^{-3} \, \mathrm{mag}^{-1}]$", "units" : "Mpc^-3 mag^-1", "remarks": ""               , "required_fields" : ["redshift", "M_1450"]}  , 
                      "UV_luminosity_function"                : { "synonyms" : ['UVLF']                                                                                                 , "description" : "Galaxy UV luminosity function"                               , "symbol" : r"$\log_{10} (phi_\mathrm{UV}) \, [\mathrm{Mpc}^{-3} \, \mathrm{mag}^{-1}]$" , "units" : "Mpc^-3 mag^-1", "remarks": ""               , "required_fields" : ["redshift", "M_UV"]  }  , 
@@ -12,12 +13,12 @@
                      "sfrd"                                  : { "synonyms" : ['SFRD', 'star formation rate density', 'star-formation-rate density', 'star-formation rate density']    , "description" : "Star-formation-rate density"                                 , "symbol" : r"$\log \Psi \, [\mathrm{M}_\odot \mathrm{yr}^{-1} \mathrm{Mpc}^{-3}]$"      , "units" : "Msun/yr/Mpc^3", "remarks": ""               , "required_fields" : ["redshift"]}  , 
                      "Lya_spike_galaxy_correlation"          : { "synonyms" : []                                                                                                       , "description" : "Ly-alpha spike - galaxy correlation"                         , "symbol" : r"$\langle f \rangle / \bar{f} - 1$"                                         , "units" : ""             , "remarks": ""               , "required_fields" : ["redshift"]}  ,
                      "mass_stellar_metallicity_relation"     : { "synonyms" : ['stellar MZR']                                                                                          , "description" : "Stellar metallicity as function of galaxy stellar mass"      , "symbol" : r"$\log(Z/Z_\odot)$"                                                         , "units" : ""             , "remarks": ""               , "required_fields" : ["redshift", "stellar mass"]}  ,
                      "mass_gas_metallicity_relation"         : { "synonyms" : ['gas MZR']                                                                                              , "description" : "Gas-phase O/H metallicity as function of galaxy stellar mass", "symbol" : r"$\log(O/H) + 12$"                                                          , "units" : ""             , "remarks": ""               , "required_fields" : ["redshift", "stellar mass"]}  ,
                      "galaxy_main_sequence"                  : { "synonyms" : ['GMS']                                                                                                  , "description" : "Star formation rate  as function of galaxy stellar mass"     , "symbol" : r"SFR [M$_\odot$/yr]"                                                        , "units" : "Msun/yr"      , "remarks": ""               , "required_fields" : ["redshift", "stellar mass"]}  ,
                      "UV_slope"                              : { "synonyms" : ['beta_UV']                                                                                              , "description" : "Slope of the galaxy UV log flux density"                     , "symbol" : r"$\beta$"                                                                   , "units" : ""             , "remarks": ""               , "required_fields" : ["redshift"]}  ,
                      "ionizing_photons_production_efficiency": { "synonyms" : ['xi_ion', 'csi_ion', 'ionizing_photon_production_efficiency', 'UV_to_ionizing_photons_conversion']      , "description" : "Number of ionizing photons produced per unit UV luminosity"  , "symbol" : r"$\log(\xi_\mathrm{ion} [\mathrm{Hz\,erg^{-1}}])$"                          , "units" : "Hz erg^-1"    , "remarks": ""               , "required_fields" : ["redshift"]}  ,
-                     "photoionization_rate"                  : { "synonyms" : ['photoionisation_rate', 'Gamma', 'GammaHI']                                                             , "description" : "Photoionsation rate of hydrogen in the IGM"                  , "symbol" : r"$\Gamma_\mathrm{HI}$ [s$^{-1}$]"                                           , "units" : "s^-1"         , "remarks": ""               , "required_fields" : ["redshift"]}  ,
+                     "HI_photoionization_rate"               : { "synonyms" : ['photoionization_rate', 'photoionisation_rate', 'Gamma', 'GammaHI']                                                             , "description" : "Photoionsation rate of hydrogen in the IGM"                  , "symbol" : r"$\Gamma_\mathrm{HI}$ [s$^{-1}$]"                                           , "units" : "s^-1"         , "remarks": ""               , "required_fields" : ["redshift"]}  ,
                      "ionizing_photons_emission_rate"        : { "synonyms" : ['ionizing_photons_production_rate', 'dotN', 'dotNion', 'Nion', 'N_ion']                                 , "description" : "Emission rate of ionizing photons per unit volume"           , "symbol" : r"$\dot{N}_\mathrm{ion}$ [s$^{-1}$ Mpc$^{-1}$]"                              , "units" : "s^-1 Mpc^-3"  , "remarks": ""               , "required_fields" : ["redshift"]}  ,
                      "reionization_midpoint"                 : { "synonyms" : ['z_mid']                                                                                                , "description" : "Redshift when x_HI = 0.5"                                    , "symbol" : r"$z_\mathrm{mid}$"                                                          , "units" : ""             , "remarks": ""               , "required_fields" : []          }  ,
                      "UV_luminosity_density"                 : { "synonyms" : ['rho_UV']                                                                                               , "description" : "Density of UV radiation in erg/s/Hz/Mpc^3"                   , "symbol" : r"$\log_{10} (\rho_\mathrm{UV}) \, [\mathrm{erg} \, \mathrm{s}^{-1} \, \mathrm{Hz}^{-1} \, \mathrm{Mpc}^{-3})$" , "units" : "erg s^-1 Hz^-1 Mpc^-3", "remarks": "", "required_fields" : ["redshift"]  }  , 
                   }
```

### Comparing `corecon-1.3/corecon/loaders.py` & `corecon-1.4/corecon/loaders.py`

 * *Files identical despite different names*

### Comparing `corecon-1.3/corecon.egg-info/PKG-INFO` & `corecon-1.4/corecon.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: corecon
-Version: 1.3
+Version: 1.4
 Summary: an open collection of constraints on the Epoch of Reionization
 Home-page: https://github.com/EGaraldi/corecon
-Download-URL: https://github.com/EGaraldi/corecon/archive/v1.3.tar.gz
+Download-URL: https://github.com/EGaraldi/corecon/archive/v1.4.tar.gz
 Author: Enrico Garaldi
 Author-email: enrico.garaldi@gmail.com
 License: gpl-3.0
 Keywords: constraints,reionization,cosmic,observations,data
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Build Tools
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE.txt
 
 ![](logo.png)
 
 [![DOI](https://zenodo.org/badge/224433919.svg)](https://zenodo.org/badge/latestdoi/224433919)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.05407/status.svg)](https://doi.org/10.21105/joss.05407)
```

### Comparing `corecon-1.3/corecon.egg-info/SOURCES.txt` & `corecon-1.4/corecon.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -15,14 +15,68 @@
 corecon.egg-info/SOURCES.txt
 corecon.egg-info/dependency_links.txt
 corecon.egg-info/requires.txt
 corecon.egg-info/top_level.txt
 corecon/data/__init__.py
 corecon/data/data_entry_template.py
 corecon/data/make_data_archive.py
+corecon/data/HII_fraction/Bolton_et_al_2011.py
+corecon/data/HII_fraction/Bosman_et_al_2022.py
+corecon/data/HII_fraction/Chornock_et_al_2013.py
+corecon/data/HII_fraction/Choudhury_et_al_2015.py
+corecon/data/HII_fraction/Choudhury_et_al_2021.py
+corecon/data/HII_fraction/Davies_et_al_2018.py
+corecon/data/HII_fraction/Dijkstra_et_al_2011.py
+corecon/data/HII_fraction/Durovcikova_et_al_2024.py
+corecon/data/HII_fraction/Fan_et_al_2006.py
+corecon/data/HII_fraction/Gaikwad_et_al_2023.py
+corecon/data/HII_fraction/Greig_et_al_2017.py
+corecon/data/HII_fraction/Greig_et_al_2019.py
+corecon/data/HII_fraction/Hoag_et_al_2019.py
+corecon/data/HII_fraction/Jensen_et_al_2013.py
+corecon/data/HII_fraction/Jung_et_al_2020.py
+corecon/data/HII_fraction/Lu_et_al_2020.py
+corecon/data/HII_fraction/Mason_et_al_2018.py
+corecon/data/HII_fraction/Mason_et_al_2019.py
+corecon/data/HII_fraction/McGreer_et_al_2011.py
+corecon/data/HII_fraction/McGreer_et_al_2015.py
+corecon/data/HII_fraction/Mesinger_et_al_2015.py
+corecon/data/HII_fraction/Mortlock_et_al_2011.py
+corecon/data/HII_fraction/Nakane_et_al_2024.py
+corecon/data/HII_fraction/Ono_et_al_2012.py
+corecon/data/HII_fraction/Ota_et_al_2008.py
+corecon/data/HII_fraction/Ouchi_et_al_2010.py
+corecon/data/HII_fraction/Pentericci_et_al_2014.py
+corecon/data/HII_fraction/Robertson_et_al_2013.py
+corecon/data/HII_fraction/Schenker_et_al_2014.py
+corecon/data/HII_fraction/Schroeder_et_al_2013.py
+corecon/data/HII_fraction/Sobacchi_Mesinger_2015.py
+corecon/data/HII_fraction/Tilvi_et_al_2014.py
+corecon/data/HII_fraction/Totani_et_al_2006.py
+corecon/data/HII_fraction/Umeda_et_al_2023.py
+corecon/data/HII_fraction/Wang_et_al_2020.py
+corecon/data/HII_fraction/Yang_et_al_2020.py
+corecon/data/HII_fraction/Yang_et_al_2020b.py
+corecon/data/HII_fraction/Zhu_et_al_2022.py
+corecon/data/HII_fraction/__init__.py
+corecon/data/HI_photoionization_rate/Becker_et_al_2013.py
+corecon/data/HI_photoionization_rate/Bolton_et_al_2007.py
+corecon/data/HI_photoionization_rate/Calverley_et_al_2011.py
+corecon/data/HI_photoionization_rate/DAloisio_et_al_2018.py
+corecon/data/HI_photoionization_rate/Davies_et_al_2018.py
+corecon/data/HI_photoionization_rate/Gaikwad_et_al_2017a.py
+corecon/data/HI_photoionization_rate/Gaikwad_et_al_2017b.py
+corecon/data/HI_photoionization_rate/Gaikwad_et_al_2023.py
+corecon/data/HI_photoionization_rate/Kollmeier_et_al_2014.py
+corecon/data/HI_photoionization_rate/Viel_et_al_2017.py
+corecon/data/HI_photoionization_rate/Wyithe_et_al_2011.py
+corecon/data/HeIII_fraction/Makan_et_al_2022.py
+corecon/data/HeIII_fraction/Worseck_et_al_2016.py
+corecon/data/HeIII_fraction/Worseck_et_al_2019.py
+corecon/data/HeIII_fraction/__init__.py
 corecon/data/HeII_to_HI_column_density_ratio/Syphers_and_Shull_2014.py
 corecon/data/HeII_to_HI_column_density_ratio/__init__.py
 corecon/data/IGM_temperature_mean_density/Becker_et_al_2011.py
 corecon/data/IGM_temperature_mean_density/Boera_et_al_2014.py
 corecon/data/IGM_temperature_mean_density/Boera_et_al_2018.py
 corecon/data/IGM_temperature_mean_density/Bolton_et_al_2010.py
 corecon/data/IGM_temperature_mean_density/Bolton_et_al_2012.py
@@ -51,43 +105,57 @@
 corecon/data/UV_luminosity_density/Bouwens_et_al_2022.py
 corecon/data/UV_luminosity_density/Donnan_et_al_2023.py
 corecon/data/UV_luminosity_density/Finkelstein_et_al_2023.py
 corecon/data/UV_luminosity_density/Harikane_et_al_2023.py
 corecon/data/UV_luminosity_density/McLeod_et_al_2023.py
 corecon/data/UV_luminosity_density/Perez-Gonzales_et_al_2023.py
 corecon/data/UV_luminosity_density/Willot_et_al_2023.py
+corecon/data/UV_luminosity_function/Adams_et_al_2023.py
 corecon/data/UV_luminosity_function/Atek_et_al_2015.py
 corecon/data/UV_luminosity_function/Atek_et_al_2018.py
 corecon/data/UV_luminosity_function/Bouwens_et_al_2015.py
 corecon/data/UV_luminosity_function/Bouwens_et_al_2016.py
 corecon/data/UV_luminosity_function/Bouwens_et_al_2017.py
 corecon/data/UV_luminosity_function/Bouwens_et_al_2022.py
+corecon/data/UV_luminosity_function/Bouwens_et_al_2023a.py
+corecon/data/UV_luminosity_function/Bouwens_et_al_2023b.py
 corecon/data/UV_luminosity_function/Bowler_et_al_2015.py
 corecon/data/UV_luminosity_function/Bowler_et_al_2020.py
+corecon/data/UV_luminosity_function/Casey_et_al_2023.py
 corecon/data/UV_luminosity_function/Castellano_et_al_2016.py
-corecon/data/UV_luminosity_function/Donnan_et_al_2022.py
+corecon/data/UV_luminosity_function/Donnan_et_al_2023a.py
+corecon/data/UV_luminosity_function/Donnan_et_al_2023b.py
+corecon/data/UV_luminosity_function/Donnan_et_al_2024.py
 corecon/data/UV_luminosity_function/Finkelstein_et_al_2015.py
 corecon/data/UV_luminosity_function/Finkelstein_et_al_2022.py
+corecon/data/UV_luminosity_function/Finkelstein_et_al_2023.py
 corecon/data/UV_luminosity_function/Harikane_et_al_2022.py
 corecon/data/UV_luminosity_function/Ishigaki_et_al_2018.py
 corecon/data/UV_luminosity_function/Kauffmann_et_al_2022.py
+corecon/data/UV_luminosity_function/Leung_et_al_2023.py
 corecon/data/UV_luminosity_function/Livermore_et_al_2017.py
 corecon/data/UV_luminosity_function/McLeod_et_al_2016.py
+corecon/data/UV_luminosity_function/McLeod_et_al_2024.py
 corecon/data/UV_luminosity_function/McLure_et_al_2013.py
 corecon/data/UV_luminosity_function/Morishita_et_al_2018.py
 corecon/data/UV_luminosity_function/Naidu_et_al_2022.py
 corecon/data/UV_luminosity_function/Oesch_et_al_2014.py
+corecon/data/UV_luminosity_function/Oesch_et_al_2018.py
+corecon/data/UV_luminosity_function/Perez-Gonzalez_et_al_2023.py
+corecon/data/UV_luminosity_function/Robertson_et_al_2023.py
 corecon/data/UV_luminosity_function/Rojas-Ruiz_et_al_2020.py
 corecon/data/UV_luminosity_function/Stefanon_et_al_2019.py
+corecon/data/UV_luminosity_function/Willott_et_al_2023.py
 corecon/data/UV_luminosity_function/__init__.py
 corecon/data/UV_slope/Atek_et_al_2023.py
 corecon/data/UV_slope/Austin_et_al_2023.py
 corecon/data/UV_slope/Bouwens_et_al_2009.py
 corecon/data/UV_slope/Cullen_et_al_2023.py
 corecon/data/UV_slope/Curtis-Lake_et_al_2022.py
+corecon/data/UV_slope/Donnan_et_al_2023.py
 corecon/data/UV_slope/Endsley_et_al_2022.py
 corecon/data/UV_slope/Finkelstein_et_al_2012.py
 corecon/data/UV_slope/Franco_et_al_2023.py
 corecon/data/UV_slope/Simmonds_et_al_2023.py
 corecon/data/UV_slope/Tacchella_et_al_2022.py
 corecon/data/UV_slope/Topping_et_al_2022.py
 corecon/data/UV_slope/Whitler_et_al_2022.py
@@ -97,58 +165,25 @@
 corecon/data/effective_optical_depth_HI_Lya/Bosman_et_al_2018.py
 corecon/data/effective_optical_depth_HI_Lya/Bosman_et_al_2022.py
 corecon/data/effective_optical_depth_HI_Lya/Eilers+18.py
 corecon/data/effective_optical_depth_HI_Lya/Fan_et_al_2006.py
 corecon/data/effective_optical_depth_HI_Lya/Liu_Bordoloi_2021.py
 corecon/data/effective_optical_depth_HI_Lya/Yang_et_al_2020.py
 corecon/data/effective_optical_depth_HI_Lya/__init__.py
+corecon/data/effective_optical_depth_HeII_Lya/Makan_et_al_2021.py
+corecon/data/effective_optical_depth_HeII_Lya/Makan_et_al_2022.py
 corecon/data/effective_optical_depth_HeII_Lya/Worseck_et_al_2016.py
+corecon/data/effective_optical_depth_HeII_Lya/Worseck_et_al_2019.py
 corecon/data/effective_optical_depth_HeII_Lya/__init__.py
 corecon/data/galaxy_main_sequence/Chen_et_al_2022.py
 corecon/data/galaxy_main_sequence/Finkelstein_et_al_2022.py
 corecon/data/galaxy_main_sequence/Leethochawali_et_al_2022.py
 corecon/data/galaxy_main_sequence/Roberts-Borsani_et_al_2022.py
 corecon/data/galaxy_main_sequence/Stefanon_et_al_2022.py
 corecon/data/galaxy_main_sequence/Tacchella_et_al_2022.py
-corecon/data/ionized_fraction/Bolton_et_al_2011.py
-corecon/data/ionized_fraction/Bosman_et_al_2022.py
-corecon/data/ionized_fraction/Chornock_et_al_2013.py
-corecon/data/ionized_fraction/Choudhury_et_al_2015.py
-corecon/data/ionized_fraction/Choudhury_et_al_2021.py
-corecon/data/ionized_fraction/Davies_et_al_2018.py
-corecon/data/ionized_fraction/Dijkstra_et_al_2011.py
-corecon/data/ionized_fraction/Fan_et_al_2006.py
-corecon/data/ionized_fraction/Gaikwad_et_al_2023.py
-corecon/data/ionized_fraction/Greig_et_al_2017.py
-corecon/data/ionized_fraction/Greig_et_al_2019.py
-corecon/data/ionized_fraction/Hoag_et_al_2019.py
-corecon/data/ionized_fraction/Jensen_et_al_2013.py
-corecon/data/ionized_fraction/Jung_et_al_2020.py
-corecon/data/ionized_fraction/Lu_et_al_2020.py
-corecon/data/ionized_fraction/Mason_et_al_2018.py
-corecon/data/ionized_fraction/Mason_et_al_2019.py
-corecon/data/ionized_fraction/McGreer_et_al_2011.py
-corecon/data/ionized_fraction/McGreer_et_al_2015.py
-corecon/data/ionized_fraction/Mesinger_et_al_2015.py
-corecon/data/ionized_fraction/Mortlock_et_al_2011.py
-corecon/data/ionized_fraction/Ono_et_al_2012.py
-corecon/data/ionized_fraction/Ota_et_al_2008.py
-corecon/data/ionized_fraction/Ouchi_et_al_2010.py
-corecon/data/ionized_fraction/Pentericci_et_al_2014.py
-corecon/data/ionized_fraction/Robertson_et_al_2013.py
-corecon/data/ionized_fraction/Schenker_et_al_2014.py
-corecon/data/ionized_fraction/Schroeder_et_al_2013.py
-corecon/data/ionized_fraction/Sobacchi_Mesinger_2015.py
-corecon/data/ionized_fraction/Tilvi_et_al_2014.py
-corecon/data/ionized_fraction/Totani_et_al_2006.py
-corecon/data/ionized_fraction/Wang_et_al_2020.py
-corecon/data/ionized_fraction/Yang_et_al_2020.py
-corecon/data/ionized_fraction/Yang_et_al_2020b.py
-corecon/data/ionized_fraction/Zhu_et_al_2022.py
-corecon/data/ionized_fraction/__init__.py
 corecon/data/ionizing_photons_emission_rate/Becker_et_al_2013.py
 corecon/data/ionizing_photons_emission_rate/Becker_et_al_2021.py
 corecon/data/ionizing_photons_emission_rate/Bouwens_et_al_2015.py
 corecon/data/ionizing_photons_emission_rate/Gaikwad_et_al_2023.py
 corecon/data/ionizing_photons_production_efficiency/Bouwens_et_al_2016.py
 corecon/data/ionizing_photons_production_efficiency/Bunker_et_al_2023.py
 corecon/data/ionizing_photons_production_efficiency/Endsley_et_al_2022.py
@@ -165,14 +200,15 @@
 corecon/data/mass_gas_metallicity_relation/Faisst_et_al_2016.py
 corecon/data/mass_gas_metallicity_relation/Fujimoto_et_al_2023.py
 corecon/data/mass_gas_metallicity_relation/Langeroodi_et_al_2022.py
 corecon/data/mass_gas_metallicity_relation/Nakajima_et_al_2023.py
 corecon/data/mass_gas_metallicity_relation/Roberts-Borsani_et_al_2022.py
 corecon/data/mass_gas_metallicity_relation/Schaerer_et_al_2022.py
 corecon/data/mass_gas_metallicity_relation/Trump_et_al_2023.py
+corecon/data/mass_gas_metallicity_relation/Venturi_et_al_2024.py
 corecon/data/mass_gas_metallicity_relation/Williams_et_al_2023.py
 corecon/data/mass_stellar_metallicity_relation/Furtak_et_al_2022.py
 corecon/data/mass_stellar_metallicity_relation/Tacchella_et_al_2022.py
 corecon/data/mean_free_path/Becker_et_al_2021.py
 corecon/data/mean_free_path/Bosman_et_al_2021.py
 corecon/data/mean_free_path/DAloisio_et_al_2018.py
 corecon/data/mean_free_path/Fumagalli_et_al_2013.py
@@ -187,19 +223,14 @@
 corecon/data/optical_depth_CMB/Planck_2015.py
 corecon/data/optical_depth_CMB/Planck_2018.py
 corecon/data/optical_depth_CMB/WMAP_5yr.py
 corecon/data/optical_depth_CMB/WMAP_7yr.py
 corecon/data/optical_depth_CMB/WMAP_9yr.py
 corecon/data/optical_depth_CMB/__init__.py
 corecon/data/optical_depth_CMB/deBelsunce_et_al_2021.py
-corecon/data/photoionization_rate/Bolton_et_al_2007.py
-corecon/data/photoionization_rate/Calverley_et_al_2011.py
-corecon/data/photoionization_rate/DAloisio_et_al_2018.py
-corecon/data/photoionization_rate/Gaikwad_et_al_2023.py
-corecon/data/photoionization_rate/Wyithe_et_al_2011.py
 corecon/data/quasar_luminosity_function/Giallongo_et_al_2015.py
 corecon/data/quasar_luminosity_function/Giallongo_et_al_2019.py
 corecon/data/quasar_luminosity_function/Glikman_et_al_2011.py
 corecon/data/quasar_luminosity_function/Jiang_et_al_2016.py
 corecon/data/quasar_luminosity_function/Kashikawa_et_al_2015.py
 corecon/data/quasar_luminosity_function/Kulkarni_et_al_2019.py
 corecon/data/quasar_luminosity_function/McGreer_et_al_2013.py
```

### Comparing `corecon-1.3/setup.py` & `corecon-1.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,9 +28,10 @@
     'Programming Language :: Python :: 3.4',
     'Programming Language :: Python :: 3.5',
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
   ],
 )
```

