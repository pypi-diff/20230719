# Comparing `tmp/di2008-0.4.7-py3-none-any.whl.zip` & `tmp/di2008-0.4.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 11149 bytes, number of entries: 7
--rw-r--r--  2.0 unx      457 b- defN 22-May-13 14:00 di2008/__init__.py
--rw-r--r--  2.0 unx    30316 b- defN 22-May-13 14:00 di2008/instrument.py
--rw-r--r--  2.0 unx       22 b- defN 22-May-13 14:00 di2008/version.py
--rw-r--r--  2.0 unx     4349 b- defN 22-May-13 14:00 di2008-0.4.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-May-13 14:00 di2008-0.4.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 22-May-13 14:00 di2008-0.4.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      517 b- defN 22-May-13 14:00 di2008-0.4.7.dist-info/RECORD
-7 files, 35760 bytes uncompressed, 10237 bytes compressed:  71.4%
+Zip file size: 11256 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      457 b- defN 23-Jul-19 15:17 di2008/__init__.py
+-rw-r--r--  2.0 unx    30316 b- defN 23-Jul-19 15:17 di2008/instrument.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-19 15:17 di2008/version.py
+-rw-r--r--  2.0 unx     4549 b- defN 23-Jul-19 15:17 di2008-0.4.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-19 15:17 di2008-0.4.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-19 15:17 di2008-0.4.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      517 b- defN 23-Jul-19 15:17 di2008-0.4.8.dist-info/RECORD
+7 files, 35960 bytes uncompressed, 10344 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: di2008/instrument.py
 Comment: 
 
 Filename: di2008/version.py
 Comment: 
 
-Filename: di2008-0.4.7.dist-info/METADATA
+Filename: di2008-0.4.8.dist-info/METADATA
 Comment: 
 
-Filename: di2008-0.4.7.dist-info/WHEEL
+Filename: di2008-0.4.8.dist-info/WHEEL
 Comment: 
 
-Filename: di2008-0.4.7.dist-info/top_level.txt
+Filename: di2008-0.4.8.dist-info/top_level.txt
 Comment: 
 
-Filename: di2008-0.4.7.dist-info/RECORD
+Filename: di2008-0.4.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## di2008/instrument.py

```diff
@@ -48,15 +48,15 @@
 def _discover_by_esn(serial_number: str) -> 'usb.core.Device':
     buffering_time = 0.05
     correct_device = None
 
     available_devices = [d for d in usb.core.find(find_all=True,
                                                   idVendor=0x0683,
                                                   idProduct=0x2008,
-                                                  backend=libusb1.get_backend())]
+                                                  backend=libusb0.get_backend())]
     dev_strings = [str(d) for d in available_devices]
     _logger.debug(f'DI-2008 instruments detected on: {", ".join(dev_strings)}')
 
     for device in available_devices:
         _logger.info(f'checking candidate device "{device}"...')
         if correct_device is not None:
             break
```

## di2008/version.py

```diff
@@ -1 +1 @@
-__version__ = '0.4.7'
+__version__ = '0.4.8'
```

