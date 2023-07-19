# Comparing `tmp/okftools-0.0.4.tar.gz` & `tmp/okftools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okftools-0.0.4.tar", last modified: Wed Jul 19 14:40:53 2023, max compression
+gzip compressed data, was "okftools-0.0.5.tar", last modified: Wed Jul 19 14:46:21 2023, max compression
```

## Comparing `okftools-0.0.4.tar` & `okftools-0.0.5.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 14:40:53.816943 okftools-0.0.4/
--rw-rw-rw-   0        0        0     2251 2023-07-19 14:40:53.815912 okftools-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1723 2023-07-19 14:37:18.000000 okftools-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 14:40:53.787788 okftools-0.0.4/code_sources/
-drwxrwxrwx   0        0        0        0 2023-07-19 14:40:53.792955 okftools-0.0.4/code_sources/GUI/
--rw-rw-rw-   0        0        0    55344 2023-07-19 11:01:11.000000 okftools-0.0.4/code_sources/GUI/okftools.py
-drwxrwxrwx   0        0        0        0 2023-07-19 14:40:53.793995 okftools-0.0.4/code_sources/kernel/
--rw-rw-rw-   0        0        0      220 2023-07-19 09:39:20.000000 okftools-0.0.4/code_sources/kernel/Makefile
--rw-rw-rw-   0        0        0    33569 2023-07-19 14:24:16.000000 okftools-0.0.4/code_sources/kernel/netlink_kernel.c
-drwxrwxrwx   0        0        0        0 2023-07-19 14:40:53.789859 okftools-0.0.4/code_sources/user/
-drwxrwxrwx   0        0        0        0 2023-07-19 14:40:53.795019 okftools-0.0.4/code_sources/user/clean_log/
--rw-rw-rw-   0        0        0      128 2023-07-16 08:14:40.000000 okftools-0.0.4/code_sources/user/clean_log/CMakeLists.txt
--rw-rw-rw-   0        0        0      119 2023-07-19 11:01:11.000000 okftools-0.0.4/code_sources/user/clean_log/clean_log.c
-drwxrwxrwx   0        0        0        0 2023-07-19 14:40:53.796103 okftools-0.0.4/code_sources/user/log_control/
--rw-rw-rw-   0        0        0      145 2023-07-19 11:01:11.000000 okftools-0.0.4/code_sources/user/log_control/CMakeLists.txt
--rw-rw-rw-   0        0        0    11843 2023-07-19 13:03:00.000000 okftools-0.0.4/code_sources/user/log_control/log_control.c
-drwxrwxrwx   0        0        0        0 2023-07-19 14:40:53.797651 okftools-0.0.4/code_sources/user/receive message/
--rw-rw-rw-   0        0        0      161 2023-07-16 08:02:34.000000 okftools-0.0.4/code_sources/user/receive message/CMakeLists.txt
--rw-rw-rw-   0        0        0     6045 2023-07-19 11:01:11.000000 okftools-0.0.4/code_sources/user/receive message/recv_msg_from_kernel.c
-drwxrwxrwx   0        0        0        0 2023-07-19 14:40:53.798200 okftools-0.0.4/code_sources/user/send message/
--rw-rw-rw-   0        0        0      155 2023-07-16 08:03:26.000000 okftools-0.0.4/code_sources/user/send message/CMakeLists.txt
--rw-rw-rw-   0        0        0     2258 2023-07-19 05:51:55.000000 okftools-0.0.4/code_sources/user/send message/send_msg_to_kernel.c
-drwxrwxrwx   0        0        0        0 2023-07-19 14:40:53.799805 okftools-0.0.4/code_sources/user/send_control_path/
--rw-rw-rw-   0        0        0      152 2023-07-16 15:50:28.000000 okftools-0.0.4/code_sources/user/send_control_path/CMakeLists.txt
--rw-rw-rw-   0        0        0     1563 2023-07-16 15:49:14.000000 okftools-0.0.4/code_sources/user/send_control_path/send_control_path.c
-drwxrwxrwx   0        0        0        0 2023-07-19 14:40:53.809655 okftools-0.0.4/okftools/
--rw-rw-rw-   0        0        0    16008 2023-07-19 14:37:52.000000 okftools-0.0.4/okftools/clean_log
--rw-rw-rw-   0        0        0     1656 2023-07-19 14:37:52.000000 okftools-0.0.4/okftools/log.txt
--rw-rw-rw-   0        0        0    21552 2023-07-19 14:37:52.000000 okftools-0.0.4/okftools/log_control
-drwxrwxrwx   0        0        0        0 2023-07-19 14:40:53.814881 okftools-0.0.4/okftools/netlink_kernel/
--rw-rw-rw-   0        0        0      214 2023-07-19 14:37:52.000000 okftools-0.0.4/okftools/netlink_kernel/Makefile
--rw-rw-rw-   0        0        0    32469 2023-07-19 14:37:52.000000 okftools-0.0.4/okftools/netlink_kernel/netlink_kernel.c
--rw-rw-rw-   0        0        0   508208 2023-07-19 14:37:52.000000 okftools-0.0.4/okftools/netlink_kernel.ko
--rw-rw-rw-   0        0        0      623 2023-07-19 14:39:52.000000 okftools-0.0.4/okftools/okftools_setup.py
--rw-rw-rw-   0        0        0    17456 2023-07-19 14:37:52.000000 okftools-0.0.4/okftools/recv_msg_from_kernel
--rw-rw-rw-   0        0        0    16408 2023-07-19 14:37:52.000000 okftools-0.0.4/okftools/send_control_path
--rw-rw-rw-   0        0        0    16536 2023-07-19 14:37:52.000000 okftools-0.0.4/okftools/send_msg_to_kernel
-drwxrwxrwx   0        0        0        0 2023-07-19 14:40:53.812817 okftools-0.0.4/okftools.egg-info/
--rw-rw-rw-   0        0        0     2251 2023-07-19 14:40:53.000000 okftools-0.0.4/okftools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1071 2023-07-19 14:40:53.000000 okftools-0.0.4/okftools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 14:40:53.000000 okftools-0.0.4/okftools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-19 14:40:53.000000 okftools-0.0.4/okftools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-19 14:40:53.000000 okftools-0.0.4/okftools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-19 14:40:53.816943 okftools-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1568 2023-07-19 14:40:32.000000 okftools-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-19 14:40:53.815912 okftools-0.0.4/tests/
--rw-rw-rw-   0        0        0      536 2023-07-19 14:21:17.000000 okftools-0.0.4/tests/test_make_gui.py
--rw-rw-rw-   0        0        0      603 2023-07-19 13:14:26.000000 okftools-0.0.4/tests/test_okftools.py
+drwxrwxrwx   0        0        0        0 2023-07-19 14:46:21.303504 okftools-0.0.5/
+-rw-rw-rw-   0        0        0     2280 2023-07-19 14:46:21.303504 okftools-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1752 2023-07-19 14:44:32.000000 okftools-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 14:46:21.274539 okftools-0.0.5/code_sources/
+drwxrwxrwx   0        0        0        0 2023-07-19 14:46:21.277771 okftools-0.0.5/code_sources/GUI/
+-rw-rw-rw-   0        0        0    55344 2023-07-19 11:01:11.000000 okftools-0.0.5/code_sources/GUI/okftools.py
+drwxrwxrwx   0        0        0        0 2023-07-19 14:46:21.278774 okftools-0.0.5/code_sources/kernel/
+-rw-rw-rw-   0        0        0      220 2023-07-19 09:39:20.000000 okftools-0.0.5/code_sources/kernel/Makefile
+-rw-rw-rw-   0        0        0    33569 2023-07-19 14:24:16.000000 okftools-0.0.5/code_sources/kernel/netlink_kernel.c
+drwxrwxrwx   0        0        0        0 2023-07-19 14:46:21.275663 okftools-0.0.5/code_sources/user/
+drwxrwxrwx   0        0        0        0 2023-07-19 14:46:21.279798 okftools-0.0.5/code_sources/user/clean_log/
+-rw-rw-rw-   0        0        0      128 2023-07-16 08:14:40.000000 okftools-0.0.5/code_sources/user/clean_log/CMakeLists.txt
+-rw-rw-rw-   0        0        0      119 2023-07-19 11:01:11.000000 okftools-0.0.5/code_sources/user/clean_log/clean_log.c
+drwxrwxrwx   0        0        0        0 2023-07-19 14:46:21.280828 okftools-0.0.5/code_sources/user/log_control/
+-rw-rw-rw-   0        0        0      145 2023-07-19 11:01:11.000000 okftools-0.0.5/code_sources/user/log_control/CMakeLists.txt
+-rw-rw-rw-   0        0        0    11843 2023-07-19 13:03:00.000000 okftools-0.0.5/code_sources/user/log_control/log_control.c
+drwxrwxrwx   0        0        0        0 2023-07-19 14:46:21.282880 okftools-0.0.5/code_sources/user/receive message/
+-rw-rw-rw-   0        0        0      161 2023-07-16 08:02:34.000000 okftools-0.0.5/code_sources/user/receive message/CMakeLists.txt
+-rw-rw-rw-   0        0        0     6045 2023-07-19 11:01:11.000000 okftools-0.0.5/code_sources/user/receive message/recv_msg_from_kernel.c
+drwxrwxrwx   0        0        0        0 2023-07-19 14:46:21.283903 okftools-0.0.5/code_sources/user/send message/
+-rw-rw-rw-   0        0        0      155 2023-07-16 08:03:26.000000 okftools-0.0.5/code_sources/user/send message/CMakeLists.txt
+-rw-rw-rw-   0        0        0     2258 2023-07-19 05:51:55.000000 okftools-0.0.5/code_sources/user/send message/send_msg_to_kernel.c
+drwxrwxrwx   0        0        0        0 2023-07-19 14:46:21.285027 okftools-0.0.5/code_sources/user/send_control_path/
+-rw-rw-rw-   0        0        0      152 2023-07-16 15:50:28.000000 okftools-0.0.5/code_sources/user/send_control_path/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1563 2023-07-16 15:49:14.000000 okftools-0.0.5/code_sources/user/send_control_path/send_control_path.c
+drwxrwxrwx   0        0        0        0 2023-07-19 14:46:21.298390 okftools-0.0.5/okftools/
+drwxrwxrwx   0        0        0        0 2023-07-19 14:46:21.301458 okftools-0.0.5/okftools/GUI/
+-rw-rw-rw-   0        0        0    54098 2023-07-19 14:37:52.000000 okftools-0.0.5/okftools/GUI/okftools.py
+-rw-rw-rw-   0        0        0    16008 2023-07-19 14:37:52.000000 okftools-0.0.5/okftools/clean_log
+-rw-rw-rw-   0        0        0     1656 2023-07-19 14:37:52.000000 okftools-0.0.5/okftools/log.txt
+-rw-rw-rw-   0        0        0    21552 2023-07-19 14:37:52.000000 okftools-0.0.5/okftools/log_control
+drwxrwxrwx   0        0        0        0 2023-07-19 14:46:21.302480 okftools-0.0.5/okftools/netlink_kernel/
+-rw-rw-rw-   0        0        0      214 2023-07-19 14:37:52.000000 okftools-0.0.5/okftools/netlink_kernel/Makefile
+-rw-rw-rw-   0        0        0    32469 2023-07-19 14:37:52.000000 okftools-0.0.5/okftools/netlink_kernel/netlink_kernel.c
+-rw-rw-rw-   0        0        0   508208 2023-07-19 14:37:52.000000 okftools-0.0.5/okftools/netlink_kernel.ko
+-rw-rw-rw-   0        0        0      623 2023-07-19 14:39:52.000000 okftools-0.0.5/okftools/okftools_setup.py
+-rw-rw-rw-   0        0        0    17456 2023-07-19 14:37:52.000000 okftools-0.0.5/okftools/recv_msg_from_kernel
+-rw-rw-rw-   0        0        0    16408 2023-07-19 14:37:52.000000 okftools-0.0.5/okftools/send_control_path
+-rw-rw-rw-   0        0        0    16536 2023-07-19 14:37:52.000000 okftools-0.0.5/okftools/send_msg_to_kernel
+drwxrwxrwx   0        0        0        0 2023-07-19 14:46:21.300436 okftools-0.0.5/okftools.egg-info/
+-rw-rw-rw-   0        0        0     2280 2023-07-19 14:46:21.000000 okftools-0.0.5/okftools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1096 2023-07-19 14:46:21.000000 okftools-0.0.5/okftools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 14:46:21.000000 okftools-0.0.5/okftools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-19 14:46:21.000000 okftools-0.0.5/okftools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-19 14:46:21.000000 okftools-0.0.5/okftools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 14:46:21.303504 okftools-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1576 2023-07-19 14:46:16.000000 okftools-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 14:46:21.303504 okftools-0.0.5/tests/
+-rw-rw-rw-   0        0        0      536 2023-07-19 14:21:17.000000 okftools-0.0.5/tests/test_make_gui.py
+-rw-rw-rw-   0        0        0      603 2023-07-19 13:14:26.000000 okftools-0.0.5/tests/test_okftools.py
```

### Comparing `okftools-0.0.4/PKG-INFO` & `okftools-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okftools
-Version: 0.0.4
+Version: 0.0.5
 Summary: okftools to achieve overloading kernel function under Linux 5.19
 Home-page: https://github.com/heatingma/NIS3302-okftools
 Author: heatingma  qigu  cfg554  halsayxi  sora
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: POSIX :: Linux
@@ -47,15 +47,15 @@
 <br>
 <strong><font face="仿宋" size=2>图2 pip show okftools</font>
 </strong>
 </center></div>
 
         3.cd the okftools path
 
