# Comparing `tmp/pyhydrophone-0.1.4.tar.gz` & `tmp/pyhydrophone-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyhydrophone-0.1.4.tar", last modified: Thu Jun  8 09:33:19 2023, max compression
+gzip compressed data, was "dist\pyhydrophone-0.1.5.tar", last modified: Wed Jul 19 10:09:43 2023, max compression
```

## Comparing `pyhydrophone-0.1.4.tar` & `pyhydrophone-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 09:33:19.000000 pyhydrophone-0.1.4/
--rw-rw-rw-   0        0        0    35823 2022-01-11 08:38:32.000000 pyhydrophone-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     6522 2023-06-08 09:33:19.000000 pyhydrophone-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     5016 2023-06-08 09:09:29.000000 pyhydrophone-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 09:33:19.000000 pyhydrophone-0.1.4/pyhydrophone/
--rw-rw-rw-   0        0        0      345 2022-11-23 08:43:01.000000 pyhydrophone-0.1.4/pyhydrophone/__init__.py
--rw-rw-rw-   0        0        0     2979 2022-02-01 08:48:19.000000 pyhydrophone-0.1.4/pyhydrophone/amar.py
--rw-rw-rw-   0        0        0     6112 2022-01-11 08:38:32.000000 pyhydrophone-0.1.4/pyhydrophone/bruelkjaer.py
--rw-rw-rw-   0        0        0     2091 2022-02-01 08:48:19.000000 pyhydrophone-0.1.4/pyhydrophone/ears.py
--rw-rw-rw-   0        0        0     4377 2022-02-04 13:20:07.000000 pyhydrophone-0.1.4/pyhydrophone/hydrophone.py
--rw-rw-rw-   0        0        0     2132 2022-11-23 08:32:21.000000 pyhydrophone-0.1.4/pyhydrophone/icListen.py
--rw-rw-rw-   0        0        0     1999 2022-02-01 08:48:19.000000 pyhydrophone-0.1.4/pyhydrophone/mte.py
--rw-rw-rw-   0        0        0    11405 2023-06-08 09:32:37.000000 pyhydrophone-0.1.4/pyhydrophone/rtsys.py
--rw-rw-rw-   0        0        0    13860 2023-06-02 14:38:03.000000 pyhydrophone-0.1.4/pyhydrophone/soundtrap.py
--rw-rw-rw-   0        0        0     2028 2022-02-01 08:48:19.000000 pyhydrophone-0.1.4/pyhydrophone/upam.py
-drwxrwxrwx   0        0        0        0 2023-06-08 09:33:19.000000 pyhydrophone-0.1.4/pyhydrophone.egg-info/
--rw-rw-rw-   0        0        0     6522 2023-06-08 09:33:19.000000 pyhydrophone-0.1.4/pyhydrophone.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-06-08 09:33:19.000000 pyhydrophone-0.1.4/pyhydrophone.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 09:33:19.000000 pyhydrophone-0.1.4/pyhydrophone.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-02-03 15:24:29.000000 pyhydrophone-0.1.4/pyhydrophone.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-06-08 09:33:19.000000 pyhydrophone-0.1.4/pyhydrophone.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      585 2023-06-08 09:33:19.000000 pyhydrophone-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      363 2023-06-08 09:25:01.000000 pyhydrophone-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:09:43.000000 pyhydrophone-0.1.5/
+-rw-rw-rw-   0        0        0    35823 2022-01-11 08:38:32.000000 pyhydrophone-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     8052 2023-07-19 10:09:43.000000 pyhydrophone-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6354 2023-06-21 13:50:06.000000 pyhydrophone-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 10:09:43.000000 pyhydrophone-0.1.5/pyhydrophone/
+-rw-rw-rw-   0        0        0      385 2023-06-21 07:26:59.000000 pyhydrophone-0.1.5/pyhydrophone/__init__.py
+-rw-rw-rw-   0        0        0     2979 2022-02-01 08:48:19.000000 pyhydrophone-0.1.5/pyhydrophone/amar.py
+-rw-rw-rw-   0        0        0     6112 2022-01-11 08:38:32.000000 pyhydrophone-0.1.5/pyhydrophone/bruelkjaer.py
+-rw-rw-rw-   0        0        0     2091 2022-02-01 08:48:19.000000 pyhydrophone-0.1.5/pyhydrophone/ears.py
+-rw-rw-rw-   0        0        0     4377 2022-02-04 13:20:07.000000 pyhydrophone-0.1.5/pyhydrophone/hydrophone.py
+-rw-rw-rw-   0        0        0     2132 2022-11-23 08:32:21.000000 pyhydrophone-0.1.5/pyhydrophone/icListen.py
+-rw-rw-rw-   0        0        0     1999 2022-02-01 08:48:19.000000 pyhydrophone-0.1.5/pyhydrophone/mte.py
+-rw-rw-rw-   0        0        0    11405 2023-07-19 10:07:41.000000 pyhydrophone-0.1.5/pyhydrophone/rtsys.py
+-rw-rw-rw-   0        0        0    13860 2023-06-02 14:38:03.000000 pyhydrophone-0.1.5/pyhydrophone/soundtrap.py
+-rw-rw-rw-   0        0        0     2129 2023-06-21 07:26:59.000000 pyhydrophone-0.1.5/pyhydrophone/uaural.py
+-rw-rw-rw-   0        0        0     2028 2022-02-01 08:48:19.000000 pyhydrophone-0.1.5/pyhydrophone/upam.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:09:43.000000 pyhydrophone-0.1.5/pyhydrophone.egg-info/
+-rw-rw-rw-   0        0        0     8052 2023-07-19 10:09:43.000000 pyhydrophone-0.1.5/pyhydrophone.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      473 2023-07-19 10:09:43.000000 pyhydrophone-0.1.5/pyhydrophone.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 10:09:43.000000 pyhydrophone-0.1.5/pyhydrophone.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-02-03 15:24:29.000000 pyhydrophone-0.1.5/pyhydrophone.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-07-19 10:09:43.000000 pyhydrophone-0.1.5/pyhydrophone.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      585 2023-07-19 10:09:43.000000 pyhydrophone-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      363 2023-07-19 10:09:05.000000 pyhydrophone-0.1.5/setup.py
```

### Comparing `pyhydrophone-0.1.4/LICENSE` & `pyhydrophone-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhydrophone-0.1.4/PKG-INFO` & `pyhydrophone-0.1.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhydrophone
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python scripts to read hydrophones files
 Home-page: https://github.com/lifewatch/pyhydrophone.git
 Author: Clea Parcerisas
 Author-email: clea.parcerisas@vliz.be
 License: UNKNOWN
 Description: # pyhydrophone
         
