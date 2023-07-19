# Comparing `tmp/iimcsim-0.1.0.tar.gz` & `tmp/iimcsim-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iimcsim-0.1.0.tar", last modified: Tue Jul 18 20:04:16 2023, max compression
+gzip compressed data, was "iimcsim-0.1.1.tar", last modified: Tue Jul 18 20:09:29 2023, max compression
```

## Comparing `iimcsim-0.1.0.tar` & `iimcsim-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 20:04:16.117699 iimcsim-0.1.0/
--rw-rw-rw-   0        0        0        0 2023-05-19 11:56:01.000000 iimcsim-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     5298 2023-07-18 20:04:16.118697 iimcsim-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4628 2023-07-18 20:03:27.000000 iimcsim-0.1.0/README.md
--rw-rw-rw-   0        0        0      108 2023-05-19 11:57:59.000000 iimcsim-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      747 2023-07-18 20:04:16.129667 iimcsim-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-18 20:04:16.042900 iimcsim-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-18 20:04:16.077808 iimcsim-0.1.0/src/iimcsim/
--rw-rw-rw-   0        0        0     2290 2023-05-22 07:22:39.000000 iimcsim-0.1.0/src/iimcsim/MC.py
--rw-rw-rw-   0        0        0    11861 2023-06-20 08:51:34.000000 iimcsim-0.1.0/src/iimcsim/MonteCarlo.py
--rw-rw-rw-   0        0        0        0 2023-05-19 11:37:00.000000 iimcsim-0.1.0/src/iimcsim/__init__.py
--rw-rw-rw-   0        0        0     4581 2023-05-19 19:30:36.000000 iimcsim-0.1.0/src/iimcsim/data_gen.py
--rw-rw-rw-   0        0        0      661 2023-07-18 15:21:44.000000 iimcsim-0.1.0/src/iimcsim/data_gen_run.py
--rw-rw-rw-   0        0        0     2392 2023-07-18 16:06:09.000000 iimcsim-0.1.0/src/iimcsim/eda.py
--rw-rw-rw-   0        0        0     2698 2023-07-18 17:05:44.000000 iimcsim-0.1.0/src/iimcsim/shape_ext.py
--rw-rw-rw-   0        0        0    17269 2023-05-19 11:37:01.000000 iimcsim-0.1.0/src/iimcsim/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-18 20:04:16.111715 iimcsim-0.1.0/src/iimcsim.egg-info/
--rw-rw-rw-   0        0        0     5298 2023-07-18 20:04:16.000000 iimcsim-0.1.0/src/iimcsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-07-18 20:04:16.000000 iimcsim-0.1.0/src/iimcsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 20:04:16.000000 iimcsim-0.1.0/src/iimcsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-18 20:04:16.000000 iimcsim-0.1.0/src/iimcsim.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-18 20:04:16.114707 iimcsim-0.1.0/tests/
--rw-rw-rw-   0        0        0      951 2023-07-18 16:07:30.000000 iimcsim-0.1.0/tests/test_mc.py
+drwxrwxrwx   0        0        0        0 2023-07-18 20:09:29.478040 iimcsim-0.1.1/
+-rw-rw-rw-   0        0        0        0 2023-05-19 11:56:01.000000 iimcsim-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5197 2023-07-18 20:09:29.479037 iimcsim-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4527 2023-07-18 20:09:11.000000 iimcsim-0.1.1/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-19 11:57:59.000000 iimcsim-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      747 2023-07-18 20:09:29.481032 iimcsim-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 20:09:29.412217 iimcsim-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 20:09:29.449118 iimcsim-0.1.1/src/iimcsim/
+-rw-rw-rw-   0        0        0     2290 2023-05-22 07:22:39.000000 iimcsim-0.1.1/src/iimcsim/MC.py
+-rw-rw-rw-   0        0        0    11861 2023-06-20 08:51:34.000000 iimcsim-0.1.1/src/iimcsim/MonteCarlo.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 11:37:00.000000 iimcsim-0.1.1/src/iimcsim/__init__.py
+-rw-rw-rw-   0        0        0     4581 2023-05-19 19:30:36.000000 iimcsim-0.1.1/src/iimcsim/data_gen.py
+-rw-rw-rw-   0        0        0      661 2023-07-18 15:21:44.000000 iimcsim-0.1.1/src/iimcsim/data_gen_run.py
+-rw-rw-rw-   0        0        0     2392 2023-07-18 16:06:09.000000 iimcsim-0.1.1/src/iimcsim/eda.py
+-rw-rw-rw-   0        0        0     2698 2023-07-18 17:05:44.000000 iimcsim-0.1.1/src/iimcsim/shape_ext.py
+-rw-rw-rw-   0        0        0    17269 2023-05-19 11:37:01.000000 iimcsim-0.1.1/src/iimcsim/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-18 20:09:29.470062 iimcsim-0.1.1/src/iimcsim.egg-info/
+-rw-rw-rw-   0        0        0     5197 2023-07-18 20:09:29.000000 iimcsim-0.1.1/src/iimcsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-07-18 20:09:29.000000 iimcsim-0.1.1/src/iimcsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 20:09:29.000000 iimcsim-0.1.1/src/iimcsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-18 20:09:29.000000 iimcsim-0.1.1/src/iimcsim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 20:09:29.475048 iimcsim-0.1.1/tests/
+-rw-rw-rw-   0        0        0      951 2023-07-18 16:07:30.000000 iimcsim-0.1.1/tests/test_mc.py
```

### Comparing `iimcsim-0.1.0/PKG-INFO` & `iimcsim-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iimcsim
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for Monte-Carlo simulation for Intensity Interferometry
 Home-page: https://github.com/jigar2099/photon_position_reconstruction/tree/main
 Author: Jigar Bhanderi
 Author-email: jigarbhanderi@gmail.com
 Project-URL: Bug Tracker, https://github.com/jigar2099/photon_position_reconstruction/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -41,36 +41,36 @@
     - Then one needs to mention number of example samples to be generated for each selected rate. This creates balanced dataset, and helps to avoide biased scenario for training.
     - Finally, in the output, MC provides two types of data
         1. Input data: consists of added pulses
         2. Lable data: consists number of pulses added, for example fully added pulse/s are represented by integer values, while float value indicates sliced pulses, which are mainly cases closer to the edges of the sample.
     - A single run of simulation produces single dataset. Therefore, one needs to use it three times for training data, testing data and validation data.
 2. Double channel MC simulation : This simulation is created in order to mimic the data geretated from the two PMTs used in the experiment. It generates single channel data first, and then in second channel data generation, it randomly determines correlated pulse positions in both channels and add the pulse into second channel data, while rest of the pulse positions could be uncorrelated. In this way, it applies the consideration of correlation from entire range of selected rates.
 ### How to use 
