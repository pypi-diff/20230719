# Comparing `tmp/vocalhost-1.1.1.tar.gz` & `tmp/vocalhost-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocalhost-1.1.1.tar", last modified: Tue Jul 18 19:06:22 2023, max compression
+gzip compressed data, was "vocalhost-1.1.2.tar", last modified: Tue Jul 18 19:11:24 2023, max compression
```

## Comparing `vocalhost-1.1.1.tar` & `vocalhost-1.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:06:22.478650 vocalhost-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-18 19:06:22.478650 vocalhost-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-18 19:06:10.000000 vocalhost-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:06:22.478650 vocalhost-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-18 19:06:10.000000 vocalhost-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:06:22.474650 vocalhost-1.1.1/vocalhost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-18 19:06:22.000000 vocalhost-1.1.1/vocalhost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-18 19:06:22.000000 vocalhost-1.1.1/vocalhost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:06:22.000000 vocalhost-1.1.1/vocalhost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 19:06:22.000000 vocalhost-1.1.1/vocalhost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 19:06:22.000000 vocalhost-1.1.1/vocalhost.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-18 19:06:10.000000 vocalhost-1.1.1/vocalhost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:11:24.163749 vocalhost-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-18 19:11:24.163749 vocalhost-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-18 19:11:09.000000 vocalhost-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:11:24.163749 vocalhost-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-18 19:11:09.000000 vocalhost-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:11:24.163749 vocalhost-1.1.2/vocalhost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-18 19:11:24.000000 vocalhost-1.1.2/vocalhost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-18 19:11:24.000000 vocalhost-1.1.2/vocalhost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:11:24.000000 vocalhost-1.1.2/vocalhost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 19:11:24.000000 vocalhost-1.1.2/vocalhost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 19:11:24.000000 vocalhost-1.1.2/vocalhost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-18 19:11:09.000000 vocalhost-1.1.2/vocalhost.py
```

### Comparing `vocalhost-1.1.1/PKG-INFO` & `vocalhost-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocalhost
-Version: 1.1.1
+Version: 1.1.2
 Summary: Localhost to Vocalhost, run functions from anywhere
 Description-Content-Type: text/markdown
 
 # Vocalhost-python
 Vocalhost is a communication solution that enables direct and reliable connections between systems using WebSocket protocol. It comprises a bridge server and a client agent, offering support for a wide range of languages, frameworks, and systems. This versatility allows for seamless interaction and efficient data exchange across diverse environments.
 
 The bridge server acts as a central hub, relaying real-time messages between connected systems over WebSocket connections. The client agent establishes a WebSocket connection with the bridge server, facilitating communication across various platforms.
```

### Comparing `vocalhost-1.1.1/README.md` & `vocalhost-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `vocalhost-1.1.1/vocalhost.egg-info/PKG-INFO` & `vocalhost-1.1.2/vocalhost.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocalhost
-Version: 1.1.1
+Version: 1.1.2
 Summary: Localhost to Vocalhost, run functions from anywhere
 Description-Content-Type: text/markdown
 
 # Vocalhost-python
 Vocalhost is a communication solution that enables direct and reliable connections between systems using WebSocket protocol. It comprises a bridge server and a client agent, offering support for a wide range of languages, frameworks, and systems. This versatility allows for seamless interaction and efficient data exchange across diverse environments.
 
 The bridge server acts as a central hub, relaying real-time messages between connected systems over WebSocket connections. The client agent establishes a WebSocket connection with the bridge server, facilitating communication across various platforms.
```

### Comparing `vocalhost-1.1.1/vocalhost.py` & `vocalhost-1.1.2/vocalhost.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         except websockets.ConnectionClosedError as e:
             print(f"Connection closed: {e.code} {e.reason}")
             if auto_reconnect:
                 if e.code == 4000 or e.code == 4001 or e.code == 4002:
                     pass
                 else:
                      print("Reconnecting...")
-                     await asyncio.sleep(5)
+                     await asyncio.sleep(30 * 60)
                      await Receiver._connect_to_server(client_id=client_id)
             
     def connect(client_id=None, auto_reconnect=False):
         asyncio.run(Receiver._connect_to_server(client_id=client_id, auto_reconnect=auto_reconnect))
 
 
 class Request:
```

