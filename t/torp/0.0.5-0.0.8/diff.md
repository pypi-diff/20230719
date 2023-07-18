# Comparing `tmp/torp-0.0.5.tar.gz` & `tmp/torp-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torp-0.0.5.tar", last modified: Tue Jul 18 22:49:53 2023, max compression
+gzip compressed data, was "torp-0.0.8.tar", last modified: Tue Jul 18 23:15:09 2023, max compression
```

## Comparing `torp-0.0.5.tar` & `torp-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 sathya    (1000) sathya    (1000)        0 2023-07-18 22:49:53.445497 torp-0.0.5/
--rw-rw-r--   0 sathya    (1000) sathya    (1000)     1068 2023-07-18 04:39:01.000000 torp-0.0.5/LICENSE.txt
--rw-rw-r--   0 sathya    (1000) sathya    (1000)       74 2023-07-18 22:49:53.445497 torp-0.0.5/PKG-INFO
--rw-rw-r--   0 sathya    (1000) sathya    (1000)     1905 2023-07-18 05:00:57.000000 torp-0.0.5/README.md
--rw-rw-r--   0 sathya    (1000) sathya    (1000)       79 2023-07-18 22:49:53.445497 torp-0.0.5/setup.cfg
--rw-rw-r--   0 sathya    (1000) sathya    (1000)     1012 2023-07-18 22:49:49.000000 torp-0.0.5/setup.py
-drwxrwxr-x   0 sathya    (1000) sathya    (1000)        0 2023-07-18 22:49:53.441497 torp-0.0.5/torp/
--rw-rw-r--   0 sathya    (1000) sathya    (1000)      790 2023-07-18 22:49:41.000000 torp-0.0.5/torp/__init__.py
--rw-rw-r--   0 sathya    (1000) sathya    (1000)    14081 2023-07-17 22:23:26.000000 torp-0.0.5/torp/helper.py
-drwxrwxr-x   0 sathya    (1000) sathya    (1000)        0 2023-07-18 22:49:53.445497 torp-0.0.5/torp.egg-info/
--rw-rw-r--   0 sathya    (1000) sathya    (1000)       74 2023-07-18 22:49:53.000000 torp-0.0.5/torp.egg-info/PKG-INFO
--rw-rw-r--   0 sathya    (1000) sathya    (1000)      184 2023-07-18 22:49:53.000000 torp-0.0.5/torp.egg-info/SOURCES.txt
--rw-rw-r--   0 sathya    (1000) sathya    (1000)        1 2023-07-18 22:49:53.000000 torp-0.0.5/torp.egg-info/dependency_links.txt
--rw-rw-r--   0 sathya    (1000) sathya    (1000)        5 2023-07-18 22:49:53.000000 torp-0.0.5/torp.egg-info/top_level.txt
+drwxrwxr-x   0 sathya    (1000) sathya    (1000)        0 2023-07-18 23:15:09.422075 torp-0.0.8/
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)     1068 2023-07-18 04:39:01.000000 torp-0.0.8/LICENSE.txt
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)       74 2023-07-18 23:15:09.422075 torp-0.0.8/PKG-INFO
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)     1905 2023-07-18 05:00:57.000000 torp-0.0.8/README.md
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)       79 2023-07-18 23:15:09.422075 torp-0.0.8/setup.cfg
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)     1012 2023-07-18 23:13:27.000000 torp-0.0.8/setup.py
+drwxrwxr-x   0 sathya    (1000) sathya    (1000)        0 2023-07-18 23:15:09.418075 torp-0.0.8/torp/
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)      790 2023-07-18 22:49:41.000000 torp-0.0.8/torp/__init__.py
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)    14081 2023-07-17 22:23:26.000000 torp-0.0.8/torp/helper.py
+drwxrwxr-x   0 sathya    (1000) sathya    (1000)        0 2023-07-18 23:15:09.422075 torp-0.0.8/torp.egg-info/
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)       74 2023-07-18 23:15:09.000000 torp-0.0.8/torp.egg-info/PKG-INFO
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)      184 2023-07-18 23:15:09.000000 torp-0.0.8/torp.egg-info/SOURCES.txt
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)        1 2023-07-18 23:15:09.000000 torp-0.0.8/torp.egg-info/dependency_links.txt
+-rw-rw-r--   0 sathya    (1000) sathya    (1000)        5 2023-07-18 23:15:09.000000 torp-0.0.8/torp.egg-info/top_level.txt
```

### Comparing `torp-0.0.5/LICENSE.txt` & `torp-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `torp-0.0.5/README.md` & `torp-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `torp-0.0.5/setup.py` & `torp-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,8 +26,8 @@
     requirement_path = lib_folder + './requirements.txt'
     install_requires = []
 
     if os.path.isfile(requirement_path):
         with open(requirement_path) as f:
             install_requires = f.read().splitlines()
     print(install_requires)
-    setup(name="torp", version='0.0.5',install_requires=install_requires)
+    setup(name="torp", version='0.0.8',install_requires=install_requires)
```

### Comparing `torp-0.0.5/torp/__init__.py` & `torp-0.0.8/torp/__init__.py`

 * *Files identical despite different names*

### Comparing `torp-0.0.5/torp/helper.py` & `torp-0.0.8/torp/helper.py`

 * *Files identical despite different names*

