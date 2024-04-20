# Comparing `tmp/devpi-common-4.0.3.tar.gz` & `tmp/devpi_common-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devpi-common-4.0.3.tar", last modified: Thu Nov 23 14:12:38 2023, max compression
+gzip compressed data, was "devpi_common-4.0.4.tar", last modified: Sat Apr 20 06:41:47 2024, max compression
```

## Comparing `devpi-common-4.0.3.tar` & `devpi_common-4.0.4.tar`

### file list

```diff
@@ -1,189 +1,203 @@
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-11-23 14:12:38.698721 devpi-common-4.0.3/
--rw-r--r--   0 fschulze   (501) staff       (20)       33 2023-11-20 15:47:49.000000 devpi-common-4.0.3/.flake8
--rw-r--r--   0 fschulze   (501) staff       (20)     6051 2023-11-23 14:09:28.000000 devpi-common-4.0.3/CHANGELOG
--rw-r--r--   0 fschulze   (501) staff       (20)     1368 2023-11-23 14:12:38.000000 devpi-common-4.0.3/CHANGELOG.short.rst
--rw-r--r--   0 fschulze   (501) staff       (20)     1061 2021-08-23 10:54:17.000000 devpi-common-4.0.3/LICENSE
--rw-r--r--   0 fschulze   (501) staff       (20)      130 2023-11-23 14:11:54.000000 devpi-common-4.0.3/MANIFEST.in
--rw-r--r--   0 fschulze   (501) staff       (20)     3746 2023-11-23 14:12:38.698166 devpi-common-4.0.3/PKG-INFO
--rw-r--r--   0 fschulze   (501) staff       (20)      128 2014-04-21 10:04:31.000000 devpi-common-4.0.3/README.rst
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-11-23 14:12:38.478654 devpi-common-4.0.3/devpi_common/
--rw-r--r--   0 fschulze   (501) staff       (20)       24 2023-11-23 14:08:43.000000 devpi-common-4.0.3/devpi_common/__init__.py
--rw-r--r--   0 fschulze   (501) staff       (20)     5367 2023-11-20 15:47:49.000000 devpi-common-4.0.3/devpi_common/archive.py
--rw-r--r--   0 fschulze   (501) staff       (20)      308 2023-11-20 15:47:49.000000 devpi-common-4.0.3/devpi_common/contextlib.py
--rw-r--r--   0 fschulze   (501) staff       (20)    10156 2023-11-23 14:07:15.000000 devpi-common-4.0.3/devpi_common/metadata.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1012 2023-11-20 15:47:49.000000 devpi-common-4.0.3/devpi_common/request.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1801 2023-11-20 15:47:49.000000 devpi-common-4.0.3/devpi_common/terminal.py
--rw-r--r--   0 fschulze   (501) staff       (20)     4638 2023-11-20 15:47:49.000000 devpi-common-4.0.3/devpi_common/types.py
--rw-r--r--   0 fschulze   (501) staff       (20)     7638 2023-11-20 15:47:49.000000 devpi-common-4.0.3/devpi_common/url.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3146 2023-11-20 15:47:49.000000 devpi-common-4.0.3/devpi_common/validation.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3193 2023-11-20 15:47:49.000000 devpi-common-4.0.3/devpi_common/viewhelp.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-11-23 14:12:38.695807 devpi-common-4.0.3/devpi_common.egg-info/
--rw-r--r--   0 fschulze   (501) staff       (20)     3746 2023-11-23 14:12:38.000000 devpi-common-4.0.3/devpi_common.egg-info/PKG-INFO
--rw-r--r--   0 fschulze   (501) staff       (20)     9679 2023-11-23 14:12:38.000000 devpi-common-4.0.3/devpi_common.egg-info/SOURCES.txt
--rw-r--r--   0 fschulze   (501) staff       (20)        1 2023-11-23 14:12:38.000000 devpi-common-4.0.3/devpi_common.egg-info/dependency_links.txt
--rw-r--r--   0 fschulze   (501) staff       (20)       35 2023-11-23 14:12:38.000000 devpi-common-4.0.3/devpi_common.egg-info/requires.txt
--rw-r--r--   0 fschulze   (501) staff       (20)       13 2023-11-23 14:12:38.000000 devpi-common-4.0.3/devpi_common.egg-info/top_level.txt
--rw-r--r--   0 fschulze   (501) staff       (20)     2021 2023-11-20 15:47:49.000000 devpi-common-4.0.3/pyproject.toml
--rw-r--r--   0 fschulze   (501) staff       (20)       38 2023-11-23 14:12:38.698827 devpi-common-4.0.3/setup.cfg
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-11-23 14:12:38.488362 devpi-common-4.0.3/testing/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-11-23 14:12:38.693066 devpi-common-4.0.3/testing/__pycache__/
--rw-------   0 fschulze   (501) staff       (20)    19975 2022-10-26 08:41:17.000000 devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-27-PYTEST.pyc
--rw-------   0 fschulze   (501) staff       (20)    17309 2019-12-05 11:15:23.000000 devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-34-PYTEST.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    17074 2019-12-05 11:15:38.000000 devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-35-pytest-5.3.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    13547 2022-07-22 09:29:47.000000 devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-35-pytest-6.1.2.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    11707 2020-10-05 15:59:53.000000 devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-36-pytest-6.0.0rc1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    11697 2020-12-13 08:42:10.000000 devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-36-pytest-6.2.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    11686 2023-01-24 12:40:09.000000 devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-36-pytest-7.0.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    11437 2022-12-12 19:22:52.000000 devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-37-pytest-7.2.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    11437 2023-01-24 12:44:20.000000 devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-37-pytest-7.2.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    11078 2022-02-08 17:21:35.000000 devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-38-pytest-7.0.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    11078 2022-03-05 07:22:58.000000 devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-38-pytest-7.0.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    11078 2022-06-23 09:34:12.000000 devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    11067 2023-01-24 11:34:57.000000 devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-38-pytest-7.2.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    11067 2023-05-13 13:23:37.000000 devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-38-pytest-7.3.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    11504 2023-08-30 15:52:29.000000 devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-38-pytest-7.4.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    11078 2023-11-20 15:47:32.000000 devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-38-pytest-7.4.2.pyc
--rw-------   0 fschulze   (501) staff       (20)    16879 2022-07-22 09:30:22.000000 devpi-common-4.0.3/testing/__pycache__/test_archive.pypy-27-PYTEST.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    14035 2022-03-05 07:23:45.000000 devpi-common-4.0.3/testing/__pycache__/test_archive.pypy37-pytest-7.0.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    14035 2022-07-22 09:30:48.000000 devpi-common-4.0.3/testing/__pycache__/test_archive.pypy37-pytest-7.1.2.pyc
--rw-------   0 fschulze   (501) staff       (20)    11712 2022-07-22 09:29:31.000000 devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-27-PYTEST.pyc
--rw-------   0 fschulze   (501) staff       (20)     9712 2019-12-05 11:15:23.000000 devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-34-PYTEST.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     9593 2019-12-05 11:15:38.000000 devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-35-pytest-5.3.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     7702 2022-07-22 09:29:47.000000 devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-35-pytest-6.1.2.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     6790 2020-10-05 15:59:05.000000 devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-36-pytest-6.0.0rc1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     6790 2020-12-13 08:42:10.000000 devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-36-pytest-6.2.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     6790 2023-01-24 12:40:09.000000 devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-36-pytest-7.0.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     6584 2022-12-12 19:22:52.000000 devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-37-pytest-7.2.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     6584 2023-01-24 12:44:20.000000 devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-37-pytest-7.2.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     6298 2022-02-08 17:21:35.000000 devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.0.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     6298 2022-03-05 07:22:58.000000 devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.0.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     6298 2022-06-23 09:34:12.000000 devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     6298 2022-10-26 08:40:19.000000 devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.2.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     6298 2023-05-13 13:23:38.000000 devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.3.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     6298 2023-08-30 11:44:06.000000 devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.4.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     6298 2023-10-11 14:36:50.000000 devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.4.2.pyc
--rw-------   0 fschulze   (501) staff       (20)     9130 2022-07-22 09:30:22.000000 devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.pypy-27-PYTEST.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     8683 2022-03-05 07:23:46.000000 devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.pypy37-pytest-7.0.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     8683 2022-07-22 09:30:48.000000 devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.pypy37-pytest-7.1.2.pyc
--rw-------   0 fschulze   (501) staff       (20)    26790 2022-10-26 08:41:17.000000 devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-27-PYTEST.pyc
--rw-------   0 fschulze   (501) staff       (20)    22898 2019-12-05 11:15:23.000000 devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-34-PYTEST.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    22599 2019-12-05 11:15:38.000000 devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-35-pytest-5.3.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    17280 2022-07-22 09:29:47.000000 devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-35-pytest-6.1.2.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    15035 2020-10-05 16:03:31.000000 devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-36-pytest-6.0.0rc1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    15035 2020-12-13 08:42:10.000000 devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-36-pytest-6.2.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    17370 2023-01-24 12:40:09.000000 devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-36-pytest-7.0.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    14020 2022-12-12 19:22:52.000000 devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-37-pytest-7.2.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    16195 2023-02-25 17:02:09.000000 devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-37-pytest-7.2.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    12956 2022-02-08 17:21:35.000000 devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-38-pytest-7.0.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    12956 2022-03-05 07:22:58.000000 devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-38-pytest-7.0.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    12966 2022-07-31 12:07:01.000000 devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    14917 2023-02-25 17:03:03.000000 devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-38-pytest-7.2.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    14375 2023-05-13 14:34:15.000000 devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-38-pytest-7.3.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    14375 2023-08-30 15:52:30.000000 devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-38-pytest-7.4.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    14433 2023-11-20 15:47:33.000000 devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-38-pytest-7.4.2.pyc
--rw-------   0 fschulze   (501) staff       (20)    22087 2022-07-22 09:30:22.000000 devpi-common-4.0.3/testing/__pycache__/test_metadata.pypy-27-PYTEST.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    16748 2022-03-05 07:23:46.000000 devpi-common-4.0.3/testing/__pycache__/test_metadata.pypy37-pytest-7.0.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    16756 2022-07-22 09:30:49.000000 devpi-common-4.0.3/testing/__pycache__/test_metadata.pypy37-pytest-7.1.2.pyc
--rw-------   0 fschulze   (501) staff       (20)     2038 2022-07-22 09:29:31.000000 devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-27-PYTEST.pyc
--rw-------   0 fschulze   (501) staff       (20)     1673 2019-12-05 11:15:23.000000 devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-34-PYTEST.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     1662 2019-12-05 11:15:38.000000 devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-35-pytest-5.3.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     1314 2022-07-22 09:29:48.000000 devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-35-pytest-6.1.2.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     1204 2020-10-05 16:03:09.000000 devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-36-pytest-6.0.0rc1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     1204 2020-12-13 08:42:10.000000 devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-36-pytest-6.2.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     1204 2023-01-24 12:40:09.000000 devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-36-pytest-7.0.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     1207 2022-12-12 19:22:52.000000 devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-37-pytest-7.2.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     1207 2023-01-24 12:44:20.000000 devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-37-pytest-7.2.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     1223 2022-02-08 17:21:35.000000 devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-38-pytest-7.0.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     1223 2022-03-05 07:22:58.000000 devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-38-pytest-7.0.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     1223 2022-06-23 09:34:12.000000 devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     1223 2022-10-26 08:40:19.000000 devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-38-pytest-7.2.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     1223 2023-11-20 15:47:33.000000 devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-38-pytest-7.4.2.pyc
--rw-------   0 fschulze   (501) staff       (20)     1761 2022-07-22 09:30:23.000000 devpi-common-4.0.3/testing/__pycache__/test_proc.pypy-27-PYTEST.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     1507 2022-03-05 07:23:46.000000 devpi-common-4.0.3/testing/__pycache__/test_proc.pypy37-pytest-7.0.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     1507 2022-07-22 09:30:49.000000 devpi-common-4.0.3/testing/__pycache__/test_proc.pypy37-pytest-7.1.2.pyc
--rw-------   0 fschulze   (501) staff       (20)     5468 2022-07-22 09:29:31.000000 devpi-common-4.0.3/testing/__pycache__/test_request.cpython-27-PYTEST.pyc
--rw-------   0 fschulze   (501) staff       (20)     4654 2019-12-05 11:15:23.000000 devpi-common-4.0.3/testing/__pycache__/test_request.cpython-34-PYTEST.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     4604 2019-12-05 11:15:38.000000 devpi-common-4.0.3/testing/__pycache__/test_request.cpython-35-pytest-5.3.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     3517 2022-07-22 09:29:48.000000 devpi-common-4.0.3/testing/__pycache__/test_request.cpython-35-pytest-6.1.2.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     3080 2020-10-05 16:03:09.000000 devpi-common-4.0.3/testing/__pycache__/test_request.cpython-36-pytest-6.0.0rc1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     3080 2020-12-13 08:42:10.000000 devpi-common-4.0.3/testing/__pycache__/test_request.cpython-36-pytest-6.2.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     3080 2023-01-24 12:40:09.000000 devpi-common-4.0.3/testing/__pycache__/test_request.cpython-36-pytest-7.0.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     2979 2022-12-12 19:22:52.000000 devpi-common-4.0.3/testing/__pycache__/test_request.cpython-37-pytest-7.2.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     2979 2023-01-24 12:44:20.000000 devpi-common-4.0.3/testing/__pycache__/test_request.cpython-37-pytest-7.2.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     2994 2022-02-08 17:21:35.000000 devpi-common-4.0.3/testing/__pycache__/test_request.cpython-38-pytest-7.0.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     2994 2022-03-05 07:22:58.000000 devpi-common-4.0.3/testing/__pycache__/test_request.cpython-38-pytest-7.0.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     2994 2022-06-23 09:34:12.000000 devpi-common-4.0.3/testing/__pycache__/test_request.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     2994 2022-10-26 08:40:19.000000 devpi-common-4.0.3/testing/__pycache__/test_request.cpython-38-pytest-7.2.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     2994 2023-05-13 13:23:38.000000 devpi-common-4.0.3/testing/__pycache__/test_request.cpython-38-pytest-7.3.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     2994 2023-08-30 11:44:06.000000 devpi-common-4.0.3/testing/__pycache__/test_request.cpython-38-pytest-7.4.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     2994 2023-10-11 14:36:50.000000 devpi-common-4.0.3/testing/__pycache__/test_request.cpython-38-pytest-7.4.2.pyc
--rw-------   0 fschulze   (501) staff       (20)     4677 2022-07-22 09:30:23.000000 devpi-common-4.0.3/testing/__pycache__/test_request.pypy-27-PYTEST.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     3582 2022-03-05 07:23:46.000000 devpi-common-4.0.3/testing/__pycache__/test_request.pypy37-pytest-7.0.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     3582 2022-07-22 09:30:49.000000 devpi-common-4.0.3/testing/__pycache__/test_request.pypy37-pytest-7.1.2.pyc
--rw-------   0 fschulze   (501) staff       (20)     6218 2022-02-08 17:21:15.000000 devpi-common-4.0.3/testing/__pycache__/test_types.cpython-27-PYTEST.pyc
--rw-------   0 fschulze   (501) staff       (20)     5297 2019-12-05 11:15:23.000000 devpi-common-4.0.3/testing/__pycache__/test_types.cpython-34-PYTEST.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     5219 2019-12-05 11:15:38.000000 devpi-common-4.0.3/testing/__pycache__/test_types.cpython-35-pytest-5.3.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     4322 2022-03-05 07:22:43.000000 devpi-common-4.0.3/testing/__pycache__/test_types.cpython-35-pytest-6.1.2.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     3689 2020-07-30 09:30:52.000000 devpi-common-4.0.3/testing/__pycache__/test_types.cpython-36-pytest-6.0.0rc1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     3689 2020-12-13 08:42:10.000000 devpi-common-4.0.3/testing/__pycache__/test_types.cpython-36-pytest-6.2.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     3689 2023-01-24 12:40:09.000000 devpi-common-4.0.3/testing/__pycache__/test_types.cpython-36-pytest-7.0.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     3581 2022-12-12 19:22:52.000000 devpi-common-4.0.3/testing/__pycache__/test_types.cpython-37-pytest-7.2.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     3672 2023-02-25 17:02:09.000000 devpi-common-4.0.3/testing/__pycache__/test_types.cpython-37-pytest-7.2.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     3599 2022-02-08 17:21:35.000000 devpi-common-4.0.3/testing/__pycache__/test_types.cpython-38-pytest-7.0.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     3599 2022-03-05 07:22:58.000000 devpi-common-4.0.3/testing/__pycache__/test_types.cpython-38-pytest-7.0.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     3599 2022-06-23 09:34:12.000000 devpi-common-4.0.3/testing/__pycache__/test_types.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     3599 2023-03-13 09:56:53.000000 devpi-common-4.0.3/testing/__pycache__/test_types.cpython-38-pytest-7.2.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     3599 2023-05-13 13:23:38.000000 devpi-common-4.0.3/testing/__pycache__/test_types.cpython-38-pytest-7.3.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     3599 2023-08-30 11:44:06.000000 devpi-common-4.0.3/testing/__pycache__/test_types.cpython-38-pytest-7.4.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     3599 2023-10-11 14:36:50.000000 devpi-common-4.0.3/testing/__pycache__/test_types.cpython-38-pytest-7.4.2.pyc
--rw-------   0 fschulze   (501) staff       (20)     5330 2022-03-05 07:23:18.000000 devpi-common-4.0.3/testing/__pycache__/test_types.pypy-27-PYTEST.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     4232 2022-03-05 07:23:46.000000 devpi-common-4.0.3/testing/__pycache__/test_types.pypy37-pytest-7.0.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     4232 2022-07-22 09:30:49.000000 devpi-common-4.0.3/testing/__pycache__/test_types.pypy37-pytest-7.1.2.pyc
--rw-------   0 fschulze   (501) staff       (20)   123091 2022-10-26 08:41:17.000000 devpi-common-4.0.3/testing/__pycache__/test_url.cpython-27-PYTEST.pyc
--rw-------   0 fschulze   (501) staff       (20)    86955 2019-12-05 11:15:23.000000 devpi-common-4.0.3/testing/__pycache__/test_url.cpython-34-PYTEST.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    85266 2019-12-05 11:15:38.000000 devpi-common-4.0.3/testing/__pycache__/test_url.cpython-35-pytest-5.3.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    77552 2022-07-22 09:29:48.000000 devpi-common-4.0.3/testing/__pycache__/test_url.cpython-35-pytest-6.1.2.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    62539 2020-09-29 17:58:02.000000 devpi-common-4.0.3/testing/__pycache__/test_url.cpython-36-pytest-6.0.0rc1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    62539 2020-12-13 08:42:10.000000 devpi-common-4.0.3/testing/__pycache__/test_url.cpython-36-pytest-6.2.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    63100 2023-01-24 12:40:09.000000 devpi-common-4.0.3/testing/__pycache__/test_url.cpython-36-pytest-7.0.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    60230 2022-12-12 19:22:52.000000 devpi-common-4.0.3/testing/__pycache__/test_url.cpython-37-pytest-7.2.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    60619 2023-02-25 17:02:10.000000 devpi-common-4.0.3/testing/__pycache__/test_url.cpython-37-pytest-7.2.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    56431 2022-02-08 17:21:35.000000 devpi-common-4.0.3/testing/__pycache__/test_url.cpython-38-pytest-7.0.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    56431 2022-03-05 07:22:59.000000 devpi-common-4.0.3/testing/__pycache__/test_url.cpython-38-pytest-7.0.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    56922 2022-07-31 12:07:01.000000 devpi-common-4.0.3/testing/__pycache__/test_url.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    57311 2023-02-25 17:03:03.000000 devpi-common-4.0.3/testing/__pycache__/test_url.cpython-38-pytest-7.2.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    57311 2023-05-13 13:23:38.000000 devpi-common-4.0.3/testing/__pycache__/test_url.cpython-38-pytest-7.3.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    56491 2023-08-30 15:52:30.000000 devpi-common-4.0.3/testing/__pycache__/test_url.cpython-38-pytest-7.4.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    56431 2023-11-20 15:47:33.000000 devpi-common-4.0.3/testing/__pycache__/test_url.cpython-38-pytest-7.4.2.pyc
--rw-------   0 fschulze   (501) staff       (20)    99908 2022-07-22 09:30:23.000000 devpi-common-4.0.3/testing/__pycache__/test_url.pypy-27-PYTEST.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    67392 2022-03-05 07:23:47.000000 devpi-common-4.0.3/testing/__pycache__/test_url.pypy37-pytest-7.0.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)    67698 2022-07-22 09:30:50.000000 devpi-common-4.0.3/testing/__pycache__/test_url.pypy37-pytest-7.1.2.pyc
--rw-------   0 fschulze   (501) staff       (20)     3219 2022-02-08 17:21:15.000000 devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-27-PYTEST.pyc
--rw-------   0 fschulze   (501) staff       (20)     2599 2019-12-05 11:15:23.000000 devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-34-PYTEST.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     2588 2019-12-05 11:15:38.000000 devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-35-pytest-5.3.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     2234 2022-03-05 07:22:43.000000 devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-35-pytest-6.1.2.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     2053 2020-07-30 09:30:53.000000 devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-36-pytest-6.0.0rc1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     2053 2020-12-13 08:42:10.000000 devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-36-pytest-6.2.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     2053 2023-01-24 12:40:09.000000 devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-36-pytest-7.0.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     2046 2022-12-12 19:22:52.000000 devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-37-pytest-7.2.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     2046 2023-01-24 12:44:21.000000 devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-37-pytest-7.2.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     2034 2022-02-08 17:21:35.000000 devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-38-pytest-7.0.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     2034 2022-03-05 07:22:59.000000 devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-38-pytest-7.0.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     2034 2022-06-23 09:34:12.000000 devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-38-pytest-7.1.2.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     2034 2022-10-26 08:40:20.000000 devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-38-pytest-7.2.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     1914 2023-05-13 14:28:34.000000 devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-38-pytest-7.3.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     1908 2023-08-30 15:52:30.000000 devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-38-pytest-7.4.0.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     2034 2023-11-20 15:47:33.000000 devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-38-pytest-7.4.2.pyc
--rw-------   0 fschulze   (501) staff       (20)     2610 2022-03-05 07:23:19.000000 devpi-common-4.0.3/testing/__pycache__/test_validation.pypy-27-PYTEST.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     2672 2022-03-05 07:23:47.000000 devpi-common-4.0.3/testing/__pycache__/test_validation.pypy37-pytest-7.0.1.pyc
--rw-r--r--   0 fschulze   (501) staff       (20)     2672 2022-07-22 09:30:50.000000 devpi-common-4.0.3/testing/__pycache__/test_validation.pypy37-pytest-7.1.2.pyc
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-11-23 14:12:38.693923 devpi-common-4.0.3/testing/data/
--rw-r--r--   0 fschulze   (501) staff       (20)      111 2014-04-21 10:04:31.000000 devpi-common-4.0.3/testing/data/slash.tar.gz
--rw-r--r--   0 fschulze   (501) staff       (20)     4355 2023-11-20 15:47:49.000000 devpi-common-4.0.3/testing/test_archive.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1915 2023-09-10 07:34:39.000000 devpi-common-4.0.3/testing/test_lazydecorator.py
--rw-r--r--   0 fschulze   (501) staff       (20)     8332 2023-11-23 14:07:15.000000 devpi-common-4.0.3/testing/test_metadata.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1176 2022-03-05 07:26:44.000000 devpi-common-4.0.3/testing/test_request.py
--rw-r--r--   0 fschulze   (501) staff       (20)      868 2023-02-25 17:16:05.000000 devpi-common-4.0.3/testing/test_types.py
--rw-r--r--   0 fschulze   (501) staff       (20)    19072 2023-11-20 15:47:49.000000 devpi-common-4.0.3/testing/test_url.py
--rw-r--r--   0 fschulze   (501) staff       (20)      717 2023-11-20 15:47:49.000000 devpi-common-4.0.3/testing/test_validation.py
--rw-r--r--   0 fschulze   (501) staff       (20)      432 2023-11-20 15:47:49.000000 devpi-common-4.0.3/tox.ini
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2024-04-20 06:41:47.433163 devpi_common-4.0.4/
+-rw-r--r--   0 fschulze   (501) staff       (20)       33 2024-03-04 07:22:59.000000 devpi_common-4.0.4/.flake8
+-rw-r--r--   0 fschulze   (501) staff       (20)     6380 2024-04-20 06:35:31.000000 devpi_common-4.0.4/CHANGELOG
+-rw-r--r--   0 fschulze   (501) staff       (20)     1451 2024-04-20 06:41:47.000000 devpi_common-4.0.4/CHANGELOG.short.rst
+-rw-r--r--   0 fschulze   (501) staff       (20)     1061 2021-08-23 10:54:17.000000 devpi_common-4.0.4/LICENSE
+-rw-r--r--   0 fschulze   (501) staff       (20)      130 2024-04-11 06:42:42.000000 devpi_common-4.0.4/MANIFEST.in
+-rw-r--r--   0 fschulze   (501) staff       (20)     3832 2024-04-20 06:41:47.432757 devpi_common-4.0.4/PKG-INFO
+-rw-r--r--   0 fschulze   (501) staff       (20)      128 2014-04-21 10:04:31.000000 devpi_common-4.0.4/README.rst
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2024-04-20 06:41:47.258819 devpi_common-4.0.4/devpi_common/
+-rw-r--r--   0 fschulze   (501) staff       (20)       24 2024-04-20 06:34:08.000000 devpi_common-4.0.4/devpi_common/__init__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     5543 2024-04-14 15:50:25.000000 devpi_common-4.0.4/devpi_common/archive.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      308 2024-03-04 07:22:59.000000 devpi_common-4.0.4/devpi_common/contextlib.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     7230 2024-04-16 11:43:32.000000 devpi_common-4.0.4/devpi_common/metadata.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1012 2023-11-26 07:11:17.000000 devpi_common-4.0.4/devpi_common/request.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1801 2024-03-04 07:22:59.000000 devpi_common-4.0.4/devpi_common/terminal.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     4638 2024-03-04 07:22:59.000000 devpi_common-4.0.4/devpi_common/types.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     7638 2024-03-04 07:22:59.000000 devpi_common-4.0.4/devpi_common/url.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3146 2024-03-04 07:22:59.000000 devpi_common-4.0.4/devpi_common/validation.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3193 2024-03-04 07:22:59.000000 devpi_common-4.0.4/devpi_common/viewhelp.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2024-04-20 06:41:47.432280 devpi_common-4.0.4/devpi_common.egg-info/
+-rw-r--r--   0 fschulze   (501) staff       (20)     3832 2024-04-20 06:41:47.000000 devpi_common-4.0.4/devpi_common.egg-info/PKG-INFO
+-rw-r--r--   0 fschulze   (501) staff       (20)    10541 2024-04-20 06:41:47.000000 devpi_common-4.0.4/devpi_common.egg-info/SOURCES.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)        1 2024-04-20 06:41:47.000000 devpi_common-4.0.4/devpi_common.egg-info/dependency_links.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)       38 2024-04-20 06:41:47.000000 devpi_common-4.0.4/devpi_common.egg-info/requires.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)       13 2024-04-20 06:41:47.000000 devpi_common-4.0.4/devpi_common.egg-info/top_level.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)     2024 2024-04-11 06:42:42.000000 devpi_common-4.0.4/pyproject.toml
+-rw-r--r--   0 fschulze   (501) staff       (20)       38 2024-04-20 06:41:47.433256 devpi_common-4.0.4/setup.cfg
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2024-04-20 06:41:47.265253 devpi_common-4.0.4/testing/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2024-04-20 06:41:47.431351 devpi_common-4.0.4/testing/__pycache__/
+-rw-------   0 fschulze   (501) staff       (20)    19975 2022-10-26 08:41:17.000000 devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-27-PYTEST.pyc
+-rw-------   0 fschulze   (501) staff       (20)    17309 2019-12-05 11:15:23.000000 devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-34-PYTEST.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    17074 2019-12-05 11:15:38.000000 devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-35-pytest-5.3.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    13547 2022-07-22 09:29:47.000000 devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-35-pytest-6.1.2.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    11707 2020-10-05 15:59:53.000000 devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-36-pytest-6.0.0rc1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    11697 2020-12-13 08:42:10.000000 devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-36-pytest-6.2.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    11686 2023-01-24 12:40:09.000000 devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-36-pytest-7.0.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    11437 2022-12-12 19:22:52.000000 devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-37-pytest-7.2.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    11437 2023-01-24 12:44:20.000000 devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-37-pytest-7.2.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    11078 2022-02-08 17:21:35.000000 devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-38-pytest-7.0.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    11078 2022-03-05 07:22:58.000000 devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-38-pytest-7.0.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    11078 2022-06-23 09:34:12.000000 devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-38-pytest-7.1.2.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    11067 2023-01-24 11:34:57.000000 devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-38-pytest-7.2.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    11067 2023-05-13 13:23:37.000000 devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-38-pytest-7.3.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    11504 2023-08-30 15:52:29.000000 devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-38-pytest-7.4.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    11078 2023-11-20 15:47:32.000000 devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-38-pytest-7.4.2.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    11504 2023-11-24 05:29:26.000000 devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-38-pytest-7.4.3.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    11304 2024-04-17 14:13:18.000000 devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-39-pytest-8.1.1.pyc
+-rw-------   0 fschulze   (501) staff       (20)    16879 2022-07-22 09:30:22.000000 devpi_common-4.0.4/testing/__pycache__/test_archive.pypy-27-PYTEST.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    14035 2022-03-05 07:23:45.000000 devpi_common-4.0.4/testing/__pycache__/test_archive.pypy37-pytest-7.0.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    14035 2022-07-22 09:30:48.000000 devpi_common-4.0.4/testing/__pycache__/test_archive.pypy37-pytest-7.1.2.pyc
+-rw-------   0 fschulze   (501) staff       (20)    11712 2022-07-22 09:29:31.000000 devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-27-PYTEST.pyc
+-rw-------   0 fschulze   (501) staff       (20)     9712 2019-12-05 11:15:23.000000 devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-34-PYTEST.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     9593 2019-12-05 11:15:38.000000 devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-35-pytest-5.3.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     7702 2022-07-22 09:29:47.000000 devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-35-pytest-6.1.2.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     6790 2020-10-05 15:59:05.000000 devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-36-pytest-6.0.0rc1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     6790 2020-12-13 08:42:10.000000 devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-36-pytest-6.2.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     6790 2023-01-24 12:40:09.000000 devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-36-pytest-7.0.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     6584 2022-12-12 19:22:52.000000 devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-37-pytest-7.2.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     6584 2023-01-24 12:44:20.000000 devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-37-pytest-7.2.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     6298 2022-02-08 17:21:35.000000 devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.0.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     6298 2022-03-05 07:22:58.000000 devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.0.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     6298 2022-06-23 09:34:12.000000 devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.1.2.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     6298 2022-10-26 08:40:19.000000 devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.2.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     6298 2023-05-13 13:23:38.000000 devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.3.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     6298 2023-08-30 11:44:06.000000 devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.4.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     6298 2023-10-11 14:36:50.000000 devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.4.2.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     6298 2023-11-24 05:29:26.000000 devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.4.3.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     6128 2024-04-17 14:13:18.000000 devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-39-pytest-8.1.1.pyc
+-rw-------   0 fschulze   (501) staff       (20)     9130 2022-07-22 09:30:22.000000 devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.pypy-27-PYTEST.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     8683 2022-03-05 07:23:46.000000 devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.pypy37-pytest-7.0.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     8683 2022-07-22 09:30:48.000000 devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.pypy37-pytest-7.1.2.pyc
+-rw-------   0 fschulze   (501) staff       (20)    26790 2022-10-26 08:41:17.000000 devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-27-PYTEST.pyc
+-rw-------   0 fschulze   (501) staff       (20)    22898 2019-12-05 11:15:23.000000 devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-34-PYTEST.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    22599 2019-12-05 11:15:38.000000 devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-35-pytest-5.3.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    17280 2022-07-22 09:29:47.000000 devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-35-pytest-6.1.2.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    15035 2020-10-05 16:03:31.000000 devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-36-pytest-6.0.0rc1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    15035 2020-12-13 08:42:10.000000 devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-36-pytest-6.2.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    17370 2023-01-24 12:40:09.000000 devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-36-pytest-7.0.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    14020 2022-12-12 19:22:52.000000 devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-37-pytest-7.2.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    16195 2023-02-25 17:02:09.000000 devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-37-pytest-7.2.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    12956 2022-02-08 17:21:35.000000 devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-38-pytest-7.0.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    12956 2022-03-05 07:22:58.000000 devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-38-pytest-7.0.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    12966 2022-07-31 12:07:01.000000 devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-38-pytest-7.1.2.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    14917 2023-02-25 17:03:03.000000 devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-38-pytest-7.2.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    14375 2023-05-13 14:34:15.000000 devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-38-pytest-7.3.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    14375 2023-08-30 15:52:30.000000 devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-38-pytest-7.4.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    14433 2023-11-20 15:47:33.000000 devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-38-pytest-7.4.2.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    16079 2023-11-25 08:45:54.000000 devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-38-pytest-7.4.3.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    14589 2024-04-17 14:13:18.000000 devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-39-pytest-8.1.1.pyc
+-rw-------   0 fschulze   (501) staff       (20)    22087 2022-07-22 09:30:22.000000 devpi_common-4.0.4/testing/__pycache__/test_metadata.pypy-27-PYTEST.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    16748 2022-03-05 07:23:46.000000 devpi_common-4.0.4/testing/__pycache__/test_metadata.pypy37-pytest-7.0.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    16756 2022-07-22 09:30:49.000000 devpi_common-4.0.4/testing/__pycache__/test_metadata.pypy37-pytest-7.1.2.pyc
+-rw-------   0 fschulze   (501) staff       (20)     2038 2022-07-22 09:29:31.000000 devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-27-PYTEST.pyc
+-rw-------   0 fschulze   (501) staff       (20)     1673 2019-12-05 11:15:23.000000 devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-34-PYTEST.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     1662 2019-12-05 11:15:38.000000 devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-35-pytest-5.3.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     1314 2022-07-22 09:29:48.000000 devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-35-pytest-6.1.2.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     1204 2020-10-05 16:03:09.000000 devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-36-pytest-6.0.0rc1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     1204 2020-12-13 08:42:10.000000 devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-36-pytest-6.2.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     1204 2023-01-24 12:40:09.000000 devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-36-pytest-7.0.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     1207 2022-12-12 19:22:52.000000 devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-37-pytest-7.2.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     1207 2023-01-24 12:44:20.000000 devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-37-pytest-7.2.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     1223 2022-02-08 17:21:35.000000 devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-38-pytest-7.0.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     1223 2022-03-05 07:22:58.000000 devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-38-pytest-7.0.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     1223 2022-06-23 09:34:12.000000 devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-38-pytest-7.1.2.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     1223 2022-10-26 08:40:19.000000 devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-38-pytest-7.2.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     1223 2023-11-20 15:47:33.000000 devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-38-pytest-7.4.2.pyc
+-rw-------   0 fschulze   (501) staff       (20)     1761 2022-07-22 09:30:23.000000 devpi_common-4.0.4/testing/__pycache__/test_proc.pypy-27-PYTEST.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     1507 2022-03-05 07:23:46.000000 devpi_common-4.0.4/testing/__pycache__/test_proc.pypy37-pytest-7.0.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     1507 2022-07-22 09:30:49.000000 devpi_common-4.0.4/testing/__pycache__/test_proc.pypy37-pytest-7.1.2.pyc
+-rw-------   0 fschulze   (501) staff       (20)     5468 2022-07-22 09:29:31.000000 devpi_common-4.0.4/testing/__pycache__/test_request.cpython-27-PYTEST.pyc
+-rw-------   0 fschulze   (501) staff       (20)     4654 2019-12-05 11:15:23.000000 devpi_common-4.0.4/testing/__pycache__/test_request.cpython-34-PYTEST.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     4604 2019-12-05 11:15:38.000000 devpi_common-4.0.4/testing/__pycache__/test_request.cpython-35-pytest-5.3.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     3517 2022-07-22 09:29:48.000000 devpi_common-4.0.4/testing/__pycache__/test_request.cpython-35-pytest-6.1.2.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     3080 2020-10-05 16:03:09.000000 devpi_common-4.0.4/testing/__pycache__/test_request.cpython-36-pytest-6.0.0rc1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     3080 2020-12-13 08:42:10.000000 devpi_common-4.0.4/testing/__pycache__/test_request.cpython-36-pytest-6.2.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     3080 2023-01-24 12:40:09.000000 devpi_common-4.0.4/testing/__pycache__/test_request.cpython-36-pytest-7.0.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     2979 2022-12-12 19:22:52.000000 devpi_common-4.0.4/testing/__pycache__/test_request.cpython-37-pytest-7.2.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     2979 2023-01-24 12:44:20.000000 devpi_common-4.0.4/testing/__pycache__/test_request.cpython-37-pytest-7.2.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     2994 2022-02-08 17:21:35.000000 devpi_common-4.0.4/testing/__pycache__/test_request.cpython-38-pytest-7.0.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     2994 2022-03-05 07:22:58.000000 devpi_common-4.0.4/testing/__pycache__/test_request.cpython-38-pytest-7.0.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     2994 2022-06-23 09:34:12.000000 devpi_common-4.0.4/testing/__pycache__/test_request.cpython-38-pytest-7.1.2.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     2994 2022-10-26 08:40:19.000000 devpi_common-4.0.4/testing/__pycache__/test_request.cpython-38-pytest-7.2.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     2994 2023-05-13 13:23:38.000000 devpi_common-4.0.4/testing/__pycache__/test_request.cpython-38-pytest-7.3.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     2994 2023-08-30 11:44:06.000000 devpi_common-4.0.4/testing/__pycache__/test_request.cpython-38-pytest-7.4.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     2994 2023-10-11 14:36:50.000000 devpi_common-4.0.4/testing/__pycache__/test_request.cpython-38-pytest-7.4.2.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     2994 2023-11-24 05:29:27.000000 devpi_common-4.0.4/testing/__pycache__/test_request.cpython-38-pytest-7.4.3.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     2954 2024-04-17 14:13:18.000000 devpi_common-4.0.4/testing/__pycache__/test_request.cpython-39-pytest-8.1.1.pyc
+-rw-------   0 fschulze   (501) staff       (20)     4677 2022-07-22 09:30:23.000000 devpi_common-4.0.4/testing/__pycache__/test_request.pypy-27-PYTEST.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     3582 2022-03-05 07:23:46.000000 devpi_common-4.0.4/testing/__pycache__/test_request.pypy37-pytest-7.0.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     3582 2022-07-22 09:30:49.000000 devpi_common-4.0.4/testing/__pycache__/test_request.pypy37-pytest-7.1.2.pyc
+-rw-------   0 fschulze   (501) staff       (20)     6218 2022-02-08 17:21:15.000000 devpi_common-4.0.4/testing/__pycache__/test_types.cpython-27-PYTEST.pyc
+-rw-------   0 fschulze   (501) staff       (20)     5297 2019-12-05 11:15:23.000000 devpi_common-4.0.4/testing/__pycache__/test_types.cpython-34-PYTEST.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     5219 2019-12-05 11:15:38.000000 devpi_common-4.0.4/testing/__pycache__/test_types.cpython-35-pytest-5.3.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     4322 2022-03-05 07:22:43.000000 devpi_common-4.0.4/testing/__pycache__/test_types.cpython-35-pytest-6.1.2.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     3689 2020-07-30 09:30:52.000000 devpi_common-4.0.4/testing/__pycache__/test_types.cpython-36-pytest-6.0.0rc1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     3689 2020-12-13 08:42:10.000000 devpi_common-4.0.4/testing/__pycache__/test_types.cpython-36-pytest-6.2.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     3689 2023-01-24 12:40:09.000000 devpi_common-4.0.4/testing/__pycache__/test_types.cpython-36-pytest-7.0.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     3581 2022-12-12 19:22:52.000000 devpi_common-4.0.4/testing/__pycache__/test_types.cpython-37-pytest-7.2.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     3672 2023-02-25 17:02:09.000000 devpi_common-4.0.4/testing/__pycache__/test_types.cpython-37-pytest-7.2.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     3599 2022-02-08 17:21:35.000000 devpi_common-4.0.4/testing/__pycache__/test_types.cpython-38-pytest-7.0.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     3599 2022-03-05 07:22:58.000000 devpi_common-4.0.4/testing/__pycache__/test_types.cpython-38-pytest-7.0.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     3599 2022-06-23 09:34:12.000000 devpi_common-4.0.4/testing/__pycache__/test_types.cpython-38-pytest-7.1.2.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     3599 2023-03-13 09:56:53.000000 devpi_common-4.0.4/testing/__pycache__/test_types.cpython-38-pytest-7.2.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     3599 2023-05-13 13:23:38.000000 devpi_common-4.0.4/testing/__pycache__/test_types.cpython-38-pytest-7.3.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     3599 2023-08-30 11:44:06.000000 devpi_common-4.0.4/testing/__pycache__/test_types.cpython-38-pytest-7.4.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     3599 2023-10-11 14:36:50.000000 devpi_common-4.0.4/testing/__pycache__/test_types.cpython-38-pytest-7.4.2.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     3599 2023-11-24 05:29:27.000000 devpi_common-4.0.4/testing/__pycache__/test_types.cpython-38-pytest-7.4.3.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     3469 2024-04-17 14:13:19.000000 devpi_common-4.0.4/testing/__pycache__/test_types.cpython-39-pytest-8.1.1.pyc
+-rw-------   0 fschulze   (501) staff       (20)     5330 2022-03-05 07:23:18.000000 devpi_common-4.0.4/testing/__pycache__/test_types.pypy-27-PYTEST.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     4232 2022-03-05 07:23:46.000000 devpi_common-4.0.4/testing/__pycache__/test_types.pypy37-pytest-7.0.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     4232 2022-07-22 09:30:49.000000 devpi_common-4.0.4/testing/__pycache__/test_types.pypy37-pytest-7.1.2.pyc
+-rw-------   0 fschulze   (501) staff       (20)   123091 2022-10-26 08:41:17.000000 devpi_common-4.0.4/testing/__pycache__/test_url.cpython-27-PYTEST.pyc
+-rw-------   0 fschulze   (501) staff       (20)    86955 2019-12-05 11:15:23.000000 devpi_common-4.0.4/testing/__pycache__/test_url.cpython-34-PYTEST.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    85266 2019-12-05 11:15:38.000000 devpi_common-4.0.4/testing/__pycache__/test_url.cpython-35-pytest-5.3.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    77552 2022-07-22 09:29:48.000000 devpi_common-4.0.4/testing/__pycache__/test_url.cpython-35-pytest-6.1.2.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    62539 2020-09-29 17:58:02.000000 devpi_common-4.0.4/testing/__pycache__/test_url.cpython-36-pytest-6.0.0rc1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    62539 2020-12-13 08:42:10.000000 devpi_common-4.0.4/testing/__pycache__/test_url.cpython-36-pytest-6.2.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    63100 2023-01-24 12:40:09.000000 devpi_common-4.0.4/testing/__pycache__/test_url.cpython-36-pytest-7.0.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    60230 2022-12-12 19:22:52.000000 devpi_common-4.0.4/testing/__pycache__/test_url.cpython-37-pytest-7.2.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    60619 2023-02-25 17:02:10.000000 devpi_common-4.0.4/testing/__pycache__/test_url.cpython-37-pytest-7.2.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    56431 2022-02-08 17:21:35.000000 devpi_common-4.0.4/testing/__pycache__/test_url.cpython-38-pytest-7.0.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    56431 2022-03-05 07:22:59.000000 devpi_common-4.0.4/testing/__pycache__/test_url.cpython-38-pytest-7.0.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    56922 2022-07-31 12:07:01.000000 devpi_common-4.0.4/testing/__pycache__/test_url.cpython-38-pytest-7.1.2.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    57311 2023-02-25 17:03:03.000000 devpi_common-4.0.4/testing/__pycache__/test_url.cpython-38-pytest-7.2.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    57311 2023-05-13 13:23:38.000000 devpi_common-4.0.4/testing/__pycache__/test_url.cpython-38-pytest-7.3.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    56491 2023-08-30 15:52:30.000000 devpi_common-4.0.4/testing/__pycache__/test_url.cpython-38-pytest-7.4.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    56431 2023-11-20 15:47:33.000000 devpi_common-4.0.4/testing/__pycache__/test_url.cpython-38-pytest-7.4.2.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    56979 2023-11-24 05:29:27.000000 devpi_common-4.0.4/testing/__pycache__/test_url.cpython-38-pytest-7.4.3.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    53995 2024-04-17 14:13:19.000000 devpi_common-4.0.4/testing/__pycache__/test_url.cpython-39-pytest-8.1.1.pyc
+-rw-------   0 fschulze   (501) staff       (20)    99908 2022-07-22 09:30:23.000000 devpi_common-4.0.4/testing/__pycache__/test_url.pypy-27-PYTEST.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    67392 2022-03-05 07:23:47.000000 devpi_common-4.0.4/testing/__pycache__/test_url.pypy37-pytest-7.0.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)    67698 2022-07-22 09:30:50.000000 devpi_common-4.0.4/testing/__pycache__/test_url.pypy37-pytest-7.1.2.pyc
+-rw-------   0 fschulze   (501) staff       (20)     3219 2022-02-08 17:21:15.000000 devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-27-PYTEST.pyc
+-rw-------   0 fschulze   (501) staff       (20)     2599 2019-12-05 11:15:23.000000 devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-34-PYTEST.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     2588 2019-12-05 11:15:38.000000 devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-35-pytest-5.3.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     2234 2022-03-05 07:22:43.000000 devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-35-pytest-6.1.2.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     2053 2020-07-30 09:30:53.000000 devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-36-pytest-6.0.0rc1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     2053 2020-12-13 08:42:10.000000 devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-36-pytest-6.2.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     2053 2023-01-24 12:40:09.000000 devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-36-pytest-7.0.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     2046 2022-12-12 19:22:52.000000 devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-37-pytest-7.2.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     2046 2023-01-24 12:44:21.000000 devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-37-pytest-7.2.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     2034 2022-02-08 17:21:35.000000 devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-38-pytest-7.0.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     2034 2022-03-05 07:22:59.000000 devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-38-pytest-7.0.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     2034 2022-06-23 09:34:12.000000 devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-38-pytest-7.1.2.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     2034 2022-10-26 08:40:20.000000 devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-38-pytest-7.2.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     1914 2023-05-13 14:28:34.000000 devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-38-pytest-7.3.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     1908 2023-08-30 15:52:30.000000 devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-38-pytest-7.4.0.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     2034 2023-11-20 15:47:33.000000 devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-38-pytest-7.4.2.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     1908 2023-11-24 05:29:27.000000 devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-38-pytest-7.4.3.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     1929 2024-04-17 14:13:19.000000 devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-39-pytest-8.1.1.pyc
+-rw-------   0 fschulze   (501) staff       (20)     2610 2022-03-05 07:23:19.000000 devpi_common-4.0.4/testing/__pycache__/test_validation.pypy-27-PYTEST.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     2672 2022-03-05 07:23:47.000000 devpi_common-4.0.4/testing/__pycache__/test_validation.pypy37-pytest-7.0.1.pyc
+-rw-r--r--   0 fschulze   (501) staff       (20)     2672 2022-07-22 09:30:50.000000 devpi_common-4.0.4/testing/__pycache__/test_validation.pypy37-pytest-7.1.2.pyc
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2024-04-20 06:41:47.431739 devpi_common-4.0.4/testing/data/
+-rw-r--r--   0 fschulze   (501) staff       (20)      111 2014-04-21 10:04:31.000000 devpi_common-4.0.4/testing/data/slash.tar.gz
+-rw-r--r--   0 fschulze   (501) staff       (20)     4355 2024-03-04 07:22:59.000000 devpi_common-4.0.4/testing/test_archive.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1915 2023-11-26 07:11:17.000000 devpi_common-4.0.4/testing/test_lazydecorator.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     8332 2024-04-16 11:43:32.000000 devpi_common-4.0.4/testing/test_metadata.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1176 2023-11-26 07:11:17.000000 devpi_common-4.0.4/testing/test_request.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      868 2023-11-26 07:11:17.000000 devpi_common-4.0.4/testing/test_types.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    19072 2024-03-04 07:22:59.000000 devpi_common-4.0.4/testing/test_url.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      717 2024-04-17 14:13:36.000000 devpi_common-4.0.4/testing/test_validation.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      432 2024-04-11 06:42:42.000000 devpi_common-4.0.4/tox.ini
```

### Comparing `devpi-common-4.0.3/CHANGELOG` & `devpi_common-4.0.4/CHANGELOG`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 
 
 .. towncrier release notes start
 
+4.0.4 (2024-04-20)
+==================
+
+Bug Fixes
+---------
+
+- Use ``filter='data'`` for ``extractall`` call on supported Python versions as additional guard to the existing out of path checks against malicious tar files.
+
+- Remove custom ``LegacyVersion`` and use ``packaging-legacy`` instead, which is also used by pypi.org.
+
+
+
 4.0.3 (2023-11-23)
 ==================
 
 Bug Fixes
 ---------
 
 - Add ``is_prerelease`` and other methods to ``LegacyVersion`` to fix ``get_sorted_versions`` with ``stable=True`` and some other cases.
```

