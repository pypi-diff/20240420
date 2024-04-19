# Comparing `tmp/Payton-1.2.0.tar.gz` & `tmp/payton-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Payton-1.2.0.tar", last modified: Fri Nov 10 15:27:28 2023, max compression
+gzip compressed data, was "payton-1.2.1.tar", last modified: Fri Apr 19 22:37:53 2024, max compression
```

## Comparing `Payton-1.2.0.tar` & `payton-1.2.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 sinan     (1000) sinan     (1000)        0 2023-11-10 15:27:28.896547 Payton-1.2.0/
--rw-rw-r--   0 sinan     (1000) sinan     (1000)     1524 2022-01-27 20:36:55.000000 Payton-1.2.0/LICENSE
--rw-rw-r--   0 sinan     (1000) sinan     (1000)      113 2022-05-16 07:03:07.000000 Payton-1.2.0/MANIFEST.in
--rw-r--r--   0 sinan     (1000) sinan     (1000)    18030 2023-11-10 15:27:28.896547 Payton-1.2.0/PKG-INFO
-drwxrwxr-x   0 sinan     (1000) sinan     (1000)        0 2023-11-10 15:27:28.888547 Payton-1.2.0/Payton.egg-info/
--rw-r--r--   0 sinan     (1000) sinan     (1000)    18030 2023-11-10 15:27:28.000000 Payton-1.2.0/Payton.egg-info/PKG-INFO
--rw-rw-r--   0 sinan     (1000) sinan     (1000)     1458 2023-11-10 15:27:28.000000 Payton-1.2.0/Payton.egg-info/SOURCES.txt
--rw-rw-r--   0 sinan     (1000) sinan     (1000)        1 2023-11-10 15:27:28.000000 Payton-1.2.0/Payton.egg-info/dependency_links.txt
--rw-rw-r--   0 sinan     (1000) sinan     (1000)       87 2023-11-10 15:27:28.000000 Payton-1.2.0/Payton.egg-info/requires.txt
--rw-rw-r--   0 sinan     (1000) sinan     (1000)        7 2023-11-10 15:27:28.000000 Payton-1.2.0/Payton.egg-info/top_level.txt
--rw-rw-r--   0 sinan     (1000) sinan     (1000)    17414 2023-11-09 08:45:13.000000 Payton-1.2.0/README.md
-drwxrwxr-x   0 sinan     (1000) sinan     (1000)        0 2023-11-10 15:27:28.888547 Payton-1.2.0/payton/
--rw-rw-r--   0 sinan     (1000) sinan     (1000)      188 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/__init__.py
-drwxrwxr-x   0 sinan     (1000) sinan     (1000)        0 2023-11-10 15:27:28.888547 Payton-1.2.0/payton/math/
--rw-rw-r--   0 sinan     (1000) sinan     (1000)      299 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/math/__init__.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)    11516 2022-03-17 17:15:24.000000 Payton-1.2.0/payton/math/functions.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)     9166 2022-05-09 17:20:43.000000 Payton-1.2.0/payton/math/geometry.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)     1223 2022-02-20 10:48:12.000000 Payton-1.2.0/payton/math/matrix.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)      198 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/math/types.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)       71 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/math/vector.py
-drwxrwxr-x   0 sinan     (1000) sinan     (1000)        0 2023-11-10 15:27:28.892547 Payton-1.2.0/payton/scene/
--rw-rw-r--   0 sinan     (1000) sinan     (1000)      903 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/scene/__init__.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)    14501 2023-11-09 08:45:13.000000 Payton-1.2.0/payton/scene/camera.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)     2433 2023-11-09 08:45:13.000000 Payton-1.2.0/payton/scene/clock.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)     4663 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/scene/collision.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)     8784 2022-03-28 18:23:00.000000 Payton-1.2.0/payton/scene/controller.py
-drwxrwxr-x   0 sinan     (1000) sinan     (1000)        0 2023-11-10 15:27:28.892547 Payton-1.2.0/payton/scene/font/
--rwxrwxr-x   0 sinan     (1000) sinan     (1000)   188640 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/scene/font/Glametrix.otf
-drwxrwxr-x   0 sinan     (1000) sinan     (1000)        0 2023-11-10 15:27:28.896547 Payton-1.2.0/payton/scene/geometry/
--rw-rw-r--   0 sinan     (1000) sinan     (1000)      733 2022-03-13 20:00:28.000000 Payton-1.2.0/payton/scene/geometry/__init__.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)     6780 2022-11-25 09:48:57.000000 Payton-1.2.0/payton/scene/geometry/awp3d.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)    38125 2022-11-25 09:47:37.000000 Payton-1.2.0/payton/scene/geometry/base.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)     4265 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/scene/geometry/cube.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)     2529 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/scene/geometry/cylinder.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)      588 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/scene/geometry/export.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)    17267 2022-11-25 09:47:56.000000 Payton-1.2.0/payton/scene/geometry/md2.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)     8807 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/scene/geometry/mesh.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)     1729 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/scene/geometry/particle.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)     3809 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/scene/geometry/plane.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)     8601 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/scene/geometry/ragdoll.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)     3795 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/scene/geometry/sphere.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)     8491 2022-05-09 17:21:15.000000 Payton-1.2.0/payton/scene/geometry/wavefront.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)     6545 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/scene/grid.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)     3899 2022-05-09 17:20:43.000000 Payton-1.2.0/payton/scene/gtk.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)     4961 2022-03-29 17:15:50.000000 Payton-1.2.0/payton/scene/gtkcontroller.py
-drwxrwxr-x   0 sinan     (1000) sinan     (1000)        0 2023-11-10 15:27:28.896547 Payton-1.2.0/payton/scene/gui/
--rw-rw-r--   0 sinan     (1000) sinan     (1000)      420 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/scene/gui/__init__.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)    12493 2023-11-10 15:23:47.000000 Payton-1.2.0/payton/scene/gui/base.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)     2347 2023-11-10 15:24:22.000000 Payton-1.2.0/payton/scene/gui/help.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)    58088 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/scene/gui/monofonto.ttf
--rw-rw-r--   0 sinan     (1000) sinan     (1000)    15635 2023-11-10 15:10:19.000000 Payton-1.2.0/payton/scene/gui/window.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)     2889 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/scene/light.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)     9733 2022-05-09 17:20:35.000000 Payton-1.2.0/payton/scene/material.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)     6879 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/scene/particle.png
--rw-rw-r--   0 sinan     (1000) sinan     (1000)      362 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/scene/physics.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)       69 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/scene/receiver.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)    29540 2022-04-18 11:13:47.000000 Payton-1.2.0/payton/scene/scene.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)    13772 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/scene/shader.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)      221 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/scene/types.py
-drwxrwxr-x   0 sinan     (1000) sinan     (1000)        0 2023-11-10 15:27:28.896547 Payton-1.2.0/payton/tools/
--rw-rw-r--   0 sinan     (1000) sinan     (1000)       28 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/tools/__init__.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)      477 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/tools/bar.py
-drwxrwxr-x   0 sinan     (1000) sinan     (1000)        0 2023-11-10 15:27:28.896547 Payton-1.2.0/payton/tools/mesh/
--rw-rw-r--   0 sinan     (1000) sinan     (1000)      289 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/tools/mesh/__init__.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)     2713 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/tools/mesh/geometry.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)     3735 2022-01-27 20:36:56.000000 Payton-1.2.0/payton/tools/mesh/line.py
--rw-rw-r--   0 sinan     (1000) sinan     (1000)      283 2023-11-09 08:45:13.000000 Payton-1.2.0/pyproject.toml
--rw-rw-r--   0 sinan     (1000) sinan     (1000)      783 2023-11-10 15:27:28.900547 Payton-1.2.0/setup.cfg
+drwxrwxr-x   0 sinan     (1000) sinan     (1000)        0 2024-04-19 22:37:53.217710 payton-1.2.1/
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)     1524 2022-01-27 20:36:55.000000 payton-1.2.1/LICENSE
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)      113 2022-05-16 07:03:07.000000 payton-1.2.1/MANIFEST.in
+-rw-r--r--   0 sinan     (1000) sinan     (1000)    18030 2024-04-19 22:37:53.217710 payton-1.2.1/PKG-INFO
+drwxrwxr-x   0 sinan     (1000) sinan     (1000)        0 2024-04-19 22:37:53.217710 payton-1.2.1/Payton.egg-info/
+-rw-r--r--   0 sinan     (1000) sinan     (1000)    18030 2024-04-19 22:37:53.000000 payton-1.2.1/Payton.egg-info/PKG-INFO
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)     1458 2024-04-19 22:37:53.000000 payton-1.2.1/Payton.egg-info/SOURCES.txt
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)        1 2024-04-19 22:37:53.000000 payton-1.2.1/Payton.egg-info/dependency_links.txt
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)       87 2024-04-19 22:37:53.000000 payton-1.2.1/Payton.egg-info/requires.txt
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)        7 2024-04-19 22:37:53.000000 payton-1.2.1/Payton.egg-info/top_level.txt
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)    17414 2023-11-09 08:45:13.000000 payton-1.2.1/README.md
+drwxrwxr-x   0 sinan     (1000) sinan     (1000)        0 2024-04-19 22:37:53.205710 payton-1.2.1/payton/
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)      189 2024-04-19 22:17:18.000000 payton-1.2.1/payton/__init__.py
+drwxrwxr-x   0 sinan     (1000) sinan     (1000)        0 2024-04-19 22:37:53.205710 payton-1.2.1/payton/math/
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)      299 2022-01-27 20:36:56.000000 payton-1.2.1/payton/math/__init__.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)    11516 2022-03-17 17:15:24.000000 payton-1.2.1/payton/math/functions.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)     9166 2022-05-09 17:20:43.000000 payton-1.2.1/payton/math/geometry.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)     1223 2022-02-20 10:48:12.000000 payton-1.2.1/payton/math/matrix.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)      198 2022-01-27 20:36:56.000000 payton-1.2.1/payton/math/types.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)       71 2022-01-27 20:36:56.000000 payton-1.2.1/payton/math/vector.py
+drwxrwxr-x   0 sinan     (1000) sinan     (1000)        0 2024-04-19 22:37:53.209710 payton-1.2.1/payton/scene/
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)      904 2024-04-19 22:17:18.000000 payton-1.2.1/payton/scene/__init__.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)    14501 2023-11-09 08:45:13.000000 payton-1.2.1/payton/scene/camera.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)     2433 2023-11-09 08:45:13.000000 payton-1.2.1/payton/scene/clock.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)     4663 2022-01-27 20:36:56.000000 payton-1.2.1/payton/scene/collision.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)     8784 2022-03-28 18:23:00.000000 payton-1.2.1/payton/scene/controller.py
+drwxrwxr-x   0 sinan     (1000) sinan     (1000)        0 2024-04-19 22:37:53.209710 payton-1.2.1/payton/scene/font/
+-rwxrwxr-x   0 sinan     (1000) sinan     (1000)   188640 2022-01-27 20:36:56.000000 payton-1.2.1/payton/scene/font/Glametrix.otf
+drwxrwxr-x   0 sinan     (1000) sinan     (1000)        0 2024-04-19 22:37:53.213710 payton-1.2.1/payton/scene/geometry/
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)      733 2022-03-13 20:00:28.000000 payton-1.2.1/payton/scene/geometry/__init__.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)     6781 2024-04-19 22:17:18.000000 payton-1.2.1/payton/scene/geometry/awp3d.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)    38126 2024-04-19 22:17:19.000000 payton-1.2.1/payton/scene/geometry/base.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)     4266 2024-04-19 22:17:18.000000 payton-1.2.1/payton/scene/geometry/cube.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)     2530 2024-04-19 22:17:18.000000 payton-1.2.1/payton/scene/geometry/cylinder.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)      589 2024-04-19 22:17:18.000000 payton-1.2.1/payton/scene/geometry/export.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)    17268 2024-04-19 22:17:19.000000 payton-1.2.1/payton/scene/geometry/md2.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)     8808 2024-04-19 22:17:18.000000 payton-1.2.1/payton/scene/geometry/mesh.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)     1729 2022-01-27 20:36:56.000000 payton-1.2.1/payton/scene/geometry/particle.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)     3810 2024-04-19 22:17:18.000000 payton-1.2.1/payton/scene/geometry/plane.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)     8602 2024-04-19 22:17:18.000000 payton-1.2.1/payton/scene/geometry/ragdoll.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)     3795 2022-01-27 20:36:56.000000 payton-1.2.1/payton/scene/geometry/sphere.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)     8491 2022-05-09 17:21:15.000000 payton-1.2.1/payton/scene/geometry/wavefront.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)     6545 2022-01-27 20:36:56.000000 payton-1.2.1/payton/scene/grid.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)     3899 2023-11-22 21:05:21.000000 payton-1.2.1/payton/scene/gtk.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)     4961 2022-03-29 17:15:50.000000 payton-1.2.1/payton/scene/gtkcontroller.py
+drwxrwxr-x   0 sinan     (1000) sinan     (1000)        0 2024-04-19 22:37:53.213710 payton-1.2.1/payton/scene/gui/
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)      420 2022-01-27 20:36:56.000000 payton-1.2.1/payton/scene/gui/__init__.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)    12670 2024-04-19 22:30:55.000000 payton-1.2.1/payton/scene/gui/base.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)     2347 2023-11-10 15:24:22.000000 payton-1.2.1/payton/scene/gui/help.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)    58088 2022-01-27 20:36:56.000000 payton-1.2.1/payton/scene/gui/monofonto.ttf
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)    15635 2023-11-10 15:10:19.000000 payton-1.2.1/payton/scene/gui/window.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)     2889 2022-01-27 20:36:56.000000 payton-1.2.1/payton/scene/light.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)     9733 2022-05-09 17:20:35.000000 payton-1.2.1/payton/scene/material.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)     6879 2022-01-27 20:36:56.000000 payton-1.2.1/payton/scene/particle.png
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)      363 2024-04-19 22:17:18.000000 payton-1.2.1/payton/scene/physics.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)       69 2022-01-27 20:36:56.000000 payton-1.2.1/payton/scene/receiver.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)    29541 2024-04-19 22:17:19.000000 payton-1.2.1/payton/scene/scene.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)    13772 2022-01-27 20:36:56.000000 payton-1.2.1/payton/scene/shader.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)      221 2022-01-27 20:36:56.000000 payton-1.2.1/payton/scene/types.py
+drwxrwxr-x   0 sinan     (1000) sinan     (1000)        0 2024-04-19 22:37:53.213710 payton-1.2.1/payton/tools/
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)       28 2022-01-27 20:36:56.000000 payton-1.2.1/payton/tools/__init__.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)      477 2022-01-27 20:36:56.000000 payton-1.2.1/payton/tools/bar.py
+drwxrwxr-x   0 sinan     (1000) sinan     (1000)        0 2024-04-19 22:37:53.217710 payton-1.2.1/payton/tools/mesh/
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)      289 2022-01-27 20:36:56.000000 payton-1.2.1/payton/tools/mesh/__init__.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)     2713 2022-01-27 20:36:56.000000 payton-1.2.1/payton/tools/mesh/geometry.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)     3736 2024-04-19 22:17:18.000000 payton-1.2.1/payton/tools/mesh/line.py
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)      283 2023-11-09 08:45:13.000000 payton-1.2.1/pyproject.toml
+-rw-rw-r--   0 sinan     (1000) sinan     (1000)      783 2024-04-19 22:37:53.217710 payton-1.2.1/setup.cfg
```

### Comparing `Payton-1.2.0/LICENSE` & `payton-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/PKG-INFO` & `payton-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: Payton
-Version: 1.2.0
+Version: 1.2.1
 Summary: "3D Graphics Programming Toolkit"
 Home-page: https://github.com/sinanislekdemir/payton
 Author: Sinan Islekdemir
 Author-email: sinan@islekdemir.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Pillow>=10.1.0
