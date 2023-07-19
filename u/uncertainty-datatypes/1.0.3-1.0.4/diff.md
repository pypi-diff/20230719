# Comparing `tmp/uncertainty-datatypes-1.0.3.tar.gz` & `tmp/uncertainty-datatypes-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uncertainty-datatypes-1.0.3.tar", last modified: Tue Jul 18 13:56:00 2023, max compression
+gzip compressed data, was "uncertainty-datatypes-1.0.4.tar", last modified: Wed Jul 19 09:01:31 2023, max compression
```

## Comparing `uncertainty-datatypes-1.0.3.tar` & `uncertainty-datatypes-1.0.4.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-18 13:56:00.096875 uncertainty-datatypes-1.0.3/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     1099 2023-07-17 07:54:55.000000 uncertainty-datatypes-1.0.3/LICENSE
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10278 2023-07-18 13:56:00.096702 uncertainty-datatypes-1.0.3/PKG-INFO
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     9507 2023-07-18 13:42:07.000000 uncertainty-datatypes-1.0.3/README.md
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-18 13:56:00.095201 uncertainty-datatypes-1.0.3/Uncertainty_Datatypes.egg-info/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10278 2023-07-18 13:56:00.000000 uncertainty-datatypes-1.0.3/Uncertainty_Datatypes.egg-info/PKG-INFO
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      665 2023-07-18 13:56:00.000000 uncertainty-datatypes-1.0.3/Uncertainty_Datatypes.egg-info/SOURCES.txt
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        1 2023-07-18 13:56:00.000000 uncertainty-datatypes-1.0.3/Uncertainty_Datatypes.egg-info/dependency_links.txt
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       14 2023-07-18 13:56:00.000000 uncertainty-datatypes-1.0.3/Uncertainty_Datatypes.egg-info/requires.txt
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       11 2023-07-18 13:56:00.000000 uncertainty-datatypes-1.0.3/Uncertainty_Datatypes.egg-info/top_level.txt
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      854 2023-07-18 13:55:47.000000 uncertainty-datatypes-1.0.3/pyproject.toml
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       38 2023-07-18 13:56:00.096915 uncertainty-datatypes-1.0.3/setup.cfg
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-18 13:56:00.095669 uncertainty-datatypes-1.0.3/test/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4428 2023-07-18 10:58:49.000000 uncertainty-datatypes-1.0.3/test/test_ubool.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    13629 2023-07-18 11:54:36.000000 uncertainty-datatypes-1.0.3/test/test_ufloat.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      773 2023-07-18 08:46:41.000000 uncertainty-datatypes-1.0.3/test/test_ufuncs.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    12724 2023-07-18 11:52:34.000000 uncertainty-datatypes-1.0.3/test/test_uint.py
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-18 13:56:00.096262 uncertainty-datatypes-1.0.3/udatatypes/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-14 08:59:58.000000 uncertainty-datatypes-1.0.3/udatatypes/__init__.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      328 2023-07-17 11:29:42.000000 uncertainty-datatypes-1.0.3/udatatypes/result.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4311 2023-07-18 13:55:19.000000 uncertainty-datatypes-1.0.3/udatatypes/ubool.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    20250 2023-07-18 13:47:37.000000 uncertainty-datatypes-1.0.3/udatatypes/unumbers.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4136 2023-07-18 13:12:04.000000 uncertainty-datatypes-1.0.3/udatatypes/utypes.py
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:01:31.861070 uncertainty-datatypes-1.0.4/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     1099 2023-07-17 07:54:55.000000 uncertainty-datatypes-1.0.4/LICENSE
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10278 2023-07-19 09:01:31.860906 uncertainty-datatypes-1.0.4/PKG-INFO
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     9507 2023-07-18 13:42:07.000000 uncertainty-datatypes-1.0.4/README.md
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      854 2023-07-19 09:01:10.000000 uncertainty-datatypes-1.0.4/pyproject.toml
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       38 2023-07-19 09:01:31.861110 uncertainty-datatypes-1.0.4/setup.cfg
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:01:31.858147 uncertainty-datatypes-1.0.4/test/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4428 2023-07-18 10:58:49.000000 uncertainty-datatypes-1.0.4/test/test_ubool.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    19028 2023-07-19 08:55:34.000000 uncertainty-datatypes-1.0.4/test/test_ufloat.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    17972 2023-07-19 08:39:29.000000 uncertainty-datatypes-1.0.4/test/test_uint.py
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:01:31.859835 uncertainty-datatypes-1.0.4/udatatypes/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-14 08:59:58.000000 uncertainty-datatypes-1.0.4/udatatypes/__init__.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      328 2023-07-17 11:29:42.000000 uncertainty-datatypes-1.0.4/udatatypes/result.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4228 2023-07-18 09:14:56.000000 uncertainty-datatypes-1.0.4/udatatypes/ubool.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    20720 2023-07-19 08:56:16.000000 uncertainty-datatypes-1.0.4/udatatypes/unumbers.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4302 2023-07-19 08:56:26.000000 uncertainty-datatypes-1.0.4/udatatypes/utypes.py
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:01:31.860734 uncertainty-datatypes-1.0.4/uncertainty_datatypes.egg-info/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10278 2023-07-19 09:01:31.000000 uncertainty-datatypes-1.0.4/uncertainty_datatypes.egg-info/PKG-INFO
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      421 2023-07-19 09:01:31.000000 uncertainty-datatypes-1.0.4/uncertainty_datatypes.egg-info/SOURCES.txt
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        1 2023-07-19 09:01:31.000000 uncertainty-datatypes-1.0.4/uncertainty_datatypes.egg-info/dependency_links.txt
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       14 2023-07-19 09:01:31.000000 uncertainty-datatypes-1.0.4/uncertainty_datatypes.egg-info/requires.txt
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       11 2023-07-19 09:01:31.000000 uncertainty-datatypes-1.0.4/uncertainty_datatypes.egg-info/top_level.txt
```

### Comparing `uncertainty-datatypes-1.0.3/LICENSE` & `uncertainty-datatypes-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.3/PKG-INFO` & `uncertainty-datatypes-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uncertainty-datatypes
-Version: 1.0.3
+Version: 1.0.4
 Summary: Uncertainty Datatypes Library
 Author: Atenea Research Group, University of Malaga, Spain
 Project-URL: Homepage, https://github.com/atenearesearchgroup/uncertainty
 Project-URL: Bug Tracker, https://github.com/atenearesearchgroup/uncertainty/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `uncertainty-datatypes-1.0.3/README.md` & `uncertainty-datatypes-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.3/Uncertainty_Datatypes.egg-info/PKG-INFO` & `uncertainty-datatypes-1.0.4/uncertainty_datatypes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uncertainty-datatypes
