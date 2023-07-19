# Comparing `tmp/brokersystem-0.2.4.tar.gz` & `tmp/brokersystem-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brokersystem-0.2.4.tar", last modified: Wed May 18 22:11:33 2022, max compression
+gzip compressed data, was "brokersystem-0.2.5.tar", last modified: Wed Jul 19 01:00:30 2023, max compression
```

## Comparing `brokersystem-0.2.4.tar` & `brokersystem-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2022-05-18 22:11:33.146967 brokersystem-0.2.4/
--rw-r--r--   0 shuntaro   (501) staff       (20)      743 2022-04-11 11:57:56.000000 brokersystem-0.2.4/LICENSE
--rw-r--r--   0 shuntaro   (501) staff       (20)     1018 2022-05-18 22:11:33.147107 brokersystem-0.2.4/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)      644 2022-05-09 02:38:48.000000 brokersystem-0.2.4/README.md
--rw-r--r--   0 shuntaro   (501) staff       (20)       93 2022-05-18 22:09:16.000000 brokersystem-0.2.4/pyproject.toml
--rw-r--r--   0 shuntaro   (501) staff       (20)      616 2022-05-18 22:11:33.147688 brokersystem-0.2.4/setup.cfg
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2022-05-18 22:11:33.139352 brokersystem-0.2.4/src/
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2022-05-18 22:11:33.143843 brokersystem-0.2.4/src/brokersystem/
--rw-r--r--   0 shuntaro   (501) staff       (20)      127 2022-04-25 04:35:08.000000 brokersystem-0.2.4/src/brokersystem/__init__.py
--rw-r--r--   0 shuntaro   (501) staff       (20)       49 2022-04-29 08:45:59.000000 brokersystem-0.2.4/src/brokersystem/__main__.py
--rw-r--r--   0 shuntaro   (501) staff       (20)       21 2022-05-18 22:02:17.000000 brokersystem-0.2.4/src/brokersystem/_version.py
--rw-r--r--   0 shuntaro   (501) staff       (20)    46453 2022-05-18 22:00:05.000000 brokersystem-0.2.4/src/brokersystem/agent.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2022-05-18 22:11:33.146691 brokersystem-0.2.4/src/brokersystem.egg-info/
--rw-r--r--   0 shuntaro   (501) staff       (20)     1018 2022-05-18 22:11:32.000000 brokersystem-0.2.4/src/brokersystem.egg-info/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)      354 2022-05-18 22:11:33.000000 brokersystem-0.2.4/src/brokersystem.egg-info/SOURCES.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        1 2022-05-18 22:11:32.000000 brokersystem-0.2.4/src/brokersystem.egg-info/dependency_links.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       51 2022-05-18 22:11:32.000000 brokersystem-0.2.4/src/brokersystem.egg-info/requires.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       13 2022-05-18 22:11:33.000000 brokersystem-0.2.4/src/brokersystem.egg-info/top_level.txt
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-19 01:00:30.542873 brokersystem-0.2.5/
+-rw-r--r--   0 shuntaro   (501) staff       (20)      743 2022-04-11 11:57:56.000000 brokersystem-0.2.5/LICENSE
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1018 2023-07-19 01:00:30.542947 brokersystem-0.2.5/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)      644 2022-05-09 02:38:48.000000 brokersystem-0.2.5/README.md
+-rw-r--r--   0 shuntaro   (501) staff       (20)       93 2022-05-18 22:09:16.000000 brokersystem-0.2.5/pyproject.toml
+-rw-r--r--   0 shuntaro   (501) staff       (20)      616 2023-07-19 01:00:30.543258 brokersystem-0.2.5/setup.cfg
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-19 01:00:30.539837 brokersystem-0.2.5/src/
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-19 01:00:30.541664 brokersystem-0.2.5/src/brokersystem/
+-rw-r--r--   0 shuntaro   (501) staff       (20)      127 2022-04-25 04:35:08.000000 brokersystem-0.2.5/src/brokersystem/__init__.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)       49 2022-04-23 12:22:57.000000 brokersystem-0.2.5/src/brokersystem/__main__.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)       21 2023-07-18 12:30:31.000000 brokersystem-0.2.5/src/brokersystem/_version.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)    46469 2023-07-18 12:30:04.000000 brokersystem-0.2.5/src/brokersystem/agent.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-19 01:00:30.542764 brokersystem-0.2.5/src/brokersystem.egg-info/
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1018 2023-07-19 01:00:30.000000 brokersystem-0.2.5/src/brokersystem.egg-info/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)      354 2023-07-19 01:00:30.000000 brokersystem-0.2.5/src/brokersystem.egg-info/SOURCES.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        1 2023-07-19 01:00:30.000000 brokersystem-0.2.5/src/brokersystem.egg-info/dependency_links.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       51 2023-07-19 01:00:30.000000 brokersystem-0.2.5/src/brokersystem.egg-info/requires.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       13 2023-07-19 01:00:30.000000 brokersystem-0.2.5/src/brokersystem.egg-info/top_level.txt
```

### Comparing `brokersystem-0.2.4/LICENSE` & `brokersystem-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `brokersystem-0.2.4/PKG-INFO` & `brokersystem-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brokersystem
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python module for communicating with brokersystem
 Author: chocolate
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `brokersystem-0.2.4/README.md` & `brokersystem-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `brokersystem-0.2.4/setup.cfg` & `brokersystem-0.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `brokersystem-0.2.4/src/brokersystem/agent.py` & `brokersystem-0.2.5/src/brokersystem/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,16 +190,18 @@
         format_dict = self.format_dict
         if isinstance(value, pd.DataFrame):
             value = value.to_dict(orient="list")
         elif (isinstance(value, list) and all([isinstance(x, dict) for x in value])) or (isinstance(value, dict) and all([isinstance(x, list) for x in value.values()])):
             value = pd.DataFrame(value).to_dict(orient="list") 
         else:
             raise Exception("The return value for table should be given by a list of dict, a dict of list or pandas DataFrame")
-        if self.graph is None and len(value.columns) >= 2:
-            format_dict["@repr"] = {"type": "graph", "key_x": value.columns[0], "key_y": value.columns[1]}
+        
+        keys = list(value.keys())
+        if self.graph is None and len(keys) >= 2:
+            format_dict["@repr"] = {"type": "graph", "key_x": keys[0], "key_y": keys[1]}
 
         return value, format_dict
             
 
 class TemplateContainer:
     def __init__(self, item_type):
         self._container_dict = {}
```

### Comparing `brokersystem-0.2.4/src/brokersystem.egg-info/PKG-INFO` & `brokersystem-0.2.5/src/brokersystem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brokersystem
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python module for communicating with brokersystem
 Author: chocolate
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

