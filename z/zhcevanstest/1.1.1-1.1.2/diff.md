# Comparing `tmp/zhcevanstest-1.1.1.tar.gz` & `tmp/zhcevanstest-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhcevanstest-1.1.1.tar", last modified: Wed Jul 19 13:16:30 2023, max compression
+gzip compressed data, was "zhcevanstest-1.1.2.tar", last modified: Wed Jul 19 14:09:43 2023, max compression
```

## Comparing `zhcevanstest-1.1.1.tar` & `zhcevanstest-1.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-19 13:16:30.549902 zhcevanstest-1.1.1/
--rw-r--r--   0 evans      (501) staff       (20)      596 2023-07-19 13:16:30.549535 zhcevanstest-1.1.1/PKG-INFO
--rw-r--r--   0 evans      (501) staff       (20)       38 2023-07-19 13:16:30.550059 zhcevanstest-1.1.1/setup.cfg
-drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-19 13:16:30.549075 zhcevanstest-1.1.1/zhcevanstest.egg-info/
--rw-r--r--   0 evans      (501) staff       (20)      596 2023-07-19 13:16:30.000000 zhcevanstest-1.1.1/zhcevanstest.egg-info/PKG-INFO
--rw-r--r--   0 evans      (501) staff       (20)      178 2023-07-19 13:16:30.000000 zhcevanstest-1.1.1/zhcevanstest.egg-info/SOURCES.txt
--rw-r--r--   0 evans      (501) staff       (20)        1 2023-07-19 13:16:30.000000 zhcevanstest-1.1.1/zhcevanstest.egg-info/dependency_links.txt
--rw-r--r--   0 evans      (501) staff       (20)       17 2023-07-19 13:16:30.000000 zhcevanstest-1.1.1/zhcevanstest.egg-info/requires.txt
--rw-r--r--   0 evans      (501) staff       (20)        1 2023-07-19 13:16:30.000000 zhcevanstest-1.1.1/zhcevanstest.egg-info/top_level.txt
+drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-19 14:09:43.357241 zhcevanstest-1.1.2/
+-rw-r--r--   0 evans      (501) staff       (20)      596 2023-07-19 14:09:43.356932 zhcevanstest-1.1.2/PKG-INFO
+-rw-r--r--   0 evans      (501) staff       (20)       38 2023-07-19 14:09:43.357336 zhcevanstest-1.1.2/setup.cfg
+drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-19 14:09:43.356541 zhcevanstest-1.1.2/zhcevanstest.egg-info/
+-rw-r--r--   0 evans      (501) staff       (20)      596 2023-07-19 14:09:43.000000 zhcevanstest-1.1.2/zhcevanstest.egg-info/PKG-INFO
+-rw-r--r--   0 evans      (501) staff       (20)      178 2023-07-19 14:09:43.000000 zhcevanstest-1.1.2/zhcevanstest.egg-info/SOURCES.txt
+-rw-r--r--   0 evans      (501) staff       (20)        1 2023-07-19 14:09:43.000000 zhcevanstest-1.1.2/zhcevanstest.egg-info/dependency_links.txt
+-rw-r--r--   0 evans      (501) staff       (20)       17 2023-07-19 14:09:43.000000 zhcevanstest-1.1.2/zhcevanstest.egg-info/requires.txt
+-rw-r--r--   0 evans      (501) staff       (20)        1 2023-07-19 14:09:43.000000 zhcevanstest-1.1.2/zhcevanstest.egg-info/top_level.txt
```

### Comparing `zhcevanstest-1.1.1/PKG-INFO` & `zhcevanstest-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhcevanstest
-Version: 1.1.1
+Version: 1.1.2
 Summary: A package for plotting Konrads data
 Home-page: https://github.com/evans1112/testforpypi
 Author: evans.zhu
 Author-email: evanszhu2001@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `zhcevanstest-1.1.1/zhcevanstest.egg-info/PKG-INFO` & `zhcevanstest-1.1.2/zhcevanstest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhcevanstest
-Version: 1.1.1
+Version: 1.1.2
 Summary: A package for plotting Konrads data
 Home-page: https://github.com/evans1112/testforpypi
 Author: evans.zhu
 Author-email: evanszhu2001@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

