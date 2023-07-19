# Comparing `tmp/djangocms-aldryn-translation-tools-1.0.0.tar.gz` & `tmp/djangocms-aldryn-translation-tools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-aldryn-translation-tools-1.0.0.tar", last modified: Wed Jul 19 06:58:50 2023, max compression
+gzip compressed data, was "djangocms-aldryn-translation-tools-1.0.1.tar", last modified: Wed Jul 19 07:18:16 2023, max compression
```

## Comparing `djangocms-aldryn-translation-tools-1.0.0.tar` & `djangocms-aldryn-translation-tools-1.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 06:58:50.222362 djangocms-aldryn-translation-tools-1.0.0/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1475 2023-06-19 07:24:37.000000 djangocms-aldryn-translation-tools-1.0.0/LICENSE.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       97 2023-06-19 07:24:37.000000 djangocms-aldryn-translation-tools-1.0.0/MANIFEST.in
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    10103 2023-07-19 06:58:50.222362 djangocms-aldryn-translation-tools-1.0.0/PKG-INFO
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     9216 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.0/README.rst
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 06:58:50.222362 djangocms-aldryn-translation-tools-1.0.0/aldryn_translation_tools/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       22 2023-07-19 06:58:32.000000 djangocms-aldryn-translation-tools-1.0.0/aldryn_translation_tools/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     5281 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.0/aldryn_translation_tools/admin.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    10346 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.0/aldryn_translation_tools/models.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1794 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.0/aldryn_translation_tools/sitemaps.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 06:58:50.218362 djangocms-aldryn-translation-tools-1.0.0/aldryn_translation_tools/static/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 06:58:50.218362 djangocms-aldryn-translation-tools-1.0.0/aldryn_translation_tools/static/css/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 06:58:50.222362 djangocms-aldryn-translation-tools-1.0.0/aldryn_translation_tools/static/css/admin/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      591 2023-06-19 07:24:37.000000 djangocms-aldryn-translation-tools-1.0.0/aldryn_translation_tools/static/css/admin/all-translations-mixin.css
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2681 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.0/aldryn_translation_tools/utils.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 06:58:50.222362 djangocms-aldryn-translation-tools-1.0.0/djangocms_aldryn_translation_tools.egg-info/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    10103 2023-07-19 06:58:50.000000 djangocms-aldryn-translation-tools-1.0.0/djangocms_aldryn_translation_tools.egg-info/PKG-INFO
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      815 2023-07-19 06:58:50.000000 djangocms-aldryn-translation-tools-1.0.0/djangocms_aldryn_translation_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2023-07-19 06:58:50.000000 djangocms-aldryn-translation-tools-1.0.0/djangocms_aldryn_translation_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2023-07-18 11:36:27.000000 djangocms-aldryn-translation-tools-1.0.0/djangocms_aldryn_translation_tools.egg-info/not-zip-safe
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       60 2023-07-19 06:58:50.000000 djangocms-aldryn-translation-tools-1.0.0/djangocms_aldryn_translation_tools.egg-info/requires.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       36 2023-07-19 06:58:50.000000 djangocms-aldryn-translation-tools-1.0.0/djangocms_aldryn_translation_tools.egg-info/top_level.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      883 2023-07-19 06:58:50.222362 djangocms-aldryn-translation-tools-1.0.0/setup.cfg
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1335 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.0/setup.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 06:58:50.222362 djangocms-aldryn-translation-tools-1.0.0/test_addon/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       22 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.0/test_addon/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      335 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.0/test_addon/cms_apps.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      307 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.0/test_addon/managers.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2600 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.0/test_addon/models.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      823 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.0/test_addon/urls.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      546 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.0/test_addon/views.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 06:58:50.222362 djangocms-aldryn-translation-tools-1.0.0/tests/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4842 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.0/tests/test_models.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4607 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.0/tests/test_utils.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 07:18:16.321604 djangocms-aldryn-translation-tools-1.0.1/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1475 2023-06-19 07:24:37.000000 djangocms-aldryn-translation-tools-1.0.1/LICENSE.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       97 2023-06-19 07:24:37.000000 djangocms-aldryn-translation-tools-1.0.1/MANIFEST.in
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     9910 2023-07-19 07:18:16.321604 djangocms-aldryn-translation-tools-1.0.1/PKG-INFO
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     9023 2023-07-19 07:14:32.000000 djangocms-aldryn-translation-tools-1.0.1/README.rst
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 07:18:16.321604 djangocms-aldryn-translation-tools-1.0.1/aldryn_translation_tools/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       22 2023-07-19 07:17:43.000000 djangocms-aldryn-translation-tools-1.0.1/aldryn_translation_tools/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     5281 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.1/aldryn_translation_tools/admin.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    10346 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.1/aldryn_translation_tools/models.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1794 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.1/aldryn_translation_tools/sitemaps.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 07:18:16.321604 djangocms-aldryn-translation-tools-1.0.1/aldryn_translation_tools/static/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 07:18:16.321604 djangocms-aldryn-translation-tools-1.0.1/aldryn_translation_tools/static/css/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 07:18:16.321604 djangocms-aldryn-translation-tools-1.0.1/aldryn_translation_tools/static/css/admin/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      591 2023-06-19 07:24:37.000000 djangocms-aldryn-translation-tools-1.0.1/aldryn_translation_tools/static/css/admin/all-translations-mixin.css
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2681 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.1/aldryn_translation_tools/utils.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 07:18:16.321604 djangocms-aldryn-translation-tools-1.0.1/djangocms_aldryn_translation_tools.egg-info/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     9910 2023-07-19 07:18:16.000000 djangocms-aldryn-translation-tools-1.0.1/djangocms_aldryn_translation_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      815 2023-07-19 07:18:16.000000 djangocms-aldryn-translation-tools-1.0.1/djangocms_aldryn_translation_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2023-07-19 07:18:16.000000 djangocms-aldryn-translation-tools-1.0.1/djangocms_aldryn_translation_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2023-07-18 11:36:27.000000 djangocms-aldryn-translation-tools-1.0.1/djangocms_aldryn_translation_tools.egg-info/not-zip-safe
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       60 2023-07-19 07:18:16.000000 djangocms-aldryn-translation-tools-1.0.1/djangocms_aldryn_translation_tools.egg-info/requires.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       36 2023-07-19 07:18:16.000000 djangocms-aldryn-translation-tools-1.0.1/djangocms_aldryn_translation_tools.egg-info/top_level.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      883 2023-07-19 07:18:16.325604 djangocms-aldryn-translation-tools-1.0.1/setup.cfg
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1335 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.1/setup.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 07:18:16.321604 djangocms-aldryn-translation-tools-1.0.1/test_addon/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       22 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.1/test_addon/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      335 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.1/test_addon/cms_apps.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      307 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.1/test_addon/managers.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2600 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.1/test_addon/models.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      823 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.1/test_addon/urls.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      546 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.1/test_addon/views.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-19 07:18:16.321604 djangocms-aldryn-translation-tools-1.0.1/tests/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4842 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.1/tests/test_models.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4607 2023-07-19 06:52:56.000000 djangocms-aldryn-translation-tools-1.0.1/tests/test_utils.py
```

### Comparing `djangocms-aldryn-translation-tools-1.0.0/LICENSE.txt` & `djangocms-aldryn-translation-tools-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-translation-tools-1.0.0/PKG-INFO` & `djangocms-aldryn-translation-tools-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-aldryn-translation-tools
-Version: 1.0.0
+Version: 1.0.1
 Summary: Collection of helpers and mixins for translated projects.
 Home-page: https://github.com/CZ-NIC/djangocms-aldryn-translation-tools
 Author: Divio AG
 Author-email: info@divio.ch
 License: BSD License
 Platform: OS Independent
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -17,24 +17,21 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
-.. image:: https://img.shields.io/badge/Continuation-Divio_Aldryn_Search-blue
-    :target: https://github.com/divio/aldryn-search
-    :alt: Continuation of the deprecated project "Divio Aldryn search"
+|Project continuation| |Pypi package| |Pypi status| |Python versions| |License|
 
