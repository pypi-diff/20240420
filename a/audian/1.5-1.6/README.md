# Comparing `tmp/audian-1.5.tar.gz` & `tmp/audian-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audian-1.5.tar", last modified: Sun Aug  7 22:03:52 2022, max compression
+gzip compressed data, was "audian-1.6.tar", last modified: Sat Apr 20 09:37:03 2024, max compression
```

## Comparing `audian-1.5.tar` & `audian-1.6.tar`

### file list

```diff
@@ -1,18 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-07 22:03:52.380851 audian-1.5/
--rw-rw-r--   0 root         (0) root         (0)    35141 2022-08-04 14:57:09.000000 audian-1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      808 2022-08-07 22:03:52.380851 audian-1.5/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1607 2022-08-06 17:30:09.000000 audian-1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-07 22:03:52.380851 audian-1.5/audian/
--rw-rw-r--   0 root         (0) root         (0)      103 2022-08-04 15:23:22.000000 audian-1.5/audian/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    52254 2022-08-07 22:01:35.000000 audian-1.5/audian/audian.py
--rw-rw-r--   0 root         (0) root         (0)    13425 2022-08-07 14:47:21.000000 audian-1.5/audian/configfile.py
--rw-rw-r--   0 root         (0) root         (0)      199 2022-08-07 22:03:32.000000 audian-1.5/audian/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-07 22:03:52.380851 audian-1.5/audian.egg-info/
--rw-r--r--   0 root         (0) root         (0)      808 2022-08-07 22:03:52.000000 audian-1.5/audian.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      283 2022-08-07 22:03:52.000000 audian-1.5/audian.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-07 22:03:52.000000 audian-1.5/audian.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2022-08-07 22:03:52.000000 audian-1.5/audian.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-08-07 22:03:52.000000 audian-1.5/audian.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-08-07 22:03:52.000000 audian-1.5/audian.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-07 22:03:52.380851 audian-1.5/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1223 2022-08-04 15:17:51.000000 audian-1.5/setup.py
+drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-20 09:37:03.470482 audian-1.6/
+-rw-rw-r--   0 benda     (1001) benda     (1001)    35141 2022-09-12 08:36:43.000000 audian-1.6/LICENSE
+-rw-r--r--   0 benda     (1001) benda     (1001)    46971 2024-04-20 09:37:03.470482 audian-1.6/PKG-INFO
+-rw-rw-r--   0 benda     (1001) benda     (1001)     5200 2024-03-13 09:56:03.000000 audian-1.6/README.md
+-rw-rw-r--   0 benda     (1001) benda     (1001)     1460 2024-04-20 09:33:52.000000 audian-1.6/pyproject.toml
+-rw-rw-r--   0 benda     (1001) benda     (1001)       38 2024-04-20 09:37:03.470482 audian-1.6/setup.cfg
+-rw-rw-r--   0 benda     (1001) benda     (1001)       38 2024-04-20 09:33:52.000000 audian-1.6/setup.py
+drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-20 09:37:03.466482 audian-1.6/src/
+drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-20 09:37:03.470482 audian-1.6/src/audian/
+-rw-rw-r--   0 benda     (1001) benda     (1001)       96 2024-04-20 09:33:52.000000 audian-1.6/src/audian/__init__.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    52259 2024-04-20 09:33:52.000000 audian-1.6/src/audian/audian.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    51241 2024-04-20 09:33:52.000000 audian-1.6/src/audian/audiangui.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    13425 2024-04-20 09:33:52.000000 audian-1.6/src/audian/configfile.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    72633 2024-04-20 09:33:52.000000 audian-1.6/src/audian/databrowser.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     7428 2024-04-20 09:33:52.000000 audian-1.6/src/audian/fulltraceplot.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    17684 2024-04-20 09:33:52.000000 audian-1.6/src/audian/markerdata.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     3470 2024-04-20 09:33:52.000000 audian-1.6/src/audian/oscillogramplot.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     4279 2024-04-20 09:33:52.000000 audian-1.6/src/audian/selectviewbox.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     6835 2024-04-20 09:33:52.000000 audian-1.6/src/audian/specitem.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     5566 2024-04-20 09:33:52.000000 audian-1.6/src/audian/spectrumplot.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     4036 2024-04-20 09:33:52.000000 audian-1.6/src/audian/timeaxisitem.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     6993 2024-04-20 09:33:52.000000 audian-1.6/src/audian/traceitem.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)      199 2024-04-20 09:33:52.000000 audian-1.6/src/audian/version.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     1209 2024-04-20 09:33:52.000000 audian-1.6/src/audian/yaxisitem.py
+drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-20 09:37:03.470482 audian-1.6/src/audian.egg-info/
+-rw-r--r--   0 benda     (1001) benda     (1001)    46971 2024-04-20 09:37:03.000000 audian-1.6/src/audian.egg-info/PKG-INFO
+-rw-rw-r--   0 benda     (1001) benda     (1001)      624 2024-04-20 09:37:03.000000 audian-1.6/src/audian.egg-info/SOURCES.txt
+-rw-rw-r--   0 benda     (1001) benda     (1001)        1 2024-04-20 09:37:03.000000 audian-1.6/src/audian.egg-info/dependency_links.txt
+-rw-rw-r--   0 benda     (1001) benda     (1001)       78 2024-04-20 09:37:03.000000 audian-1.6/src/audian.egg-info/entry_points.txt
+-rw-rw-r--   0 benda     (1001) benda     (1001)       65 2024-04-20 09:37:03.000000 audian-1.6/src/audian.egg-info/requires.txt
+-rw-rw-r--   0 benda     (1001) benda     (1001)        7 2024-04-20 09:37:03.000000 audian-1.6/src/audian.egg-info/top_level.txt
```

### Comparing `audian-1.5/LICENSE` & `audian-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `audian-1.5/audian/audian.py` & `audian-1.6/src/audian/audian.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,15 +339,15 @@
     return all_peaks, threshold, center
 
     
 ###############################################################################
 ## plotting etc.
     
 class SignalPlot:
-    def __init__(self, samplingrate, data, unit, filename, channel, path):
+    def __init__(self, data, samplingrate, unit, filename, channel, path):
         self.filepath = ''
         if platform.system() == 'Windows':
             self.filepath = path
         self.filename = filename
         self.channel = channel
         self.rate = samplingrate
         self.data = data
@@ -400,15 +400,15 @@
         plt.rcParams['keymap.save'] = ''
         if 'keymap.all_axes' in plt.rcParams:
             plt.rcParams['keymap.all_axes'] = ''
         
         # the figure:
         plt.ioff()
         self.fig = plt.figure(figsize=(15, 9), constrained_layout=True)
-        self.fig.canvas.manager.set_window_title('AUDIoANalyser: ' + self.filename + ' channel {0:d}'.format(self.channel))
+        self.fig.canvas.manager.set_window_title('AUDIoANalyzer: ' + self.filename + ' channel {0:d}'.format(self.channel))
         self.fig.canvas.mpl_connect('key_press_event', self.keypress)
         self.fig.canvas.mpl_connect('button_press_event', self.buttonpress)
         self.fig.canvas.mpl_connect('pick_event', self.onpick)
         gs = self.fig.add_gridspec(2, 1, height_ratios=[5, 2])
         gst = gs[0].subgridspec(2, 1, hspace=0.0)
         gsp = gs[1].subgridspec(1, 2)
         # trace plot:
@@ -1224,15 +1224,16 @@
         if not args.low_pass is None:
             data = bandpass_filter(data, rate, args.high_pass, args.low_pass)
         else:
             data = highpass_filter(data, rate, args.high_pass)
     unit = 'a.u.'
     
     # plot:
-    sp = SignalPlot(rate, data, unit, filename, channel, os.path.dirname(filepath))
+    sp = SignalPlot(data, rate, unit, filename, channel, os.path.dirname(filepath))
 
 
 def run():
     main(sys.argv[1:])
 
+    
 if __name__ == '__main__':
     run()
```

