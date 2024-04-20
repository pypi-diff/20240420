# Comparing `tmp/owlspec-0.1.tar.gz` & `tmp/owlspec-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owlspec-0.1.tar", last modified: Sun Apr 14 04:54:10 2024, max compression
+gzip compressed data, was "owlspec-0.2.tar", last modified: Sat Apr 20 17:28:00 2024, max compression
```

## Comparing `owlspec-0.1.tar` & `owlspec-0.2.tar`

### file list

```diff
@@ -1,44 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 04:54:10.936784 owlspec-0.1/
--rw-rw-rw-   0        0        0     1282 2024-04-14 04:54:10.936784 owlspec-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      803 2023-11-24 22:56:05.000000 owlspec-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 04:54:10.846856 owlspec-0.1/owlspec/
--rw-rw-rw-   0        0        0      340 2023-11-24 23:31:14.000000 owlspec-0.1/owlspec/__init__.py
--rw-rw-rw-   0        0        0     5716 2023-11-24 20:35:28.000000 owlspec-0.1/owlspec/emission_line.py
-drwxrwxrwx   0        0        0        0 2024-04-14 04:54:10.876885 owlspec-0.1/owlspec/emitter/
--rw-rw-rw-   0        0        0       65 2023-04-21 00:56:27.000000 owlspec-0.1/owlspec/emitter/__init__.py
--rw-rw-rw-   0        0        0     5554 2024-04-14 04:31:20.000000 owlspec-0.1/owlspec/emitter/level.py
--rw-rw-rw-   0        0        0     4339 2024-01-26 22:36:44.000000 owlspec-0.1/owlspec/emitter/transition.py
-drwxrwxrwx   0        0        0        0 2024-04-14 04:54:10.905573 owlspec-0.1/owlspec/nist_levels/
--rw-rw-rw-   0        0        0      698 2024-02-23 16:37:17.000000 owlspec-0.1/owlspec/nist_levels/__init__.py
--rw-rw-rw-   0        0        0     5241 2024-04-14 03:57:55.000000 owlspec-0.1/owlspec/nist_levels/core.py
-drwxrwxrwx   0        0        0        0 2024-04-14 04:54:10.927077 owlspec-0.1/owlspec/nist_levels/tests/
--rw-rw-rw-   0        0        0        0 2024-02-23 16:37:17.000000 owlspec-0.1/owlspec/nist_levels/tests/__init__.py
--rw-rw-rw-   0        0        0      210 2024-02-23 16:37:17.000000 owlspec-0.1/owlspec/nist_levels/tests/setup_package.py
--rw-rw-rw-   0        0        0     1956 2024-02-23 16:37:17.000000 owlspec-0.1/owlspec/nist_levels/tests/test_nist.py
--rw-rw-rw-   0        0        0     1086 2024-02-23 16:37:17.000000 owlspec-0.1/owlspec/nist_levels/tests/test_nist_remote.py
-drwxrwxrwx   0        0        0        0 2024-04-14 04:54:10.933778 owlspec-0.1/owlspec/spectrometer/
--rw-rw-rw-   0        0        0      125 2022-09-14 15:32:26.000000 owlspec-0.1/owlspec/spectrometer/__init__.py
--rw-rw-rw-   0        0        0      794 2022-05-12 14:02:58.000000 owlspec-0.1/owlspec/spectrometer/avantes.py
--rw-rw-rw-   0        0        0      899 2022-05-12 14:02:58.000000 owlspec-0.1/owlspec/spectrometer/basic.py
--rw-rw-rw-   0        0        0     2851 2022-10-04 20:20:06.000000 owlspec-0.1/owlspec/spectrometer/newport.py
--rw-rw-rw-   0        0        0     4573 2022-05-12 14:02:58.000000 owlspec-0.1/owlspec/spectrometer/pgs.py
--rw-rw-rw-   0        0        0     1912 2022-05-12 14:02:58.000000 owlspec-0.1/owlspec/spectrometer/triax.py
--rw-rw-rw-   0        0        0    10597 2024-04-14 04:30:56.000000 owlspec-0.1/owlspec/spectrum.py
-drwxrwxrwx   0        0        0        0 2024-04-14 04:54:10.936784 owlspec-0.1/owlspec/stark/
--rw-rw-rw-   0        0        0       39 2022-05-12 14:02:58.000000 owlspec-0.1/owlspec/stark/__init__.py
--rw-rw-rw-   0        0        0     8133 2023-11-24 23:39:14.000000 owlspec-0.1/owlspec/stark/gigosos_he_loader.py
--rw-rw-rw-   0        0        0     7066 2023-11-24 23:40:20.000000 owlspec-0.1/owlspec/stark/gigosos_loader.py
--rw-rw-rw-   0        0        0     2779 2023-04-21 01:39:19.000000 owlspec-0.1/owlspec/stark/griem.py
--rw-rw-rw-   0        0        0     3386 2023-11-24 21:43:57.000000 owlspec-0.1/owlspec/stark/stark.py
--rw-rw-rw-   0        0        0     6399 2024-01-26 23:28:12.000000 owlspec-0.1/owlspec/util.py
-drwxrwxrwx   0        0        0        0 2024-04-14 04:54:10.936784 owlspec-0.1/owlspec/vdW/
--rw-rw-rw-   0        0        0       37 2022-05-12 14:06:55.000000 owlspec-0.1/owlspec/vdW/__init__.py
--rw-rw-rw-   0        0        0     4559 2023-04-21 01:54:23.000000 owlspec-0.1/owlspec/vdW/vdW.py
-drwxrwxrwx   0        0        0        0 2024-04-14 04:54:10.870370 owlspec-0.1/owlspec.egg-info/
--rw-rw-rw-   0        0        0     1282 2024-04-14 04:54:10.000000 owlspec-0.1/owlspec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      929 2024-04-14 04:54:10.000000 owlspec-0.1/owlspec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 04:54:10.000000 owlspec-0.1/owlspec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2024-04-14 04:54:10.000000 owlspec-0.1/owlspec.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-14 04:54:10.000000 owlspec-0.1/owlspec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 04:54:10.936784 owlspec-0.1/setup.cfg
--rw-rw-rw-   0        0        0      893 2024-04-14 04:34:25.000000 owlspec-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 17:28:00.284655 owlspec-0.2/
+-rw-rw-rw-   0        0        0     1089 2024-04-20 00:47:16.000000 owlspec-0.2/LICENSE
+-rw-rw-rw-   0        0        0    15738 2024-04-20 17:28:00.283655 owlspec-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    15236 2024-04-20 17:21:16.000000 owlspec-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 17:28:00.226955 owlspec-0.2/owlspec/
+-rw-rw-rw-   0        0        0      313 2024-04-20 15:14:45.000000 owlspec-0.2/owlspec/__init__.py
+-rw-rw-rw-   0        0        0     8238 2024-04-20 15:19:49.000000 owlspec-0.2/owlspec/emission_line.py
+drwxrwxrwx   0        0        0        0 2024-04-20 17:28:00.271613 owlspec-0.2/owlspec/emitter/
+-rw-rw-rw-   0        0        0       65 2024-04-20 15:11:09.000000 owlspec-0.2/owlspec/emitter/__init__.py
+-rw-rw-rw-   0        0        0     5561 2024-04-20 15:14:23.000000 owlspec-0.2/owlspec/emitter/level.py
+-rw-rw-rw-   0        0        0     4328 2024-04-20 15:14:19.000000 owlspec-0.2/owlspec/emitter/transition.py
+drwxrwxrwx   0        0        0        0 2024-04-20 17:28:00.273654 owlspec-0.2/owlspec/nist_levels/
+-rw-rw-rw-   0        0        0      694 2024-04-20 00:47:16.000000 owlspec-0.2/owlspec/nist_levels/__init__.py
+-rw-rw-rw-   0        0        0     5230 2024-04-20 00:47:16.000000 owlspec-0.2/owlspec/nist_levels/core.py
+-rw-rw-rw-   0        0        0    10043 2024-04-20 15:11:11.000000 owlspec-0.2/owlspec/spectrum.py
+drwxrwxrwx   0        0        0        0 2024-04-20 17:28:00.280658 owlspec-0.2/owlspec/stark/
+-rw-rw-rw-   0        0        0       39 2022-05-12 14:02:58.000000 owlspec-0.2/owlspec/stark/__init__.py
+-rw-rw-rw-   0        0        0     8133 2023-11-24 23:39:14.000000 owlspec-0.2/owlspec/stark/gigosos_he_loader.py
+-rw-rw-rw-   0        0        0     7066 2023-11-24 23:40:20.000000 owlspec-0.2/owlspec/stark/gigosos_loader.py
+-rw-rw-rw-   0        0        0     3105 2024-04-20 00:47:16.000000 owlspec-0.2/owlspec/stark/griem.py
+-rw-rw-rw-   0        0        0     3386 2023-11-24 21:43:57.000000 owlspec-0.2/owlspec/stark/stark.py
+-rw-rw-rw-   0        0        0     6606 2024-04-20 15:11:07.000000 owlspec-0.2/owlspec/util.py
+drwxrwxrwx   0        0        0        0 2024-04-20 17:28:00.281655 owlspec-0.2/owlspec/vdW/
+-rw-rw-rw-   0        0        0       37 2022-05-12 14:06:55.000000 owlspec-0.2/owlspec/vdW/__init__.py
+-rw-rw-rw-   0        0        0     4518 2024-04-20 15:11:10.000000 owlspec-0.2/owlspec/vdW/vdW.py
+drwxrwxrwx   0        0        0        0 2024-04-20 17:28:00.268668 owlspec-0.2/owlspec.egg-info/
+-rw-rw-rw-   0        0        0    15738 2024-04-20 17:28:00.000000 owlspec-0.2/owlspec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      586 2024-04-20 17:28:00.000000 owlspec-0.2/owlspec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 17:28:00.000000 owlspec-0.2/owlspec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2024-04-20 17:28:00.000000 owlspec-0.2/owlspec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-20 17:28:00.000000 owlspec-0.2/owlspec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 17:28:00.284655 owlspec-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      893 2024-04-20 17:22:51.000000 owlspec-0.2/setup.py
```

### Comparing `owlspec-0.1/owlspec/emitter/level.py` & `owlspec-0.2/owlspec/emitter/level.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         except:
             self.l = np.nan
         
         self.g = float(nist_levels[level_idx]['g']) # statistical weight
         self.conf = row['Configuration'] # configuration and term string
         
         if 'Landé' in nist_levels.keys():
