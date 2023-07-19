# Comparing `tmp/gascompressibility-0.1.7.tar.gz` & `tmp/gascompressibility-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gascompressibility-0.1.7.tar", last modified: Thu Jul  6 19:14:11 2023, max compression
+gzip compressed data, was "gascompressibility-1.0.0.tar", last modified: Wed Jul 19 07:03:49 2023, max compression
```

## Comparing `gascompressibility-0.1.7.tar` & `gascompressibility-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 19:14:11.251023 gascompressibility-0.1.7/
--rw-rw-rw-   0        0        0     1095 2023-05-23 14:19:22.000000 gascompressibility-0.1.7/LICENSE
--rw-rw-rw-   0        0        0    11101 2023-07-06 19:14:11.251023 gascompressibility-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0    10123 2023-07-06 14:22:50.000000 gascompressibility-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 19:14:11.226741 gascompressibility-0.1.7/gascompressibility/
--rw-rw-rw-   0        0        0      275 2023-07-06 19:01:31.000000 gascompressibility-0.1.7/gascompressibility/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 19:14:11.240742 gascompressibility-0.1.7/gascompressibility/pseudocritical/
--rw-rw-rw-   0        0        0    17335 2023-06-29 17:48:34.000000 gascompressibility-0.1.7/gascompressibility/pseudocritical/Piper.py
--rw-rw-rw-   0        0        0    20224 2023-06-29 17:48:34.000000 gascompressibility-0.1.7/gascompressibility/pseudocritical/Sutton.py
--rw-rw-rw-   0        0        0       56 2023-06-29 18:25:42.000000 gascompressibility-0.1.7/gascompressibility/pseudocritical/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 19:14:11.242741 gascompressibility-0.1.7/gascompressibility/utilities/
--rw-rw-rw-   0        0        0        0 2023-05-31 21:10:39.000000 gascompressibility-0.1.7/gascompressibility/utilities/__init__.py
--rw-rw-rw-   0        0        0      317 2023-06-17 04:32:50.000000 gascompressibility-0.1.7/gascompressibility/utilities/utilities.py
-drwxrwxrwx   0        0        0        0 2023-07-06 19:14:11.248022 gascompressibility-0.1.7/gascompressibility/z_correlation/
--rw-rw-rw-   0        0        0     1088 2023-06-11 02:01:39.000000 gascompressibility-0.1.7/gascompressibility/z_correlation/DAK.py
--rw-rw-rw-   0        0        0        0 2023-06-26 15:16:19.000000 gascompressibility-0.1.7/gascompressibility/z_correlation/__init__.py
--rw-rw-rw-   0        0        0      746 2023-06-11 02:05:15.000000 gascompressibility-0.1.7/gascompressibility/z_correlation/hall_yarborough.py
--rw-rw-rw-   0        0        0     2097 2023-06-18 06:10:02.000000 gascompressibility-0.1.7/gascompressibility/z_correlation/kareem.py
--rw-rw-rw-   0        0        0     1195 2023-06-11 03:43:15.000000 gascompressibility-0.1.7/gascompressibility/z_correlation/londono.py
--rw-rw-rw-   0        0        0     8846 2023-07-06 19:01:44.000000 gascompressibility-0.1.7/gascompressibility/z_correlation/z_helper.py
-drwxrwxrwx   0        0        0        0 2023-07-06 19:14:11.237741 gascompressibility-0.1.7/gascompressibility.egg-info/
--rw-rw-rw-   0        0        0    11101 2023-07-06 19:14:11.000000 gascompressibility-0.1.7/gascompressibility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      878 2023-07-06 19:14:11.000000 gascompressibility-0.1.7/gascompressibility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 19:14:11.000000 gascompressibility-0.1.7/gascompressibility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-06 19:14:11.000000 gascompressibility-0.1.7/gascompressibility.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-07-06 19:14:11.000000 gascompressibility-0.1.7/gascompressibility.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 19:14:11.251023 gascompressibility-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1522 2023-07-06 19:03:50.000000 gascompressibility-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 19:14:11.250023 gascompressibility-0.1.7/tests/
--rw-rw-rw-   0        0        0      137 2023-06-10 01:30:30.000000 gascompressibility-0.1.7/tests/__init__.py
--rw-rw-rw-   0        0        0    30936 2023-06-28 22:59:10.000000 gascompressibility-0.1.7/tests/test_gascomp.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:03:49.955025 gascompressibility-1.0.0/
+-rw-rw-rw-   0        0        0     1095 2023-05-23 14:19:22.000000 gascompressibility-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0    16990 2023-07-19 07:03:49.952035 gascompressibility-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    16011 2023-07-19 06:57:17.000000 gascompressibility-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 07:03:49.920142 gascompressibility-1.0.0/gascompressibility/
+-rw-rw-rw-   0        0        0      275 2023-07-19 03:28:35.000000 gascompressibility-1.0.0/gascompressibility/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:03:49.941071 gascompressibility-1.0.0/gascompressibility/pseudocritical/
+-rw-rw-rw-   0        0        0    17621 2023-07-19 03:28:35.000000 gascompressibility-1.0.0/gascompressibility/pseudocritical/Piper.py
+-rw-rw-rw-   0        0        0    20416 2023-07-19 03:28:35.000000 gascompressibility-1.0.0/gascompressibility/pseudocritical/Sutton.py
+-rw-rw-rw-   0        0        0       56 2023-07-19 03:28:35.000000 gascompressibility-1.0.0/gascompressibility/pseudocritical/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:03:49.943065 gascompressibility-1.0.0/gascompressibility/utilities/
+-rw-rw-rw-   0        0        0        0 2023-07-19 03:28:35.000000 gascompressibility-1.0.0/gascompressibility/utilities/__init__.py
+-rw-rw-rw-   0        0        0      317 2023-07-19 03:28:35.000000 gascompressibility-1.0.0/gascompressibility/utilities/utilities.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:03:49.949045 gascompressibility-1.0.0/gascompressibility/z_correlation/
+-rw-rw-rw-   0        0        0     1088 2023-07-19 03:28:35.000000 gascompressibility-1.0.0/gascompressibility/z_correlation/DAK.py
+-rw-rw-rw-   0        0        0        0 2023-07-19 03:28:35.000000 gascompressibility-1.0.0/gascompressibility/z_correlation/__init__.py
+-rw-rw-rw-   0        0        0      723 2023-07-19 03:28:35.000000 gascompressibility-1.0.0/gascompressibility/z_correlation/hall_yarborough.py
+-rw-rw-rw-   0        0        0     2097 2023-07-19 03:28:35.000000 gascompressibility-1.0.0/gascompressibility/z_correlation/kareem.py
+-rw-rw-rw-   0        0        0     1195 2023-07-19 03:28:35.000000 gascompressibility-1.0.0/gascompressibility/z_correlation/londono.py
+-rw-rw-rw-   0        0        0    18940 2023-07-19 03:28:35.000000 gascompressibility-1.0.0/gascompressibility/z_correlation/z_helper.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:03:49.939078 gascompressibility-1.0.0/gascompressibility.egg-info/
+-rw-rw-rw-   0        0        0    16990 2023-07-19 07:03:49.000000 gascompressibility-1.0.0/gascompressibility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      878 2023-07-19 07:03:49.000000 gascompressibility-1.0.0/gascompressibility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 07:03:49.000000 gascompressibility-1.0.0/gascompressibility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-19 07:03:49.000000 gascompressibility-1.0.0/gascompressibility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-07-19 07:03:49.000000 gascompressibility-1.0.0/gascompressibility.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 07:03:49.955025 gascompressibility-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1522 2023-07-19 03:28:35.000000 gascompressibility-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:03:49.951038 gascompressibility-1.0.0/tests/
+-rw-rw-rw-   0        0        0      137 2023-07-19 03:28:35.000000 gascompressibility-1.0.0/tests/__init__.py
+-rw-rw-rw-   0        0        0    30936 2023-07-19 03:28:35.000000 gascompressibility-1.0.0/tests/test_gascomp.py
```

### Comparing `gascompressibility-0.1.7/LICENSE` & `gascompressibility-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.7/gascompressibility/pseudocritical/Piper.py` & `gascompressibility-1.0.0/gascompressibility/pseudocritical/Piper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import numpy as np
 import inspect
 
 from gascompressibility.utilities.utilities import calc_Fahrenheit_to_Rankine
 from gascompressibility.utilities.utilities import calc_psig_to_psia
 
