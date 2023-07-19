# Comparing `tmp/automation-utilities-1.3.7.tar.gz` & `tmp/automation-utilities-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation-utilities-1.3.7.tar", last modified: Wed Jul  5 16:30:53 2023, max compression
+gzip compressed data, was "automation-utilities-1.3.8.tar", last modified: Wed Jul 19 15:42:12 2023, max compression
```

## Comparing `automation-utilities-1.3.7.tar` & `automation-utilities-1.3.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 16:30:53.216412 automation-utilities-1.3.7/
-drwxrwxrwx   0        0        0        0 2023-07-05 16:30:53.214907 automation-utilities-1.3.7/Automation_Utilities.egg-info/
--rw-rw-rw-   0        0        0      134 2023-07-05 16:30:52.000000 automation-utilities-1.3.7/Automation_Utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      596 2023-07-05 16:30:52.000000 automation-utilities-1.3.7/Automation_Utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 16:30:52.000000 automation-utilities-1.3.7/Automation_Utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-05 16:30:52.000000 automation-utilities-1.3.7/Automation_Utilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-05 16:30:52.000000 automation-utilities-1.3.7/Automation_Utilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      134 2023-07-05 16:30:53.215907 automation-utilities-1.3.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-05 16:30:53.207900 automation-utilities-1.3.7/automation_utilities/
--rw-rw-rw-   0        0        0     1358 2023-07-02 20:29:10.000000 automation-utilities-1.3.7/automation_utilities/Data.py
--rw-rw-rw-   0        0        0      700 2023-07-03 15:16:47.000000 automation-utilities-1.3.7/automation_utilities/Files.py
--rw-rw-rw-   0        0        0      456 2023-07-04 17:58:58.000000 automation-utilities-1.3.7/automation_utilities/Generator.py
--rw-rw-rw-   0        0        0      147 2023-07-02 15:43:12.000000 automation-utilities-1.3.7/automation_utilities/Input.py
--rw-rw-rw-   0        0        0      835 2023-06-27 20:34:27.000000 automation-utilities-1.3.7/automation_utilities/PhoneNumbers.py
--rw-rw-rw-   0        0        0        0 2023-06-26 15:36:31.000000 automation-utilities-1.3.7/automation_utilities/__init__.py
--rw-rw-rw-   0        0        0       42 2023-07-05 16:30:53.216412 automation-utilities-1.3.7/setup.cfg
--rw-rw-rw-   0        0        0      271 2023-07-05 16:30:48.000000 automation-utilities-1.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:42:12.069236 automation-utilities-1.3.8/
+drwxrwxrwx   0        0        0        0 2023-07-19 15:42:12.068225 automation-utilities-1.3.8/Automation_Utilities.egg-info/
+-rw-rw-rw-   0        0        0      134 2023-07-19 15:42:11.000000 automation-utilities-1.3.8/Automation_Utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      596 2023-07-19 15:42:11.000000 automation-utilities-1.3.8/Automation_Utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 15:42:11.000000 automation-utilities-1.3.8/Automation_Utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-19 15:42:11.000000 automation-utilities-1.3.8/Automation_Utilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-19 15:42:11.000000 automation-utilities-1.3.8/Automation_Utilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      134 2023-07-19 15:42:12.069236 automation-utilities-1.3.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-19 15:42:12.062144 automation-utilities-1.3.8/automation_utilities/
+-rw-rw-rw-   0        0        0     1452 2023-07-16 17:33:33.000000 automation-utilities-1.3.8/automation_utilities/Data.py
+-rw-rw-rw-   0        0        0      936 2023-07-18 19:42:13.000000 automation-utilities-1.3.8/automation_utilities/Files.py
+-rw-rw-rw-   0        0        0      456 2023-07-04 17:58:58.000000 automation-utilities-1.3.8/automation_utilities/Generator.py
+-rw-rw-rw-   0        0        0      147 2023-07-02 15:43:12.000000 automation-utilities-1.3.8/automation_utilities/Input.py
+-rw-rw-rw-   0        0        0      835 2023-06-27 20:34:27.000000 automation-utilities-1.3.8/automation_utilities/PhoneNumbers.py
+-rw-rw-rw-   0        0        0        0 2023-06-26 15:36:31.000000 automation-utilities-1.3.8/automation_utilities/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-07-19 15:42:12.070459 automation-utilities-1.3.8/setup.cfg
+-rw-rw-rw-   0        0        0      271 2023-07-19 15:41:56.000000 automation-utilities-1.3.8/setup.py
```

### Comparing `automation-utilities-1.3.7/Automation_Utilities.egg-info/SOURCES.txt` & `automation-utilities-1.3.8/Automation_Utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automation-utilities-1.3.7/automation_utilities/Data.py` & `automation-utilities-1.3.8/automation_utilities/Data.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 
 class Data:
     lock = threading.Lock()
 
     def __init__(self, file_name: str):
         self.file_name = file_name
         try:
-            self.data = json.load(open(file_name, 'r'))
+            self.data = json.load(open(file_name, 'r', encoding='utf-8'))
         except FileNotFoundError:
             self.data = {}
         self._privte = 15
 
     def get(self, key, from_list: list = None, loop: bool = False):
         if key not in self.data.keys():
             self.data[key] = 0
         if isinstance(self.data[key], int):
             Data.lock.acquire()
             self.data[key] += 1
-            json.dump(self.data, open(self.file_name, 'w'), indent=2)
+            json.dump(self.data, open(self.file_name, 'w', encoding='utf-8'), indent=2, ensure_ascii=False)
             Data.lock.release()
             try:
                 return self.data[key] - 1 if from_list is None else from_list[self.data[key] - 1]
             except IndexError as IE:
                 if loop:
                     self.reset(key)
                     if len(from_list) > 0:
@@ -34,9 +34,9 @@
                     raise IE
         else:
             return self.data[key]
 
     def reset(self, key):
         self.data[key] = 0
         Data.lock.acquire()
-        json.dump(self.data, open(self.file_name, 'w'), indent=2)
+        json.dump(self.data, open(self.file_name, 'w', encoding='utf-8'), indent=2, ensure_ascii=False)
         Data.lock.release()
```

### Comparing `automation-utilities-1.3.7/automation_utilities/Files.py` & `automation-utilities-1.3.8/automation_utilities/Files.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import threading
 
 lock = threading.Lock()
 
 
 def add(text: str, to: str) -> None:
     lock.acquire()
@@ -9,19 +10,24 @@
     lock.release()
 
 
 def load(*file_names: str):
     lists = []
     for file_name in file_names:
         try:
-            lists.append(list(line.strip() for line in open(file_name, 'r').read().split('\n')))
+            lists.append(open(file_name, 'r').read().strip().split('\n'))
         except FileNotFoundError:
             open(file_name, 'w').write('')
             lists.append([])
     return lists if len(lists) > 1 else lists[0]
 
 
 def delete(text: str, from_file: str):
-    lock.acquire()
-    new_text = open(from_file, 'r').read().replace(text, '')
-    open(from_file, 'w').write(new_text)
-    lock.release()
+    with open(from_file, "r") as file_input:
+        with open("temp.txt", "w") as output:
+            # iterate all lines from file
+            for line in file_input.readlines():
+                # if text matches then don't write it
+                if line != text:
+                    output.write(line)
+    # replace file with original name
+    os.replace('temp.txt', from_file)
```

### Comparing `automation-utilities-1.3.7/automation_utilities/PhoneNumbers.py` & `automation-utilities-1.3.8/automation_utilities/PhoneNumbers.py`

 * *Files identical despite different names*