-'''ruby
+```ruby
 import iimcsim.data_gen_run as dg
 dg.data_gen_run().generate_data(train_exe = 50,
-                    name = r"C:\Users\jigar\Downloads\photon_position_reconstruction-main\photon_position_reconstruction-main\src\data\plateauless_uniq_pulses_2345.npy",
+                    name = r"C:\photon_position_reconstruction-main\main\src\data\plateauless_uniq_pulses_2345.npy",
                     samp_size = 256,
                     max_num_photon = 90,
                     folder_name = 'sh06x2')
-'''
+```
 
 #### sample generation
-'''
+```ruby
 import iimcsim.shape_ext as sh_ext
 shapes = sh_ext.shape_generator(
-                        calib_file=r"C:\Users\calib_ch0.npy",
+                        calib_file=r"C:\calib_ch0.npy",
                         high_rate_file = r"C:\Usersn\shaula_00000-003_ch0.npy",
-                        path_to_save='C:\\Users\\reconstruction-main\\photon_position_reconstruction-main\\notebooks\\',
+                        path_to_save='C:\\Usestruction-main\\notebooks\\',
 )
 x1=shapes.generator(threshold=0, bin_num=2147483600)
-'''
+```
 
 #### Data analysis
 
-'''ruby
+```ruby
 from iimcsim.tools import pulse_height, pulse_width, pulse_kurtosis, pulse_skewness
 pulse_height(x1)
 pulse_width(x1)
 pulse_kurtosis(x1)
 pulse_skewness(x1)
-'''
+```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iimcsim Version: 0.1.0 Summary: A package for
+Metadata-Version: 2.1 Name: iimcsim Version: 0.1.1 Summary: A package for
 Monte-Carlo simulation for Intensity Interferometry Home-page: https://
 github.com/jigar2099/photon_position_reconstruction/tree/main Author: Jigar
 Bhanderi Author-email: jigarbhanderi@gmail.com Project-URL: Bug Tracker, https:
 //github.com/jigar2099/photon_position_reconstruction/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # Photon Position
