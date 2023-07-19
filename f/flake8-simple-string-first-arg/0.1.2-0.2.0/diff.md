# Comparing `tmp/flake8_simple_string_first_arg-0.1.2.tar.gz` & `tmp/flake8_simple_string_first_arg-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_simple_string_first_arg-0.1.2.tar", max compression
+gzip compressed data, was "flake8_simple_string_first_arg-0.2.0.tar", max compression
```

## Comparing `flake8_simple_string_first_arg-0.1.2.tar` & `flake8_simple_string_first_arg-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2023-01-16 12:31:57.213344 flake8_simple_string_first_arg-0.1.2/LICENSE
--rw-r--r--   0        0        0     1163 2023-01-16 14:33:22.508500 flake8_simple_string_first_arg-0.1.2/README.md
--rw-r--r--   0        0        0     5486 2023-01-16 10:49:43.873000 flake8_simple_string_first_arg-0.1.2/flake8_simple_string_first_arg.py
--rw-r--r--   0        0        0     1664 2023-01-16 14:42:30.904131 flake8_simple_string_first_arg-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1958 1970-01-01 00:00:00.000000 flake8_simple_string_first_arg-0.1.2/setup.py
--rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 flake8_simple_string_first_arg-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-01-16 12:31:57.213344 flake8_simple_string_first_arg-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1163 2023-01-16 14:33:22.508500 flake8_simple_string_first_arg-0.2.0/README.md
+-rw-r--r--   0        0        0     5486 2023-07-19 15:04:39.775755 flake8_simple_string_first_arg-0.2.0/flake8_simple_string_first_arg.py
+-rw-r--r--   0        0        0     2061 2023-07-19 14:58:26.256703 flake8_simple_string_first_arg-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1958 1970-01-01 00:00:00.000000 flake8_simple_string_first_arg-0.2.0/setup.py
+-rw-r--r--   0        0        0     2246 1970-01-01 00:00:00.000000 flake8_simple_string_first_arg-0.2.0/PKG-INFO
```

### Comparing `flake8_simple_string_first_arg-0.1.2/LICENSE` & `flake8_simple_string_first_arg-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_simple_string_first_arg-0.1.2/README.md` & `flake8_simple_string_first_arg-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `flake8_simple_string_first_arg-0.1.2/flake8_simple_string_first_arg.py` & `flake8_simple_string_first_arg-0.2.0/flake8_simple_string_first_arg.py`

 * *Files identical despite different names*

### Comparing `flake8_simple_string_first_arg-0.1.2/pyproject.toml` & `flake8_simple_string_first_arg-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,61 +1,73 @@
 [tool.poetry]
 name = "flake8-simple-string-first-arg"
-version = "0.1.2"
+version = "0.2.0"
 license = "MIT"
 description = "This Flake8 plugin for checking that first param of callable is simple string."
 authors = ["Kozyar Valeriy <monqpepers@gmail.com>"]
 readme = "README.md"
 keywords = ["flake8-simple-string-first-arg", "flake8", "plugin", "simple string", "first arg", "simple first arg"]
 
 classifiers=[
     "Framework :: Flake8",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Quality Assurance",
 ]
 
 [tool.poetry.plugins]
 [tool.poetry.plugins."flake8.extension"]
 SFA = "flake8_simple_string_first_arg:Plugin"
 
-[tool.black]
-line-length = 120
-
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 flake8 = "*"
 
-[tool.poetry.dev-dependencies]
-autoflake = "^1"
-black = "^22.12.0"
-flake8-builtins = "^2.1.0"
-flake8-comprehensions = "^3.10.1"
-flake8-eradicate = "^1.4.0"
-flake8-isort = "^6.0.0"
-flake8-print = "^5.0.0"
+[tool.poetry.group.dev.dependencies]
+astpretty = "^3.0"
+autoflake = "^2.2"
+black = "^23.7"
+flake8-builtins = "^2.1"
+flake8-comprehensions = "^3.14"
+flake8-eradicate = "^1.5"
+flake8-isort = "^6.0"
+flake8-print = "^5.0"
 flake8-pytest = "^1.4"
