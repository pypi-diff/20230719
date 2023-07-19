# Comparing `tmp/era_5g_client-0.4.0.tar.gz` & `tmp/era_5g_client-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "era_5g_client-0.4.0.tar", last modified: Mon Jul 17 13:05:24 2023, max compression
+gzip compressed data, was "era_5g_client-0.4.1.tar", last modified: Wed Jul 19 09:49:01 2023, max compression
```

## Comparing `era_5g_client-0.4.0.tar` & `era_5g_client-0.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 13:05:24.169156 era_5g_client-0.4.0/
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       12 2023-07-17 13:05:23.000000 era_5g_client-0.4.0/MANIFEST.in
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      420 2023-07-17 13:05:24.169156 era_5g_client-0.4.0/PKG-INFO
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      749 2023-07-17 13:05:23.000000 era_5g_client-0.4.0/backend_shim.py
-drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 13:05:24.169156 era_5g_client-0.4.0/era_5g_client/
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 13:05:23.000000 era_5g_client-0.4.0/era_5g_client/__init__.py
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)    11799 2023-07-17 13:05:23.000000 era_5g_client-0.4.0/era_5g_client/client.py
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     8530 2023-07-17 13:05:23.000000 era_5g_client-0.4.0/era_5g_client/client_base.py
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      523 2023-07-17 13:05:23.000000 era_5g_client-0.4.0/era_5g_client/dataclasses.py
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      662 2023-07-17 13:05:23.000000 era_5g_client-0.4.0/era_5g_client/exceptions.py
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     2715 2023-07-17 13:05:23.000000 era_5g_client-0.4.0/era_5g_client/middleware_resource_checker.py
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 13:05:23.000000 era_5g_client-0.4.0/era_5g_client/py.typed
-drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-17 13:05:24.169156 era_5g_client-0.4.0/era_5g_client.egg-info/
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      420 2023-07-17 13:05:24.000000 era_5g_client-0.4.0/era_5g_client.egg-info/PKG-INFO
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      470 2023-07-17 13:05:24.000000 era_5g_client-0.4.0/era_5g_client.egg-info/SOURCES.txt
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        1 2023-07-17 13:05:24.000000 era_5g_client-0.4.0/era_5g_client.egg-info/dependency_links.txt
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        1 2023-07-17 13:05:24.000000 era_5g_client-0.4.0/era_5g_client.egg-info/namespace_packages.txt
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      127 2023-07-17 13:05:24.000000 era_5g_client-0.4.0/era_5g_client.egg-info/requires.txt
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       14 2023-07-17 13:05:24.000000 era_5g_client-0.4.0/era_5g_client.egg-info/top_level.txt
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       38 2023-07-17 13:05:24.169156 era_5g_client-0.4.0/setup.cfg
--rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     1015 2023-07-17 13:05:23.000000 era_5g_client-0.4.0/setup.py
+drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-19 09:49:01.439323 era_5g_client-0.4.1/
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       12 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/MANIFEST.in
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      414 2023-07-19 09:49:01.439323 era_5g_client-0.4.1/PKG-INFO
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      749 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/backend_shim.py
+drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-19 09:49:01.439323 era_5g_client-0.4.1/era_5g_client/
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client/__init__.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)    11708 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client/client.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     8643 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client/client_base.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      523 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client/dataclasses.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      662 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client/exceptions.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     2715 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client/middleware_resource_checker.py
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client/py.typed
+drwxr-xr-x   0 ikapinus  (1000) ikapinus  (1000)        0 2023-07-19 09:49:01.439323 era_5g_client-0.4.1/era_5g_client.egg-info/
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      414 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client.egg-info/PKG-INFO
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      470 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client.egg-info/SOURCES.txt
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        1 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client.egg-info/dependency_links.txt
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)        1 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client.egg-info/namespace_packages.txt
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)      127 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client.egg-info/requires.txt
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       14 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/era_5g_client.egg-info/top_level.txt
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)       38 2023-07-19 09:49:01.439323 era_5g_client-0.4.1/setup.cfg
+-rw-r--r--   0 ikapinus  (1000) ikapinus  (1000)     1009 2023-07-19 09:49:01.000000 era_5g_client-0.4.1/setup.py
```

### Comparing `era_5g_client-0.4.0/backend_shim.py` & `era_5g_client-0.4.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `era_5g_client-0.4.0/era_5g_client/client.py` & `era_5g_client-0.4.1/era_5g_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 import logging
-import os
 from collections.abc import Callable
 from enum import Enum
 from typing import Dict, Optional
 
 import requests
 from requests import HTTPError
 
 from era_5g_client.client_base import NetAppClientBase
 from era_5g_client.dataclasses import MiddlewareInfo
 from era_5g_client.exceptions import FailedToConnect, NetAppNotReady
 from era_5g_client.middleware_resource_checker import MiddlewareResourceChecker
 
-# port of the netapp's server
-NETAPP_PORT = int(os.getenv("NETAPP_PORT", 5896))
-
 
 class RunTaskMode(Enum):
     # deploy the task but don't wait until it is ready, do not register with it
     DO_NOTHING = 1
     # wait until the netapp is ready, do not register with it
     WAIT = 2
     # wait until the netapp is ready and register with it afterwards
```