-Version: 1.0.3
+Version: 1.0.4
 Summary: Uncertainty Datatypes Library
 Author: Atenea Research Group, University of Malaga, Spain
 Project-URL: Homepage, https://github.com/atenearesearchgroup/uncertainty
 Project-URL: Bug Tracker, https://github.com/atenearesearchgroup/uncertainty/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `uncertainty-datatypes-1.0.3/test/test_ubool.py` & `uncertainty-datatypes-1.0.4/test/test_ubool.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.3/test/test_ufloat.py` & `uncertainty-datatypes-1.0.4/test/test_ufloat.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def execute(l, r, e, func, method, op, rev_op):
     t(func(l, r), e)            #   add(l, r)
     if isinstance(l, ufloat): 
         t(method(l, r), e)      #   l.add(r)
         t(op(l, r),     e)      #   l + r
     elif isinstance(r, ufloat): 
-        t(rev_op(l, r), e)      #   5 + r
+        t(rev_op(r, l), e)      #   5 + r
 
 def negs(l, e):
     t(neg(l),  e)
     t(l.neg(), e)
     t(-l,      e)
 
 def adds(l, r, e):
@@ -34,16 +34,19 @@
 def floordivs(l, r, e):
     execute(l, r, e, floordiv, ufloat.floordiv, ufloat.__floordiv__,  ufloat.__rfloordiv__)
 
 def pows(l, r, e):
     execute(l, r, e, pow, ufloat.power, ufloat.__pow__,  ufloat.__pow__)
 
 def func_execute(l, e, func, method):
-    t(func(l,), e)    #   sqrt(l)
-    t(method(l,), e)  #   sqrt(l)
+    t(func(l), e)    #   sqrt(l)
+    t(method(l), e)  #   sqrt(l)
+
+def abss(l, e):
+    func_execute(l, e, abs, ufloat.abs)
 
 def sqrts(l, e):
     func_execute(l, e, sqrt, ufloat.sqrt)
 
 def sins(l, e):
     func_execute(l, e, sin, ufloat.sin)
 
@@ -134,152 +137,227 @@
         t(ufloat('23.4', '1.7'), ufloat(23.4, 1.7))
         t(ufloat('25', '1'),     ufloat(25.0, 1.0))
 
     '''
         Operators
     '''
     def test_add(self):
-        ''' add + ufloat '''
+        ''' add ufloat + ufloat '''
         adds(self.ufa, self.ufa, ufloat(-8.000, 4.243))
         adds(self.ufa, self.ufb, ufloat(-2.000, 5.000))
         adds(self.ufb, self.ufb, ufloat( 4.000, 5.657))
         adds(self.ufb, self.ufa, ufloat(-2.000, 5.000))
 
     def test_add_uint(self):
-        ''' add + uint '''
+        ''' add ufloat + uint '''
         adds(self.ufa, self.uia, ufloat(-8.000, 4.243))
         adds(self.ufa, self.uib, ufloat(-2.000, 5.000))
         adds(self.ufb, self.uia, ufloat(-2.000, 5.000))
         adds(self.ufb, self.uib, ufloat( 4.000, 5.657))
+        ''' add uint + ufloat '''
+        adds(self.uia, self.ufa, ufloat(-8.000, 4.243))
+        adds(self.uib, self.ufa, ufloat(-2.000, 5.000))
+        adds(self.uia, self.ufb, ufloat(-2.000, 5.000))
+        adds(self.uib, self.ufb, ufloat( 4.000, 5.657))
 
     def test_add_int(self):
-        ''' add + int '''
+        ''' add ufloat + int '''
         adds(self.ufa, self.ia, ufloat(-8.000, 3.000))
         adds(self.ufa, self.ib, ufloat(-2.000, 3.000))
         adds(self.ufb, self.ia, ufloat(-2.000, 4.000))
         adds(self.ufb, self.ib, ufloat( 4.000, 4.000))
+        ''' add int + ufloat '''
+        adds(self.ia, self.ufa, ufloat(-8.000, 3.000))
+        adds(self.ib, self.ufa, ufloat(-2.000, 3.000))
+        adds(self.ia, self.ufb, ufloat(-2.000, 4.000))
+        adds(self.ib, self.ufb, ufloat( 4.000, 4.000))
 
     def test_add_float(self):
-        ''' add + float '''
+        ''' add ufloat + float '''
         adds(self.ufa, self.fa, ufloat(-28.720, 3.000))
         adds(self.ufa, self.fb, ufloat(8.560, 3.000))
         adds(self.ufb, self.fa, ufloat(-22.720, 4.000))
         adds(self.ufb, self.fb, ufloat(14.560, 4.000))
+        ''' add float + ufloat '''
+        adds(self.fa, self.ufa, ufloat(-28.720, 3.000))
+        adds(self.fb, self.ufa, ufloat(8.560, 3.000))
+        adds(self.fa, self.ufb, ufloat(-22.720, 4.000))
+        adds(self.fb, self.ufb, ufloat(14.560, 4.000))
 
     def test_sub(self):
-        ''' sub - ufloat '''
+        ''' sub ufloat - ufloat '''
         subs(self.ufa, self.ufa, ufloat( 0.000, 0.000))
         subs(self.ufa, self.ufb, ufloat(-6.000, 5.000))
         subs(self.ufb, self.ufb, ufloat( 0.000, 0.000))
         subs(self.ufb, self.ufa, ufloat( 6.000, 5.000))
 
     def test_sub_uint(self):
-        ''' sub - uint '''
+        ''' sub ufloat - uint '''
         subs(self.ufa, self.uia, ufloat( 0.000, 4.243))
         subs(self.ufa, self.uib, ufloat(-6.000, 5.000))
         subs(self.ufb, self.uia, ufloat( 6.000, 5.000))
         subs(self.ufb, self.uib, ufloat( 0.000, 5.657))
+        ''' sub uint - ufloat '''
+        subs(self.uia, self.ufa, ufloat( 0.000, 4.243))
+        subs(self.uib, self.ufa, ufloat( 6.000, 5.000))
+        subs(self.uia, self.ufb, ufloat(-6.000, 5.000))
+        subs(self.uib, self.ufb, ufloat( 0.000, 5.657))
 
     def test_sub_int(self):
-        ''' sub - int '''
+        ''' sub ufloat - int '''
         subs(self.ufa, self.ia, ufloat( 0.000, 3.000))
         subs(self.ufa, self.ib, ufloat(-6.000, 3.000))
         subs(self.ufb, self.ia, ufloat( 6.000, 4.000))
         subs(self.ufb, self.ib, ufloat( 0.000, 4.000))
+        ''' sub int - ufloat '''
+        subs(self.ia, self.ufa, ufloat( 0.000, 3.000))
+        subs(self.ib, self.ufa, ufloat( 6.000, 3.000))
+        subs(self.ia, self.ufb, ufloat(-6.000, 4.000))
+        subs(self.ib, self.ufb, ufloat( 0.000, 4.000))
 
     def test_sub_float(self):
