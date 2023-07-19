# Comparing `tmp/tools_wzy-0.0.5.tar.gz` & `tmp/tools_wzy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tools_wzy-0.0.5.tar", last modified: Tue Jul 18 03:28:15 2023, max compression
+gzip compressed data, was "tools_wzy-0.0.6.tar", last modified: Wed Jul 19 12:15:15 2023, max compression
```

## Comparing `tools_wzy-0.0.5.tar` & `tools_wzy-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 03:28:15.534023 tools_wzy-0.0.5/
--rw-rw-rw-   0        0        0      308 2023-07-18 03:28:15.533026 tools_wzy-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-18 03:28:15.534023 tools_wzy-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1030 2023-07-18 03:27:45.000000 tools_wzy-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 03:28:15.530036 tools_wzy-0.0.5/tools_wzy/
--rw-rw-rw-   0        0        0        0 2023-07-13 09:07:59.000000 tools_wzy-0.0.5/tools_wzy/__init__.py
--rw-rw-rw-   0        0        0     9507 2023-07-17 06:15:57.000000 tools_wzy-0.0.5/tools_wzy/node_coverage.py
--rw-rw-rw-   0        0        0     5153 2023-07-18 03:25:19.000000 tools_wzy-0.0.5/tools_wzy/yolo_need.py
-drwxrwxrwx   0        0        0        0 2023-07-18 03:28:15.533026 tools_wzy-0.0.5/tools_wzy.egg-info/
--rw-rw-rw-   0        0        0      308 2023-07-18 03:28:15.000000 tools_wzy-0.0.5/tools_wzy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-07-18 03:28:15.000000 tools_wzy-0.0.5/tools_wzy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 03:28:15.000000 tools_wzy-0.0.5/tools_wzy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-18 03:28:15.000000 tools_wzy-0.0.5/tools_wzy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-18 03:28:15.000000 tools_wzy-0.0.5/tools_wzy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 12:15:15.150186 tools_wzy-0.0.6/
+-rw-rw-rw-   0        0        0      308 2023-07-19 12:15:15.150186 tools_wzy-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-19 12:15:15.150186 tools_wzy-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1030 2023-07-19 12:14:55.000000 tools_wzy-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 12:15:15.146199 tools_wzy-0.0.6/tools_wzy/
+-rw-rw-rw-   0        0        0        0 2023-07-13 09:07:59.000000 tools_wzy-0.0.6/tools_wzy/__init__.py
+-rw-rw-rw-   0        0        0     9507 2023-07-17 06:15:57.000000 tools_wzy-0.0.6/tools_wzy/node_coverage.py
+-rw-rw-rw-   0        0        0     5153 2023-07-18 03:25:19.000000 tools_wzy-0.0.6/tools_wzy/yolo_need.py
+drwxrwxrwx   0        0        0        0 2023-07-19 12:15:15.149190 tools_wzy-0.0.6/tools_wzy.egg-info/
+-rw-rw-rw-   0        0        0      308 2023-07-19 12:15:15.000000 tools_wzy-0.0.6/tools_wzy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-07-19 12:15:15.000000 tools_wzy-0.0.6/tools_wzy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 12:15:15.000000 tools_wzy-0.0.6/tools_wzy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-19 12:15:15.000000 tools_wzy-0.0.6/tools_wzy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-19 12:15:15.000000 tools_wzy-0.0.6/tools_wzy.egg-info/top_level.txt
```

### Comparing `tools_wzy-0.0.5/setup.py` & `tools_wzy-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Created Time:  2023-07-18
 #############################################
 
 from setuptools import setup, find_packages            #这个包没有的可以pip一下
 
 setup(
     name = "tools_wzy",      #这里是pip项目发布的名称
-    version = "0.0.5",  #版本号，数值大的会优先被pip
+    version = "0.0.6",  #版本号，数值大的会优先被pip
     keywords = ["pip", "tools_wzy"],
     description = "Some python tools for work from Zhiyuan",
     long_description = "Some python tools for work from Zhiyuan",
     license = "MIT Licence",
 
     url = "https://gitee.com/Zhiyuan_WZY",     #项目相关文件地址，一般是github
     author = "Zhiyuan Wang",
```

### Comparing `tools_wzy-0.0.5/tools_wzy/node_coverage.py` & `tools_wzy-0.0.6/tools_wzy/node_coverage.py`

 * *Files identical despite different names*

### Comparing `tools_wzy-0.0.5/tools_wzy/yolo_need.py` & `tools_wzy-0.0.6/tools_wzy/yolo_need.py`

 * *Files identical despite different names*

