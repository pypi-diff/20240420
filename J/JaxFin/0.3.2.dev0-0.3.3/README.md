# Comparing `tmp/JaxFin-0.3.2.dev0.tar.gz` & `tmp/jaxfin-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JaxFin-0.3.2.dev0.tar", last modified: Fri Apr 12 16:00:42 2024, max compression
+gzip compressed data, was "jaxfin-0.3.3.tar", last modified: Sat Apr 20 16:41:38 2024, max compression
```

## Comparing `JaxFin-0.3.2.dev0.tar` & `jaxfin-0.3.3.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.726980 JaxFin-0.3.2.dev0/
-drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.230162 JaxFin-0.3.2.dev0/.github/
-drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.331615 JaxFin-0.3.2.dev0/.github/workflows/
--rw-rw-rw-   0        0        0      597 2024-03-17 17:34:48.000000 JaxFin-0.3.2.dev0/.github/workflows/linting.yml
--rw-rw-rw-   0        0        0      617 2024-02-20 14:16:18.000000 JaxFin-0.3.2.dev0/.github/workflows/pytest.yml
--rw-rw-rw-   0        0        0      822 2024-03-05 14:09:37.000000 JaxFin-0.3.2.dev0/.github/workflows/quality_check.yml
--rw-rw-rw-   0        0        0      497 2024-03-17 17:29:55.000000 JaxFin-0.3.2.dev0/.gitignore
-drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.402893 JaxFin-0.3.2.dev0/.idea/
--rw-rw-rw-   0        0        0      184 2023-11-27 18:39:40.000000 JaxFin-0.3.2.dev0/.idea/.gitignore
--rw-rw-rw-   0        0        0      435 2024-03-05 13:42:17.000000 JaxFin-0.3.2.dev0/.idea/aws.xml
-drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.414401 JaxFin-0.3.2.dev0/.idea/inspectionProfiles/
--rw-rw-rw-   0        0        0      179 2023-11-27 18:39:40.000000 JaxFin-0.3.2.dev0/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-rw-   0        0        0      434 2024-02-20 14:21:44.000000 JaxFin-0.3.2.dev0/.idea/misc.xml
--rw-rw-rw-   0        0        0      283 2023-11-27 18:39:40.000000 JaxFin-0.3.2.dev0/.idea/modules.xml
--rw-rw-rw-   0        0        0      191 2023-12-15 20:40:10.000000 JaxFin-0.3.2.dev0/.idea/other.xml
--rw-rw-rw-   0        0        0      409 2024-02-20 14:21:44.000000 JaxFin-0.3.2.dev0/.idea/py-exopricer.iml
--rw-rw-rw-   0        0        0      172 2023-11-27 18:39:40.000000 JaxFin-0.3.2.dev0/.idea/vcs.xml
--rw-rw-rw-   0        0        0     2418 2024-02-16 14:21:51.000000 JaxFin-0.3.2.dev0/CONTRIBUTING.md
-drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.715816 JaxFin-0.3.2.dev0/JaxFin.egg-info/
--rw-rw-rw-   0        0        0     7521 2024-04-12 16:00:41.000000 JaxFin-0.3.2.dev0/JaxFin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1608 2024-04-12 16:00:42.000000 JaxFin-0.3.2.dev0/JaxFin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 16:00:41.000000 JaxFin-0.3.2.dev0/JaxFin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-12 16:00:41.000000 JaxFin-0.3.2.dev0/JaxFin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-12 16:00:41.000000 JaxFin-0.3.2.dev0/JaxFin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-02-10 17:05:30.000000 JaxFin-0.3.2.dev0/LICENSE
--rw-rw-rw-   0        0        0      660 2024-04-12 15:55:17.000000 JaxFin-0.3.2.dev0/Makefile
--rw-rw-rw-   0        0        0     7521 2024-04-12 16:00:42.715816 JaxFin-0.3.2.dev0/PKG-INFO
--rw-rw-rw-   0        0        0     6632 2024-04-03 15:58:34.000000 JaxFin-0.3.2.dev0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.470896 JaxFin-0.3.2.dev0/jaxfin/
--rw-rw-rw-   0        0        0        0 2024-02-17 09:50:48.000000 JaxFin-0.3.2.dev0/jaxfin/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.476555 JaxFin-0.3.2.dev0/jaxfin/models/
--rw-rw-rw-   0        0        0      211 2024-02-17 10:10:13.000000 JaxFin-0.3.2.dev0/jaxfin/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.510543 JaxFin-0.3.2.dev0/jaxfin/models/gbm/
--rw-rw-rw-   0        0        0      230 2024-02-20 14:21:44.000000 JaxFin-0.3.2.dev0/jaxfin/models/gbm/__init__.py
--rw-rw-rw-   0        0        0     7604 2024-03-07 14:43:03.000000 JaxFin-0.3.2.dev0/jaxfin/models/gbm/gbm.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.515813 JaxFin-0.3.2.dev0/jaxfin/models/heston/
--rw-rw-rw-   0        0        0      159 2024-03-07 14:43:03.000000 JaxFin-0.3.2.dev0/jaxfin/models/heston/__init__.py
--rw-rw-rw-   0        0        0    11977 2024-04-12 15:56:31.000000 JaxFin-0.3.2.dev0/jaxfin/models/heston/heston.py
--rw-rw-rw-   0        0        0      381 2024-03-07 14:43:03.000000 JaxFin-0.3.2.dev0/jaxfin/models/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.518954 JaxFin-0.3.2.dev0/jaxfin/price_engine/
--rw-rw-rw-   0        0        0        0 2024-02-17 09:50:48.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.525551 JaxFin-0.3.2.dev0/jaxfin/price_engine/black/
--rw-rw-rw-   0        0        0      249 2024-02-20 14:16:18.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/black/__init__.py
--rw-rw-rw-   0        0        0     4809 2024-03-05 14:09:37.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/black/black_model.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.531700 JaxFin-0.3.2.dev0/jaxfin/price_engine/black_scholes/
--rw-rw-rw-   0        0        0      423 2024-03-04 19:28:01.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/black_scholes/__init__.py
--rw-rw-rw-   0        0        0     8033 2024-03-05 14:09:37.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/black_scholes/vanilla_options.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.537226 JaxFin-0.3.2.dev0/jaxfin/price_engine/fft/
--rw-rw-rw-   0        0        0      290 2024-04-03 15:58:34.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/fft/__init__.py
--rw-rw-rw-   0        0        0     5916 2024-04-03 15:58:34.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/fft/vanilla_options.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.546009 JaxFin-0.3.2.dev0/jaxfin/price_engine/math/
--rw-rw-rw-   0        0        0        0 2024-03-05 14:09:37.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/math/__init__.py
--rw-rw-rw-   0        0        0     2609 2024-03-05 14:09:37.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/math/bs_common.py
--rw-rw-rw-   0        0        0      640 2024-03-05 14:09:37.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/math/norm.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.552376 JaxFin-0.3.2.dev0/jaxfin/price_engine/utils/
--rw-rw-rw-   0        0        0        0 2024-03-05 14:09:37.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/utils/__init__.py
--rw-rw-rw-   0        0        0      920 2024-03-05 14:09:37.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/utils/arrays.py
--rw-rw-rw-   0        0        0     2788 2024-03-05 14:09:37.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/utils/vect.py
--rw-rw-rw-   0        0        0      175 2024-02-10 14:03:34.000000 JaxFin-0.3.2.dev0/noxfile.py
--rw-rw-rw-   0        0        0    23014 2024-03-23 15:48:12.000000 JaxFin-0.3.2.dev0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.577593 JaxFin-0.3.2.dev0/requirements/
--rw-rw-rw-   0        0        0      505 2024-03-17 17:32:57.000000 JaxFin-0.3.2.dev0/requirements/build.txt
--rw-rw-rw-   0        0        0     2528 2024-03-17 17:26:30.000000 JaxFin-0.3.2.dev0/requirements/dev.txt
-drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.692484 JaxFin-0.3.2.dev0/scripts/
--rwxrwxrwx   0        0        0       61 2023-12-19 18:23:50.000000 JaxFin-0.3.2.dev0/scripts/basedir.bat
--rwxrwxrwx   0        0        0       68 2024-02-10 16:19:46.000000 JaxFin-0.3.2.dev0/scripts/black-reformat.bat
--rwxrwxrwx   0        0        0       76 2024-02-10 16:19:46.000000 JaxFin-0.3.2.dev0/scripts/check-black.bat
--rwxrwxrwx   0        0        0      376 2024-02-17 11:13:18.000000 JaxFin-0.3.2.dev0/scripts/configure-python.bat
--rwxrwxrwx   0        0        0      720 2024-02-17 11:22:03.000000 JaxFin-0.3.2.dev0/scripts/create-new-version.bat
--rwxrwxrwx   0        0        0      102 2024-02-20 14:16:18.000000 JaxFin-0.3.2.dev0/scripts/get-tests-cov.bat
--rwxrwxrwx   0        0        0       96 2024-03-17 17:31:24.000000 JaxFin-0.3.2.dev0/scripts/run-linter.bat
--rwxrwxrwx   0        0        0       69 2024-02-10 17:00:41.000000 JaxFin-0.3.2.dev0/scripts/run-mypy.bat
--rwxrwxrwx   0        0        0      126 2024-02-10 16:58:40.000000 JaxFin-0.3.2.dev0/scripts/run-tests.bat
--rw-rw-rw-   0        0        0       42 2024-04-12 16:00:42.726980 JaxFin-0.3.2.dev0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.692484 JaxFin-0.3.2.dev0/tests/
--rw-rw-rw-   0        0        0        0 2023-11-27 18:43:58.000000 JaxFin-0.3.2.dev0/tests/.gitkeep
-drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.705422 JaxFin-0.3.2.dev0/tests/models/
--rw-rw-rw-   0        0        0     1760 2024-04-03 15:58:34.000000 JaxFin-0.3.2.dev0/tests/models/test_gbm.py
--rw-rw-rw-   0        0        0     3396 2024-04-12 15:50:02.000000 JaxFin-0.3.2.dev0/tests/models/test_heston.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.715433 JaxFin-0.3.2.dev0/tests/price_engine/
--rw-rw-rw-   0        0        0     6518 2024-04-03 15:58:34.000000 JaxFin-0.3.2.dev0/tests/price_engine/test_black.py
--rw-rw-rw-   0        0        0    11089 2024-04-03 15:58:34.000000 JaxFin-0.3.2.dev0/tests/price_engine/test_bs.py
--rw-rw-rw-   0        0        0     3335 2024-04-03 15:58:34.000000 JaxFin-0.3.2.dev0/tests/price_engine/test_fft.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:41:38.306327 jaxfin-0.3.3/
+drwxrwxrwx   0        0        0        0 2024-04-20 16:41:37.649815 jaxfin-0.3.3/.github/
+drwxrwxrwx   0        0        0        0 2024-04-20 16:41:37.771052 jaxfin-0.3.3/.github/workflows/
+-rw-rw-rw-   0        0        0      597 2024-03-17 17:34:48.000000 jaxfin-0.3.3/.github/workflows/linting.yml
+-rw-rw-rw-   0        0        0      617 2024-02-20 14:16:18.000000 jaxfin-0.3.3/.github/workflows/pytest.yml
+-rw-rw-rw-   0        0        0      822 2024-03-05 14:09:37.000000 jaxfin-0.3.3/.github/workflows/quality_check.yml
+-rw-rw-rw-   0        0        0      497 2024-03-17 17:29:55.000000 jaxfin-0.3.3/.gitignore
+drwxrwxrwx   0        0        0        0 2024-04-20 16:41:37.848628 jaxfin-0.3.3/.idea/
+-rw-rw-rw-   0        0        0      184 2023-11-27 18:39:40.000000 jaxfin-0.3.3/.idea/.gitignore
+-rw-rw-rw-   0        0        0      435 2024-04-20 10:33:19.000000 jaxfin-0.3.3/.idea/aws.xml
+drwxrwxrwx   0        0        0        0 2024-04-20 16:41:37.859656 jaxfin-0.3.3/.idea/inspectionProfiles/
+-rw-rw-rw-   0        0        0      179 2023-11-27 18:39:40.000000 jaxfin-0.3.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0        0        0      434 2024-04-20 16:35:09.000000 jaxfin-0.3.3/.idea/misc.xml
+-rw-rw-rw-   0        0        0      283 2023-11-27 18:39:40.000000 jaxfin-0.3.3/.idea/modules.xml
+-rw-rw-rw-   0        0        0      191 2023-12-15 20:40:10.000000 jaxfin-0.3.3/.idea/other.xml
+-rw-rw-rw-   0        0        0      409 2024-04-20 16:35:11.000000 jaxfin-0.3.3/.idea/py-exopricer.iml
+-rw-rw-rw-   0        0        0      172 2023-11-27 18:39:40.000000 jaxfin-0.3.3/.idea/vcs.xml
+-rw-rw-rw-   0        0        0     2418 2024-02-16 14:21:51.000000 jaxfin-0.3.3/CONTRIBUTING.md
+drwxrwxrwx   0        0        0        0 2024-04-20 16:41:38.296296 jaxfin-0.3.3/JaxFin.egg-info/
+-rw-rw-rw-   0        0        0     7516 2024-04-20 16:41:37.000000 jaxfin-0.3.3/JaxFin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1624 2024-04-20 16:41:37.000000 jaxfin-0.3.3/JaxFin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 16:41:37.000000 jaxfin-0.3.3/JaxFin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-20 16:41:37.000000 jaxfin-0.3.3/JaxFin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-20 16:41:37.000000 jaxfin-0.3.3/JaxFin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-02-10 17:05:30.000000 jaxfin-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0      668 2024-04-19 09:13:49.000000 jaxfin-0.3.3/Makefile
+-rw-rw-rw-   0        0        0     7516 2024-04-20 16:41:38.303371 jaxfin-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6632 2024-04-03 15:58:34.000000 jaxfin-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 16:41:37.935714 jaxfin-0.3.3/jaxfin/
+-rw-rw-rw-   0        0        0        0 2024-02-17 09:50:48.000000 jaxfin-0.3.3/jaxfin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:41:37.941039 jaxfin-0.3.3/jaxfin/models/
+-rw-rw-rw-   0        0        0      211 2024-02-17 10:10:13.000000 jaxfin-0.3.3/jaxfin/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:41:37.951574 jaxfin-0.3.3/jaxfin/models/gbm/
+-rw-rw-rw-   0        0        0      230 2024-02-20 14:21:44.000000 jaxfin-0.3.3/jaxfin/models/gbm/__init__.py
+-rw-rw-rw-   0        0        0     7562 2024-04-19 09:13:49.000000 jaxfin-0.3.3/jaxfin/models/gbm/gbm.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:41:37.956950 jaxfin-0.3.3/jaxfin/models/heston/
+-rw-rw-rw-   0        0        0      159 2024-03-07 14:43:03.000000 jaxfin-0.3.3/jaxfin/models/heston/__init__.py
+-rw-rw-rw-   0        0        0    11977 2024-04-19 09:13:49.000000 jaxfin-0.3.3/jaxfin/models/heston/heston.py
+-rw-rw-rw-   0        0        0      381 2024-03-07 14:43:03.000000 jaxfin-0.3.3/jaxfin/models/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:41:37.959826 jaxfin-0.3.3/jaxfin/price_engine/
+-rw-rw-rw-   0        0        0        0 2024-02-17 09:50:48.000000 jaxfin-0.3.3/jaxfin/price_engine/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:41:37.969456 jaxfin-0.3.3/jaxfin/price_engine/black/
+-rw-rw-rw-   0        0        0      249 2024-02-20 14:16:18.000000 jaxfin-0.3.3/jaxfin/price_engine/black/__init__.py
+-rw-rw-rw-   0        0        0     4809 2024-03-05 14:09:37.000000 jaxfin-0.3.3/jaxfin/price_engine/black/black_model.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:41:37.976065 jaxfin-0.3.3/jaxfin/price_engine/black_scholes/
+-rw-rw-rw-   0        0        0      423 2024-03-04 19:28:01.000000 jaxfin-0.3.3/jaxfin/price_engine/black_scholes/__init__.py
+-rw-rw-rw-   0        0        0     8033 2024-04-20 16:35:37.000000 jaxfin-0.3.3/jaxfin/price_engine/black_scholes/vanilla_options.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:41:37.986011 jaxfin-0.3.3/jaxfin/price_engine/fft/
+-rw-rw-rw-   0        0        0      290 2024-04-03 15:58:34.000000 jaxfin-0.3.3/jaxfin/price_engine/fft/__init__.py
+-rw-rw-rw-   0        0        0     5916 2024-04-03 15:58:34.000000 jaxfin-0.3.3/jaxfin/price_engine/fft/vanilla_options.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:41:37.998148 jaxfin-0.3.3/jaxfin/price_engine/math/
+-rw-rw-rw-   0        0        0        0 2024-03-05 14:09:37.000000 jaxfin-0.3.3/jaxfin/price_engine/math/__init__.py
+-rw-rw-rw-   0        0        0     2609 2024-03-05 14:09:37.000000 jaxfin-0.3.3/jaxfin/price_engine/math/bs_common.py
+-rw-rw-rw-   0        0        0      640 2024-03-05 14:09:37.000000 jaxfin-0.3.3/jaxfin/price_engine/math/norm.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:41:38.004203 jaxfin-0.3.3/jaxfin/price_engine/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-05 14:09:37.000000 jaxfin-0.3.3/jaxfin/price_engine/utils/__init__.py
+-rw-rw-rw-   0        0        0      920 2024-03-05 14:09:37.000000 jaxfin-0.3.3/jaxfin/price_engine/utils/arrays.py
+-rw-rw-rw-   0        0        0     2788 2024-03-05 14:09:37.000000 jaxfin-0.3.3/jaxfin/price_engine/utils/vect.py
+-rw-rw-rw-   0        0        0        0 2024-04-20 16:36:00.000000 jaxfin-0.3.3/jaxfin/py.typed
+-rw-rw-rw-   0        0        0      175 2024-02-10 14:03:34.000000 jaxfin-0.3.3/noxfile.py
+-rw-rw-rw-   0        0        0    23014 2024-03-23 15:48:12.000000 jaxfin-0.3.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-20 16:41:38.038098 jaxfin-0.3.3/requirements/
+-rw-rw-rw-   0        0        0      505 2024-03-17 17:32:57.000000 jaxfin-0.3.3/requirements/build.txt
+-rw-rw-rw-   0        0        0     2528 2024-03-17 17:26:30.000000 jaxfin-0.3.3/requirements/dev.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 16:41:38.234314 jaxfin-0.3.3/scripts/
+-rwxrwxrwx   0        0        0       61 2023-12-19 18:23:50.000000 jaxfin-0.3.3/scripts/basedir.bat
+-rwxrwxrwx   0        0        0       68 2024-02-10 16:19:46.000000 jaxfin-0.3.3/scripts/black-reformat.bat
+-rwxrwxrwx   0        0        0       76 2024-02-10 16:19:46.000000 jaxfin-0.3.3/scripts/check-black.bat
+-rwxrwxrwx   0        0        0      376 2024-02-17 11:13:18.000000 jaxfin-0.3.3/scripts/configure-python.bat
+-rwxrwxrwx   0        0        0      720 2024-02-17 11:22:03.000000 jaxfin-0.3.3/scripts/create-new-version.bat
+-rwxrwxrwx   0        0        0      102 2024-02-20 14:16:18.000000 jaxfin-0.3.3/scripts/get-tests-cov.bat
+-rwxrwxrwx   0        0        0       96 2024-03-17 17:31:24.000000 jaxfin-0.3.3/scripts/run-linter.bat
+-rwxrwxrwx   0        0        0       69 2024-02-10 17:00:41.000000 jaxfin-0.3.3/scripts/run-mypy.bat
+-rwxrwxrwx   0        0        0      126 2024-02-10 16:58:40.000000 jaxfin-0.3.3/scripts/run-tests.bat
+-rw-rw-rw-   0        0        0       42 2024-04-20 16:41:38.313695 jaxfin-0.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-20 16:41:38.235938 jaxfin-0.3.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-11-27 18:43:58.000000 jaxfin-0.3.3/tests/.gitkeep
+drwxrwxrwx   0        0        0        0 2024-04-20 16:41:38.276506 jaxfin-0.3.3/tests/models/
+-rw-rw-rw-   0        0        0     1792 2024-04-19 09:13:49.000000 jaxfin-0.3.3/tests/models/test_gbm.py
+-rw-rw-rw-   0        0        0     3396 2024-04-19 09:13:49.000000 jaxfin-0.3.3/tests/models/test_heston.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:41:38.292219 jaxfin-0.3.3/tests/price_engine/
+-rw-rw-rw-   0        0        0     6518 2024-04-03 15:58:34.000000 jaxfin-0.3.3/tests/price_engine/test_black.py
+-rw-rw-rw-   0        0        0    11089 2024-04-03 15:58:34.000000 jaxfin-0.3.3/tests/price_engine/test_bs.py
+-rw-rw-rw-   0        0        0     3335 2024-04-03 15:58:34.000000 jaxfin-0.3.3/tests/price_engine/test_fft.py
```

### Comparing `JaxFin-0.3.2.dev0/.github/workflows/linting.yml` & `jaxfin-0.3.3/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.2.dev0/.github/workflows/pytest.yml` & `jaxfin-0.3.3/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.2.dev0/.github/workflows/quality_check.yml` & `jaxfin-0.3.3/.github/workflows/quality_check.yml`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.2.dev0/CONTRIBUTING.md` & `jaxfin-0.3.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.2.dev0/JaxFin.egg-info/PKG-INFO` & `jaxfin-0.3.3/JaxFin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JaxFin
-Version: 0.3.2.dev0
+Version: 0.3.3
 Summary: JaxFin is a powerful and versatile Python library designed for pricing exotic options using a range of advanced financial techniques.
 Author-email: Paolo D'Elia <paolo.delia99@gmail.com>, Samuele D'Elia <delia.samuele00@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `JaxFin-0.3.2.dev0/JaxFin.egg-info/SOURCES.txt` & `jaxfin-0.3.3/JaxFin.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 .idea/inspectionProfiles/profiles_settings.xml
 JaxFin.egg-info/PKG-INFO
 JaxFin.egg-info/SOURCES.txt
 JaxFin.egg-info/dependency_links.txt
 JaxFin.egg-info/requires.txt
 JaxFin.egg-info/top_level.txt
 jaxfin/__init__.py