-Continuation of the deprecated project `Divio Aldryn search <https://github.com/divio/aldryn-translation-tools>`_.
 
 Aldryn Translation Tools
 ========================
 
-|Project continuation| |Pypi package| |Pypi status| |Python versions| |License|
+Continuation of the deprecated project `Divio Aldryn search <https://github.com/divio/aldryn-translation-tools>`_.
 
 A collection of shared helpers and mixins for translated django-CMS projects.
 
 To use, install it into your project using pip::
 
     pip install djangocms-aldryn-translation-tools
 
@@ -257,19 +254,19 @@
 resulting in a NoReverseFound exception or 404 and which clearly is not
 respecting the fallback preferences set by the developer.
 
 
 .. |Project continuation| image:: https://img.shields.io/badge/Continuation-Divio_Aldryn_Search-blue
     :target: https://github.com/CZ-NIC/djangocms-aldryn-translation-tools
     :alt: Continuation of the deprecated project "Divio Aldryn translation tools"
-.. |Pypi package| image:: https://img.shields.io/pypi/v/djangocms-translation-tools.svg
-    :target: https://pypi.python.org/pypi/djangocms-translation-tools/
+.. |Pypi package| image:: https://img.shields.io/pypi/v/djangocms-aldryn-translation.svg
+    :target: https://pypi.python.org/pypi/djangocms-aldryn-translation/
     :alt: Pypi package
