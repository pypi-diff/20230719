# Comparing `tmp/vocalhost-1.1.3.tar.gz` & `tmp/vocalhost-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocalhost-1.1.3.tar", last modified: Wed Jul 19 14:34:45 2023, max compression
+gzip compressed data, was "vocalhost-1.1.4.tar", last modified: Wed Jul 19 15:26:21 2023, max compression
```

## Comparing `vocalhost-1.1.3.tar` & `vocalhost-1.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:34:45.642766 vocalhost-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-19 14:34:45.642766 vocalhost-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-19 14:34:33.000000 vocalhost-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 14:34:45.642766 vocalhost-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-19 14:34:33.000000 vocalhost-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:34:45.642766 vocalhost-1.1.3/vocalhost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-19 14:34:45.000000 vocalhost-1.1.3/vocalhost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-19 14:34:45.000000 vocalhost-1.1.3/vocalhost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 14:34:45.000000 vocalhost-1.1.3/vocalhost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-19 14:34:45.000000 vocalhost-1.1.3/vocalhost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 14:34:45.000000 vocalhost-1.1.3/vocalhost.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-19 14:34:33.000000 vocalhost-1.1.3/vocalhost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:26:21.918559 vocalhost-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-19 15:26:21.918559 vocalhost-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-19 15:26:08.000000 vocalhost-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 15:26:21.918559 vocalhost-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-19 15:26:08.000000 vocalhost-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:26:21.918559 vocalhost-1.1.4/vocalhost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-19 15:26:21.000000 vocalhost-1.1.4/vocalhost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-19 15:26:21.000000 vocalhost-1.1.4/vocalhost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 15:26:21.000000 vocalhost-1.1.4/vocalhost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-19 15:26:21.000000 vocalhost-1.1.4/vocalhost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 15:26:21.000000 vocalhost-1.1.4/vocalhost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-19 15:26:08.000000 vocalhost-1.1.4/vocalhost.py
```

### Comparing `vocalhost-1.1.3/PKG-INFO` & `vocalhost-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocalhost
-Version: 1.1.3
+Version: 1.1.4
 Summary: Localhost to Vocalhost, run functions from anywhere
 Description-Content-Type: text/markdown
 
 # Vocalhost-python
 Vocalhost is a communication solution that enables direct and reliable connections between systems using WebSocket protocol. It comprises a bridge server and a client agent, offering support for a wide range of languages, frameworks, and systems. This versatility allows for seamless interaction and efficient data exchange across diverse environments.
 
 The bridge server acts as a central hub, relaying real-time messages between connected systems over WebSocket connections. The client agent establishes a WebSocket connection with the bridge server, facilitating communication across various platforms.
```

### Comparing `vocalhost-1.1.3/README.md` & `vocalhost-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `vocalhost-1.1.3/vocalhost.egg-info/PKG-INFO` & `vocalhost-1.1.4/vocalhost.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocalhost
-Version: 1.1.3
+Version: 1.1.4
 Summary: Localhost to Vocalhost, run functions from anywhere
 Description-Content-Type: text/markdown
 
 # Vocalhost-python
 Vocalhost is a communication solution that enables direct and reliable connections between systems using WebSocket protocol. It comprises a bridge server and a client agent, offering support for a wide range of languages, frameworks, and systems. This versatility allows for seamless interaction and efficient data exchange across diverse environments.
 
 The bridge server acts as a central hub, relaying real-time messages between connected systems over WebSocket connections. The client agent establishes a WebSocket connection with the bridge server, facilitating communication across various platforms.
```

### Comparing `vocalhost-1.1.3/vocalhost.py` & `vocalhost-1.1.4/vocalhost.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     async def _connect_to_server(client_id=None, auto_reconnect=None):
         ssl_context = ssl.create_default_context(cafile=certifi.where())
         ssl_context.verify_mode = ssl.CERT_REQUIRED
         remote_url = 'wss://vocalhost.reiserx.com/'
 
         try:
-            async with websockets.connect(remote_url+'ws/?client_id=' + client_id + '&api_key='+API_KEY, ssl=ssl_context) as websocket:
+            async with websockets.connect(remote_url+'ws/?client_id=' + client_id + '&api_key='+API_KEY, ssl=ssl_context, ping_interval=None) as websocket:
                 print("Connected: " + client_id)
                 Receiver.websocket = websocket
                 await Receiver.receive_message()
 
         except websockets.ConnectionClosedError as e:
             print(f"Connection closed: {e.code} {e}")
             if auto_reconnect is not None:
```

