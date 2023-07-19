# Comparing `tmp/jsonmerge-1.9.1.tar.gz` & `tmp/jsonmerge-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jsonmerge-1.9.1.tar", last modified: Thu Jul 13 09:37:37 2023, max compression
+gzip compressed data, was "dist/jsonmerge-1.9.2.tar", last modified: Wed Jul 19 08:07:48 2023, max compression
```

## Comparing `jsonmerge-1.9.1.tar` & `jsonmerge-1.9.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-sr-x   0 avian     (1000) avian     (1000)        0 2023-07-13 09:37:37.000000 jsonmerge-1.9.1/
--rw-r--r--   0 avian     (1000) avian     (1000)     4037 2023-07-13 09:32:02.000000 jsonmerge-1.9.1/ChangeLog
--rw-r--r--   0 avian     (1000) avian     (1000)     1098 2022-10-22 14:31:04.000000 jsonmerge-1.9.1/LICENSE
--rw-r--r--   0 avian     (1000) avian     (1000)       82 2018-01-31 17:33:19.000000 jsonmerge-1.9.1/MANIFEST.in
--rw-r--r--   0 avian     (1000) avian     (1000)    26190 2023-07-13 09:37:37.000000 jsonmerge-1.9.1/PKG-INFO
--rw-r--r--   0 avian     (1000) avian     (1000)    21373 2022-11-21 14:40:26.000000 jsonmerge-1.9.1/README.rst
-drwxr-sr-x   0 avian     (1000) avian     (1000)        0 2023-07-13 09:37:37.000000 jsonmerge-1.9.1/jsonmerge/
--rw-r--r--   0 avian     (1000) avian     (1000)    13486 2022-11-21 14:40:26.000000 jsonmerge-1.9.1/jsonmerge/__init__.py
--rw-r--r--   0 avian     (1000) avian     (1000)     4217 2022-11-21 14:40:26.000000 jsonmerge-1.9.1/jsonmerge/descenders.py
--rw-r--r--   0 avian     (1000) avian     (1000)      566 2019-07-19 14:32:45.000000 jsonmerge-1.9.1/jsonmerge/exceptions.py
--rw-r--r--   0 avian     (1000) avian     (1000)     2012 2022-10-22 15:10:14.000000 jsonmerge-1.9.1/jsonmerge/jsonvalue.py
--rw-r--r--   0 avian     (1000) avian     (1000)      810 2022-10-22 14:31:04.000000 jsonmerge-1.9.1/jsonmerge/resolver.py
--rw-r--r--   0 avian     (1000) avian     (1000)    12662 2022-10-22 15:58:03.000000 jsonmerge-1.9.1/jsonmerge/strategies.py
-drwxr-sr-x   0 avian     (1000) avian     (1000)        0 2023-07-13 09:37:37.000000 jsonmerge-1.9.1/jsonmerge.egg-info/
--rw-r--r--   0 avian     (1000) avian     (1000)    26190 2023-07-13 09:37:36.000000 jsonmerge-1.9.1/jsonmerge.egg-info/PKG-INFO
--rw-r--r--   0 avian     (1000) avian     (1000)      439 2023-07-13 09:37:37.000000 jsonmerge-1.9.1/jsonmerge.egg-info/SOURCES.txt
--rw-r--r--   0 avian     (1000) avian     (1000)        1 2023-07-13 09:37:36.000000 jsonmerge-1.9.1/jsonmerge.egg-info/dependency_links.txt
--rw-r--r--   0 avian     (1000) avian     (1000)       26 2023-07-13 09:37:36.000000 jsonmerge-1.9.1/jsonmerge.egg-info/requires.txt
--rw-r--r--   0 avian     (1000) avian     (1000)       10 2023-07-13 09:37:36.000000 jsonmerge-1.9.1/jsonmerge.egg-info/top_level.txt
--rw-r--r--   0 avian     (1000) avian     (1000)       38 2023-07-13 09:37:37.000000 jsonmerge-1.9.1/setup.cfg
--rw-r--r--   0 avian     (1000) avian     (1000)      693 2023-07-13 09:32:06.000000 jsonmerge-1.9.1/setup.py
-drwxr-sr-x   0 avian     (1000) avian     (1000)        0 2023-07-13 09:37:37.000000 jsonmerge-1.9.1/tests/
--rw-r--r--   0 avian     (1000) avian     (1000)        0 2018-01-31 17:33:19.000000 jsonmerge-1.9.1/tests/__init__.py
--rw-r--r--   0 avian     (1000) avian     (1000)    72698 2022-11-21 14:40:26.000000 jsonmerge-1.9.1/tests/test_jsonmerge.py
--rw-r--r--   0 avian     (1000) avian     (1000)     2652 2022-10-22 15:09:10.000000 jsonmerge-1.9.1/tests/test_jsonvalue.py
--rw-r--r--   0 avian     (1000) avian     (1000)      131 2020-09-24 17:13:51.000000 jsonmerge-1.9.1/tests/test_readme.py
+drwxr-sr-x   0 avian     (1000) avian     (1000)        0 2023-07-19 08:07:48.000000 jsonmerge-1.9.2/
+-rw-r--r--   0 avian     (1000) avian     (1000)     4111 2023-07-19 07:53:44.000000 jsonmerge-1.9.2/ChangeLog
+-rw-r--r--   0 avian     (1000) avian     (1000)     1098 2023-07-18 15:13:37.000000 jsonmerge-1.9.2/LICENSE
+-rw-r--r--   0 avian     (1000) avian     (1000)       82 2018-01-31 17:33:19.000000 jsonmerge-1.9.2/MANIFEST.in
+-rw-r--r--   0 avian     (1000) avian     (1000)    26190 2023-07-19 08:07:48.000000 jsonmerge-1.9.2/PKG-INFO
+-rw-r--r--   0 avian     (1000) avian     (1000)    21373 2023-07-18 15:13:37.000000 jsonmerge-1.9.2/README.rst
+drwxr-sr-x   0 avian     (1000) avian     (1000)        0 2023-07-19 08:07:48.000000 jsonmerge-1.9.2/jsonmerge/
+-rw-r--r--   0 avian     (1000) avian     (1000)    13486 2023-07-17 18:02:45.000000 jsonmerge-1.9.2/jsonmerge/__init__.py
+-rw-r--r--   0 avian     (1000) avian     (1000)     4217 2022-11-21 14:40:26.000000 jsonmerge-1.9.2/jsonmerge/descenders.py
+-rw-r--r--   0 avian     (1000) avian     (1000)      566 2019-07-19 14:32:45.000000 jsonmerge-1.9.2/jsonmerge/exceptions.py
+-rw-r--r--   0 avian     (1000) avian     (1000)     2012 2022-10-22 15:10:14.000000 jsonmerge-1.9.2/jsonmerge/jsonvalue.py
+-rw-r--r--   0 avian     (1000) avian     (1000)      810 2023-07-17 17:59:43.000000 jsonmerge-1.9.2/jsonmerge/resolver.py
+-rw-r--r--   0 avian     (1000) avian     (1000)    12662 2022-10-22 15:58:03.000000 jsonmerge-1.9.2/jsonmerge/strategies.py
+drwxr-sr-x   0 avian     (1000) avian     (1000)        0 2023-07-19 08:07:48.000000 jsonmerge-1.9.2/jsonmerge.egg-info/
+-rw-r--r--   0 avian     (1000) avian     (1000)    26190 2023-07-19 08:07:47.000000 jsonmerge-1.9.2/jsonmerge.egg-info/PKG-INFO
+-rw-r--r--   0 avian     (1000) avian     (1000)      439 2023-07-19 08:07:48.000000 jsonmerge-1.9.2/jsonmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 avian     (1000) avian     (1000)        1 2023-07-19 08:07:48.000000 jsonmerge-1.9.2/jsonmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 avian     (1000) avian     (1000)       17 2023-07-19 08:07:48.000000 jsonmerge-1.9.2/jsonmerge.egg-info/requires.txt
+-rw-r--r--   0 avian     (1000) avian     (1000)       10 2023-07-19 08:07:48.000000 jsonmerge-1.9.2/jsonmerge.egg-info/top_level.txt
+-rw-r--r--   0 avian     (1000) avian     (1000)       38 2023-07-19 08:07:48.000000 jsonmerge-1.9.2/setup.cfg
+-rw-r--r--   0 avian     (1000) avian     (1000)      684 2023-07-19 07:54:40.000000 jsonmerge-1.9.2/setup.py
+drwxr-sr-x   0 avian     (1000) avian     (1000)        0 2023-07-19 08:07:48.000000 jsonmerge-1.9.2/tests/
+-rw-r--r--   0 avian     (1000) avian     (1000)        0 2018-01-31 17:33:19.000000 jsonmerge-1.9.2/tests/__init__.py
+-rw-r--r--   0 avian     (1000) avian     (1000)    72703 2023-07-15 19:58:53.000000 jsonmerge-1.9.2/tests/test_jsonmerge.py
+-rw-r--r--   0 avian     (1000) avian     (1000)     2652 2022-10-22 15:09:10.000000 jsonmerge-1.9.2/tests/test_jsonvalue.py
+-rw-r--r--   0 avian     (1000) avian     (1000)      131 2020-09-24 17:13:51.000000 jsonmerge-1.9.2/tests/test_readme.py
```

### Comparing `jsonmerge-1.9.1/ChangeLog` & `jsonmerge-1.9.2/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-07-19	jsonmerge	1.9.2
+	* Fix failing tests with jsonschema>=4.18.0.
+
 2023-07-13	jsonmerge	1.9.1
 	* Require jsonschema 4.17.3 or earlier since some tests currently fail
 	  with 4.18.0 and later releases.
 
 2022-11-02	jsonmerge	1.9.0
 
 	* Add sortByRef and sortReverse options for the append and
