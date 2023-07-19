# Comparing `tmp/pydoclint-0.1.0.tar.gz` & `tmp/pydoclint-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoclint-0.1.0.tar", last modified: Sun Jul 16 00:19:47 2023, max compression
+gzip compressed data, was "pydoclint-0.1.1.tar", last modified: Wed Jul 19 02:27:17 2023, max compression
```

## Comparing `pydoclint-0.1.0.tar` & `pydoclint-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 00:19:47.940734 pydoclint-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-16 00:19:32.000000 pydoclint-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-07-16 00:19:47.940734 pydoclint-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12893 2023-07-16 00:19:32.000000 pydoclint-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 00:19:47.940734 pydoclint-0.1.0/pydoclint/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/flake8_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10517 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/parse_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 00:19:47.940734 pydoclint-0.1.0/pydoclint/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/astTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/internal_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/method_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/return_anno.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/return_arg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/return_yield_raise.py
--rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/unparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/violation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/utils/walk.py
--rw-r--r--   0 runner    (1001) docker     (123)    23893 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pydoclint/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 00:19:47.940734 pydoclint-0.1.0/pydoclint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-07-16 00:19:47.000000 pydoclint-0.1.0/pydoclint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-16 00:19:47.000000 pydoclint-0.1.0/pydoclint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 00:19:47.000000 pydoclint-0.1.0/pydoclint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-16 00:19:47.000000 pydoclint-0.1.0/pydoclint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-16 00:19:47.000000 pydoclint-0.1.0/pydoclint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-16 00:19:47.000000 pydoclint-0.1.0/pydoclint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-16 00:19:32.000000 pydoclint-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-16 00:19:47.940734 pydoclint-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-16 00:19:32.000000 pydoclint-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 00:19:47.940734 pydoclint-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-16 00:19:32.000000 pydoclint-0.1.0/tests/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    40155 2023-07-16 00:19:32.000000 pydoclint-0.1.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-16 00:19:32.000000 pydoclint-0.1.0/tests/test_parse_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:27:17.775635 pydoclint-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-19 02:27:07.000000 pydoclint-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13276 2023-07-19 02:27:17.775635 pydoclint-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-07-19 02:27:07.000000 pydoclint-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:27:17.767635 pydoclint-0.1.1/pydoclint/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/flake8_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/parse_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:27:17.775635 pydoclint-0.1.1/pydoclint/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/astTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/internal_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/method_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/return_anno.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/return_arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/return_yield_raise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/unparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/violation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/utils/walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23893 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pydoclint/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:27:17.771635 pydoclint-0.1.1/pydoclint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13276 2023-07-19 02:27:17.000000 pydoclint-0.1.1/pydoclint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-19 02:27:17.000000 pydoclint-0.1.1/pydoclint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 02:27:17.000000 pydoclint-0.1.1/pydoclint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-19 02:27:17.000000 pydoclint-0.1.1/pydoclint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-19 02:27:17.000000 pydoclint-0.1.1/pydoclint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 02:27:17.000000 pydoclint-0.1.1/pydoclint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-19 02:27:07.000000 pydoclint-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-19 02:27:17.775635 pydoclint-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-19 02:27:07.000000 pydoclint-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:27:17.775635 pydoclint-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-19 02:27:07.000000 pydoclint-0.1.1/tests/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40155 2023-07-19 02:27:07.000000 pydoclint-0.1.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-19 02:27:07.000000 pydoclint-0.1.1/tests/test_parse_config.py
```

### Comparing `pydoclint-0.1.0/LICENSE` & `pydoclint-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.0/PKG-INFO` & `pydoclint-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoclint
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python docstring linter that checks arguments, returns, yields, and raises sections
 Home-page: https://github.com/jsh9/pydoclint
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
@@ -23,23 +23,21 @@
 Here is a comparison of linting time on some famous Python projects:
 
 |                                                              | pydoclint | darglint                          |
 | ------------------------------------------------------------ | --------- | --------------------------------- |
 | [numpy](https://github.com/numpy/numpy)                      | 2.0 sec   | 49 min 9 sec (1,475x slower)      |
 | [scikit-learn](https://github.com/scikit-learn/scikit-learn) | 2.4 sec   | 3 hr 5 min 33 sec (4,639x slower) |
 
-Currently, _pydoclint_ supports two docstring styles:
+Currently, _pydoclint_ supports three docstring styles:
 
 - The [numpy stlyle](https://numpydoc.readthedocs.io/en/latest/format.html)
 - The
   [Google style](https://www.sphinx-doc.org/en/master/usage/extensions/example_google.html)
-
-Support for the
-[Sphinx style](https://sphinx-rtd-tutorial.readthedocs.io/en/latest/docstrings.html)
-may be added in the future if there are requests for it.
+- The
+  [Sphinx style](https://sphinx-rtd-tutorial.readthedocs.io/en/latest/docstrings.html)
 
 Another note: this linter and [pydocstyle](https://github.com/PyCQA/pydocstyle)
 serves complementary purposes. It is recommended that you use both together.
 
 ## 1. Installation
 
 ```
```

### Comparing `pydoclint-0.1.0/README.md` & `pydoclint-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,23 +10,21 @@
 Here is a comparison of linting time on some famous Python projects:
 
 |                                                              | pydoclint | darglint                          |
 | ------------------------------------------------------------ | --------- | --------------------------------- |
 | [numpy](https://github.com/numpy/numpy)                      | 2.0 sec   | 49 min 9 sec (1,475x slower)      |
 | [scikit-learn](https://github.com/scikit-learn/scikit-learn) | 2.4 sec   | 3 hr 5 min 33 sec (4,639x slower) |
 
-Currently, _pydoclint_ supports two docstring styles:
+Currently, _pydoclint_ supports three docstring styles:
 
 - The [numpy stlyle](https://numpydoc.readthedocs.io/en/latest/format.html)
 - The
   [Google style](https://www.sphinx-doc.org/en/master/usage/extensions/example_google.html)
-
-Support for the
-[Sphinx style](https://sphinx-rtd-tutorial.readthedocs.io/en/latest/docstrings.html)
-may be added in the future if there are requests for it.
+- The
+  [Sphinx style](https://sphinx-rtd-tutorial.readthedocs.io/en/latest/docstrings.html)
 
 Another note: this linter and [pydocstyle](https://github.com/PyCQA/pydocstyle)
 serves complementary purposes. It is recommended that you use both together.
 
 ## 1. Installation
 
 ```
```

### Comparing `pydoclint-0.1.0/pydoclint/flake8_entry.py` & `pydoclint-0.1.1/pydoclint/flake8_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,17 +137,17 @@
             self.allow_init_docstring,
         )
         requireReturnSectionWhenReturningNone = self._bool(
             '--require-return-section-when-returning-none',
             self.require_return_section_when_returning_none,
         )
 
-        if self.style not in {'numpy', 'google'}:
+        if self.style not in {'numpy', 'google', 'sphinx'}:
             raise ValueError(
-                'Invalid value for "--style": must be "numpy" or "google"'
+                'Invalid value for "--style": must be "numpy", "google", or "sphinx"'
             )
 
         v = Visitor(
             typeHintsInSignature=typeHintsInSignature,
             typeHintsInDocstring=typeHintsInDocstring,
             checkArgOrder=checkArgOrder,
             skipCheckingShortDocstrings=skipCheckingShortDocstrings,
```

### Comparing `pydoclint-0.1.0/pydoclint/main.py` & `pydoclint-0.1.1/pydoclint/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 def validateStyleValue(
         context: click.Context,
         param: click.Parameter,
         value: Optional[str],
 ) -> Optional[str]:
     """Validate the value of the 'style' option"""
-    if value not in {'numpy', 'google'}:
+    if value not in {'numpy', 'google', 'sphinx'}:
         raise click.BadParameter(
             '"--style" must be "numpy", "google", or "sphinx"'
         )
 
     return value
```

### Comparing `pydoclint-0.1.0/pydoclint/parse_config.py` & `pydoclint-0.1.1/pydoclint/parse_config.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.0/pydoclint/utils/annotation.py` & `pydoclint-0.1.1/pydoclint/utils/annotation.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.0/pydoclint/utils/arg.py` & `pydoclint-0.1.1/pydoclint/utils/arg.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.0/pydoclint/utils/astTypes.py` & `pydoclint-0.1.1/pydoclint/utils/astTypes.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.0/pydoclint/utils/doc.py` & `pydoclint-0.1.1/pydoclint/utils/doc.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.0/pydoclint/utils/generic.py` & `pydoclint-0.1.1/pydoclint/utils/generic.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.0/pydoclint/utils/return_anno.py` & `pydoclint-0.1.1/pydoclint/utils/return_anno.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.0/pydoclint/utils/return_yield_raise.py` & `pydoclint-0.1.1/pydoclint/utils/return_yield_raise.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.0/pydoclint/utils/unparser.py` & `pydoclint-0.1.1/pydoclint/utils/unparser.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.0/pydoclint/utils/violation.py` & `pydoclint-0.1.1/pydoclint/utils/violation.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.0/pydoclint/utils/walk.py` & `pydoclint-0.1.1/pydoclint/utils/walk.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.0/pydoclint/visitor.py` & `pydoclint-0.1.1/pydoclint/visitor.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.0/pydoclint.egg-info/PKG-INFO` & `pydoclint-0.1.1/pydoclint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoclint
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python docstring linter that checks arguments, returns, yields, and raises sections
 Home-page: https://github.com/jsh9/pydoclint
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
@@ -23,23 +23,21 @@
 Here is a comparison of linting time on some famous Python projects:
 
 |                                                              | pydoclint | darglint                          |
 | ------------------------------------------------------------ | --------- | --------------------------------- |
 | [numpy](https://github.com/numpy/numpy)                      | 2.0 sec   | 49 min 9 sec (1,475x slower)      |
 | [scikit-learn](https://github.com/scikit-learn/scikit-learn) | 2.4 sec   | 3 hr 5 min 33 sec (4,639x slower) |
 
-Currently, _pydoclint_ supports two docstring styles:
+Currently, _pydoclint_ supports three docstring styles:
 
 - The [numpy stlyle](https://numpydoc.readthedocs.io/en/latest/format.html)
 - The
   [Google style](https://www.sphinx-doc.org/en/master/usage/extensions/example_google.html)
-
-Support for the
-[Sphinx style](https://sphinx-rtd-tutorial.readthedocs.io/en/latest/docstrings.html)
-may be added in the future if there are requests for it.
+- The
+  [Sphinx style](https://sphinx-rtd-tutorial.readthedocs.io/en/latest/docstrings.html)
 
 Another note: this linter and [pydocstyle](https://github.com/PyCQA/pydocstyle)
 serves complementary purposes. It is recommended that you use both together.
 
 ## 1. Installation
 
 ```
```

### Comparing `pydoclint-0.1.0/pydoclint.egg-info/SOURCES.txt` & `pydoclint-0.1.1/pydoclint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.0/setup.cfg` & `pydoclint-0.1.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pydoclint
-version = 0.1.0
+version = 0.1.1
 description = A Python docstring linter that checks arguments, returns, yields, and raises sections
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jsh9/pydoclint
 license = MIT
 license_file = LICENSE
 classifiers =
```

### Comparing `pydoclint-0.1.0/tests/test_generic.py` & `pydoclint-0.1.1/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.0/tests/test_main.py` & `pydoclint-0.1.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.1.0/tests/test_parse_config.py` & `pydoclint-0.1.1/tests/test_parse_config.py`

 * *Files identical despite different names*

