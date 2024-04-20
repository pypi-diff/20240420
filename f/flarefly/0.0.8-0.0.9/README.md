# Comparing `tmp/flarefly-0.0.8.tar.gz` & `tmp/flarefly-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flarefly-0.0.8.tar", last modified: Thu May 11 07:43:14 2023, max compression
+gzip compressed data, was "flarefly-0.0.9.tar", last modified: Thu Aug  3 14:02:25 2023, max compression
```

## Comparing `flarefly-0.0.8.tar` & `flarefly-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:43:14.116884 flarefly-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-11 07:43:01.000000 flarefly-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 07:43:01.000000 flarefly-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-11 07:43:14.116884 flarefly-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-11 07:43:01.000000 flarefly-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:43:14.112884 flarefly-0.0.8/flarefly/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-11 07:43:01.000000 flarefly-0.0.8/flarefly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-11 07:43:01.000000 flarefly-0.0.8/flarefly/custom_pdfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-05-11 07:43:01.000000 flarefly-0.0.8/flarefly/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    95113 2023-05-11 07:43:01.000000 flarefly-0.0.8/flarefly/fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-11 07:43:01.000000 flarefly-0.0.8/flarefly/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 07:43:14.116884 flarefly-0.0.8/flarefly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-11 07:43:14.000000 flarefly-0.0.8/flarefly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-11 07:43:14.000000 flarefly-0.0.8/flarefly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 07:43:14.000000 flarefly-0.0.8/flarefly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-11 07:43:14.000000 flarefly-0.0.8/flarefly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-11 07:43:14.000000 flarefly-0.0.8/flarefly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 07:43:14.000000 flarefly-0.0.8/flarefly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 07:43:14.116884 flarefly-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-11 07:43:01.000000 flarefly-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:02:25.622574 flarefly-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-03 14:02:11.000000 flarefly-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:02:11.000000 flarefly-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-08-03 14:02:25.622574 flarefly-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-03 14:02:11.000000 flarefly-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:02:25.622574 flarefly-0.0.9/flarefly/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-03 14:02:11.000000 flarefly-0.0.9/flarefly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-08-03 14:02:11.000000 flarefly-0.0.9/flarefly/custom_pdfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-08-03 14:02:11.000000 flarefly-0.0.9/flarefly/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96365 2023-08-03 14:02:11.000000 flarefly-0.0.9/flarefly/fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-08-03 14:02:11.000000 flarefly-0.0.9/flarefly/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:02:25.622574 flarefly-0.0.9/flarefly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-08-03 14:02:25.000000 flarefly-0.0.9/flarefly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-03 14:02:25.000000 flarefly-0.0.9/flarefly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:02:25.000000 flarefly-0.0.9/flarefly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 14:02:25.000000 flarefly-0.0.9/flarefly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-03 14:02:25.000000 flarefly-0.0.9/flarefly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 14:02:25.000000 flarefly-0.0.9/flarefly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 14:02:25.622574 flarefly-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-08-03 14:02:11.000000 flarefly-0.0.9/setup.py
```

### Comparing `flarefly-0.0.8/LICENSE` & `flarefly-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flarefly-0.0.8/PKG-INFO` & `flarefly-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: flarefly
-Version: 0.0.8
+Version: 0.0.9
 Summary: FLexible And REliable Fitting LibrarY for particle physics analysis
 Home-page: https://github.com/flarefly/flarefly
 Author: flarefly-developers
 Author-email: flarefly@googlegroups.com
 License: GPL
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <img src="./flarefly_logo.png" width="200" /> <sub><sup>Logo by Andrea Sofia Triolo</sup></sub>
 
@@ -54,8 +54,7 @@
 
 
 | Type | Link |
 
 | -------------- | ------------- |
 
 | Binned invariant mass fit |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/flarefly/flarefly/blob/main/tutorials/flarefly_tutorial_Bzero.ipynb) |
-
```

### Comparing `flarefly-0.0.8/README.md` & `flarefly-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `flarefly-0.0.8/flarefly/custom_pdfs.py` & `flarefly-0.0.9/flarefly/custom_pdfs.py`

 * *Files identical despite different names*

### Comparing `flarefly-0.0.8/flarefly/data_handler.py` & `flarefly-0.0.9/flarefly/data_handler.py`

 * *Files identical despite different names*

### Comparing `flarefly-0.0.8/flarefly/fitter.py` & `flarefly-0.0.9/flarefly/fitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,16 @@
         -------------------------------------------------
         data_handler: flarefly.DataHandler
             The data handler containing the data to fit
 
         name_signal_pdf: list
             The list of names for the signal pdfs. The possible options are:
 
+            - 'nosignal'
+
             - 'gaussian'
 
             - 'doublegaus'
 
             - 'crystalball'
 
             - 'doublecb'
