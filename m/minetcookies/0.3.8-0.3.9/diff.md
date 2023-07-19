# Comparing `tmp/minetcookies-0.3.8.tar.gz` & `tmp/minetcookies-0.3.9.tar.gz`

## Comparing `minetcookies-0.3.8.tar` & `minetcookies-0.3.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 minetcookies-0.3.8/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 minetcookies-0.3.8/src/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 minetcookies-0.3.8/src/minetcookies/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 minetcookies-0.3.8/src/minetcookies/__init__.py
--rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 minetcookies-0.3.8/src/minetcookies/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 minetcookies-0.3.8/tests/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 minetcookies-0.3.8/.gitignore
--rw-r--r--   0        0        0    34503 2020-02-02 00:00:00.000000 minetcookies-0.3.8/LICENSE.txt
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 minetcookies-0.3.8/README.md
--rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 minetcookies-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 minetcookies-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 minetcookies-0.3.9/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 minetcookies-0.3.9/src/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 minetcookies-0.3.9/src/minetcookies/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 minetcookies-0.3.9/src/minetcookies/__init__.py
+-rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 minetcookies-0.3.9/src/minetcookies/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 minetcookies-0.3.9/tests/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 minetcookies-0.3.9/.gitignore
+-rw-r--r--   0        0        0    34503 2020-02-02 00:00:00.000000 minetcookies-0.3.9/LICENSE.txt
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 minetcookies-0.3.9/README.md
+-rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 minetcookies-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 minetcookies-0.3.9/PKG-INFO
```

### Comparing `minetcookies-0.3.8/src/minetcookies/main.py` & `minetcookies-0.3.9/src/minetcookies/main.py`

 * *Files identical despite different names*

### Comparing `minetcookies-0.3.8/LICENSE.txt` & `minetcookies-0.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `minetcookies-0.3.8/README.md` & `minetcookies-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `minetcookies-0.3.8/pyproject.toml` & `minetcookies-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     "Programming Language :: Python :: Implementation :: PyPy",
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "minet~=0.67.1",
     "PyYAML~=6.0",
+    "tqdm~=2.2.0",
 ]
 
 
 [project.urls]
 Documentation = "https://github.com/Marceau-h/minetcookies#readme"
 Issues = "https://github.com/Marceau-h/minetcookies/issues"
 Source = "https://github.com/Marceau-h/minetcookies"
```

### Comparing `minetcookies-0.3.8/PKG-INFO` & `minetcookies-0.3.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minetcookies
-Version: 0.3.8
+Version: 0.3.9
 Summary: A simple cookie manager for Minet by Medialab
 Project-URL: Documentation, https://github.com/Marceau-h/minetcookies#readme
 Project-URL: Issues, https://github.com/Marceau-h/minetcookies/issues
 Project-URL: Source, https://github.com/Marceau-h/minetcookies
 Author-email: Marceau-h <106751184+Marceau-h@users.noreply.github.com>
 Maintainer-email: Marceau-h <106751184+Marceau-h@users.noreply.github.com>
 License-Expression: AGPL-3.0-or-later
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: minet~=0.67.1
 Requires-Dist: pyyaml~=6.0
+Requires-Dist: tqdm~=2.2.0
 Description-Content-Type: text/markdown
 
 # minetcookies
 
 [![PyPI - Version](https://img.shields.io/pypi/v/minetcookies.svg)](https://pypi.org/project/minetcookies)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/minetcookies.svg)](https://pypi.org/project/minetcookies)
```

