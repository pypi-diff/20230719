# Comparing `tmp/json2xml-3.9.0.tar.gz` & `tmp/json2xml-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json2xml-3.9.0.tar", last modified: Sat Dec 18 19:58:27 2021, max compression
+gzip compressed data, was "json2xml-4.0.0.tar", last modified: Wed Jul 19 06:20:37 2023, max compression
```

## Comparing `json2xml-3.9.0.tar` & `json2xml-4.0.0.tar`

### file list

```diff
@@ -1,44 +1,41 @@
-drwxr-xr-x   0 vinitkumar   (501) staff       (20)        0 2021-12-18 19:58:27.321149 json2xml-3.9.0/
--rw-r--r--   0 vinitkumar   (501) staff       (20)      159 2021-12-18 19:21:26.000000 json2xml-3.9.0/AUTHORS.rst
--rw-r--r--   0 vinitkumar   (501) staff       (20)     3542 2019-02-25 20:05:41.000000 json2xml-3.9.0/CONTRIBUTING.rst
--rw-r--r--   0 vinitkumar   (501) staff       (20)     4039 2021-12-18 19:57:03.000000 json2xml-3.9.0/HISTORY.rst
--rw-r--r--   0 vinitkumar   (501) staff       (20)      583 2019-02-25 20:05:41.000000 json2xml-3.9.0/LICENSE
--rw-r--r--   0 vinitkumar   (501) staff       (20)      320 2021-08-28 15:38:28.000000 json2xml-3.9.0/MANIFEST.in
--rw-r--r--   0 vinitkumar   (501) staff       (20)    10225 2021-12-18 19:58:27.321362 json2xml-3.9.0/PKG-INFO
--rw-r--r--   0 vinitkumar   (501) staff       (20)     5406 2021-12-18 19:55:32.000000 json2xml-3.9.0/README.rst
-drwxr-xr-x   0 vinitkumar   (501) staff       (20)        0 2021-12-18 19:58:27.308545 json2xml-3.9.0/docs/
--rw-r--r--   0 vinitkumar   (501) staff       (20)      609 2019-02-25 20:05:41.000000 json2xml-3.9.0/docs/Makefile
-drwxr-xr-x   0 vinitkumar   (501) staff       (20)        0 2021-12-18 19:58:27.296012 json2xml-3.9.0/docs/_build/
-drwxr-xr-x   0 vinitkumar   (501) staff       (20)        0 2021-12-18 19:58:27.296250 json2xml-3.9.0/docs/_build/html/
-drwxr-xr-x   0 vinitkumar   (501) staff       (20)        0 2021-12-18 19:58:27.312723 json2xml-3.9.0/docs/_build/html/_static/
--rw-r--r--   0 vinitkumar   (501) staff       (20)      286 2021-10-10 07:21:47.000000 json2xml-3.9.0/docs/_build/html/_static/file.png
--rw-r--r--   0 vinitkumar   (501) staff       (20)       90 2021-10-10 07:21:47.000000 json2xml-3.9.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 vinitkumar   (501) staff       (20)       90 2021-10-10 07:21:47.000000 json2xml-3.9.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 vinitkumar   (501) staff       (20)       28 2019-02-25 20:05:41.000000 json2xml-3.9.0/docs/authors.rst
--rwxr-xr-x   0 vinitkumar   (501) staff       (20)     4814 2021-10-10 08:04:11.000000 json2xml-3.9.0/docs/conf.py
--rw-r--r--   0 vinitkumar   (501) staff       (20)       33 2019-02-25 20:05:41.000000 json2xml-3.9.0/docs/contributing.rst
--rw-r--r--   0 vinitkumar   (501) staff       (20)       28 2019-02-25 20:05:41.000000 json2xml-3.9.0/docs/history.rst
--rw-r--r--   0 vinitkumar   (501) staff       (20)      305 2019-02-25 20:05:41.000000 json2xml-3.9.0/docs/index.rst
--rw-r--r--   0 vinitkumar   (501) staff       (20)     1130 2019-02-25 20:05:41.000000 json2xml-3.9.0/docs/installation.rst
--rw-r--r--   0 vinitkumar   (501) staff       (20)      584 2021-10-10 08:15:24.000000 json2xml-3.9.0/docs/json2xml.rst
--rw-r--r--   0 vinitkumar   (501) staff       (20)      770 2019-02-25 20:05:41.000000 json2xml-3.9.0/docs/make.bat
--rw-r--r--   0 vinitkumar   (501) staff       (20)       61 2021-10-10 08:15:24.000000 json2xml-3.9.0/docs/modules.rst
--rw-r--r--   0 vinitkumar   (501) staff       (20)       27 2019-02-25 20:05:41.000000 json2xml-3.9.0/docs/readme.rst
--rw-r--r--   0 vinitkumar   (501) staff       (20)       71 2019-02-25 20:05:41.000000 json2xml-3.9.0/docs/usage.rst
-drwxr-xr-x   0 vinitkumar   (501) staff       (20)        0 2021-12-18 19:58:27.315689 json2xml-3.9.0/json2xml/
--rw-r--r--   0 vinitkumar   (501) staff       (20)      215 2021-12-18 19:49:54.000000 json2xml-3.9.0/json2xml/__init__.py
--rwxr-xr-x   0 vinitkumar   (501) staff       (20)    14823 2021-12-18 19:21:26.000000 json2xml-3.9.0/json2xml/dicttoxml.py
--rw-r--r--   0 vinitkumar   (501) staff       (20)     1076 2021-10-10 11:29:33.000000 json2xml-3.9.0/json2xml/json2xml.py
--rw-r--r--   0 vinitkumar   (501) staff       (20)     1709 2021-09-10 17:09:57.000000 json2xml-3.9.0/json2xml/utils.py
-drwxr-xr-x   0 vinitkumar   (501) staff       (20)        0 2021-12-18 19:58:27.319798 json2xml-3.9.0/json2xml.egg-info/
--rw-r--r--   0 vinitkumar   (501) staff       (20)    10225 2021-12-18 19:58:27.000000 json2xml-3.9.0/json2xml.egg-info/PKG-INFO
--rw-r--r--   0 vinitkumar   (501) staff       (20)      706 2021-12-18 19:58:27.000000 json2xml-3.9.0/json2xml.egg-info/SOURCES.txt
--rw-r--r--   0 vinitkumar   (501) staff       (20)        1 2021-12-18 19:58:27.000000 json2xml-3.9.0/json2xml.egg-info/dependency_links.txt
--rw-r--r--   0 vinitkumar   (501) staff       (20)        1 2021-12-18 19:58:27.000000 json2xml-3.9.0/json2xml.egg-info/not-zip-safe
--rw-r--r--   0 vinitkumar   (501) staff       (20)      306 2021-12-18 19:58:27.000000 json2xml-3.9.0/json2xml.egg-info/requires.txt
--rw-r--r--   0 vinitkumar   (501) staff       (20)        9 2021-12-18 19:58:27.000000 json2xml-3.9.0/json2xml.egg-info/top_level.txt
--rw-r--r--   0 vinitkumar   (501) staff       (20)      650 2021-12-18 19:58:27.322445 json2xml-3.9.0/setup.cfg
--rw-r--r--   0 vinitkumar   (501) staff       (20)     1445 2021-12-18 19:49:54.000000 json2xml-3.9.0/setup.py
-drwxr-xr-x   0 vinitkumar   (501) staff       (20)        0 2021-12-18 19:58:27.320620 json2xml-3.9.0/tests/
--rw-r--r--   0 vinitkumar   (501) staff       (20)       63 2019-02-25 20:05:41.000000 json2xml-3.9.0/tests/__init__.py
--rw-r--r--   0 vinitkumar   (501) staff       (20)     6305 2021-12-18 19:21:26.000000 json2xml-3.9.0/tests/test_json2xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:20:37.741792 json2xml-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-19 06:20:28.000000 json2xml-4.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-19 06:20:28.000000 json2xml-4.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-07-19 06:20:28.000000 json2xml-4.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-19 06:20:28.000000 json2xml-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-19 06:20:28.000000 json2xml-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16107 2023-07-19 06:20:37.745792 json2xml-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-07-19 06:20:28.000000 json2xml-4.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:20:37.741792 json2xml-4.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-19 06:20:28.000000 json2xml-4.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-19 06:20:28.000000 json2xml-4.0.0/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4783 2023-07-19 06:20:28.000000 json2xml-4.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-19 06:20:28.000000 json2xml-4.0.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-19 06:20:28.000000 json2xml-4.0.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-19 06:20:28.000000 json2xml-4.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-19 06:20:28.000000 json2xml-4.0.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-19 06:20:28.000000 json2xml-4.0.0/docs/json2xml.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-19 06:20:28.000000 json2xml-4.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-19 06:20:28.000000 json2xml-4.0.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-19 06:20:28.000000 json2xml-4.0.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-19 06:20:28.000000 json2xml-4.0.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:20:37.741792 json2xml-4.0.0/json2xml/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-19 06:20:28.000000 json2xml-4.0.0/json2xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22708 2023-07-19 06:20:28.000000 json2xml-4.0.0/json2xml/dicttoxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-19 06:20:28.000000 json2xml-4.0.0/json2xml/json2xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-19 06:20:28.000000 json2xml-4.0.0/json2xml/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:20:37.741792 json2xml-4.0.0/json2xml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16107 2023-07-19 06:20:37.000000 json2xml-4.0.0/json2xml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-19 06:20:37.000000 json2xml-4.0.0/json2xml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 06:20:37.000000 json2xml-4.0.0/json2xml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 06:20:37.000000 json2xml-4.0.0/json2xml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-19 06:20:37.000000 json2xml-4.0.0/json2xml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 06:20:37.000000 json2xml-4.0.0/json2xml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-19 06:20:28.000000 json2xml-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-19 06:20:28.000000 json2xml-4.0.0/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-19 06:20:37.745792 json2xml-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-19 06:20:28.000000 json2xml-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:20:37.741792 json2xml-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 06:20:28.000000 json2xml-4.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14475 2023-07-19 06:20:28.000000 json2xml-4.0.0/tests/test_dict2xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-07-19 06:20:28.000000 json2xml-4.0.0/tests/test_json2xml.py
```

### Comparing `json2xml-3.9.0/CONTRIBUTING.rst` & `json2xml-4.0.0/CONTRIBUTING.rst`

 * *Files 6% similar despite different names*

```diff
@@ -98,17 +98,15 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, and add the
    feature to the list in README.rst.
