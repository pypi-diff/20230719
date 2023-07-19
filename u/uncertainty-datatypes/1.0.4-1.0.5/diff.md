# Comparing `tmp/uncertainty-datatypes-1.0.4.tar.gz` & `tmp/uncertainty-datatypes-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uncertainty-datatypes-1.0.4.tar", last modified: Wed Jul 19 09:01:31 2023, max compression
+gzip compressed data, was "uncertainty-datatypes-1.0.5.tar", last modified: Wed Jul 19 09:14:20 2023, max compression
```

## Comparing `uncertainty-datatypes-1.0.4.tar` & `uncertainty-datatypes-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:01:31.861070 uncertainty-datatypes-1.0.4/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     1099 2023-07-17 07:54:55.000000 uncertainty-datatypes-1.0.4/LICENSE
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10278 2023-07-19 09:01:31.860906 uncertainty-datatypes-1.0.4/PKG-INFO
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     9507 2023-07-18 13:42:07.000000 uncertainty-datatypes-1.0.4/README.md
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      854 2023-07-19 09:01:10.000000 uncertainty-datatypes-1.0.4/pyproject.toml
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       38 2023-07-19 09:01:31.861110 uncertainty-datatypes-1.0.4/setup.cfg
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:01:31.858147 uncertainty-datatypes-1.0.4/test/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4428 2023-07-18 10:58:49.000000 uncertainty-datatypes-1.0.4/test/test_ubool.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    19028 2023-07-19 08:55:34.000000 uncertainty-datatypes-1.0.4/test/test_ufloat.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    17972 2023-07-19 08:39:29.000000 uncertainty-datatypes-1.0.4/test/test_uint.py
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:01:31.859835 uncertainty-datatypes-1.0.4/udatatypes/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-14 08:59:58.000000 uncertainty-datatypes-1.0.4/udatatypes/__init__.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      328 2023-07-17 11:29:42.000000 uncertainty-datatypes-1.0.4/udatatypes/result.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4228 2023-07-18 09:14:56.000000 uncertainty-datatypes-1.0.4/udatatypes/ubool.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    20720 2023-07-19 08:56:16.000000 uncertainty-datatypes-1.0.4/udatatypes/unumbers.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4302 2023-07-19 08:56:26.000000 uncertainty-datatypes-1.0.4/udatatypes/utypes.py
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:01:31.860734 uncertainty-datatypes-1.0.4/uncertainty_datatypes.egg-info/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10278 2023-07-19 09:01:31.000000 uncertainty-datatypes-1.0.4/uncertainty_datatypes.egg-info/PKG-INFO
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      421 2023-07-19 09:01:31.000000 uncertainty-datatypes-1.0.4/uncertainty_datatypes.egg-info/SOURCES.txt
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        1 2023-07-19 09:01:31.000000 uncertainty-datatypes-1.0.4/uncertainty_datatypes.egg-info/dependency_links.txt
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       14 2023-07-19 09:01:31.000000 uncertainty-datatypes-1.0.4/uncertainty_datatypes.egg-info/requires.txt
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       11 2023-07-19 09:01:31.000000 uncertainty-datatypes-1.0.4/uncertainty_datatypes.egg-info/top_level.txt
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:14:20.622406 uncertainty-datatypes-1.0.5/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     1099 2023-07-17 07:54:55.000000 uncertainty-datatypes-1.0.5/LICENSE
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10214 2023-07-19 09:14:20.622248 uncertainty-datatypes-1.0.5/PKG-INFO
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     9443 2023-07-19 09:12:21.000000 uncertainty-datatypes-1.0.5/README.md
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      854 2023-07-19 09:12:39.000000 uncertainty-datatypes-1.0.5/pyproject.toml
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       38 2023-07-19 09:14:20.622441 uncertainty-datatypes-1.0.5/setup.cfg
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:14:20.620681 uncertainty-datatypes-1.0.5/test/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4428 2023-07-18 10:58:49.000000 uncertainty-datatypes-1.0.5/test/test_ubool.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    19028 2023-07-19 08:55:34.000000 uncertainty-datatypes-1.0.5/test/test_ufloat.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    17972 2023-07-19 08:39:29.000000 uncertainty-datatypes-1.0.5/test/test_uint.py
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:14:20.621519 uncertainty-datatypes-1.0.5/udatatypes/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-14 08:59:58.000000 uncertainty-datatypes-1.0.5/udatatypes/__init__.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      328 2023-07-17 11:29:42.000000 uncertainty-datatypes-1.0.5/udatatypes/result.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4311 2023-07-19 09:11:30.000000 uncertainty-datatypes-1.0.5/udatatypes/ubool.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    20720 2023-07-19 08:56:16.000000 uncertainty-datatypes-1.0.5/udatatypes/unumbers.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4302 2023-07-19 08:56:26.000000 uncertainty-datatypes-1.0.5/udatatypes/utypes.py
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:14:20.622092 uncertainty-datatypes-1.0.5/uncertainty_datatypes.egg-info/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10214 2023-07-19 09:14:20.000000 uncertainty-datatypes-1.0.5/uncertainty_datatypes.egg-info/PKG-INFO
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      421 2023-07-19 09:14:20.000000 uncertainty-datatypes-1.0.5/uncertainty_datatypes.egg-info/SOURCES.txt
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        1 2023-07-19 09:14:20.000000 uncertainty-datatypes-1.0.5/uncertainty_datatypes.egg-info/dependency_links.txt
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       14 2023-07-19 09:14:20.000000 uncertainty-datatypes-1.0.5/uncertainty_datatypes.egg-info/requires.txt
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       11 2023-07-19 09:14:20.000000 uncertainty-datatypes-1.0.5/uncertainty_datatypes.egg-info/top_level.txt
```

### Comparing `uncertainty-datatypes-1.0.4/LICENSE` & `uncertainty-datatypes-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.4/PKG-INFO` & `uncertainty-datatypes-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uncertainty-datatypes
-Version: 1.0.4
+Version: 1.0.5
 Summary: Uncertainty Datatypes Library
 Author: Atenea Research Group, University of Malaga, Spain
 Project-URL: Homepage, https://github.com/atenearesearchgroup/uncertainty
 Project-URL: Bug Tracker, https://github.com/atenearesearchgroup/uncertainty/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -15,37 +15,33 @@
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Uncertainty Python Library
 