-            self.G = nist_levels[level_idx]['Landé'] #Lande g factor
+            self.G = float(nist_levels[level_idx]['Landé']) #Lande g factor
         else:
             self.G = None
         
 
 
     def l_name_to_num(self, name):
         chars = ["s","p","d","f","g","h","i","j"]
```

### Comparing `owlspec-0.1/owlspec/emitter/transition.py` & `owlspec-0.2/owlspec/emitter/transition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #!/usr/bin/python
 
-import os
 import numpy as np
 import re
 from ..util import parse_spectroscopic_name, get_spectroscopic_name
 from .level import level
 import mendeleev 
 from astroquery.nist import Nist
 import astropy.units as u
```

### Comparing `owlspec-0.1/owlspec/nist_levels/__init__.py` & `owlspec-0.2/owlspec/nist_levels/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Licensed under a 3-clause BSD style license - see LICENSE.rst
+# Licensed under a 3-clause BSD style license - see LICENSE
 """
 Fetches level information from the NIST Atomic Spectra Database.
 """
 from astropy import config as _config
 
 
 class Conf(_config.ConfigNamespace):
```

### Comparing `owlspec-0.1/owlspec/nist_levels/core.py` & `owlspec-0.2/owlspec/nist_levels/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-# Licensed under a 3-clause BSD style license - see LICENSE.rst
+# Licensed under a 3-clause BSD style license - see LICENSE
 
 
 import html
 import re
 