-flake8-pytest-style = "^1.6.0"
-flake8-quotes = "^3.3.2"
-flake8-return = "^1.2.0"
-isort = "^5.11.4"
-mypy = "^0.991"
+flake8-pytest-style = "^1.7"
+flake8-quotes = "^3.3"
+flake8-return = "^1.2"
+isort = "^5.12"
+mypy = "^1.4"
 pep8-naming = "^0.12"
-pylint = "^2.15.10"
-pytest = "^7.2.1"
-pytest-cov = "^4.0.0"
-pytest-deadfixtures = "^2.2.1"
+pylint = "^2.17"
+pytest = "^7.2"
+pytest-cov = "^4.1"
+pytest-deadfixtures = "^2.2"
 unify = "^0.5"
 
+[tool.black]
+line-length = 120
+
+[tool.isort]
+balanced_wrapping=true
+default_section="THIRDPARTY"
+include_trailing_comma=true
+known_first_party="tests"
+line_length=88
+multi_line_output=3
 
 [tool.pylint]
 max-args = 5
 output-format = "colorized"
 max-line-length=120
 disable = [
+    "C0103", # Attribute name doesn't conform to snake_case naming style (invalid-name)
     "C0114", # Missing module docstring (missing-docstring)
     "C0115", # Missing class docstring (missing-class-docstring)
     "C0116", # Missing function or method docstring (missing-function-docstring)
-    "C0103", # invalid-name
+    "C0301", # Line too long (m/n) (line-too-long)
 ]
```

### Comparing `flake8_simple_string_first_arg-0.1.2/setup.py` & `flake8_simple_string_first_arg-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 ['flake8']
 
 entry_points = \
 {'flake8.extension': ['SFA = flake8_simple_string_first_arg:Plugin']}
 
 setup_kwargs = {
     'name': 'flake8-simple-string-first-arg',
-    'version': '0.1.2',
+    'version': '0.2.0',
     'description': 'This Flake8 plugin for checking that first param of callable is simple string.',
     'long_description': '# flake8-simple-string-first-arg\n\nThis *Flake8* plugin for checking that first param of callable object is simple string. \nPlugin will check for specified callable objects that \nit is not allowed to use f-sting, .format method, string concat and % statement for first parameter\n\n# Quick Start Guide\n\n1. Install ``flake8-simple-string-first-arg`` from PyPI with pip:\n\n        pip install flake8-simple-string-first-arg\n\n2. Configure a mark that you would like to validate:\n\n        cd project_root/\n        vi setup.cfg\n\n3. Add to file following: \n   \n        [flake8]  \n        simple-string-first-arg = SomeClassName, OtherClassName:url\n\n3. Run flake8::\n\n        flake8 .\n\n# flake8 codes\n\n   * SFA100: In calling {CallableName} f-string is used\n   * SFA200: In calling {CallableName} string.format() is used\n   * SFA300: In calling {CallableName} string concatenation ("+") is used\n   * SFA400: In calling {CallableName} "%" is used\n\n# Settings\n\n**simple-string-first-arg**  \nIt specifies a list of name of callable objects, that should have simple string as first arg.\nYou can add the name of the argument via `:` to check if it is passed as a named parameter.\n',
     'author': 'Kozyar Valeriy',
     'author_email': 'monqpepers@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'py_modules': modules,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `flake8_simple_string_first_arg-0.1.2/PKG-INFO` & `flake8_simple_string_first_arg-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: flake8-simple-string-first-arg
-Version: 0.1.2
+Version: 0.2.0
 Summary: This Flake8 plugin for checking that first param of callable is simple string.
 License: MIT
 Keywords: flake8-simple-string-first-arg,flake8,plugin,simple string,first arg,simple first arg
 Author: Kozyar Valeriy
 Author-email: monqpepers@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Framework :: Flake8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Dist: flake8
 Description-Content-Type: text/markdown
 
 # flake8-simple-string-first-arg
```