-3. The pull request should work for Python 2.7, 3.4, 3.5 and 3.6, and for PyPy. Check
-   https://travis-ci.org/vinitkumar/json2xml/pull_requests
-   and make sure that the tests pass for all supported Python versions.
+3. The pull request should work for 3.7+, and for PyPy. Make sure that the tests pass for all supported Python versions.
 
 Tips
 ----
 
 To run a subset of tests::
```

### Comparing `json2xml-3.9.0/LICENSE` & `json2xml-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `json2xml-3.9.0/README.rst` & `json2xml-4.0.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,66 @@
 ========
 json2xml
 ========
 
 
-.. image:: https://img.shields.io/pypi/v/json2xml.svg
-        :target: https://pypi.python.org/pypi/json2xml
+.. image:: https://badge.fury.io/py/json2xml.svg
+.. image:: https://static.pepy.tech/personalized-badge/json2xml?period=total&units=international_system&left_color=blue&right_color=orange&left_text=Downloads
+        :target: https://pepy.tech/project/json2xml
+
 .. image:: https://github.com/vinitkumar/json2xml/actions/workflows/pythonpackage.yml/badge.svg
 .. image:: https://img.shields.io/pypi/pyversions/json2xml.svg
-.. image:: https://badge.fury.io/py/json2xml.svg
 .. image:: https://readthedocs.org/projects/json2xml/badge/?version=latest
         :target: https://json2xml.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
-.. image:: https://coveralls.io/repos/github/vinitkumar/json2xml/badge.svg?branch=master
-     :target: https://coveralls.io/github/vinitkumar/json2xml?branch=master
-
-
-Simple Python Library to convert JSON to XML
-
-* Free software: Apache Software License 2.0
-* Documentation: https://json2xml.readthedocs.io.
+.. image:: https://codecov.io/gh/vinitkumar/json2xml/branch/master/graph/badge.svg?token=Yt2h55eTL2
+      :target: https://codecov.io/gh/vinitkumar/json2xml
 
+A simple Python Library to convert JSON to XML
+Documentation: https://json2xml.readthedocs.io.
 
-Update
-------
-
-The dict2xml project has been forked and integrated in the project itself. This helped with cleaning up the code
-and also doing improvements. The goal is to remove all the dependencies from this project.
+An earlier dependency `dict2xml` project has been integrated into the project itself. It helped in cleaning up the code, adding types and tests.
 
 Features
---------
+^^^^^^^^
 
-It lets you convert json to xml in following ways:
+The library supports the following features:
 
-* from a `json` string
-* from a `json` file
-* from an API that emits `json` data
+* convert from a `json` string
+* convert from a `json` file
+* convert from an API that emits `json` data
 
 Usage
------
+^^^^^
 
-The usage is simple:
+The library can be used in these ways:
 
 
 .. code-block:: python
 
     from json2xml import json2xml
     from json2xml.utils import readfromurl, readfromstring, readfromjson
 
     # get the xml from an URL that return json
     data = readfromurl("https://coderwall.com/vinitcool76.json")
     print(json2xml.Json2xml(data).to_xml())
 
-    # get the xml from a json string
+    # get the xml from a json string like this:
     data = readfromstring(
         '{"login":"mojombo","id":1,"avatar_url":"https://avatars0.githubusercontent.com/u/1?v=4"}'
     )
     print(json2xml.Json2xml(data).to_xml())
 
-    # get the data from an URL
+    # get the data from an a JSON file like this:
     data = readfromjson("examples/licht.json")
     print(json2xml.Json2xml(data).to_xml())
 
 
 Custom Wrappers and indent
---------------------------
+^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 By default, a wrapper `all` and pretty `True` is set. However, you can change this easily in your code like this:
 
 .. code-block:: python
 
     from json2xml import json2xml
     from json2xml.utils import readfromurl, readfromstring, readfromjson
@@ -86,15 +79,15 @@
     <all>
       <login type="str">mojombo</login>
       <id type="int">1</id>
       <avatar_url type="str">https://avatars0.githubusercontent.com/u/1?v=4</avatar_url>
     </all>
 
 Omit List item
---------------
+^^^^^^^^^^^^^^
 
 Assume the following json input
 
 .. code-block:: json
 
     {
       "my_items": [
@@ -156,15 +149,15 @@
         </my_item>
       </my_items>
       <my_str_items type="str">a</my_str_items>
       <my_str_items type="str">b</my_str_items>
     </all>
 
 Optional Attribute Type Support
--------------------------------
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Now, we can also specify if the output xml needs to have type specified or not. Here is the usage:
 
  .. code-block:: python
 
     from json2xml import json2xml
     from json2xml.utils import readfromurl, readfromstring, readfromjson
@@ -186,14 +179,24 @@
       <avatar_url>https://avatars0.githubusercontent.com/u/1?v=4</avatar_url>
     </all>
 
 
 The methods are simple and easy to use and there are also checks inside of code to exit cleanly
 in case any of the input(file, string or API URL) returns invalid JSON.
 
-Credits
--------
+How to run tests
+^^^^^^^^^^^^^^^^
+
+This is provided by pytest, which is straight forward.
+
+ .. code-block:: console
+
+    virtualenv venv -p $(which python3.9)
+    pip install -r requirements-dev.txt
+    python setup.py install
+    pytest -vv
+
 
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+Help and Support to maintain this project
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+- You can sponsor my work for this plugin here: https://github.com/sponsors/vinitkumar/
```