@@ -47,20 +47,18 @@
 times for training data, testing data and validation data. 2. Double channel MC
 simulation : This simulation is created in order to mimic the data geretated
 from the two PMTs used in the experiment. It generates single channel data
 first, and then in second channel data generation, it randomly determines
 correlated pulse positions in both channels and add the pulse into second
 channel data, while rest of the pulse positions could be uncorrelated. In this
 way, it applies the consideration of correlation from entire range of selected
-rates. ### How to use '''ruby import iimcsim.data_gen_run as dg dg.data_gen_run
-().generate_data(train_exe = 50, name = r"C:
-\Users\jigar\Downloads\photon_position_reconstruction-
-main\photon_position_reconstruction-
-main\src\data\plateauless_uniq_pulses_2345.npy", samp_size = 256,
-max_num_photon = 90, folder_name = 'sh06x2') ''' #### sample generation '''
+rates. ### How to use ```ruby import iimcsim.data_gen_run as dg dg.data_gen_run
+().generate_data(train_exe = 50, name = r"C:\photon_position_reconstruction-
+main\main\src\data\plateauless_uniq_pulses_2345.npy", samp_size = 256,
+max_num_photon = 90, folder_name = 'sh06x2') ``` #### sample generation ```ruby
 import iimcsim.shape_ext as sh_ext shapes = sh_ext.shape_generator
