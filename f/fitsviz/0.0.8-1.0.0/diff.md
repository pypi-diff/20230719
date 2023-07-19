# Comparing `tmp/fitsviz-0.0.8.tar.gz` & `tmp/fitsviz-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fitsviz-0.0.8.tar", last modified: Tue Jul 18 23:22:27 2023, max compression
+gzip compressed data, was "fitsviz-1.0.0.tar", last modified: Wed Jul 19 09:55:45 2023, max compression
```

## Comparing `fitsviz-0.0.8.tar` & `fitsviz-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxr-sr-x   0 openvscode-server  (1000) openvscode-server  (1000)        0 2023-07-18 23:22:27.671363 fitsviz-0.0.8/
--rw-r--r--   0 openvscode-server  (1000) openvscode-server  (1000)     2126 2023-07-18 23:22:27.671363 fitsviz-0.0.8/PKG-INFO
--rw-r--r--   0 openvscode-server  (1000) openvscode-server  (1000)     1888 2023-07-18 23:09:57.000000 fitsviz-0.0.8/README.md
-drwxr-sr-x   0 openvscode-server  (1000) openvscode-server  (1000)        0 2023-07-18 23:22:27.669363 fitsviz-0.0.8/fitsviz/
--rw-r--r--   0 openvscode-server  (1000) openvscode-server  (1000)      203 2023-07-18 23:09:57.000000 fitsviz-0.0.8/fitsviz/__init__.py
--rw-r--r--   0 openvscode-server  (1000) openvscode-server  (1000)     2829 2023-07-18 23:10:23.000000 fitsviz-0.0.8/fitsviz/__main__.py
-drwxr-sr-x   0 openvscode-server  (1000) openvscode-server  (1000)        0 2023-07-18 23:22:27.670363 fitsviz-0.0.8/fitsviz/detection/
--rw-r--r--   0 openvscode-server  (1000) openvscode-server  (1000)       71 2023-07-18 23:09:57.000000 fitsviz-0.0.8/fitsviz/detection/__init__.py
--rw-r--r--   0 openvscode-server  (1000) openvscode-server  (1000)     8040 2023-07-18 23:09:57.000000 fitsviz-0.0.8/fitsviz/detection/ap_photometry.py
--rw-r--r--   0 openvscode-server  (1000) openvscode-server  (1000)     1485 2023-07-18 23:09:57.000000 fitsviz-0.0.8/fitsviz/detection/core.py
-drwxr-sr-x   0 openvscode-server  (1000) openvscode-server  (1000)        0 2023-07-18 23:22:27.670363 fitsviz-0.0.8/fitsviz/tests/
--rw-r--r--   0 openvscode-server  (1000) openvscode-server  (1000)        0 2023-07-18 23:09:57.000000 fitsviz-0.0.8/fitsviz/tests/__init__.py
--rw-r--r--   0 openvscode-server  (1000) openvscode-server  (1000)        0 2023-07-18 23:09:57.000000 fitsviz-0.0.8/fitsviz/tests/test_loading.py
--rw-r--r--   0 openvscode-server  (1000) openvscode-server  (1000)        0 2023-07-18 23:09:57.000000 fitsviz-0.0.8/fitsviz/tests/test_viz.py
-drwxr-sr-x   0 openvscode-server  (1000) openvscode-server  (1000)        0 2023-07-18 23:22:27.670363 fitsviz-0.0.8/fitsviz/utils/
--rw-r--r--   0 openvscode-server  (1000) openvscode-server  (1000)       21 2023-07-18 23:09:57.000000 fitsviz-0.0.8/fitsviz/utils/__init__.py
--rw-r--r--   0 openvscode-server  (1000) openvscode-server  (1000)     2392 2023-07-18 23:09:57.000000 fitsviz-0.0.8/fitsviz/utils/cutils.py
-drwxr-sr-x   0 openvscode-server  (1000) openvscode-server  (1000)        0 2023-07-18 23:22:27.671363 fitsviz-0.0.8/fitsviz/viz/
--rw-r--r--   0 openvscode-server  (1000) openvscode-server  (1000)        0 2023-07-18 23:09:57.000000 fitsviz-0.0.8/fitsviz/viz/__init__.py
--rw-r--r--   0 openvscode-server  (1000) openvscode-server  (1000)     2315 2023-07-18 23:09:57.000000 fitsviz-0.0.8/fitsviz/viz/plot_bokeh.py
--rw-r--r--   0 openvscode-server  (1000) openvscode-server  (1000)     1226 2023-07-18 23:09:57.000000 fitsviz-0.0.8/fitsviz/viz/plot_matplotlib.py
-drwxr-sr-x   0 openvscode-server  (1000) openvscode-server  (1000)        0 2023-07-18 23:22:27.669363 fitsviz-0.0.8/fitsviz.egg-info/
--rw-r--r--   0 openvscode-server  (1000) openvscode-server  (1000)     2126 2023-07-18 23:22:27.000000 fitsviz-0.0.8/fitsviz.egg-info/PKG-INFO
--rw-r--r--   0 openvscode-server  (1000) openvscode-server  (1000)      522 2023-07-18 23:22:27.000000 fitsviz-0.0.8/fitsviz.egg-info/SOURCES.txt
--rw-r--r--   0 openvscode-server  (1000) openvscode-server  (1000)        1 2023-07-18 23:22:27.000000 fitsviz-0.0.8/fitsviz.egg-info/dependency_links.txt
--rw-r--r--   0 openvscode-server  (1000) openvscode-server  (1000)      117 2023-07-18 23:22:27.000000 fitsviz-0.0.8/fitsviz.egg-info/requires.txt
--rw-r--r--   0 openvscode-server  (1000) openvscode-server  (1000)        8 2023-07-18 23:22:27.000000 fitsviz-0.0.8/fitsviz.egg-info/top_level.txt
--rw-r--r--   0 openvscode-server  (1000) openvscode-server  (1000)      556 2023-07-18 23:22:22.000000 fitsviz-0.0.8/pyproject.toml
--rw-r--r--   0 openvscode-server  (1000) openvscode-server  (1000)       38 2023-07-18 23:22:27.671363 fitsviz-0.0.8/setup.cfg
+drwxr-xr-x   0 phani      (501) staff       (20)        0 2023-07-19 09:55:45.031513 fitsviz-1.0.0/
+-rw-r--r--   0 phani      (501) staff       (20)     2126 2023-07-19 09:55:45.031212 fitsviz-1.0.0/PKG-INFO
+-rw-r--r--   0 phani      (501) staff       (20)     1888 2023-07-18 03:58:12.000000 fitsviz-1.0.0/README.md
+drwxr-xr-x   0 phani      (501) staff       (20)        0 2023-07-19 09:55:45.021777 fitsviz-1.0.0/fitsviz/
+-rw-r--r--   0 phani      (501) staff       (20)      203 2023-07-18 19:56:37.000000 fitsviz-1.0.0/fitsviz/__init__.py
+-rw-r--r--   0 phani      (501) staff       (20)     4644 2023-07-19 09:42:18.000000 fitsviz-1.0.0/fitsviz/__main__.py
+drwxr-xr-x   0 phani      (501) staff       (20)        0 2023-07-19 09:55:45.027443 fitsviz-1.0.0/fitsviz/detection/
+-rw-r--r--   0 phani      (501) staff       (20)       71 2023-07-18 03:23:42.000000 fitsviz-1.0.0/fitsviz/detection/__init__.py
+-rw-r--r--   0 phani      (501) staff       (20)     4147 2023-07-19 09:42:19.000000 fitsviz-1.0.0/fitsviz/detection/ap_photometry.py
+-rw-r--r--   0 phani      (501) staff       (20)     1898 2023-07-19 09:42:19.000000 fitsviz-1.0.0/fitsviz/detection/core.py
+drwxr-xr-x   0 phani      (501) staff       (20)        0 2023-07-19 09:55:45.029083 fitsviz-1.0.0/fitsviz/tests/
+-rw-r--r--   0 phani      (501) staff       (20)        0 2023-07-15 02:14:13.000000 fitsviz-1.0.0/fitsviz/tests/__init__.py
+-rw-r--r--   0 phani      (501) staff       (20)        0 2023-07-15 22:40:02.000000 fitsviz-1.0.0/fitsviz/tests/test_loading.py
+-rw-r--r--   0 phani      (501) staff       (20)        0 2023-07-15 02:19:14.000000 fitsviz-1.0.0/fitsviz/tests/test_viz.py
+drwxr-xr-x   0 phani      (501) staff       (20)        0 2023-07-19 09:55:45.029962 fitsviz-1.0.0/fitsviz/utils/
+-rw-r--r--   0 phani      (501) staff       (20)       22 2023-07-19 09:42:18.000000 fitsviz-1.0.0/fitsviz/utils/__init__.py
+-rw-r--r--   0 phani      (501) staff       (20)     2467 2023-07-19 09:48:10.000000 fitsviz-1.0.0/fitsviz/utils/cutils.py
+drwxr-xr-x   0 phani      (501) staff       (20)        0 2023-07-19 09:55:45.030772 fitsviz-1.0.0/fitsviz/viz/
+-rw-r--r--   0 phani      (501) staff       (20)        0 2023-07-19 09:47:33.000000 fitsviz-1.0.0/fitsviz/viz/__init__.py
+-rw-r--r--   0 phani      (501) staff       (20)     5920 2023-07-19 09:47:31.000000 fitsviz-1.0.0/fitsviz/viz/plot_bokeh.py
+drwxr-xr-x   0 phani      (501) staff       (20)        0 2023-07-19 09:55:45.025784 fitsviz-1.0.0/fitsviz.egg-info/
+-rw-r--r--   0 phani      (501) staff       (20)     2126 2023-07-19 09:55:44.000000 fitsviz-1.0.0/fitsviz.egg-info/PKG-INFO
+-rw-r--r--   0 phani      (501) staff       (20)      491 2023-07-19 09:55:45.000000 fitsviz-1.0.0/fitsviz.egg-info/SOURCES.txt
+-rw-r--r--   0 phani      (501) staff       (20)        1 2023-07-19 09:55:44.000000 fitsviz-1.0.0/fitsviz.egg-info/dependency_links.txt
+-rw-r--r--   0 phani      (501) staff       (20)      173 2023-07-19 09:55:44.000000 fitsviz-1.0.0/fitsviz.egg-info/requires.txt
+-rw-r--r--   0 phani      (501) staff       (20)        8 2023-07-19 09:55:44.000000 fitsviz-1.0.0/fitsviz.egg-info/top_level.txt
+-rw-r--r--   0 phani      (501) staff       (20)      612 2023-07-19 09:55:42.000000 fitsviz-1.0.0/pyproject.toml
+-rw-r--r--   0 phani      (501) staff       (20)       38 2023-07-19 09:55:45.031602 fitsviz-1.0.0/setup.cfg
```

### Comparing `fitsviz-0.0.8/PKG-INFO` & `fitsviz-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fitsviz
-Version: 0.0.8
+Version: 1.0.0
 Summary: Autodetection of sources and visualization of FITS files
 Author-email: Phani Velicheti <phaniv@arizona.edu>
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 
 # fitsviz
