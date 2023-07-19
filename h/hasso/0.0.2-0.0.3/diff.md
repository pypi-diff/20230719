# Comparing `tmp/hasso-0.0.2.tar.gz` & `tmp/hasso-0.0.3.tar.gz`

## Comparing `hasso-0.0.2.tar` & `hasso-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 hasso-0.0.2/.DS_Store
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 hasso-0.0.2/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hasso-0.0.2/requirements.txt
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 hasso-0.0.2/src/__init__.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 hasso-0.0.2/src/file_format/csv_format.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hasso-0.0.2/src/file_format/tsv_format.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hasso-0.0.2/src/table/__init__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 hasso-0.0.2/src/table/table.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hasso-0.0.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 hasso-0.0.2/LICENSE
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 hasso-0.0.2/README.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 hasso-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 hasso-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 hasso-0.0.3/Makefile
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hasso-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 hasso-0.0.3/src/hasso/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hasso-0.0.3/src/hasso/file_format/__init__.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 hasso-0.0.3/src/hasso/file_format/csv_format.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hasso-0.0.3/src/hasso/table/__init__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 hasso-0.0.3/src/hasso/table/table.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hasso-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 hasso-0.0.3/LICENSE
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 hasso-0.0.3/README.md
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 hasso-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 hasso-0.0.3/PKG-INFO
```

### Comparing `hasso-0.0.2/.gitignore` & `hasso-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `hasso-0.0.2/LICENSE` & `hasso-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hasso-0.0.2/pyproject.toml` & `hasso-0.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "hasso"
-version = "0.0.2"
+description = "A simple library for data analysis"
+version = "0.0.3"
 authors = [
   { name="Kaiming Tao", email="mads396@gmail.com" },
 ]
-description = "Python library"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `hasso-0.0.2/PKG-INFO` & `hasso-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hasso
-Version: 0.0.2
-Summary: Python library
+Version: 0.0.3
+Summary: A simple library for data analysis
 Project-URL: Homepage, https://github.com/KaimingTao/hasso
 Project-URL: Bug Tracker, https://github.com/KaimingTao/hasso/issues
 Author-email: Kaiming Tao <mads396@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

