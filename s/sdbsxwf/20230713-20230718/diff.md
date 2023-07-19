# Comparing `tmp/sdbsxwf-20230713.tar.gz` & `tmp/sdbsxwf-20230718.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdbsxwf-20230713.tar", last modified: Thu Jul 13 13:27:12 2023, max compression
+gzip compressed data, was "sdbsxwf-20230718.tar", last modified: Tue Jul 18 14:24:02 2023, max compression
```

## Comparing `sdbsxwf-20230713.tar` & `sdbsxwf-20230718.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 13:27:12.516471 sdbsxwf-20230713/
--rw-rw-rw-   0        0        0      841 2023-07-13 13:27:12.517458 sdbsxwf-20230713/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-13 13:27:12.517458 sdbsxwf-20230713/setup.cfg
--rw-rw-rw-   0        0        0     1332 2023-07-13 13:21:04.000000 sdbsxwf-20230713/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:27:12.505259 sdbsxwf-20230713/src/
-drwxrwxrwx   0        0        0        0 2023-07-13 13:27:12.510241 sdbsxwf-20230713/src/sdbsxwf/
--rw-rw-rw-   0        0        0      328 2023-07-13 13:18:38.000000 sdbsxwf-20230713/src/sdbsxwf/__init__.py
--rw-rw-rw-   0        0        0       43 2023-07-13 13:19:21.000000 sdbsxwf-20230713/src/sdbsxwf/mkgjx.py
--rw-rw-rw-   0        0        0      257 2023-07-13 13:20:15.000000 sdbsxwf-20230713/src/sdbsxwf/mkmain.py
-drwxrwxrwx   0        0        0        0 2023-07-13 13:27:12.516471 sdbsxwf-20230713/src/sdbsxwf.egg-info/
--rw-rw-rw-   0        0        0      841 2023-07-13 13:27:12.000000 sdbsxwf-20230713/src/sdbsxwf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-07-13 13:27:12.000000 sdbsxwf-20230713/src/sdbsxwf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 13:27:12.000000 sdbsxwf-20230713/src/sdbsxwf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-07-13 13:27:12.000000 sdbsxwf-20230713/src/sdbsxwf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-13 13:27:12.000000 sdbsxwf-20230713/src/sdbsxwf.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 14:24:02.498580 sdbsxwf-20230718/
+-rw-rw-rw-   0        0        0      841 2023-07-18 14:24:02.498580 sdbsxwf-20230718/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-18 14:24:02.498580 sdbsxwf-20230718/setup.cfg
+-rw-rw-rw-   0        0        0     1332 2023-07-18 14:23:31.000000 sdbsxwf-20230718/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:24:02.488096 sdbsxwf-20230718/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 14:24:02.492599 sdbsxwf-20230718/src/sdbsxwf/
+-rw-rw-rw-   0        0        0      352 2023-07-18 14:14:01.000000 sdbsxwf-20230718/src/sdbsxwf/__init__.py
+-rw-rw-rw-   0        0        0       43 2023-07-13 13:19:21.000000 sdbsxwf-20230718/src/sdbsxwf/mkgjx.py
+-rw-rw-rw-   0        0        0      257 2023-07-13 13:20:15.000000 sdbsxwf-20230718/src/sdbsxwf/mkmain.py
+-rw-rw-rw-   0        0        0     6373 2023-07-18 14:22:24.000000 sdbsxwf-20230718/src/sdbsxwf/xlsxzl.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:24:02.497658 sdbsxwf-20230718/src/sdbsxwf.egg-info/
+-rw-rw-rw-   0        0        0      841 2023-07-18 14:24:02.000000 sdbsxwf-20230718/src/sdbsxwf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-07-18 14:24:02.000000 sdbsxwf-20230718/src/sdbsxwf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 14:24:02.000000 sdbsxwf-20230718/src/sdbsxwf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-18 14:24:02.000000 sdbsxwf-20230718/src/sdbsxwf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-18 14:24:02.000000 sdbsxwf-20230718/src/sdbsxwf.egg-info/top_level.txt
```

### Comparing `sdbsxwf-20230713/PKG-INFO` & `sdbsxwf-20230718/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdbsxwf
-Version: 20230713
+Version: 20230718
 Summary: 个人工具箱
 Home-page: 
 Author: xwf
 Author-email: 453211170@qq.com
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `sdbsxwf-20230713/setup.py` & `sdbsxwf-20230718/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 from setuptools import find_packages
  
 setup(name = 'sdbsxwf',     # 包名
-      version = '20230713',  # 版本号
+      version = '20230718',  # 版本号
       description = '个人工具箱',
       long_description = '试着改变世界', 
       author = 'xwf',
       author_email = '453211170@qq.com',
       url = '',
       license = '',
       install_requires=[
```

### Comparing `sdbsxwf-20230713/src/sdbsxwf.egg-info/PKG-INFO` & `sdbsxwf-20230718/src/sdbsxwf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdbsxwf
-Version: 20230713
+Version: 20230718
 Summary: 个人工具箱
 Home-page: 
 Author: xwf
 Author-email: 453211170@qq.com
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
```

