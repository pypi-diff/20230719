# Comparing `tmp/hpcom-0.1.8.tar.gz` & `tmp/hpcom-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpcom-0.1.8.tar", last modified: Thu Jul 13 15:39:56 2023, max compression
+gzip compressed data, was "hpcom-0.1.9.tar", last modified: Wed Jul 19 13:08:56 2023, max compression
```

## Comparing `hpcom-0.1.8.tar` & `hpcom-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-13 15:39:56.868414 hpcom-0.1.8/
--rw-rw-r--   0 esf0      (1000) esf0      (1000)    35137 2022-11-10 15:49:50.000000 hpcom-0.1.8/LICENSE
--rw-rw-r--   0 esf0      (1000) esf0      (1000)    42235 2023-07-13 15:39:56.868414 hpcom-0.1.8/PKG-INFO
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     1080 2023-04-30 12:37:52.000000 hpcom-0.1.8/README.md
-drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-13 15:39:56.864414 hpcom-0.1.8/hpcom/
--rw-rw-r--   0 esf0      (1000) esf0      (1000)      239 2022-12-14 10:00:50.000000 hpcom-0.1.8/hpcom/__init__.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)    58698 2023-07-13 15:38:19.000000 hpcom-0.1.8/hpcom/channel.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)      434 2022-11-11 14:09:01.000000 hpcom-0.1.8/hpcom/decorators.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)    13393 2022-11-23 13:08:09.000000 hpcom-0.1.8/hpcom/hpcom_old.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     4996 2023-04-13 16:56:44.000000 hpcom-0.1.8/hpcom/metrics.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     7485 2022-11-23 13:22:15.000000 hpcom-0.1.8/hpcom/modulation.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)      452 2023-04-12 17:22:11.000000 hpcom-0.1.8/hpcom/plot.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)    23931 2023-07-11 13:29:01.000000 hpcom-0.1.8/hpcom/signal.py
-drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-13 15:39:56.864414 hpcom-0.1.8/hpcom.egg-info/
--rw-rw-r--   0 esf0      (1000) esf0      (1000)    42235 2023-07-13 15:39:56.000000 hpcom-0.1.8/hpcom.egg-info/PKG-INFO
--rw-rw-r--   0 esf0      (1000) esf0      (1000)      425 2023-07-13 15:39:56.000000 hpcom-0.1.8/hpcom.egg-info/SOURCES.txt
--rw-rw-r--   0 esf0      (1000) esf0      (1000)        1 2023-07-13 15:39:56.000000 hpcom-0.1.8/hpcom.egg-info/dependency_links.txt
--rw-rw-r--   0 esf0      (1000) esf0      (1000)        6 2023-07-13 15:39:56.000000 hpcom-0.1.8/hpcom.egg-info/top_level.txt
--rw-rw-r--   0 esf0      (1000) esf0      (1000)      707 2023-07-13 15:38:19.000000 hpcom-0.1.8/pyproject.toml
--rw-rw-r--   0 esf0      (1000) esf0      (1000)       38 2023-07-13 15:39:56.868414 hpcom-0.1.8/setup.cfg
-drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-13 15:39:56.864414 hpcom-0.1.8/tests/
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     2216 2023-07-06 13:53:07.000000 hpcom-0.1.8/tests/test_back_to_back.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     1910 2023-01-18 15:52:29.000000 hpcom-0.1.8/tests/test_channel_model.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)      719 2022-12-14 10:08:52.000000 hpcom-0.1.8/tests/test_generation.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     1730 2023-06-21 12:18:51.000000 hpcom-0.1.8/tests/test_ofdm_generation.py
--rw-rw-r--   0 esf0      (1000) esf0      (1000)     2421 2022-12-14 11:09:37.000000 hpcom-0.1.8/tests/test_propagation.py
+drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-19 13:08:56.520934 hpcom-0.1.9/
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)    35137 2022-11-10 15:49:50.000000 hpcom-0.1.9/LICENSE
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)    42235 2023-07-19 13:08:56.520934 hpcom-0.1.9/PKG-INFO
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     1080 2023-04-30 12:37:52.000000 hpcom-0.1.9/README.md
+drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-19 13:08:56.520934 hpcom-0.1.9/hpcom/
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)      265 2023-07-14 12:02:08.000000 hpcom-0.1.9/hpcom/__init__.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)    25306 2023-07-14 12:04:05.000000 hpcom-0.1.9/hpcom/_sklearn_functions.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)    59741 2023-07-19 13:06:33.000000 hpcom-0.1.9/hpcom/channel.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)      434 2022-11-11 14:09:01.000000 hpcom-0.1.9/hpcom/decorators.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)    13393 2022-11-23 13:08:09.000000 hpcom-0.1.9/hpcom/hpcom_old.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     5379 2023-07-14 12:05:37.000000 hpcom-0.1.9/hpcom/metrics.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     9795 2023-07-18 15:09:23.000000 hpcom-0.1.9/hpcom/modulation.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     1046 2023-07-18 14:31:18.000000 hpcom-0.1.9/hpcom/plot.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)    24387 2023-07-18 15:09:23.000000 hpcom-0.1.9/hpcom/signal.py
+drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-19 13:08:56.520934 hpcom-0.1.9/hpcom.egg-info/
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)    42235 2023-07-19 13:08:56.000000 hpcom-0.1.9/hpcom.egg-info/PKG-INFO
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)      453 2023-07-19 13:08:56.000000 hpcom-0.1.9/hpcom.egg-info/SOURCES.txt
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)        1 2023-07-19 13:08:56.000000 hpcom-0.1.9/hpcom.egg-info/dependency_links.txt
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)        6 2023-07-19 13:08:56.000000 hpcom-0.1.9/hpcom.egg-info/top_level.txt
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)      707 2023-07-19 13:07:31.000000 hpcom-0.1.9/pyproject.toml
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)       38 2023-07-19 13:08:56.520934 hpcom-0.1.9/setup.cfg
+drwxrwxr-x   0 esf0      (1000) esf0      (1000)        0 2023-07-19 13:08:56.520934 hpcom-0.1.9/tests/
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     2216 2023-07-06 13:53:07.000000 hpcom-0.1.9/tests/test_back_to_back.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     1910 2023-01-18 15:52:29.000000 hpcom-0.1.9/tests/test_channel_model.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)      719 2022-12-14 10:08:52.000000 hpcom-0.1.9/tests/test_generation.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     1730 2023-06-21 12:18:51.000000 hpcom-0.1.9/tests/test_ofdm_generation.py
+-rw-rw-r--   0 esf0      (1000) esf0      (1000)     2421 2022-12-14 11:09:37.000000 hpcom-0.1.9/tests/test_propagation.py
```

### Comparing `hpcom-0.1.8/LICENSE` & `hpcom-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.8/PKG-INFO` & `hpcom-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpcom
-Version: 0.1.8
+Version: 0.1.9
 Summary: High performance optical communication library
 Author-email: Egor Sedov <e.sedov@g.nsu.ru>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hpcom-0.1.8/README.md` & `hpcom-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.8/hpcom/channel.py` & `hpcom-0.1.9/hpcom/channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from datetime import datetime
 
 from .signal import create_wdm_parameters, generate_wdm, generate_wdm_optimise, receiver, receiver_wdm,\
     nonlinear_shift, dbm_to_mw, get_default_wdm_parameters, get_points_wdm
 from .modulation import get_modulation_type_from_order, get_scale_coef_constellation, \
     get_nearest_constellation_points_unscaled
 from .metrics import get_ber_by_points, get_ber_by_points_ultimate, get_energy, get_average_power, get_evm_ultimate, \
