# Comparing `tmp/xgo-pythonlib-0.2.4.tar.gz` & `tmp/xgo-pythonlib-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgo-pythonlib-0.2.4.tar", last modified: Thu Jul 13 03:16:22 2023, max compression
+gzip compressed data, was "xgo-pythonlib-0.2.5.tar", last modified: Wed Jul 19 04:35:19 2023, max compression
```

## Comparing `xgo-pythonlib-0.2.4.tar` & `xgo-pythonlib-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 03:16:22.333249 xgo-pythonlib-0.2.4/
--rw-rw-rw-   0        0        0     2490 2023-07-13 03:16:22.333249 xgo-pythonlib-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1863 2023-07-04 13:33:41.000000 xgo-pythonlib-0.2.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-13 03:16:22.333249 xgo-pythonlib-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     3744 2023-07-13 03:16:10.000000 xgo-pythonlib-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 03:16:22.323589 xgo-pythonlib-0.2.4/xgo_pythonlib.egg-info/
--rw-rw-rw-   0        0        0     2490 2023-07-13 03:16:22.000000 xgo-pythonlib-0.2.4/xgo_pythonlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-07-13 03:16:22.000000 xgo-pythonlib-0.2.4/xgo_pythonlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 03:16:22.000000 xgo-pythonlib-0.2.4/xgo_pythonlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-13 03:16:22.000000 xgo-pythonlib-0.2.4/xgo_pythonlib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-13 03:16:22.325587 xgo-pythonlib-0.2.4/xgoedu/
--rw-rw-rw-   0        0        0    49547 2023-07-13 03:15:23.000000 xgo-pythonlib-0.2.4/xgoedu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 03:16:22.326587 xgo-pythonlib-0.2.4/xgolib/
--rw-rw-rw-   0        0        0    26390 2023-06-19 03:02:36.000000 xgo-pythonlib-0.2.4/xgolib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 03:16:22.331250 xgo-pythonlib-0.2.4/xgoscreen/
--rw-rw-rw-   0        0        0     5339 2023-06-07 11:44:32.000000 xgo-pythonlib-0.2.4/xgoscreen/LCD_2inch.py
--rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.2.4/xgoscreen/__init__.py
--rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.2.4/xgoscreen/lcdconfig.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:35:19.873250 xgo-pythonlib-0.2.5/
+-rw-rw-rw-   0        0        0     2727 2023-07-19 04:35:19.872251 xgo-pythonlib-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2100 2023-07-19 04:33:55.000000 xgo-pythonlib-0.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-19 04:35:19.874251 xgo-pythonlib-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     3744 2023-07-19 04:34:29.000000 xgo-pythonlib-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:35:19.854251 xgo-pythonlib-0.2.5/xgo_pythonlib.egg-info/
+-rw-rw-rw-   0        0        0     2727 2023-07-19 04:35:19.000000 xgo-pythonlib-0.2.5/xgo_pythonlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-07-19 04:35:19.000000 xgo-pythonlib-0.2.5/xgo_pythonlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 04:35:19.000000 xgo-pythonlib-0.2.5/xgo_pythonlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-19 04:35:19.000000 xgo-pythonlib-0.2.5/xgo_pythonlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 04:35:19.856254 xgo-pythonlib-0.2.5/xgoedu/
+-rw-rw-rw-   0        0        0    49547 2023-07-13 03:15:23.000000 xgo-pythonlib-0.2.5/xgoedu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:35:19.859250 xgo-pythonlib-0.2.5/xgolib/
+-rw-rw-rw-   0        0        0    26358 2023-07-19 04:33:55.000000 xgo-pythonlib-0.2.5/xgolib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:35:19.869249 xgo-pythonlib-0.2.5/xgoscreen/
+-rw-rw-rw-   0        0        0     5339 2023-06-07 11:44:32.000000 xgo-pythonlib-0.2.5/xgoscreen/LCD_2inch.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.2.5/xgoscreen/__init__.py
+-rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.2.5/xgoscreen/lcdconfig.py
```

### Comparing `xgo-pythonlib-0.2.4/PKG-INFO` & `xgo-pythonlib-0.2.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: xgo-pythonlib
-Version: 0.2.4
-Summary: PythonLib for XGO2-DOG
-Home-page: https://github.com/Xgorobot/XGO-PythonLib
-Author: luwudynamics
-Author-email: hello@xgorobot.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-
-
 # XGO-PythonLib
 
 XGO2 has built-in motion libraries for controlling the movement and various features of the machine dog, including battery level, firmware version, and servo angle. The motion library enables users to control translation and pose movement, as well as single servo and single-leg movement. The education library facilitates camera, screen, key, microphone, and speaker operations, as well as commonly used AI functions such as gesture recognition, face detection, emotional recognition, and age and gender recognition.  The detailed instructions for use of the library are as follows.
 
 PythonLib included xgolib.py and xgoedu.py
 
 [Luwu Dynamics · WIKI](https://www.yuque.com/luwudynamics)
@@ -53,17 +35,30 @@
 xgolib library example
 ```python
 from xgolib import XGO
 dog = XGO('xgomini')
 dog.action(1)
 ```
 ### 
+## Change Log
+
+### [0.2.5] - 2023-07-19
+
+#### Fixed
+
+- Methods: Change the __init__ in xgolib.py to add delay to resolve some movement irregularities.
 
 ## Change Log
 
+### [0.2.4] - 2023-07-13
+
+#### Fixed
+
+- Methods: lcd_clear() was fixed.
+
 ### [0.2.3] - 2023-07-04
 
 #### Added
 
 - Methods: cap_color_mask added.
 
 #### Fixed
```

### Comparing `xgo-pythonlib-0.2.4/setup.py` & `xgo-pythonlib-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 NAME = 'xgo-pythonlib'
 DESCRIPTION = 'PythonLib for XGO2-DOG'
 URL = 'https://github.com/Xgorobot/XGO-PythonLib'
 EMAIL = 'hello@xgorobot.com'
 AUTHOR = 'luwudynamics'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.2.4'
+VERSION = '0.2.5'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

### Comparing `xgo-pythonlib-0.2.4/xgo_pythonlib.egg-info/PKG-INFO` & `xgo-pythonlib-0.2.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.2.4
+Version: 0.2.5
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: luwudynamics
 Author-email: hello@xgorobot.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -53,17 +53,30 @@
 xgolib library example
 ```python
 from xgolib import XGO
 dog = XGO('xgomini')
 dog.action(1)
 ```
 ### 
+## Change Log
+
+### [0.2.5] - 2023-07-19
+
+#### Fixed
+
+- Methods: Change the __init__ in xgolib.py to add delay to resolve some movement irregularities.
 
 ## Change Log
 
+### [0.2.4] - 2023-07-13
+
+#### Fixed
+
+- Methods: lcd_clear() was fixed.
+
 ### [0.2.3] - 2023-07-04
 
 #### Added
 
 - Methods: cap_color_mask added.
 
 #### Fixed
```

### Comparing `xgo-pythonlib-0.2.4/xgoedu/__init__.py` & `xgo-pythonlib-0.2.5/xgoedu/__init__.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.2.4/xgolib/__init__.py` & `xgo-pythonlib-0.2.5/xgolib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import serial
 import struct
 import time
 import math
-__version__ = '1.3.3'
-__last_modified__ = '2023/6/19'
+__version__ = '1.3.4'
+__last_modified__ = '2023/7/19'
 
 """
 XGOorder 用来存放命令地址和对应数据
 XGOorder is used to store the command address and corresponding data
 """
 
 XGOorder = {
@@ -135,27 +135,27 @@
         self.ser.flushInput()
         self.port = port
         self.rx_FLAG = 0
         self.rx_COUNT = 0
         self.rx_ADDR = 0
         self.rx_LEN = 0
         self.rx_data = bytearray(50)
-        time.sleep(1)
+        time.sleep(0.25)
         self.version = self.read_firmware()
         if self.version[0] == 'M':
             changePara('xgomini')
         elif self.version[0] == 'L':
             changePara('xgolite')
         else:
             changePara('xgomini')
             print("ERROR!Can't read firmware version!")
         self.mintime = 0.65
         self.reset()
-        time.sleep(0.5)
         self.init_yaw = self.read_yaw()
+        time.sleep(1.25)
         pass
 
     def __send(self, key, index=1, len=1):
         mode = 0x01
         order = XGOorder[key][0] + index - 1
         value = []
         value_sum = 0
@@ -168,14 +168,15 @@
         tx.extend(value)
         tx.extend([sum_data, 0x00, 0xAA])
         self.ser.write(tx)
         if self.verbose:
             print("tx_data: ", tx)
 
     def __read(self, addr, read_len=1):
+        self.ser.flushInput()
         mode = 0x02
         sum_data = (0x09 + mode + addr + read_len) % 256
         sum_data = 255 - sum_data
         tx = [0x55, 0x00, 0x09, mode, addr, read_len, sum_data, 0x00, 0xAA]
         self.ser.flushInput()
         self.ser.write(tx)
         if self.verbose:
@@ -324,15 +325,15 @@
 
     def reset(self):
         """
         机器狗停止运动，所有参数恢复到初始状态
         The robot dog stops moving and all parameters return to the initial state
         """
         self.action(255)
-        time.sleep(0.2)
+        time.sleep(0.75)
 
     def leg(self, leg_id, data):
         """
         控制机器狗的单腿的三轴移动
         Control the three-axis movement of a single leg of the robot
         """
         value = [0, 0, 0]
@@ -353,14 +354,15 @@
             self.__send("LEG_POS", index)
 
     def __motor(self, index, data):
         if index < 13:
             XGOorder["MOTOR_ANGLE"][index] = conver2u8(data, XGOparam["MOTOR_LIMIT"][index % 3 - 1])
         elif index == 13:
             self.claw(conver2u8(data, XGOparam["MOTOR_LIMIT"][3]))
+            return
         else:
             XGOorder["MOTOR_ANGLE"][index] = conver2u8(data, XGOparam["MOTOR_LIMIT"][index - 10])
         self.__send("MOTOR_ANGLE", index)
 
     def motor(self, motor_id, data):
         """
         控制机器狗单个舵机转动
@@ -546,60 +548,57 @@
             print("ERROR!Name only supports characters in ASCII code!")
 
     def read_motor(self):
         """
         读取15个舵机的角度
         """
         self.__read(XGOorder["MOTOR_ANGLE"][0], 15)
-        self.ser.read_all()
         angle = []
         if self.__unpack():
             for i in range(self.rx_COUNT + 1):
                 if i < 12:
                     angle.append(round(conver2float(self.rx_data[i], XGOparam["MOTOR_LIMIT"][i % 3]), 2))
                 else:
                     angle.append(round(conver2float(self.rx_data[i], XGOparam["MOTOR_LIMIT"][i - 9]), 2))
         return angle
 
     def read_battery(self):
-        self.ser.read_all()
         self.__read(XGOorder["BATTERY"][0], 1)
         battery = 0
         if self.__unpack():
             battery = int(self.rx_data[0])
         return battery
 
     def read_firmware(self):
         self.__read(XGOorder["FIRMWARE_VERSION"][0], 10)
-        self.ser.read_all()
         firmware_version = 'Null'
         if self.__unpack():
             data = self.rx_data[0:10]
-            firmware_version = data.decode("ascii").strip('\0')
+            try:
+                firmware_version = data.decode("ascii").strip('\0')
+            except Exception as e:
+                print(e)
         return firmware_version
 
     def read_roll(self):
         self.__read(XGOorder["ROLL"][0], 4)
-        self.ser.read_all()
         roll = 0
         if self.__unpack():
             roll = Byte2Float(self.rx_data)
         return round(roll, 2)
 
     def read_pitch(self):
         self.__read(XGOorder["PITCH"][0], 4)
-        self.ser.read_all()
         pitch = 0
         if self.__unpack():
             pitch = Byte2Float(self.rx_data)
         return round(pitch, 2)
 
     def read_yaw(self):
         self.__read(XGOorder["YAW"][0], 4)
-        self.ser.read_all()
         yaw = 0
         if self.__unpack():
             yaw = Byte2Float(self.rx_data)
         return round(yaw, 2)
 
     def __unpack(self, timeout=1):
         t = time.time()
@@ -782,7 +781,8 @@
             if ord(c) > 255:
                 print("The name can only contain numbers and letters")
                 return
             else:
                 XGOorder["BT_NAME"].append(ord(c))
         print(XGOorder["BT_NAME"])
         self.__send("BT_NAME", len=length)
+
```

### Comparing `xgo-pythonlib-0.2.4/xgoscreen/LCD_2inch.py` & `xgo-pythonlib-0.2.5/xgoscreen/LCD_2inch.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.2.4/xgoscreen/lcdconfig.py` & `xgo-pythonlib-0.2.5/xgoscreen/lcdconfig.py`

 * *Files identical despite different names*