-        4.python okftools_setup.py 
+        4.python okftools_setup.py or python3 okftools_setup.py 
 <div><center>
 <img src=docs/setup.png width=70% height=70% >
 <br>
 <strong><font face="仿宋" size=2>图4 python okftools_setup.py</font>
 </strong>
 </center></div>
```

### Comparing `okftools-0.0.4/README.md` & `okftools-0.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 <br>
 <strong><font face="仿宋" size=2>图2 pip show okftools</font>
 </strong>
 </center></div>
 
         3.cd the okftools path
 
-        4.python okftools_setup.py 
+        4.python okftools_setup.py or python3 okftools_setup.py 
 <div><center>
 <img src=docs/setup.png width=70% height=70% >
 <br>
 <strong><font face="仿宋" size=2>图4 python okftools_setup.py</font>
 </strong>
 </center></div>
```

### Comparing `okftools-0.0.4/code_sources/GUI/okftools.py` & `okftools-0.0.5/code_sources/GUI/okftools.py`

 * *Files identical despite different names*

### Comparing `okftools-0.0.4/code_sources/kernel/netlink_kernel.c` & `okftools-0.0.5/code_sources/kernel/netlink_kernel.c`

 * *Files identical despite different names*

### Comparing `okftools-0.0.4/code_sources/user/log_control/log_control.c` & `okftools-0.0.5/code_sources/user/log_control/log_control.c`

 * *Files identical despite different names*

### Comparing `okftools-0.0.4/code_sources/user/receive message/recv_msg_from_kernel.c` & `okftools-0.0.5/code_sources/user/receive message/recv_msg_from_kernel.c`

 * *Files identical despite different names*

### Comparing `okftools-0.0.4/code_sources/user/send message/send_msg_to_kernel.c` & `okftools-0.0.5/code_sources/user/send message/send_msg_to_kernel.c`

 * *Files identical despite different names*

### Comparing `okftools-0.0.4/code_sources/user/send_control_path/send_control_path.c` & `okftools-0.0.5/code_sources/user/send_control_path/send_control_path.c`

 * *Files identical despite different names*

### Comparing `okftools-0.0.4/okftools/clean_log` & `okftools-0.0.5/okftools/clean_log`

 * *Files identical despite different names*

### Comparing `okftools-0.0.4/okftools/log.txt` & `okftools-0.0.5/okftools/log.txt`

 * *Files identical despite different names*

### Comparing `okftools-0.0.4/okftools/log_control` & `okftools-0.0.5/okftools/log_control`

 * *Files identical despite different names*

### Comparing `okftools-0.0.4/okftools/netlink_kernel/netlink_kernel.c` & `okftools-0.0.5/okftools/netlink_kernel/netlink_kernel.c`

 * *Files identical despite different names*

### Comparing `okftools-0.0.4/okftools/netlink_kernel.ko` & `okftools-0.0.5/okftools/netlink_kernel.ko`

 * *Files identical despite different names*

### Comparing `okftools-0.0.4/okftools/okftools_setup.py` & `okftools-0.0.5/okftools/okftools_setup.py`

 * *Files identical despite different names*

### Comparing `okftools-0.0.4/okftools/recv_msg_from_kernel` & `okftools-0.0.5/okftools/recv_msg_from_kernel`

 * *Files identical despite different names*

### Comparing `okftools-0.0.4/okftools/send_control_path` & `okftools-0.0.5/okftools/send_control_path`

 * *Files identical despite different names*

### Comparing `okftools-0.0.4/okftools/send_msg_to_kernel` & `okftools-0.0.5/okftools/send_msg_to_kernel`

 * *Files identical despite different names*

### Comparing `okftools-0.0.4/okftools.egg-info/PKG-INFO` & `okftools-0.0.5/okftools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okftools
-Version: 0.0.4
+Version: 0.0.5
 Summary: okftools to achieve overloading kernel function under Linux 5.19
 Home-page: https://github.com/heatingma/NIS3302-okftools
 Author: heatingma  qigu  cfg554  halsayxi  sora
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: POSIX :: Linux
@@ -47,15 +47,15 @@
 <br>
 <strong><font face="仿宋" size=2>图2 pip show okftools</font>
 </strong>
 </center></div>
 
         3.cd the okftools path
 