-.. |Pypi status| image:: https://img.shields.io/pypi/status/djangocms-translation-tools.svg
-   :target: https://pypi.python.org/pypi/djangocms-translation-tools
+.. |Pypi status| image:: https://img.shields.io/pypi/status/djangocms-aldryn-translation.svg
+   :target: https://pypi.python.org/pypi/djangocms-aldryn-translation
    :alt: status
-.. |Python versions| image:: https://img.shields.io/pypi/pyversions/djangocms-translation-tools.svg
-   :target: https://pypi.python.org/pypi/djangocms-translation-tools
+.. |Python versions| image:: https://img.shields.io/pypi/pyversions/djangocms-aldryn-translation.svg
+   :target: https://pypi.python.org/pypi/djangocms-aldryn-translation
    :alt: Python versions
-.. |License| image:: https://img.shields.io/pypi/l/djangocms-translation-tools.svg
-    :target: https://pypi.python.org/pypi/djangocms-translation-tools/
+.. |License| image:: https://img.shields.io/pypi/l/djangocms-aldryn-translation.svg
+    :target: https://pypi.python.org/pypi/djangocms-aldryn-translation/
     :alt: license
```

### Comparing `djangocms-aldryn-translation-tools-1.0.0/README.rst` & `djangocms-aldryn-translation-tools-1.0.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-.. image:: https://img.shields.io/badge/Continuation-Divio_Aldryn_Search-blue
-    :target: https://github.com/divio/aldryn-search
-    :alt: Continuation of the deprecated project "Divio Aldryn search"
+|Project continuation| |Pypi package| |Pypi status| |Python versions| |License|
 
-Continuation of the deprecated project `Divio Aldryn search <https://github.com/divio/aldryn-translation-tools>`_.
 
 Aldryn Translation Tools
 ========================
 
-|Project continuation| |Pypi package| |Pypi status| |Python versions| |License|
+Continuation of the deprecated project `Divio Aldryn search <https://github.com/divio/aldryn-translation-tools>`_.
 
 A collection of shared helpers and mixins for translated django-CMS projects.
 
 To use, install it into your project using pip::
 
     pip install djangocms-aldryn-translation-tools
 
@@ -234,19 +231,19 @@
 resulting in a NoReverseFound exception or 404 and which clearly is not
 respecting the fallback preferences set by the developer.
 
 
 .. |Project continuation| image:: https://img.shields.io/badge/Continuation-Divio_Aldryn_Search-blue
     :target: https://github.com/CZ-NIC/djangocms-aldryn-translation-tools
     :alt: Continuation of the deprecated project "Divio Aldryn translation tools"
-.. |Pypi package| image:: https://img.shields.io/pypi/v/djangocms-translation-tools.svg
-    :target: https://pypi.python.org/pypi/djangocms-translation-tools/
+.. |Pypi package| image:: https://img.shields.io/pypi/v/djangocms-aldryn-translation.svg
+    :target: https://pypi.python.org/pypi/djangocms-aldryn-translation/
     :alt: Pypi package
-.. |Pypi status| image:: https://img.shields.io/pypi/status/djangocms-translation-tools.svg
-   :target: https://pypi.python.org/pypi/djangocms-translation-tools
+.. |Pypi status| image:: https://img.shields.io/pypi/status/djangocms-aldryn-translation.svg
+   :target: https://pypi.python.org/pypi/djangocms-aldryn-translation
    :alt: status
-.. |Python versions| image:: https://img.shields.io/pypi/pyversions/djangocms-translation-tools.svg
-   :target: https://pypi.python.org/pypi/djangocms-translation-tools
+.. |Python versions| image:: https://img.shields.io/pypi/pyversions/djangocms-aldryn-translation.svg
+   :target: https://pypi.python.org/pypi/djangocms-aldryn-translation
    :alt: Python versions
-.. |License| image:: https://img.shields.io/pypi/l/djangocms-translation-tools.svg
-    :target: https://pypi.python.org/pypi/djangocms-translation-tools/
+.. |License| image:: https://img.shields.io/pypi/l/djangocms-aldryn-translation.svg
+    :target: https://pypi.python.org/pypi/djangocms-aldryn-translation/
     :alt: license
