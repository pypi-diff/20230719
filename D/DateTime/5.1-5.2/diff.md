# Comparing `tmp/DateTime-5.1.tar.gz` & `tmp/DateTime-5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DateTime-5.1.tar", last modified: Tue Mar 14 16:17:56 2023, max compression
+gzip compressed data, was "DateTime-5.2.tar", last modified: Wed Jul 19 06:25:15 2023, max compression
```

## Comparing `DateTime-5.1.tar` & `DateTime-5.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-14 16:17:56.435197 DateTime-5.1/
--rw-r--r--   0 mac        (513) staff       (20)     8355 2023-03-14 16:17:55.000000 DateTime-5.1/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      805 2023-03-14 16:17:55.000000 DateTime-5.1/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2023-03-14 16:17:55.000000 DateTime-5.1/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2023-03-14 16:17:55.000000 DateTime-5.1/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      225 2023-03-14 16:17:55.000000 DateTime-5.1/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)    32782 2023-03-14 16:17:56.435377 DateTime-5.1/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      776 2023-03-14 16:17:55.000000 DateTime-5.1/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      303 2023-03-14 16:17:55.000000 DateTime-5.1/buildout.cfg
--rw-r--r--   0 mac        (513) staff       (20)      467 2023-03-14 16:17:56.436099 DateTime-5.1/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     2574 2023-03-14 16:17:55.000000 DateTime-5.1/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-14 16:17:56.426720 DateTime-5.1/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-14 16:17:56.432011 DateTime-5.1/src/DateTime/
--rw-r--r--   0 mac        (513) staff       (20)    71299 2023-03-14 16:17:55.000000 DateTime-5.1/src/DateTime/DateTime.py
--rw-r--r--   0 mac        (513) staff       (20)    22487 2023-03-14 16:17:55.000000 DateTime-5.1/src/DateTime/DateTime.txt
--rw-r--r--   0 mac        (513) staff       (20)      714 2023-03-14 16:17:55.000000 DateTime-5.1/src/DateTime/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)    12256 2023-03-14 16:17:55.000000 DateTime-5.1/src/DateTime/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)     5618 2023-03-14 16:17:55.000000 DateTime-5.1/src/DateTime/pytz.txt
--rw-r--r--   0 mac        (513) staff       (20)    11788 2023-03-14 16:17:55.000000 DateTime-5.1/src/DateTime/pytz_support.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-14 16:17:56.434890 DateTime-5.1/src/DateTime/tests/
--rw-r--r--   0 mac        (513) staff       (20)      683 2023-03-14 16:17:55.000000 DateTime-5.1/src/DateTime/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     1397 2023-03-14 16:17:55.000000 DateTime-5.1/src/DateTime/tests/julian_testdata.txt
--rw-r--r--   0 mac        (513) staff       (20)    27651 2023-03-14 16:17:55.000000 DateTime-5.1/src/DateTime/tests/test_datetime.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-14 16:17:56.433967 DateTime-5.1/src/DateTime.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)    32782 2023-03-14 16:17:56.000000 DateTime-5.1/src/DateTime.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      590 2023-03-14 16:17:56.000000 DateTime-5.1/src/DateTime.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-03-14 16:17:56.000000 DateTime-5.1/src/DateTime.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-03-14 16:17:56.000000 DateTime-5.1/src/DateTime.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)       20 2023-03-14 16:17:56.000000 DateTime-5.1/src/DateTime.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        9 2023-03-14 16:17:56.000000 DateTime-5.1/src/DateTime.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1680 2023-03-14 16:17:55.000000 DateTime-5.1/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:25:15.163924 DateTime-5.2/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8557 2023-07-19 06:25:14.000000 DateTime-5.2/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      805 2023-07-19 06:25:14.000000 DateTime-5.2/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-19 06:25:14.000000 DateTime-5.2/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-07-19 06:25:14.000000 DateTime-5.2/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      225 2023-07-19 06:25:14.000000 DateTime-5.2/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)    32984 2023-07-19 06:25:15.164005 DateTime-5.2/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      776 2023-07-19 06:25:14.000000 DateTime-5.2/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      303 2023-07-19 06:25:14.000000 DateTime-5.2/buildout.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)      467 2023-07-19 06:25:15.164251 DateTime-5.2/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2574 2023-07-19 06:25:14.000000 DateTime-5.2/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:25:15.160067 DateTime-5.2/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:25:15.162476 DateTime-5.2/src/DateTime/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    71034 2023-07-19 06:25:14.000000 DateTime-5.2/src/DateTime/DateTime.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    22487 2023-07-19 06:25:14.000000 DateTime-5.2/src/DateTime/DateTime.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      714 2023-07-19 06:25:14.000000 DateTime-5.2/src/DateTime/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    12256 2023-07-19 06:25:14.000000 DateTime-5.2/src/DateTime/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5618 2023-07-19 06:25:14.000000 DateTime-5.2/src/DateTime/pytz.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11788 2023-07-19 06:25:14.000000 DateTime-5.2/src/DateTime/pytz_support.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:25:15.163771 DateTime-5.2/src/DateTime/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      683 2023-07-19 06:25:14.000000 DateTime-5.2/src/DateTime/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1397 2023-07-19 06:25:14.000000 DateTime-5.2/src/DateTime/tests/julian_testdata.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)    28398 2023-07-19 06:25:14.000000 DateTime-5.2/src/DateTime/tests/test_datetime.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:25:15.163356 DateTime-5.2/src/DateTime.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    32984 2023-07-19 06:25:15.000000 DateTime-5.2/src/DateTime.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      590 2023-07-19 06:25:15.000000 DateTime-5.2/src/DateTime.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-19 06:25:15.000000 DateTime-5.2/src/DateTime.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-19 06:25:15.000000 DateTime-5.2/src/DateTime.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)       20 2023-07-19 06:25:15.000000 DateTime-5.2/src/DateTime.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        9 2023-07-19 06:25:15.000000 DateTime-5.2/src/DateTime.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1680 2023-07-19 06:25:14.000000 DateTime-5.2/tox.ini
```

### Comparing `DateTime-5.1/CHANGES.rst` & `DateTime-5.2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+5.2 (2023-07-19)
+----------------
+
+- Cast int to float in compare methods.
+- Fix compare methods between DateTime instances and None.
+  (`#52 <https://github.com/zopefoundation/DateTime/issues/52>`_)
+
+
 5.1 (2023-03-14)
 ----------------
 
 - Add missing ``python_requires`` to ``setup.py``.
 
 
 5.0 (2023-01-12)