-import astropy.io.ascii as asciitable
+# import astropy.io.ascii as asciitable
+from astropy.table import Table
 
 from astroquery.query import BaseQuery
 from astroquery.utils import async_to_sync, prepend_docstr_nosections
 from . import conf
 from astroquery.exceptions import TableParseError
 
 __all__ = ['NistLevels', 'NistLevelsClass']
@@ -133,16 +134,16 @@
             pre = pre_re.findall(content)[0]
         except IndexError:
             raise Exception("Result did not contain a table")
         try:
             table = _strip_blanks(pre)
             table = links_re.sub(r'\1', table)
             table = html.unescape(table)
-            table = asciitable.read(table, Reader=asciitable.FixedWidth,
-                                    data_start=1, delimiter='|')
+            table = Table.read(table, format='ascii.fixed_width', data_start=1, delimiter='|')
+
             return table
         except Exception as ex:
             self.response = response
             self.table_parse_error = ex
             raise TableParseError("Failed to parse asciitable! The raw "
                                   "response can be found in self.response, "
                                   "and the error in self.table_parse_error.")
```

### Comparing `owlspec-0.1/owlspec/spectrum.py` & `owlspec-0.2/owlspec/spectrum.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,113 +1,88 @@
 #!/bin/python3
 import numpy as np
