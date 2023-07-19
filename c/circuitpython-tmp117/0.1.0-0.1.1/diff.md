# Comparing `tmp/circuitpython-tmp117-0.1.0.tar.gz` & `tmp/circuitpython-tmp117-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-tmp117-0.1.0.tar", last modified: Sun May 14 21:16:19 2023, max compression
+gzip compressed data, was "circuitpython-tmp117-0.1.1.tar", last modified: Wed Jul 19 00:42:59 2023, max compression
```

## Comparing `circuitpython-tmp117-0.1.0.tar` & `circuitpython-tmp117-0.1.1.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:16:19.098994 circuitpython-tmp117-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:16:19.090995 circuitpython-tmp117-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:16:19.094994 circuitpython-tmp117-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-14 21:15:54.000000 circuitpython-tmp117-0.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-14 21:15:54.000000 circuitpython-tmp117-0.1.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-14 21:15:54.000000 circuitpython-tmp117-0.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-14 21:15:54.000000 circuitpython-tmp117-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-14 21:15:54.000000 circuitpython-tmp117-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-14 21:15:54.000000 circuitpython-tmp117-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-14 21:15:54.000000 circuitpython-tmp117-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-14 21:15:54.000000 circuitpython-tmp117-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-14 21:15:54.000000 circuitpython-tmp117-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-14 21:16:19.098994 circuitpython-tmp117-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-14 21:15:54.000000 circuitpython-tmp117-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:16:19.094994 circuitpython-tmp117-0.1.0/circuitpython_tmp117.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-14 21:16:19.000000 circuitpython-tmp117-0.1.0/circuitpython_tmp117.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-14 21:16:19.000000 circuitpython-tmp117-0.1.0/circuitpython_tmp117.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 21:16:19.000000 circuitpython-tmp117-0.1.0/circuitpython_tmp117.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-14 21:16:19.000000 circuitpython-tmp117-0.1.0/circuitpython_tmp117.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-14 21:16:19.000000 circuitpython-tmp117-0.1.0/circuitpython_tmp117.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:16:19.094994 circuitpython-tmp117-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:16:19.098994 circuitpython-tmp117-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-14 21:15:54.000000 circuitpython-tmp117-0.1.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-14 21:15:54.000000 circuitpython-tmp117-0.1.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-14 21:15:54.000000 circuitpython-tmp117-0.1.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-14 21:15:54.000000 circuitpython-tmp117-0.1.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-14 21:15:54.000000 circuitpython-tmp117-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-14 21:15:54.000000 circuitpython-tmp117-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 21:15:54.000000 circuitpython-tmp117-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-14 21:15:54.000000 circuitpython-tmp117-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-14 21:15:54.000000 circuitpython-tmp117-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-14 21:15:54.000000 circuitpython-tmp117-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-14 21:15:54.000000 circuitpython-tmp117-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:16:19.098994 circuitpython-tmp117-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-14 21:16:09.000000 circuitpython-tmp117-0.1.0/examples/tmp117_averaged_measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-14 21:16:09.000000 circuitpython-tmp117-0.1.0/examples/tmp117_limits_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-14 21:16:09.000000 circuitpython-tmp117-0.1.0/examples/tmp117_measurement_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-14 21:16:09.000000 circuitpython-tmp117-0.1.0/examples/tmp117_offset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-14 21:16:09.000000 circuitpython-tmp117-0.1.0/examples/tmp117_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-14 21:16:09.000000 circuitpython-tmp117-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-14 21:15:54.000000 circuitpython-tmp117-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 21:16:19.098994 circuitpython-tmp117-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-05-14 21:16:09.000000 circuitpython-tmp117-0.1.0/tmp117.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:42:59.164439 circuitpython-tmp117-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:42:59.156438 circuitpython-tmp117-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:42:59.160439 circuitpython-tmp117-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-19 00:42:40.000000 circuitpython-tmp117-0.1.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-19 00:42:40.000000 circuitpython-tmp117-0.1.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-19 00:42:40.000000 circuitpython-tmp117-0.1.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-19 00:42:40.000000 circuitpython-tmp117-0.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-19 00:42:40.000000 circuitpython-tmp117-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-19 00:42:40.000000 circuitpython-tmp117-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-19 00:42:40.000000 circuitpython-tmp117-0.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-19 00:42:40.000000 circuitpython-tmp117-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-19 00:42:40.000000 circuitpython-tmp117-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-19 00:42:59.164439 circuitpython-tmp117-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-19 00:42:40.000000 circuitpython-tmp117-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:42:59.160439 circuitpython-tmp117-0.1.1/circuitpython_tmp117.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-19 00:42:59.000000 circuitpython-tmp117-0.1.1/circuitpython_tmp117.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-19 00:42:59.000000 circuitpython-tmp117-0.1.1/circuitpython_tmp117.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 00:42:59.000000 circuitpython-tmp117-0.1.1/circuitpython_tmp117.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-19 00:42:59.000000 circuitpython-tmp117-0.1.1/circuitpython_tmp117.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-19 00:42:59.000000 circuitpython-tmp117-0.1.1/circuitpython_tmp117.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:42:59.160439 circuitpython-tmp117-0.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:42:59.164439 circuitpython-tmp117-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-19 00:42:40.000000 circuitpython-tmp117-0.1.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-19 00:42:40.000000 circuitpython-tmp117-0.1.1/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-19 00:42:40.000000 circuitpython-tmp117-0.1.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-19 00:42:40.000000 circuitpython-tmp117-0.1.1/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-19 00:42:40.000000 circuitpython-tmp117-0.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-19 00:42:40.000000 circuitpython-tmp117-0.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-19 00:42:40.000000 circuitpython-tmp117-0.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-07-19 00:42:40.000000 circuitpython-tmp117-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-19 00:42:40.000000 circuitpython-tmp117-0.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-19 00:42:40.000000 circuitpython-tmp117-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-19 00:42:40.000000 circuitpython-tmp117-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:42:59.164439 circuitpython-tmp117-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-19 00:42:51.000000 circuitpython-tmp117-0.1.1/examples/tmp117_averaged_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-19 00:42:51.000000 circuitpython-tmp117-0.1.1/examples/tmp117_limits_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-19 00:42:51.000000 circuitpython-tmp117-0.1.1/examples/tmp117_measurement_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-19 00:42:51.000000 circuitpython-tmp117-0.1.1/examples/tmp117_offset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-19 00:42:51.000000 circuitpython-tmp117-0.1.1/examples/tmp117_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1600424 2023-07-19 00:42:40.000000 circuitpython-tmp117-0.1.1/mpy-cross
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-19 00:42:51.000000 circuitpython-tmp117-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-19 00:42:40.000000 circuitpython-tmp117-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 00:42:59.164439 circuitpython-tmp117-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    21534 2023-07-19 00:42:51.000000 circuitpython-tmp117-0.1.1/tmp117.py
```

### Comparing `circuitpython-tmp117-0.1.0/.github/workflows/build.yml` & `circuitpython-tmp117-0.1.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-tmp117-0.1.0/.github/workflows/release_gh.yml` & `circuitpython-tmp117-0.1.1/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-tmp117-0.1.0/.pre-commit-config.yaml` & `circuitpython-tmp117-0.1.1/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,31 @@
-# SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
+# SPDX-FileCopyrightText: 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.15.5
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
-        exclude: "^(docs/|examples/|tests/|setup.py$)"
+        exclude: "^(docs/|examples/|tests/)"
       - id: pylint
         name: pylint (example code)
         description: Run pylint rules on "examples/*.py" files
         types: [python]
         files: "^examples/"
         args:
           - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
