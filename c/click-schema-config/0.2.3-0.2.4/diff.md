# Comparing `tmp/click_schema_config-0.2.3.tar.gz` & `tmp/click_schema_config-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click_schema_config-0.2.3.tar", max compression
+gzip compressed data, was "click_schema_config-0.2.4.tar", max compression
```

## Comparing `click_schema_config-0.2.3.tar` & `click_schema_config-0.2.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0     1069 2023-07-12 10:09:59.473612 click_schema_config-0.2.3/LICENSE
--rwxr-xr-x   0        0        0     5255 2023-07-12 10:09:59.481612 click_schema_config-0.2.3/README.md
--rwxr-xr-x   0        0        0      150 2023-07-12 10:09:59.477612 click_schema_config-0.2.3/click_schema_config/__init__.py
--rwxr-xr-x   0        0        0     2518 2023-07-12 13:08:33.665625 click_schema_config-0.2.3/click_schema_config/click.py
--rw-r--r--   0        0        0     3344 2023-07-12 12:39:05.946883 click_schema_config-0.2.3/click_schema_config/commands/codegen.py
--rw-r--r--   0        0        0       69 2023-07-12 10:09:59.481612 click_schema_config-0.2.3/click_schema_config/commands/templates/__init__.py.jinja
--rw-r--r--   0        0        0      768 2023-07-12 10:09:59.481612 click_schema_config-0.2.3/click_schema_config/commands/templates/dataclass.py.jinja
--rw-r--r--   0        0        0        0 2023-07-12 10:09:59.473612 click_schema_config-0.2.3/click_schema_config/py.typed
--rwxr-xr-x   0        0        0     3585 2023-07-12 10:09:59.481612 click_schema_config-0.2.3/click_schema_config/read_config.py
--rw-r--r--   0        0        0      408 2023-07-12 10:09:59.481612 click_schema_config-0.2.3/click_schema_config/types.py
--rwxr-xr-x   0        0        0      762 2023-07-12 13:09:53.242127 click_schema_config-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     5883 1970-01-01 00:00:00.000000 click_schema_config-0.2.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-07-12 10:09:59.473612 click_schema_config-0.2.4/LICENSE
+-rwxr-xr-x   0        0        0     5255 2023-07-12 10:09:59.481612 click_schema_config-0.2.4/README.md
+-rwxr-xr-x   0        0        0      150 2023-07-12 10:09:59.477612 click_schema_config-0.2.4/click_schema_config/__init__.py
+-rwxr-xr-x   0        0        0     2551 2023-07-13 12:37:29.353520 click_schema_config-0.2.4/click_schema_config/click.py
+-rw-r--r--   0        0        0     3344 2023-07-12 12:39:05.946883 click_schema_config-0.2.4/click_schema_config/commands/codegen.py
+-rw-r--r--   0        0        0       69 2023-07-12 10:09:59.481612 click_schema_config-0.2.4/click_schema_config/commands/templates/__init__.py.jinja
+-rw-r--r--   0        0        0      768 2023-07-12 10:09:59.481612 click_schema_config-0.2.4/click_schema_config/commands/templates/dataclass.py.jinja
+-rw-r--r--   0        0        0        0 2023-07-12 10:09:59.473612 click_schema_config-0.2.4/click_schema_config/py.typed
+-rwxr-xr-x   0        0        0     3585 2023-07-12 10:09:59.481612 click_schema_config-0.2.4/click_schema_config/read_config.py
+-rw-r--r--   0        0        0      408 2023-07-12 10:09:59.481612 click_schema_config-0.2.4/click_schema_config/types.py
+-rwxr-xr-x   0        0        0      762 2023-07-19 08:27:48.805517 click_schema_config-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     5843 1970-01-01 00:00:00.000000 click_schema_config-0.2.4/PKG-INFO
```

### Comparing `click_schema_config-0.2.3/LICENSE` & `click_schema_config-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `click_schema_config-0.2.3/README.md` & `click_schema_config-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `click_schema_config-0.2.3/click_schema_config/click.py` & `click_schema_config-0.2.4/click_schema_config/click.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 
 FC = Callable[..., Any]
 
 
 def schema_from_inis(
     files: list[FileLike] | FileLike = ["config.default.ini", "config.ini"],
     insecure_eval: bool = False,
-    **kwargs: Any,
+    **kwargs: Any,  # type: ignore[return-value]
 ) -> "IdentityFunction":
     """Decorate a click command to load options from a config file.
 
     Parameters
     ----------
-    filenames : list[FileLike] | files, optional
+    filenames : list[FileLike] | FileLike, optional
         List of files (either open file-pointers or filenames) to load, by default ["config.default.ini", "config.ini"]
     insecure_eval : bool, optional
         Whether or not to allow arbitrary code execution, by default False
     **kwargs : Any
         Passed to click.option
     """
```

### Comparing `click_schema_config-0.2.3/click_schema_config/commands/codegen.py` & `click_schema_config-0.2.4/click_schema_config/commands/codegen.py`

 * *Files identical despite different names*

### Comparing `click_schema_config-0.2.3/click_schema_config/commands/templates/dataclass.py.jinja` & `click_schema_config-0.2.4/click_schema_config/commands/templates/dataclass.py.jinja`

 * *Files identical despite different names*

### Comparing `click_schema_config-0.2.3/click_schema_config/read_config.py` & `click_schema_config-0.2.4/click_schema_config/read_config.py`

 * *Files identical despite different names*

### Comparing `click_schema_config-0.2.3/pyproject.toml` & `click_schema_config-0.2.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "click-schema-config"
-version = "0.2.3"
+version = "0.2.4"
 description = ""
 authors = ["Joy Void Joy <joy.void.joy@gmail.com>"]
 readme = "README.md"
 packages = [{include = "click_schema_config"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.4"
 pyyaml = "^6.0"
 pydantic = "^2.0.2"
 jinja2 = "^3.1.2"
-black = {version = "^22.8.0", allow-prereleases = true}
 halo = "^0.0.31"
 types-click = "^7.1.8" # not dev-dependency because having types-click fixes the types
 
 [tool.poetry.group.dev.dependencies]
+black = {version = "^22.8.0", allow-prereleases = true}
 mypy = "^1.4.1"
 ipython = "^8.14.0"
 halo = "^0.0.31"
 types-pyyaml = "^6.0.12.10"
 
 [tool.poetry.scripts]
 codegen-ini = "click_schema_config.commands.codegen:codegen"
```

### Comparing `click_schema_config-0.2.3/PKG-INFO` & `click_schema_config-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: click-schema-config
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Author: Joy Void Joy
 Author-email: joy.void.joy@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: black (>=22.8.0,<23.0.0)
 Requires-Dist: click (>=8.1.4,<9.0.0)
 Requires-Dist: halo (>=0.0.31,<0.0.32)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pydantic (>=2.0.2,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: types-click (>=7.1.8,<8.0.0)
 Description-Content-Type: text/markdown
```