+Requires-Dist: Pillow>=10.3.0
 Requires-Dist: PyOpenGL>=3.1.7
 Requires-Dist: pyrr>=0.10.3
 Requires-Dist: PySDL2>=0.9.16
 Requires-Dist: Cython>=3.0.5
-Requires-Dist: numpy>=1.26.1
+Requires-Dist: numpy>=1.26.4
 
 # Payton 3D SDK
 
 ![example workflow](https://github.com/sinanislekdemir/payton/actions/workflows/pythonpackage.yml/badge.svg)
 [![Downloads](https://pepy.tech/badge/payton/month)](https://pepy.tech/project/payton)
 [![Downloads](https://pepy.tech/badge/payton/week)](https://pepy.tech/project/payton)
```

### Comparing `Payton-1.2.0/Payton.egg-info/PKG-INFO` & `payton-1.2.1/Payton.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: Payton
-Version: 1.2.0
+Version: 1.2.1
 Summary: "3D Graphics Programming Toolkit"
 Home-page: https://github.com/sinanislekdemir/payton
 Author: Sinan Islekdemir
 Author-email: sinan@islekdemir.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Pillow>=10.1.0
+Requires-Dist: Pillow>=10.3.0
 Requires-Dist: PyOpenGL>=3.1.7
 Requires-Dist: pyrr>=0.10.3
 Requires-Dist: PySDL2>=0.9.16
 Requires-Dist: Cython>=3.0.5
-Requires-Dist: numpy>=1.26.1
+Requires-Dist: numpy>=1.26.4
 
 # Payton 3D SDK
 
 ![example workflow](https://github.com/sinanislekdemir/payton/actions/workflows/pythonpackage.yml/badge.svg)
 [![Downloads](https://pepy.tech/badge/payton/month)](https://pepy.tech/project/payton)
 [![Downloads](https://pepy.tech/badge/payton/week)](https://pepy.tech/project/payton)
```

### Comparing `Payton-1.2.0/Payton.egg-info/SOURCES.txt` & `payton-1.2.1/Payton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/README.md` & `payton-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/payton/math/functions.py` & `payton-1.2.1/payton/math/functions.py`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/payton/math/geometry.py` & `payton-1.2.1/payton/math/geometry.py`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/payton/math/matrix.py` & `payton-1.2.1/payton/math/matrix.py`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/payton/scene/__init__.py` & `payton-1.2.1/payton/scene/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,12 +15,13 @@
     * Material (`payton.scene.material`)
       * Shader (`payton.scene.shader`)
     * Type Support (`payton.scene.types`)
 
 Also, `payton.scene.scene` contents are accessible through `payton.scene` main
 module
 """
+
 # pylama:ignore=W
 from payton.scene.physics import physics_client
 from payton.scene.scene import SHADOW_HIGH, SHADOW_LOW, SHADOW_MID, SHADOW_NONE, Background, Scene
 
 __all__ = ["Scene", "Background", "SHADOW_HIGH", "SHADOW_LOW", "SHADOW_MID", "SHADOW_NONE", "physics_client"]
```

### Comparing `Payton-1.2.0/payton/scene/camera.py` & `payton-1.2.1/payton/scene/camera.py`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/payton/scene/clock.py` & `payton-1.2.1/payton/scene/clock.py`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/payton/scene/collision.py` & `payton-1.2.1/payton/scene/collision.py`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/payton/scene/controller.py` & `payton-1.2.1/payton/scene/controller.py`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/payton/scene/font/Glametrix.otf` & `payton-1.2.1/payton/scene/font/Glametrix.otf`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/payton/scene/geometry/__init__.py` & `payton-1.2.1/payton/scene/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/payton/scene/geometry/awp3d.py` & `payton-1.2.1/payton/scene/geometry/awp3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 Animated Wavefront Pack 3D files (AWP3D) are simply ZIP
 files with each frame packed inside.
 
 Easiest way to generate those files is through using Blender Export
 Add-On.
 """
+
 import os
 import time
 from typing import Any, Dict, List, Optional, Tuple
 from zipfile import ZipFile
 
 import numpy as np
```

### Comparing `Payton-1.2.0/payton/scene/geometry/base.py` & `payton-1.2.1/payton/scene/geometry/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base geometry definitions."""
+
 # pylama:ignore=C901
 import ctypes
 import logging
 from copy import deepcopy
 from functools import lru_cache
 from typing import Any, Dict, List, Optional, Tuple, Union, cast
```

### Comparing `Payton-1.2.0/payton/scene/geometry/cube.py` & `payton-1.2.1/payton/scene/geometry/cube.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Cube object module."""
+
 from typing import Any, Optional
 
 from payton.math.functions import min_max
 from payton.math.vector import Vector3D
 from payton.scene.geometry.mesh import Mesh
 from payton.scene.material import DEFAULT
```

### Comparing `Payton-1.2.0/payton/scene/geometry/cylinder.py` & `payton-1.2.1/payton/scene/geometry/cylinder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Cylinder module."""
+
 import math
 from typing import Any
 
 from payton.scene.geometry.mesh import Mesh
 
 
 class Cylinder(Mesh):
```

### Comparing `Payton-1.2.0/payton/scene/geometry/export.py` & `payton-1.2.1/payton/scene/geometry/export.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Export Import all to JSON."""
+
 from typing import Any
 
 from payton.scene.geometry.mesh import Mesh
 
 
 def export_json(mesh: Mesh, filename: str, **kwargs: Any) -> None:
     """Export the given mesh as JSON.
```

### Comparing `Payton-1.2.0/payton/scene/geometry/md2.py` & `payton-1.2.1/payton/scene/geometry/md2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 ID Software Quake 2 Model File.
 
 Some parts of this file is based on the original work from:
 https://github.com/adamlwgriffiths/PyMesh/tree/master/pymesh/md2
 """
+
 import logging
 import os
 import struct
 import time
 from copy import deepcopy
 from typing import Any, BinaryIO, Dict, Generator, List, NamedTuple, Optional, Tuple, cast
```

### Comparing `Payton-1.2.0/payton/scene/geometry/mesh.py` & `payton-1.2.1/payton/scene/geometry/mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Mesh object is a better option than using Object directly."""
+
 # pylama:ignore=C901
 import json
 import logging
 from typing import Any, Dict, Optional
 
 from payton.math.functions import invert_vector, plane_normal, vector_angle
 from payton.scene.geometry.base import Object
```

### Comparing `Payton-1.2.0/payton/scene/geometry/particle.py` & `payton-1.2.1/payton/scene/geometry/particle.py`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/payton/scene/geometry/plane.py` & `payton-1.2.1/payton/scene/geometry/plane.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Plane geometry module."""
+
 from itertools import product
 from typing import Any, List
 
 from payton.scene.geometry.mesh import Mesh
 from payton.scene.material import SOLID, WHITE
 
 _BULLET = False
```

### Comparing `Payton-1.2.0/payton/scene/geometry/ragdoll.py` & `payton-1.2.1/payton/scene/geometry/ragdoll.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Ragdoll Object
 
 Please note that, this is not a complete feature. Most likely many things
 are still quite hard to accomplish using RagDoll. But it will be gradually
 better in time. It just needs some time. Therefore, I am going to visit
 this file every now and then.
 """
+
 import math
 from typing import Any, Dict, Union
 
 from payton.scene.geometry.base import Line, Object
 from payton.scene.geometry.cube import Cube
 from payton.scene.geometry.sphere import Sphere
 from payton.scene.material import WIREFRAME
```

### Comparing `Payton-1.2.0/payton/scene/geometry/sphere.py` & `payton-1.2.1/payton/scene/geometry/sphere.py`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/payton/scene/geometry/wavefront.py` & `payton-1.2.1/payton/scene/geometry/wavefront.py`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/payton/scene/grid.py` & `payton-1.2.1/payton/scene/grid.py`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/payton/scene/gtk.py` & `payton-1.2.1/payton/scene/gtk.py`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/payton/scene/gtkcontroller.py` & `payton-1.2.1/payton/scene/gtkcontroller.py`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/payton/scene/gui/base.py` & `payton-1.2.1/payton/scene/gui/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import math
 import os
 from textwrap import wrap
 from typing import Any, Callable, Dict, List, Optional, Tuple, TypeVar, cast
 
 import numpy as np
 from OpenGL.GL import GL_DEPTH_TEST, glDisable, glEnable
-from PIL import Image, ImageDraw, ImageFont
+from PIL import Image, ImageDraw
+from PIL.ImageFont import ImageFont, truetype
 
 from payton.math.functions import ortho
 from payton.math.vector import Vector3D
 from payton.scene.geometry.base import Object
 from payton.scene.geometry.mesh import Mesh
 from payton.scene.shader import Shader
 
 S2 = TypeVar("S2", bound="Shape2D")
 
 
-def text_size(s: str, font: ImageFont) -> Tuple[int, int]:
+def text_size(s: str, font: ImageFont | None) -> Tuple[int, int]:
     timg = Image.new("RGBA", (1, 1))
     d = ImageDraw.Draw(timg)
     size = d.textbbox((0, 0), s, font=font)
     x = size[2] - size[0]
     y = size[3] - size[1]
     return int(x), int(y)
 
@@ -98,15 +99,15 @@
         We override the `lit` parameter for the super.
         This is not actually intended to be used publicly except if you want to
         setup your own render cycle.
         """
         super().render(False, shader, parent_matrix)
 
     @property
-    def font(self) -> None:
+    def font(self) -> None | ImageFont:
         """Return the fond of the shape"""
         if self._font is not None:
             return self._font
         if self.parent is not None:
             return self.parent.font
         return None
 
@@ -250,14 +251,16 @@
         if not self._init_text:
             self.draw_text()
         super().render(lit, shader, parent_matrix)
 
     @property
     def text_size(self) -> Tuple[int, int]:
         """Return the text size in pixels"""
+        if self.font is None:
+            return (0, 0)
         x, y = text_size(self.label, self.font)
         return max(int(self.size[0]), x), max(int(self.size[1]), y)
 
     def wrap(self, width_in_pixels: int) -> None:
         """Word-wrap the text to fit into the given pixel size
 
         Keyword arguments:
@@ -291,15 +294,15 @@
         color = (int(self.color[0] * 255), int(self.color[1] * 255), int(self.color[2] * 255), 255)
         if self.font is not None:
             d.text((1, 1), self.label, fill=color, font=self.font)
         else:
             d.text((1, 1), self.label, fill=color)
 
         if any(self.crop):
-            img = img.crop(self.crop)
+            img = img.crop((self.crop[0], self.crop[1], self.crop[2], self.crop[3]))
 
         del d
 
         self.material._image = img
         self.material.opacity = 1.0
         self.material.refresh()
         self._init_text = True
@@ -328,24 +331,24 @@
         self.width: int = width
         self.height: int = height
         self._fontname: str = font
         self.children: Dict[str, Object] = {}
         self._font_size: int = font_size
         if self._fontname != "":
             self.set_font(self._fontname, self._font_size)
-        self._font: ImageFont = None
+        self._font: ImageFont | None = None
         self._projection_matrix: Optional[np.ndarray] = None
         try:
             self.set_font(os.path.join(os.path.dirname(os.path.abspath(__file__)), "monofonto.ttf"))
         except OSError:
             # font not found but pillow has better than nothinf font
             pass
 
     @property
-    def font(self) -> ImageFont:
+    def font(self) -> ImageFont | None:
         """Return the HUD Image Font"""
         return self._font
 
     def add_child(self, name: str, obj: Object) -> bool:
         """Add 2D Shape into Hud.
 
         Note: this is a type ignore due to it's mismatch with Object add_child method
@@ -401,8 +404,8 @@
     def set_font(self, font_name: str, font_size: int = 16) -> None:
         """Set True Type font for the Hud
 
         Keyword arguments:
         font_name -- Name of the True Type font installed in the system
         font_size -- Size of the font in pixels
         """
-        self._font = ImageFont.truetype(font_name, font_size)
+        self._font = truetype(font_name, font_size)  # type: ignore
```

### Comparing `Payton-1.2.0/payton/scene/gui/help.py` & `payton-1.2.1/payton/scene/gui/help.py`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/payton/scene/gui/monofonto.ttf` & `payton-1.2.1/payton/scene/gui/monofonto.ttf`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/payton/scene/gui/window.py` & `payton-1.2.1/payton/scene/gui/window.py`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/payton/scene/light.py` & `payton-1.2.1/payton/scene/light.py`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/payton/scene/material.py` & `payton-1.2.1/payton/scene/material.py`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/payton/scene/particle.png` & `payton-1.2.1/payton/scene/particle.png`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/payton/scene/scene.py` & `payton-1.2.1/payton/scene/scene.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Main Scene Handler.
 
 Scene is the universe. Everything about Payton happens inside a Scene.
 """
+
 # pylama:ignore=C901
 import ctypes
 import logging
 import os
 import time
 from dataclasses import dataclass
 from typing import Any, Callable, Dict, List, Optional, Tuple, TypeVar
```

### Comparing `Payton-1.2.0/payton/scene/shader.py` & `payton-1.2.1/payton/scene/shader.py`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/payton/tools/mesh/geometry.py` & `payton-1.2.1/payton/tools/mesh/geometry.py`

 * *Files identical despite different names*

### Comparing `Payton-1.2.0/payton/tools/mesh/line.py` & `payton-1.2.1/payton/tools/mesh/line.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Payton Line to Mesh module"""
+
 from typing import List
 
 from payton.math.functions import add_vectors, create_rotation_matrix_raw, scale_vector, vector_transform
 from payton.math.vector import Vector3D
 from payton.scene.geometry import Line, Mesh
```

### Comparing `Payton-1.2.0/setup.cfg` & `payton-1.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Payton
-version = v1.2.0
+version = v1.2.1
 author = Sinan Islekdemir
 author_email = sinan@islekdemir.com
 description = "3D Graphics Programming Toolkit"
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sinanislekdemir/payton
 classifiers = 
@@ -13,20 +13,20 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 python_requires = >=3.10
 include_package_data = True
 install_requires = 
-	Pillow >=10.1.0
+	Pillow >=10.3.0
 	PyOpenGL >=3.1.7
 	pyrr >=0.10.3
 	PySDL2 >=0.9.16
 	Cython >=3.0.5
-	numpy >=1.26.1
+	numpy >=1.26.4
 
 [flake8]
 max-line-length = 120
 ignore = E203,W503
 max-complexity = 25
 
 [pylama:pycodestyle]
```

