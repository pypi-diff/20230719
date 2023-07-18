# Comparing `tmp/namespace_mahdimir-2.4.1.tar.gz` & `tmp/namespace_mahdimir-2.5.0.tar.gz`

## Comparing `namespace_mahdimir-2.4.1.tar` & `namespace_mahdimir-2.5.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.1/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.1/src/namespace_mahdimir/__init__.py
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.1/src/namespace_mahdimir/tse.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.1/src/namespace_mahdimir/tse_github_data_url.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.1/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.1/README.md
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.1/pyproject.toml
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 namespace_mahdimir-2.5.0/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namespace_mahdimir-2.5.0/src/namespace_mahdimir/__init__.py
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 namespace_mahdimir-2.5.0/src/namespace_mahdimir/tse.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 namespace_mahdimir-2.5.0/src/namespace_mahdimir/tse_github_data_url.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 namespace_mahdimir-2.5.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 namespace_mahdimir-2.5.0/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namespace_mahdimir-2.5.0/README.md
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 namespace_mahdimir-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 namespace_mahdimir-2.5.0/PKG-INFO
```

### Comparing `namespace_mahdimir-2.4.1/src/namespace_mahdimir/tse.py` & `namespace_mahdimir-2.5.0/src/namespace_mahdimir/tse.py`

 * *Files identical despite different names*

### Comparing `namespace_mahdimir-2.4.1/src/namespace_mahdimir/tse_github_data_url.py` & `namespace_mahdimir-2.5.0/src/namespace_mahdimir/tse_github_data_url.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,12 +14,13 @@
     codal_tics_2_ftics = 'CodalTicker-2-FirmTicker'
     adj_price = 'Adj-Price'
     tse_work_days = 'TSE-Work-Days'
     adj_ret = 'Adj-Ret'
     tedpix = 'TEDPIX'
     nom_price = 'Nominal-Price'
     id_2_ftic = 'TSETMC_ID-2-FirmTicker'
+    os = 'Outstanding-Shares'
 
     def __init__(self) :
         for ky , vl in vars(GitHubDataUrl).items() :
             if not ky.startswith('_') :
                 setattr(self , ky , m + 'd-' + vl)
```

### Comparing `namespace_mahdimir-2.4.1/.gitignore` & `namespace_mahdimir-2.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `namespace_mahdimir-2.4.1/LICENSE` & `namespace_mahdimir-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `namespace_mahdimir-2.4.1/pyproject.toml` & `namespace_mahdimir-2.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "namespace_mahdimir"
-version = "2.4.1"
+version = "2.5.0"
 authors = [{ name = "Mahdi Mir", email = "imahdimir@gmail.com" }]
 description = "Some Namespaces for Python"
 readme = "README.md"
 license = { file = "LICENSE" }
 dependencies = [
 
 ]
```

### Comparing `namespace_mahdimir-2.4.1/PKG-INFO` & `namespace_mahdimir-2.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: namespace_mahdimir
-Version: 2.4.1
+Version: 2.5.0
 Summary: Some Namespaces for Python
 Project-URL: Homepage, https://github.com/imahdimir/namespace_mahdimir
 Project-URL: Bug Tracker, https://github.com/imahdimir/namespace_mahdimir/issues
 Author-email: Mahdi Mir <imahdimir@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Mahdi
```