-Uncertainty is a Python library providing uncertainty datatypes including u-type, a-type and s-type.
+Uncertainty is a Python library providing uncertainty datatypes including u-type, a-type and s-type: 
+1. **u-type** datatypes: ubool, uint, ufloat, ustr, uenum.
+    Type U is a pair (x, u), noted x ± u, that represents a random variable whose average is x and standard deviation is u.
+2. **a-type** datatypes: abool, aint, afloat.
+    Type A, maintain the set of the measured values as X = {x1,...,xn}, x ± u could be calculated as the mean and standard deviation.
+3. **s-type** datatype: sbool.
+    A particular type of subjective uncertainty (Belief Uncertainty) when a user is not sure about the truth of a statement.
+
+Math functions with the datatypes are also provided.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.
 
 ```bash
 pip install uncertainty-datatypes
 ```
 <sub>Note pip3 may be used instead of pip</sub> 
 
-## The library
-
-The library provides three kinds of datatypes: 
-1. **u-type** datatypes: ubool, uint, ufloat, ustr, uenum.
-    Type U is a pair (x, u), noted x ± u, that represents a random variable whose average is x and standard deviation is u.
-2. **a-type** datatypes: abool, aint, afloat.
-    Type A, maintain the set of the measured values as X = {x1,...,xn}, x ± u could be calculated as the mean and standard deviation.
-3. **s-type** datatype: sbool.
-    A particular type of subjective uncertainty (Belief Uncertainty) when a user is not sure about the truth of a statement.
-
-Math functions with the datatypes are also provided.
-
 ## Usage
 
 Import all the datatypes and functions using:
 ```python
 from udatatypes.utypes import *
 ```
```

### Comparing `uncertainty-datatypes-1.0.4/README.md` & `uncertainty-datatypes-1.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 # Uncertainty Python Library
 
-Uncertainty is a Python library providing uncertainty datatypes including u-type, a-type and s-type.
+Uncertainty is a Python library providing uncertainty datatypes including u-type, a-type and s-type: 
+1. **u-type** datatypes: ubool, uint, ufloat, ustr, uenum.
+    Type U is a pair (x, u), noted x ± u, that represents a random variable whose average is x and standard deviation is u.
+2. **a-type** datatypes: abool, aint, afloat.
+    Type A, maintain the set of the measured values as X = {x1,...,xn}, x ± u could be calculated as the mean and standard deviation.
+3. **s-type** datatype: sbool.
+    A particular type of subjective uncertainty (Belief Uncertainty) when a user is not sure about the truth of a statement.
+
+Math functions with the datatypes are also provided.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.
 
 ```bash
 pip install uncertainty-datatypes
 ```
 <sub>Note pip3 may be used instead of pip</sub> 
 
