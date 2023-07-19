# Comparing `tmp/PySocketLib-0.3.tar.gz` & `tmp/PySocketLib-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySocketLib-0.3.tar", last modified: Mon Jul 17 11:18:43 2023, max compression
+gzip compressed data, was "PySocketLib-0.3.1.tar", last modified: Tue Jul 18 11:21:53 2023, max compression
```

## Comparing `PySocketLib-0.3.tar` & `PySocketLib-0.3.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-17 11:18:43.216003 PySocketLib-0.3/
--rw-rw-r--   0 igors     (1000) igors     (1000)     1070 2023-07-17 11:03:51.000000 PySocketLib-0.3/LICENSE
--rw-rw-r--   0 igors     (1000) igors     (1000)     1145 2023-07-17 11:18:43.216003 PySocketLib-0.3/PKG-INFO
--rw-rw-r--   0 igors     (1000) igors     (1000)      621 2023-07-17 11:16:00.000000 PySocketLib-0.3/README.md
--rw-rw-r--   0 igors     (1000) igors     (1000)      509 2023-07-17 11:03:17.000000 PySocketLib-0.3/pyproject.toml
--rw-rw-r--   0 igors     (1000) igors     (1000)       38 2023-07-17 11:18:43.216003 PySocketLib-0.3/setup.cfg
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-17 11:18:43.212003 PySocketLib-0.3/src/
--rw-rw-r--   0 igors     (1000) igors     (1000)      351 2023-07-17 10:27:23.000000 PySocketLib-0.3/src/ExampleClient.py
--rw-rw-r--   0 igors     (1000) igors     (1000)      537 2023-07-17 09:50:41.000000 PySocketLib-0.3/src/ExampleServer.py
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-17 11:18:43.212003 PySocketLib-0.3/src/PySocketLib/
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-17 11:18:43.212003 PySocketLib-0.3/src/PySocketLib/CExceptions/
--rw-rw-r--   0 igors     (1000) igors     (1000)       36 2023-06-01 17:51:49.000000 PySocketLib-0.3/src/PySocketLib/CExceptions/InitExceptions.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       37 2023-07-15 13:04:00.000000 PySocketLib-0.3/src/PySocketLib/CExceptions/ProtocolExceptions.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       95 2023-07-17 09:15:35.000000 PySocketLib-0.3/src/PySocketLib/CExceptions/RunTime.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       83 2023-07-16 12:01:42.000000 PySocketLib-0.3/src/PySocketLib/CExceptions/__init__.py
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-17 11:18:43.216003 PySocketLib-0.3/src/PySocketLib/Client/
--rw-rw-r--   0 igors     (1000) igors     (1000)      674 2023-07-16 12:30:42.000000 PySocketLib-0.3/src/PySocketLib/Client/Client.py
--rw-rw-r--   0 igors     (1000) igors     (1000)      438 2023-07-16 06:23:18.000000 PySocketLib-0.3/src/PySocketLib/Client/ConnectedClient.py
--rw-rw-r--   0 igors     (1000) igors     (1000)     1411 2023-07-16 12:34:03.000000 PySocketLib-0.3/src/PySocketLib/Client/TCPClient.py
--rw-rw-r--   0 igors     (1000) igors     (1000)     1507 2023-07-17 10:43:54.000000 PySocketLib-0.3/src/PySocketLib/Client/UDPClient.py
--rw-rw-r--   0 igors     (1000) igors     (1000)      177 2023-06-11 13:47:22.000000 PySocketLib-0.3/src/PySocketLib/Client/__init__.py
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-17 11:18:43.216003 PySocketLib-0.3/src/PySocketLib/Server/
--rw-rw-r--   0 igors     (1000) igors     (1000)     4069 2023-07-17 09:50:52.000000 PySocketLib-0.3/src/PySocketLib/Server/Server.py
--rw-rw-r--   0 igors     (1000) igors     (1000)     3518 2023-07-17 09:51:12.000000 PySocketLib-0.3/src/PySocketLib/Server/TCPServer.py
--rw-rw-r--   0 igors     (1000) igors     (1000)     2504 2023-07-17 10:44:38.000000 PySocketLib-0.3/src/PySocketLib/Server/UDPServer.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       92 2023-07-15 14:41:30.000000 PySocketLib-0.3/src/PySocketLib/Server/__init__.py
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-17 11:18:43.216003 PySocketLib-0.3/src/PySocketLib/Utility/
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-17 11:18:43.216003 PySocketLib-0.3/src/PySocketLib/Utility/Protocol/
--rw-rw-r--   0 igors     (1000) igors     (1000)       68 2023-06-11 12:59:17.000000 PySocketLib-0.3/src/PySocketLib/Utility/Protocol/Protocol.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       30 2023-06-11 12:28:03.000000 PySocketLib-0.3/src/PySocketLib/Utility/Protocol/__init__.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       22 2023-06-11 12:28:52.000000 PySocketLib-0.3/src/PySocketLib/Utility/__init__.py
--rw-rw-r--   0 igors     (1000) igors     (1000)       89 2023-06-11 12:28:40.000000 PySocketLib-0.3/src/PySocketLib/__init__.py
-drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-17 11:18:43.212003 PySocketLib-0.3/src/PySocketLib.egg-info/
--rw-rw-r--   0 igors     (1000) igors     (1000)     1145 2023-07-17 11:18:43.000000 PySocketLib-0.3/src/PySocketLib.egg-info/PKG-INFO
--rw-rw-r--   0 igors     (1000) igors     (1000)      881 2023-07-17 11:18:43.000000 PySocketLib-0.3/src/PySocketLib.egg-info/SOURCES.txt
--rw-rw-r--   0 igors     (1000) igors     (1000)        1 2023-07-17 11:18:43.000000 PySocketLib-0.3/src/PySocketLib.egg-info/dependency_links.txt
--rw-rw-r--   0 igors     (1000) igors     (1000)       40 2023-07-17 11:18:43.000000 PySocketLib-0.3/src/PySocketLib.egg-info/top_level.txt
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-18 11:21:53.877819 PySocketLib-0.3.1/
+-rw-rw-r--   0 igors     (1000) igors     (1000)     1070 2023-07-17 11:03:51.000000 PySocketLib-0.3.1/LICENSE
+-rw-rw-r--   0 igors     (1000) igors     (1000)     1147 2023-07-18 11:21:53.877819 PySocketLib-0.3.1/PKG-INFO
+-rw-rw-r--   0 igors     (1000) igors     (1000)      621 2023-07-17 11:16:00.000000 PySocketLib-0.3.1/README.md
+-rw-rw-r--   0 igors     (1000) igors     (1000)      511 2023-07-18 11:21:24.000000 PySocketLib-0.3.1/pyproject.toml
+-rw-rw-r--   0 igors     (1000) igors     (1000)       38 2023-07-18 11:21:53.877819 PySocketLib-0.3.1/setup.cfg
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-18 11:21:53.873819 PySocketLib-0.3.1/src/
+-rw-rw-r--   0 igors     (1000) igors     (1000)      351 2023-07-17 11:45:32.000000 PySocketLib-0.3.1/src/ExampleClient.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)      971 2023-07-17 11:47:31.000000 PySocketLib-0.3.1/src/ExampleServer.py
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-18 11:21:53.873819 PySocketLib-0.3.1/src/PySocketLib/
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-18 11:21:53.873819 PySocketLib-0.3.1/src/PySocketLib/CExceptions/
+-rw-rw-r--   0 igors     (1000) igors     (1000)       36 2023-06-01 17:51:49.000000 PySocketLib-0.3.1/src/PySocketLib/CExceptions/InitExceptions.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       37 2023-07-15 13:04:00.000000 PySocketLib-0.3.1/src/PySocketLib/CExceptions/ProtocolExceptions.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       95 2023-07-17 09:15:35.000000 PySocketLib-0.3.1/src/PySocketLib/CExceptions/RunTime.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       83 2023-07-16 12:01:42.000000 PySocketLib-0.3.1/src/PySocketLib/CExceptions/__init__.py
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-18 11:21:53.877819 PySocketLib-0.3.1/src/PySocketLib/Client/
+-rw-rw-r--   0 igors     (1000) igors     (1000)      674 2023-07-16 12:30:42.000000 PySocketLib-0.3.1/src/PySocketLib/Client/Client.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)      438 2023-07-16 06:23:18.000000 PySocketLib-0.3.1/src/PySocketLib/Client/ConnectedClient.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)     1411 2023-07-16 12:34:03.000000 PySocketLib-0.3.1/src/PySocketLib/Client/TCPClient.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)     1507 2023-07-17 10:43:54.000000 PySocketLib-0.3.1/src/PySocketLib/Client/UDPClient.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)      177 2023-06-11 13:47:22.000000 PySocketLib-0.3.1/src/PySocketLib/Client/__init__.py
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-18 11:21:53.877819 PySocketLib-0.3.1/src/PySocketLib/Server/
+-rw-rw-r--   0 igors     (1000) igors     (1000)     4174 2023-07-17 13:16:11.000000 PySocketLib-0.3.1/src/PySocketLib/Server/Server.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)     3535 2023-07-17 13:23:15.000000 PySocketLib-0.3.1/src/PySocketLib/Server/TCPServer.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)     2549 2023-07-18 07:15:20.000000 PySocketLib-0.3.1/src/PySocketLib/Server/UDPServer.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       92 2023-07-15 14:41:30.000000 PySocketLib-0.3.1/src/PySocketLib/Server/__init__.py
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-18 11:21:53.877819 PySocketLib-0.3.1/src/PySocketLib/Utility/
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-18 11:21:53.877819 PySocketLib-0.3.1/src/PySocketLib/Utility/Protocol/
+-rw-rw-r--   0 igors     (1000) igors     (1000)       68 2023-06-11 12:59:17.000000 PySocketLib-0.3.1/src/PySocketLib/Utility/Protocol/Protocol.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       30 2023-06-11 12:28:03.000000 PySocketLib-0.3.1/src/PySocketLib/Utility/Protocol/__init__.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       22 2023-06-11 12:28:52.000000 PySocketLib-0.3.1/src/PySocketLib/Utility/__init__.py
+-rw-rw-r--   0 igors     (1000) igors     (1000)       89 2023-06-11 12:28:40.000000 PySocketLib-0.3.1/src/PySocketLib/__init__.py
+drwxrwxr-x   0 igors     (1000) igors     (1000)        0 2023-07-18 11:21:53.873819 PySocketLib-0.3.1/src/PySocketLib.egg-info/
+-rw-rw-r--   0 igors     (1000) igors     (1000)     1147 2023-07-18 11:21:53.000000 PySocketLib-0.3.1/src/PySocketLib.egg-info/PKG-INFO
+-rw-rw-r--   0 igors     (1000) igors     (1000)      881 2023-07-18 11:21:53.000000 PySocketLib-0.3.1/src/PySocketLib.egg-info/SOURCES.txt
+-rw-rw-r--   0 igors     (1000) igors     (1000)        1 2023-07-18 11:21:53.000000 PySocketLib-0.3.1/src/PySocketLib.egg-info/dependency_links.txt
+-rw-rw-r--   0 igors     (1000) igors     (1000)       40 2023-07-18 11:21:53.000000 PySocketLib-0.3.1/src/PySocketLib.egg-info/top_level.txt
```

### Comparing `PySocketLib-0.3/LICENSE` & `PySocketLib-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PySocketLib-0.3/PKG-INFO` & `PySocketLib-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySocketLib
-Version: 0.3
+Version: 0.3.1
 Summary: Library to simplify working with socket
 Author-email: Samsonov Igor <ig.samsonov10@yandex.ru>
 Project-URL: Homepage, https://github.com/Minuta18/PySocketLib
 Project-URL: Bug Tracker, https://github.com/Minuta18/PySocketLib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PySocketLib-0.3/README.md` & `PySocketLib-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `PySocketLib-0.3/src/PySocketLib/Client/Client.py` & `PySocketLib-0.3.1/src/PySocketLib/Client/Client.py`

 * *Files identical despite different names*