-        ''' sub - float '''
+        ''' sub ufloat - float '''
         subs(self.ufa, self.fa, ufloat( 20.720, 3.000))
         subs(self.ufa, self.fb, ufloat(-16.560, 3.000))
         subs(self.ufb, self.fa, ufloat( 26.720, 4.000))
         subs(self.ufb, self.fb, ufloat(-10.560, 4.000))
+        ''' sub float - ufloat'''
+        subs(self.fa, self.ufa, ufloat(-20.720, 3.000))
+        subs(self.fb, self.ufa, ufloat( 16.560, 3.000))
+        subs(self.fa, self.ufb, ufloat(-26.720, 4.000))
+        subs(self.fb, self.ufb, ufloat( 10.560, 4.000))
         
     def test_mul(self):
-        ''' mul * ufloat '''
+        ''' mul ufloat * ufloat '''
         muls(self.ufa, self.ufa, ufloat(16.000, 16.971))
         muls(self.ufa, self.ufb, ufloat(-8.000, 17.088))
         muls(self.ufb, self.ufb, ufloat( 4.000, 11.314))
         muls(self.ufb, self.ufa, ufloat(-8.000, 17.088))
         
     def test_mul_uint(self):
-        ''' mul * uint '''
+        ''' mul ufloat * uint '''
         muls(self.ufa, self.uia, ufloat(16.000, 16.971))
         muls(self.ufa, self.uib, ufloat(-8.000, 17.088))
         muls(self.ufb, self.uia, ufloat(-8.000, 17.088))
         muls(self.ufb, self.uib, ufloat( 4.000, 11.314))
+        ''' mul uint * ufloat '''
+        muls(self.uia, self.ufa, ufloat(16.000, 16.971))
+        muls(self.uib, self.ufa, ufloat(-8.000, 17.088))
+        muls(self.uia, self.ufb, ufloat(-8.000, 17.088))
+        muls(self.uib, self.ufb, ufloat( 4.000, 11.314))
 
     def test_mul_int(self):
-        ''' mul * int '''
+        ''' mul ufloat * int '''
         muls(self.ufa, self.ia, ufloat(16.000, 12.000))
         muls(self.ufa, self.ib, ufloat(-8.000,  6.000))
         muls(self.ufb, self.ia, ufloat(-8.000, 16.000))
         muls(self.ufb, self.ib, ufloat( 4.000,  8.000))
+        ''' mul int * ufloat '''
+        muls(self.ia, self.ufa, ufloat(16.000, 12.000))
+        muls(self.ib, self.ufa, ufloat(-8.000,  6.000))
+        muls(self.ia, self.ufb, ufloat(-8.000, 16.000))
+        muls(self.ib, self.ufb, ufloat( 4.000,  8.000))
 
     def test_mul_float(self):
-        ''' mul * float '''
+        ''' mul ufloat * float '''
         muls(self.ufa, self.fa, ufloat( 98.880, 74.160))
         muls(self.ufa, self.fb, ufloat(-50.240, 37.680))
         muls(self.ufb, self.fa, ufloat(-49.440, 98.880))
         muls(self.ufb, self.fb, ufloat( 25.120, 50.240))
+        ''' mul float * ufloat '''
+        muls(self.fa, self.ufa, ufloat( 98.880, 74.160))
+        muls(self.fb, self.ufa, ufloat(-50.240, 37.680))
+        muls(self.fa, self.ufb, ufloat(-49.440, 98.880))
+        muls(self.fb, self.ufb, ufloat( 25.120, 50.240))
 
     def test_div(self):
-        ''' div / ufloat '''
+        ''' div ufloat / ufloat '''
         divs(self.ufa, self.ufa, ufloat( 1.000, 0.000))
         divs(self.ufa, self.ufb, ufloat(-2.000, 4.528))
         divs(self.ufb, self.ufb, ufloat( 1.000, 0.000))
         divs(self.ufb, self.ufa, ufloat(-0.500, 2.035))
         
     def test_div_uint(self):
-        ''' div / uint '''
+        ''' div ufloat / uint '''
         divs(self.ufa, self.uia, ufloat( 1.000, 1.677))
         divs(self.ufa, self.uib, ufloat(-2.000, 4.528))
         divs(self.ufb, self.uia, ufloat(-0.500, 2.035))
         divs(self.ufb, self.uib, ufloat( 1.000, 3.464))
+        ''' div uint / ufloat '''
+        divs(self.uia, self.ufa, ufloat( 1.000, 1.677))
+        divs(self.uib, self.ufa, ufloat(-0.500, 2.035))
+        divs(self.uia, self.ufb, ufloat(-2.000, 4.528))
+        divs(self.uib, self.ufb, ufloat( 1.000, 3.464))
 
     def test_div_int(self):
-        ''' div / int '''
+        ''' div ufloat / int '''
         divs(self.ufa, self.ia, ufloat( 1.000, 0.750))
         divs(self.ufa, self.ib, ufloat(-2.000, 1.500))
         divs(self.ufb, self.ia, ufloat(-0.500, 1.000))
         divs(self.ufb, self.ib, ufloat( 1.000, 2.000))
+        ''' div int / ufloat '''
+        divs(self.ia, self.ufa, ufloat( 1.000, 0.188))
+        divs(self.ib, self.ufa, ufloat(-0.500, 0.188))
+        divs(self.ia, self.ufb, ufloat(-2.000, 1.000))
+        divs(self.ib, self.ufb, ufloat( 1.000, 1.000))
 
     def test_div_float(self):
-        ''' div / float '''
-        divs(self.ufa, self.fa, ufloat(0.162, 0.121))
+        ''' div ufloat / float '''
+        divs(self.ufa, self.fa, ufloat( 0.162, 0.121))
         divs(self.ufa, self.fb, ufloat(-0.318, 0.239))
         divs(self.ufb, self.fa, ufloat(-0.081, 0.162))
-        divs(self.ufb, self.fb, ufloat(0.159, 0.318))
+        divs(self.ufb, self.fb, ufloat( 0.159, 0.318))
+        ''' div float / ufloat '''
+        divs(self.fa, self.ufa, ufloat(  6.180, 0.188))
+        divs(self.fb, self.ufa, ufloat(- 3.140, 0.188))
+        divs(self.fa, self.ufb, ufloat(-12.360, 1.000))
+        divs(self.fb, self.ufb, ufloat(  6.280, 1.000))
 
     def test_floordiv(self):