-( calib_file=r"C:\Users\calib_ch0.npy", high_rate_file = r"C:
-\Usersn\shaula_00000-003_ch0.npy", path_to_save='C:\\Users\\reconstruction-
-main\\photon_position_reconstruction-main\\notebooks\\', ) x1=shapes.generator
-(threshold=0, bin_num=2147483600) ''' #### Data analysis '''ruby from
-iimcsim.tools import pulse_height, pulse_width, pulse_kurtosis, pulse_skewness
-pulse_height(x1) pulse_width(x1) pulse_kurtosis(x1) pulse_skewness(x1) '''
+( calib_file=r"C:\calib_ch0.npy", high_rate_file = r"C:\Usersn\shaula_00000-
+003_ch0.npy", path_to_save='C:\\Usestruction-main\\notebooks\\', )
+x1=shapes.generator(threshold=0, bin_num=2147483600) ``` #### Data analysis
+```ruby from iimcsim.tools import pulse_height, pulse_width, pulse_kurtosis,
+pulse_skewness pulse_height(x1) pulse_width(x1) pulse_kurtosis(x1)
+pulse_skewness(x1) ```
```

### Comparing `iimcsim-0.1.0/README.md` & `iimcsim-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -26,36 +26,36 @@
     - Then one needs to mention number of example samples to be generated for each selected rate. This creates balanced dataset, and helps to avoide biased scenario for training.
     - Finally, in the output, MC provides two types of data
         1. Input data: consists of added pulses
         2. Lable data: consists number of pulses added, for example fully added pulse/s are represented by integer values, while float value indicates sliced pulses, which are mainly cases closer to the edges of the sample.
     - A single run of simulation produces single dataset. Therefore, one needs to use it three times for training data, testing data and validation data.
 2. Double channel MC simulation : This simulation is created in order to mimic the data geretated from the two PMTs used in the experiment. It generates single channel data first, and then in second channel data generation, it randomly determines correlated pulse positions in both channels and add the pulse into second channel data, while rest of the pulse positions could be uncorrelated. In this way, it applies the consideration of correlation from entire range of selected rates.
 ### How to use 
-'''ruby
+```ruby
 import iimcsim.data_gen_run as dg
 dg.data_gen_run().generate_data(train_exe = 50,
-                    name = r"C:\Users\jigar\Downloads\photon_position_reconstruction-main\photon_position_reconstruction-main\src\data\plateauless_uniq_pulses_2345.npy",
+                    name = r"C:\photon_position_reconstruction-main\main\src\data\plateauless_uniq_pulses_2345.npy",
                     samp_size = 256,
                     max_num_photon = 90,
                     folder_name = 'sh06x2')
-'''
+```
 
 #### sample generation
-'''
+```ruby
 import iimcsim.shape_ext as sh_ext
 shapes = sh_ext.shape_generator(
-                        calib_file=r"C:\Users\calib_ch0.npy",
+                        calib_file=r"C:\calib_ch0.npy",
                         high_rate_file = r"C:\Usersn\shaula_00000-003_ch0.npy",
-                        path_to_save='C:\\Users\\reconstruction-main\\photon_position_reconstruction-main\\notebooks\\',
+                        path_to_save='C:\\Usestruction-main\\notebooks\\',
 )
 x1=shapes.generator(threshold=0, bin_num=2147483600)
-'''
+```
 
 #### Data analysis
 
-'''ruby
+```ruby
 from iimcsim.tools import pulse_height, pulse_width, pulse_kurtosis, pulse_skewness
 pulse_height(x1)
 pulse_width(x1)
 pulse_kurtosis(x1)
 pulse_skewness(x1)
-'''
+```
```

#### html2text {}

```diff
@@ -39,20 +39,19 @@
 dataset. Therefore, one needs to use it three times for training data, testing
 data and validation data. 2. Double channel MC simulation : This simulation is
 created in order to mimic the data geretated from the two PMTs used in the
 experiment. It generates single channel data first, and then in second channel
 data generation, it randomly determines correlated pulse positions in both
 channels and add the pulse into second channel data, while rest of the pulse
 positions could be uncorrelated. In this way, it applies the consideration of
-correlation from entire range of selected rates. ### How to use '''ruby import
+correlation from entire range of selected rates. ### How to use ```ruby import
 iimcsim.data_gen_run as dg dg.data_gen_run().generate_data(train_exe = 50, name
-= r"C:\Users\jigar\Downloads\photon_position_reconstruction-
-main\photon_position_reconstruction-
-main\src\data\plateauless_uniq_pulses_2345.npy", samp_size = 256,
-max_num_photon = 90, folder_name = 'sh06x2') ''' #### sample generation '''
+= r"C:\photon_position_reconstruction-
+main\main\src\data\plateauless_uniq_pulses_2345.npy", samp_size = 256,
+max_num_photon = 90, folder_name = 'sh06x2') ``` #### sample generation ```ruby
 import iimcsim.shape_ext as sh_ext shapes = sh_ext.shape_generator
