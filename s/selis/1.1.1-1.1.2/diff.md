# Comparing `tmp/selis-1.1.1.tar.gz` & `tmp/selis-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selis-1.1.1.tar", last modified: Wed Jul 12 16:06:16 2023, max compression
+gzip compressed data, was "selis-1.1.2.tar", last modified: Wed Jul 19 13:20:52 2023, max compression
```

## Comparing `selis-1.1.1.tar` & `selis-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-07-12 16:06:16.082054 selis-1.1.1/
--rw-r--r--   0 client     (501) staff       (20)      130 2023-07-12 16:06:16.081936 selis-1.1.1/PKG-INFO
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-07-12 16:06:16.080691 selis-1.1.1/selis/
--rw-r--r--   0 client     (501) staff       (20)        0 2023-06-24 12:32:58.000000 selis-1.1.1/selis/__init__.py
--rw-r--r--   0 client     (501) staff       (20)     4077 2023-07-12 16:04:07.000000 selis-1.1.1/selis/client.py
--rw-r--r--   0 client     (501) staff       (20)      653 2023-07-12 16:02:51.000000 selis-1.1.1/selis/computerinfo.py
--rw-r--r--   0 client     (501) staff       (20)     1159 2023-07-12 16:02:42.000000 selis-1.1.1/selis/selis.py
--rw-r--r--   0 client     (501) staff       (20)      514 2023-07-12 16:04:03.000000 selis-1.1.1/selis/utils.py
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-07-12 16:06:16.081728 selis-1.1.1/selis.egg-info/
--rw-r--r--   0 client     (501) staff       (20)      130 2023-07-12 16:06:16.000000 selis-1.1.1/selis.egg-info/PKG-INFO
--rw-r--r--   0 client     (501) staff       (20)      270 2023-07-12 16:06:16.000000 selis-1.1.1/selis.egg-info/SOURCES.txt
--rw-r--r--   0 client     (501) staff       (20)        1 2023-07-12 16:06:16.000000 selis-1.1.1/selis.egg-info/dependency_links.txt
--rw-r--r--   0 client     (501) staff       (20)       44 2023-07-12 16:06:16.000000 selis-1.1.1/selis.egg-info/entry_points.txt
--rw-r--r--   0 client     (501) staff       (20)        9 2023-07-12 16:06:16.000000 selis-1.1.1/selis.egg-info/requires.txt
--rw-r--r--   0 client     (501) staff       (20)        6 2023-07-12 16:06:16.000000 selis-1.1.1/selis.egg-info/top_level.txt
--rw-r--r--   0 client     (501) staff       (20)       38 2023-07-12 16:06:16.082098 selis-1.1.1/setup.cfg
--rw-r--r--   0 client     (501) staff       (20)      256 2023-07-12 16:06:08.000000 selis-1.1.1/setup.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-07-19 13:20:52.259243 selis-1.1.2/
+-rw-r--r--   0 client     (501) staff       (20)      130 2023-07-19 13:20:52.259114 selis-1.1.2/PKG-INFO
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-07-19 13:20:52.253087 selis-1.1.2/selis/
+-rw-r--r--   0 client     (501) staff       (20)        0 2023-06-24 12:32:58.000000 selis-1.1.2/selis/__init__.py
+-rw-r--r--   0 client     (501) staff       (20)     4873 2023-07-19 13:19:25.000000 selis-1.1.2/selis/client.py
+-rw-r--r--   0 client     (501) staff       (20)      653 2023-07-19 13:20:08.000000 selis-1.1.2/selis/computerinfo.py
+-rw-r--r--   0 client     (501) staff       (20)     1568 2023-07-19 13:20:17.000000 selis-1.1.2/selis/selis.py
+-rw-r--r--   0 client     (501) staff       (20)      507 2023-07-19 13:19:56.000000 selis-1.1.2/selis/utils.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-07-19 13:20:52.258833 selis-1.1.2/selis.egg-info/
+-rw-r--r--   0 client     (501) staff       (20)      130 2023-07-19 13:20:52.000000 selis-1.1.2/selis.egg-info/PKG-INFO
+-rw-r--r--   0 client     (501) staff       (20)      270 2023-07-19 13:20:52.000000 selis-1.1.2/selis.egg-info/SOURCES.txt
+-rw-r--r--   0 client     (501) staff       (20)        1 2023-07-19 13:20:52.000000 selis-1.1.2/selis.egg-info/dependency_links.txt
+-rw-r--r--   0 client     (501) staff       (20)       44 2023-07-19 13:20:52.000000 selis-1.1.2/selis.egg-info/entry_points.txt
+-rw-r--r--   0 client     (501) staff       (20)        9 2023-07-19 13:20:52.000000 selis-1.1.2/selis.egg-info/requires.txt
+-rw-r--r--   0 client     (501) staff       (20)        6 2023-07-19 13:20:52.000000 selis-1.1.2/selis.egg-info/top_level.txt
+-rw-r--r--   0 client     (501) staff       (20)       38 2023-07-19 13:20:52.259352 selis-1.1.2/setup.cfg
+-rw-r--r--   0 client     (501) staff       (20)      256 2023-07-19 13:20:28.000000 selis-1.1.2/setup.py
```

### Comparing `selis-1.1.1/selis/client.py` & `selis-1.1.2/selis/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,65 @@
 import socket
 import threading
 import sys
 import getpass