-        ''' floor div // ufloat '''
+        ''' floordiv ufloat // ufloat '''
         floordivs(self.ufa, self.ufa, ufloat( 1.000, 0.000))
         floordivs(self.ufa, self.ufb, ufloat(-2.000, 4.528))
         floordivs(self.ufb, self.ufb, ufloat( 1.000, 0.000))
         floordivs(self.ufb, self.ufa, ufloat(-1.000, 2.035))
         
     def test_floordiv_uint(self):
-        ''' floor div // uint '''
+        ''' floordiv ufloat // uint '''
         floordivs(self.ufa, self.uia, ufloat( 1.000, 1.677))
         floordivs(self.ufa, self.uib, ufloat(-2.000, 4.528))
         floordivs(self.ufb, self.uia, ufloat(-1.000, 2.035))
         floordivs(self.ufb, self.uib, ufloat( 1.000, 3.464))
+        ''' floordiv uint // ufloat '''
+        floordivs(self.uia, self.ufa, ufloat( 1.000, 1.677))
+        floordivs(self.uib, self.ufa, ufloat(-1.000, 2.035))
+        floordivs(self.uia, self.ufb, ufloat(-2.000, 4.528))
+        floordivs(self.uib, self.ufb, ufloat( 1.000, 3.464))
 
     def test_floordiv_int(self):
-        ''' floor div // int '''
+        ''' floordiv ufloat // int '''
         floordivs(self.ufa, self.ia, ufloat( 1.000, 0.750))
         floordivs(self.ufa, self.ib, ufloat(-2.000, 1.500))
         floordivs(self.ufb, self.ia, ufloat(-1.000, 1.000))
         floordivs(self.ufb, self.ib, ufloat( 1.000, 2.000))
+        ''' floordiv int // ufloat '''
+        floordivs(self.ia, self.ufa, ufloat( 1.000, 0.188))
+        floordivs(self.ib, self.ufa, ufloat(-1.000, 0.188))
+        floordivs(self.ia, self.ufb, ufloat(-2.000, 1.000))
+        floordivs(self.ib, self.ufb, ufloat( 1.000, 1.000))
 
     def test_floordiv_float(self):
-        ''' floor div // float '''
-        floordivs(self.ufa, self.fa, ufloat(0.000, 0.121))
+        ''' floordiv ufloat // float '''
+        floordivs(self.ufa, self.fa, ufloat( 0.000, 0.121))
         floordivs(self.ufa, self.fb, ufloat(-1.000, 0.239))
         floordivs(self.ufb, self.fa, ufloat(-1.000, 0.162))
-        floordivs(self.ufb, self.fb, ufloat(0.000, 0.318))
+        floordivs(self.ufb, self.fb, ufloat( 0.000, 0.318))
+        ''' floordiv float // ufloat '''
+        floordivs(self.fa, self.ufa, ufloat(  6.000, 0.188))
+        floordivs(self.fb, self.ufa, ufloat(- 4.000, 0.188))
+        floordivs(self.fa, self.ufb, ufloat(-13.000, 1.000))
+        floordivs(self.fb, self.ufb, ufloat(  6.000, 1.000))
 
     def test_neg(self):
         ''' neg - '''
         negs(self.ufa, ufloat( 4.000, 3.000))
         negs(self.ufb, ufloat(-2.000, 4.000))
         negs(self.uia, ufloat( 4.000, 3.000))
         negs(self.uib, ufloat(-2.000, 4.000))     
@@ -293,14 +371,19 @@
         pows(self.ufb, 3.25, ufloat( 9.514,  61.839))
         pows(self.ufb, 5.03, ufloat(32.672, 328.684))
 
 
     '''
         Functions
     '''
+    def test_abs(self):
+        ''' abs '''
+        abss(self.ufa, ufloat( 4.0, 3.0))
+        abss(self.ufb, ufloat( 2.0, 4.0))
+        abss(self.ufc, ufloat(23.0, 5.3))
 
     def test_sqrt(self):
         ''' sqrt '''
         sqrts(self.ufb, ufloat(1.414, 1.414))
         sqrts(self.ufc, ufloat(4.796, 0.553))
 
     def test_sin(self):
@@ -349,14 +432,28 @@
     def test_round(self):
         ''' round '''
         rounds(mul(self.ufa, self.fa), ufloat( 99.000, 74.160))
         rounds(mul(self.ufa, self.fb), ufloat(-50.000, 37.680))
         rounds(mul(self.ufb, self.fa), ufloat(-49.000, 98.880))
         rounds(mul(self.ufb, self.fb), ufloat( 25.000, 50.240))
 
+    def test_max(self):
+        ''' max '''
+        t(max(self.ufa, self.ufb, self.ufc), self.ufc)
+        t(max(abs(self.ufa), abs(self.ufb), abs(self.ufc)), self.ufc)
+        t(max(ufloat(2.2, 12), ufloat(1.3, 12), ufloat(3.7, 12), ufloat(5.3, 12), ufloat(3.1, 12), ufloat(2.6, 12), ufloat(0.6, 12), ufloat(4.4, 12)), ufloat(5.3, 12))
+        t(max(ufloat(2.2, 12), ufloat(-1.3, 12), ufloat(3.7, 12), ufloat(5.3, 12), ufloat(-3.1, 12), ufloat(2.6, 12), ufloat(-0.6, 12), ufloat(4.4, 12)), ufloat(5.3, 12))
+
+    def test_min(self):
+        ''' min '''
+        t(min(self.ufa, self.ufb, self.ufc), self.ufa)
+        t(min(abs(self.ufa), abs(self.ufb), abs(self.ufc)), self.ufb)
+        t(min(ufloat(2.2, 1), ufloat(1.3, 1), ufloat(3.7, 1), ufloat(3.3, 1), ufloat(2.1, 1), ufloat(0.6, 1), ufloat(4.6, 1), ufloat(5.4, 1)), ufloat(0.6, 1))
+        t(min(ufloat(2.2, 1), ufloat(-1.3, 1), ufloat(3.7, 1), ufloat(3.3, 1), ufloat(-2.1, 1), ufloat(0.6, 1), ufloat(-4.6, 1), ufloat(5.4, 1)), ufloat(-4.6, 1))
+
     '''
         Comparison Operators
     '''
     def test_eq(self):
         ''' eq == '''
         eqs(self.ufa, self.ufa, ubool(1.000))
         eqs(self.ufa, self.ufb, ubool(0.385))
```

### Comparing `uncertainty-datatypes-1.0.3/test/test_uint.py` & `uncertainty-datatypes-1.0.4/test/test_uint.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def execute(l, r, e, func, method, op, rev_op):
     t(func(l, r), e)            #   add(l, r)
     if isinstance(l, uint): 
         t(method(l, r), e)      #   l.add(r)
         t(op(l, r),     e)      #   l + r
     elif isinstance(r, uint): 