+jaxfin/py.typed
 jaxfin/models/__init__.py
 jaxfin/models/utils.py
 jaxfin/models/gbm/__init__.py
 jaxfin/models/gbm/gbm.py
 jaxfin/models/heston/__init__.py
 jaxfin/models/heston/heston.py
 jaxfin/price_engine/__init__.py
```

### Comparing `JaxFin-0.3.2.dev0/LICENSE` & `jaxfin-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.2.dev0/Makefile` & `jaxfin-0.3.3/Makefile`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 SHELL=/bin/bash
 LINT_PATHS=jaxfin/ tests/
 
+build:
+	python -m build
+
 pytest:
 	python -m pytest --no-header -vv --html=test_report.html --self-contained-html
 
 pylint:
 	pylint jaxfin --output-format=text:pylint_res.txt,colorized
 
 type: 
@@ -21,15 +24,15 @@
 
 check-codestyle:
 	black ${LINT_PATHS} --check
 
 commit-checks: format type lint
 
 release: 
-	python -m build
+	build
 	twine upload dist/*
 
 test-release: 
-	python -m build
+	build
 	twine upload dist/* -r testpypi
 
 .PHONY: clean spelling doc lint format check-codestyle commit-checks pylint
```

### Comparing `JaxFin-0.3.2.dev0/PKG-INFO` & `jaxfin-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JaxFin
-Version: 0.3.2.dev0
+Version: 0.3.3
 Summary: JaxFin is a powerful and versatile Python library designed for pricing exotic options using a range of advanced financial techniques.
 Author-email: Paolo D'Elia <paolo.delia99@gmail.com>, Samuele D'Elia <delia.samuele00@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `JaxFin-0.3.2.dev0/README.md` & `jaxfin-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.2.dev0/jaxfin/models/gbm/gbm.py` & `jaxfin-0.3.3/jaxfin/models/gbm/gbm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Geometric Brownian Motion class implementation"""
 from typing import List, Optional, Union
 
 import jax
 import jax.numpy as jnp
-from jax import random
+import numpy as np
 
 from ..utils import check_symmetric
 
 
 class UnivGeometricBrownianMotion:
     """
     Geometric Brownian Motion
@@ -81,38 +81,38 @@
         """Return the underlying dtype of the GBM
 
         Returns:
             jax.numpy.dtype: The dtype of the GBM
         """
         return self._dtype
 
-    def sample_paths(self, seed: int, maturity: float, n: int, n_sim: int) -> jax.Array:
+    def sample_paths(self, maturity: float, n: int, n_sim: int) -> jax.Array:
         """
         Simulate a sample of paths from the Geometric Brownian Motion (GBM).
 
         Args:
             maturity (float): Time in years.
             n (int): Number of steps.
             n_sim (int): Number of simulations.
 
         Returns:
             jax.Array: Array containing the sample paths.
         """
-        key = random.PRNGKey(seed)
-
         dt = maturity / n
 
-        Xt = jnp.exp(
+        Xt = np.exp(
             (self._mean - self._sigma**2 / 2) * dt
-            + self._sigma * jnp.sqrt(dt) * random.normal(key, shape=(n_sim, n - 1)).T
+            + self._sigma
+            * np.sqrt(dt)
+            * np.random.normal(loc=0, scale=1, size=(n_sim, n - 1)).T
         )
 
-        Xt = jnp.vstack([jnp.ones(n_sim), Xt])
+        Xt = np.vstack([np.ones(n_sim), Xt])
 
-        return self._s0 * Xt.cumprod(axis=0)
+        return jnp.asarray(self._s0 * Xt.cumprod(axis=0))
 
 
 class MultiGeometricBrownianMotion:
     """
     Geometric Brownian Motion
 
     Represent a d-dimensional GBM
@@ -203,32 +203,30 @@
     @property
     def dimension(self) -> int:
         """
         :return: Returns the dimension of the GBM
         """
         return self._dim
 
-    def sample_paths(self, seed: int, maturity: float, n: int, n_sim: int) -> jax.Array:
+    def sample_paths(self, maturity: float, n: int, n_sim: int) -> jax.Array:
         """
         Simulate a sample of paths from the Multivariate Geometric Brownian Motion (GBM).
 
         Args:
             maturity (float): Time in years.
             n (int): Number of steps.
             n_sim (int): Number of simulations.
 
         Returns:
             jax.Array: Array containing the sample paths.
         """
-        key = random.PRNGKey(seed)
-
         dt = maturity / n
 
-        normal_draw = random.normal(key, shape=(n_sim, n * self._dim))
-        normal_draw = jnp.reshape(normal_draw, (n_sim, n, self._dim)).transpose(
+        normal_draw = np.random.normal(loc=0, scale=1, size=(n_sim, n * self._dim))
+        normal_draw = np.reshape(normal_draw, (n_sim, n, self._dim)).transpose(
             (1, 0, 2)
         )
 
         cholesky_matrix = jnp.linalg.cholesky(self._corr)
 
         stochastic_increments = normal_draw @ cholesky_matrix
```

