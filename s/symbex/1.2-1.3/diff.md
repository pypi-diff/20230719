# Comparing `tmp/symbex-1.2.tar.gz` & `tmp/symbex-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbex-1.2.tar", last modified: Sun Jul 16 16:55:50 2023, max compression
+gzip compressed data, was "symbex-1.3.tar", last modified: Wed Jul 19 01:52:09 2023, max compression
```

## Comparing `symbex-1.2.tar` & `symbex-1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:55:50.441049 symbex-1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-16 16:55:34.000000 symbex-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17913 2023-07-16 16:55:50.441049 symbex-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17417 2023-07-16 16:55:34.000000 symbex-1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 16:55:50.441049 symbex-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-16 16:55:34.000000 symbex-1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:55:50.437049 symbex-1.2/symbex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 16:55:34.000000 symbex-1.2/symbex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-16 16:55:34.000000 symbex-1.2/symbex/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13881 2023-07-16 16:55:34.000000 symbex-1.2/symbex/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11434 2023-07-16 16:55:34.000000 symbex-1.2/symbex/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:55:50.441049 symbex-1.2/symbex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17913 2023-07-16 16:55:50.000000 symbex-1.2/symbex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-16 16:55:50.000000 symbex-1.2/symbex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 16:55:50.000000 symbex-1.2/symbex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-16 16:55:50.000000 symbex-1.2/symbex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-16 16:55:50.000000 symbex-1.2/symbex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-16 16:55:50.000000 symbex-1.2/symbex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:55:50.441049 symbex-1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-07-16 16:55:34.000000 symbex-1.2/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-16 16:55:34.000000 symbex-1.2/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-16 16:55:34.000000 symbex-1.2/tests/test_replace.py
--rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-16 16:55:34.000000 symbex-1.2/tests/test_symbex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-07-16 16:55:34.000000 symbex-1.2/tests/test_symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 01:52:09.262379 symbex-1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-19 01:51:54.000000 symbex-1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19020 2023-07-19 01:52:09.262379 symbex-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18524 2023-07-19 01:51:54.000000 symbex-1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 01:52:09.262379 symbex-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-19 01:51:54.000000 symbex-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 01:52:09.258379 symbex-1.3/symbex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 01:51:54.000000 symbex-1.3/symbex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-19 01:51:54.000000 symbex-1.3/symbex/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14974 2023-07-19 01:51:54.000000 symbex-1.3/symbex/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11434 2023-07-19 01:51:54.000000 symbex-1.3/symbex/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 01:52:09.258379 symbex-1.3/symbex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19020 2023-07-19 01:52:09.000000 symbex-1.3/symbex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-19 01:52:09.000000 symbex-1.3/symbex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 01:52:09.000000 symbex-1.3/symbex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-19 01:52:09.000000 symbex-1.3/symbex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-19 01:52:09.000000 symbex-1.3/symbex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-19 01:52:09.000000 symbex-1.3/symbex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 01:52:09.262379 symbex-1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-07-19 01:51:54.000000 symbex-1.3/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-19 01:51:54.000000 symbex-1.3/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-19 01:51:54.000000 symbex-1.3/tests/test_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-19 01:51:54.000000 symbex-1.3/tests/test_symbex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-07-19 01:51:54.000000 symbex-1.3/tests/test_symbols.py
```

### Comparing `symbex-1.2/LICENSE` & `symbex-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `symbex-1.2/PKG-INFO` & `symbex-1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbex
-Version: 1.2
+Version: 1.3
 Summary: Find the Python code for specified symbols
 Home-page: https://github.com/simonw/symbex
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/symbex/issues
 Project-URL: CI, https://github.com/simonw/symbex/actions
 Project-URL: Changelog, https://github.com/simonw/symbex/releases
@@ -111,14 +111,17 @@
 
 - `--function` - only functions
 - `--class` - only classes
 - `--async` - only `async def` functions
 - `--unasync` - only non-async functions
 - `--documented` - functions/classes that have a docstring
 - `--undocumented` - functions/classes that do not have a docstring
+- `--public` - functions/classes that are public - don't have a `_name` prefix (or are `__*__` methods)
+- `--private` - functions/classes that are private - have a `_name` prefix and are not `__*__`
+- `--dunder` - functions matching `__*__` - this should usually be used with `*.*` to find all dunder methods
 - `--typed` - functions that have at least one type annotation
 - `--untyped` - functions that have no type annotations
 - `--partially-typed` - functions that have some type annotations but not all
 - `--fully-typed` - functions that have type annotations for every argument and the return value
 - `--no-init` - Exclude `__init__(self)` methods. This is useful when combined with `--fully-typed '*.*'` to avoid returning `__init__(self)` methods that would otherwise be classified as fully typed, since `__init__` doesn't need argument or return type annotations.
 
 For example, to see the signatures of every `async def` function in your project that doesn't have any type annotations:
@@ -131,14 +134,20 @@
 
 This example shows the full source code of every class method in the Python standard library that has type annotations for all of the arguments and the return value:
 
 ```bash
 symbex --fully-typed --no-init '*.*' --stdlib
 ```
 
+To find all public functions and methods that lack documentation, just showing the signature of each one:
+
+```bash
+symbex '*' '*.*' --public --undocumented --signatures
+```
+
 ### Example output
 
 In a fresh checkout of [Datasette](https://github.com/simonw/datasette) I ran this command:
 
 ```bash
 symbex MessagesDebugView get_long_description
 ```
@@ -395,22 +404,32 @@
     """
     return a + b + 3
 ```
 ## Using in CI
 
 The `--check` option causes `symbex` to return a non-zero exit code if any matches are found for your query.
 