-from scipy import constants as const
 from .util import *
-import os
-from .emitter import transition
 import mendeleev 
 from astroquery.nist import Nist
-from .nist_levels import NistLevels
 import astropy.units as u
 import re
 import warnings
 
 
 class spectrum():
-    """ Holds information about a complete emission spectrum of the given
-    particles in the wavelength range defined by <wl_range> or the
-    owl.spectrometer object.
-
-    particles: list of owl.emitter.particle objects
-    spectrometer: owl.spectrometer object
-    wl_range: tuple or list of lower and upper wavelength of the spectrum"""
+    """ Calculates complete or partial emission spectra for the emitter 
+    specified by <emitter name> inr the wavelength range defined by 
+    <wl_range>.
+
+    <emitter_name>: Name of the emitting species in spectroscopic notation,
+    e.g. "Ar I" for argon neutrals or Fe IV for tripply charged iron.
+    <wl_range>: Tuple of lower and upper wavelength of the spectrum."""
 
-    def __init__(self, emitter_name, spectrometer=None, wl_range=None):
+    def __init__(self, emitter_name, wl_range=None):
         self.name, self.charge = parse_spectroscopic_name(emitter_name)
         self.spec_name = get_spectroscopic_name(self.name, self.charge)
         self.emitter = self.particle = mendeleev.element(self.name)
         self.emitter.charge = self.charge
         self.emitter.m = self.emitter.mass
         self.emitter.Ei = self.emitter.ionenergies[1]
         self.charge = self.emitter.charge
         
-        self.spectrometer = spectrometer
         self.wl_range = wl_range
         self.linedata = None
-        if spectrometer and not wl_range:
-            if spectrometer.x is not None:
-                self.wl_range = (spectrometer.x[0],spectrometer.x[-1])
-
 
 
     def get_linedata(self):
         if self.wl_range is not None:
             wl_low = self.wl_range[0]
             wl_high = self.wl_range[-1]
         else:
             wl_low = 0
             wl_high = 9999
             
         nist_lines = Nist.query(wl_low*u.nm, wl_high*u.nm, 
-                                linename=self.spec_name, wavelength_type='vac+air')
+                            linename=self.spec_name, wavelength_type='vac+air')
 
         return nist_lines
 
 