-        t(rev_op(l, r), e)      #   5 + r
+        t(rev_op(r, l), e)      #   5 + r
 
 def negs(l, e):
     t(neg(l),  e)
     t(l.neg(), e)
     t(-l,      e)
 
 def adds(l, r, e):
@@ -37,17 +37,20 @@
 def pows(l, r, e):
     execute(l, r, e, pow, uint.power, uint.__pow__,  uint.__pow__)
 
 def mods(l, r, e):
     execute(l, r, e, mod, uint.mod, uint.__mod__,  uint.__rmod__)
 
 def func_execute(l, e, func, method = None):
-    t(func(l,), e)    #   sqrt(l)
+    t(func(l), e)    #   sqrt(l)
     if method is not None:
-        t(method(l,), e)  #   l.sqrt())
+        t(method(l), e)  #   l.sqrt())
+
+def abss(l, e):
+    func_execute(l, e, abs)
 
 def sqrts(l, e):
     func_execute(l, e, sqrt)
 
 def sins(l, e):
     func_execute(l, e, sin)
 
@@ -74,16 +77,19 @@
 
 def floors(l, e):
     func_execute(l, e, floor)
 
 def rounds(l, e):
     func_execute(l, e, round)
 
-def mods(l, r, e):
-    execute(l, r, e, mod, uint.mod, uint.__mod__,  uint.__rmod__)
+def maxs(l, e):
+    func_execute(l, e, max)
+    
+def mins(l, e):
+    func_execute(l, e, min)
 
 def comparison_execute(l, r, e, func, method, op):
     t(func(l, r),   e)  #   lt(l, r)
     t(method(l, r), e)  #   l.lt(r)
     t(op(l, r),     e)  #   l < r
 
 def eqs(l, r, e):
@@ -131,150 +137,227 @@
         t(uint('20', '1'), uint(20, 1.0))
         t(uint('25', '1'), uint(25, 1.0))
 
     '''
         Operators
     '''
     def test_add(self):
-        ''' add + uint '''
+        ''' add uint + uint '''
         adds(self.uia, self.uia, uint(-8, 4.243))
         adds(self.uia, self.uib, uint(-2, 5.000))
         adds(self.uib, self.uib, uint( 4, 5.657))
         adds(self.uib, self.uia, uint(-2, 5.000))
-    def test_add_uint(self):
-        ''' add + uint '''
-        adds(self.uia, self.ufa, uint(-8, 4.243))
-        adds(self.uia, self.ufb, uint(-2, 5.000))
-        adds(self.uib, self.ufa, uint(-2, 5.000))
-        adds(self.uib, self.ufb, uint( 4, 5.657))
+
+    def test_add_ufloat(self):
+        ''' add uint + ufloat '''
+        adds(self.uia, self.ufa, ufloat(-8.000, 4.243))
+        adds(self.uia, self.ufb, ufloat(-2.000, 5.000))
+        adds(self.uib, self.ufa, ufloat(-2.000, 5.000))
+        adds(self.uib, self.ufb, ufloat( 4.000, 5.657))
+        ''' add ufloat + uint '''
+        adds(self.ufa, self.uia, ufloat(-8.000, 4.243))
+        adds(self.ufa, self.uib, ufloat(-2.000, 5.000))
+        adds(self.ufb, self.uia, ufloat(-2.000, 5.000))
+        adds(self.ufb, self.uib, ufloat( 4.000, 5.657))
 
     def test_add_int(self):
-        ''' add + int '''
+        ''' add uint + int '''
         adds(self.uia, self.ia, uint(-8, 3.000))
         adds(self.uia, self.ib, uint(-2, 3.000))
         adds(self.uib, self.ia, uint(-2, 4.000))
         adds(self.uib, self.ib, uint( 4, 4.000))
+        ''' add int + uint '''
+        adds(self.ia, self.uia, uint(-8, 3.000))
+        adds(self.ib, self.uia, uint(-2, 3.000))
+        adds(self.ia, self.uib, uint(-2, 4.000))
+        adds(self.ib, self.uib, uint( 4, 4.000))
 
     def test_add_float(self):
-        ''' add + float '''
+        ''' add uint + float '''
         adds(self.uia, self.fa, ufloat(-28.720, 3.000))
-        adds(self.uia, self.fb, ufloat(8.560, 3.000))
+        adds(self.uia, self.fb, ufloat(  8.560, 3.000))
         adds(self.uib, self.fa, ufloat(-22.720, 4.000))
-        adds(self.uib, self.fb, ufloat(14.560, 4.000))
+        adds(self.uib, self.fb, ufloat( 14.560, 4.000))
+        ''' add float + uint'''
+        adds(self.fa, self.uia, ufloat(-28.720, 3.000))
+        adds(self.fb, self.uia, ufloat(  8.560, 3.000))
+        adds(self.fa, self.uib, ufloat(-22.720, 4.000))
+        adds(self.fb, self.uib, ufloat( 14.560, 4.000))
 
     def test_sub(self):
-        ''' sub - uint '''
+        ''' sub uint - uint '''
         subs(self.uia, self.uia, uint( 0, 0.000))
         subs(self.uia, self.uib, uint(-6, 5.000))
         subs(self.uib, self.uib, uint( 0, 0.000))
         subs(self.uib, self.uia, uint( 6, 5.000))
 
-    def test_sub_uint(self):
-        ''' sub - uint '''
-        subs(self.uia, self.ufa, uint( 0, 4.243))
-        subs(self.uia, self.ufb, uint(-6, 5.000))
-        subs(self.uib, self.ufa, uint( 6, 5.000))
-        subs(self.uib, self.ufb, uint( 0, 5.657))
+    def test_sub_ufloat(self):
+        ''' sub uint - ufloat '''
+        subs(self.uia, self.ufa, ufloat( 0.000, 4.243))
+        subs(self.uia, self.ufb, ufloat(-6.000, 5.000))
+        subs(self.uib, self.ufa, ufloat( 6.000, 5.000))
+        subs(self.uib, self.ufb, ufloat( 0.000, 5.657))
+        ''' sub ufloat - uint '''
+        subs(self.ufa, self.uia, ufloat( 0.000, 4.243))
+        subs(self.ufb, self.uia, ufloat( 6.000, 5.000))
+        subs(self.ufa, self.uib, ufloat(-6.000, 5.000))
+        subs(self.ufb, self.uib, ufloat( 0.000, 5.657))
 
     def test_sub_int(self):
-        ''' sub - int '''
+        ''' sub uint - int '''
         subs(self.uia, self.ia, uint( 0, 3.000))
         subs(self.uia, self.ib, uint(-6, 3.000))
         subs(self.uib, self.ia, uint( 6, 4.000))
         subs(self.uib, self.ib, uint( 0, 4.000))