### Comparing `PySocketLib-0.3/src/PySocketLib/Client/TCPClient.py` & `PySocketLib-0.3.1/src/PySocketLib/Client/TCPClient.py`

 * *Files identical despite different names*

### Comparing `PySocketLib-0.3/src/PySocketLib/Client/UDPClient.py` & `PySocketLib-0.3.1/src/PySocketLib/Client/UDPClient.py`

 * *Files identical despite different names*

### Comparing `PySocketLib-0.3/src/PySocketLib/Server/Server.py` & `PySocketLib-0.3.1/src/PySocketLib/Server/Server.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,33 +32,35 @@
         return f'[{self.date}] received from {self.from_} to {self.to}: {self.content}'
 
 class Server(ABC):
     '''Socket server abstract class'''
     def __init__(self,
         addr: tuple,             
         package_size: int=1024,
+        use_ipv6: bool=False,
     ):
         try:
             self._ip_addr, self._port = addr
             self._addr = addr
+            self._ipv6_using = use_ipv6
             self.package_size = package_size
         except ValueError as e:
             raise ValueError('Invalid address')
-        self._server_socket = self._server_socket_setup(addr)
+        self._server_socket = self._server_socket_setup(addr, use_ipv6=use_ipv6)
         self._socket_selector = self._selector_setup(self._server_socket)
         self._clients = dict()
         self._messages = list()
 
     @abstractmethod
     def __del__(self):
         '''Close all connections'''
         pass
 
     @abstractmethod