-"""
-This is a Piper module
-"""
-
 
 class Piper(object):
     """
-    An example docstring for a class definition.
+    Class object to calculate pseudo-critical properties based on Piper's method.
+
+    The model uses Piper's model (1993) [1]_ to correlate specific gravity (:math:`\gamma_g`) to pseudo-critical pressure (:math:`P_{pc}`) and pseudo-critical
+    temperature (:math:`T_{pc}`). It supports corrections for acid gas fractions (:math:`H_2S`, :math:`CO_2`, and :math:`N2`)
     """
 
     def __init__(self):
 
         self.sg = None
         """specific gravity (dimensionless)"""
         self.T_f = None
```

### Comparing `gascompressibility-0.1.7/gascompressibility/pseudocritical/Sutton.py` & `gascompressibility-1.0.0/gascompressibility/pseudocritical/Sutton.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 from gascompressibility.utilities.utilities import calc_Fahrenheit_to_Rankine
 from gascompressibility.utilities.utilities import calc_psig_to_psia
 
 
 class Sutton():
 
     """
-    Class object to calculate pseudo-critical properties.
-
-    Based on Sutton's specific gravity correlation [1]_ and Wichert & Aziz correction for acid gases (:math:`H_2S` and :math:`CO_2`) [2]_.
+    Class object to calculate pseudo-critical properties based on Sutton's method.
 
+    The model uses Sutton's model (1985) [1]_ to correlate specific gravity (:math:`\gamma_g`) to pseudo-critical pressure (:math:`P_{pc}`) and pseudo-critical
+    temperature (:math:`T_{pc}`). It supports corrections for acid gas fractions (:math:`H_2S` and :math:`CO_2`) using
+    Wichert & Aziz method (1970) [2]_.
     """
 
     def __init__(self):
 
         self.sg = None
         """specific gravity (dimensionless)"""
         self.T_f = None