```

### Comparing `jsonmerge-1.9.1/LICENSE` & `jsonmerge-1.9.2/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2022, Tomaz Solc <tomaz.solc@tablix.org>
+Copyright 2023, Tomaz Solc <tomaz.solc@tablix.org>
 
 The MIT License (MIT)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `jsonmerge-1.9.1/PKG-INFO` & `jsonmerge-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: jsonmerge
-Version: 1.9.1
+Version: 1.9.2
 Summary: Merge a series of JSON documents.
 Home-page: UNKNOWN
 Author: Tomaz Solc
 Author-email: tomaz.solc@tablix.org
 License: MIT
 Description: Merge a series of JSON documents
         ================================
@@ -517,15 +517,15 @@
         * Passes all existing tests and includes new tests that cover added code.
         * Updates *README.rst* to document added functionality.
         
         
         License
         -------
         
-        Copyright 2022, Tomaz Solc <tomaz.solc@tablix.org>
+        Copyright 2023, Tomaz Solc <tomaz.solc@tablix.org>
         
         The MIT License (MIT)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `jsonmerge-1.9.1/README.rst` & `jsonmerge-1.9.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -509,15 +509,15 @@
 * Passes all existing tests and includes new tests that cover added code.
 * Updates *README.rst* to document added functionality.
 
 
 License
 -------
 
