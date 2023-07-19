# Comparing `tmp/flake8-complicated-walrus-2.0.0.tar.gz` & `tmp/flake8_complicated_walrus-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-complicated-walrus-2.0.0.tar", max compression
+gzip compressed data, was "flake8_complicated_walrus-2.1.0.tar", max compression
```

## Comparing `flake8-complicated-walrus-2.0.0.tar` & `flake8_complicated_walrus-2.1.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1070 2022-05-06 06:20:01.638300 flake8-complicated-walrus-2.0.0/LICENSE
--rw-r--r--   0        0        0      993 2022-06-06 11:45:17.182121 flake8-complicated-walrus-2.0.0/README.md
--rw-r--r--   0        0        0     3705 2022-06-06 07:09:56.612491 flake8-complicated-walrus-2.0.0/flake8_complicated_walrus.py
--rw-r--r--   0        0        0     1682 2022-06-06 12:09:25.910763 flake8-complicated-walrus-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1834 2022-06-06 12:09:33.229256 flake8-complicated-walrus-2.0.0/setup.py
--rw-r--r--   0        0        0     2144 2022-06-06 12:09:33.229517 flake8-complicated-walrus-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-05-06 06:20:01.638300 flake8_complicated_walrus-2.1.0/LICENSE
+-rw-r--r--   0        0        0      993 2022-06-06 11:45:17.182121 flake8_complicated_walrus-2.1.0/README.md
+-rw-r--r--   0        0        0     3721 2023-07-19 12:58:28.623428 flake8_complicated_walrus-2.1.0/flake8_complicated_walrus.py
+-rw-r--r--   0        0        0     2231 2023-07-19 13:19:43.110413 flake8_complicated_walrus-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2033 1970-01-01 00:00:00.000000 flake8_complicated_walrus-2.1.0/PKG-INFO
```

### Comparing `flake8-complicated-walrus-2.0.0/LICENSE` & `flake8_complicated_walrus-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-complicated-walrus-2.0.0/README.md` & `flake8_complicated_walrus-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `flake8-complicated-walrus-2.0.0/flake8_complicated_walrus.py` & `flake8_complicated_walrus-2.1.0/flake8_complicated_walrus.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,11 +93,11 @@
     def __init__(self, tree: ast.AST) -> None:
         self._tree = tree
 
     def run(self) -> Generator[tuple[int, int, str, Type[Any]], None, None]:
         """
         Any module from specified package could not be import in another package
         """
-        visitor = Visitor(self._restrict_walrus_level)
+        visitor = Visitor(self._restrict_walrus_level)  # type: ignore
         visitor.visit(self._tree)
         for line, col, msg in visitor.errors:
             yield line, col, msg, type(self)
```

### Comparing `flake8-complicated-walrus-2.0.0/pyproject.toml` & `flake8_complicated_walrus-2.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,78 @@
 [tool.poetry]
 name = "flake8-complicated-walrus"
-version = "2.0.0"
+version = "2.1.0"
 license = "MIT"
 description = "This Flake8 plugin for checking complicated assignment expressions."
 authors = ["Dudov Dmitry <dudov.dm@gmail.com>"]
 readme = "README.md"
 keywords = ["flake8-complicated-walrus", "flake8", "plugin", "walrus", "assignment expression", "if", "conditions"]
 repository = "https://github.com/DDmitiy/flake8-complicated-walrus"
 classifiers=[
     "Framework :: Flake8",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.5",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Quality Assurance",
 ]
 
 [tool.poetry.plugins]
 [tool.poetry.plugins."flake8.extension"]
 FCW = "flake8_complicated_walrus:Plugin"
 
 [tool.black]
 line-length = 120
 
 [tool.poetry.dependencies]
-python = "^3.7"
-flake8 = "^3"
-astpretty = "^2.1.0"
-
-[tool.poetry.dev-dependencies]
-pytest = "^6.2.2"
-twine = "^3.4.1"
-black = "^22.3.0"
-flake8-builtins = "^1.5.3"
-flake8-comprehensions = "^3.10.0"
-flake8-eradicate = "^1.2.1"
-flake8-isort = "^4.1.1"
-flake8-logging-format = "^0.6.0"
+python = "^3.9"
+flake8 = "*"
+astpretty = "^3.0"
+
+[tool.poetry.group.dev.dependencies]
+autoflake = "^1.4"
+pytest = "^7.4"
+black = "^23.7"
+twine = "^4.0"
+flake8-builtins = "^2.1"
+flake8-comprehensions = "^3.14"
+flake8-eradicate = "^1.5"
+flake8-isort = "^6.0"
+flake8-logging-format = "^0.9"
 flake8-print = "^5.0.0"
-flake8-pytest = "^1.3"
-flake8-pytest-style = "^1.6.0"
-flake8-quotes = "^3.3.1"
-flake8-return = "^1.1.3"
-isort = "^5.10.1"
-mypy = "^0.950"
-pep8-naming = "^0.12.1"
-pylint = "^2.13.9"
-pytest-asyncio = "^0.18.3"
-pytest-cov = "^3.0.0"
+flake8-pytest = "^1.4"
+flake8-pytest-style = "^1.7"
+flake8-quotes = "^3.3"
+flake8-return = "^1.2"
+isort = "^5.12"
+mypy = "^1.4"
+pep8-naming = "^0.13"
+pylint = "^2.17"
+pytest-asyncio = "^0.21"
+pytest-cov = "^4.1"
 pytest-deadfixtures = "^2.2.1"
 pytest-lazy-fixture = "^0.6.3"
-pytest-mock = "^3.7.0"
+pytest-mock = "^3.11"
+unify = "^0.5"
+
+[tool.isort]
+balanced_wrapping=true
+default_section="THIRDPARTY"
+include_trailing_comma=true
+known_first_party="tests"
+line_length=88
+multi_line_output=3
+
+[tool.pylint]
+max-args = 5
+output-format = "colorized"
+max-line-length=120
+disable = [
+    "C0103", # Attribute name doesn't conform to snake_case naming style (invalid-name)
+    "C0114", # Missing module docstring (missing-docstring)
+    "C0115", # Missing class docstring (missing-class-docstring)
+    "C0116", # Missing function or method docstring (missing-function-docstring)
+    "C0301", # Line too long (m/n) (line-too-long)
+]
```

### Comparing `flake8-complicated-walrus-2.0.0/PKG-INFO` & `flake8_complicated_walrus-2.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: flake8-complicated-walrus
-Version: 2.0.0
+Version: 2.1.0
 Summary: This Flake8 plugin for checking complicated assignment expressions.
 Home-page: https://github.com/DDmitiy/flake8-complicated-walrus
 License: MIT
 Keywords: flake8-complicated-walrus,flake8,plugin,walrus,assignment expression,if,conditions
 Author: Dudov Dmitry
 Author-email: dudov.dm@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Framework :: Flake8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
-Requires-Dist: astpretty (>=2.1.0,<3.0.0)
-Requires-Dist: flake8 (>=3,<4)
+Requires-Dist: astpretty (>=3.0,<4.0)
+Requires-Dist: flake8
 Project-URL: Repository, https://github.com/DDmitiy/flake8-complicated-walrus
 Description-Content-Type: text/markdown
 
 # flake8-complicated-walrus
 
 This *Flake8* plugin for checking complicated assignment expressions.
 There are 3 levels for this linter:
```