-    get_evm
+    get_evm, calculate_mutual_information
 
 from ssfm_gpu.propagation import propagate_manakov, propagate_manakov_backward, \
     propagate_schrodinger, dispersion_compensation_manakov
 
 # Channel parameters
 
 
@@ -525,38 +525,49 @@
 
         ber_x = []
         ber_y = []
         q_x = []
         q_y = []
         evm_x = []
         evm_y = []
+        mi_x = []
+        mi_y = []
 
         for k in range(wdm['n_channels']):
             print('WDM channel', k) if verbose >= 1 else ...
 
             start_time = datetime.now()
             points_x_found.append(get_nearest_constellation_points_unscaled(points_x_shifted[k], mod_type))
             points_y_found.append(get_nearest_constellation_points_unscaled(points_y_shifted[k], mod_type))
             print("search x and y points took",
                   (datetime.now() - start_time).total_seconds() * 1000, "ms") if verbose >= 2 else ...
 
+            points_x_orig_scaled = points_x_orig[k] * scale_constellation
+            points_y_orig_scaled = points_y_orig[k] * scale_constellation
+
+
             start_time = datetime.now()
-            ber_x.append(get_ber_by_points(points_x_orig[k] * scale_constellation, points_x_found[k], mod_type))
-            ber_y.append(get_ber_by_points(points_y_orig[k] * scale_constellation, points_y_found[k], mod_type))
+            ber_x.append(get_ber_by_points(points_x_orig_scaled, points_x_found[k], mod_type))
+            ber_y.append(get_ber_by_points(points_y_orig_scaled, points_y_found[k], mod_type))
             print("ber for x and y took",
                   (datetime.now() - start_time).total_seconds() * 1000, "ms") if verbose >= 2 else ...
 
             q_x.append(np.sqrt(2) * sp.special.erfcinv(2 * ber_x[k][0]))
             q_y.append(np.sqrt(2) * sp.special.erfcinv(2 * ber_y[k][0]))
 
