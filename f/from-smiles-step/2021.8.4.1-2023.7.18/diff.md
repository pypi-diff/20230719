# Comparing `tmp/from_smiles_step-2021.8.4.1.tar.gz` & `tmp/from_smiles_step-2023.7.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "from_smiles_step-2021.8.4.1.tar", last modified: Wed Aug  4 15:23:18 2021, max compression
+gzip compressed data, was "from_smiles_step-2023.7.18.tar", last modified: Wed Jul 19 13:54:14 2023, max compression
```

## Comparing `from_smiles_step-2021.8.4.1.tar` & `from_smiles_step-2023.7.18.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 15:23:18.029586 from_smiles_step-2021.8.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3339 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1481 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1510 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      348 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5034 2021-08-04 15:23:18.029586 from_smiles_step-2021.8.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2725 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 15:23:18.025586 from_smiles_step-2021.8.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     6802 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     8800 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 15:23:18.025586 from_smiles_step-2021.8.4.1/docs/developer/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/docs/developer/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      234 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/docs/developer/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1220 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/docs/developer/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/docs/developer/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)       94 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/docs/developer/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      555 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6479 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 15:23:18.025586 from_smiles_step-2021.8.4.1/docs/user/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/docs/user/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       59 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/docs/user/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 15:23:18.029586 from_smiles_step-2021.8.4.1/from_smiles_step/
--rw-r--r--   0 runner    (1001) docker     (121)      734 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/from_smiles_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      502 2021-08-04 15:23:18.029586 from_smiles_step-2021.8.4.1/from_smiles_step/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 15:23:18.029586 from_smiles_step-2021.8.4.1/from_smiles_step/data/
--rw-r--r--   0 runner    (1001) docker     (121)     2053 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/from_smiles_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (121)     8320 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/from_smiles_step/from_smiles.py
--rw-r--r--   0 runner    (1001) docker     (121)     1009 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/from_smiles_step/from_smiles_parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     1207 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/from_smiles_step/from_smiles_step.py
--rw-r--r--   0 runner    (1001) docker     (121)     1434 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/from_smiles_step/tk_from_smiles.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 15:23:18.029586 from_smiles_step-2021.8.4.1/from_smiles_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5034 2021-08-04 15:23:18.000000 from_smiles_step-2021.8.4.1/from_smiles_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      973 2021-08-04 15:23:18.000000 from_smiles_step-2021.8.4.1/from_smiles_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-04 15:23:18.000000 from_smiles_step-2021.8.4.1/from_smiles_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      141 2021-08-04 15:23:18.000000 from_smiles_step-2021.8.4.1/from_smiles_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-08-04 15:23:18.000000 from_smiles_step-2021.8.4.1/from_smiles_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-08-04 15:23:18.000000 from_smiles_step-2021.8.4.1/from_smiles_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       89 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/requirements_install.txt
--rw-r--r--   0 runner    (1001) docker     (121)      378 2021-08-04 15:23:18.029586 from_smiles_step-2021.8.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2884 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-04 15:23:18.029586 from_smiles_step-2021.8.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      594 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/tests/test_from_smiles_step.py
--rw-r--r--   0 runner    (1001) docker     (121)    68611 2021-08-04 15:23:05.000000 from_smiles_step-2021.8.4.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:54:14.129142 from_smiles_step-2023.7.18/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-07-19 13:54:14.129142 from_smiles_step-2023.7.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:54:14.125141 from_smiles_step-2023.7.18/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8800 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:54:14.125141 from_smiles_step-2023.7.18/docs/developer/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/docs/developer/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/docs/developer/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/docs/developer/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/docs/developer/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/docs/developer/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:54:14.125141 from_smiles_step-2023.7.18/docs/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/docs/user/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/docs/user/overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:54:14.133142 from_smiles_step-2023.7.18/from_smiles_step/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/from_smiles_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-19 13:54:14.133142 from_smiles_step-2023.7.18/from_smiles_step/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:54:14.129142 from_smiles_step-2023.7.18/from_smiles_step/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/from_smiles_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/from_smiles_step/from_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/from_smiles_step/from_smiles_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/from_smiles_step/from_smiles_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/from_smiles_step/tk_from_smiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:54:14.129142 from_smiles_step-2023.7.18/from_smiles_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-07-19 13:54:14.000000 from_smiles_step-2023.7.18/from_smiles_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-19 13:54:14.000000 from_smiles_step-2023.7.18/from_smiles_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 13:54:14.000000 from_smiles_step-2023.7.18/from_smiles_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-19 13:54:14.000000 from_smiles_step-2023.7.18/from_smiles_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 13:54:14.000000 from_smiles_step-2023.7.18/from_smiles_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-19 13:54:14.000000 from_smiles_step-2023.7.18/from_smiles_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/requirements_install.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-19 13:54:14.129142 from_smiles_step-2023.7.18/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:54:14.129142 from_smiles_step-2023.7.18/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/tests/test_from_smiles_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-19 13:53:46.000000 from_smiles_step-2023.7.18/versioneer.py
```

### Comparing `from_smiles_step-2021.8.4.1/CONTRIBUTING.rst` & `from_smiles_step-2023.7.18/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `from_smiles_step-2021.8.4.1/HISTORY.rst` & `from_smiles_step-2023.7.18/HISTORY.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 =======
 History
 =======
 
+2023.7.18 -- Added support for InChI and InChIKeys
+
 2021.2.10 (10 February 2021)
 ----------------------------
 
 * Updated the README file to give a better description.
 * Updated the short description in setup.py to work with the new installer.
 * Added keywords for better searchability.
```