-    def get_spectrum(self,x=None, width=0.02, mu=0.2, min_int=-1, min_Aik=-1):
+    def get_spectrum(self, x, width=0.02, mu=0.2, min_int=-1, min_Aik=-1):
         """ Return simulated spectrum. Lines are pseudo Voigt with
         the set width (FWHM) in nm and form parameter mu (0 = Gauss)  """
-        try:
-            if not x:
-                x = self.spectrometer.x
-        except:
-            x = x
-            
         nist_lines = self.get_linedata()
         spectrum = self.table_to_spec_rel(x, nist_lines, width, mu, min_int, min_Aik)
-
         return spectrum
 
 
     def get_LTE_spectrum(self, x, Te, width=0.02, mu=0.2, norm=False, min_int=-1, min_Aik=-1):
         """ Return simulated spectrum with LTE line intnsities in units 
         proportional (!) to Photons/s (NOT W/cm²s)
         Lines are pseudo Voigt with the set width (FWHM) in nm and form 
         parameter mu (0 = Gauss).
         Set norm=True to normalize the intensity to 1 for easier fitting.
         """
-        try:
-            if not x:
-                x = self.spectrometer.x
-        except:
-            x = x
         nist_lines = self.get_linedata()
         spectrum = self.table_to_spec_LTE(x, nist_lines, Te, width, mu, min_int, min_Aik)
         if norm == True:
             spectrum = spectrum/np.max(spectrum)
         return spectrum
         
         
     def get_ident_spectrum(self, min_int=-1, min_Aik=-1):
         """ Return simulated spectrum. Marks the wavelenght position
         with thin lines. """
-            
         nist_lines = self.get_linedata()
         x, y = self.table_to_ident(nist_lines, min_int, min_Aik)