### Comparing `json2xml-3.9.0/docs/Makefile` & `json2xml-4.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `json2xml-3.9.0/docs/conf.py` & `json2xml-4.0.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 #
 # json2xml documentation build configuration file, created by
 # sphinx-quickstart on Fri Jun  9 13:47:02 2017.
 #
 # This file is execfile()d with the current directory set to its
 # containing dir.
 #
@@ -43,17 +42,17 @@
 # source_suffix = ['.rst', '.md']
 source_suffix = '.rst'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
-project = u'json2xml'
-copyright = u"2019, Vinit Kumar"
-author = u"Vinit Kumar"
+project = 'json2xml'
+copyright = "2019, Vinit Kumar"
+author = "Vinit Kumar"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
 version = json2xml.__version__
@@ -125,38 +124,38 @@
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass
 # [howto, manual, or own class]).
 latex_documents = [
     (master_doc, 'json2xml.tex',
-     u'json2xml Documentation',
-     u'Vinit Kumar', 'manual'),
+     'json2xml Documentation',
+     'Vinit Kumar', 'manual'),
 ]
 
 
 # -- Options for manual page output ------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
     (master_doc, 'json2xml',
-     u'json2xml Documentation',
+     'json2xml Documentation',
      [author], 1)
 ]
 
 
 # -- Options for Texinfo output ----------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     (master_doc, 'json2xml',