-You can use this in CI to guard against things like functions being added without documentation:
+You can use this in CI to guard against things like public functions being added without documentation:
 
 ```bash
-symbex --function --undocumented --check
+symbex --function --public --undocumented --check
 ```
 This will fail silently but set a `1` exit code if there are any undocumented functions.
 
-`--check` will not output anything by default. Add `--count` to output a count of matching symbols, or `-s/--signatures` to output the signatures of the matching symbols.
+Using this as a step in a CI tool such as GitHub Actions should result in a test failure.
+
+Run this to see the exit code from the last command:
+```bash
+echo $?
+```
+
+`--check` will not output anything by default. Add `--count` to output a count of matching symbols, or `-s/--signatures` to output the signatures of the matching symbols, for example:
+```bash
+symbex --function --public --undocumented --check --count
+```
 
 ## Similar tools
 
 - [pyastgrep](https://github.com/spookylukey/pyastgrep) by Luke Plant offers advanced capabilities for viewing and searching through Python ASTs using XPath.
 - [cq](https://github.com/fullstackio/cq) is a tool thet lets you "extract code snippets using CSS-like selectors", built using [Tree-sitter](https://tree-sitter.github.io/tree-sitter/) and primarily targetting JavaScript and TypeScript.
 
 ## symbex --help
@@ -461,14 +480,18 @@
 
       # Replace my_function with a new implementation:
       echo "def my_function(a, b):
           # This is a replacement implementation
           return a + b + 3
       " | symbex my_function --replace
 
+      # Replace my_function with the output of a command:
+      symbex first_function --rexec "sed 's/^/# /'"
+      # This uses sed to comment out the function body
+
 Options:
   --version                  Show the version and exit.
   -f, --file FILE            Files to search
   -d, --directory DIRECTORY  Directories to search
   --stdlib                   Search the Python standard library
   -x, --exclude DIRECTORY    Directories to exclude
   -s, --signatures           Show just function and class signatures
@@ -481,14 +504,17 @@
   --silent                   Silently ignore Python files with parse errors
   --function                 Filter functions
   --async                    Filter async functions
   --unasync                  Filter non-async functions
   --class                    Filter classes
   --documented               Filter functions with docstrings
   --undocumented             Filter functions without docstrings
+  --public                   Filter for symbols without a _ prefix
+  --private                  Filter for symbols with a _ prefix
+  --dunder                   Filter for symbols matching __*__
   --typed                    Filter functions with type annotations
   --untyped                  Filter functions without type annotations
   --partially-typed          Filter functions with partial type annotations
   --fully-typed              Filter functions with full type annotations
   --no-init                  Filter to exclude any __init__ methods
   --check                    Exit with non-zero code if any matches found
   --replace                  Replace matching symbol with text from stdin
```

### Comparing `symbex-1.2/README.md` & `symbex-1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -96,14 +96,17 @@
 
 - `--function` - only functions
 - `--class` - only classes
 - `--async` - only `async def` functions
 - `--unasync` - only non-async functions
 - `--documented` - functions/classes that have a docstring
 - `--undocumented` - functions/classes that do not have a docstring
+- `--public` - functions/classes that are public - don't have a `_name` prefix (or are `__*__` methods)
+- `--private` - functions/classes that are private - have a `_name` prefix and are not `__*__`
+- `--dunder` - functions matching `__*__` - this should usually be used with `*.*` to find all dunder methods
 - `--typed` - functions that have at least one type annotation
 - `--untyped` - functions that have no type annotations
 - `--partially-typed` - functions that have some type annotations but not all
 - `--fully-typed` - functions that have type annotations for every argument and the return value
 - `--no-init` - Exclude `__init__(self)` methods. This is useful when combined with `--fully-typed '*.*'` to avoid returning `__init__(self)` methods that would otherwise be classified as fully typed, since `__init__` doesn't need argument or return type annotations.
 
 For example, to see the signatures of every `async def` function in your project that doesn't have any type annotations:
@@ -116,14 +119,20 @@
 
 This example shows the full source code of every class method in the Python standard library that has type annotations for all of the arguments and the return value:
 
 ```bash
 symbex --fully-typed --no-init '*.*' --stdlib
 ```
 
+To find all public functions and methods that lack documentation, just showing the signature of each one:
+
+```bash
+symbex '*' '*.*' --public --undocumented --signatures
+```
+
 ### Example output
 
 In a fresh checkout of [Datasette](https://github.com/simonw/datasette) I ran this command:
 
 ```bash
 symbex MessagesDebugView get_long_description
 ```
@@ -380,22 +389,32 @@
     """
     return a + b + 3
 ```
 ## Using in CI
 
 The `--check` option causes `symbex` to return a non-zero exit code if any matches are found for your query.
 
-You can use this in CI to guard against things like functions being added without documentation:
+You can use this in CI to guard against things like public functions being added without documentation:
 
 ```bash
-symbex --function --undocumented --check
+symbex --function --public --undocumented --check
 ```
 This will fail silently but set a `1` exit code if there are any undocumented functions.
 
-`--check` will not output anything by default. Add `--count` to output a count of matching symbols, or `-s/--signatures` to output the signatures of the matching symbols.
+Using this as a step in a CI tool such as GitHub Actions should result in a test failure.
+
+Run this to see the exit code from the last command:
+```bash
+echo $?
+```
+
+`--check` will not output anything by default. Add `--count` to output a count of matching symbols, or `-s/--signatures` to output the signatures of the matching symbols, for example:
+```bash
+symbex --function --public --undocumented --check --count
+```
 
 ## Similar tools
 
 - [pyastgrep](https://github.com/spookylukey/pyastgrep) by Luke Plant offers advanced capabilities for viewing and searching through Python ASTs using XPath.
 - [cq](https://github.com/fullstackio/cq) is a tool thet lets you "extract code snippets using CSS-like selectors", built using [Tree-sitter](https://tree-sitter.github.io/tree-sitter/) and primarily targetting JavaScript and TypeScript.
 
 ## symbex --help
@@ -446,14 +465,18 @@
 
       # Replace my_function with a new implementation:
       echo "def my_function(a, b):
           # This is a replacement implementation
           return a + b + 3
       " | symbex my_function --replace
 
+      # Replace my_function with the output of a command:
+      symbex first_function --rexec "sed 's/^/# /'"
+      # This uses sed to comment out the function body
+
 Options:
   --version                  Show the version and exit.
   -f, --file FILE            Files to search
   -d, --directory DIRECTORY  Directories to search
   --stdlib                   Search the Python standard library
   -x, --exclude DIRECTORY    Directories to exclude
   -s, --signatures           Show just function and class signatures
@@ -466,14 +489,17 @@
   --silent                   Silently ignore Python files with parse errors
   --function                 Filter functions
   --async                    Filter async functions
   --unasync                  Filter non-async functions
   --class                    Filter classes
   --documented               Filter functions with docstrings
   --undocumented             Filter functions without docstrings
+  --public                   Filter for symbols without a _ prefix
+  --private                  Filter for symbols with a _ prefix
+  --dunder                   Filter for symbols matching __*__
   --typed                    Filter functions with type annotations
   --untyped                  Filter functions without type annotations
   --partially-typed          Filter functions with partial type annotations
   --fully-typed              Filter functions with full type annotations
   --no-init                  Filter to exclude any __init__ methods
   --check                    Exit with non-zero code if any matches found
   --replace                  Replace matching symbol with text from stdin
```

### Comparing `symbex-1.2/setup.py` & `symbex-1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "1.2"
+VERSION = "1.3"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `symbex-1.2/symbex/cli.py` & `symbex-1.3/symbex/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -117,14 +117,29 @@
 )
 @click.option(
     "--undocumented",
     is_flag=True,
     help="Filter functions without docstrings",
 )
 @click.option(
+    "--public",
+    is_flag=True,
+    help="Filter for symbols without a _ prefix",
+)
+@click.option(
+    "--private",
+    is_flag=True,
+    help="Filter for symbols with a _ prefix",
+)
+@click.option(
+    "--dunder",
+    is_flag=True,
+    help="Filter for symbols matching __*__",
+)
+@click.option(
     "--typed",
     is_flag=True,
     help="Filter functions with type annotations",
 )
 @click.option(
     "--untyped",
     is_flag=True,
@@ -170,14 +185,17 @@
     silent,
     function,
     async_,
     unasync,
     class_,
     documented,
     undocumented,
+    public,
+    private,
+    dunder,
     typed,
     untyped,
     partially_typed,
     fully_typed,
     no_init,
     check,
     replace,
@@ -230,14 +248,19 @@
 
     \b
         # Replace my_function with a new implementation:
         echo "def my_function(a, b):
             # This is a replacement implementation
             return a + b + 3
         " | symbex my_function --replace
+
+    \b
+        # Replace my_function with the output of a command:
+        symbex first_function --rexec "sed 's/^/# /'"
+        # This uses sed to comment out the function body
     """
     if modules:
         module_dirs = []
         module_files = []
         for module in modules:
             try:
                 mod = importlib.import_module(module)
@@ -277,14 +300,17 @@
             signatures,
             async_,
             unasync,
             function,
             class_,
             documented,
             undocumented,
+            public,
+            private,
+            dunder,
             typed,
             untyped,
             partially_typed,
             fully_typed,
             no_init,
             modules,
         ]
@@ -308,14 +334,17 @@
                 signatures,
                 async_,
                 unasync,
                 function,
                 class_,
                 documented,
                 undocumented,
+                public,
+                private,
+                dunder,
                 typed,
                 untyped,
                 partially_typed,
                 fully_typed,
                 no_init,
                 modules,
             ]
@@ -343,14 +372,17 @@
         [
             async_,
             unasync,
             function,
             class_,
             documented,
             undocumented,
+            public,
+            private,
+            dunder,
             typed,
             untyped,
             partially_typed,
             fully_typed,
             no_init,
         ]
     ):