-            evm_x.append(get_evm(points_x_orig[k] * scale_constellation, points_x_shifted[k] * scale_constellation))
-            evm_y.append(get_evm(points_y_orig[k] * scale_constellation, points_y_shifted[k] * scale_constellation))
+            evm_x.append(get_evm(points_x_orig_scaled, points_x_shifted[k] * scale_constellation))
+            evm_y.append(get_evm(points_y_orig_scaled, points_y_shifted[k] * scale_constellation))
+
+            mi_x.append(calculate_mutual_information(points_x_orig_scaled, points_x_found[k]))
+            mi_y.append(calculate_mutual_information(points_y_orig_scaled, points_y_found[k]))
 
             print("BER (x / y):", ber_x[k], ber_y[k]) if verbose >= 1 else ...
             print(r'Q^2-factor (x / y):', q_x[k], q_y[k]) if verbose >= 1 else ...
+            print(r'EVM (x / y):', evm_x[k], evm_y[k]) if verbose >= 1 else ...
+            print(r'MI (x / y):', mi_x[k], mi_y[k]) if verbose >= 1 else ...
 
     elif channels_type == 'middle':
 
         k = (wdm['n_channels'] - 1) // 2
 
         samples_x_temp = samples_x[k]
         samples_y_temp = samples_y[k]
@@ -575,28 +586,36 @@
 
         start_time = datetime.now()
         points_x_found = get_nearest_constellation_points_unscaled(points_x_shifted, mod_type)
         points_y_found = get_nearest_constellation_points_unscaled(points_y_shifted, mod_type)
         print("search x and y points took",
               (datetime.now() - start_time).total_seconds() * 1000, "ms") if verbose >= 2 else ...
 
+        points_x_orig_scaled = points_x_orig[k] * scale_constellation
+        points_y_orig_scaled = points_y_orig[k] * scale_constellation
+
         start_time = datetime.now()