+import time
 
-from selis.computerinfo import ComputerInfo
-from selis.utils import *
+from module.client.computerinfo import ComputerInfo
+from module.utils.utils import *
 
 
 class ChatClient:
-    def __init__(self, ip, port, nickname):
+    def __init__(self, ip, port, nickname, password=None):
         self.connection = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         try:
             self.connection.connect((ip, port))
             self.connection.settimeout(None)
-        except:
-            print(f"\033[91m[-] Sever not found\033[0m")
+        except ConnectionRefusedError:
+            print("\033[91m[-] Server not found\033[0m")
             sys.exit()
 
+        self.password = str(password)
         self.nickname = nickname
         self.send_client_info_to_server()
         self.is_running = True
 
 
     def send_client_info_to_server(self):
         client_computer = ComputerInfo()
         info = client_computer.get()
-        msg = self.nickname + "/" + info
+        msg = self.password + "/" + self.nickname + "/" + info
 
         self.send_message(msg)
 
 
     def process_admin_mode(self):
-        password = getpass.getpass("\033[1m[*] Admin's Password: \n>> \033[0m")
+        password = getpass.getpass("\033[1m[*] Admin's Password: \033[0m")
         msg = "/check-admin " + self.nickname + " " + password
         self.send_message(msg)
 
 
     def send_message(self, message):
         self.connection.send(message.encode())
 
 
     def receive_message(self):
         return self.connection.recv(1024).decode()
 
 
     def exit(self):
         self.is_running = False
+        self.connection.close()
         guide_to_exit()
+
+
+    def left(self):
+        self.send_message(f"client/exit {self.nickname}")
+        print("\033[0m[+] You left the room")
+        time.sleep(0.4)
         self.connection.close()
 
 
     def process_receiving_message(self):
         try:
             while True:
                 response = self.receive_message()
@@ -58,44 +67,59 @@
                 if response:
                     my_message = f">>> {self.nickname}:"
 
                     if my_message in response:
                         continue
 
 
-                    if "admin/open-url" in response:
+                    elif "admin/open-url" in response:
                         url = response.split(" ")[1]
                         open_url(url)
 
                     elif response == "system/exist_nickname":
-                        print("\033[91m[!] This nickname already exists\033[0m")
+                        print("\033[91m\033[1m[!] This nickname already exists\033[0m")
                         self.exit()
                         break
 
                     elif response == "admin/close":
-                        print("\033[91m[-] Server is not available\033[0m")
+                        print("\033[91m\033[1m[-] You are kicked\033[0m")
                         self.exit()
                         break
 
                     elif response == "admin/ban&kick":
-                        print("\033[91m[-] Server is not available\033[0m")
+                        print("\033[91m\033[1m[-] You are kicked\033[0m")
+                        self.exit()
+                        break
+
+                    elif response == "admin/r-password":
+                        print("\033[91m\033[1m[-] This room requires a password\033[0m")
+                        self.exit()
+                        break
+
+                    elif response == "admin/w-password":
+                        print("\033[91m\033[1m[-] Wrong password !\033[0m")
                         self.exit()
                         break
 
                     elif response == "admin/close-server":
                         print("\033[91m\033[1m[-] Admin closes the server\033[0m")
                         self.exit()
                         break
 
                     else:
                         print(response)
 
-        except:
+        except ConnectionResetError:
+            print("\033[91m[-] Server is not available\033[0m")
+            guide_to_exit()
+            self.is_running = False
+            sys.exit(0)
+
+        except OSError:
             print("\033[91m[-] Connection is closed\033[0m")
-            self.connection.close()
             self.is_running = False
             sys.exit(0)
 
 
     def process_sending_message(self):
         try:
             while True:
@@ -103,16 +127,15 @@
 
                 if self.is_running:
                     if content == "":
                         print("\033[91m[-] Typing something before sending\033[0m")
                         continue
 
                     elif content == "/exit":
-                        self.send_message(f"client/exit {self.nickname}")
-                        self.connection.close()
+                        self.left()
                         break
 
                     elif content == "/clear":
                         clear_screen()
 
                     elif content == "/admin":
                         self.process_admin_mode()
```

### Comparing `selis-1.1.1/selis/computerinfo.py` & `selis-1.1.2/selis/computerinfo.py`

 * *Files identical despite different names*