```

### Comparing `djangocms-aldryn-translation-tools-1.0.0/aldryn_translation_tools/admin.py` & `djangocms-aldryn-translation-tools-1.0.1/aldryn_translation_tools/admin.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-translation-tools-1.0.0/aldryn_translation_tools/models.py` & `djangocms-aldryn-translation-tools-1.0.1/aldryn_translation_tools/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-translation-tools-1.0.0/aldryn_translation_tools/sitemaps.py` & `djangocms-aldryn-translation-tools-1.0.1/aldryn_translation_tools/sitemaps.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-translation-tools-1.0.0/aldryn_translation_tools/static/css/admin/all-translations-mixin.css` & `djangocms-aldryn-translation-tools-1.0.1/aldryn_translation_tools/static/css/admin/all-translations-mixin.css`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-translation-tools-1.0.0/aldryn_translation_tools/utils.py` & `djangocms-aldryn-translation-tools-1.0.1/aldryn_translation_tools/utils.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-translation-tools-1.0.0/djangocms_aldryn_translation_tools.egg-info/PKG-INFO` & `djangocms-aldryn-translation-tools-1.0.1/djangocms_aldryn_translation_tools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-aldryn-translation-tools
-Version: 1.0.0
+Version: 1.0.1
 Summary: Collection of helpers and mixins for translated projects.
 Home-page: https://github.com/CZ-NIC/djangocms-aldryn-translation-tools
 Author: Divio AG
 Author-email: info@divio.ch
 License: BSD License
 Platform: OS Independent
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -17,24 +17,21 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
-.. image:: https://img.shields.io/badge/Continuation-Divio_Aldryn_Search-blue
-    :target: https://github.com/divio/aldryn-search
-    :alt: Continuation of the deprecated project "Divio Aldryn search"
+|Project continuation| |Pypi package| |Pypi status| |Python versions| |License|
 
-Continuation of the deprecated project `Divio Aldryn search <https://github.com/divio/aldryn-translation-tools>`_.
 
 Aldryn Translation Tools
 ========================
 
-|Project continuation| |Pypi package| |Pypi status| |Python versions| |License|
+Continuation of the deprecated project `Divio Aldryn search <https://github.com/divio/aldryn-translation-tools>`_.
 
 A collection of shared helpers and mixins for translated django-CMS projects.
 
 To use, install it into your project using pip::
 
     pip install djangocms-aldryn-translation-tools
 
@@ -257,19 +254,19 @@
 resulting in a NoReverseFound exception or 404 and which clearly is not
 respecting the fallback preferences set by the developer.
 
 
 .. |Project continuation| image:: https://img.shields.io/badge/Continuation-Divio_Aldryn_Search-blue
     :target: https://github.com/CZ-NIC/djangocms-aldryn-translation-tools
     :alt: Continuation of the deprecated project "Divio Aldryn translation tools"
-.. |Pypi package| image:: https://img.shields.io/pypi/v/djangocms-translation-tools.svg
-    :target: https://pypi.python.org/pypi/djangocms-translation-tools/
+.. |Pypi package| image:: https://img.shields.io/pypi/v/djangocms-aldryn-translation.svg
+    :target: https://pypi.python.org/pypi/djangocms-aldryn-translation/
     :alt: Pypi package
-.. |Pypi status| image:: https://img.shields.io/pypi/status/djangocms-translation-tools.svg
-   :target: https://pypi.python.org/pypi/djangocms-translation-tools
+.. |Pypi status| image:: https://img.shields.io/pypi/status/djangocms-aldryn-translation.svg
+   :target: https://pypi.python.org/pypi/djangocms-aldryn-translation
    :alt: status
-.. |Python versions| image:: https://img.shields.io/pypi/pyversions/djangocms-translation-tools.svg
-   :target: https://pypi.python.org/pypi/djangocms-translation-tools
+.. |Python versions| image:: https://img.shields.io/pypi/pyversions/djangocms-aldryn-translation.svg
+   :target: https://pypi.python.org/pypi/djangocms-aldryn-translation
    :alt: Python versions
-.. |License| image:: https://img.shields.io/pypi/l/djangocms-translation-tools.svg
-    :target: https://pypi.python.org/pypi/djangocms-translation-tools/
+.. |License| image:: https://img.shields.io/pypi/l/djangocms-aldryn-translation.svg
+    :target: https://pypi.python.org/pypi/djangocms-aldryn-translation/
     :alt: license
```

### Comparing `djangocms-aldryn-translation-tools-1.0.0/djangocms_aldryn_translation_tools.egg-info/SOURCES.txt` & `djangocms-aldryn-translation-tools-1.0.1/djangocms_aldryn_translation_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-translation-tools-1.0.0/setup.cfg` & `djangocms-aldryn-translation-tools-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-translation-tools-1.0.0/setup.py` & `djangocms-aldryn-translation-tools-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-translation-tools-1.0.0/test_addon/models.py` & `djangocms-aldryn-translation-tools-1.0.1/test_addon/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-translation-tools-1.0.0/test_addon/urls.py` & `djangocms-aldryn-translation-tools-1.0.1/test_addon/urls.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-translation-tools-1.0.0/test_addon/views.py` & `djangocms-aldryn-translation-tools-1.0.1/test_addon/views.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-translation-tools-1.0.0/tests/test_models.py` & `djangocms-aldryn-translation-tools-1.0.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-translation-tools-1.0.0/tests/test_utils.py` & `djangocms-aldryn-translation-tools-1.0.1/tests/test_utils.py`

 * *Files identical despite different names*

