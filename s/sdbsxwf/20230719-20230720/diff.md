# Comparing `tmp/sdbsxwf-20230719.tar.gz` & `tmp/sdbsxwf-20230720.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdbsxwf-20230719.tar", last modified: Wed Jul 19 04:51:13 2023, max compression
+gzip compressed data, was "sdbsxwf-20230720.tar", last modified: Wed Jul 19 04:58:26 2023, max compression
```

## Comparing `sdbsxwf-20230719.tar` & `sdbsxwf-20230720.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 04:51:13.705796 sdbsxwf-20230719/
--rw-rw-rw-   0        0        0      664 2023-07-19 04:51:13.705796 sdbsxwf-20230719/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-19 04:51:13.706876 sdbsxwf-20230719/setup.cfg
--rw-rw-rw-   0        0        0     1262 2023-07-19 04:50:17.000000 sdbsxwf-20230719/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-19 04:51:13.694968 sdbsxwf-20230719/src/
-drwxrwxrwx   0        0        0        0 2023-07-19 04:51:13.700049 sdbsxwf-20230719/src/sdbsxwf/
--rw-rw-rw-   0        0        0      374 2023-07-18 15:08:45.000000 sdbsxwf-20230719/src/sdbsxwf/__init__.py
--rw-rw-rw-   0        0        0       43 2023-07-13 13:19:21.000000 sdbsxwf-20230719/src/sdbsxwf/mkgjx.py
--rw-rw-rw-   0        0        0      270 2023-07-19 00:29:19.000000 sdbsxwf-20230719/src/sdbsxwf/mkmain.py
--rw-rw-rw-   0        0        0     6373 2023-07-18 14:22:24.000000 sdbsxwf-20230719/src/sdbsxwf/xlsxzl.py
-drwxrwxrwx   0        0        0        0 2023-07-19 04:51:13.705796 sdbsxwf-20230719/src/sdbsxwf.egg-info/
--rw-rw-rw-   0        0        0      664 2023-07-19 04:51:13.000000 sdbsxwf-20230719/src/sdbsxwf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-07-19 04:51:13.000000 sdbsxwf-20230719/src/sdbsxwf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 04:51:13.000000 sdbsxwf-20230719/src/sdbsxwf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-07-19 04:51:13.000000 sdbsxwf-20230719/src/sdbsxwf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-19 04:51:13.000000 sdbsxwf-20230719/src/sdbsxwf.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 04:58:26.206968 sdbsxwf-20230720/
+-rw-rw-rw-   0        0        0      670 2023-07-19 04:58:26.206968 sdbsxwf-20230720/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-19 04:58:26.207964 sdbsxwf-20230720/setup.cfg
+-rw-rw-rw-   0        0        0     1268 2023-07-19 04:57:34.000000 sdbsxwf-20230720/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:58:26.196000 sdbsxwf-20230720/src/
+drwxrwxrwx   0        0        0        0 2023-07-19 04:58:26.199989 sdbsxwf-20230720/src/sdbsxwf/
+-rw-rw-rw-   0        0        0      374 2023-07-18 15:08:45.000000 sdbsxwf-20230720/src/sdbsxwf/__init__.py
+-rw-rw-rw-   0        0        0       43 2023-07-13 13:19:21.000000 sdbsxwf-20230720/src/sdbsxwf/mkgjx.py
+-rw-rw-rw-   0        0        0      270 2023-07-19 00:29:19.000000 sdbsxwf-20230720/src/sdbsxwf/mkmain.py
+-rw-rw-rw-   0        0        0     6373 2023-07-18 14:22:24.000000 sdbsxwf-20230720/src/sdbsxwf/xlsxzl.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:58:26.205971 sdbsxwf-20230720/src/sdbsxwf.egg-info/
+-rw-rw-rw-   0        0        0      670 2023-07-19 04:58:26.000000 sdbsxwf-20230720/src/sdbsxwf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-07-19 04:58:26.000000 sdbsxwf-20230720/src/sdbsxwf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 04:58:26.000000 sdbsxwf-20230720/src/sdbsxwf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-07-19 04:58:26.000000 sdbsxwf-20230720/src/sdbsxwf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-19 04:58:26.000000 sdbsxwf-20230720/src/sdbsxwf.egg-info/top_level.txt
```

### Comparing `sdbsxwf-20230719/PKG-INFO` & `sdbsxwf-20230720/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: sdbsxwf
-Version: 20230719
+Version: 20230720
 Summary: 个人工具箱
 Home-page: 
 Author: xwf
 Author-email: 453211170@qq.com
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Utilities
 
-试着改变世界
-20230718添加pandas读和写xlsx
-20230719优化导入模块接口
+试着改变世界<br>20230718添加pandas读和写xlsx;<br>20230719优化导入模块接口;
```

### Comparing `sdbsxwf-20230719/setup.py` & `sdbsxwf-20230720/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 from setuptools import find_packages
  
 setup(name = 'sdbsxwf',     # 包名
-      version = '20230719',  # 版本号
+      version = '20230720',  # 版本号
       description = '个人工具箱',
-      long_description = '试着改变世界\n20230718添加pandas读和写xlsx\n20230719优化导入模块接口', 
+      long_description = '试着改变世界<br>20230718添加pandas读和写xlsx;<br>20230719优化导入模块接口;', 
       author = 'xwf',
       author_email = '453211170@qq.com',
       url = '',
       license = '',
       install_requires=[        
         'pandas>=1.5.3',
         'numpy>=1.24.2',
```

### Comparing `sdbsxwf-20230719/src/sdbsxwf/xlsxzl.py` & `sdbsxwf-20230720/src/sdbsxwf/xlsxzl.py`

 * *Files identical despite different names*

### Comparing `sdbsxwf-20230719/src/sdbsxwf.egg-info/PKG-INFO` & `sdbsxwf-20230720/src/sdbsxwf.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: sdbsxwf
-Version: 20230719
+Version: 20230720
 Summary: 个人工具箱
 Home-page: 
 Author: xwf
 Author-email: 453211170@qq.com
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Utilities
 
-试着改变世界
-20230718添加pandas读和写xlsx
-20230719优化导入模块接口
+试着改变世界<br>20230718添加pandas读和写xlsx;<br>20230719优化导入模块接口;
```

