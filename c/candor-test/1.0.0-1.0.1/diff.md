# Comparing `tmp/candor-test-1.0.0.tar.gz` & `tmp/candor-test-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "candor-test-1.0.0.tar", last modified: Tue Jul 18 22:06:03 2023, max compression
+gzip compressed data, was "candor-test-1.0.1.tar", last modified: Tue Jul 18 22:09:18 2023, max compression
```

## Comparing `candor-test-1.0.0.tar` & `candor-test-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 jbeal      (501) staff       (20)        0 2023-07-18 22:06:03.863953 candor-test-1.0.0/
--rw-r--r--   0 jbeal      (501) staff       (20)     1137 2023-07-18 22:06:03.863836 candor-test-1.0.0/PKG-INFO
--rw-r--r--   0 jbeal      (501) staff       (20)      871 2023-07-18 21:57:50.000000 candor-test-1.0.0/README.md
-drwxr-xr-x   0 jbeal      (501) staff       (20)        0 2023-07-18 22:06:03.863617 candor-test-1.0.0/candor_test.egg-info/
--rw-r--r--   0 jbeal      (501) staff       (20)     1137 2023-07-18 22:06:03.000000 candor-test-1.0.0/candor_test.egg-info/PKG-INFO
--rw-r--r--   0 jbeal      (501) staff       (20)      192 2023-07-18 22:06:03.000000 candor-test-1.0.0/candor_test.egg-info/SOURCES.txt
--rw-r--r--   0 jbeal      (501) staff       (20)        1 2023-07-18 22:06:03.000000 candor-test-1.0.0/candor_test.egg-info/dependency_links.txt
--rw-r--r--   0 jbeal      (501) staff       (20)        9 2023-07-18 22:06:03.000000 candor-test-1.0.0/candor_test.egg-info/requires.txt
--rw-r--r--   0 jbeal      (501) staff       (20)        1 2023-07-18 22:06:03.000000 candor-test-1.0.0/candor_test.egg-info/top_level.txt
--rw-r--r--   0 jbeal      (501) staff       (20)       38 2023-07-18 22:06:03.864003 candor-test-1.0.0/setup.cfg
--rw-r--r--   0 jbeal      (501) staff       (20)      467 2023-07-18 22:05:43.000000 candor-test-1.0.0/setup.py
+drwxr-xr-x   0 jbeal      (501) staff       (20)        0 2023-07-18 22:09:18.374266 candor-test-1.0.1/
+-rw-r--r--   0 jbeal      (501) staff       (20)     1137 2023-07-18 22:09:18.374147 candor-test-1.0.1/PKG-INFO
+-rw-r--r--   0 jbeal      (501) staff       (20)      871 2023-07-18 21:57:50.000000 candor-test-1.0.1/README.md
+drwxr-xr-x   0 jbeal      (501) staff       (20)        0 2023-07-18 22:09:18.373925 candor-test-1.0.1/candor_test.egg-info/
+-rw-r--r--   0 jbeal      (501) staff       (20)     1137 2023-07-18 22:09:18.000000 candor-test-1.0.1/candor_test.egg-info/PKG-INFO
+-rw-r--r--   0 jbeal      (501) staff       (20)      192 2023-07-18 22:09:18.000000 candor-test-1.0.1/candor_test.egg-info/SOURCES.txt
+-rw-r--r--   0 jbeal      (501) staff       (20)        1 2023-07-18 22:09:18.000000 candor-test-1.0.1/candor_test.egg-info/dependency_links.txt
+-rw-r--r--   0 jbeal      (501) staff       (20)        9 2023-07-18 22:09:18.000000 candor-test-1.0.1/candor_test.egg-info/requires.txt
+-rw-r--r--   0 jbeal      (501) staff       (20)        1 2023-07-18 22:09:18.000000 candor-test-1.0.1/candor_test.egg-info/top_level.txt
+-rw-r--r--   0 jbeal      (501) staff       (20)       38 2023-07-18 22:09:18.374327 candor-test-1.0.1/setup.cfg
+-rw-r--r--   0 jbeal      (501) staff       (20)      467 2023-07-18 22:08:02.000000 candor-test-1.0.1/setup.py
```

### Comparing `candor-test-1.0.0/PKG-INFO` & `candor-test-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: candor-test
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple wrapper for the Candor API.
 Home-page: https://github.com/FroostySnoowman/Candor
 Author: FroostySnoowman
 Author-email: froostysnoowmanbusiness@gmail.com
 Description-Content-Type: text/markdown
 
 # candor.py
```

### Comparing `candor-test-1.0.0/README.md` & `candor-test-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `candor-test-1.0.0/candor_test.egg-info/PKG-INFO` & `candor-test-1.0.1/candor_test.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: candor-test
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple wrapper for the Candor API.
 Home-page: https://github.com/FroostySnoowman/Candor
 Author: FroostySnoowman
 Author-email: froostysnoowmanbusiness@gmail.com
 Description-Content-Type: text/markdown
 
 # candor.py
```