-      - id: pylint
-        name: pylint (test code)
-        description: Run pylint rules on "tests/*.py" files
-        types: [python]
-        files: "^tests/"
-        args:
-          - --disable=missing-docstring,consider-using-f-string,duplicate-code
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `circuitpython-tmp117-0.1.0/LICENSE` & `circuitpython-tmp117-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-tmp117-0.1.0/PKG-INFO` & `circuitpython-tmp117-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: circuitpython-tmp117
-Version: 0.1.0
+Version: 0.1.1
 Summary: CircuitPython TMP117 Temperature Sensor Low Memory driver
-Author-email: "Jose D. Montoya" <jlib@mailmeto.mozmail.com>
+Author-email: JDM <jdm@mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_TMP117
-Keywords: sensor,blinka,circuitpython,micropython,tmp117,temperature,tmp117,TMP117,low,memory,sensor,driver
+Keywords: sensor,circuitpython,tmp117,temperature,TMP117,low,memory,sensor,driver
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
```

### Comparing `circuitpython-tmp117-0.1.0/README.rst` & `circuitpython-tmp117-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-tmp117-0.1.0/circuitpython_tmp117.egg-info/PKG-INFO` & `circuitpython-tmp117-0.1.1/circuitpython_tmp117.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: circuitpython-tmp117
-Version: 0.1.0
+Version: 0.1.1
 Summary: CircuitPython TMP117 Temperature Sensor Low Memory driver
