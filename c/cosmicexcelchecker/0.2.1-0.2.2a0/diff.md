# Comparing `tmp/cosmicexcelchecker-0.2.1.tar.gz` & `tmp/cosmicexcelchecker-0.2.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmicexcelchecker-0.2.1.tar", last modified: Wed Jul 19 08:24:13 2023, max compression
+gzip compressed data, was "cosmicexcelchecker-0.2.2a0.tar", last modified: Wed Jul 19 08:36:48 2023, max compression
```

## Comparing `cosmicexcelchecker-0.2.1.tar` & `cosmicexcelchecker-0.2.2a0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 08:24:13.374448 cosmicexcelchecker-0.2.1/
--rw-rw-rw-   0        0        0    11166 2023-07-19 08:24:13.373449 cosmicexcelchecker-0.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-19 08:24:13.359449 cosmicexcelchecker-0.2.1/cosmicexcelchecker/
--rw-rw-rw-   0        0        0      359 2023-07-19 08:22:35.000000 cosmicexcelchecker-0.2.1/cosmicexcelchecker/__init__.py
--rw-rw-rw-   0        0        0     2856 2023-07-14 01:30:24.000000 cosmicexcelchecker-0.2.1/cosmicexcelchecker/_baseclass.py
--rw-rw-rw-   0        0        0     7183 2023-07-18 07:30:39.000000 cosmicexcelchecker-0.2.1/cosmicexcelchecker/conf.py
--rw-rw-rw-   0        0        0    33542 2023-07-18 08:49:25.000000 cosmicexcelchecker-0.2.1/cosmicexcelchecker/cosmic.py
--rw-rw-rw-   0        0        0      825 2023-07-07 02:29:19.000000 cosmicexcelchecker-0.2.1/cosmicexcelchecker/errors.py
--rw-rw-rw-   0        0        0      897 2023-07-11 01:28:39.000000 cosmicexcelchecker-0.2.1/cosmicexcelchecker/find.py
--rw-rw-rw-   0        0        0     2520 2023-07-18 06:54:21.000000 cosmicexcelchecker-0.2.1/cosmicexcelchecker/obf.py
--rw-rw-rw-   0        0        0     3708 2023-07-12 07:11:45.000000 cosmicexcelchecker-0.2.1/cosmicexcelchecker/openpyxltest.py
--rw-rw-rw-   0        0        0    43355 2023-07-18 07:19:56.000000 cosmicexcelchecker-0.2.1/cosmicexcelchecker/test.py
--rw-rw-rw-   0        0        0     1334 2023-07-12 06:19:53.000000 cosmicexcelchecker-0.2.1/cosmicexcelchecker/testaio.py
-drwxrwxrwx   0        0        0        0 2023-07-19 08:24:13.371449 cosmicexcelchecker-0.2.1/cosmicexcelchecker.egg-info/
--rw-rw-rw-   0        0        0    11166 2023-07-19 08:24:13.000000 cosmicexcelchecker-0.2.1/cosmicexcelchecker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      511 2023-07-19 08:24:13.000000 cosmicexcelchecker-0.2.1/cosmicexcelchecker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 08:24:13.000000 cosmicexcelchecker-0.2.1/cosmicexcelchecker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-07-19 08:24:13.000000 cosmicexcelchecker-0.2.1/cosmicexcelchecker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-07-19 08:24:13.000000 cosmicexcelchecker-0.2.1/cosmicexcelchecker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-19 08:24:13.374448 cosmicexcelchecker-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1069 2023-07-19 08:22:24.000000 cosmicexcelchecker-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 08:36:48.507470 cosmicexcelchecker-0.2.2a0/
+-rw-rw-rw-   0        0        0    11168 2023-07-19 08:36:48.506470 cosmicexcelchecker-0.2.2a0/PKG-INFO
+-rw-rw-rw-   0        0        0    10600 2023-07-18 07:08:36.000000 cosmicexcelchecker-0.2.2a0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 08:36:48.476365 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/
+-rw-rw-rw-   0        0        0      358 2023-07-19 08:35:18.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/__init__.py
+-rw-rw-rw-   0        0        0     2856 2023-07-14 01:30:24.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/_baseclass.py
+-rw-rw-rw-   0        0        0     7183 2023-07-18 07:30:39.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/conf.py
+-rw-rw-rw-   0        0        0    33542 2023-07-18 08:49:25.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/cosmic.py
+-rw-rw-rw-   0        0        0      825 2023-07-07 02:29:19.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/errors.py
+-rw-rw-rw-   0        0        0      897 2023-07-11 01:28:39.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/find.py
+-rw-rw-rw-   0        0        0     2520 2023-07-18 06:54:21.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/obf.py
+-rw-rw-rw-   0        0        0     3708 2023-07-12 07:11:45.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/openpyxltest.py
+-rw-rw-rw-   0        0        0    43355 2023-07-18 07:19:56.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/test.py
+-rw-rw-rw-   0        0        0     1334 2023-07-12 06:19:53.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/testaio.py
+drwxrwxrwx   0        0        0        0 2023-07-19 08:36:48.502878 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker.egg-info/
+-rw-rw-rw-   0        0        0    11168 2023-07-19 08:36:48.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      521 2023-07-19 08:36:48.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 08:36:48.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-07-19 08:36:48.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-19 08:36:48.000000 cosmicexcelchecker-0.2.2a0/cosmicexcelchecker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 08:36:48.507470 cosmicexcelchecker-0.2.2a0/setup.cfg
+-rw-rw-rw-   0        0        0     1048 2023-07-19 08:35:48.000000 cosmicexcelchecker-0.2.2a0/setup.py
```

### Comparing `cosmicexcelchecker-0.2.1/PKG-INFO` & `cosmicexcelchecker-0.2.2a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmicexcelchecker
-Version: 0.2.1
+Version: 0.2.2a0
 Summary: A high flexibility package for checking cosmic-related excels under CMDI cosmic standards
 Author: TimG233
 Author-email: gaosh0830@gmail.com
 Maintainer: TimG233
 License: GPL-3.0-only
 Keywords: cosmic,excel,CMDI,checker,data
 Platform: any