### Comparing `devpi-common-4.0.3/CHANGELOG.short.rst` & `devpi_common-4.0.4/CHANGELOG.short.rst`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,26 @@
 =========
 
 
 
 
 .. towncrier release notes start
 
+4.0.4 (2024-04-20)
+==================
+
+Bug Fixes
+---------
+
+- Use ``filter='data'`` for ``extractall`` call on supported Python versions as additional guard to the existing out of path checks against malicious tar files.
+
+- Remove custom ``LegacyVersion`` and use ``packaging-legacy`` instead, which is also used by pypi.org.
+
+
+
 4.0.3 (2023-11-23)
 ==================
 
 Bug Fixes
 ---------
 
 - Add ``is_prerelease`` and other methods to ``LegacyVersion`` to fix ``get_sorted_versions`` with ``stable=True`` and some other cases.
@@ -60,22 +72,7 @@
 
 
 Bug Fixes
 ---------
 
 - Fix #939: custom legacy version parsing (non PEP 440) after packaging >= 22.0 removed support.
 
-
-3.7.2 (2023-01-24)
-==================
-
-
-
-
-
-Bug Fixes
----------
-
-- Fix #928: correct default for pre-release matching after switching from ``pkg_resources`` to ``packaging``.
-
-- Fix #949: correct parsing of wheel tags for Python 3.10 and above.
-
```

### Comparing `devpi-common-4.0.3/LICENSE` & `devpi_common-4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/PKG-INFO` & `devpi_common-4.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devpi-common
-Version: 4.0.3
+Version: 4.0.4
 Summary: Utilities jointly used by devpi-server, devpi-client and others.
 Maintainer-email: Florian Schulze <mail@pyfidelity.com>
 License: 
           Permission is hereby granted, free of charge, to any person obtaining a copy
           of this software and associated documentation files (the "Software"), to deal
           in the Software without restriction, including without limitation the rights
           to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -36,15 +36,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: lazy