### Comparing `JaxFin-0.3.2.dev0/jaxfin/models/heston/heston.py` & `jaxfin-0.3.3/jaxfin/models/heston/heston.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.2.dev0/jaxfin/price_engine/black/black_model.py` & `jaxfin-0.3.3/jaxfin/price_engine/black/black_model.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.2.dev0/jaxfin/price_engine/black_scholes/vanilla_options.py` & `jaxfin-0.3.3/jaxfin/price_engine/black_scholes/vanilla_options.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.2.dev0/jaxfin/price_engine/fft/vanilla_options.py` & `jaxfin-0.3.3/jaxfin/price_engine/fft/vanilla_options.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.2.dev0/jaxfin/price_engine/math/bs_common.py` & `jaxfin-0.3.3/jaxfin/price_engine/math/bs_common.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.2.dev0/jaxfin/price_engine/math/norm.py` & `jaxfin-0.3.3/jaxfin/price_engine/math/norm.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.2.dev0/jaxfin/price_engine/utils/arrays.py` & `jaxfin-0.3.3/jaxfin/price_engine/utils/arrays.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.2.dev0/jaxfin/price_engine/utils/vect.py` & `jaxfin-0.3.3/jaxfin/price_engine/utils/vect.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.2.dev0/pyproject.toml` & `jaxfin-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.2.dev0/requirements/dev.txt` & `jaxfin-0.3.3/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.2.dev0/scripts/create-new-version.bat` & `jaxfin-0.3.3/scripts/create-new-version.bat`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.2.dev0/tests/models/test_gbm.py` & `jaxfin-0.3.3/tests/models/test_gbm.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import jax.numpy as jnp
+import numpy as np
 
 from jaxfin.models.gbm import MultiGeometricBrownianMotion, UnivGeometricBrownianMotion
 
 SEED: int = 42
 