### Comparing `audian-1.5/audian/configfile.py` & `audian-1.6/src/audian/configfile.py`

 * *Files identical despite different names*

### Comparing `audian-1.5/setup.py` & `audian-1.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,55 @@
-from setuptools import setup, find_packages
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
 
-exec(open('audian/version.py').read())
+[project]
+name = "audian"
+dynamic = ["version"]
+dependencies = [
+  "scipy",
+  "numpy",
+  "numba",
+  "pandas",
+  "matplotlib",
+  "PyQt5",
+  "pyqtgraph",
+  "audioio>=2.1"
+]
+requires-python = ">=3.4"
+authors = [
+  {name = "Jan Benda", email = "jan.benda@uni-tuebingen.de"},
+]
+maintainers = [
+  {name = "Jan Benda", email = "jan.benda@uni-tuebingen.de"},
+]
+description = "GUI for viewing and analyzing recordings of animal vocalizations."
+readme = "README.md"
+license = {file = "LICENSE"}
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Environment :: Console",
+    "Intended Audience :: Science/Research",
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+    "Natural Language :: English",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.12",
+    "Operating System :: OS Independent",
+    "Topic :: Multimedia :: Sound/Audio",
+    "Topic :: Multimedia :: Sound/Audio :: Analysis",
+    "Topic :: Scientific/Engineering",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+]
 
-long_description = """
-# AUDIoANalyser
+[project.urls]
+Repository    = "https://github.com/bendalab/audian"
 
-Simple GUI for viewing biosignals.
-"""
+[project.scripts]
+audian    = "audian.audian:run"
+audiangui = "audian.audiangui:run"
 
-setup(
-    name = 'audian',
-    version = __version__,
-    author = 'Jan Benda',
-    author_email = "jan.benda@uni-tuebingen.de",
-    description = 'Simple GUI for viewing biosignals.',
-    long_description = long_description,
-    long_description_content_type = "text/markdown",
-    url = "https://github.com/bendalab/audian",
-    license = "GPLv3",
-    classifiers = [
-        "Development Status :: 4 - Beta",
-        "Environment :: Console",
-        "Intended Audience :: Science/Research",
-        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-        "Natural Language :: English",
-        "Programming Language :: Python :: 3",
-        "Operating System :: OS Independent",
-        "Topic :: Scientific/Engineering",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-    ],
-    packages = ['audian'],
-    entry_points = {
-        'console_scripts': [
-            'audian = audian.audian:run',
-        ]},
-    python_requires = '>=3.4',
-    install_requires = ['scipy', 'numpy', 'matplotlib', 'audioio'],
-)
+[tool.setuptools.dynamic]
+version = {attr = "audian.version.__version__"}
+
+[tool.pytest.ini_options]
+pythonpath = "src"
```