-Requires-Dist: packaging>=22
+Requires-Dist: packaging-legacy
 Requires-Dist: requests>=2.3.0
 
 
 This package contains utility functions used by devpi-server and devpi-client.
 
 See http://doc.devpi.net for more information.
 
@@ -55,14 +55,26 @@
 =========
 
 
 
 
 .. towncrier release notes start
 
+4.0.4 (2024-04-20)
+==================
+
+Bug Fixes
+---------
+
+- Use ``filter='data'`` for ``extractall`` call on supported Python versions as additional guard to the existing out of path checks against malicious tar files.
+
+- Remove custom ``LegacyVersion`` and use ``packaging-legacy`` instead, which is also used by pypi.org.
+
+
+
 4.0.3 (2023-11-23)
 ==================
 
 Bug Fixes
 ---------
 
 - Add ``is_prerelease`` and other methods to ``LegacyVersion`` to fix ``get_sorted_versions`` with ``stable=True`` and some other cases.
@@ -110,22 +122,7 @@
 
 
 Bug Fixes
 ---------
 
 - Fix #939: custom legacy version parsing (non PEP 440) after packaging >= 22.0 removed support.
 
-
-3.7.2 (2023-01-24)
-==================
-
-
-
-
-
-Bug Fixes
----------
-
-- Fix #928: correct default for pre-release matching after switching from ``pkg_resources`` to ``packaging``.
-
-- Fix #949: correct parsing of wheel tags for Python 3.10 and above.
-
```

### Comparing `devpi-common-4.0.3/devpi_common/archive.py` & `devpi_common-4.0.4/devpi_common/archive.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,15 +91,18 @@
         for member in members:
             target = to_path.joinpath(member.name)
             try:
                 target.relative_to(to_path)
             except ValueError as e:
                 raise ValueError(
                     f"archive name {member.name!r} out of bound") from e
