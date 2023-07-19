# Comparing `tmp/PyComps-0.3.1.tar.gz` & `tmp/PyComps-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyComps-0.3.1.tar", last modified: Wed Jul 19 12:26:44 2023, max compression
+gzip compressed data, was "PyComps-0.3.2.tar", last modified: Wed Jul 19 12:33:05 2023, max compression
```

## Comparing `PyComps-0.3.1.tar` & `PyComps-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 12:26:44.458900 PyComps-0.3.1/
--rw-rw-rw-   0        0        0     1084 2023-07-04 11:01:15.000000 PyComps-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     1583 2023-07-19 12:26:44.457896 PyComps-0.3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-19 12:26:44.438968 PyComps-0.3.1/PyComps/
--rw-rw-rw-   0        0        0   121931 2023-07-18 15:16:20.000000 PyComps-0.3.1/PyComps/LaminateCalculator.py
--rw-rw-rw-   0        0        0    24380 2023-07-18 07:55:18.000000 PyComps-0.3.1/PyComps/Micromechanics.py
--rw-rw-rw-   0        0        0      130 2023-07-04 12:54:46.000000 PyComps-0.3.1/PyComps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 12:26:44.451914 PyComps-0.3.1/PyComps.egg-info/
--rw-rw-rw-   0        0        0     1583 2023-07-19 12:26:44.000000 PyComps-0.3.1/PyComps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2023-07-19 12:26:44.000000 PyComps-0.3.1/PyComps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 12:26:44.000000 PyComps-0.3.1/PyComps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-19 12:26:44.000000 PyComps-0.3.1/PyComps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1262 2023-07-19 12:26:18.000000 PyComps-0.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-19 12:26:44.459892 PyComps-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      519 2023-07-19 12:26:33.000000 PyComps-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-19 12:26:44.456899 PyComps-0.3.1/test/
--rw-rw-rw-   0        0        0    18499 2023-07-18 15:48:45.000000 PyComps-0.3.1/test/test_LaminateCalculator.py
--rw-rw-rw-   0        0        0    12485 2023-07-05 09:35:14.000000 PyComps-0.3.1/test/test_Micromechanics.py
+drwxrwxrwx   0        0        0        0 2023-07-19 12:33:05.629349 PyComps-0.3.2/
+-rw-rw-rw-   0        0        0     1084 2023-07-04 11:01:15.000000 PyComps-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     1583 2023-07-19 12:33:05.628354 PyComps-0.3.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-19 12:33:05.611413 PyComps-0.3.2/PyComps/
+-rw-rw-rw-   0        0        0   121931 2023-07-18 15:16:20.000000 PyComps-0.3.2/PyComps/LaminateCalculator.py
+-rw-rw-rw-   0        0        0    24380 2023-07-18 07:55:18.000000 PyComps-0.3.2/PyComps/Micromechanics.py
+-rw-rw-rw-   0        0        0      130 2023-07-04 12:54:46.000000 PyComps-0.3.2/PyComps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 12:33:05.624369 PyComps-0.3.2/PyComps.egg-info/
+-rw-rw-rw-   0        0        0     1583 2023-07-19 12:33:05.000000 PyComps-0.3.2/PyComps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2023-07-19 12:33:05.000000 PyComps-0.3.2/PyComps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 12:33:05.000000 PyComps-0.3.2/PyComps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-19 12:33:05.000000 PyComps-0.3.2/PyComps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1262 2023-07-19 12:31:14.000000 PyComps-0.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-19 12:33:05.630344 PyComps-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      519 2023-07-19 12:32:54.000000 PyComps-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 12:33:05.627354 PyComps-0.3.2/test/
+-rw-rw-rw-   0        0        0    18499 2023-07-18 15:48:45.000000 PyComps-0.3.2/test/test_LaminateCalculator.py
+-rw-rw-rw-   0        0        0    12485 2023-07-05 09:35:14.000000 PyComps-0.3.2/test/test_Micromechanics.py
```

### Comparing `PyComps-0.3.1/LICENSE` & `PyComps-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyComps-0.3.1/PKG-INFO` & `PyComps-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComps
-Version: 0.3.1
+Version: 0.3.2
 Summary: A sample Python package
 Home-page: https://github.com/edo-147/PyComp
 Author: Edoardo Mancini
 Author-email: edoardo.mancini0@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -44,8 +44,8 @@
 - **cured ply thickness** estimation
 
 
 ### Source Code: 
 https://github.com/edo-147/PyComp
 
 ### notes: 
-aligned with GitHub tag v0.3.0
+aligned with GitHub tag v0.3.1
```

### Comparing `PyComps-0.3.1/PyComps/LaminateCalculator.py` & `PyComps-0.3.2/PyComps/LaminateCalculator.py`

 * *Files identical despite different names*

### Comparing `PyComps-0.3.1/PyComps/Micromechanics.py` & `PyComps-0.3.2/PyComps/Micromechanics.py`

 * *Files identical despite different names*

### Comparing `PyComps-0.3.1/PyComps.egg-info/PKG-INFO` & `PyComps-0.3.2/PyComps.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComps
-Version: 0.3.1
+Version: 0.3.2
 Summary: A sample Python package
 Home-page: https://github.com/edo-147/PyComp
 Author: Edoardo Mancini
 Author-email: edoardo.mancini0@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -44,8 +44,8 @@
 - **cured ply thickness** estimation
 
 
 ### Source Code: 
 https://github.com/edo-147/PyComp
 
 ### notes: 
-aligned with GitHub tag v0.3.0
+aligned with GitHub tag v0.3.1
```

### Comparing `PyComps-0.3.1/README.md` & `PyComps-0.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -33,8 +33,8 @@
 - **cured ply thickness** estimation
 
 
 ### Source Code: 
 https://github.com/edo-147/PyComp
 
 ### notes: 
-aligned with GitHub tag v0.3.0
+aligned with GitHub tag v0.3.1
```

### Comparing `PyComps-0.3.1/setup.py` & `PyComps-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     readme = f.read()
     
 setup(
     name='PyComps', 
-    version='0.3.1',
+    version='0.3.2',
     description='A sample Python package',
     author='Edoardo Mancini',
     author_email='edoardo.mancini0@gmail.com',
     classifiers=["License :: OSI Approved :: MIT License"],
     url='https://github.com/edo-147/PyComp',
     long_description=readme,
     long_description_content_type="text/markdown",
```

### Comparing `PyComps-0.3.1/test/test_LaminateCalculator.py` & `PyComps-0.3.2/test/test_LaminateCalculator.py`

 * *Files identical despite different names*

### Comparing `PyComps-0.3.1/test/test_Micromechanics.py` & `PyComps-0.3.2/test/test_Micromechanics.py`

 * *Files identical despite different names*