### Comparing `era_5g_client-0.4.0/era_5g_client/client_base.py` & `era_5g_client-0.4.1/era_5g_client/client_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 import socketio
 from socketio.exceptions import ConnectionError
 
 from era_5g_client.exceptions import FailedToConnect
 from era_5g_interface.dataclasses.control_command import ControlCmdType, ControlCommand
 from era_5g_interface.h264_encoder import H264Encoder, H264EncoderError
 
-logging.basicConfig()
-
 
 class NetAppClientBase:
     """Basic implementation of the NetApp client.
 
     It creates the Requests object with session and bind callbacks for
     connection info and results from the NetApp.
     """
@@ -51,15 +49,15 @@
 
         Raises:
             FailedToConnect: When connection to the middleware could not be set or
                 login failed
             FailedToObtainPlan: When the plan was not successfully returned from
                 the middleware
         """
-        self._sio = socketio.Client(logger=socketio_debug)
+        self._sio = socketio.Client(logger=socketio_debug, reconnection_attempts=1, handle_sigint=False)
         self.netapp_address: Union[str, None] = None
         self._sio.on("message", results_event, namespace="/results")
         self._sio.on("connect", self.on_connect_event, namespace="/results")
         self._sio.on("image_error", image_error_event, namespace="/data")
         self._sio.on("json_error", json_error_event, namespace="/data")
         self._sio.on("connect_error", self.on_connect_error, namespace="/results")
         self._sio.on("control_cmd_result", control_cmd_event, namespace="/control")
@@ -173,14 +171,15 @@
                 data["metadata"] = metadata
             self._sio.emit("image", data, "/data")
         except H264EncoderError as e:
             self.logger.error(f"H264 encoder error: {e}")
             self.disconnect()
             raise e
         except Exception as e:
+            # TODO: Create recovery sequence if server goes down and then starts up again
             self.logger.error(f"Send image emit error: {e}")
             self.disconnect()
             raise e
 
     def send_image_ws_raw(self, data: Dict):
         """Sends already encoded image data to /data namespace.
```

### Comparing `era_5g_client-0.4.0/era_5g_client/dataclasses.py` & `era_5g_client-0.4.1/era_5g_client/dataclasses.py`

 * *Files identical despite different names*

### Comparing `era_5g_client-0.4.0/era_5g_client/exceptions.py` & `era_5g_client-0.4.1/era_5g_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `era_5g_client-0.4.0/era_5g_client/middleware_resource_checker.py` & `era_5g_client-0.4.1/era_5g_client/middleware_resource_checker.py`

 * *Files identical despite different names*

### Comparing `era_5g_client-0.4.0/setup.py` & `era_5g_client-0.4.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
         'Operating System :: OS Independent',
         'Intended Audience :: Developers',
     ],
     'description': 'A client for 5G-ERA NetApps',
     'install_requires': (
-        'era-5g-interface~=0.4.0',
+        'era-5g-interface~=0.4.1',
         'numpy>=1.24.2',
         'opencv-python>=4.6.0.66',
         'python-socketio>=5.8.0',
         'requests>=2.28.2',
         'types-requests==2.31.0.1',
     ),
     'license': 'LGPL',
@@ -30,10 +30,10 @@
         'era_5g_client': (
             'py.typed',
         ),
     },
     'packages': (
         'era_5g_client',
     ),
-    'python_requires': '>=3.8,<3.11',
-    'version': '0.4.0',
+    'python_requires': '>=3.8',
+    'version': '0.4.1',
 })
```