```

### Comparing `fitsviz-0.0.8/README.md` & `fitsviz-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `fitsviz-0.0.8/fitsviz/detection/core.py` & `fitsviz-1.0.0/fitsviz/detection/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,22 +23,33 @@
             science_data (np.ndarray): Science data
             rms_data (np.ndarray): RMS data
 
         Returns:
             table (pd.DataFrame): table with xcentroid,ycentroid,flux,spectral_index as columns. or None
         """
         raise NotImplementedError('Needs to be implemented in a subclass.')
-    
+
+    @abstractmethod
+    def get_fluxs(self, sources):
+        """Given science and rms files, apply a custom detection algorithm
+
+        Args:
+            science_data (np.ndarray): Science data
+            rms_data (np.ndarray): RMS data
+
+        Returns:
+            table (pd.DataFrame): table with xcentroid,ycentroid,flux,spectral_index as columns. or None
+        """
+        raise NotImplementedError('Needs to be implemented in a subclass.')
+
     @abstractmethod
-    def process_sources(self, science_data, rms_data):
+    def get_summary(self, fluxs):
         """Given science and rms files, apply a custom detection algorithm
 
         Args:
             science_data (np.ndarray): Science data
             rms_data (np.ndarray): RMS data
 
         Returns:
             table (pd.DataFrame): table with xcentroid,ycentroid,flux,spectral_index as columns. or None
         """
         raise NotImplementedError('Needs to be implemented in a subclass.')
-        
-
```

