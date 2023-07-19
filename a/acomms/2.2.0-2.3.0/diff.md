# Comparing `tmp/acomms-2.2.0.tar.gz` & `tmp/acomms-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acomms-2.2.0.tar", last modified: Fri Sep 16 02:24:32 2022, max compression
+gzip compressed data, was "acomms-2.3.0.tar", last modified: Wed Jul 19 15:57:03 2023, max compression
```

## Comparing `acomms-2.2.0.tar` & `acomms-2.3.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 caileigh  (1000) caileigh  (1000)        0 2022-09-16 02:24:32.985125 acomms-2.2.0/
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)      404 2022-06-03 22:01:21.000000 acomms-2.2.0/CHANGES.txt
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     7814 2022-06-03 22:01:21.000000 acomms-2.2.0/LICENSE.txt
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)       43 2022-06-03 22:01:21.000000 acomms-2.2.0/MANIFEST.in
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     1003 2022-09-16 02:24:32.985125 acomms-2.2.0/PKG-INFO
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)      319 2022-06-03 22:01:21.000000 acomms-2.2.0/README.txt
-drwxrwxr-x   0 caileigh  (1000) caileigh  (1000)        0 2022-09-16 02:24:32.981125 acomms-2.2.0/acomms/
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)      329 2022-06-03 22:01:21.000000 acomms-2.2.0/acomms/__init__.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)    24838 2022-06-03 22:01:21.000000 acomms-2.2.0/acomms/acomms_xmodem.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)    16495 2022-06-03 22:01:21.000000 acomms-2.2.0/acomms/ccl.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)    21106 2022-06-03 22:01:21.000000 acomms-2.2.0/acomms/commstate.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)    15857 2022-08-11 15:22:24.000000 acomms-2.2.0/acomms/cyclestats.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     5938 2022-08-11 15:22:24.000000 acomms-2.2.0/acomms/flexibledataprotocol.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     4463 2022-06-03 22:01:21.000000 acomms-2.2.0/acomms/index_list.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)    12329 2022-08-11 15:22:24.000000 acomms-2.2.0/acomms/messageparams.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)    22915 2022-08-11 15:45:33.000000 acomms-2.2.0/acomms/messageparser.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)    67084 2022-08-11 15:22:24.000000 acomms-2.2.0/acomms/micromodem.py
-drwxrwxr-x   0 caileigh  (1000) caileigh  (1000)        0 2022-09-16 02:24:32.985125 acomms-2.2.0/acomms/modem_connections/
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)      532 2022-06-03 22:01:21.000000 acomms-2.2.0/acomms/modem_connections/__init__.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)      237 2022-06-03 22:01:21.000000 acomms-2.2.0/acomms/modem_connections/connection_utilities.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     4219 2022-06-03 22:01:21.000000 acomms-2.2.0/acomms/modem_connections/iridium_connection.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)      616 2022-06-03 22:01:21.000000 acomms-2.2.0/acomms/modem_connections/modem_connection.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     4738 2022-06-03 22:01:21.000000 acomms-2.2.0/acomms/modem_connections/sbd_connection.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     2150 2022-06-03 22:01:21.000000 acomms-2.2.0/acomms/modem_connections/serial_connection.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     2592 2022-06-03 22:01:21.000000 acomms-2.2.0/acomms/modem_connections/tcp_client_connection.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     1461 2022-06-03 22:01:21.000000 acomms-2.2.0/acomms/modem_connections/tcp_connection.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     3527 2022-06-03 22:01:21.000000 acomms-2.2.0/acomms/modem_connections/udp_connection.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     2063 2022-06-03 22:01:21.000000 acomms-2.2.0/acomms/modemlog.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     2911 2022-06-03 22:01:21.000000 acomms-2.2.0/acomms/net_modem.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     5714 2022-06-03 22:01:21.000000 acomms-2.2.0/acomms/net_packet.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)      444 2022-06-03 22:01:21.000000 acomms-2.2.0/acomms/nmealistener.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)      302 2022-06-03 22:01:21.000000 acomms-2.2.0/acomms/pid_defs.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     4677 2022-06-03 22:01:21.000000 acomms-2.2.0/acomms/ping.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     2081 2022-06-03 22:01:21.000000 acomms-2.2.0/acomms/timeutil.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     2737 2022-06-03 22:01:21.000000 acomms-2.2.0/acomms/unifiedlog.py
-drwxrwxr-x   0 caileigh  (1000) caileigh  (1000)        0 2022-09-16 02:24:32.981125 acomms-2.2.0/acomms.egg-info/
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     1003 2022-09-16 02:24:32.000000 acomms-2.2.0/acomms.egg-info/PKG-INFO
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     1297 2022-09-16 02:24:32.000000 acomms-2.2.0/acomms.egg-info/SOURCES.txt
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)        1 2022-09-16 02:24:32.000000 acomms-2.2.0/acomms.egg-info/dependency_links.txt
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)       79 2022-09-16 02:24:32.000000 acomms-2.2.0/acomms.egg-info/requires.txt
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)       20 2022-09-16 02:24:32.000000 acomms-2.2.0/acomms.egg-info/top_level.txt
-drwxrwxr-x   0 caileigh  (1000) caileigh  (1000)        0 2022-09-16 02:24:32.985125 acomms-2.2.0/bin/
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)        0 2022-06-03 22:01:21.000000 acomms-2.2.0/bin/__init__.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)      539 2022-06-03 22:01:21.000000 acomms-2.2.0/bin/ccl_decoder.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)      941 2022-06-03 22:01:21.000000 acomms-2.2.0/bin/console_logger.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     1528 2022-06-03 22:01:21.000000 acomms-2.2.0/bin/cst_forwarder.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     8473 2022-06-03 22:01:21.000000 acomms-2.2.0/bin/iridium_csd_listener.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     6678 2022-06-03 22:01:21.000000 acomms-2.2.0/bin/legacy_to_fdp_translator.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     8449 2022-06-03 22:01:21.000000 acomms-2.2.0/bin/magiccstbox.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     3153 2022-06-03 22:01:21.000000 acomms-2.2.0/bin/modem_bridge.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     1234 2022-06-03 22:01:21.000000 acomms-2.2.0/bin/ping_transponder.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)    10527 2022-06-03 22:01:21.000000 acomms-2.2.0/bin/plotter.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     3796 2022-06-03 22:01:21.000000 acomms-2.2.0/bin/ranger_to_gprmc.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     1029 2022-06-22 21:16:11.000000 acomms-2.2.0/bin/test_interactive_local_acomms.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)      306 2022-06-03 22:01:21.000000 acomms-2.2.0/build_notes.txt
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     8019 2022-06-03 22:01:21.000000 acomms-2.2.0/ez_setup.py
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)       80 2022-09-16 02:24:32.985125 acomms-2.2.0/setup.cfg
--rw-rw-r--   0 caileigh  (1000) caileigh  (1000)     1601 2022-09-16 02:16:42.000000 acomms-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:57:03.630666 acomms-2.3.0/
+-rw-rw-rw-   0        0        0      524 2023-07-19 15:51:41.000000 acomms-2.3.0/CHANGES.txt
+-rw-rw-rw-   0        0        0     7814 2020-09-08 17:07:07.000000 acomms-2.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       43 2020-09-08 17:07:07.000000 acomms-2.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1028 2023-07-19 15:57:03.630666 acomms-2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2020-09-08 17:07:07.000000 acomms-2.3.0/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 15:57:03.594366 acomms-2.3.0/acomms/
+-rw-rw-rw-   0        0        0      329 2021-12-06 16:48:02.000000 acomms-2.3.0/acomms/__init__.py
+-rw-rw-rw-   0        0        0    24838 2020-09-08 17:07:07.000000 acomms-2.3.0/acomms/acomms_xmodem.py
+-rw-rw-rw-   0        0        0    16495 2021-03-20 13:58:23.000000 acomms-2.3.0/acomms/ccl.py
+-rw-rw-rw-   0        0        0    21106 2021-10-03 02:49:15.000000 acomms-2.3.0/acomms/commstate.py
+-rw-rw-rw-   0        0        0    15968 2023-07-19 15:44:17.000000 acomms-2.3.0/acomms/cyclestats.py
+-rw-rw-rw-   0        0        0     5938 2023-07-19 15:39:59.000000 acomms-2.3.0/acomms/flexibledataprotocol.py
+-rw-rw-rw-   0        0        0     4463 2021-12-06 16:48:02.000000 acomms-2.3.0/acomms/index_list.py
+-rw-rw-rw-   0        0        0    12329 2022-10-08 03:44:55.000000 acomms-2.3.0/acomms/messageparams.py
+-rw-rw-rw-   0        0        0    22915 2022-06-29 14:09:26.000000 acomms-2.3.0/acomms/messageparser.py
+-rw-rw-rw-   0        0        0    67084 2022-10-08 03:44:55.000000 acomms-2.3.0/acomms/micromodem.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:57:03.614048 acomms-2.3.0/acomms/modem_connections/
+-rw-rw-rw-   0        0        0      532 2020-09-08 17:07:07.000000 acomms-2.3.0/acomms/modem_connections/__init__.py
+-rw-rw-rw-   0        0        0      237 2020-09-08 17:07:07.000000 acomms-2.3.0/acomms/modem_connections/connection_utilities.py
+-rw-rw-rw-   0        0        0     4219 2020-09-08 17:07:07.000000 acomms-2.3.0/acomms/modem_connections/iridium_connection.py
+-rw-rw-rw-   0        0        0      616 2020-09-08 17:07:07.000000 acomms-2.3.0/acomms/modem_connections/modem_connection.py
+-rw-rw-rw-   0        0        0     4738 2020-09-08 17:07:07.000000 acomms-2.3.0/acomms/modem_connections/sbd_connection.py
+-rw-rw-rw-   0        0        0     2150 2020-09-08 17:07:07.000000 acomms-2.3.0/acomms/modem_connections/serial_connection.py
+-rw-rw-rw-   0        0        0     2592 2020-09-08 17:07:07.000000 acomms-2.3.0/acomms/modem_connections/tcp_client_connection.py
+-rw-rw-rw-   0        0        0     1461 2020-09-08 17:07:07.000000 acomms-2.3.0/acomms/modem_connections/tcp_connection.py
+-rw-rw-rw-   0        0        0     3527 2021-10-03 02:49:15.000000 acomms-2.3.0/acomms/modem_connections/udp_connection.py
+-rw-rw-rw-   0        0        0     2063 2020-09-08 17:07:07.000000 acomms-2.3.0/acomms/modemlog.py
+-rw-rw-rw-   0        0        0     2911 2021-02-19 19:08:52.000000 acomms-2.3.0/acomms/net_modem.py
+-rw-rw-rw-   0        0        0     5714 2021-02-19 19:08:52.000000 acomms-2.3.0/acomms/net_packet.py
+-rw-rw-rw-   0        0        0      444 2020-09-08 17:07:07.000000 acomms-2.3.0/acomms/nmealistener.py
+-rw-rw-rw-   0        0        0      302 2021-02-19 19:08:52.000000 acomms-2.3.0/acomms/pid_defs.py
+-rw-rw-rw-   0        0        0     4677 2021-10-03 02:49:15.000000 acomms-2.3.0/acomms/ping.py
+-rw-rw-rw-   0        0        0     2081 2020-09-08 17:07:07.000000 acomms-2.3.0/acomms/timeutil.py
+-rw-rw-rw-   0        0        0     2737 2020-09-08 17:07:07.000000 acomms-2.3.0/acomms/unifiedlog.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:57:03.599914 acomms-2.3.0/acomms.egg-info/
+-rw-rw-rw-   0        0        0     1028 2023-07-19 15:57:03.000000 acomms-2.3.0/acomms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1297 2023-07-19 15:57:03.000000 acomms-2.3.0/acomms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 15:57:03.000000 acomms-2.3.0/acomms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-07-19 15:57:03.000000 acomms-2.3.0/acomms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-19 15:57:03.000000 acomms-2.3.0/acomms.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 15:57:03.629670 acomms-2.3.0/bin/
+-rw-rw-rw-   0        0        0        0 2020-09-08 17:07:07.000000 acomms-2.3.0/bin/__init__.py
+-rw-rw-rw-   0        0        0      539 2020-09-08 17:07:07.000000 acomms-2.3.0/bin/ccl_decoder.py
+-rw-rw-rw-   0        0        0      941 2020-09-08 17:07:07.000000 acomms-2.3.0/bin/console_logger.py
+-rw-rw-rw-   0        0        0     1528 2020-09-08 17:07:07.000000 acomms-2.3.0/bin/cst_forwarder.py
+-rw-rw-rw-   0        0        0     8473 2020-09-08 17:07:07.000000 acomms-2.3.0/bin/iridium_csd_listener.py
+-rw-rw-rw-   0        0        0     6708 2021-05-13 14:40:51.000000 acomms-2.3.0/bin/legacy_to_fdp_translator.py
+-rw-rw-rw-   0        0        0     8449 2020-09-08 17:07:07.000000 acomms-2.3.0/bin/magiccstbox.py
+-rw-rw-rw-   0        0        0     3153 2020-09-08 17:07:07.000000 acomms-2.3.0/bin/modem_bridge.py
+-rw-rw-rw-   0        0        0     1234 2020-09-08 17:07:07.000000 acomms-2.3.0/bin/ping_transponder.py
+-rw-rw-rw-   0        0        0    10527 2020-09-08 17:07:07.000000 acomms-2.3.0/bin/plotter.py
+-rw-rw-rw-   0        0        0     3796 2020-09-08 17:07:07.000000 acomms-2.3.0/bin/ranger_to_gprmc.py
+-rw-rw-rw-   0        0        0      980 2022-06-29 14:09:26.000000 acomms-2.3.0/bin/test_interactive_local_acomms.py
+-rw-rw-rw-   0        0        0      306 2020-09-08 17:07:07.000000 acomms-2.3.0/build_notes.txt
+-rw-rw-rw-   0        0        0     8019 2021-02-19 19:08:52.000000 acomms-2.3.0/ez_setup.py
+-rw-rw-rw-   0        0        0       87 2023-07-19 15:57:03.631700 acomms-2.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1601 2023-07-19 15:50:42.000000 acomms-2.3.0/setup.py
```

### Comparing `acomms-2.2.0/LICENSE.txt` & `acomms-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/PKG-INFO` & `acomms-2.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1
-Name: acomms
-Version: 2.2.0
-Summary: WHOI Micromodem Interface Library and Tools
-Home-page: http://acomms.whoi.edu/
-Author: Eric Gallimore, Caileigh Fitzgerald
-Author-email: pyacomms@whoi.edu, cfitzgerald@whoi.edu
-License: LGPLv3+
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Scientific/Engineering
-License-File: LICENSE.txt
-
-===========
-pyAcomms
-===========
-
-pyAcomms provides a Python interface to Micromodem and Micromodem-2 hardware from the
-`Acoustic Communications Group <http://acomms.whoi.edu/>`_ at the `Woods Hole Oceanographic Institution <http://www.whoi.edu/>`_.
-
-See examples in the ``/examples`` and ``/bin`` directories.
+Metadata-Version: 2.1
+Name: acomms
+Version: 2.3.0
+Summary: WHOI Micromodem Interface Library and Tools
+Home-page: http://acomms.whoi.edu/
+Author: Eric Gallimore, Caileigh Fitzgerald
+Author-email: pyacomms@whoi.edu, cfitzgerald@whoi.edu
+License: LGPLv3+
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Scientific/Engineering
+License-File: LICENSE.txt
+
+===========
+pyAcomms
+===========
+
+pyAcomms provides a Python interface to Micromodem and Micromodem-2 hardware from the
+`Acoustic Communications Group <http://acomms.whoi.edu/>`_ at the `Woods Hole Oceanographic Institution <http://www.whoi.edu/>`_.
+
+See examples in the ``/examples`` and ``/bin`` directories.
```

### Comparing `acomms-2.2.0/acomms/acomms_xmodem.py` & `acomms-2.3.0/acomms/acomms_xmodem.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/acomms/ccl.py` & `acomms-2.3.0/acomms/ccl.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/acomms/commstate.py` & `acomms-2.3.0/acomms/commstate.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/acomms/cyclestats.py` & `acomms-2.3.0/acomms/cyclestats.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,15 @@
     '''
 
     # Note that we don't override the dict initalizer.
 
     fields = ('time','toa_mode','mode', 'probe_length',
               'bandwidth', 'carrier', 'rate_num', 'src', 'dest',
               'ack', 'num_frames_expected', 'num_frames_sent', 'packet_type',
-              'nbytes', 'version_number', 'actual_carrier')
+              'nbytes', 'version_number', 'actual_carrier', 'pwramp_txlevel')
 
     # This automagically retrieves values from the dictionary when they are referenced as properties.
     # Whether this is awesome or sucks is open to debate.
     def __getattr__(self, item):
         """Maps values to attributes.
         Only called if there *isn't* an attribute with this name
         """
@@ -273,15 +273,15 @@
 
 
     @classmethod
     def from_nmea_msg(cls, msg, log_datetime=None, drop_data_timeout=True):
 
         values = dict.fromkeys(TransmitStats.fields)
         version_number = int(msg['params'][0])
-        if( version_number==6 or version_number==7):
+        if version_number in (6, 7, 8):
             values['version_number'] = version_number
 
             date = datetime.datetime.strptime(str(msg['params'][1]), "%Y%m%d")
 
             # Parse the time field into a fractional datetime object.
             whole, fract = str(msg['params'][2]).split('.')
             time = datetime.datetime.strptime(whole, '%H%M%S')
@@ -304,16 +304,18 @@
             values['dest'] = int(msg['params'][10])
             values['ack'] = int(msg['params'][11])
             values['num_frames_expected'] = int(msg['params'][12])
             values['num_frames_sent'] = int(msg['params'][13])
             values['packet_type'] = int(msg['params'][14])
             values['nbytes'] = int(msg['params'][15])
 
-            if version_number == 7:
+            if version_number >= 7:
                 values['actual_carrier'] = int(msg['params'][16])
+            if version_number >= 8:
+                values['pwramp_txlevel'] = int(msg['params'][17])
 
         else:
             version_number = 0
             date = datetime.datetime.strptime(str(msg['params'][0]), "%Y%m%d")
 
             # Parse the time field into a fractional datetime object.
             whole, fract = str(msg['params'][1]).split('.')
@@ -337,14 +339,15 @@
             values['dest'] = int(msg['params'][9])
             values['ack'] = int(msg['params'][10])
             values['num_frames_expected'] = int(msg['params'][11])
             values['num_frames_sent'] = int(msg['params'][12])
             values['packet_type'] = int(msg['params'][13])
             values['nbytes'] = int(msg['params'][14])
 
+
             values['version_number'] = version_number
 
 
         # Make a CycleStats
         xst = cls(values)
 
         return xst
```

### Comparing `acomms-2.2.0/acomms/flexibledataprotocol.py` & `acomms-2.3.0/acomms/flexibledataprotocol.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/acomms/index_list.py` & `acomms-2.3.0/acomms/index_list.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/acomms/messageparams.py` & `acomms-2.3.0/acomms/messageparams.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/acomms/messageparser.py` & `acomms-2.3.0/acomms/messageparser.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/acomms/micromodem.py` & `acomms-2.3.0/acomms/micromodem.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/acomms/modem_connections/__init__.py` & `acomms-2.3.0/acomms/modem_connections/__init__.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/acomms/modem_connections/iridium_connection.py` & `acomms-2.3.0/acomms/modem_connections/iridium_connection.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/acomms/modem_connections/modem_connection.py` & `acomms-2.3.0/acomms/modem_connections/modem_connection.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/acomms/modem_connections/sbd_connection.py` & `acomms-2.3.0/acomms/modem_connections/sbd_connection.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/acomms/modem_connections/serial_connection.py` & `acomms-2.3.0/acomms/modem_connections/serial_connection.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/acomms/modem_connections/tcp_client_connection.py` & `acomms-2.3.0/acomms/modem_connections/tcp_client_connection.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/acomms/modem_connections/tcp_connection.py` & `acomms-2.3.0/acomms/modem_connections/tcp_connection.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/acomms/modem_connections/udp_connection.py` & `acomms-2.3.0/acomms/modem_connections/udp_connection.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/acomms/modemlog.py` & `acomms-2.3.0/acomms/modemlog.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/acomms/net_modem.py` & `acomms-2.3.0/acomms/net_modem.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/acomms/net_packet.py` & `acomms-2.3.0/acomms/net_packet.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/acomms/ping.py` & `acomms-2.3.0/acomms/ping.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/acomms/timeutil.py` & `acomms-2.3.0/acomms/timeutil.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/acomms/unifiedlog.py` & `acomms-2.3.0/acomms/unifiedlog.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/acomms.egg-info/PKG-INFO` & `acomms-2.3.0/acomms.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1
-Name: acomms
-Version: 2.2.0
-Summary: WHOI Micromodem Interface Library and Tools
-Home-page: http://acomms.whoi.edu/
-Author: Eric Gallimore, Caileigh Fitzgerald
-Author-email: pyacomms@whoi.edu, cfitzgerald@whoi.edu
-License: LGPLv3+
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Scientific/Engineering
-License-File: LICENSE.txt
-
-===========
-pyAcomms
-===========
-
-pyAcomms provides a Python interface to Micromodem and Micromodem-2 hardware from the
-`Acoustic Communications Group <http://acomms.whoi.edu/>`_ at the `Woods Hole Oceanographic Institution <http://www.whoi.edu/>`_.
-
-See examples in the ``/examples`` and ``/bin`` directories.
+Metadata-Version: 2.1
+Name: acomms
+Version: 2.3.0
+Summary: WHOI Micromodem Interface Library and Tools
+Home-page: http://acomms.whoi.edu/
+Author: Eric Gallimore, Caileigh Fitzgerald
+Author-email: pyacomms@whoi.edu, cfitzgerald@whoi.edu
+License: LGPLv3+
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Scientific/Engineering
+License-File: LICENSE.txt
+
+===========
+pyAcomms
+===========
+
+pyAcomms provides a Python interface to Micromodem and Micromodem-2 hardware from the
+`Acoustic Communications Group <http://acomms.whoi.edu/>`_ at the `Woods Hole Oceanographic Institution <http://www.whoi.edu/>`_.
+
+See examples in the ``/examples`` and ``/bin`` directories.
```

### Comparing `acomms-2.2.0/acomms.egg-info/SOURCES.txt` & `acomms-2.3.0/acomms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/bin/ccl_decoder.py` & `acomms-2.3.0/bin/ccl_decoder.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/bin/console_logger.py` & `acomms-2.3.0/bin/console_logger.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/bin/cst_forwarder.py` & `acomms-2.3.0/bin/cst_forwarder.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/bin/iridium_csd_listener.py` & `acomms-2.3.0/bin/iridium_csd_listener.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/bin/legacy_to_fdp_translator.py` & `acomms-2.3.0/bin/legacy_to_fdp_translator.py`

 * *Files 5% similar despite different names*

```diff
@@ -146,16 +146,16 @@
 if __name__ == '__main__':
     ap = argparse.ArgumentParser(description='Connect to a MM for testing purposes')
     ap.add_argument("-C", "--COM", help='COM Port to connect', default="/dev/ttyO1")
     ap.add_argument("-BR", "--Baudrate", help="COM Port Baud Rate", default=19200)
 
     args = ap.parse_args()
 
-    #translator = FdpTranslator("COM20", 19200, '10.11.62.211', 4001)
-    translator = FdpTranslator(remote_address='10.19.30.199', remote_port=4002, local_port=4002,
-                               modem_remote_address='10.19.30.61', modem_remote_port=4001, modem_local_port=4001)
+    translator = FdpTranslator('10.11.62.175', 4002, modem_serial_port="COM20", modem_baud=19200)
+    #translator = FdpTranslator(remote_address='10.19.30.199', remote_port=4002, local_port=4002,
+    #                           modem_remote_address='10.19.30.61', modem_remote_port=4001, modem_local_port=4001)
 
     try:
         while True:
             sleep(1)
     finally:
         translator = None
```

### Comparing `acomms-2.2.0/bin/magiccstbox.py` & `acomms-2.3.0/bin/magiccstbox.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/bin/modem_bridge.py` & `acomms-2.3.0/bin/modem_bridge.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/bin/ping_transponder.py` & `acomms-2.3.0/bin/ping_transponder.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/bin/plotter.py` & `acomms-2.3.0/bin/plotter.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/bin/ranger_to_gprmc.py` & `acomms-2.3.0/bin/ranger_to_gprmc.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/bin/test_interactive_local_acomms.py` & `acomms-2.3.0/bin/test_interactive_local_acomms.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,14 +14,13 @@
 
 from acomms import micromodem, unifiedlog
 import logging
 
 unified_log = unifiedlog.UnifiedLog(log_path='./', console_log_level=logging.INFO)
 
 um = micromodem.Micromodem(name='Micromodem2',unified_log=unified_log)
-# um = micromodem.Micromodem(name='Micromodem2')
 
 print('\n---')
 print('Not currently connected to a micromodem!')
 print('To connect:...... um.connect_serial(\'/dev/ttyUSB0\', 19200)')
 print('To disconnect:... um.disconnect()')
 print('\n---')
```

### Comparing `acomms-2.2.0/ez_setup.py` & `acomms-2.3.0/ez_setup.py`

 * *Files identical despite different names*

### Comparing `acomms-2.2.0/setup.py` & `acomms-2.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='acomms',
-    version='2.2.0',
+    version='2.3.0',
     author='Eric Gallimore, Caileigh Fitzgerald',
     author_email='pyacomms@whoi.edu, cfitzgerald@whoi.edu',
     packages=['acomms', 'acomms.modem_connections', 'bin',],
     url='http://acomms.whoi.edu/',
     license='LGPLv3+',
     description='WHOI Micromodem Interface Library and Tools',
     long_description=read('README.txt'),
```