+        ''' sub int - uint '''
+        subs(self.ia, self.uia, uint( 0, 3.000))
+        subs(self.ib, self.uia, uint( 6, 3.000))
+        subs(self.ia, self.uib, uint(-6, 4.000))
+        subs(self.ib, self.uib, uint( 0, 4.000))
 
     def test_sub_float(self):
-        ''' sub - float '''
+        ''' sub uint - float '''
         subs(self.uia, self.fa, ufloat( 20.720, 3.000))
         subs(self.uia, self.fb, ufloat(-16.560, 3.000))
         subs(self.uib, self.fa, ufloat( 26.720, 4.000))
         subs(self.uib, self.fb, ufloat(-10.560, 4.000))
+        ''' sub float - uint '''
+        subs(self.fa, self.uia, ufloat(-20.720, 3.000))
+        subs(self.fb, self.uia, ufloat( 16.560, 3.000))
+        subs(self.fa, self.uib, ufloat(-26.720, 4.000))
+        subs(self.fb, self.uib, ufloat( 10.560, 4.000))
 
     def test_mul(self):
-        ''' mul * uint '''
+        ''' mul uint * uint '''
         muls(self.uia, self.uia, uint(16, 16.971))
         muls(self.uia, self.uib, uint(-8, 17.088))
         muls(self.uib, self.uib, uint( 4, 11.314))
         muls(self.uib, self.uia, uint(-8, 17.088))
         
-    def test_mul_uint(self):
-        ''' mul * uint '''
-        muls(self.uia, self.ufa, uint(16, 16.971))
-        muls(self.uia, self.ufb, uint(-8, 17.088))
-        muls(self.uib, self.ufa, uint(-8, 17.088))
-        muls(self.uib, self.ufb, uint( 4, 11.314))
+    def test_mul_ufloat(self):
+        ''' mul uint * ufloat '''
+        muls(self.uia, self.ufa, ufloat(16.000, 16.971))
+        muls(self.uia, self.ufb, ufloat(-8.000, 17.088))
+        muls(self.uib, self.ufa, ufloat(-8.000, 17.088))
+        muls(self.uib, self.ufb, ufloat( 4.000, 11.314))
+        ''' mul ufloat * uint '''
+        muls(self.ufa, self.uia, ufloat(16.000, 16.971))
+        muls(self.ufb, self.uia, ufloat(-8.000, 17.088))
+        muls(self.ufa, self.uib, ufloat(-8.000, 17.088))
+        muls(self.ufb, self.uib, ufloat( 4.000, 11.314))
 
     def test_mul_int(self):
-        ''' mul * int '''
+        ''' mul uint * int '''
         muls(self.uia, self.ia, uint(16, 12.000))
         muls(self.uia, self.ib, uint(-8,  6.000))
         muls(self.uib, self.ia, uint(-8, 16.000))
         muls(self.uib, self.ib, uint( 4,  8.000))
+        ''' mul int * uint '''
+        muls(self.ia, self.uia, uint(16, 12.000))
+        muls(self.ib, self.uia, uint(-8,  6.000))
+        muls(self.ia, self.uib, uint(-8, 16.000))
+        muls(self.ib, self.uib, uint( 4,  8.000))
 
     def test_mul_float(self):
-        ''' mul * float '''
+        ''' mul uint * float '''
         muls(self.uia, self.fa, ufloat( 98.880, 74.160))
         muls(self.uia, self.fb, ufloat(-50.240, 37.680))
         muls(self.uib, self.fa, ufloat(-49.440, 98.880))
         muls(self.uib, self.fb, ufloat( 25.120, 50.240))
+        ''' mul float * uint '''
+        muls(self.fa, self.uia, ufloat( 98.880, 74.160))
+        muls(self.fb, self.uia, ufloat(-50.240, 37.680))
+        muls(self.fa, self.uib, ufloat(-49.440, 98.880))
+        muls(self.fb, self.uib, ufloat( 25.120, 50.240))
 
     def test_div(self):
-        ''' div / uint '''
+        ''' div uint / uint '''
         divs(self.uia, self.uia, ufloat( 1.000, 1.677))
         divs(self.uia, self.uib, ufloat(-2.000, 4.528))
         divs(self.uib, self.uib, ufloat( 1.000, 3.464))
         divs(self.uib, self.uia, ufloat(-0.500, 2.035))
         
-    def test_div_uint(self):
-        ''' div / uint '''
+    def test_div_ufloat(self):
+        ''' div uint / ufloat '''
         divs(self.uia, self.ufa, ufloat( 1.000, 1.677))
         divs(self.uia, self.ufb, ufloat(-2.000, 4.528))
         divs(self.uib, self.ufa, ufloat(-0.500, 2.035))
         divs(self.uib, self.ufb, ufloat( 1.000, 3.464))
+        ''' div ufloat / uint '''
+        divs(self.ufa, self.uia, ufloat( 1.000, 1.677))
+        divs(self.ufb, self.uia, ufloat(-0.500, 2.035))
+        divs(self.ufa, self.uib, ufloat(-2.000, 4.528))
+        divs(self.ufb, self.uib, ufloat( 1.000, 3.464))
 
     def test_div_int(self):
-        ''' div / int '''
+        ''' div uint / int '''
         divs(self.uia, self.ia, ufloat( 1.000, 0.750))
         divs(self.uia, self.ib, ufloat(-2.000, 1.500))
         divs(self.uib, self.ia, ufloat(-0.500, 1.000))
         divs(self.uib, self.ib, ufloat( 1.000, 2.000))
+        ''' div int / uint '''
+        divs(self.ia, self.uia, ufloat( 1.000, 0.188))
+        divs(self.ib, self.uia, ufloat(-0.500, 0.188))
+        divs(self.ia, self.uib, ufloat(-2.000, 1.000))
+        divs(self.ib, self.uib, ufloat( 1.000, 1.000))
 
     def test_div_float(self):
-        ''' div / float '''
+        ''' div uint / float '''
         divs(self.uia, self.fa, ufloat(0.162, 0.121))
         divs(self.uia, self.fb, ufloat(-0.318, 0.239))
         divs(self.uib, self.fa, ufloat(-0.081, 0.162))
         divs(self.uib, self.fb, ufloat(0.159, 0.318))
+        ''' div float / uint '''
+        divs(self.fa, self.uia, ufloat(  6.180, 0.188))
+        divs(self.fb, self.uia, ufloat(- 3.140, 0.188))
+        divs(self.fa, self.uib, ufloat(-12.360, 1.000))
+        divs(self.fb, self.uib, ufloat(  6.280, 1.000))
+    
     def test_floordiv(self):
-        ''' floor div // uint '''
+        ''' floordiv uint // uint '''
         floordivs(self.uia, self.uia, uint( 1, 0.000))
         floordivs(self.uia, self.uib, uint(-2, 4.528))
         floordivs(self.uib, self.uib, uint( 1, 0.000))
         floordivs(self.uib, self.uia, uint(-1, 2.035))
         