-        self._archive.extractall(str(to_path))
+        if hasattr(tarfile, 'data_filter'):
+            self._archive.extractall(str(to_path), members=members, filter='data')
+        else:
+            self._archive.extractall(str(to_path), members=members)  # noqa: S202
 
 
 class ZipArchive(BaseArchive):
     def __init__(self, file):
         super(ZipArchive, self).__init__(file)
         self._archive = zipfile.ZipFile(file)
```

### Comparing `devpi-common-4.0.3/devpi_common/request.py` & `devpi_common-4.0.4/devpi_common/request.py`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/devpi_common/terminal.py` & `devpi_common-4.0.4/devpi_common/terminal.py`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/devpi_common/types.py` & `devpi_common-4.0.4/devpi_common/types.py`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/devpi_common/url.py` & `devpi_common-4.0.4/devpi_common/url.py`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/devpi_common/validation.py` & `devpi_common-4.0.4/devpi_common/validation.py`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/devpi_common/viewhelp.py` & `devpi_common-4.0.4/devpi_common/viewhelp.py`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/devpi_common.egg-info/PKG-INFO` & `devpi_common-4.0.4/devpi_common.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devpi-common
-Version: 4.0.3
+Version: 4.0.4
 Summary: Utilities jointly used by devpi-server, devpi-client and others.
 Maintainer-email: Florian Schulze <mail@pyfidelity.com>
 License: 
           Permission is hereby granted, free of charge, to any person obtaining a copy
           of this software and associated documentation files (the "Software"), to deal
           in the Software without restriction, including without limitation the rights
           to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -36,15 +36,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: lazy