-## The library
-
-The library provides three kinds of datatypes: 
-1. **u-type** datatypes: ubool, uint, ufloat, ustr, uenum.
-    Type U is a pair (x, u), noted x ± u, that represents a random variable whose average is x and standard deviation is u.
-2. **a-type** datatypes: abool, aint, afloat.
-    Type A, maintain the set of the measured values as X = {x1,...,xn}, x ± u could be calculated as the mean and standard deviation.
-3. **s-type** datatype: sbool.
-    A particular type of subjective uncertainty (Belief Uncertainty) when a user is not sure about the truth of a statement.
-
-Math functions with the datatypes are also provided.
-
 ## Usage
 
 Import all the datatypes and functions using:
 ```python
 from udatatypes.utypes import *
 ```
```

### Comparing `uncertainty-datatypes-1.0.4/pyproject.toml` & `uncertainty-datatypes-1.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "uncertainty-datatypes"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Atenea Research Group, University of Malaga, Spain" },
 ]
 description = "Uncertainty Datatypes Library"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers=[
```

### Comparing `uncertainty-datatypes-1.0.4/test/test_ubool.py` & `uncertainty-datatypes-1.0.5/test/test_ubool.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.4/test/test_ufloat.py` & `uncertainty-datatypes-1.0.5/test/test_ufloat.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.4/test/test_uint.py` & `uncertainty-datatypes-1.0.5/test/test_uint.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.4/udatatypes/ubool.py` & `uncertainty-datatypes-1.0.5/udatatypes/ubool.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,14 +142,17 @@
 
     def copy(self) -> ubool:
         return ubool(self.c)
 
     ''' Conversions '''
     def __str__(self) -> str:
         return 'ubool({:5.3f})'.format(self.c)
+    
+    def __repr__(self) -> str:
+        return 'ubool({:5.3f})'.format(self.c)
 
     def tobool(self, c: float = None) -> bool:
         if c is None:
             c = self.__class__.CERTAINTY
         return self.c >= c
     
     def __bool__(self) -> bool:
```

### Comparing `uncertainty-datatypes-1.0.4/udatatypes/unumbers.py` & `uncertainty-datatypes-1.0.5/udatatypes/unumbers.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.4/udatatypes/utypes.py` & `uncertainty-datatypes-1.0.5/udatatypes/utypes.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.4/uncertainty_datatypes.egg-info/PKG-INFO` & `uncertainty-datatypes-1.0.5/uncertainty_datatypes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uncertainty-datatypes
-Version: 1.0.4
+Version: 1.0.5
 Summary: Uncertainty Datatypes Library
 Author: Atenea Research Group, University of Malaga, Spain
 Project-URL: Homepage, https://github.com/atenearesearchgroup/uncertainty
 Project-URL: Bug Tracker, https://github.com/atenearesearchgroup/uncertainty/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -15,37 +15,33 @@
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Uncertainty Python Library
 
-Uncertainty is a Python library providing uncertainty datatypes including u-type, a-type and s-type.
+Uncertainty is a Python library providing uncertainty datatypes including u-type, a-type and s-type: 
+1. **u-type** datatypes: ubool, uint, ufloat, ustr, uenum.
+    Type U is a pair (x, u), noted x ± u, that represents a random variable whose average is x and standard deviation is u.
+2. **a-type** datatypes: abool, aint, afloat.
+    Type A, maintain the set of the measured values as X = {x1,...,xn}, x ± u could be calculated as the mean and standard deviation.
+3. **s-type** datatype: sbool.
+    A particular type of subjective uncertainty (Belief Uncertainty) when a user is not sure about the truth of a statement.
+
+Math functions with the datatypes are also provided.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.
 
 ```bash
 pip install uncertainty-datatypes
 ```
 <sub>Note pip3 may be used instead of pip</sub> 
 
-## The library
-
-The library provides three kinds of datatypes: 
-1. **u-type** datatypes: ubool, uint, ufloat, ustr, uenum.
-    Type U is a pair (x, u), noted x ± u, that represents a random variable whose average is x and standard deviation is u.
-2. **a-type** datatypes: abool, aint, afloat.
-    Type A, maintain the set of the measured values as X = {x1,...,xn}, x ± u could be calculated as the mean and standard deviation.
-3. **s-type** datatype: sbool.
-    A particular type of subjective uncertainty (Belief Uncertainty) when a user is not sure about the truth of a statement.
-
-Math functions with the datatypes are also provided.
-
 ## Usage
 
 Import all the datatypes and functions using:
 ```python
 from udatatypes.utypes import *
 ```
```