-Copyright 2022, Tomaz Solc <tomaz.solc@tablix.org>
+Copyright 2023, Tomaz Solc <tomaz.solc@tablix.org>
 
 The MIT License (MIT)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `jsonmerge-1.9.1/jsonmerge/__init__.py` & `jsonmerge-1.9.2/jsonmerge/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonmerge-1.9.1/jsonmerge/descenders.py` & `jsonmerge-1.9.2/jsonmerge/descenders.py`

 * *Files identical despite different names*

### Comparing `jsonmerge-1.9.1/jsonmerge/exceptions.py` & `jsonmerge-1.9.2/jsonmerge/exceptions.py`

 * *Files identical despite different names*

### Comparing `jsonmerge-1.9.1/jsonmerge/jsonvalue.py` & `jsonmerge-1.9.2/jsonmerge/jsonvalue.py`

 * *Files identical despite different names*

### Comparing `jsonmerge-1.9.1/jsonmerge/resolver.py` & `jsonmerge-1.9.2/jsonmerge/resolver.py`

 * *Files identical despite different names*

### Comparing `jsonmerge-1.9.1/jsonmerge/strategies.py` & `jsonmerge-1.9.2/jsonmerge/strategies.py`

 * *Files identical despite different names*

### Comparing `jsonmerge-1.9.1/jsonmerge.egg-info/PKG-INFO` & `jsonmerge-1.9.2/jsonmerge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: jsonmerge
-Version: 1.9.1
+Version: 1.9.2
 Summary: Merge a series of JSON documents.
 Home-page: UNKNOWN
 Author: Tomaz Solc
 Author-email: tomaz.solc@tablix.org
 License: MIT
 Description: Merge a series of JSON documents
         ================================