-Requires-Dist: packaging>=22
+Requires-Dist: packaging-legacy
 Requires-Dist: requests>=2.3.0
 
 
 This package contains utility functions used by devpi-server and devpi-client.
 
 See http://doc.devpi.net for more information.
 
@@ -55,14 +55,26 @@
 =========
 
 
 
 
 .. towncrier release notes start
 
+4.0.4 (2024-04-20)
+==================
+
+Bug Fixes
+---------
+
+- Use ``filter='data'`` for ``extractall`` call on supported Python versions as additional guard to the existing out of path checks against malicious tar files.
+
+- Remove custom ``LegacyVersion`` and use ``packaging-legacy`` instead, which is also used by pypi.org.
+
+
+
 4.0.3 (2023-11-23)
 ==================
 
 Bug Fixes
 ---------
 
 - Add ``is_prerelease`` and other methods to ``LegacyVersion`` to fix ``get_sorted_versions`` with ``stable=True`` and some other cases.
@@ -110,22 +122,7 @@
 
 
 Bug Fixes
 ---------
 
 - Fix #939: custom legacy version parsing (non PEP 440) after packaging >= 22.0 removed support.
 
-
-3.7.2 (2023-01-24)
-==================
-
-
-
-
-
-Bug Fixes
----------
-
-- Fix #928: correct default for pre-release matching after switching from ``pkg_resources`` to ``packaging``.
-
-- Fix #949: correct parsing of wheel tags for Python 3.10 and above.
-
```

### Comparing `devpi-common-4.0.3/devpi_common.egg-info/SOURCES.txt` & `devpi_common-4.0.4/devpi_common.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 testing/__pycache__/test_archive.cpython-38-pytest-7.0.0.pyc
 testing/__pycache__/test_archive.cpython-38-pytest-7.0.1.pyc
 testing/__pycache__/test_archive.cpython-38-pytest-7.1.2.pyc
 testing/__pycache__/test_archive.cpython-38-pytest-7.2.0.pyc
 testing/__pycache__/test_archive.cpython-38-pytest-7.3.1.pyc
 testing/__pycache__/test_archive.cpython-38-pytest-7.4.0.pyc
 testing/__pycache__/test_archive.cpython-38-pytest-7.4.2.pyc