@@ -367,14 +399,20 @@
                 return False
             if class_ and not isinstance(node, ast.ClassDef):
                 return False
             if documented and not ast.get_docstring(node):
                 return False
             if undocumented and ast.get_docstring(node):
                 return False
+            if public and node.name.startswith("_") and not is_dunder(node.name):
+                return False
+            if private and (is_dunder(node.name) or not node.name.startswith("_")):
+                return False
+            if dunder and not is_dunder(node.name):
+                return False
             summary = type_summary(node)
             # if no summary, type filters all fail
             if not summary and (
                 typed or untyped or partially_typed or fully_typed or no_init
             ):
                 return False
             # Apply type filters
@@ -495,7 +533,11 @@
 
 def is_subpath(path: pathlib.Path, parent: pathlib.Path) -> bool:
     try:
         path.relative_to(parent)
         return True
     except ValueError:
         return False
+
+
+def is_dunder(name):
+    return name.startswith("__") and name.endswith("__")
```

### Comparing `symbex-1.2/symbex/lib.py` & `symbex-1.3/symbex/lib.py`

 * *Files identical despite different names*

### Comparing `symbex-1.2/symbex.egg-info/PKG-INFO` & `symbex-1.3/symbex.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbex
-Version: 1.2
+Version: 1.3
 Summary: Find the Python code for specified symbols
 Home-page: https://github.com/simonw/symbex
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/symbex/issues
 Project-URL: CI, https://github.com/simonw/symbex/actions
 Project-URL: Changelog, https://github.com/simonw/symbex/releases