@@ -56,18 +56,39 @@
         and you would not have to worry about which format the file name has or where the information of the datetime is stored.
         
         
         
         For more information about the parameters that each hydrophone takes, see examples folder: 
         
         ```
-        upam = pyhy.uPam(name, model, sensitivity, preamp_gain)
         st = pyhy.SoundTrap(name, model, serial_number)
-        am = pyhy.AmarG3(name, model, sensitivity, preamp_gain, mems_sensitivity)
-        bk = pyhy.BruelKjaer(name, model, amplif)
+        
+        am = pyhy.AmarG3(name, model, sensitivity, preamp_gain, mems_sensitivity, Vpp)
+        
+        uaural = pyhy.uAural(sensitivity=-180, name='uAural', model='RX', serial_number=1, preamp_gain=12, Vpp=2.0)
+        
+        bk_test = pyhy.BruelKjaer(name=bk_name, model=bk_model, preamp_gain=preamp_gain, Vpp=bk_Vpp, serial_number=1,
+                                  type_signal='test')
+        bk_ref = pyhy.BruelKjaer(name=bk_name, model=bk_model, preamp_gain=preamp_gain, Vpp=bk_Vpp, serial_number=1,
+                                 type_signal='ref')
+        
+        upam = pyhy.uPam(name=upam_name, model=upam_name, serial_number=upam_serial_number,
+                         sensitivity=upam_sensitivity,
+                         preamp_gain=upam_preamp_gain, Vpp=upam_Vpp)
+        
+        aural = pyhy.MTE(name=aural_name, model=aural_model, serial_number=aural_serial_number,
+                         sensitivity=aural_sensitivity,
+                         preamp_gain=aural_preamp_gain, Vpp=aural_Vpp, string_format='%y%m%d_%H%M%S')
+        
+        rtsys = pyhy.RTSys(name=rtsys_name, model=rtsys_model, serial_number=serial_number,
+                           sensitivity=rtsys_sensitivity,
+                           preamp_gain=rtsys_preamp_gain, Vpp=rtsys_Vpp, mode='lowpower', channel='A')
+        
+        icListen = pyhy.icListen(name=icListen_name, model=icListen_model, serial_number=icListen_serial_number,
+                                 sensitivity=icListen_sensitivity, preamp_gain=icListen_preamp_gain, Vpp=icListen_Vpp)
         ```
         
         
         
         ### Hydrophone
         It is the base class, which can be used in case the user is only interested in keeping the parameters together. 
         