```

### Comparing `DateTime-5.1/CONTRIBUTING.md` & `DateTime-5.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `DateTime-5.1/LICENSE.txt` & `DateTime-5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DateTime-5.1/PKG-INFO` & `DateTime-5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DateTime
-Version: 5.1
+Version: 5.2
 Summary: This package provides a DateTime data type, as known from Zope. Unless you need to communicate with Zope APIs, you're probably better off using Python's built-in datetime module.
 Home-page: https://github.com/zopefoundation/DateTime
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Web Environment
@@ -835,14 +835,22 @@
   >>> float(dt)
   857933100.0
 
 
 Changelog
 =========
 
+5.2 (2023-07-19)
+----------------
+
+- Cast int to float in compare methods.
+- Fix compare methods between DateTime instances and None.
+  (`#52 <https://github.com/zopefoundation/DateTime/issues/52>`_)
+
+
 5.1 (2023-03-14)
 ----------------
 
 - Add missing ``python_requires`` to ``setup.py``.
 
 
 5.0 (2023-01-12)
```

### Comparing `DateTime-5.1/README.rst` & `DateTime-5.2/README.rst`

 * *Files identical despite different names*

### Comparing `DateTime-5.1/setup.py` & `DateTime-5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 with open(os.path.join(here, 'README.rst')) as f:
     HEADER = f.read()
 with open(os.path.join(here, 'src', 'DateTime', 'DateTime.txt')) as f:
     README = f.read()
 with open(os.path.join(here, 'CHANGES.rst')) as f:
     CHANGES = f.read()
 
