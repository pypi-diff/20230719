# Comparing `tmp/anoexpress-0.1.6.tar.gz` & `tmp/anoexpress-0.1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anoexpress-0.1.6.tar", max compression
+gzip compressed data, was "anoexpress-0.1.7.1.tar", max compression
```

## Comparing `anoexpress-0.1.6.tar` & `anoexpress-0.1.7.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1075 2022-11-12 23:31:02.745561 anoexpress-0.1.6/LICENSE
--rw-r--r--   0        0        0       66 2023-03-06 23:08:43.188006 anoexpress-0.1.6/anoexpress/__init__.py
--rw-r--r--   0        0        0    38048 2023-05-11 14:40:55.533855 anoexpress-0.1.6/anoexpress/anoexpress.py
--rw-r--r--   0        0        0      786 2023-05-11 14:41:46.593855 anoexpress-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      891 1970-01-01 00:00:00.000000 anoexpress-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1075 2022-11-12 23:31:02.745561 anoexpress-0.1.7.1/LICENSE
+-rw-r--r--   0        0        0       66 2023-03-06 23:08:43.188006 anoexpress-0.1.7.1/anoexpress/__init__.py
+-rw-r--r--   0        0        0    38080 2023-07-19 15:13:08.054363 anoexpress-0.1.7.1/anoexpress/anoexpress.py
+-rw-r--r--   0        0        0      788 2023-07-19 15:14:22.951063 anoexpress-0.1.7.1/pyproject.toml
+-rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 anoexpress-0.1.7.1/PKG-INFO
```

### Comparing `anoexpress-0.1.6/LICENSE` & `anoexpress-0.1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anoexpress-0.1.6/anoexpress/anoexpress.py` & `anoexpress-0.1.7.1/anoexpress/anoexpress.py`

 * *Files 1% similar despite different names*

```diff
@@ -805,15 +805,16 @@
         active_drag="xpan",
         sizing_mode=sizing_mode,
         width=width,
         height=height,
         toolbar_location="above",
         tooltips=tooltips,
         x_range=x_range,
-        y_range=y_range
+        y_range=y_range,
+        output_backend='webgl'
     )
 
     # plot 
     fig.circle(
         x="midpoint",
         y="fold_change",
         size=4,
```

### Comparing `anoexpress-0.1.6/pyproject.toml` & `anoexpress-0.1.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anoexpress"
-version = "0.1.6"
+version = "0.1.7.1"
 description = "A package to access insecticide resistance gene expression meta analyse in Anopheles mosquitoes"
 authors = [
     "Sanjay Nagi <sanjay.nagi@lstmed.ac.uk>",
     ]
 packages = [
     { include = "anoexpress" }
 ]
```

### Comparing `anoexpress-0.1.6/PKG-INFO` & `anoexpress-0.1.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anoexpress
-Version: 0.1.6
+Version: 0.1.7.1
 Summary: A package to access insecticide resistance gene expression meta analyse in Anopheles mosquitoes
 License: MIT
 Author: Sanjay Nagi
 Author-email: sanjay.nagi@lstmed.ac.uk
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