```

### Comparing `cosmicexcelchecker-0.2.1/cosmicexcelchecker/_baseclass.py` & `cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/_baseclass.py`

 * *Files identical despite different names*

### Comparing `cosmicexcelchecker-0.2.1/cosmicexcelchecker/conf.py` & `cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/conf.py`

 * *Files identical despite different names*

### Comparing `cosmicexcelchecker-0.2.1/cosmicexcelchecker/cosmic.py` & `cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/cosmic.py`

 * *Files identical despite different names*

### Comparing `cosmicexcelchecker-0.2.1/cosmicexcelchecker/errors.py` & `cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/errors.py`

 * *Files identical despite different names*

### Comparing `cosmicexcelchecker-0.2.1/cosmicexcelchecker/find.py` & `cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/find.py`

 * *Files identical despite different names*

### Comparing `cosmicexcelchecker-0.2.1/cosmicexcelchecker/obf.py` & `cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/obf.py`

 * *Files identical despite different names*

### Comparing `cosmicexcelchecker-0.2.1/cosmicexcelchecker/openpyxltest.py` & `cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/openpyxltest.py`

 * *Files identical despite different names*

### Comparing `cosmicexcelchecker-0.2.1/cosmicexcelchecker/test.py` & `cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/test.py`

 * *Files identical despite different names*

### Comparing `cosmicexcelchecker-0.2.1/cosmicexcelchecker/testaio.py` & `cosmicexcelchecker-0.2.2a0/cosmicexcelchecker/testaio.py`

 * *Files identical despite different names*

### Comparing `cosmicexcelchecker-0.2.1/cosmicexcelchecker.egg-info/PKG-INFO` & `cosmicexcelchecker-0.2.2a0/cosmicexcelchecker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmicexcelchecker
-Version: 0.2.1
+Version: 0.2.2a0
 Summary: A high flexibility package for checking cosmic-related excels under CMDI cosmic standards
 Author: TimG233
 Author-email: gaosh0830@gmail.com
 Maintainer: TimG233
 License: GPL-3.0-only
 Keywords: cosmic,excel,CMDI,checker,data
 Platform: any
```

### Comparing `cosmicexcelchecker-0.2.1/setup.py` & `cosmicexcelchecker-0.2.2a0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from setuptools import setup, find_packages
 
-with open('./docs/README.md', 'r', encoding='utf-8') as f:
+with open('./README.md', 'r', encoding='utf-8') as f:
     long_des = f.read()
 
 setup(
     name="cosmicexcelchecker",
-    version="0.2.1",
+    version="0.2.2a",
     license="GPL-3.0-only",
     author="TimG233",
     author_email="gaosh0830@gmail.com",
     maintainer="TimG233",
     description="A high flexibility package for checking cosmic-related excels under CMDI cosmic standards",
     long_description=long_des,
     long_description_content_type="text/markdown",
     packages=[
         "cosmicexcelchecker",
-        "docs",
     ],
     keywords=["cosmic", "excel", "CMDI", "checker", "data"],
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
```