@@ -517,15 +517,15 @@
         * Passes all existing tests and includes new tests that cover added code.
         * Updates *README.rst* to document added functionality.
         
         
         License
         -------
         
-        Copyright 2022, Tomaz Solc <tomaz.solc@tablix.org>
+        Copyright 2023, Tomaz Solc <tomaz.solc@tablix.org>
         
         The MIT License (MIT)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `jsonmerge-1.9.1/setup.py` & `jsonmerge-1.9.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/python
 # vim:ts=4 sw=4 expandtab softtabstop=4
 
 from setuptools import setup
 
 setup(name='jsonmerge',
-    version='1.9.1',
+    version='1.9.2',
     description='Merge a series of JSON documents.',
     license='MIT',
     long_description=open("README.rst").read(),
     author='Tomaz Solc',
     author_email='tomaz.solc@tablix.org',
     packages = [ 'jsonmerge' ],
-    install_requires = [ 'jsonschema>2.4.0,<=4.17.3' ],
+    install_requires = [ 'jsonschema>2.4.0' ],
     test_suite = 'tests',
     classifiers = [
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
         "Intended Audience :: Developers",
```

### Comparing `jsonmerge-1.9.1/tests/test_jsonmerge.py` & `jsonmerge-1.9.2/tests/test_jsonmerge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # vim:ts=4 sw=4 expandtab softtabstop=4
 import unittest
 import warnings
+import sys
 
 from collections import OrderedDict
 import jsonmerge
 import jsonmerge.strategies
 from jsonmerge.exceptions import (
     HeadInstanceError,
     BaseInstanceError,
@@ -87,24 +88,22 @@
 
         schema = {'mergeStrategy': 'version'}
         merger = jsonmerge.Merger(schema)
 
         with self.assertRaises(SchemaError) as cm:
             merger.merge(None, "a", merge_options={'version': {'metadata': 'foo'}})
 
+    @unittest.skipIf(sys.version_info < (3,2), "not supported on Python <3.2")
     def test_version_meta_deprecated(self):
         schema = {'mergeStrategy': 'version'}
         merger = jsonmerge.Merger(schema)
 
-        with warnings.catch_warnings(record=True) as w:
+        with self.assertWarnsRegex(DeprecationWarning, r"'meta' argument is deprecated"):
             base = merger.merge(None, 'a', meta={'foo': 'bar'})
 
-            self.assertEqual(len(w), 1)
-            self.assertTrue(issubclass(w[0].category, DeprecationWarning))
-
     def test_version_ignoredups_false(self):
 
         schema = {'mergeStrategy': 'version',
                   'mergeOptions': {'ignoreDups': False}}
 
         merger = jsonmerge.Merger(schema)
 
@@ -1800,24 +1799,22 @@
                                      'value': {'type': 'object'},
                                      'date': {},
                                      'version': {}
                                  }
                              }
                          })
 
+    @unittest.skipIf(sys.version_info < (3,2), "not supported on Python <3.2")
     def test_version_meta_deprecated(self):
         schema = {'mergeStrategy': 'version'}
         merger = jsonmerge.Merger(schema)
 
-        with warnings.catch_warnings(record=True) as w:
+        with self.assertWarnsRegex(DeprecationWarning, r"'meta' argument is deprecated"):
             merger.get_schema(meta={'foo': 'bar'})
 
-            self.assertEqual(len(w), 1)
-            self.assertTrue(issubclass(w[0].category, DeprecationWarning))
-
     def test_version_meta_in_schema(self):
         schema = {
                 'type': 'object',
                 'mergeStrategy': 'version',
                 'mergeOptions': {
                     'metadataSchema': {
                         'properties': {
```

### Comparing `jsonmerge-1.9.1/tests/test_jsonvalue.py` & `jsonmerge-1.9.2/tests/test_jsonvalue.py`

 * *Files identical despite different names*