+testing/__pycache__/test_archive.cpython-38-pytest-7.4.3.pyc
+testing/__pycache__/test_archive.cpython-39-pytest-8.1.1.pyc
 testing/__pycache__/test_archive.pypy-27-PYTEST.pyc
 testing/__pycache__/test_archive.pypy37-pytest-7.0.1.pyc
 testing/__pycache__/test_archive.pypy37-pytest-7.1.2.pyc
 testing/__pycache__/test_lazydecorator.cpython-27-PYTEST.pyc
 testing/__pycache__/test_lazydecorator.cpython-34-PYTEST.pyc
 testing/__pycache__/test_lazydecorator.cpython-35-pytest-5.3.1.pyc
 testing/__pycache__/test_lazydecorator.cpython-35-pytest-6.1.2.pyc
@@ -59,14 +61,16 @@
 testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.0.0.pyc
 testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.0.1.pyc
 testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.1.2.pyc
 testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.2.0.pyc
 testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.3.1.pyc
 testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.4.0.pyc
 testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.4.2.pyc
+testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.4.3.pyc
+testing/__pycache__/test_lazydecorator.cpython-39-pytest-8.1.1.pyc
 testing/__pycache__/test_lazydecorator.pypy-27-PYTEST.pyc
 testing/__pycache__/test_lazydecorator.pypy37-pytest-7.0.1.pyc
 testing/__pycache__/test_lazydecorator.pypy37-pytest-7.1.2.pyc
 testing/__pycache__/test_metadata.cpython-27-PYTEST.pyc
 testing/__pycache__/test_metadata.cpython-34-PYTEST.pyc
 testing/__pycache__/test_metadata.cpython-35-pytest-5.3.1.pyc
 testing/__pycache__/test_metadata.cpython-35-pytest-6.1.2.pyc
