# Comparing `tmp/zhcevanstest-1.1.2.tar.gz` & `tmp/zhcevanstest-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhcevanstest-1.1.2.tar", last modified: Wed Jul 19 14:09:43 2023, max compression
+gzip compressed data, was "zhcevanstest-1.1.4.tar", last modified: Wed Jul 19 15:03:31 2023, max compression
```

## Comparing `zhcevanstest-1.1.2.tar` & `zhcevanstest-1.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-19 14:09:43.357241 zhcevanstest-1.1.2/
--rw-r--r--   0 evans      (501) staff       (20)      596 2023-07-19 14:09:43.356932 zhcevanstest-1.1.2/PKG-INFO
--rw-r--r--   0 evans      (501) staff       (20)       38 2023-07-19 14:09:43.357336 zhcevanstest-1.1.2/setup.cfg
-drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-19 14:09:43.356541 zhcevanstest-1.1.2/zhcevanstest.egg-info/
--rw-r--r--   0 evans      (501) staff       (20)      596 2023-07-19 14:09:43.000000 zhcevanstest-1.1.2/zhcevanstest.egg-info/PKG-INFO
--rw-r--r--   0 evans      (501) staff       (20)      178 2023-07-19 14:09:43.000000 zhcevanstest-1.1.2/zhcevanstest.egg-info/SOURCES.txt
--rw-r--r--   0 evans      (501) staff       (20)        1 2023-07-19 14:09:43.000000 zhcevanstest-1.1.2/zhcevanstest.egg-info/dependency_links.txt
--rw-r--r--   0 evans      (501) staff       (20)       17 2023-07-19 14:09:43.000000 zhcevanstest-1.1.2/zhcevanstest.egg-info/requires.txt
--rw-r--r--   0 evans      (501) staff       (20)        1 2023-07-19 14:09:43.000000 zhcevanstest-1.1.2/zhcevanstest.egg-info/top_level.txt
+drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-19 15:03:31.482299 zhcevanstest-1.1.4/
+-rw-r--r--   0 evans      (501) staff       (20)      544 2023-07-19 15:03:31.481992 zhcevanstest-1.1.4/PKG-INFO
+-rw-r--r--   0 evans      (501) staff       (20)       38 2023-07-19 15:03:31.482400 zhcevanstest-1.1.4/setup.cfg
+drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-19 15:03:31.481609 zhcevanstest-1.1.4/zhcevanstest.egg-info/
+-rw-r--r--   0 evans      (501) staff       (20)      544 2023-07-19 15:03:31.000000 zhcevanstest-1.1.4/zhcevanstest.egg-info/PKG-INFO
+-rw-r--r--   0 evans      (501) staff       (20)      178 2023-07-19 15:03:31.000000 zhcevanstest-1.1.4/zhcevanstest.egg-info/SOURCES.txt
+-rw-r--r--   0 evans      (501) staff       (20)        1 2023-07-19 15:03:31.000000 zhcevanstest-1.1.4/zhcevanstest.egg-info/dependency_links.txt
+-rw-r--r--   0 evans      (501) staff       (20)       17 2023-07-19 15:03:31.000000 zhcevanstest-1.1.4/zhcevanstest.egg-info/requires.txt
+-rw-r--r--   0 evans      (501) staff       (20)        1 2023-07-19 15:03:31.000000 zhcevanstest-1.1.4/zhcevanstest.egg-info/top_level.txt
```

### Comparing `zhcevanstest-1.1.2/PKG-INFO` & `zhcevanstest-1.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: zhcevanstest
-Version: 1.1.2
+Version: 1.1.4
 Summary: A package for plotting Konrads data
-Home-page: https://github.com/evans1112/testforpypi
 Author: evans.zhu
 Author-email: evanszhu2001@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `zhcevanstest-1.1.2/zhcevanstest.egg-info/PKG-INFO` & `zhcevanstest-1.1.4/zhcevanstest.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: zhcevanstest
-Version: 1.1.2
+Version: 1.1.4
 Summary: A package for plotting Konrads data
-Home-page: https://github.com/evans1112/testforpypi
 Author: evans.zhu
 Author-email: evanszhu2001@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