-    def _server_socket_setup(self, addr: tuple) -> socket.socket:
+    def _server_socket_setup(self, addr: tuple, use_ipv6=False) -> socket.socket:
         '''Setup server socket'''
         pass
 
     def _selector_setup(self, server_socket: socket.socket):
         '''Setup selector'''
 
         socket_selector = selectors.DefaultSelector()
```

### Comparing `PySocketLib-0.3/src/PySocketLib/Server/TCPServer.py` & `PySocketLib-0.3.1/src/PySocketLib/Server/TCPServer.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 from PySocketLib.Client import ConnectedTCPClient, ConnectedClient
 
 class TCPServer(Server):
     '''Simple TCP server'''
     def __init__(self,
         addr: tuple,             
         package_size: int=1024,
+        use_ipv6: bool=False,
     ):
         try:
             self._ip_addr, self._port = addr
             self._addr = addr
+            self._ipv6_using = use_ipv6
             self.package_size = package_size
         except ValueError as e:
             raise ValueError('Invalid address')
-        self._server_socket = self._server_socket_setup(addr)
+        self._server_socket = self._server_socket_setup(addr, use_ipv6=use_ipv6)
         self._socket_selector = self._selector_setup(self._server_socket)
         self._clients = dict()
         self._messages = list()
 
     def __del__(self):
         self._socket_selector.close()
 
