# Comparing `tmp/chess_tuning_tools-0.9.4.tar.gz` & `tmp/chess_tuning_tools-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess_tuning_tools-0.9.4.tar", max compression
+gzip compressed data, was "chess_tuning_tools-0.9.5.tar", max compression
```

## Comparing `chess_tuning_tools-0.9.4.tar` & `chess_tuning_tools-0.9.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      592 2023-07-19 11:34:31.348552 chess_tuning_tools-0.9.4/LICENSE
--rw-r--r--   0        0        0     2135 2023-07-19 11:34:31.348552 chess_tuning_tools-0.9.4/README.rst
--rw-r--r--   0        0        0     1858 2023-07-19 11:34:31.352552 chess_tuning_tools-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     1056 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/__init__.py
--rw-r--r--   0        0        0    18500 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/cli.py
--rw-r--r--   0        0        0      124 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/db_workers/__init__.py
--rw-r--r--   0        0        0      186 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/db_workers/dbmodels/__init__.py
--rw-r--r--   0        0        0      180 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/db_workers/dbmodels/base_model.py
--rw-r--r--   0        0        0     5906 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/db_workers/dbmodels/models.py
--rw-r--r--   0        0        0    15852 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/db_workers/tuning_client.py
--rw-r--r--   0        0        0    17488 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/db_workers/tuning_server.py
--rw-r--r--   0        0        0     4019 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/db_workers/utils.py
--rw-r--r--   0        0        0     8997 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/io.py
--rw-r--r--   0        0        0    42654 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/local.py
--rw-r--r--   0        0        0    27559 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/plots.py
--rw-r--r--   0        0        0     4785 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/priors.py
--rw-r--r--   0        0        0     2739 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/summary.py
--rw-r--r--   0        0        0     5407 2023-07-19 11:34:31.356552 chess_tuning_tools-0.9.4/tune/utils.py
--rw-r--r--   0        0        0     3726 1970-01-01 00:00:00.000000 chess_tuning_tools-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0      592 2023-07-19 15:48:10.820363 chess_tuning_tools-0.9.5/LICENSE
+-rw-r--r--   0        0        0     2135 2023-07-19 15:48:10.820363 chess_tuning_tools-0.9.5/README.rst
+-rw-r--r--   0        0        0     1854 2023-07-19 15:48:10.824362 chess_tuning_tools-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     1056 2023-07-19 15:48:10.824362 chess_tuning_tools-0.9.5/tune/__init__.py
+-rw-r--r--   0        0        0    18500 2023-07-19 15:48:10.824362 chess_tuning_tools-0.9.5/tune/cli.py
+-rw-r--r--   0        0        0      124 2023-07-19 15:48:10.824362 chess_tuning_tools-0.9.5/tune/db_workers/__init__.py
+-rw-r--r--   0        0        0      186 2023-07-19 15:48:10.824362 chess_tuning_tools-0.9.5/tune/db_workers/dbmodels/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-19 15:48:10.824362 chess_tuning_tools-0.9.5/tune/db_workers/dbmodels/base_model.py
+-rw-r--r--   0        0        0     5906 2023-07-19 15:48:10.824362 chess_tuning_tools-0.9.5/tune/db_workers/dbmodels/models.py
+-rw-r--r--   0        0        0    15852 2023-07-19 15:48:10.824362 chess_tuning_tools-0.9.5/tune/db_workers/tuning_client.py
+-rw-r--r--   0        0        0    17488 2023-07-19 15:48:10.824362 chess_tuning_tools-0.9.5/tune/db_workers/tuning_server.py
+-rw-r--r--   0        0        0     4019 2023-07-19 15:48:10.824362 chess_tuning_tools-0.9.5/tune/db_workers/utils.py
+-rw-r--r--   0        0        0     8997 2023-07-19 15:48:10.824362 chess_tuning_tools-0.9.5/tune/io.py
+-rw-r--r--   0        0        0    42654 2023-07-19 15:48:10.824362 chess_tuning_tools-0.9.5/tune/local.py
+-rw-r--r--   0        0        0    27559 2023-07-19 15:48:10.824362 chess_tuning_tools-0.9.5/tune/plots.py
+-rw-r--r--   0        0        0     4785 2023-07-19 15:48:10.824362 chess_tuning_tools-0.9.5/tune/priors.py
+-rw-r--r--   0        0        0     2739 2023-07-19 15:48:10.824362 chess_tuning_tools-0.9.5/tune/summary.py
+-rw-r--r--   0        0        0     5407 2023-07-19 15:48:10.828361 chess_tuning_tools-0.9.5/tune/utils.py
+-rw-r--r--   0        0        0     3772 1970-01-01 00:00:00.000000 chess_tuning_tools-0.9.5/PKG-INFO
```

### Comparing `chess_tuning_tools-0.9.4/LICENSE` & `chess_tuning_tools-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chess_tuning_tools-0.9.4/README.rst` & `chess_tuning_tools-0.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `chess_tuning_tools-0.9.4/pyproject.toml` & `chess_tuning_tools-0.9.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chess-tuning-tools"
-version = "0.9.4"
+version = "0.9.5"
 description = "A collection of tools for local and distributed tuning of chess engines."
 authors = ["Karlson Pfannschmidt <kiudee@mail.upb.de>"]
 license = "Apache-2.0"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Natural Language :: English"
@@ -14,22 +14,22 @@
 keywords = ["chess", "tuning", "optimization", "engine"]
 documentation = "https://chess-tuning-tools.readthedocs.io"
 packages = [
     {include = "tune"}
 ]
 
 [tool.poetry.dependencies]
-python = "~3.8"
+python = ">=3.8,<3.10"
 bask = ">=0.9.3"
-Click = ">=7.1.2,"
+Click = ">=7.1.2"
 numpy = ">=1.19.1,<1.24"
 scipy = ">=1.5.2"
-scikit-optimize = "^0.8"
+scikit-optimize = "^0.9"
 atomicwrites = ">=1.4.0"
-scikit-learn = ">=0.22,<0.24"
+scikit-learn = "^1"
 dill = ">=0.3.4"
 joblib = {version = ">=0.16.0", optional = true}
 psycopg2 = {version = ">=2.8.5", optional = true}
 sqlalchemy = {version = ">=1.3.18", optional = true}
 pandas = {version = ">=1.1.0", optional = true}
 Sphinx = {version = ">=3", optional = true}
 sphinx-book-theme = {version = ">=0.0.35", optional = true}
@@ -38,15 +38,15 @@
 [tool.poetry.extras]
 dist = ["joblib", "psycopg2", "sqlalchemy", "pandas"]
 docs = ["Sphinx", "sphinx-book-theme", "myst-nb"]
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6.0.1,<8"
 pip = ">=21.1.2"
-wheel = ">=0.34.2,<0.37"
+wheel = ">=0.34.2,<0.39"
 flake8 = ">=3.8.3"
 Sphinx = ">=3"
 black = "~22"
 pre-commit = ">=2.6.0"
 isort = "^5.3.2"
 flake8-bugbear = ">=20.1.4"
 sphinx-book-theme = ">=0.0.35"
```