-        ber_x = get_ber_by_points(points_x_orig[k] * scale_constellation, points_x_found, mod_type)
-        ber_y = get_ber_by_points(points_y_orig[k] * scale_constellation, points_y_found, mod_type)
+        ber_x = get_ber_by_points(points_x_orig_scaled, points_x_found, mod_type)
+        ber_y = get_ber_by_points(points_y_orig_scaled, points_y_found, mod_type)
         print("ber for x and y took",
               (datetime.now() - start_time).total_seconds() * 1000, "ms") if verbose >= 2 else ...
 
         q_x = np.sqrt(2) * sp.special.erfcinv(2 * ber_x[0])
         q_y = np.sqrt(2) * sp.special.erfcinv(2 * ber_y[0])
 
-        evm_x = get_evm(points_x_orig[k] * scale_constellation, points_x_shifted[k] * scale_constellation)
-        evm_y = get_evm(points_y_orig[k] * scale_constellation, points_y_shifted[k] * scale_constellation)
+        evm_x = get_evm(points_x_orig_scaled, points_x_shifted[k] * scale_constellation)
+        evm_y = get_evm(points_y_orig_scaled, points_y_shifted[k] * scale_constellation)
+
+        mi_x = calculate_mutual_information(points_x_orig_scaled, points_x_found[k])
+        mi_y = calculate_mutual_information(points_y_orig_scaled, points_y_found[k])
 
-        print("BER (x / y):", ber_x, ber_y) if verbose >= 1 else ...
-        print(r'Q^2-factor (x / y):', q_x, q_y) if verbose >= 1 else ...
+        print("BER (x / y):", ber_x[k], ber_y[k]) if verbose >= 1 else ...
+        print(r'Q^2-factor (x / y):', q_x[k], q_y[k]) if verbose >= 1 else ...
+        print(r'EVM (x / y):', evm_x[k], evm_y[k]) if verbose >= 1 else ...
+        print(r'MI (x / y):', mi_x[k], mi_y[k]) if verbose >= 1 else ...
 
     else:
         print('Error[full_line_model_wdm]: no such type of channels_type variable')
 
 
     if optimise == 'not':
 
@@ -610,25 +629,31 @@
             'points_y_shifted': points_y_shifted,
             'points_y_found': points_y_found,
             'ber_x': ber_x,
             'ber_y': ber_y,
             'q_x': q_x,
             'q_y': q_y,
             'evm_x': evm_x,
-            'evm_y': evm_y
+            'evm_y': evm_y,
+            'mi_x': mi_x,
+            'mi_y': mi_y
         }
 
     elif optimise == 'ber_x':
         return ber_x
     elif optimise == 'ber_y':
         return ber_y
     elif optimise == 'evm_x':
         return evm_x
     elif optimise == 'evm_y':
         return evm_y
+    elif optimise == 'mi_x':
+        return mi_x
+    elif optimise == 'mi_y':
+        return mi_y
     else:
         print('Error[full_line_model_wdm]: no such type of optimise variable')
         return None
 
     return result
```

### Comparing `hpcom-0.1.8/hpcom/hpcom_old.py` & `hpcom-0.1.9/hpcom/hpcom_old.py`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.8/hpcom/metrics.py` & `hpcom-0.1.9/hpcom/metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import numpy as np
 import scipy as sp
 
+# from ._sklearn_functions import crosstab, mutual_info_score
+from scipy.stats.contingency import crosstab
+from sklearn.metrics import mutual_info_score
+
 # from . import modulation
 # from hpcom.modulation import get_scale_coef, get_constellation, get_nearest_constellation_points_new, \
 #     get_bits_from_constellation_points
 from .modulation import get_scale_coef, get_constellation, get_nearest_constellation_points_new, \
     get_bits_from_constellation_points
 
+
 def get_energy(signal, dt):
     """
     Computes the energy of a signal.
 
     Args:
         signal: An array containing the signal.
         dt: The time step.
@@ -148,8 +153,18 @@
     scale_init = get_scale_coef(points_init, mod_type)
     return get_evm(points_init * scale_init, points * scale)
 
 
 def get_ber_from_evm(points_init, points, m):
     evm_rms = get_evm_rms_new(points_init, points)
     ber = 2 * (1. - np.power(m, -0.5)) / (np.log2(m)) * sp.special.erfc(np.sqrt(1.5 / ((m - 1) * np.power(evm_rms, 2))))
-    return ber
+    return ber
+
+
+def get_q_factor_from_ber(ber):
+    return np.sqrt(2) * sp.special.erfcinv(2 * ber)
+
+
+def calculate_mutual_information(x, y):
+    c_xy = crosstab(x, y)
+    mi = mutual_info_score(None, None, contingency=c_xy[1])
+    return mi
```