@@ -80,15 +101,15 @@
         They do not have to be specified by the user.
         (Gain type "High" or "Low" has to be specified).
         A routine for reading the xml file is provided (still some parameters missing).
         
         If the serial number is passed, the calibration information will automatically be obtained
         from http://oceaninstruments.azurewebsites.net/App/#/%23). 
         If when searching for your serial number there are multiple options, it is important that you specify the model of the 
-        hydrophone correctly (as listed in the calibration sheed in oceaninstruments) so the right calibration is selected.
+        hydrophone correctly (as listed in the calibration sheet in oceaninstruments) so the right calibration is selected.
         
         SoundTrapHF (inherited from SoundTrap) comes with a routine to read the *.dwv files from SoundTrap and store all the 
         high frequency clicks as a pandas df to be able to work with them. 
         
         A folder with several (xml, bcl, dwv) files can be specified and passed to the function.
         
         ### uPam
@@ -129,13 +150,16 @@
         
         ### MTE AURAL
         Just provides a method to read the date time from the name.
         http://www.multi-electronique.com/files/AURAL/user/AURAL-M2_USER_GUIDE.pdf
         
         ### icListen 
         In development. Just provides a method to read the date time from the name for the moment.
+        
+        ### uAural (micoAural)
+        In development. Just provides a method to read the date time from the name for the moment. 
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pyhydrophone-0.1.4/README.md` & `pyhydrophone-0.1.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -48,18 +48,39 @@
 and you would not have to worry about which format the file name has or where the information of the datetime is stored.
 
 
 
 For more information about the parameters that each hydrophone takes, see examples folder: 
 
 ```
-upam = pyhy.uPam(name, model, sensitivity, preamp_gain)
 st = pyhy.SoundTrap(name, model, serial_number)
-am = pyhy.AmarG3(name, model, sensitivity, preamp_gain, mems_sensitivity)
-bk = pyhy.BruelKjaer(name, model, amplif)
+
+am = pyhy.AmarG3(name, model, sensitivity, preamp_gain, mems_sensitivity, Vpp)
+
+uaural = pyhy.uAural(sensitivity=-180, name='uAural', model='RX', serial_number=1, preamp_gain=12, Vpp=2.0)
+
+bk_test = pyhy.BruelKjaer(name=bk_name, model=bk_model, preamp_gain=preamp_gain, Vpp=bk_Vpp, serial_number=1,
+                          type_signal='test')
+bk_ref = pyhy.BruelKjaer(name=bk_name, model=bk_model, preamp_gain=preamp_gain, Vpp=bk_Vpp, serial_number=1,
+                         type_signal='ref')
+
+upam = pyhy.uPam(name=upam_name, model=upam_name, serial_number=upam_serial_number,
+                 sensitivity=upam_sensitivity,
+                 preamp_gain=upam_preamp_gain, Vpp=upam_Vpp)
+
+aural = pyhy.MTE(name=aural_name, model=aural_model, serial_number=aural_serial_number,
+                 sensitivity=aural_sensitivity,
+                 preamp_gain=aural_preamp_gain, Vpp=aural_Vpp, string_format='%y%m%d_%H%M%S')
+
+rtsys = pyhy.RTSys(name=rtsys_name, model=rtsys_model, serial_number=serial_number,
+                   sensitivity=rtsys_sensitivity,
+                   preamp_gain=rtsys_preamp_gain, Vpp=rtsys_Vpp, mode='lowpower', channel='A')
+
+icListen = pyhy.icListen(name=icListen_name, model=icListen_model, serial_number=icListen_serial_number,
+                         sensitivity=icListen_sensitivity, preamp_gain=icListen_preamp_gain, Vpp=icListen_Vpp)
 ```
 
 
 
 ### Hydrophone
 It is the base class, which can be used in case the user is only interested in keeping the parameters together. 
 
