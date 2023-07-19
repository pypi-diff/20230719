# Comparing `tmp/PyComps-0.3.0.tar.gz` & `tmp/PyComps-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyComps-0.3.0.tar", last modified: Wed Jul 19 12:23:08 2023, max compression
+gzip compressed data, was "PyComps-0.3.1.tar", last modified: Wed Jul 19 12:26:44 2023, max compression
```

## Comparing `PyComps-0.3.0.tar` & `PyComps-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 12:23:08.313496 PyComps-0.3.0/
--rw-rw-rw-   0        0        0     1084 2023-07-04 11:01:15.000000 PyComps-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     1536 2023-07-19 12:23:08.312488 PyComps-0.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-19 12:23:08.292554 PyComps-0.3.0/PyComps/
--rw-rw-rw-   0        0        0   121931 2023-07-18 15:16:20.000000 PyComps-0.3.0/PyComps/LaminateCalculator.py
--rw-rw-rw-   0        0        0    24380 2023-07-18 07:55:18.000000 PyComps-0.3.0/PyComps/Micromechanics.py
--rw-rw-rw-   0        0        0      130 2023-07-04 12:54:46.000000 PyComps-0.3.0/PyComps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 12:23:08.306509 PyComps-0.3.0/PyComps.egg-info/
--rw-rw-rw-   0        0        0     1536 2023-07-19 12:23:08.000000 PyComps-0.3.0/PyComps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2023-07-19 12:23:08.000000 PyComps-0.3.0/PyComps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 12:23:08.000000 PyComps-0.3.0/PyComps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-19 12:23:08.000000 PyComps-0.3.0/PyComps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1215 2023-07-19 12:19:24.000000 PyComps-0.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-19 12:23:08.313496 PyComps-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      519 2023-07-19 12:22:52.000000 PyComps-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-19 12:23:08.310504 PyComps-0.3.0/test/
--rw-rw-rw-   0        0        0    18499 2023-07-18 15:48:45.000000 PyComps-0.3.0/test/test_LaminateCalculator.py
--rw-rw-rw-   0        0        0    12485 2023-07-05 09:35:14.000000 PyComps-0.3.0/test/test_Micromechanics.py
+drwxrwxrwx   0        0        0        0 2023-07-19 12:26:44.458900 PyComps-0.3.1/
+-rw-rw-rw-   0        0        0     1084 2023-07-04 11:01:15.000000 PyComps-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     1583 2023-07-19 12:26:44.457896 PyComps-0.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-19 12:26:44.438968 PyComps-0.3.1/PyComps/
+-rw-rw-rw-   0        0        0   121931 2023-07-18 15:16:20.000000 PyComps-0.3.1/PyComps/LaminateCalculator.py
+-rw-rw-rw-   0        0        0    24380 2023-07-18 07:55:18.000000 PyComps-0.3.1/PyComps/Micromechanics.py
+-rw-rw-rw-   0        0        0      130 2023-07-04 12:54:46.000000 PyComps-0.3.1/PyComps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 12:26:44.451914 PyComps-0.3.1/PyComps.egg-info/
+-rw-rw-rw-   0        0        0     1583 2023-07-19 12:26:44.000000 PyComps-0.3.1/PyComps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2023-07-19 12:26:44.000000 PyComps-0.3.1/PyComps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 12:26:44.000000 PyComps-0.3.1/PyComps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-19 12:26:44.000000 PyComps-0.3.1/PyComps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1262 2023-07-19 12:26:18.000000 PyComps-0.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-19 12:26:44.459892 PyComps-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      519 2023-07-19 12:26:33.000000 PyComps-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 12:26:44.456899 PyComps-0.3.1/test/
+-rw-rw-rw-   0        0        0    18499 2023-07-18 15:48:45.000000 PyComps-0.3.1/test/test_LaminateCalculator.py
+-rw-rw-rw-   0        0        0    12485 2023-07-05 09:35:14.000000 PyComps-0.3.1/test/test_Micromechanics.py
```

### Comparing `PyComps-0.3.0/LICENSE` & `PyComps-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyComps-0.3.0/PKG-INFO` & `PyComps-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: PyComps
-Version: 0.3.0
+Version: 0.3.1
 Summary: A sample Python package
 Home-page: https://github.com/edo-147/PyComp
 Author: Edoardo Mancini
 Author-email: edoardo.mancini0@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# PyComp 
+# PyComps
 
 Easy calculation of composite properties
 
 
 ## Brief description
 
 
@@ -42,7 +42,10 @@
 - calculation of **ply mechanical properties** starting from that of isotropic constituents.
 - the former can be attained with different methods: **ROM**, **Halpin-Tsai**, or **PMM**
 - **cured ply thickness** estimation
 
 
 ### Source Code: 
 https://github.com/edo-147/PyComp
+
+### notes: 
+aligned with GitHub tag v0.3.0
```

### Comparing `PyComps-0.3.0/PyComps/LaminateCalculator.py` & `PyComps-0.3.1/PyComps/LaminateCalculator.py`

 * *Files identical despite different names*

### Comparing `PyComps-0.3.0/PyComps/Micromechanics.py` & `PyComps-0.3.1/PyComps/Micromechanics.py`

 * *Files identical despite different names*

### Comparing `PyComps-0.3.0/PyComps.egg-info/PKG-INFO` & `PyComps-0.3.1/PyComps.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: PyComps
-Version: 0.3.0
+Version: 0.3.1
 Summary: A sample Python package
 Home-page: https://github.com/edo-147/PyComp
 Author: Edoardo Mancini
 Author-email: edoardo.mancini0@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# PyComp 
+# PyComps
 
 Easy calculation of composite properties
 
 
 ## Brief description
 
 
@@ -42,7 +42,10 @@
 - calculation of **ply mechanical properties** starting from that of isotropic constituents.
 - the former can be attained with different methods: **ROM**, **Halpin-Tsai**, or **PMM**
 - **cured ply thickness** estimation
 
 
 ### Source Code: 
 https://github.com/edo-147/PyComp
+
+### notes: 
+aligned with GitHub tag v0.3.0
```

### Comparing `PyComps-0.3.0/README.md` & `PyComps-0.3.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# PyComp 
+# PyComps
 
 Easy calculation of composite properties
 
 
 ## Brief description
 
 
@@ -30,8 +30,11 @@
 
 - calculation of **ply mechanical properties** starting from that of isotropic constituents.
 - the former can be attained with different methods: **ROM**, **Halpin-Tsai**, or **PMM**
 - **cured ply thickness** estimation
 
 
 ### Source Code: 
-https://github.com/edo-147/PyComp
+https://github.com/edo-147/PyComp
+
+### notes: 
+aligned with GitHub tag v0.3.0
```

### Comparing `PyComps-0.3.0/setup.py` & `PyComps-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     readme = f.read()
     
 setup(
     name='PyComps', 
-    version='0.3.0',
+    version='0.3.1',
     description='A sample Python package',
     author='Edoardo Mancini',
     author_email='edoardo.mancini0@gmail.com',
     classifiers=["License :: OSI Approved :: MIT License"],
     url='https://github.com/edo-147/PyComp',
     long_description=readme,
     long_description_content_type="text/markdown",
```

### Comparing `PyComps-0.3.0/test/test_LaminateCalculator.py` & `PyComps-0.3.1/test/test_LaminateCalculator.py`

 * *Files identical despite different names*

### Comparing `PyComps-0.3.0/test/test_Micromechanics.py` & `PyComps-0.3.1/test/test_Micromechanics.py`

 * *Files identical despite different names*