-Author-email: "Jose D. Montoya" <jlib@mailmeto.mozmail.com>
+Author-email: JDM <jdm@mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_TMP117
-Keywords: sensor,blinka,circuitpython,micropython,tmp117,temperature,tmp117,TMP117,low,memory,sensor,driver
+Keywords: sensor,circuitpython,tmp117,temperature,TMP117,low,memory,sensor,driver
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
```

### Comparing `circuitpython-tmp117-0.1.0/circuitpython_tmp117.egg-info/SOURCES.txt` & `circuitpython-tmp117-0.1.1/circuitpython_tmp117.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .gitignore
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yaml
 LICENSE
 README.rst
+mpy-cross
 pyproject.toml
 requirements.txt
 tmp117.py
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
 .github/workflows/release_gh.yml
 .github/workflows/release_pypi.yml
```

### Comparing `circuitpython-tmp117-0.1.0/docs/_static/Logo.png` & `circuitpython-tmp117-0.1.1/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `circuitpython-tmp117-0.1.0/docs/_static/favicon.ico` & `circuitpython-tmp117-0.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-tmp117-0.1.0/docs/conf.py` & `circuitpython-tmp117-0.1.1/docs/conf.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
-    "sphinx.ext.napoleon",
     "sphinx.ext.viewcode",
     "sphinx_immaterial",
 ]
 
 autodoc_preserve_defaults = True
 
 intersphinx_mapping = {
@@ -184,65 +183,7 @@
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
 # These paths are either relative to html_static_path
 # or fully qualified paths (eg. https://...)
 html_css_files = ["extra_css.css"]
-
-
-# -- Options for LaTeX output ---------------------------------------------
-
-latex_elements = {
-    # The paper size ('letterpaper' or 'a4paper').
-    # 'papersize': 'letterpaper',
-    # The font size ('10pt', '11pt' or '12pt').
-    # 'pointsize': '10pt',
-    # Additional stuff for the LaTeX preamble.
-    # 'preamble': '',
-    # Latex figure (float) alignment
-    # 'figure_align': 'htbp',
-}
-
-# Grouping the document tree into LaTeX files. List of tuples
-# (source start file, target name, title,
-#  author, documentclass [howto, manual, or own class]).
-latex_documents = [
-    (
-        master_doc,
-        "CircuitPython_tmp117_Library.tex",
-        "CircuitPython tmp117 Library Documentation",
-        author,
-        "manual",
-    ),
-]
-
-# -- Options for manual page output ---------------------------------------
-
-# One entry per manual page. List of tuples
-# (source start file, name, description, authors, manual section).
-man_pages = [
-    (
-        master_doc,
-        "CircuitPython_tmp117_Library",
-        "circuitPython tmp117 Library Documentation",
-        [author],
-        1,
-    ),
-]
-
-# -- Options for Texinfo output -------------------------------------------
-
-# Grouping the document tree into Texinfo files. List of tuples
-# (source start file, target name, title, author,
-#  dir menu entry, description, category)
-texinfo_documents = [
-    (
-        master_doc,
-        "CircuitPython_tmp117_Library",
-        "CircuitPython tmp117 Library Documentation",
-        author,
-        "CircuitPython_tmp117_Library",
-        "One line description of project.",
-        "Miscellaneous",
-    ),
-]
```

### Comparing `circuitpython-tmp117-0.1.0/docs/examples.rst` & `circuitpython-tmp117-0.1.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-tmp117-0.1.0/examples/tmp117_averaged_measurements.py` & `circuitpython-tmp117-0.1.1/examples/tmp117_averaged_measurements.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 
 tmp.averaged_measurements = tmp117.AVERAGE_1X
 
 while True:
     for averaged_measurements in tmp117.averaged_measurements_values:
         print("Current Averaged measurements setting: ", tmp.averaged_measurements)
         for _ in range(10):