### Comparing `fitsviz-0.0.8/fitsviz/utils/cutils.py` & `fitsviz-1.0.0/fitsviz/utils/cutils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+"""
+Common utils for all modules and algorithms
+"""
 from astropy.io import fits
 import numpy as np
 from dask.distributed import Client
 
 
-
-
 def load_fits(file_name):
     """
     Load FITS files and index into data
 
     Args:
         file_name (str):file path 
 
@@ -27,24 +28,25 @@
 
     Returns:
         np.ndarray: Returned fits file at the first axis
     """
     file_name = file_name.replace("tt0.subim.fits", "tt0.rms.subim.fits")
     return fits.getdata(file_name)[0, 0, :, :]
 
+
 def get_image_with_least_freq(science_img_names):
     """
     Given a list of science files, get the image name with the lowest frequency.
     Args:
         science_img_names (list[str]): science file names
 
     Returns:
         str: science file name of lowest frequency
     """
-    #MAX INT in python3
+    # maximum value for a 64-bit signed integer.
     cur_freq = 9223372036854775807
     least_freq_img = None
 
     for sci_img in science_img_names:
         sci_img_freq = fits.getheader(sci_img)['CRVAL3']
         if cur_freq > sci_img_freq:
             cur_freq = sci_img_freq
@@ -57,14 +59,15 @@
 
     Args:
         dask_client (dask.distributed.Client): Dask client
     """
     client = Client(n_workers=n_workers)
     return client
 