### Comparing `chess_tuning_tools-0.9.4/tune/__init__.py` & `chess_tuning_tools-0.9.5/tune/__init__.py`

 * *Files identical despite different names*

### Comparing `chess_tuning_tools-0.9.4/tune/cli.py` & `chess_tuning_tools-0.9.5/tune/cli.py`

 * *Files identical despite different names*

### Comparing `chess_tuning_tools-0.9.4/tune/db_workers/dbmodels/models.py` & `chess_tuning_tools-0.9.5/tune/db_workers/dbmodels/models.py`

 * *Files identical despite different names*

### Comparing `chess_tuning_tools-0.9.4/tune/db_workers/tuning_client.py` & `chess_tuning_tools-0.9.5/tune/db_workers/tuning_client.py`

 * *Files identical despite different names*

### Comparing `chess_tuning_tools-0.9.4/tune/db_workers/tuning_server.py` & `chess_tuning_tools-0.9.5/tune/db_workers/tuning_server.py`

 * *Files identical despite different names*

### Comparing `chess_tuning_tools-0.9.4/tune/db_workers/utils.py` & `chess_tuning_tools-0.9.5/tune/db_workers/utils.py`

 * *Files identical despite different names*

### Comparing `chess_tuning_tools-0.9.4/tune/io.py` & `chess_tuning_tools-0.9.5/tune/io.py`

 * *Files identical despite different names*

### Comparing `chess_tuning_tools-0.9.4/tune/local.py` & `chess_tuning_tools-0.9.5/tune/local.py`

 * *Files identical despite different names*

### Comparing `chess_tuning_tools-0.9.4/tune/plots.py` & `chess_tuning_tools-0.9.5/tune/plots.py`

 * *Files identical despite different names*

### Comparing `chess_tuning_tools-0.9.4/tune/priors.py` & `chess_tuning_tools-0.9.5/tune/priors.py`

 * *Files identical despite different names*

### Comparing `chess_tuning_tools-0.9.4/tune/summary.py` & `chess_tuning_tools-0.9.5/tune/summary.py`

 * *Files identical despite different names*

### Comparing `chess_tuning_tools-0.9.4/tune/utils.py` & `chess_tuning_tools-0.9.5/tune/utils.py`

 * *Files identical despite different names*

### Comparing `chess_tuning_tools-0.9.4/PKG-INFO` & `chess_tuning_tools-0.9.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: chess-tuning-tools
-Version: 0.9.4
+Version: 0.9.5
 Summary: A collection of tools for local and distributed tuning of chess engines.
 Home-page: https://github.com/kiudee/chess-tuning-tools
 License: Apache-2.0
 Keywords: chess,tuning,optimization,engine
 Author: Karlson Pfannschmidt
 Author-email: kiudee@mail.upb.de
-Requires-Python: >=3.8,<3.9
+Requires-Python: >=3.8,<3.10
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: dist
 Provides-Extra: docs
 Requires-Dist: Click (>=7.1.2)
 Requires-Dist: Sphinx (>=3) ; extra == "docs"
 Requires-Dist: atomicwrites (>=1.4.0)
 Requires-Dist: bask (>=0.9.3)
 Requires-Dist: dill (>=0.3.4)
 Requires-Dist: joblib (>=0.16.0) ; extra == "dist"
 Requires-Dist: myst-nb (>=0.9) ; extra == "docs"
 Requires-Dist: numpy (>=1.19.1,<1.24)
 Requires-Dist: pandas (>=1.1.0) ; extra == "dist"
 Requires-Dist: psycopg2 (>=2.8.5) ; extra == "dist"
-Requires-Dist: scikit-learn (>=0.22,<0.24)
-Requires-Dist: scikit-optimize (>=0.8,<0.9)
+Requires-Dist: scikit-learn (>=1,<2)
+Requires-Dist: scikit-optimize (>=0.9,<0.10)
 Requires-Dist: scipy (>=1.5.2)
 Requires-Dist: sphinx-book-theme (>=0.0.35) ; extra == "docs"
 Requires-Dist: sqlalchemy (>=1.3.18) ; extra == "dist"
 Project-URL: Bug Tracker, https://github.com/kiudee/chess-tuning-tools/issues
 Project-URL: Documentation, https://chess-tuning-tools.readthedocs.io
 Project-URL: Repository, https://github.com/kiudee/chess-tuning-tools
 Description-Content-Type: text/x-rst
```