@@ -78,14 +82,16 @@
 testing/__pycache__/test_metadata.cpython-38-pytest-7.0.0.pyc
 testing/__pycache__/test_metadata.cpython-38-pytest-7.0.1.pyc
 testing/__pycache__/test_metadata.cpython-38-pytest-7.1.2.pyc
 testing/__pycache__/test_metadata.cpython-38-pytest-7.2.0.pyc
 testing/__pycache__/test_metadata.cpython-38-pytest-7.3.1.pyc
 testing/__pycache__/test_metadata.cpython-38-pytest-7.4.0.pyc
 testing/__pycache__/test_metadata.cpython-38-pytest-7.4.2.pyc
+testing/__pycache__/test_metadata.cpython-38-pytest-7.4.3.pyc
+testing/__pycache__/test_metadata.cpython-39-pytest-8.1.1.pyc
 testing/__pycache__/test_metadata.pypy-27-PYTEST.pyc
 testing/__pycache__/test_metadata.pypy37-pytest-7.0.1.pyc
 testing/__pycache__/test_metadata.pypy37-pytest-7.1.2.pyc
 testing/__pycache__/test_proc.cpython-27-PYTEST.pyc
 testing/__pycache__/test_proc.cpython-34-PYTEST.pyc
 testing/__pycache__/test_proc.cpython-35-pytest-5.3.1.pyc
 testing/__pycache__/test_proc.cpython-35-pytest-6.1.2.pyc
@@ -114,14 +120,16 @@
 testing/__pycache__/test_request.cpython-38-pytest-7.0.0.pyc
 testing/__pycache__/test_request.cpython-38-pytest-7.0.1.pyc
 testing/__pycache__/test_request.cpython-38-pytest-7.1.2.pyc
 testing/__pycache__/test_request.cpython-38-pytest-7.2.0.pyc
 testing/__pycache__/test_request.cpython-38-pytest-7.3.1.pyc
 testing/__pycache__/test_request.cpython-38-pytest-7.4.0.pyc
 testing/__pycache__/test_request.cpython-38-pytest-7.4.2.pyc
+testing/__pycache__/test_request.cpython-38-pytest-7.4.3.pyc
+testing/__pycache__/test_request.cpython-39-pytest-8.1.1.pyc
 testing/__pycache__/test_request.pypy-27-PYTEST.pyc
 testing/__pycache__/test_request.pypy37-pytest-7.0.1.pyc
 testing/__pycache__/test_request.pypy37-pytest-7.1.2.pyc
 testing/__pycache__/test_types.cpython-27-PYTEST.pyc
 testing/__pycache__/test_types.cpython-34-PYTEST.pyc
 testing/__pycache__/test_types.cpython-35-pytest-5.3.1.pyc
 testing/__pycache__/test_types.cpython-35-pytest-6.1.2.pyc
@@ -133,14 +141,16 @@
 testing/__pycache__/test_types.cpython-38-pytest-7.0.0.pyc
 testing/__pycache__/test_types.cpython-38-pytest-7.0.1.pyc
 testing/__pycache__/test_types.cpython-38-pytest-7.1.2.pyc
 testing/__pycache__/test_types.cpython-38-pytest-7.2.0.pyc
 testing/__pycache__/test_types.cpython-38-pytest-7.3.1.pyc
 testing/__pycache__/test_types.cpython-38-pytest-7.4.0.pyc
 testing/__pycache__/test_types.cpython-38-pytest-7.4.2.pyc
+testing/__pycache__/test_types.cpython-38-pytest-7.4.3.pyc
+testing/__pycache__/test_types.cpython-39-pytest-8.1.1.pyc
 testing/__pycache__/test_types.pypy-27-PYTEST.pyc
 testing/__pycache__/test_types.pypy37-pytest-7.0.1.pyc
 testing/__pycache__/test_types.pypy37-pytest-7.1.2.pyc
 testing/__pycache__/test_url.cpython-27-PYTEST.pyc
 testing/__pycache__/test_url.cpython-34-PYTEST.pyc
 testing/__pycache__/test_url.cpython-35-pytest-5.3.1.pyc
 testing/__pycache__/test_url.cpython-35-pytest-6.1.2.pyc
@@ -152,14 +162,16 @@
 testing/__pycache__/test_url.cpython-38-pytest-7.0.0.pyc
 testing/__pycache__/test_url.cpython-38-pytest-7.0.1.pyc
 testing/__pycache__/test_url.cpython-38-pytest-7.1.2.pyc
 testing/__pycache__/test_url.cpython-38-pytest-7.2.0.pyc
 testing/__pycache__/test_url.cpython-38-pytest-7.3.1.pyc
 testing/__pycache__/test_url.cpython-38-pytest-7.4.0.pyc
 testing/__pycache__/test_url.cpython-38-pytest-7.4.2.pyc
+testing/__pycache__/test_url.cpython-38-pytest-7.4.3.pyc
+testing/__pycache__/test_url.cpython-39-pytest-8.1.1.pyc
 testing/__pycache__/test_url.pypy-27-PYTEST.pyc
 testing/__pycache__/test_url.pypy37-pytest-7.0.1.pyc
 testing/__pycache__/test_url.pypy37-pytest-7.1.2.pyc
 testing/__pycache__/test_validation.cpython-27-PYTEST.pyc
 testing/__pycache__/test_validation.cpython-34-PYTEST.pyc
 testing/__pycache__/test_validation.cpython-35-pytest-5.3.1.pyc
 testing/__pycache__/test_validation.cpython-35-pytest-6.1.2.pyc
@@ -171,11 +183,13 @@
 testing/__pycache__/test_validation.cpython-38-pytest-7.0.0.pyc
 testing/__pycache__/test_validation.cpython-38-pytest-7.0.1.pyc
 testing/__pycache__/test_validation.cpython-38-pytest-7.1.2.pyc
 testing/__pycache__/test_validation.cpython-38-pytest-7.2.0.pyc
 testing/__pycache__/test_validation.cpython-38-pytest-7.3.1.pyc
 testing/__pycache__/test_validation.cpython-38-pytest-7.4.0.pyc
 testing/__pycache__/test_validation.cpython-38-pytest-7.4.2.pyc
+testing/__pycache__/test_validation.cpython-38-pytest-7.4.3.pyc
+testing/__pycache__/test_validation.cpython-39-pytest-8.1.1.pyc
 testing/__pycache__/test_validation.pypy-27-PYTEST.pyc
 testing/__pycache__/test_validation.pypy37-pytest-7.0.1.pyc
 testing/__pycache__/test_validation.pypy37-pytest-7.1.2.pyc
 testing/data/slash.tar.gz
```

### Comparing `devpi-common-4.0.3/pyproject.toml` & `devpi_common-4.0.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [project]
 dynamic = ["version", "readme"]
 name = "devpi-common"
 description = "Utilities jointly used by devpi-server, devpi-client and others."
 dependencies = [
     "lazy",
-    "packaging>=22",
+    "packaging-legacy",
     "requests>=2.3.0",
 ]
 requires-python = ">=3.7"
 maintainers = [
     {name = "Florian Schulze", email = "mail@pyfidelity.com"}
 ]
 license = {file = "LICENSE"}