@@ -105,18 +107,24 @@
                 chi2 minimization if True, nll minmization else
                 Default value to False
         """
 
         self._data_handler_ = data_handler
         self._name_signal_pdf_ = name_signal_pdf
         self._name_background_pdf_ = name_background_pdf
-        self._signal_pdf_ = [None for _ in enumerate(name_signal_pdf)]
-        self._hist_signal_sample_ = [None for _ in enumerate(name_signal_pdf)]
-        self._kde_signal_sample_ = [None for _ in enumerate(name_signal_pdf)]
-        self._kde_signal_option_ = [None for _ in enumerate(name_signal_pdf)]
+        if self._name_signal_pdf_[0] == 'nosignal':
+            self._signal_pdf_ = []
+            self._hist_signal_sample_ = []
+            self._kde_signal_sample_ = []
+            self._kde_signal_option_ = []
+        else:
+            self._signal_pdf_ = [None for _ in enumerate(name_signal_pdf)]
+            self._hist_signal_sample_ = [None for _ in enumerate(name_signal_pdf)]
+            self._kde_signal_sample_ = [None for _ in enumerate(name_signal_pdf)]
+            self._kde_signal_option_ = [None for _ in enumerate(name_signal_pdf)]
         if self._name_background_pdf_[0] == 'nobkg':
             self._background_pdf_ = []
             self._hist_bkg_sample_ = []
             self._kde_bkg_sample_ = []
             self._kde_bkg_option_ = []
         else:
             self._background_pdf_ = [None for _ in enumerate(name_background_pdf)]
@@ -138,18 +146,22 @@
         self._init_bkg_pars_ = [{} for _ in enumerate(name_signal_pdf)]
         self._limits_sgn_pars_ = [{} for _ in enumerate(name_signal_pdf)]
         self._limits_bkg_pars_ = [{} for _ in enumerate(name_signal_pdf)]
         self._fix_sgn_pars_ = [{} for _ in enumerate(name_signal_pdf)]
         self._fix_bkg_pars_ = [{} for _ in enumerate(name_signal_pdf)]
         self._sgn_pars_ = [{} for _ in enumerate(name_signal_pdf)]
         self._bkg_pars_ = [{} for _ in enumerate(name_background_pdf)]
-        if self._name_background_pdf_[0] == 'nobkg':
+        if self._name_signal_pdf_[0] != 'nosignal' and self._name_background_pdf_[0] == 'nobkg':
             self._fracs_ = [None for _ in range(2 * len(name_signal_pdf) - 1)]
-        else:
+        elif self._name_signal_pdf_[0] == 'nosignal' and self._name_background_pdf_[0] != 'nobkg':
+            self._fracs_ = [None for _ in range(len(name_background_pdf) - 1)]
+        elif self._name_signal_pdf_[0] != 'nosignal' and self._name_background_pdf_[0] != 'nobkg':
             self._fracs_ = [None for _ in range(2 * len(name_signal_pdf) + len(name_background_pdf) - 1)]
+        else:
+            Logger('No signal nor background pdf defined', 'FATAL')
         self._rawyield_ = [0. for _ in enumerate(name_signal_pdf)]
         self._rawyield_err_ = [0. for _ in enumerate(name_signal_pdf)]
         self._minimizer_ = zfit.minimize.Minuit(verbosity=7)
         self._name_ = kwargs.get('name', '')
         self._ndf_ = None
         self._chi2_loss_ = kwargs.get('chi2_loss', False)
         self._base_sgn_cmap_ = plt.cm.get_cmap('viridis', len(self._signal_pdf_) * 4)
@@ -165,14 +177,17 @@
     # pylint: disable=too-many-branches, too-many-statements
     def __build_signal_pdfs(self, obs):
         """
         Helper function to compose the signal pdfs
         """
 
         for ipdf, pdf_name in enumerate(self._name_signal_pdf_):
+            if pdf_name == 'nosignal':
+                Logger('Performing fit with no signal pdf', 'WARNING')
+                break
             if pdf_name == 'gaussian':
                 self._init_sgn_pars_[ipdf].setdefault('mu', 1.865)
                 self._init_sgn_pars_[ipdf].setdefault('sigma', 0.010)
                 self._fix_sgn_pars_[ipdf].setdefault('mu', False)
                 self._fix_sgn_pars_[ipdf].setdefault('sigma', False)
                 self._limits_sgn_pars_[ipdf].setdefault('mu', [0, 1.e6])
                 self._limits_sgn_pars_[ipdf].setdefault('sigma', [0., 1.e6])
@@ -583,16 +598,20 @@
         # order of the pdfs is signal, background
 
         self.__build_signal_pdfs(obs)
         self.__build_background_pdfs(obs)
         self.__build_reflection_pdfs(obs)
 
         if len(self._signal_pdf_) + len(self._background_pdf_) == 1:
-            self._total_pdf_ = self._signal_pdf_[0]
-            return
+            if len(self._signal_pdf_) == 0:
+                self._total_pdf_ = self._background_pdf_[0]
+                return
+            if len(self._background_pdf_) == 0:
+                self._total_pdf_ = self._signal_pdf_[0]
+                return
 
         for ipdf, _ in enumerate(self._signal_pdf_):
             self._init_sgn_pars_[ipdf].setdefault('frac', 0.1)
             self._fix_sgn_pars_[ipdf].setdefault('frac', False)
             self._limits_sgn_pars_[ipdf].setdefault('frac', [0, 1.])
             if len(self._background_pdf_) == 0 and ipdf == len(self._signal_pdf_) - 1:
                 continue
@@ -678,16 +697,20 @@
                 refl_fracs.append(signal_fracs[-1] * self._refl_over_sgn_[isgn])
                 refl_err_fracs.append(signal_err_fracs[-1] * self._refl_over_sgn_[isgn])
             elif f'{self._name_}_frac_bkg' in par_name:
                 bkg_fracs.append(self._fit_result_.params[par_name]['value'])
                 bkg_err_fracs.append(self._fit_result_.params[par_name]['hesse']['error'])
 
         if len(signal_fracs) == len(bkg_fracs) == len(refl_fracs) == 0:
-            signal_fracs.append(1.)
-            signal_err_fracs.append(0.)
+            if len(self._background_pdf_) == 0:
+                signal_fracs.append(1.)
+                signal_err_fracs.append(0.)
+            elif len(self._signal_pdf_) == 0:
+                bkg_fracs.append(1.)
+                bkg_err_fracs.append(0.)
 
         return signal_fracs, bkg_fracs, refl_fracs, signal_err_fracs, bkg_err_fracs, refl_err_fracs
 
     def mass_zfit(self):
         """
         Perform a mass fit with the zfit library
 