-( calib_file=r"C:\Users\calib_ch0.npy", high_rate_file = r"C:
-\Usersn\shaula_00000-003_ch0.npy", path_to_save='C:\\Users\\reconstruction-
-main\\photon_position_reconstruction-main\\notebooks\\', ) x1=shapes.generator
-(threshold=0, bin_num=2147483600) ''' #### Data analysis '''ruby from
-iimcsim.tools import pulse_height, pulse_width, pulse_kurtosis, pulse_skewness
-pulse_height(x1) pulse_width(x1) pulse_kurtosis(x1) pulse_skewness(x1) '''
+( calib_file=r"C:\calib_ch0.npy", high_rate_file = r"C:\Usersn\shaula_00000-
+003_ch0.npy", path_to_save='C:\\Usestruction-main\\notebooks\\', )
+x1=shapes.generator(threshold=0, bin_num=2147483600) ``` #### Data analysis
+```ruby from iimcsim.tools import pulse_height, pulse_width, pulse_kurtosis,
+pulse_skewness pulse_height(x1) pulse_width(x1) pulse_kurtosis(x1)
+pulse_skewness(x1) ```
```

### Comparing `iimcsim-0.1.0/setup.cfg` & `iimcsim-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 696d 6373 696d 0d0a 7665 7273   = iimcsim..vers
-00000020: 696f 6e20 3d20 302e 312e 300d 0a61 7574  ion = 0.1.0..aut
+00000020: 696f 6e20 3d20 302e 312e 310d 0a61 7574  ion = 0.1.1..aut
 00000030: 686f 7220 3d20 4a69 6761 7220 4268 616e  hor = Jigar Bhan
 00000040: 6465 7269 0d0a 6175 7468 6f72 5f65 6d61  deri..author_ema
 00000050: 696c 203d 206a 6967 6172 6268 616e 6465  il = jigarbhande
 00000060: 7269 4067 6d61 696c 2e63 6f6d 0d0a 6465  ri@gmail.com..de
 00000070: 7363 7269 7074 696f 6e20 3d20 4120 7061  scription = A pa
 00000080: 636b 6167 6520 666f 7220 4d6f 6e74 652d  ckage for Monte-
 00000090: 4361 726c 6f20 7369 6d75 6c61 7469 6f6e  Carlo simulation
```

### Comparing `iimcsim-0.1.0/src/iimcsim/MC.py` & `iimcsim-0.1.1/src/iimcsim/MC.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.1.0/src/iimcsim/MonteCarlo.py` & `iimcsim-0.1.1/src/iimcsim/MonteCarlo.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.1.0/src/iimcsim/data_gen.py` & `iimcsim-0.1.1/src/iimcsim/data_gen.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.1.0/src/iimcsim/data_gen_run.py` & `iimcsim-0.1.1/src/iimcsim/data_gen_run.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.1.0/src/iimcsim/eda.py` & `iimcsim-0.1.1/src/iimcsim/eda.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.1.0/src/iimcsim/shape_ext.py` & `iimcsim-0.1.1/src/iimcsim/shape_ext.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.1.0/src/iimcsim/tools.py` & `iimcsim-0.1.1/src/iimcsim/tools.py`

 * *Files identical despite different names*

### Comparing `iimcsim-0.1.0/src/iimcsim.egg-info/PKG-INFO` & `iimcsim-0.1.1/src/iimcsim.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iimcsim
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for Monte-Carlo simulation for Intensity Interferometry
 Home-page: https://github.com/jigar2099/photon_position_reconstruction/tree/main
 Author: Jigar Bhanderi
 Author-email: jigarbhanderi@gmail.com
 Project-URL: Bug Tracker, https://github.com/jigar2099/photon_position_reconstruction/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -41,36 +41,36 @@
     - Then one needs to mention number of example samples to be generated for each selected rate. This creates balanced dataset, and helps to avoide biased scenario for training.
     - Finally, in the output, MC provides two types of data
         1. Input data: consists of added pulses
         2. Lable data: consists number of pulses added, for example fully added pulse/s are represented by integer values, while float value indicates sliced pulses, which are mainly cases closer to the edges of the sample.
     - A single run of simulation produces single dataset. Therefore, one needs to use it three times for training data, testing data and validation data.
 2. Double channel MC simulation : This simulation is created in order to mimic the data geretated from the two PMTs used in the experiment. It generates single channel data first, and then in second channel data generation, it randomly determines correlated pulse positions in both channels and add the pulse into second channel data, while rest of the pulse positions could be uncorrelated. In this way, it applies the consideration of correlation from entire range of selected rates.
 ### How to use 
-'''ruby
+```ruby
 import iimcsim.data_gen_run as dg
 dg.data_gen_run().generate_data(train_exe = 50,
-                    name = r"C:\Users\jigar\Downloads\photon_position_reconstruction-main\photon_position_reconstruction-main\src\data\plateauless_uniq_pulses_2345.npy",
+                    name = r"C:\photon_position_reconstruction-main\main\src\data\plateauless_uniq_pulses_2345.npy",
                     samp_size = 256,
                     max_num_photon = 90,
                     folder_name = 'sh06x2')
-'''
+```
 
 #### sample generation
-'''
+```ruby
 import iimcsim.shape_ext as sh_ext
 shapes = sh_ext.shape_generator(
-                        calib_file=r"C:\Users\calib_ch0.npy",
+                        calib_file=r"C:\calib_ch0.npy",
                         high_rate_file = r"C:\Usersn\shaula_00000-003_ch0.npy",
-                        path_to_save='C:\\Users\\reconstruction-main\\photon_position_reconstruction-main\\notebooks\\',
+                        path_to_save='C:\\Usestruction-main\\notebooks\\',
 )
 x1=shapes.generator(threshold=0, bin_num=2147483600)
-'''
+```
 
 #### Data analysis
 
-'''ruby
+```ruby
 from iimcsim.tools import pulse_height, pulse_width, pulse_kurtosis, pulse_skewness
 pulse_height(x1)
 pulse_width(x1)
 pulse_kurtosis(x1)
 pulse_skewness(x1)
-'''
+```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iimcsim Version: 0.1.0 Summary: A package for
+Metadata-Version: 2.1 Name: iimcsim Version: 0.1.1 Summary: A package for
 Monte-Carlo simulation for Intensity Interferometry Home-page: https://
 github.com/jigar2099/photon_position_reconstruction/tree/main Author: Jigar
 Bhanderi Author-email: jigarbhanderi@gmail.com Project-URL: Bug Tracker, https:
 //github.com/jigar2099/photon_position_reconstruction/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # Photon Position
@@ -47,20 +47,18 @@
 times for training data, testing data and validation data. 2. Double channel MC
 simulation : This simulation is created in order to mimic the data geretated
 from the two PMTs used in the experiment. It generates single channel data
 first, and then in second channel data generation, it randomly determines
 correlated pulse positions in both channels and add the pulse into second
 channel data, while rest of the pulse positions could be uncorrelated. In this
 way, it applies the consideration of correlation from entire range of selected
-rates. ### How to use '''ruby import iimcsim.data_gen_run as dg dg.data_gen_run
-().generate_data(train_exe = 50, name = r"C:
-\Users\jigar\Downloads\photon_position_reconstruction-
-main\photon_position_reconstruction-
-main\src\data\plateauless_uniq_pulses_2345.npy", samp_size = 256,
-max_num_photon = 90, folder_name = 'sh06x2') ''' #### sample generation '''
+rates. ### How to use ```ruby import iimcsim.data_gen_run as dg dg.data_gen_run
+().generate_data(train_exe = 50, name = r"C:\photon_position_reconstruction-
+main\main\src\data\plateauless_uniq_pulses_2345.npy", samp_size = 256,
+max_num_photon = 90, folder_name = 'sh06x2') ``` #### sample generation ```ruby
 import iimcsim.shape_ext as sh_ext shapes = sh_ext.shape_generator
-( calib_file=r"C:\Users\calib_ch0.npy", high_rate_file = r"C:
-\Usersn\shaula_00000-003_ch0.npy", path_to_save='C:\\Users\\reconstruction-
-main\\photon_position_reconstruction-main\\notebooks\\', ) x1=shapes.generator
-(threshold=0, bin_num=2147483600) ''' #### Data analysis '''ruby from
-iimcsim.tools import pulse_height, pulse_width, pulse_kurtosis, pulse_skewness
-pulse_height(x1) pulse_width(x1) pulse_kurtosis(x1) pulse_skewness(x1) '''
+( calib_file=r"C:\calib_ch0.npy", high_rate_file = r"C:\Usersn\shaula_00000-
+003_ch0.npy", path_to_save='C:\\Usestruction-main\\notebooks\\', )
+x1=shapes.generator(threshold=0, bin_num=2147483600) ``` #### Data analysis
+```ruby from iimcsim.tools import pulse_height, pulse_width, pulse_kurtosis,
+pulse_skewness pulse_height(x1) pulse_width(x1) pulse_kurtosis(x1)
+pulse_skewness(x1) ```
```

### Comparing `iimcsim-0.1.0/tests/test_mc.py` & `iimcsim-0.1.1/tests/test_mc.py`

 * *Files identical despite different names*