```

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-27-PYTEST.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-27-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-34-PYTEST.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-34-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-35-pytest-5.3.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-35-pytest-5.3.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-35-pytest-6.1.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-35-pytest-6.1.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-36-pytest-6.0.0rc1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-36-pytest-6.0.0rc1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-36-pytest-6.2.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-36-pytest-6.2.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-36-pytest-7.0.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-36-pytest-7.0.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-37-pytest-7.2.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-37-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-37-pytest-7.2.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-37-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-38-pytest-7.0.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-38-pytest-7.0.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-38-pytest-7.0.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-38-pytest-7.0.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-38-pytest-7.1.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-38-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-38-pytest-7.2.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-38-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-38-pytest-7.3.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-38-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-38-pytest-7.4.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-38-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_archive.cpython-38-pytest-7.4.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_archive.cpython-38-pytest-7.4.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_archive.pypy-27-PYTEST.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_archive.pypy-27-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_archive.pypy37-pytest-7.0.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_archive.pypy37-pytest-7.0.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_archive.pypy37-pytest-7.1.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_archive.pypy37-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-27-PYTEST.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-27-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-34-PYTEST.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-34-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-35-pytest-5.3.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-35-pytest-5.3.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-35-pytest-6.1.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-35-pytest-6.1.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-36-pytest-6.0.0rc1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-36-pytest-6.0.0rc1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-36-pytest-6.2.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-36-pytest-6.2.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-36-pytest-7.0.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-36-pytest-7.0.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-37-pytest-7.2.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-37-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-37-pytest-7.2.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-37-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.0.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.0.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.0.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.0.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.1.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.2.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.3.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.4.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.4.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.cpython-38-pytest-7.4.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.pypy-27-PYTEST.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.pypy-27-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.pypy37-pytest-7.0.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.pypy37-pytest-7.0.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_lazydecorator.pypy37-pytest-7.1.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_lazydecorator.pypy37-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-27-PYTEST.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-27-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-34-PYTEST.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-34-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-35-pytest-5.3.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-35-pytest-5.3.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-35-pytest-6.1.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-35-pytest-6.1.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-36-pytest-6.0.0rc1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-36-pytest-6.0.0rc1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-36-pytest-6.2.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-36-pytest-6.2.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-36-pytest-7.0.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-36-pytest-7.0.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-37-pytest-7.2.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-37-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-37-pytest-7.2.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-37-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-38-pytest-7.0.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-38-pytest-7.0.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-38-pytest-7.0.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-38-pytest-7.0.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-38-pytest-7.1.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-38-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-38-pytest-7.2.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-38-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-38-pytest-7.3.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-38-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-38-pytest-7.4.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-38-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_metadata.cpython-38-pytest-7.4.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_metadata.cpython-38-pytest-7.4.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_metadata.pypy-27-PYTEST.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_metadata.pypy-27-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_metadata.pypy37-pytest-7.0.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_metadata.pypy37-pytest-7.0.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_metadata.pypy37-pytest-7.1.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_metadata.pypy37-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-27-PYTEST.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-27-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-34-PYTEST.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-34-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-35-pytest-5.3.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-35-pytest-5.3.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-35-pytest-6.1.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-35-pytest-6.1.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-36-pytest-6.0.0rc1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-36-pytest-6.0.0rc1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-36-pytest-6.2.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-36-pytest-6.2.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-36-pytest-7.0.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-36-pytest-7.0.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-37-pytest-7.2.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-37-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-37-pytest-7.2.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-37-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-38-pytest-7.0.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-38-pytest-7.0.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-38-pytest-7.0.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-38-pytest-7.0.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-38-pytest-7.1.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-38-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-38-pytest-7.2.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-38-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_proc.cpython-38-pytest-7.4.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_proc.cpython-38-pytest-7.4.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_proc.pypy-27-PYTEST.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_proc.pypy-27-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_proc.pypy37-pytest-7.0.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_proc.pypy37-pytest-7.0.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_proc.pypy37-pytest-7.1.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_proc.pypy37-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_request.cpython-27-PYTEST.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_request.cpython-27-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_request.cpython-34-PYTEST.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_request.cpython-34-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_request.cpython-35-pytest-5.3.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_request.cpython-35-pytest-5.3.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_request.cpython-35-pytest-6.1.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_request.cpython-35-pytest-6.1.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_request.cpython-36-pytest-6.0.0rc1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_request.cpython-36-pytest-6.0.0rc1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_request.cpython-36-pytest-6.2.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_request.cpython-36-pytest-6.2.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_request.cpython-36-pytest-7.0.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_request.cpython-36-pytest-7.0.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_request.cpython-37-pytest-7.2.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_request.cpython-37-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_request.cpython-37-pytest-7.2.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_request.cpython-37-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_request.cpython-38-pytest-7.0.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_request.cpython-38-pytest-7.0.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_request.cpython-38-pytest-7.0.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_request.cpython-38-pytest-7.0.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_request.cpython-38-pytest-7.1.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_request.cpython-38-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_request.cpython-38-pytest-7.2.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_request.cpython-38-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_request.cpython-38-pytest-7.3.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_request.cpython-38-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_request.cpython-38-pytest-7.4.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_request.cpython-38-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_request.cpython-38-pytest-7.4.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_request.cpython-38-pytest-7.4.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_request.pypy-27-PYTEST.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_request.pypy-27-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_request.pypy37-pytest-7.0.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_request.pypy37-pytest-7.0.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_request.pypy37-pytest-7.1.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_request.pypy37-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_types.cpython-27-PYTEST.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_types.cpython-27-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_types.cpython-34-PYTEST.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_types.cpython-34-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_types.cpython-35-pytest-5.3.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_types.cpython-35-pytest-5.3.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_types.cpython-35-pytest-6.1.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_types.cpython-35-pytest-6.1.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_types.cpython-36-pytest-6.0.0rc1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_types.cpython-36-pytest-6.0.0rc1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_types.cpython-36-pytest-6.2.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_types.cpython-36-pytest-6.2.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_types.cpython-36-pytest-7.0.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_types.cpython-36-pytest-7.0.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_types.cpython-37-pytest-7.2.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_types.cpython-37-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_types.cpython-37-pytest-7.2.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_types.cpython-37-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_types.cpython-38-pytest-7.0.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_types.cpython-38-pytest-7.0.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_types.cpython-38-pytest-7.0.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_types.cpython-38-pytest-7.0.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_types.cpython-38-pytest-7.1.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_types.cpython-38-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_types.cpython-38-pytest-7.2.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_types.cpython-38-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_types.cpython-38-pytest-7.3.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_types.cpython-38-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_types.cpython-38-pytest-7.4.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_types.cpython-38-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_types.cpython-38-pytest-7.4.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_types.cpython-38-pytest-7.4.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_types.pypy-27-PYTEST.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_types.pypy-27-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_types.pypy37-pytest-7.0.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_types.pypy37-pytest-7.0.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_types.pypy37-pytest-7.1.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_types.pypy37-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_url.cpython-27-PYTEST.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_url.cpython-27-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_url.cpython-34-PYTEST.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_url.cpython-34-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_url.cpython-35-pytest-5.3.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_url.cpython-35-pytest-5.3.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_url.cpython-35-pytest-6.1.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_url.cpython-35-pytest-6.1.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_url.cpython-36-pytest-6.0.0rc1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_url.cpython-36-pytest-6.0.0rc1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_url.cpython-36-pytest-6.2.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_url.cpython-36-pytest-6.2.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_url.cpython-36-pytest-7.0.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_url.cpython-36-pytest-7.0.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_url.cpython-37-pytest-7.2.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_url.cpython-37-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_url.cpython-37-pytest-7.2.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_url.cpython-37-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_url.cpython-38-pytest-7.0.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_url.cpython-38-pytest-7.0.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_url.cpython-38-pytest-7.0.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_url.cpython-38-pytest-7.0.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_url.cpython-38-pytest-7.1.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_url.cpython-38-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_url.cpython-38-pytest-7.2.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_url.cpython-38-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_url.cpython-38-pytest-7.3.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_url.cpython-38-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_url.cpython-38-pytest-7.4.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_url.cpython-38-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_url.cpython-38-pytest-7.4.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_url.cpython-38-pytest-7.4.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_url.pypy-27-PYTEST.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_url.pypy-27-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_url.pypy37-pytest-7.0.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_url.pypy37-pytest-7.0.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_url.pypy37-pytest-7.1.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_url.pypy37-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-27-PYTEST.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-27-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-34-PYTEST.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-34-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-35-pytest-5.3.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-35-pytest-5.3.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-35-pytest-6.1.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-35-pytest-6.1.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-36-pytest-6.0.0rc1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-36-pytest-6.0.0rc1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-36-pytest-6.2.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-36-pytest-6.2.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-36-pytest-7.0.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-36-pytest-7.0.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-37-pytest-7.2.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-37-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-37-pytest-7.2.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-37-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-38-pytest-7.0.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-38-pytest-7.0.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-38-pytest-7.0.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-38-pytest-7.0.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-38-pytest-7.1.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-38-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-38-pytest-7.2.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-38-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-38-pytest-7.3.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-38-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-38-pytest-7.4.0.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-38-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_validation.cpython-38-pytest-7.4.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_validation.cpython-38-pytest-7.4.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_validation.pypy-27-PYTEST.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_validation.pypy-27-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_validation.pypy37-pytest-7.0.1.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_validation.pypy37-pytest-7.0.1.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/__pycache__/test_validation.pypy37-pytest-7.1.2.pyc` & `devpi_common-4.0.4/testing/__pycache__/test_validation.pypy37-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/test_archive.py` & `devpi_common-4.0.4/testing/test_archive.py`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/test_lazydecorator.py` & `devpi_common-4.0.4/testing/test_lazydecorator.py`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/test_metadata.py` & `devpi_common-4.0.4/testing/test_metadata.py`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/test_request.py` & `devpi_common-4.0.4/testing/test_request.py`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/test_types.py` & `devpi_common-4.0.4/testing/test_types.py`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/test_url.py` & `devpi_common-4.0.4/testing/test_url.py`

 * *Files identical despite different names*

### Comparing `devpi-common-4.0.3/testing/test_validation.py` & `devpi_common-4.0.4/testing/test_validation.py`

 * *Files identical despite different names*