@@ -121,15 +122,15 @@
         self._initialize_sg(sg)
         self.Ppc = 756.8 - 131.07 * self.sg - 3.6 * self.sg ** 2
         self.ps_props['Ppc'] = self.Ppc
         return self.Ppc
 
     def calc_e_correction(self, H2S=None, CO2=None):
         """
-        Calculates the temperature-correction factor for acid gases, ε (°R)
+        Calculates temperature-correction factor for acid gases, ε (°R)
 
         Parameters
         ----------
         H2S : float
             mole fraction of H2S (dimensionless)
         CO2 : float
             mole fraction of CO2 (dimensionless)
@@ -144,15 +145,15 @@
         self._initialize_B(B=None, H2S=H2S)
         self.e_correction = 120 * (self.A ** 0.9 - self.A ** 1.6) + 15 * (self.B ** 0.5 - self.B ** 4)
         self.ps_props['e_correction'] = self.e_correction
         return self.e_correction
 
     def calc_Tpc_corrected(self, sg=None, Tpc=None, e_correction=None, H2S=None, CO2=None, ignore_conflict=False):
         """
-        Calculates the corrected pseudo-critical temperature, T'pc (°R)
+        Calculates corrected pseudo-critical temperature, T'pc (°R)
 
         Parameters
         ----------
         sg : float
             specific gravity of gas (dimensionless)
         Tpc : float
             pseudo-critical temperature, Tpc (°R)