@@ -829,15 +852,15 @@
         for bkg_pdf in self._background_pdf_:
             bkg_funcs.append(zfit.run(bkg_pdf.pdf(x_plot, norm_range=obs)))
 
         signal_fracs, bkg_fracs, refl_fracs, _, _, _ = self.__get_all_fracs()
 
         # first draw backgrounds
         for ibkg, bkg_func in enumerate(bkg_funcs):
-            if ibkg < len(bkg_fracs) - 1:
+            if ibkg < len(bkg_fracs) - 1 or len(signal_fracs) == 0:
                 plt.plot(x_plot, bkg_func * norm * bkg_fracs[ibkg], color=self._bkg_cmap_(ibkg),
                          ls='--', label=f'background {ibkg}')
             else:
                 plt.plot(x_plot, bkg_func * norm * (1-sum(bkg_fracs)-sum(signal_fracs)-sum(refl_fracs)),
                          color='firebrick', ls='--', label=f'background {ibkg}')
         # then draw signals
         for isgn, (signal_func, frac) in enumerate(zip(signal_funcs, signal_fracs)):
@@ -871,15 +894,15 @@
                                               frameon=False)
             # signal and background info for all signals
             text = []
             for idx, _ in enumerate(self._name_signal_pdf_):
                 mass, mass_unc = self.get_mass(idx)
                 sigma, sigma_unc = None, None
                 gamma, gamma_unc = None, None
-                if self._name_signal_pdf_[idx] in ['gaussian', 'crystalball', 'voigtian', 'hist']:
+                if self._name_signal_pdf_[idx] in ['gaussian', 'crystalball', 'doublecb', 'voigtian', 'hist']:
                     sigma, sigma_unc = self.get_sigma(idx)
                 if self._name_signal_pdf_[idx] in ['cauchy', 'voigtian']:
                     gamma, gamma_unc = self.get_signal_parameter(idx, 'gamma')
                 extra_info = fr'signal{idx}''\n' + fr'  $\mu = {mass*1000:.1f}\pm{mass_unc*1000:.1f}$ MeV$/c^2$''\n'
                 if sigma is not None:
                     extra_info += fr'  $\sigma = {sigma*1000:.1f}\pm{sigma_unc*1000:.1f}$ MeV$/c^2$''\n'
                 if gamma is not None:
@@ -1388,15 +1411,15 @@
         Returns
         -------------------------------------------------
         sigma: float
             The sigma value obtained from the fit
         sigma_err: float
             The sigma error obtained from the fit
         """
-        if self._name_signal_pdf_[idx] not in ['gaussian', 'crystalball', 'voigtian', 'hist']:
+        if self._name_signal_pdf_[idx] not in ['gaussian', 'crystalball', 'doublecb', 'voigtian', 'hist']:
             Logger(f'Sigma parameter not defined for {self._name_signal_pdf_[idx]} pdf!', 'ERROR')
             return 0., 0.
 
         # if histogram, the rms is used as proxy
         if 'hist' in self._name_signal_pdf_[idx]:
             Logger(f'RMS used as proxy for sigma parameter of {self._name_signal_pdf_[idx]} pdf!', 'WARNING')
             mean = self.get_mass(idx)[0]
@@ -1567,15 +1590,15 @@
                 return 0., 0.
             mass, _ = self.get_mass(idx)
             hwhm, _ = self.get_hwhm(idx)
             min_value = mass - nhwhm * hwhm
             max_value = mass + nhwhm * hwhm
 
         if use_nsigma:
-            if self._name_signal_pdf_[idx] not in ['gaussian', 'crystalball', 'hist']:
+            if self._name_signal_pdf_[idx] not in ['gaussian', 'crystalball', 'doublecb', 'voigtian', 'hist']:
                 Logger('Sigma not defined, I cannot compute the signal for this pdf', 'ERROR')
                 return 0., 0.
             mass, _ = self.get_mass(idx)
             sigma, _ = self.get_sigma(idx)
             min_value = mass - nsigma * sigma
             max_value = mass + nsigma * sigma
 
@@ -1660,15 +1683,15 @@
                 return 0., 0.
             mass, _ = self.get_mass(idx)
             hwhm, _ = self.get_hwhm(idx)
             min_value = mass - nhwhm * hwhm
             max_value = mass + nhwhm * hwhm
 
         if use_nsigma:
-            if self._name_signal_pdf_[idx] not in ['gaussian', 'crystalball', 'hist']:
+            if self._name_signal_pdf_[idx] not in ['gaussian', 'crystalball', 'doublecb', 'voigtian', 'hist']:
                 Logger('Sigma not defined, I cannot compute the signal for this pdf', 'ERROR')
                 return 0., 0.
             mass, _ = self.get_mass(idx)
             sigma, _ = self.get_sigma(idx)
             min_value = mass - nsigma * sigma
             max_value = mass + nsigma * sigma
```

### Comparing `flarefly-0.0.8/flarefly/utils.py` & `flarefly-0.0.9/flarefly/utils.py`

 * *Files identical despite different names*

### Comparing `flarefly-0.0.8/flarefly.egg-info/PKG-INFO` & `flarefly-0.0.9/flarefly.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: flarefly
-Version: 0.0.8
+Version: 0.0.9
 Summary: FLexible And REliable Fitting LibrarY for particle physics analysis
 Home-page: https://github.com/flarefly/flarefly
 Author: flarefly-developers
 Author-email: flarefly@googlegroups.com
 License: GPL
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <img src="./flarefly_logo.png" width="200" /> <sub><sup>Logo by Andrea Sofia Triolo</sup></sub>
 
@@ -54,8 +54,7 @@
 
 
 | Type | Link |
 
 | -------------- | ------------- |
 
 | Binned invariant mass fit |  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/flarefly/flarefly/blob/main/tutorials/flarefly_tutorial_Bzero.ipynb) |
-
```

### Comparing `flarefly-0.0.8/setup.py` & `flarefly-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         setup(**self.conf)
 
 
 SETUP = Setup(
     name="flarefly",
 
     # LAST-TAG is a placeholder. Automatically replaced at deploy time with the right tag
-    version="0.0.8",
+    version="0.0.9",
     description="FLexible And REliable Fitting LibrarY for particle physics analysis",
     url="https://github.com/flarefly/flarefly",
     author="flarefly-developers",
     author_email="flarefly@googlegroups.com",
     license="GPL",
 
     # See https://pypi.org/classifiers/
@@ -68,30 +68,31 @@
         "Development Status :: 3 - Alpha", "Intended Audience :: Education",
         "Intended Audience :: Developers",
         "Topic :: Scientific/Engineering :: Physics",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10"
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11"
     ],
 
     # What does your project relate to?
     keywords="",
 
     # You can just specify the packages manually here if your project is simple. Or you can use
     # find_packages().
     packages=find_packages(exclude=['tutorials']),
 
     # List run-time dependencies here. These will be installed by pip when your project is
     # installed. For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
     install_requires=[
         "psutil", "dutil", "prophet>=1.0.1", "numpy>=1.20", "pandas>=1.1.5", "uproot>=4.3.4",
-        "ipython>=7.16.1", "jedi==0.17.2", "zfit>=0.12.1", "mplhep>=0.3.25", "matplotlib>=3.1.3",
+        "ipython>=7.16.1", "jedi==0.17.2", "zfit>=0.14.0", "mplhep>=0.3.25", "matplotlib>=3.1.3",
         "particle>=0.20.1", "scipy>=1.7.3"
     ],
     python_requires=">=3.8",
 
     # List additional groups of dependencies here (e.g. development dependencies). You can install
     # these using the following syntax, for example:
     # $ pip install -e .[dev,test]
```