-            temp = tmp.temperature
-            print("Temperature: {:.2f}C".format(temp))
+            print(f"Temperature: {tmp.temperature:.2f}°C")
+            print()
             time.sleep(0.5)
         tmp.averaged_measurements = averaged_measurements
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `circuitpython-tmp117-0.1.0/examples/tmp117_measurement_delay.py` & `circuitpython-tmp117-0.1.1/examples/tmp117_measurement_delay.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,11 +23,11 @@
 }
 
 
 while True:
     for measurement_delay in range(8):
         print("Current Measurement delay setting: ", delay_times[tmp.measurement_delay])
         for _ in range(10):
-            temp = tmp.temperature
-            print("Temperature: {:.2f}C".format(temp))
+            print(f"Temperature: {tmp.temperature:.2f}°C")
+            print()
             time.sleep(0.5)
         tmp.measurement_delay = measurement_delay
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `circuitpython-tmp117-0.1.0/pyproject.toml` & `circuitpython-tmp117-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,28 +8,25 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-tmp117"
 description = "CircuitPython TMP117 Temperature Sensor Low Memory driver"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.rst"
 authors = [
-    {name = "Jose D. Montoya", email = "jlib@mailmeto.mozmail.com"}
+    {name = "JDM", email = "jdm@mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_TMP117"}
 keywords = [
     "sensor",
-    "blinka",
     "circuitpython",
-    "micropython",
     "tmp117",
     "temperature",
-    "tmp117",
     "TMP117",
     "low",
     "memory",
     "sensor",
     "driver",
 ]
 license = {text = "MIT"}
```

### Comparing `circuitpython-tmp117-0.1.0/tmp117.py` & `circuitpython-tmp117-0.1.1/tmp117.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 try:
     from typing import Tuple
     from busio import I2C
     from typing_extensions import Literal
 except ImportError:
     pass
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __repo__ = "https://github.com/jposada202020/CircuitPython_TMP117.git"
 
 _I2C_ADDR = 0x48  # default I2C Address
 _TEMP_RESULT = const(0x00)
 _CONFIGURATION = const(0x01)
 _T_HIGH_LIMIT = const(0x02)
 _T_LOW_LIMIT = const(0x03)
@@ -129,15 +129,14 @@
     _avg_3 = {0: 1, 1: 1, 2: 1, 3: 1, 4: 1, 5: 4, 6: 8, 7: 16}
     _avg_2 = {0: 0.5, 1: 0.5, 2: 0.5, 3: 0.5, 4: 1, 5: 4, 6: 8, 7: 16}
     _avg_1 = {0: 0.125, 1: 0.125, 2: 0.25, 3: 0.5, 4: 1, 5: 4, 6: 8, 7: 16}
     _avg_0 = {0: 0.0155, 1: 0.125, 2: 0.25, 3: 0.5, 4: 1, 5: 4, 6: 8, 7: 16}
     _averaging_modes = {0: _avg_0, 1: _avg_1, 2: _avg_2, 3: _avg_3}
 
     def __init__(self, i2c_bus: I2C, address: int = _I2C_ADDR) -> None:
-
         self.i2c_device = i2c_device.I2CDevice(i2c_bus, address)
         if self._part_id != _DEVICE_ID_VALUE:
             raise AttributeError("Cannot find a TMP117")
         self._soft_reset = True
         # Following a reset, the temperature register reads –256 °C until the first
         # conversion, including averaging, is complete. So we sleep for that amount of time
         time.sleep(
@@ -184,26 +183,28 @@
     @temperature_offset.setter
     def temperature_offset(self, value: float) -> None:
         self._raw_temperature_offset = self._scaled_limit(value)
 
     @property
     def high_limit(self) -> float:
         """The high temperature limit in Celsius. When the measured temperature exceeds this
-        value, the `high_alert` attribute of the `alert_status` property will be True."""
+        value, the `high_alert` attribute of the `alert_status` property will be True.
+        """
 
         return self._raw_high_limit * _TMP117_RESOLUTION
 
     @high_limit.setter
     def high_limit(self, value: float) -> None:
         self._raw_high_limit = self._scaled_limit(value)
 
     @property
     def low_limit(self) -> float:
         """The low  temperature limit in Celsius. When the measured temperature goes below
-        this value, the `low_alert` attribute of the `alert_status` property will be True."""
+        this value, the `low_alert` attribute of the `alert_status` property will be True.
+        """
 
         return self._raw_low_limit * _TMP117_RESOLUTION
 
     @low_limit.setter
     def low_limit(self, value: float) -> None:
         self._raw_low_limit = self._scaled_limit(value)
 
@@ -490,15 +491,14 @@
                 eeprom3_data[1],
             ]
         )
         # Convert to an integer
         return combined_id
 
     def _set_mode_and_wait_for_measurement(self, mode: int) -> float:
-
         self._mode = mode
         # poll for data ready
         while not self._read_status()[2]:
             time.sleep(0.001)
 
         return self._raw_temperature * _TMP117_RESOLUTION
```