@@ -72,15 +93,15 @@
 They do not have to be specified by the user.
 (Gain type "High" or "Low" has to be specified).
 A routine for reading the xml file is provided (still some parameters missing).
 
 If the serial number is passed, the calibration information will automatically be obtained
 from http://oceaninstruments.azurewebsites.net/App/#/%23). 
 If when searching for your serial number there are multiple options, it is important that you specify the model of the 
-hydrophone correctly (as listed in the calibration sheed in oceaninstruments) so the right calibration is selected.
+hydrophone correctly (as listed in the calibration sheet in oceaninstruments) so the right calibration is selected.
 
 SoundTrapHF (inherited from SoundTrap) comes with a routine to read the *.dwv files from SoundTrap and store all the 
 high frequency clicks as a pandas df to be able to work with them. 
 
 A folder with several (xml, bcl, dwv) files can be specified and passed to the function.
 
 ### uPam
@@ -120,8 +141,11 @@
 Just provides a method to read the date time from the name.
 
 ### MTE AURAL
 Just provides a method to read the date time from the name.
 http://www.multi-electronique.com/files/AURAL/user/AURAL-M2_USER_GUIDE.pdf
 
 ### icListen 
-In development. Just provides a method to read the date time from the name for the moment.
+In development. Just provides a method to read the date time from the name for the moment.
+
+### uAural (micoAural)
+In development. Just provides a method to read the date time from the name for the moment.
```

### Comparing `pyhydrophone-0.1.4/pyhydrophone/amar.py` & `pyhydrophone-0.1.5/pyhydrophone/amar.py`

 * *Files identical despite different names*

### Comparing `pyhydrophone-0.1.4/pyhydrophone/bruelkjaer.py` & `pyhydrophone-0.1.5/pyhydrophone/bruelkjaer.py`

 * *Files identical despite different names*

### Comparing `pyhydrophone-0.1.4/pyhydrophone/ears.py` & `pyhydrophone-0.1.5/pyhydrophone/ears.py`

 * *Files identical despite different names*

### Comparing `pyhydrophone-0.1.4/pyhydrophone/hydrophone.py` & `pyhydrophone-0.1.5/pyhydrophone/hydrophone.py`

 * *Files identical despite different names*

### Comparing `pyhydrophone-0.1.4/pyhydrophone/icListen.py` & `pyhydrophone-0.1.5/pyhydrophone/icListen.py`

 * *Files identical despite different names*

### Comparing `pyhydrophone-0.1.4/pyhydrophone/mte.py` & `pyhydrophone-0.1.5/pyhydrophone/mte.py`

 * *Files identical despite different names*

### Comparing `pyhydrophone-0.1.4/pyhydrophone/rtsys.py` & `pyhydrophone-0.1.5/pyhydrophone/rtsys.py`

 * *Files identical despite different names*

### Comparing `pyhydrophone-0.1.4/pyhydrophone/soundtrap.py` & `pyhydrophone-0.1.5/pyhydrophone/soundtrap.py`

 * *Files identical despite different names*

### Comparing `pyhydrophone-0.1.4/pyhydrophone/upam.py` & `pyhydrophone-0.1.5/pyhydrophone/upam.py`

 * *Files identical despite different names*

### Comparing `pyhydrophone-0.1.4/pyhydrophone.egg-info/PKG-INFO` & `pyhydrophone-0.1.5/pyhydrophone.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhydrophone
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python scripts to read hydrophones files
 Home-page: https://github.com/lifewatch/pyhydrophone.git
 Author: Clea Parcerisas
 Author-email: clea.parcerisas@vliz.be
 License: UNKNOWN
 Description: # pyhydrophone
         