-version = '5.1'
+version = '5.2'
 
 setup(
     name='DateTime',
     version=version,
     url='https://github.com/zopefoundation/DateTime',
     license='ZPL 2.1',
     description="""\
```

### Comparing `DateTime-5.1/src/DateTime/DateTime.py` & `DateTime-5.2/src/DateTime/DateTime.py`

 * *Files 1% similar despite different names*

```diff
@@ -1244,21 +1244,19 @@
         Returns true if the object represents a date/time greater
         than the specified DateTime or time module style time.
 
         Revised to give more correct results through comparison of
         long integer microseconds.
         """
         if t is None:
-            t = 0
-        if isinstance(t, float):
+            return True
+        if isinstance(t, (float, int)):
             return self._micros > long(t * 1000000)
-        try:
+        else:
             return self._micros > t._micros
-        except AttributeError:
-            return self._micros > t
 
     __gt__ = greaterThan
 
     def greaterThanEqualTo(self, t):
         """Compare this DateTime object to another DateTime object
         OR a floating point number such as that which is returned
         by the python time module.
@@ -1267,21 +1265,19 @@
         than or equal to the specified DateTime or time module style
         time.
 
         Revised to give more correct results through comparison of
         long integer microseconds.
         """
         if t is None:
-            t = 0
-        if isinstance(t, float):
+            return True
+        if isinstance(t, (float, int)):
             return self._micros >= long(t * 1000000)
-        try:
+        else:
             return self._micros >= t._micros
-        except AttributeError:
-            return self._micros >= t
 
     __ge__ = greaterThanEqualTo
 
     def equalTo(self, t):
         """Compare this DateTime object to another DateTime object
         OR a floating point number such as that which is returned
         by the python time module.
@@ -1289,21 +1285,19 @@
         Returns true if the object represents a date/time equal to
         the specified DateTime or time module style time.
 
         Revised to give more correct results through comparison of
         long integer microseconds.
         """
         if t is None:
-            t = 0
-        if isinstance(t, float):
+            return False
+        if isinstance(t, (float, int)):
             return self._micros == long(t * 1000000)
-        try:
+        else:
             return self._micros == t._micros
-        except AttributeError:
-            return self._micros == t
 
     def notEqualTo(self, t):
         """Compare this DateTime object to another DateTime object
         OR a floating point number such as that which is returned
         by the python time module.
 
         Returns true if the object represents a date/time not equal
@@ -1336,21 +1330,19 @@
         Returns true if the object represents a date/time less than
         the specified DateTime or time module style time.
 
         Revised to give more correct results through comparison of
         long integer microseconds.
         """
         if t is None:
-            t = 0
-        if isinstance(t, float):
+            return False
+        if isinstance(t, (float, int)):
             return self._micros < long(t * 1000000)
-        try:
+        else:
             return self._micros < t._micros
-        except AttributeError:
-            return self._micros < t
 
     __lt__ = lessThan
 
     def lessThanEqualTo(self, t):
         """Compare this DateTime object to another DateTime object
         OR a floating point number such as that which is returned
         by the python time module.
@@ -1358,21 +1350,19 @@
         Returns true if the object represents a date/time less than
         or equal to the specified DateTime or time module style time.
 
         Revised to give more correct results through comparison of
         long integer microseconds.
         """
         if t is None:
-            t = 0
-        if isinstance(t, float):
+            return False
+        if isinstance(t, (float, int)):
             return self._micros <= long(t * 1000000)
-        try:
+        else:
             return self._micros <= t._micros
-        except AttributeError:
-            return self._micros <= t
 
     __le__ = lessThanEqualTo
 
     def isLeapYear(self):
         """Return true if the current year (in the context of the
         object\'s timezone) is a leap year.
         """
```

### Comparing `DateTime-5.1/src/DateTime/DateTime.txt` & `DateTime-5.2/src/DateTime/DateTime.txt`

 * *Files identical despite different names*

### Comparing `DateTime-5.1/src/DateTime/__init__.py` & `DateTime-5.2/src/DateTime/__init__.py`

 * *Files identical despite different names*

### Comparing `DateTime-5.1/src/DateTime/interfaces.py` & `DateTime-5.2/src/DateTime/interfaces.py`

 * *Files identical despite different names*

### Comparing `DateTime-5.1/src/DateTime/pytz.txt` & `DateTime-5.2/src/DateTime/pytz.txt`

 * *Files identical despite different names*

### Comparing `DateTime-5.1/src/DateTime/pytz_support.py` & `DateTime-5.2/src/DateTime/pytz_support.py`

 * *Files identical despite different names*

### Comparing `DateTime-5.1/src/DateTime/tests/__init__.py` & `DateTime-5.2/src/DateTime/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `DateTime-5.1/src/DateTime/tests/julian_testdata.txt` & `DateTime-5.2/src/DateTime/tests/julian_testdata.txt`

 * *Files identical despite different names*

### Comparing `DateTime-5.1/src/DateTime/tests/test_datetime.py` & `DateTime-5.2/src/DateTime/tests/test_datetime.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,24 +213,41 @@
         dt1 = DateTime('1997/2/2')
         self.assertTrue(dt1.greaterThan(dt))
         self.assertTrue(dt1.greaterThanEqualTo(dt))
         self.assertTrue(dt.lessThan(dt1))
         self.assertTrue(dt.lessThanEqualTo(dt1))
         self.assertTrue(dt.notEqualTo(dt1))
         self.assertFalse(dt.equalTo(dt1))
+        # Compare a date to float
+        dt = DateTime(1.0)
+        self.assertFalse(dt.greaterThan(1.0))
+        self.assertTrue(dt.greaterThanEqualTo(1.0))
+        self.assertFalse(dt.lessThan(1.0))
+        self.assertTrue(dt.lessThanEqualTo(1.0))
+        self.assertFalse(dt.notEqualTo(1.0))
+        self.assertTrue(dt.equalTo(1.0))
+        # Compare a date to int
+        dt = DateTime(1)
+        self.assertEqual(dt, DateTime(1.0))
+        self.assertFalse(dt.greaterThan(1))
+        self.assertTrue(dt.greaterThanEqualTo(1))
+        self.assertFalse(dt.lessThan(1))
+        self.assertTrue(dt.lessThanEqualTo(1))
+        self.assertFalse(dt.notEqualTo(1))
+        self.assertTrue(dt.equalTo(1))
 
     def test_compare_methods_none(self):
         # Compare a date to None
-        dt = DateTime('1997/1/1')
-        self.assertTrue(dt.greaterThan(None))
-        self.assertTrue(dt.greaterThanEqualTo(None))
-        self.assertFalse(dt.lessThan(None))
-        self.assertFalse(dt.lessThanEqualTo(None))
-        self.assertTrue(dt.notEqualTo(None))
-        self.assertFalse(dt.equalTo(None))
+        for dt in (DateTime('1997/1/1'), DateTime(0)):
+            self.assertTrue(dt.greaterThan(None))
+            self.assertTrue(dt.greaterThanEqualTo(None))
+            self.assertFalse(dt.lessThan(None))
+            self.assertFalse(dt.lessThanEqualTo(None))
+            self.assertTrue(dt.notEqualTo(None))
+            self.assertFalse(dt.equalTo(None))
 
     def test_pickle(self):
         dt = DateTime()
         data = pickle.dumps(dt, 1)
         new = pickle.loads(data)
         for key in DateTime.__slots__:
             self.assertEqual(getattr(dt, key), getattr(new, key))
```

### Comparing `DateTime-5.1/src/DateTime.egg-info/PKG-INFO` & `DateTime-5.2/src/DateTime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DateTime
-Version: 5.1
+Version: 5.2
 Summary: This package provides a DateTime data type, as known from Zope. Unless you need to communicate with Zope APIs, you're probably better off using Python's built-in datetime module.
 Home-page: https://github.com/zopefoundation/DateTime
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Web Environment
@@ -835,14 +835,22 @@
   >>> float(dt)
   857933100.0
 
 
 Changelog
 =========
 
+5.2 (2023-07-19)
+----------------
+
+- Cast int to float in compare methods.
+- Fix compare methods between DateTime instances and None.
+  (`#52 <https://github.com/zopefoundation/DateTime/issues/52>`_)
+
+
 5.1 (2023-03-14)
 ----------------
 
 - Add missing ``python_requires`` to ``setup.py``.
 
 
 5.0 (2023-01-12)
```

### Comparing `DateTime-5.1/src/DateTime.egg-info/SOURCES.txt` & `DateTime-5.2/src/DateTime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DateTime-5.1/tox.ini` & `DateTime-5.2/tox.ini`

 * *Files identical despite different names*