+
 def calculate_spectral_indices(frequencies, flux_densities):
     """
     Calculate the spectral index of a source given a list of frequencies and flux densities
     Args:
         frequencies (list[float]): List of frequencies
         flux_densities (list[float]): List of flux densities
         Returns:
@@ -76,16 +79,14 @@
     # Fit a linear regression to calculate the spectral index
     coefficients = np.polyfit(log_frequencies, log_flux_densities, deg=1)
     spectral_index = coefficients[0]
 
     return spectral_index
 
 
-
-
 def cleanup_dask_client(dask_client):
     """Clean up dask dask client on system exit
 
     Args:
         dask_client (dask.distributed.Client): Dask client
     """
     if dask_client is not None:
```

### Comparing `fitsviz-0.0.8/fitsviz.egg-info/PKG-INFO` & `fitsviz-1.0.0/fitsviz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fitsviz
-Version: 0.0.8
+Version: 1.0.0
 Summary: Autodetection of sources and visualization of FITS files
 Author-email: Phani Velicheti <phaniv@arizona.edu>
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 
 # fitsviz
```

### Comparing `fitsviz-0.0.8/pyproject.toml` & `fitsviz-1.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ['setuptools>=68.0.0']
 
 [project]
 
 name = "fitsviz"
-version = "0.0.8"
+version = "1.0.0"
 description = "Autodetection of sources and visualization of FITS files"
 
 authors = [
     {name="Phani Velicheti",email = "phaniv@arizona.edu"}
 ]
 
 readme = "README.md"
 requires-python = ">= 3.8, < 3.12"
 
 dependencies = [
     'poetry-core',
-    'astropy',
-    'bokeh',
-    'click',
-    'dask',
+    'astropy==5.3.1',
+    'bokeh==3.2.0',
+    'click==8.1.5',
+    'dask==2023.7.0',
     'matplotlib==3.7.2',
-    'numpy',
-    'pandas',
-    'scipy==1.11.0',
+    'numpy==1.25.1',
+    'pandas==2.0.3',
+    'scipy==1.11.1',
     'photutils==1.8.0',
-    'dask[distributed]'
+    'dask[distributed]==2023.7.0'
 
 ]
```