@@ -183,15 +184,15 @@
         self._initialize_e_correction(e_correction, H2S=H2S, CO2=CO2, ignore_conflict=ignore_conflict)
         self.Tpc_corrected = self.Tpc - self.e_correction
         self.ps_props['Tpc_corrected'] = self.Tpc_corrected
         return self.Tpc_corrected
 
     def calc_Ppc_corrected(self, sg=None, Tpc=None, Ppc=None, e_correction=None, Tpc_corrected=None, H2S=None, CO2=None, ignore_conflict=False):
         """
-        Calculates the corrected pseudo-critical pressure, P'pc (psia)
+        Calculates corrected pseudo-critical pressure, P'pc (psia)
 
         Parameters
         ----------
         sg : float
             specific gravity of gas (dimensionless)
         Tpc : float
             pseudo-critical temperature, Tpc (°R)
```

### Comparing `gascompressibility-0.1.7/gascompressibility/z_correlation/DAK.py` & `gascompressibility-1.0.0/gascompressibility/z_correlation/DAK.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.7/gascompressibility/z_correlation/hall_yarborough.py` & `gascompressibility-1.0.0/gascompressibility/z_correlation/hall_yarborough.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,13 +12,11 @@
     t = 1 / Tr
 
     A1 = 0.06125 * t * np.exp(-1.2 * (1 - t) ** 2)
     A2 = 14.76 * t - 9.76 * t ** 2 + 4.58 * t ** 3
     A3 = 90.7 * t - 242.2 * t ** 2 + 42.4 * t ** 3
     A4 = 2.18 + 2.82 * t
 
-    ((A1 * Pr) / z)
-
     return -A1 * Pr \
         + (((A1 * Pr) / z) + ((A1 * Pr) / z) ** 2 + ((A1 * Pr) / z) ** 3 - ((A1 * Pr) / z) ** 4)/(1 - ((A1 * Pr) / z)) ** 3 \
         - A2 * ((A1 * Pr) / z) ** 2 + A3 * ((A1 * Pr) / z) ** A4
```

### Comparing `gascompressibility-0.1.7/gascompressibility/z_correlation/kareem.py` & `gascompressibility-1.0.0/gascompressibility/z_correlation/kareem.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.7/gascompressibility/z_correlation/londono.py` & `gascompressibility-1.0.0/gascompressibility/z_correlation/londono.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.7/gascompressibility.egg-info/SOURCES.txt` & `gascompressibility-1.0.0/gascompressibility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.7/setup.py` & `gascompressibility-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def classifiers():
     with open('classifiers.txt') as f:
         return f.read().strip().split('\n')
 
 
 setup(
     name='gascompressibility',
-    version='0.1.7',
+    version='1.0.0',
     packages=find_packages(exclude=[
         "tutorials",
         "LICENSE",
         ".gitignore",
         "README.md",
         "misc",
         ".travis.yml",
```

### Comparing `gascompressibility-0.1.7/tests/test_gascomp.py` & `gascompressibility-1.0.0/tests/test_gascomp.py`

 * *Files 0% similar despite different names*

```diff
@@ -526,96 +526,96 @@
         self.assertAlmostEqual(instance.Ppc, 747.9479, places=3)
         self.assertAlmostEqual(instance.Pr, 2.6874, places=3)
 
         print('calc_Pr passed (mode="Piper")')
 
     def test_calc_z(self):
 
-        ps_props = calc_z(P=1995.3, T=75, CO2=0.1, H2S=0.07, sg=0.7, ps_props=True, zmodel='DAK', pmodel='Sutton')
+        ps_props = calc_z(P=1995.3, T=75, CO2=0.1, H2S=0.07, sg=0.7, ps_props=True, zmodel='DAK', pmodel='sutton')
 
         self.assertAlmostEqual(ps_props['z'], 0.7730, places=3)
         self.assertAlmostEqual(ps_props['e_correction'], 21.2778, places=3)
         self.assertAlmostEqual(ps_props['Ppc_corrected'], 628.2143, places=3)
         self.assertAlmostEqual(ps_props['Tpc_corrected'], 356.3122, places=3)
         self.assertAlmostEqual(ps_props['Ppc'], 663.287, places=3)
         self.assertAlmostEqual(ps_props['Tpc'], 377.59, places=3)
         self.assertAlmostEqual(ps_props['Pr'], 3.1995, places=3)
         self.assertAlmostEqual(ps_props['Tr'], 1.5006, places=3)
 
-        ps_props = calc_z(P=1995.3, T=75, Ppc=747.9, Tpc=373.6, ps_props=True, zmodel='DAK', pmodel='Sutton')
+        ps_props = calc_z(P=1995.3, T=75, Ppc=747.9, Tpc=373.6, ps_props=True, zmodel='DAK', pmodel='sutton')
 
         self.assertAlmostEqual(ps_props['z'], 0.7418, places=3)
         self.assertEqual(ps_props['Ppc'], None)
         self.assertEqual(ps_props['Tpc'], None)
         self.assertAlmostEqual(ps_props['e_correction'], 0.0, places=3)
         self.assertAlmostEqual(ps_props['Ppc_corrected'], 747.9, places=3)
         self.assertAlmostEqual(ps_props['Tpc_corrected'], 373.6, places=3)
         self.assertAlmostEqual(ps_props['Pr'], 2.6875, places=3)
         self.assertAlmostEqual(ps_props['Tr'], 1.4311, places=3)
 
-        ps_props = calc_z(Pr=3.1995, T=75, Tpc=377.59, e_correction=21.278, ignore_conflict=True, ps_props=True, zmodel='DAK', pmodel='Sutton')
+        ps_props = calc_z(Pr=3.1995, T=75, Tpc=377.59, e_correction=21.278, ignore_conflict=True, ps_props=True, zmodel='DAK', pmodel='sutton')
 
         self.assertAlmostEqual(ps_props['z'], 0.7730, places=3)
         self.assertAlmostEqual(ps_props['Tpc_corrected'], 356.312, places=3)
         self.assertAlmostEqual(ps_props['Tr'], 1.5006, places=3)
 
-        ps_props = calc_z(Tpc_corrected=356.31, sg=0.7, P=1995.3, T=75, H2S=0.07, CO2=0.1, ignore_conflict=True, ps_props=True, zmodel='DAK', pmodel='Sutton')
+        ps_props = calc_z(Tpc_corrected=356.31, sg=0.7, P=1995.3, T=75, H2S=0.07, CO2=0.1, ignore_conflict=True, ps_props=True, zmodel='DAK', pmodel='sutton')
 
         self.assertAlmostEqual(ps_props['z'], 0.7730, places=3)
         self.assertAlmostEqual(ps_props['e_correction'], 21.2778, places=3)
         self.assertAlmostEqual(ps_props['Ppc_corrected'], 628.2104, places=3)
         self.assertAlmostEqual(ps_props['Ppc'], 663.287, places=3)
         self.assertAlmostEqual(ps_props['Tpc'], 377.59, places=3)
         self.assertAlmostEqual(ps_props['Pr'], 3.1996, places=3)
         self.assertAlmostEqual(ps_props['Tr'], 1.5006, places=3)
 
         print('calc_z passed (mode="Sutton")')
 
-        ps_props = calc_z(P=1995.3, T=75, sg=0.7, H2S=0.07, CO2=0.1, N2=0, ps_props=True, zmodel='DAK', pmodel='Piper')
+        ps_props = calc_z(P=1995.3, T=75, sg=0.7, H2S=0.07, CO2=0.1, N2=0, ps_props=True, zmodel='DAK', pmodel='piper')
 
         self.assertAlmostEqual(ps_props['z'], 0.7418, places=3)
         self.assertAlmostEqual(ps_props['J'], 0.4995, places=3)
         self.assertAlmostEqual(ps_props['K'], 13.6612, places=3)
         self.assertAlmostEqual(ps_props['Ppc'], 747.9468, places=3)
         self.assertAlmostEqual(ps_props['Tpc'], 373.6153, places=3)
         self.assertAlmostEqual(ps_props['Pr'], 2.6874, places=3)
         self.assertAlmostEqual(ps_props['Tr'], 1.4311, places=3)
 
-        ps_props = calc_z(P=1995.3, T=75, sg=0.7, H2S=0.07, CO2=0.1, N2=0.1, ps_props=True, zmodel='DAK', pmodel='Piper')
+        ps_props = calc_z(P=1995.3, T=75, sg=0.7, H2S=0.07, CO2=0.1, N2=0.1, ps_props=True, zmodel='DAK', pmodel='piper')
 
         self.assertAlmostEqual(ps_props['z'], 0.8093, places=3)
         self.assertAlmostEqual(ps_props['J'], 0.4691, places=3)
         self.assertAlmostEqual(ps_props['K'], 12.7271, places=3)
         self.assertAlmostEqual(ps_props['Ppc'], 736.2064, places=3)
         self.assertAlmostEqual(ps_props['Tpc'], 345.3259, places=3)
         self.assertAlmostEqual(ps_props['Pr'], 2.7302, places=3)
         self.assertAlmostEqual(ps_props['Tr'], 1.5483, places=3)
 
-        ps_props = calc_z(P=1995.3, T=75, K=13.661, J=0.4995, ps_props=True, zmodel='DAK', pmodel='Piper')
+        ps_props = calc_z(P=1995.3, T=75, K=13.661, J=0.4995, ps_props=True, zmodel='DAK', pmodel='piper')
 
         self.assertAlmostEqual(ps_props['z'], 0.7418, places=3)
         self.assertAlmostEqual(ps_props['Ppc'], 747.9869, places=3)
         self.assertAlmostEqual(ps_props['Tpc'], 373.6195, places=3)
         self.assertAlmostEqual(ps_props['Pr'], 2.6872, places=3)
         self.assertAlmostEqual(ps_props['Tr'], 1.4311, places=3)
 
-        ps_props = calc_z(P=1995.3, T=75, Tpc=373.6, J=0.4995, ignore_conflict=True, ps_props=True, zmodel='DAK', pmodel='Piper')
+        ps_props = calc_z(P=1995.3, T=75, Tpc=373.6, J=0.4995, ignore_conflict=True, ps_props=True, zmodel='DAK', pmodel='piper')
 
         self.assertAlmostEqual(ps_props['z'], 0.7418, places=3)
         self.assertAlmostEqual(ps_props['Ppc'], 747.9479, places=3)
         self.assertAlmostEqual(ps_props['Pr'], 2.6874, places=3)
         self.assertAlmostEqual(ps_props['Tr'], 1.4311, places=3)
 
-        ps_props = calc_z(T=75, Pr=2.687, K=13.661, J=0.4995, ignore_conflict=True, ps_props=True, zmodel='DAK', pmodel='Piper')
+        ps_props = calc_z(T=75, Pr=2.687, K=13.661, J=0.4995, ignore_conflict=True, ps_props=True, zmodel='DAK', pmodel='piper')
 
         self.assertAlmostEqual(ps_props['z'], 0.7418, places=3)
         self.assertAlmostEqual(ps_props['Tpc'], 373.6195, places=3)
         self.assertAlmostEqual(ps_props['Tr'], 1.4311, places=3)
 
-        ps_props = calc_z(P=1995.3, T=75, Ppc=663.28, Tpc=377.59, ignore_conflict=True, ps_props=True, zmodel='DAK', pmodel='Piper')
+        ps_props = calc_z(P=1995.3, T=75, Ppc=663.28, Tpc=377.59, ignore_conflict=True, ps_props=True, zmodel='DAK', pmodel='piper')
 
         self.assertAlmostEqual(ps_props['z'], 0.7207, places=3)
         self.assertAlmostEqual(ps_props['Pr'], 3.0304, places=3)
         self.assertAlmostEqual(ps_props['Tr'], 1.416, places=3)
 
         print('calc_z passed (mode="Piper")')
 
@@ -633,34 +633,34 @@
         self.assertAlmostEqual(result, 0.7754, places=3)
         print('calc_z_models passed (model="londono")')
 
         result = calc_z(zmodel="kareem", Pr=3.1995, Tr=1.5006)
         self.assertAlmostEqual(result, 0.7667, places=3)
         print('calc_z_models passed (model="kareem")')
 
-        result = calc_z(sg=0.7, H2S=0.07, CO2=0.1, P=2010-14.7, T=75, guess=0.9, zmodel='DAK', pmodel='Sutton')
+        result = calc_z(sg=0.7, H2S=0.07, CO2=0.1, P=2010-14.7, T=75, guess=0.9, zmodel='DAK', pmodel='sutton')
         self.assertAlmostEqual(result, 0.7730, places=3)
 
-        result = calc_z(sg=0.7, H2S=0.07, CO2=0.1, N2=0.1, P=2010-14.7, guess=0.9, T=75, zmodel='DAK', pmodel='Piper')
+        result = calc_z(sg=0.7, H2S=0.07, CO2=0.1, N2=0.1, P=2010-14.7, guess=0.9, T=75, zmodel='DAK', pmodel='piper')
         self.assertAlmostEqual(result, 0.8093, places=3)
 
-        result = calc_z(sg=0.7, H2S=0.07, CO2=0.1, P=2010-14.7, T=75, zmodel='kareem', pmodel='Piper')
+        result = calc_z(sg=0.7, H2S=0.07, CO2=0.1, P=2010-14.7, T=75, zmodel='kareem', pmodel='piper')
         self.assertAlmostEqual(result, 0.7319, places=3)
 
-        result = calc_z(sg=0.7, H2S=0.07, CO2=0.1, P=2010-14.7, T=75, N2=0.1, zmodel='hall_yarborough', pmodel='Piper')
+        result = calc_z(sg=0.7, H2S=0.07, CO2=0.1, P=2010-14.7, T=75, N2=0.1, zmodel='hall_yarborough', pmodel='piper')
         self.assertAlmostEqual(result, 0.8084, places=3)
 
         with self.assertRaises(TypeError):
-            calc_z(sg=0.7, H2S=0.07, CO2=0.1, P=2010 - 14.7, Ppc=135, T=75, zmodel='DAK', pmodel='Piper')
+            calc_z(sg=0.7, H2S=0.07, CO2=0.1, P=2010 - 14.7, Ppc=135, T=75, zmodel='DAK', pmodel='piper')
 
         with self.assertRaises(TypeError):
-            calc_z(sg=0.7, H2S=0.07, CO2=0.1, P=2010 - 14.7, Pr=1.5, T=75, zmodel='DAK', pmodel='Sutton')
+            calc_z(sg=0.7, H2S=0.07, CO2=0.1, P=2010 - 14.7, Pr=1.5, T=75, zmodel='DAK', pmodel='sutton')
 
         with self.assertRaises(KeyError):
-            calc_z(sg=0.7, H2S=0.07, CO2=0.1, N2=0.1, P=2010 - 14.7, T=75, guess=0.9, zmodel='kareem', pmodel='Piper')
+            calc_z(sg=0.7, H2S=0.07, CO2=0.1, N2=0.1, P=2010 - 14.7, T=75, guess=0.9, zmodel='kareem', pmodel='piper')
 
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