-    def test_floordiv_uint(self):
-        ''' floor div // uint '''
-        floordivs(self.uia, self.ufa, uint( 1, 1.677))
-        floordivs(self.uia, self.ufb, uint(-2, 4.528))
-        floordivs(self.uib, self.ufa, uint(-1, 2.035))
-        floordivs(self.uib, self.ufb, uint( 1, 3.464))
+    def test_floordiv_ufloat(self):
+        ''' floordiv uint // ufloat '''
+        floordivs(self.uia, self.ufa, ufloat( 1.000, 1.677))
+        floordivs(self.uia, self.ufb, ufloat(-2.000, 4.528))
+        floordivs(self.uib, self.ufa, ufloat(-1.000, 2.035))
+        floordivs(self.uib, self.ufb, ufloat( 1.000, 3.464))
+        ''' floordiv ufloat // uint '''
+        floordivs(self.ufa, self.uia, ufloat( 1.000, 1.677))
+        floordivs(self.ufb, self.uia, ufloat(-1.000, 2.035))
+        floordivs(self.ufa, self.uib, ufloat(-2.000, 4.528))
+        floordivs(self.ufb, self.uib, ufloat( 1.000, 3.464))
 
     def test_floordiv_int(self):
-        ''' floor div // int '''
+        ''' floordiv uint // int '''
         floordivs(self.uia, self.ia, uint( 1, 0.750))
         floordivs(self.uia, self.ib, uint(-2, 1.500))
         floordivs(self.uib, self.ia, uint(-1, 1.000))
         floordivs(self.uib, self.ib, uint( 1, 2.000))
+        ''' floordiv int // uint '''
+        floordivs(self.ia, self.uia, uint( 1, 0.188))
+        floordivs(self.ib, self.uia, uint(-1, 0.188))
+        floordivs(self.ia, self.uib, uint(-2, 1.000))
+        floordivs(self.ia, self.uib, uint(-2, 1.000))
 
     def test_floordiv_float(self):
-        ''' floor div // float '''
-        floordivs(self.uia, self.fa, uint( 0, 0.121))
-        floordivs(self.uia, self.fb, uint(-1, 0.239))
-        floordivs(self.uib, self.fa, uint(-1, 0.162))
-        floordivs(self.uib, self.fb, uint( 0, 0.318))
+        ''' floordiv uint // float '''
+        floordivs(self.uia, self.fa, ufloat( 0.000, 0.121))
+        floordivs(self.uia, self.fb, ufloat(-1.000, 0.239))
+        floordivs(self.uib, self.fa, ufloat(-1.000, 0.162))
+        floordivs(self.uib, self.fb, ufloat( 0.000, 0.318))
+        ''' floordiv float // uint '''
+        floordivs(self.fa, self.uia, ufloat(  6.000, 0.188))
+        floordivs(self.fb, self.uia, ufloat(- 4.000, 0.188))
+        floordivs(self.fa, self.uib, ufloat(-13.000, 1.000))
+        floordivs(self.fb, self.uib, ufloat(  6.000, 1.000))
         
     def test_neg(self):
         ''' neg - '''
         negs(self.uia, uint( 4, 3.000))
         negs(self.uib, uint(-2, 4.000))
         negs(self.ufa, uint( 4, 3.000))
         negs(self.ufb, uint(-2, 4.000))     
@@ -287,14 +370,19 @@
         pows(self.uib, 2.50, ufloat( 5.657,  28.284))
         pows(self.uib, 3.25, ufloat( 9.514,  61.839))
         pows(self.uib, 5.03, ufloat(32.672, 328.684))
 
     '''
         Functions
     '''
+    def test_abs(self):
+        ''' abs '''
+        abss(self.uia, ufloat( 4.0, 3.0))
+        abss(self.uib, ufloat( 2.0, 4.0))
+        abss(self.uic, ufloat(23.0, 5.3))
 
     def test_sqrt(self):
         ''' sqrt '''
         sqrts(self.uib, ufloat(1.414, 1.414))
         sqrts(self.uic, ufloat(4.796, 0.553))
 
     def test_sin(self):
@@ -343,14 +431,28 @@
     def test_round(self):
         ''' round '''
         rounds(mul(self.uia, self.fa), uint( 99, 74.160))
         rounds(mul(self.uia, self.fb), uint(-50, 37.680))
         rounds(mul(self.uib, self.fa), uint(-49, 98.880))
         rounds(mul(self.uib, self.fb), uint( 25, 50.240))
 
+    def test_max(self):
+        ''' max '''
+        t(max(self.uia, self.uib, self.uic), self.uic)
+        t(max(abs(self.uia), abs(self.uib), abs(self.uic)), self.uic)
+        t(max(uint(2, 12), uint(1, 12), uint(3, 12), uint(5, 12), uint(3, 12), uint(2, 12), uint(0, 12), uint(4, 12)), uint(5, 12))
+        t(max(uint(2, 12), uint(-1, 12), uint(3, 12), uint(5, 12), uint(-3, 12), uint(2, 12), uint(-0, 12), uint(4, 12)), uint(5, 12))
+
+    def test_min(self):
+        ''' min '''
+        t(min(self.uia, self.uib, self.uic), self.uia)
+        t(min(abs(self.uia), abs(self.uib), abs(self.uic)), self.uib)
+        t(min(uint(2, 1), uint(1, 1), uint(3, 1), uint(3, 1), uint(2, 1), uint(0, 1), uint(4, 1), uint(5, 1)), uint(0, 1))
+        t(min(uint(2, 1), uint(-1, 1), uint(3, 1), uint(3, 1), uint(-2, 1), uint(0, 1), uint(-4, 1), uint(5, 1)), uint(-4, 1))
+
     '''
         Comparison Operators
     '''
     def test_eq(self):
         ''' eq == '''
         eqs(self.uia, self.uia, ubool(1.000))
         eqs(self.uia, self.uib, ubool(0.385))
```

### Comparing `uncertainty-datatypes-1.0.3/udatatypes/ubool.py` & `uncertainty-datatypes-1.0.4/udatatypes/ubool.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,17 +142,14 @@
 
     def copy(self) -> ubool:
         return ubool(self.c)
 
     ''' Conversions '''
     def __str__(self) -> str:
         return 'ubool({:5.3f})'.format(self.c)
-    
-    def __repr__(self) -> str:
-        return 'ubool({:5.3f})'.format(self.c)
 
     def tobool(self, c: float = None) -> bool:
         if c is None:
             c = self.__class__.CERTAINTY
         return self.c >= c
     
     def __bool__(self) -> bool:
```

### Comparing `uncertainty-datatypes-1.0.3/udatatypes/unumbers.py` & `uncertainty-datatypes-1.0.4/udatatypes/unumbers.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,17 +51,22 @@
 			
 		return uint(self.x + r.x, math.sqrt((self.u * self.u) + (r.u**2) + 2 * covariance))
 	
 	def __add__(self, r: int|uint) -> uint:
 		return self.add(r)
 	
 	def __radd__(self, left) -> uint:
-		return uint(left).__add__(self)
+		if isinstance(left, int):
+			left = uint(left)
+		elif isinstance(left, float):
+			left = ufloat(left)
+
+		return left + self
 	
-	def sub(self, r: int|uint, covariance: float = 0.0) -> uint:
+	def sub(self, r: int|uint, covariance: float = 0.0) -> uint|ufloat:
 		if isinstance(r, float):
 			return self.toufloat() - ufloat(r)
 		elif isinstance(r, ufloat):
 			return self.toufloat() - r
 		elif isinstance(r, int):
 			r = uint(r)
 
@@ -70,15 +75,20 @@
 		else: 
 			return uint(self.x - r.x, math.sqrt((self.u*self.u) + (r.u**2)  - 2 * covariance))
 	
 	def __sub__(self, r: int|uint|float|ufloat):
 		return self.sub(r)
 	
 	def __rsub__(self, left) -> uint:
-		return uint(left).__sub__(self)
+		if isinstance(left, int):
+			left = uint(left)
+		elif isinstance(left, float):
+			left = ufloat(left)
+			
+		return left - self
 
 	def mul(self, r: int|uint, covariance: float = 0.0) -> uint:
 		if isinstance(r, float):
 			return self.toufloat() * ufloat(r)
 		elif isinstance(r, ufloat):
 			return self.toufloat() * r
 		elif isinstance(r, int):
@@ -90,15 +100,20 @@
 
 		return uint(self.x * r.x, math.sqrt(a + b + c))
 
 	def __mul__(self, r) -> uint:
 		return self.mul(r)
 	
 	def __rmul__(self, left) -> uint:
-		return uint(left).__mul__(self)
+		if isinstance(left, int):
+			left = uint(left)
+		elif isinstance(left, float):
+			left = ufloat(left)
+			
+		return left * self
 
 	''' self operation returns a ufloat '''
 	def __div(self, r: ufloat, covariance:float = 0.0) -> ufloat:
 		if r == self:    		# pathological cases x/x
 			return 1, 0.0
 		elif r.u == 0.0:  		# r is a scalar
 			return self.x / r.x, self.u / r.x 		# "self" may be a scalar, too
@@ -116,30 +131,40 @@
 	def div(self, r: uint|ufloat|int|float, covariance: float = 0.0) -> ufloat:
 		return self.toufloat() / (ufloat(r) if isinstance(r, (int,float)) else r.toufloat())
 
 	def __truediv__(self, r) -> uint:
 		return self.div(r, 0.0)
 	
 	def __rtruediv__(self, left) -> uint:
-		return uint(left).__truediv__(self)
+		if isinstance(left, int):
+			left = uint(left)
+		elif isinstance(left, float):
+			left = ufloat(left)
+			
+		return left / self
 		
 	def floordiv(self, r: uint|ufloat|int|float, covariance: float = 0.0) -> uint|ufloat:
 		if isinstance(r, (int, uint)):
 			x, u = self.__div(uint(r) if isinstance(r, int) else r , covariance)
 			return uint(math.floor(x), u)
 		elif isinstance(r, (float, ufloat)):
 			return self.toufloat().floordiv(ufloat(r) if isinstance(r, float) else r, covariance)
 		else:
 			raise RuntimeError("Invalid divisor")
 		
 	def __floordiv__(self, r):
 		return self.floordiv(r, 0.0)
 	
 	def __rfloordiv__(self, left):
-		return uint(left).__floordiv__(self)
+		if isinstance(left, int):
+			left = uint(left)
+		elif isinstance(left, float):
+			left = ufloat(left)
+			
+		return left // self
 
 	def mod(self, r: int|uint, covariance: float = 0.0) -> uint|ufloat:
 		if isinstance(r, int):
 			r = uint(r)
 	
 		if id(r) == id(self):  		# pathological cases x/x
 			return uint(0, 0.0)
@@ -246,15 +271,15 @@
 		return self.ge(r)
 
 	''' END OF FuZZY COMPARISON OPERATIONS '''
 
 	''' Conversions '''
 	def __str__(self) -> str:
 		return "uint({:d}, {:5.3f})".format(self.x, self.u)
-    
+	
 	def __repr__(self) -> str:
 		return "uint({:d}, {:5.3f})".format(self.x, self.u)
 
 	def toint(self) -> int:
 		return self.x
 	
 	def touint(self) -> uint:
@@ -394,15 +419,15 @@
 		else:
 			raise RuntimeError("Invalid divisor")
 
 	def __floordiv__(self, r):
 		return self.floordiv(r, 0.0)
 	
 	def __rfloordiv__(self, left):
-		return uint(left).__floordiv__(self)
+		return ufloat(left).__floordiv__(self)
 
 	def abs(self) -> ufloat:
 		return ufloat(abs(self.x), self.u)
 	
 	def __abs__(self) -> ufloat:
 		return self.abs()
 
@@ -695,10 +720,10 @@
 	
 	def copy(self) -> ufloat:
 		return ufloat(self.x, self.u)
 
 	''' Conversions '''
 	def __str__(self) -> str:
 		return "ufloat({:5.3f}, {:5.3f})".format(self.x, self.u)
-
+	
 	def __repr__(self) -> str:
-		return "ufloat({:5.3f}, {:5.3f})".format(self.x, self.u)
+		return "ufloat({:5.3f}, {:5.3f})".format(self.x, self.u)
```

### Comparing `uncertainty-datatypes-1.0.3/udatatypes/utypes.py` & `uncertainty-datatypes-1.0.4/udatatypes/utypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,19 +80,23 @@
 # inverse
 def inverse(obj: uint|ufloat) -> uint|ufloat:
     __check_obj(obj)
     return __call_func(obj, inverse.__name__)
 
 def __search(rs: Iterable, eval):
     if len(rs) == 0:
-        raise ValueError('max expected at least 1 argument, got 0')
+        raise ValueError('expected at least 1 argument, got 0')
+    if len(rs) == 1:
+        return rs[0]
     
-    best = rs[0]
+    ev = eval(rs[0], rs[1]); rev = eval(rs[1], rs[0])
+    best = rs[0] if ev.c > rev.c else rs[1]
     for r in rs:
-        if eval(r, best):
+        ev = eval(best, r); rev = eval(r, best)
+        if ev.c < rev.c:
             best = r
     
     if is_utype(best):
         return best.copy()
     else:
         best
```