## Comparing `di2008-0.4.7.dist-info/METADATA` & `di2008-0.4.8.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: di2008
-Version: 0.4.7
+Version: 0.4.8
 Summary: Object-oriented API for DATAQ DI-2008
 Home-page: https://github.com/slightlynybbled/di2008
 Author: Jason R. Jones
 Author-email: slightlynybbled@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -31,24 +30,24 @@
 away the lowest-level functionality which may result in a hiding or loss of 
 feature implementation available in the hardware.  If this happens to you, feel 
 free to use the nuts and bolts exposed herein to inform your own development or, 
 better yet, send us a pull request!
 
 Check out the [documentation](https://slightlynybbled.github.io/di2008/)!
 
-# Installation
+## Installation
 
 The hardware drivers must be installed before this package may be utilized.  Hardware 
 drivers may be downloaded from the [manufacturer's product page](https://www.dataq.com/products/di-2008/).
 
 Once drivers are installed:
 
     $> pip install di2008
 
-# Project Status and Future
+## Project Status and Future
 
 The objects provided are tested and demonstrated to function well, however, there are still some features that have not been implemented.
 
 Items marked out have already been completed.  The list is in approximate order of priority and marked out items have been completed.
 
  * ~~Implement Analog Scan List~~ complete
  * ~~Read Thermocouples~~ complete
@@ -57,31 +56,39 @@
  * Read Event Input
  * Read Counter Input
  * ~~Read Digital Input(s)~~ complete
  * ~~Write to Digital Outputs~~ complete
  * Better sample hardware timing control
  * Hardware Synchronization
 
-# Usage
+## Usage
 
 Regarding the specifics of usage, it may be very helpful for the user to read the device documentation so that some of the concepts enshrined herein are more precisely interpreted.  Specifically, the concept of a "scan list" is somewhat unique to the product and difficult to abstract.  As the project matures, more of the hardware idiosyncrasies are expected to be exposed to the user.
 
-## Hardware Setup
+## Deployment
+
+When deploying using `pyinstaller` in a windows environment, the `pyusb` library doesn't
+play well with `libusb-1.0.dll`, so you will need to package `libusb0.dll` into your
+pyinsteller `*.spec` file using the following line:
+
+    datas=[('C:\\Windows\\System32\\libusb0.dll', '.'),],
+
+### Hardware Setup
 
 Place device into 'USB' mode, not COM mode!!!
 
  1. Disconnect from USB
  2. Wait 5 seconds
  3. Connect to USB and press button on side rapidly until LED changes
  
 The device setting is persistent and will not need to be changed again.  
 If you see a COM port in your device manager with the label `DATAQ DI-2008` 
 then the device is NOT in the correct mode!
 
-## Software Setup
+### Software Setup
 
 To read a few analog inputs, device setup is relatively simple.
 
  1. Define the ports
  2. Create the `Di2008` instance
  3. Add the scan list
  4. Start the scanning process
@@ -108,13 +115,7 @@
         print(f'{an0.value:.02f}')
         print(f'{an1.value:.02f}')
         print(f'{an2.value:.02f}')
         print(f'{rate.value:.02f}')
         print()
         
         sleep(1.0)
-        
-# Contributions
-
-Project could use some work, particularly in documentation.
-
-
```

## Comparing `di2008-0.4.7.dist-info/RECORD` & `di2008-0.4.8.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 di2008/__init__.py,sha256=3H1uz7Hsrjo0mVPsvbhIY0-mkFOvRbo1PVumBj5FM0Y,457
-di2008/instrument.py,sha256=2cpLZtlLsAUhiC7ekGKcH4HsKW-2aXvSxDgiVoVvxCU,30316
-di2008/version.py,sha256=UmVafZY7kcXtTkcxANj_olsrrxex9xg7OUKA4sTbnN8,22
-di2008-0.4.7.dist-info/METADATA,sha256=YJNYnZP5dUmfFGeOJY1fLUEN2nHVm63NbB0-ooCA824,4349
-di2008-0.4.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-di2008-0.4.7.dist-info/top_level.txt,sha256=748Xjf7h2N5jlZ5xxobun8xk-UNMJkjV8Wa-Oj79Om8,7
-di2008-0.4.7.dist-info/RECORD,,
+di2008/instrument.py,sha256=8wBUb-gox7K-F2apiEcssWuPxBZwBOfD_FwWXKwa3_g,30316
+di2008/version.py,sha256=QYyML8JANUWyfBi9eNLi2Hyi1YO-e89h9bGB3Ng0Suo,22
+di2008-0.4.8.dist-info/METADATA,sha256=t7LDtNu17T0ArDImW-GxbSQcoXj45485PbE5Gu8khHk,4549
+di2008-0.4.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+di2008-0.4.8.dist-info/top_level.txt,sha256=748Xjf7h2N5jlZ5xxobun8xk-UNMJkjV8Wa-Oj79Om8,7
+di2008-0.4.8.dist-info/RECORD,,
```