@@ -111,14 +111,17 @@
 
 - `--function` - only functions
 - `--class` - only classes
 - `--async` - only `async def` functions
 - `--unasync` - only non-async functions
 - `--documented` - functions/classes that have a docstring
 - `--undocumented` - functions/classes that do not have a docstring
+- `--public` - functions/classes that are public - don't have a `_name` prefix (or are `__*__` methods)
+- `--private` - functions/classes that are private - have a `_name` prefix and are not `__*__`
+- `--dunder` - functions matching `__*__` - this should usually be used with `*.*` to find all dunder methods
 - `--typed` - functions that have at least one type annotation
 - `--untyped` - functions that have no type annotations
 - `--partially-typed` - functions that have some type annotations but not all
 - `--fully-typed` - functions that have type annotations for every argument and the return value
 - `--no-init` - Exclude `__init__(self)` methods. This is useful when combined with `--fully-typed '*.*'` to avoid returning `__init__(self)` methods that would otherwise be classified as fully typed, since `__init__` doesn't need argument or return type annotations.
 
 For example, to see the signatures of every `async def` function in your project that doesn't have any type annotations:
@@ -131,14 +134,20 @@
 
 This example shows the full source code of every class method in the Python standard library that has type annotations for all of the arguments and the return value:
 
 ```bash
 symbex --fully-typed --no-init '*.*' --stdlib
 ```
 