+np.random.seed(SEED)
+
 
 class TestUnivGBM:
     def test_init(self):
         s0 = 10
         mean = 0.1
         sigma = 0.3
         dtype = jnp.float32
@@ -21,15 +24,15 @@
     def test_sim_paths_shape(self):
         s0 = 10
         mean = 0.1
         sigma = 0.3
         dtype = jnp.float32
         gbm = UnivGeometricBrownianMotion(s0, mean, sigma, dtype)
 
-        stock_paths = gbm.sample_paths(SEED, 1.0, 52, 100)
+        stock_paths = gbm.sample_paths(1.0, 52, 100)
 
         assert stock_paths.shape == (52, 100)
 
 
 class TestMultiGBM:
     def test_init(self):
         s0 = jnp.array([10, 12])
@@ -49,10 +52,10 @@
     def test_sample_path(self):
         s0 = jnp.array([10, 12])
         mean = jnp.array([0.1, 0.0])
         sigma = jnp.array([0.3, 0.5])
         corr = jnp.array([[1, 0.1], [0.1, 1]])
         dtype = jnp.float32
         gbm = MultiGeometricBrownianMotion(s0, mean, sigma, corr, dtype)
-        sample_path = gbm.sample_paths(SEED, 1.0, 52, 100)
+        sample_path = gbm.sample_paths(1.0, 52, 100)
 
         assert sample_path.shape == (52, 100, 2)
```

### Comparing `JaxFin-0.3.2.dev0/tests/models/test_heston.py` & `jaxfin-0.3.3/tests/models/test_heston.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.2.dev0/tests/price_engine/test_black.py` & `jaxfin-0.3.3/tests/price_engine/test_black.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.2.dev0/tests/price_engine/test_bs.py` & `jaxfin-0.3.3/tests/price_engine/test_bs.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.2.dev0/tests/price_engine/test_fft.py` & `jaxfin-0.3.3/tests/price_engine/test_fft.py`

 * *Files identical despite different names*