-        4.python okftools_setup.py 
+        4.python okftools_setup.py or python3 okftools_setup.py 
 <div><center>
 <img src=docs/setup.png width=70% height=70% >
 <br>
 <strong><font face="仿宋" size=2>图4 python okftools_setup.py</font>
 </strong>
 </center></div>
```

### Comparing `okftools-0.0.4/okftools.egg-info/SOURCES.txt` & `okftools-0.0.5/okftools.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -22,11 +22,12 @@
 okftools/send_control_path
 okftools/send_msg_to_kernel
 okftools.egg-info/PKG-INFO
 okftools.egg-info/SOURCES.txt
 okftools.egg-info/dependency_links.txt
 okftools.egg-info/requires.txt
 okftools.egg-info/top_level.txt
+okftools/GUI/okftools.py
 okftools/netlink_kernel/Makefile
 okftools/netlink_kernel/netlink_kernel.c
 tests/test_make_gui.py
 tests/test_okftools.py
```

### Comparing `okftools-0.0.4/setup.py` & `okftools-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,22 +22,22 @@
     with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 setup(
     name=NAME,
-    version='0.0.4',
+    version='0.0.5',
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     url=URL,
     packages=['okftools','code_sources'],
-    package_data={'okftools': ['*','netlink_kernel/*'], 
+    package_data={'okftools': ['*','netlink_kernel/*','GUI/*'], 
                   'code_sources': ['GUI/*', 'kernel/*', 'user/clean_log/*', 'user/log_control/*', \
                                    'user/receive message/*', 'user/send message/*', 'user/send_control_path/*']},
     install_requires=REQUIRED,
     include_package_data=True,
     license='Mulan PSL v2',
     python_requires='>=3.7',
     classifiers=[
```

### Comparing `okftools-0.0.4/tests/test_make_gui.py` & `okftools-0.0.5/tests/test_make_gui.py`

 * *Files identical despite different names*

### Comparing `okftools-0.0.4/tests/test_okftools.py` & `okftools-0.0.5/tests/test_okftools.py`

 * *Files identical despite different names*