### Comparing `hpcom-0.1.8/hpcom/signal.py` & `hpcom-0.1.9/hpcom/signal.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,16 @@
     wdm['upsampling'] = upsampling
     wdm['downsampling_rate'] = downsampling_rate
     wdm['symb_freq'] = symb_freq
     wdm['sample_freq'] = int(symb_freq * upsampling)
     wdm['np_filter'] = np_filter
     wdm['p_ave'] = (10 ** (wdm['p_ave_dbm'] / 10)) / 1000
     wdm['seed'] = seed
+    wdm['scale_coef'] = get_scale_coef_constellation(wdm['modulation_type']) / \
+                        np.sqrt(wdm['p_ave'] / wdm['n_polarisations'])
 
     return wdm
 
 
 def get_default_wdm_parameters():
 
     wdm = {}
@@ -107,24 +109,28 @@
     wdm['symb_freq'] = 64e9  # GHz
     wdm['sample_freq'] = int(wdm['symb_freq'] * wdm['upsampling'])
     wdm['np_filter'] = 2 ** 12
     wdm['p_ave'] = (10 ** (wdm['p_ave_dbm'] / 10)) / 1000  # mW
     wdm['modulation_type'] = get_modulation_type_from_order(wdm['m_order'])
     wdm['n_bits_symbol'] = get_n_bits(wdm['modulation_type'])
     wdm['seed'] = 'fixed'
+    wdm['scale_coef'] = get_scale_coef_constellation(wdm['modulation_type']) / \
+                        np.sqrt(wdm['p_ave'] / wdm['n_polarisations'])
 
     return wdm
 
 
 def update_wdm_parameters(wdm):
 
     wdm['sample_freq'] = int(wdm['symb_freq'] * wdm['upsampling'])
     wdm['p_ave'] = (10 ** (wdm['p_ave_dbm'] / 10)) / 1000  # mW
     wdm['modulation_type'] = get_modulation_type_from_order(wdm['m_order'])
     wdm['n_bits_symbol'] = get_n_bits(wdm['modulation_type'])
+    wdm['scale_coef'] = get_scale_coef_constellation(wdm['modulation_type']) / \
+                        np.sqrt(wdm['p_ave'] / wdm['n_polarisations'])
 
     return wdm
 
 
 def update_wdm_parameters_from_json(json_file):
     # Load the JSON file as a dictionary
     with open(json_file, 'r') as f:
```

### Comparing `hpcom-0.1.8/hpcom.egg-info/PKG-INFO` & `hpcom-0.1.9/hpcom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpcom
-Version: 0.1.8
+Version: 0.1.9
 Summary: High performance optical communication library
 Author-email: Egor Sedov <e.sedov@g.nsu.ru>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hpcom-0.1.8/pyproject.toml` & `hpcom-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hpcom"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Egor Sedov", email="e.sedov@g.nsu.ru" },
 ]
 description = "High performance optical communication library"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `hpcom-0.1.8/tests/test_back_to_back.py` & `hpcom-0.1.9/tests/test_back_to_back.py`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.8/tests/test_channel_model.py` & `hpcom-0.1.9/tests/test_channel_model.py`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.8/tests/test_generation.py` & `hpcom-0.1.9/tests/test_generation.py`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.8/tests/test_ofdm_generation.py` & `hpcom-0.1.9/tests/test_ofdm_generation.py`

 * *Files identical despite different names*

### Comparing `hpcom-0.1.8/tests/test_propagation.py` & `hpcom-0.1.9/tests/test_propagation.py`

 * *Files identical despite different names*