-     u'json2xml Documentation',
+     'json2xml Documentation',
      author,
      'json2xml',
      'One line description of project.',
      'Miscellaneous'),
 ]
```

### Comparing `json2xml-3.9.0/docs/installation.rst` & `json2xml-4.0.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `json2xml-3.9.0/docs/json2xml.rst` & `json2xml-4.0.0/docs/json2xml.rst`

 * *Files identical despite different names*

### Comparing `json2xml-3.9.0/docs/make.bat` & `json2xml-4.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `json2xml-3.9.0/json2xml.egg-info/SOURCES.txt` & `json2xml-4.0.0/json2xml.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
+requirements.in
 setup.cfg
 setup.py
 docs/Makefile
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/json2xml.rst
 docs/make.bat
 docs/modules.rst
 docs/readme.rst
 docs/usage.rst
-docs/_build/html/_static/file.png
-docs/_build/html/_static/minus.png
-docs/_build/html/_static/plus.png
 json2xml/__init__.py
 json2xml/dicttoxml.py
 json2xml/json2xml.py
 json2xml/utils.py
 json2xml.egg-info/PKG-INFO
 json2xml.egg-info/SOURCES.txt
 json2xml.egg-info/dependency_links.txt
 json2xml.egg-info/not-zip-safe
 json2xml.egg-info/requires.txt
 json2xml.egg-info/top_level.txt
 tests/__init__.py