@@ -51,22 +53,20 @@
                 self._messages.append(Message(
                     self._clients[conn].addr,
                     self._addr,
                     recv_data,
                     self.get_date(),
                 ))
 
-    def _server_socket_setup(self, addr: tuple) -> socket.socket:
+    def _server_socket_setup(self, addr: tuple, use_ipv6=False) -> socket.socket:
         sock = None
-        if len(addr) == 2:
+        if not use_ipv6:
             sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        elif len(addr) == 4:
-            sock = socket.socket(socket.AF_INET6, socket.SOCK_STREAM, 0)
         else:
-            raise ValueError(f'Invalid address: {addr}')
+            sock = socket.socket(socket.AF_INET6, socket.SOCK_STREAM, 0)
         
         sock.bind(addr)
         sock.listen()
         sock.setblocking(False)
 
         return sock
```

### Comparing `PySocketLib-0.3/src/PySocketLib/Server/UDPServer.py` & `PySocketLib-0.3.1/src/PySocketLib/Server/UDPServer.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,36 +8,36 @@
 from PySocketLib.Client import ConnectedClient, ConnectedTCPClient, ConnectedUDPClient
 from PySocketLib.Utility.Protocol import Protocol
 
 class UDPServer(Server):
     def __init__(self,
         addr: tuple,
         package_size: int=1024,
+        use_ipv6: bool=False
     ):
         try:
             self._ip_addr, self._port = addr
             self._addr = addr
+            self._ipv6_using = use_ipv6
             self.package_size = package_size
         except ValueError as e:
             raise ValueError('Invalid address')
-        self._server_socket = self._server_socket_setup(addr)
+        self._server_socket = self._server_socket_setup(addr, use_ipv6=use_ipv6)
         self._clients = dict()
         self._messages = list()
 
     def __del__(self):
         pass
 
-    def _server_socket_setup(self, addr: tuple) -> socket.socket:
+    def _server_socket_setup(self, addr: tuple, use_ipv6=False) -> socket.socket:
         sock = None
-        if len(addr) == 2:
-            sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-        elif len(addr) == 4:
-            sock = socket.socket(socket.AF_INET6, socket.SOCK_DGRAM, 0)
+        if not use_ipv6:
+            sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         else:
-            raise ValueError(f'Invalid address: {addr}')
+            sock = socket.socket(socket.AF_INET6, socket.SOCK_STREAM, 0)
         sock.bind(addr)
 
         return sock
 
     def _service_connection(self):
         data, addr = self._server_socket.recvfrom(self.package_size)
         if data != '' and data != None:
@@ -65,10 +65,11 @@
             self._addr,
             client.addr,
             edited_data,
             self.get_date(),
         )
         self._messages.append(new_message)
         self._server_socket.sendto(edited_data, client.addr)
+        return new_message
 
     def proceed(self):
         self._service_connection()
```

### Comparing `PySocketLib-0.3/src/PySocketLib.egg-info/PKG-INFO` & `PySocketLib-0.3.1/src/PySocketLib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySocketLib
-Version: 0.3
+Version: 0.3.1
 Summary: Library to simplify working with socket
 Author-email: Samsonov Igor <ig.samsonov10@yandex.ru>
 Project-URL: Homepage, https://github.com/Minuta18/PySocketLib
 Project-URL: Bug Tracker, https://github.com/Minuta18/PySocketLib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PySocketLib-0.3/src/PySocketLib.egg-info/SOURCES.txt` & `PySocketLib-0.3.1/src/PySocketLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