@@ -56,18 +56,39 @@
         and you would not have to worry about which format the file name has or where the information of the datetime is stored.
         
         
         
         For more information about the parameters that each hydrophone takes, see examples folder: 
         
         ```
-        upam = pyhy.uPam(name, model, sensitivity, preamp_gain)
         st = pyhy.SoundTrap(name, model, serial_number)
-        am = pyhy.AmarG3(name, model, sensitivity, preamp_gain, mems_sensitivity)
-        bk = pyhy.BruelKjaer(name, model, amplif)
+        
+        am = pyhy.AmarG3(name, model, sensitivity, preamp_gain, mems_sensitivity, Vpp)
+        
+        uaural = pyhy.uAural(sensitivity=-180, name='uAural', model='RX', serial_number=1, preamp_gain=12, Vpp=2.0)
+        
+        bk_test = pyhy.BruelKjaer(name=bk_name, model=bk_model, preamp_gain=preamp_gain, Vpp=bk_Vpp, serial_number=1,
+                                  type_signal='test')
+        bk_ref = pyhy.BruelKjaer(name=bk_name, model=bk_model, preamp_gain=preamp_gain, Vpp=bk_Vpp, serial_number=1,
+                                 type_signal='ref')
+        
+        upam = pyhy.uPam(name=upam_name, model=upam_name, serial_number=upam_serial_number,
+                         sensitivity=upam_sensitivity,
+                         preamp_gain=upam_preamp_gain, Vpp=upam_Vpp)
+        
+        aural = pyhy.MTE(name=aural_name, model=aural_model, serial_number=aural_serial_number,
+                         sensitivity=aural_sensitivity,
+                         preamp_gain=aural_preamp_gain, Vpp=aural_Vpp, string_format='%y%m%d_%H%M%S')
+        
+        rtsys = pyhy.RTSys(name=rtsys_name, model=rtsys_model, serial_number=serial_number,
+                           sensitivity=rtsys_sensitivity,
+                           preamp_gain=rtsys_preamp_gain, Vpp=rtsys_Vpp, mode='lowpower', channel='A')
+        
+        icListen = pyhy.icListen(name=icListen_name, model=icListen_model, serial_number=icListen_serial_number,
+                                 sensitivity=icListen_sensitivity, preamp_gain=icListen_preamp_gain, Vpp=icListen_Vpp)
         ```
         
         
         
         ### Hydrophone
         It is the base class, which can be used in case the user is only interested in keeping the parameters together. 
         
@@ -80,15 +101,15 @@
         They do not have to be specified by the user.
         (Gain type "High" or "Low" has to be specified).
         A routine for reading the xml file is provided (still some parameters missing).
         
         If the serial number is passed, the calibration information will automatically be obtained
         from http://oceaninstruments.azurewebsites.net/App/#/%23). 
         If when searching for your serial number there are multiple options, it is important that you specify the model of the 
-        hydrophone correctly (as listed in the calibration sheed in oceaninstruments) so the right calibration is selected.
+        hydrophone correctly (as listed in the calibration sheet in oceaninstruments) so the right calibration is selected.
         
         SoundTrapHF (inherited from SoundTrap) comes with a routine to read the *.dwv files from SoundTrap and store all the 
         high frequency clicks as a pandas df to be able to work with them. 
         
         A folder with several (xml, bcl, dwv) files can be specified and passed to the function.
         
         ### uPam
@@ -129,13 +150,16 @@
         
         ### MTE AURAL
         Just provides a method to read the date time from the name.
         http://www.multi-electronique.com/files/AURAL/user/AURAL-M2_USER_GUIDE.pdf
         
         ### icListen 
         In development. Just provides a method to read the date time from the name for the moment.
+        
+        ### uAural (micoAural)
+        In development. Just provides a method to read the date time from the name for the moment. 
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pyhydrophone-0.1.4/setup.cfg` & `pyhydrophone-0.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7968 7964 726f 7068 6f6e 650d   = pyhydrophone.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e34  .version = 0.1.4
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e35  .version = 0.1.5
 00000030: 0d0a 6175 7468 6f72 203d 2043 6c65 6120  ..author = Clea 
 00000040: 5061 7263 6572 6973 6173 0d0a 6175 7468  Parcerisas..auth
 00000050: 6f72 5f65 6d61 696c 203d 2063 6c65 612e  or_email = clea.
 00000060: 7061 7263 6572 6973 6173 4076 6c69 7a2e  parcerisas@vliz.
 00000070: 6265 0d0a 6465 7363 7269 7074 696f 6e20  be..description 
 00000080: 3d20 5079 7468 6f6e 2073 6372 6970 7473  = Python scripts
 00000090: 2074 6f20 7265 6164 2068 7964 726f 7068   to read hydroph
```