+tests/test_dict2xml.py
 tests/test_json2xml.py
```

### Comparing `json2xml-3.9.0/setup.cfg` & `json2xml-4.0.0/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 replace = version='{new_version}'
 
 [bumpversion:file:json2xml/__init__.py]
 search = __version__ = '{current_version}'
 replace = __version__ = '{new_version}'
 
 [bdist_wheel]
-universal = 1
+universal = false
 
 [flake8]
 exclude = docs
 max-line-length = 120
 
 [aliases]
 
@@ -26,11 +26,14 @@
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
 no_implicit_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 ignore_missing_imports = true
 
+[coverage:run]
+relative_files = True
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `json2xml-3.9.0/setup.py` & `json2xml-4.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 from json2xml import __version__
 
 with open("README.rst") as readme_file:
     readme = readme_file.read()
 
 with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
-requirements = [open("requirements.txt").read()]
+with open("requirements.in") as requirements_in:
+    requirements = [requirements_in.read()]
 
 setup_requirements = []
 
-test_requirements = []
+test_requirements = ["pytest==7.0.1", "py==1.11.0"]
 
 setup(
     author="Vinit Kumar",
     author_email="mail@vinitkumar.me",
     classifiers=[
         "Development Status :: 6 - Mature",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Programming Language :: Python :: Implementation :: PyPy",
+        "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     description="Simple Python Library to convert JSON to XML",
     install_requires=requirements,
     license="Apache Software License 2.0",
     long_description=readme + "\n\n" + history,
+    long_description_content_type="text/x-rst",
     include_package_data=True,
     keywords="json2xml",
     name="json2xml",
     packages=find_packages(include=["json2xml"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
```