-        
         return x,y
 
 
     def get_ident_spectrum_LTE(self, Te, min_int=-1, min_Aik=-1):
         """ Return simulated spectrum. Marks the wavelenght position
-        with thin lines. """
-            
+        with thin lines. """   
         nist_lines = self.get_linedata()
         x, y = self.table_to_ident_LTE(nist_lines, Te, min_int, min_Aik)
-        
         return x,y
         
 
     def table_to_spec_LTE(self, x, nist_lines, Te, width=0.1, mu=0.5, min_int=-1, min_Aik=-1):
         spectrum = np.zeros(len(x))
         for line in  nist_lines:   
             c1 = str(line['Observed'])
@@ -173,15 +148,16 @@
                             Aik =  float(line['Aki'])
                     else:
                         Aik = 1
                         
                     if rel_int > min_int and Aik > min_Aik:
                         profile = rel_int*psd_voigt_function(x, wl, width, mu)
                         spectrum = spectrum + profile
-                except:
+                except Exception as err:
+                    print(err)
                     pass
                 
         return spectrum
 
         
     def table_to_ident(self, nist_lines, min_int=-1, min_Aik=-1):
         x = []
```

### Comparing `owlspec-0.1/owlspec/stark/gigosos_he_loader.py` & `owlspec-0.2/owlspec/stark/gigosos_he_loader.py`

 * *Files identical despite different names*

### Comparing `owlspec-0.1/owlspec/stark/gigosos_loader.py` & `owlspec-0.2/owlspec/stark/gigosos_loader.py`

 * *Files identical despite different names*

### Comparing `owlspec-0.1/owlspec/stark/griem.py` & `owlspec-0.2/owlspec/stark/griem.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,100 +1,104 @@
-#!/usr/bin/python3
-
-import numpy as np
-from scipy import constants as const
-from ..util import *
-import os
-
-class griem():
-    def __init__(self, transition):
-        self.transition = transition
-
-    def get_width_shift(self, ne, Te):
-        ele = self.transition.emitter.symbol
-        wl = self.transition.wl
-
-        if ele == "O" and round(wl, 0) == 777.:
-            A,B,we,de = self.params_O777(Te)
-
-        if ele == "Ar" and (round(wl, 3) == 810.369 or round(wl, 3) == 738.398):
-            A,B,we,de = self.params_Ar8104(Te)
-
-        w = self.width(ne,Te,A,we)
-        d = self.shift(ne,Te,A,we,de)
-
-        return w,d
-
-
-    def width(self,ne,Te,A,we):
-        """ Te in eV, ne in m^-3
-        we, de in Angstrom @ 1e22/m^3 density
-        Returns w in nm
-        """
-
-        # we need Te in K
-        T = Te * const.eV / const.k
-        # we need ne in cm^-3
-        n = ne * 1e-6
-
-        w = 2 * we * n * 1e-16 * (1 +
-            1.75 * 1e-4 * n**(1/4) * A * (1 - 0.068*n**(1/6) * T**(-1/2) ) )
-
-        # w is Angstrom
-        w = w/10
-        return w
-
-
-    def shift(self,ne,Te,A,we,de):
-        """ Te in eV, ne in m^-3
-        we, de in Angstrom @ 1e22/m^3 density """
-
-        # we need Te in K
-        T = Te * const.eV / const.k
-        # we need ne in cm^-3
-        n = ne * 1e-6
-
-        d = n*1e-16 * (de + 2e-4 * n**(1/4) * A * we * (1-0.068 * n**(1/6) * T**(-1/2)))
-
-        # d is Angstrom
-        d = d/10
-        return d
-
-
-    def params_O777(self,Te):
-        """ Parameters fitted from:
-         H.R. Griem: Spectral Line Broadening by Plasmas
-         returns A,B and we,de in Angstrom
-         All values at ne = 10^16 /cm^3
-         """
-
-        # we need Te in K
-        T = Te * const.eV / const.k
-
-        B = 0.00023718 * T # recommended by Griem
-        A = 0.27661461 * T**(-0.33635335) # Just fits okay.
-        we = 4.36767799e-04 * T**(0.465538767) # Fitted; in Angstrom
-
-        a0,a1,a2,a3,a4 = [1.39308003e-02,1.88771484e-07,-2.17304732e-11,
-        6.29115391e-16,-6.33972112e-21] # very much overdefined...
-        de = a0 + a1*T + a2*T**2 + a3*T**3 + a4*T**4
-
-        return A,B,we,de
-
-
-    def params_Ar8104(self,Te):
-        """ Parameters fitted from:
-         H.R. Griem: Spectral Line Broadening by Plasmas
-         returns A,B and we,de in Angstrom
-         All values at ne = 10^16 /cm^3
-         """
-
-        # we need Te in K
-        T = Te * const.eV / const.k
-
-        B = 5.25e-5 * T # recommended by Griem
-        A = 0.3248611802364256 * T**(-0.2795132945865003) # Just fits okay.
-        we = -0.001503172622523098 + 0.002098004523296234 * T**0.358775514451271
-        a0,a1,a2,a3 = [0.056, -6.4e-07, 4e-12, -48] # very much overdefined...
-        de =  a0 + a1*T + a2*T**2 +  a3*T**-1
-
-        return A,B,we,de
+#!/usr/bin/python3
+
+import numpy as np
+from scipy import constants as const
+from ..util import *
+import os
+
+class griem():
+    def __init__(self, transition):
+        self.transition = transition
+
+    def get_width_shift(self, ne, Te):
+        ele = self.transition.emitter.symbol
+        wl = self.transition.wl
+
+        if ele == "O" and round(wl, 0) == 777.:
+            A,B,we,de = self.params_O777(Te)
+            w = self.width(ne,Te,A,we)
+            d = self.shift(ne,Te,A,we,de)
+        if ele == "Ar" and (round(wl, 3) == 810.369 or round(wl, 3) == 738.398):
+            A,B,we,de = self.params_Ar8104(Te)
+            w = self.width(ne,Te,A,we)
+            d = self.shift(ne,Te,A,we,de)
+        else:
+            w = 1e-12
+            d = 1e-12
+            print("Stark broadening not implemented for this line.")
+        
+        return w,d
+
+
+    def width(self,ne,Te,A,we):
+        """ Te in eV, ne in m^-3
+        we, de in Angstrom @ 1e22/m^3 density
+        Returns w in nm
+        """
+
+        # we need Te in K
+        T = Te * const.eV / const.k
+        # we need ne in cm^-3
+        n = ne * 1e-6
+
+        w = 2 * we * n * 1e-16 * (1 +
+            1.75 * 1e-4 * n**(1/4) * A * (1 - 0.068*n**(1/6) * T**(-1/2) ) )
+
+        # w is Angstrom
+        w = w/10
+        return w
+
+
+    def shift(self,ne,Te,A,we,de):
+        """ Te in eV, ne in m^-3
+        we, de in Angstrom @ 1e22/m^3 density """
+
+        # we need Te in K
+        T = Te * const.eV / const.k
+        # we need ne in cm^-3
+        n = ne * 1e-6
+
+        d = n*1e-16 * (de + 2e-4 * n**(1/4) * A * we * (1-0.068 * n**(1/6) * T**(-1/2)))
+
+        # d is Angstrom
+        d = d/10
+        return d
+
+
+    def params_O777(self,Te):
+        """ Parameters fitted from:
+         H.R. Griem: Spectral Line Broadening by Plasmas
+         returns A,B and we,de in Angstrom
+         All values at ne = 10^16 /cm^3
+         """
+
+        # we need Te in K
+        T = Te * const.eV / const.k
+
+        B = 0.00023718 * T # recommended by Griem
+        A = 0.27661461 * T**(-0.33635335) # Just fits okay.
+        we = 4.36767799e-04 * T**(0.465538767) # Fitted; in Angstrom
+
+        a0,a1,a2,a3,a4 = [1.39308003e-02,1.88771484e-07,-2.17304732e-11,
+        6.29115391e-16,-6.33972112e-21] # very much overdefined...
+        de = a0 + a1*T + a2*T**2 + a3*T**3 + a4*T**4
+
+        return A,B,we,de
+
+
+    def params_Ar8104(self,Te):
+        """ Parameters fitted from:
+         H.R. Griem: Spectral Line Broadening by Plasmas
+         returns A,B and we,de in Angstrom
+         All values at ne = 10^16 /cm^3
+         """
+
+        # we need Te in K
+        T = Te * const.eV / const.k
+
+        B = 5.25e-5 * T # recommended by Griem
+        A = 0.3248611802364256 * T**(-0.2795132945865003) # Just fits okay.
+        we = -0.001503172622523098 + 0.002098004523296234 * T**0.358775514451271
+        a0,a1,a2,a3 = [0.056, -6.4e-07, 4e-12, -48] # very much overdefined...
+        de =  a0 + a1*T + a2*T**2 +  a3*T**-1
+
+        return A,B,we,de
```

### Comparing `owlspec-0.1/owlspec/stark/stark.py` & `owlspec-0.2/owlspec/stark/stark.py`

 * *Files identical despite different names*

### Comparing `owlspec-0.1/owlspec/vdW/vdW.py` & `owlspec-0.2/owlspec/vdW/vdW.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 #!/usr/bin/python
 
 import numpy as np
 from ..util import *
-from .. import emitter
-import mendeleev 
 from scipy import constants as const
 
 class vdW():
     def __init__(self, transition, pert):
         self.transition = transition
         self.pert = pert
```

### Comparing `owlspec-0.1/setup.py` & `owlspec-0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="owlspec",
-    version="0.1",
+    version="0.2",
     author="Julian Held",
     author_email="julian.held@umn.edu",
     license='MIT',
     platforms=['any'],
     description="Library for optical emission spectroscopy of low-temperature plasmas.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