### Comparing `from_smiles_step-2021.8.4.1/LICENSE` & `from_smiles_step-2023.7.18/LICENSE`

 * *Files identical despite different names*

### Comparing `from_smiles_step-2021.8.4.1/PKG-INFO` & `from_smiles_step-2023.7.18/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: from_smiles_step
-Version: 2021.8.4.1
+Version: 2023.7.18
 Summary: A SEAMM plug-in for creating structures from a SMILES string.
 Home-page: https://github.com/molssi-seamm/from_smiles_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,SMILES,molecule
 Platform: Linux
@@ -12,16 +12,16 @@
 Platform: Unix
 Platform: Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 .. image:: https://img.shields.io/github/issues-pr-raw/molssi-seamm/from_smiles_step
    :target: https://github.com/molssi-seamm/from_smiles_step/pulls
    :alt: GitHub pull requests
@@ -46,14 +46,18 @@
    :target: https://pyup.io/repos/github/molssi-seamm/from_smiles_step/
    :alt: Updates for Dependencies
 
 .. image:: https://img.shields.io/pypi/v/from_smiles_step.svg
    :target: https://pypi.python.org/pypi/from_smiles_step
    :alt: PyPi VERSION
 
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5159800.svg
+   :target: https://doi.org/10.5281/zenodo.5159800
+   :alt: DOI
+
 =========================
 SEAMM From SMILES plug-in
 =========================
 
 A SEAMM plug-in for creating structures from a SMILES string.
 
 This plug-in accepts SMILES_ (Simplified Molecular-Input Line Entry
@@ -81,24 +85,26 @@
 This package was created with Cookiecutter_ and the `molssi-seamm/cookiecutter-seamm-plugin`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`molssi-seamm/cookiecutter-seamm-plugin`: https://github.com/molssi-seamm/cookiecutter-seamm-plugin
 
 Developed by the Molecular Sciences Software Institute (MolSSI_),
 which receives funding from the `National Science Foundation`_ under
-award ACI-1547580
+award OAC-1547580 and CHE-2136142.
 
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
+2023.7.18 -- Added support for InChI and InChIKeys
+
 2021.2.10 (10 February 2021)
 ----------------------------
 
 * Updated the README file to give a better description.
 * Updated the short description in setup.py to work with the new installer.
 * Added keywords for better searchability.
 
@@ -153,9 +159,7 @@
 
 * Internal changes cleaning the code.
   
 0.1.0 (20 January 2018)
 -----------------------
 
 * First release on PyPI.
-
-
```

### Comparing `from_smiles_step-2021.8.4.1/README.rst` & `from_smiles_step-2023.7.18/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,18 @@
    :target: https://pyup.io/repos/github/molssi-seamm/from_smiles_step/
    :alt: Updates for Dependencies
 
 .. image:: https://img.shields.io/pypi/v/from_smiles_step.svg
    :target: https://pypi.python.org/pypi/from_smiles_step
    :alt: PyPi VERSION
 
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5159800.svg
+   :target: https://doi.org/10.5281/zenodo.5159800
+   :alt: DOI
+
 =========================
 SEAMM From SMILES plug-in
 =========================
 
 A SEAMM plug-in for creating structures from a SMILES string.
 
 This plug-in accepts SMILES_ (Simplified Molecular-Input Line Entry
@@ -57,11 +61,11 @@
 This package was created with Cookiecutter_ and the `molssi-seamm/cookiecutter-seamm-plugin`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`molssi-seamm/cookiecutter-seamm-plugin`: https://github.com/molssi-seamm/cookiecutter-seamm-plugin
 
 Developed by the Molecular Sciences Software Institute (MolSSI_),
 which receives funding from the `National Science Foundation`_ under
-award ACI-1547580
+award OAC-1547580 and CHE-2136142.
 
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
```

### Comparing `from_smiles_step-2021.8.4.1/docs/Makefile` & `from_smiles_step-2023.7.18/docs/Makefile`

 * *Files identical despite different names*

### Comparing `from_smiles_step-2021.8.4.1/docs/conf.py` & `from_smiles_step-2023.7.18/docs/conf.py`

 * *Files identical despite different names*

### Comparing `from_smiles_step-2021.8.4.1/docs/developer/installation.rst` & `from_smiles_step-2023.7.18/docs/developer/installation.rst`

 * *Files identical despite different names*

### Comparing `from_smiles_step-2021.8.4.1/docs/index.rst` & `from_smiles_step-2023.7.18/docs/index.rst`

 * *Files identical despite different names*

### Comparing `from_smiles_step-2021.8.4.1/docs/make.bat` & `from_smiles_step-2023.7.18/docs/make.bat`

 * *Files identical despite different names*

### Comparing `from_smiles_step-2021.8.4.1/from_smiles_step/__init__.py` & `from_smiles_step-2023.7.18/from_smiles_step/__init__.py`

 * *Files identical despite different names*

### Comparing `from_smiles_step-2021.8.4.1/from_smiles_step/data/references.bib` & `from_smiles_step-2023.7.18/from_smiles_step/data/references.bib`

 * *Files 8% similar despite different names*

```diff
@@ -20,22 +20,25 @@
 first line of the entry after the 'article' or 'misc' (for software) keyword.
 
 See the documentation for the Reference Handler for the other arguments to cite().
 
 # End of initial comments #
 
 @Misc{ from_smiles_step,
-	author = {Paul Saxe},
-	title = {From Smiles plug-in for SEAMM for creating structures from SMILES},
-	month = {$month},
-	year = {$year},
-	organization = {The Molecular Sciences Software Institute (MolSSI)},
-	url = {https://github.com/molssi-seamm/from_smiles_step},
-	address = {Virginia Tech, Blacksburg, VA, USA},
-	version = {$version}
+  author       = {Paul Saxe},
+  title        = {From Smiles plug-in for SEAMM for creating structures from SMILES},
+  month        = {$month},
+  year         = {$year},
+  doi          = {10.5281/zenodo.5159800},
+  organization = {The Molecular Sciences Software Institute (MolSSI)},
+  url          = {https://github.com/molssi-seamm/from_smiles_step},
+  address      = {Virginia Tech, Blacksburg, VA, USA},
+  version      = {$version},
+  note         = {{Funding including NSF OAC-1547580 and CHE-2136142 grants}},
+  publisher    = {Zenodo}
 }
                   
 @Article{openbabel,
     author={O'Boyle, Noel M.
     and Banck, Michael
     and James, Craig A.
     and Morley, Chris
```

### Comparing `from_smiles_step-2021.8.4.1/from_smiles_step/from_smiles.py` & `from_smiles_step-2023.7.18/from_smiles_step/from_smiles.py`

 * *Files 18% similar despite different names*

```diff
@@ -55,21 +55,33 @@
                 or final values. If None, then the parameters values will
                 be used as is.
         """
 
         if not P:
             P = self.parameters.values_to_dict()
 
-        if P["smiles string"][0] == "$":
-            text = (
-                "Create the structure from the SMILES in the variable"
-                " '{smiles string}', "
-            )
+        if P["notation"] == "perceive":
+            if P["smiles string"][0] == "$":
+                text = (
+                    "Perceive the line notation (SMILES, InChI,...) and create the "
+                    "structure from the string in the variable '{smiles string}', "
+                )
+            else:
+                text = (
+                    "Perceive the line notation (SMILES, InChI,...) and create the "
+                    "structure from the string '{smiles string}', "
+                )
         else:
-            text = "Create the structure from the SMILES '{smiles string}', "
+            if P["smiles string"][0] == "$":
+                text = (
+                    "Create the structure from the {notation} in the variable"
+                    " '{smiles string}', "
+                )
+            else:
+                text = "Create the structure from the {notation} '{smiles string}', "
 
         handling = P["structure handling"]
         if handling == "Overwrite the current configuration":
             text += "overwriting the current configuration."
         elif handling == "Create a new configuration":
             text += "creating a new configuration for it."
         elif handling == "Create a new system and configuration":
@@ -115,14 +127,16 @@
 
         # Print what we are doing
         printer.important(self.description_text(P))
 
         if P["smiles string"] is None or P["smiles string"] == "":
             return None
 
+        notation = P["notation"]
+
         # Get the system
         system_db = self.get_variable("_system_db")
 
         handling = P["structure handling"]
         if handling == "Overwrite the current configuration":
             system = system_db.system
             if system is None:
@@ -141,36 +155,68 @@
             configuration = system.create_configuration()
         else:
             raise ValueError(
                 f"Do not understand how to handle the structure: '{handling}'"
             )
 
         # Create the structure in the given configuration
-        configuration.from_smiles(P["smiles string"])
+        text = P["smiles string"]
+        if notation == "perceive":
+            if len(text) == 27:
+                tmp = text.split("-")
+                if (
+                    len(tmp) == 3
+                    and len(tmp[0]) == 14
+                    and len(tmp[1]) == 10
+                    and len(tmp[2]) == 1
+                ):
+                    notation = "InChIKey"
+        if notation == "perceive":
+            if text[0:7] == "InChI=":
+                notation = "InChI"
+            else:
+                notation = "SMILES"
+
+        if notation == "SMILES":
+            configuration.from_smiles(text)
+        elif notation == "InChI":
+            configuration.from_inchi(text)
+        elif notation == "InChIKey":
+            configuration.from_inchikey(text)
+        else:
+            raise RuntimeError(f"Can not handle line notation '{text}'")
 
         # Now set the names of the system and configuration, as appropriate.
         name = P["system name"]
         canonical_smiles = None
         if name != "keep current name":
             if name == "use SMILES string":
-                name = P["smiles string"]
+                name = configuration.smiles
             elif name == "use Canonical SMILES string":
                 name = configuration.canonical_smiles
                 canonical_smiles = name
+            elif name == "use InChI":
+                name = configuration.inchi
+            elif name == "use InChIKey":
+                name = configuration.inchikey
             system.name = name
 
         name = P["configuration name"]
         if name != "keep current name":
             if name == "use SMILES string":
                 name = P["smiles string"]
             elif name == "use Canonical SMILES string":
                 if canonical_smiles is None:
                     name = configuration.canonical_smiles
                 else:
                     name = canonical_smiles
+            elif name == "use InChI":
+                name = configuration.inchi
+            elif name == "use InChIKey":
+                name = configuration.inchikey
             configuration.name = name
 
         # Finish the output
         printer.important(
             __(
                 f"\n    Created a molecular structure with {configuration.n_atoms} "
                 "atoms."
```

### Comparing `from_smiles_step-2021.8.4.1/from_smiles_step/from_smiles_step.py` & `from_smiles_step-2023.7.18/from_smiles_step/from_smiles_step.py`

 * *Files identical despite different names*

### Comparing `from_smiles_step-2021.8.4.1/from_smiles_step/tk_from_smiles.py` & `from_smiles_step-2023.7.18/from_smiles_step/tk_from_smiles.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         P = self.node.parameters
         for key in P:
             self[key] = P[key].widget(frame)
 
         widgets = []
         row = 0
         for item in (
+            "notation",
             "smiles string",
             "structure handling",
             "system name",
             "configuration name",
         ):
             self[item].grid(row=row, column=0, columnspan=2, sticky=tk.EW)
             widgets.append(self[item])
```

### Comparing `from_smiles_step-2021.8.4.1/from_smiles_step.egg-info/PKG-INFO` & `from_smiles_step-2023.7.18/from_smiles_step.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: from-smiles-step
-Version: 2021.8.4.1
+Version: 2023.7.18
 Summary: A SEAMM plug-in for creating structures from a SMILES string.
 Home-page: https://github.com/molssi-seamm/from_smiles_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,SMILES,molecule
 Platform: Linux
@@ -12,16 +12,16 @@
 Platform: Unix
 Platform: Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 .. image:: https://img.shields.io/github/issues-pr-raw/molssi-seamm/from_smiles_step
    :target: https://github.com/molssi-seamm/from_smiles_step/pulls
    :alt: GitHub pull requests
@@ -46,14 +46,18 @@
    :target: https://pyup.io/repos/github/molssi-seamm/from_smiles_step/
    :alt: Updates for Dependencies
 
 .. image:: https://img.shields.io/pypi/v/from_smiles_step.svg
    :target: https://pypi.python.org/pypi/from_smiles_step
    :alt: PyPi VERSION
 
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5159800.svg
+   :target: https://doi.org/10.5281/zenodo.5159800
+   :alt: DOI
+
 =========================
 SEAMM From SMILES plug-in
 =========================
 
 A SEAMM plug-in for creating structures from a SMILES string.
 
 This plug-in accepts SMILES_ (Simplified Molecular-Input Line Entry
@@ -81,24 +85,26 @@
 This package was created with Cookiecutter_ and the `molssi-seamm/cookiecutter-seamm-plugin`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`molssi-seamm/cookiecutter-seamm-plugin`: https://github.com/molssi-seamm/cookiecutter-seamm-plugin
 
 Developed by the Molecular Sciences Software Institute (MolSSI_),
 which receives funding from the `National Science Foundation`_ under
-award ACI-1547580
+award OAC-1547580 and CHE-2136142.
 
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
+2023.7.18 -- Added support for InChI and InChIKeys
+
 2021.2.10 (10 February 2021)
 ----------------------------
 
 * Updated the README file to give a better description.
 * Updated the short description in setup.py to work with the new installer.
 * Added keywords for better searchability.
 
@@ -153,9 +159,7 @@
 
 * Internal changes cleaning the code.
   
 0.1.0 (20 January 2018)
 -----------------------
 
 * First release on PyPI.
-
-
```

### Comparing `from_smiles_step-2021.8.4.1/from_smiles_step.egg-info/SOURCES.txt` & `from_smiles_step-2023.7.18/from_smiles_step.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `from_smiles_step-2021.8.4.1/setup.py` & `from_smiles_step-2023.7.18/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,16 +70,16 @@
     keywords=['SEAMM', 'plug-in', 'flowchart', 'SMILES', 'molecule'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
     ],
     entry_points={
         'org.molssi.seamm': [
             'FromSMILESStep = from_smiles_step:FromSMILESStep',
         ],
         'org.molssi.seamm.tk': [
             'FromSMILESStep = from_smiles_step:FromSMILESStep',
```

### Comparing `from_smiles_step-2021.8.4.1/tests/test_from_smiles_step.py` & `from_smiles_step-2023.7.18/tests/test_from_smiles_step.py`

 * *Files identical despite different names*

### Comparing `from_smiles_step-2021.8.4.1/versioneer.py` & `from_smiles_step-2023.7.18/versioneer.py`

 * *Files identical despite different names*