+To find all public functions and methods that lack documentation, just showing the signature of each one:
+
+```bash
+symbex '*' '*.*' --public --undocumented --signatures
+```
+
 ### Example output
 
 In a fresh checkout of [Datasette](https://github.com/simonw/datasette) I ran this command:
 
 ```bash
 symbex MessagesDebugView get_long_description
 ```
@@ -395,22 +404,32 @@
     """
     return a + b + 3
 ```
 ## Using in CI
 
 The `--check` option causes `symbex` to return a non-zero exit code if any matches are found for your query.
 
-You can use this in CI to guard against things like functions being added without documentation:
+You can use this in CI to guard against things like public functions being added without documentation:
 
 ```bash
-symbex --function --undocumented --check
+symbex --function --public --undocumented --check
 ```
 This will fail silently but set a `1` exit code if there are any undocumented functions.
 
-`--check` will not output anything by default. Add `--count` to output a count of matching symbols, or `-s/--signatures` to output the signatures of the matching symbols.
+Using this as a step in a CI tool such as GitHub Actions should result in a test failure.
+
+Run this to see the exit code from the last command:
+```bash
+echo $?
+```
+
+`--check` will not output anything by default. Add `--count` to output a count of matching symbols, or `-s/--signatures` to output the signatures of the matching symbols, for example:
+```bash
+symbex --function --public --undocumented --check --count
+```
 
 ## Similar tools
 
 - [pyastgrep](https://github.com/spookylukey/pyastgrep) by Luke Plant offers advanced capabilities for viewing and searching through Python ASTs using XPath.
 - [cq](https://github.com/fullstackio/cq) is a tool thet lets you "extract code snippets using CSS-like selectors", built using [Tree-sitter](https://tree-sitter.github.io/tree-sitter/) and primarily targetting JavaScript and TypeScript.
 
 ## symbex --help
@@ -461,14 +480,18 @@
 
       # Replace my_function with a new implementation:
       echo "def my_function(a, b):
           # This is a replacement implementation
           return a + b + 3
       " | symbex my_function --replace
 
+      # Replace my_function with the output of a command:
+      symbex first_function --rexec "sed 's/^/# /'"
+      # This uses sed to comment out the function body
+
 Options:
   --version                  Show the version and exit.
   -f, --file FILE            Files to search
   -d, --directory DIRECTORY  Directories to search
   --stdlib                   Search the Python standard library
   -x, --exclude DIRECTORY    Directories to exclude
   -s, --signatures           Show just function and class signatures
@@ -481,14 +504,17 @@
   --silent                   Silently ignore Python files with parse errors
   --function                 Filter functions
   --async                    Filter async functions
   --unasync                  Filter non-async functions
   --class                    Filter classes
   --documented               Filter functions with docstrings
   --undocumented             Filter functions without docstrings
+  --public                   Filter for symbols without a _ prefix
+  --private                  Filter for symbols with a _ prefix
+  --dunder                   Filter for symbols matching __*__
   --typed                    Filter functions with type annotations
   --untyped                  Filter functions without type annotations
   --partially-typed          Filter functions with partial type annotations
   --fully-typed              Filter functions with full type annotations
   --no-init                  Filter to exclude any __init__ methods
   --check                    Exit with non-zero code if any matches found
   --replace                  Replace matching symbol with text from stdin
```

### Comparing `symbex-1.2/tests/test_imports.py` & `symbex-1.3/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `symbex-1.2/tests/test_replace.py` & `symbex-1.3/tests/test_replace.py`

 * *Files identical despite different names*

### Comparing `symbex-1.2/tests/test_symbex.py` & `symbex-1.3/tests/test_symbex.py`

 * *Files identical despite different names*

### Comparing `symbex-1.2/tests/test_symbols.py` & `symbex-1.3/tests/test_symbols.py`

 * *Files identical despite different names*

