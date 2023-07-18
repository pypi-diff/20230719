# Comparing `tmp/pyastgrep-1.2.2.tar.gz` & `tmp/pyastgrep-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyastgrep-1.2.2.tar", last modified: Tue Jun 27 15:41:42 2023, max compression
+gzip compressed data, was "pyastgrep-1.3.tar", last modified: Tue Jul 18 22:22:00 2023, max compression
```

## Comparing `pyastgrep-1.2.2.tar` & `pyastgrep-1.3.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-27 15:41:42.811281 pyastgrep-1.2.2/
--rw-r--r--   0 luke      (1000) luke      (1000)      378 2022-10-17 13:09:58.000000 pyastgrep-1.2.2/.gitattributes
--rw-r--r--   0 luke      (1000) luke      (1000)     1771 2022-11-07 12:01:43.000000 pyastgrep-1.2.2/.gitignore
--rw-rw-rw-   0 luke      (1000) luke      (1000)    15748 2023-06-27 15:41:42.811281 pyastgrep-1.2.2/PKG-INFO
--rw-r--r--   0 luke      (1000) luke      (1000)    14926 2023-06-22 18:47:11.000000 pyastgrep-1.2.2/README.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      755 2023-04-17 15:02:16.000000 pyastgrep-1.2.2/pyproject.toml
--rw-r--r--   0 luke      (1000) luke      (1000)     1120 2023-06-27 15:41:42.815281 pyastgrep-1.2.2/setup.cfg
--rw-r--r--   0 luke      (1000) luke      (1000)       38 2022-10-21 16:01:47.000000 pyastgrep-1.2.2/setup.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-27 15:41:42.803281 pyastgrep-1.2.2/src/
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-27 15:41:42.807281 pyastgrep-1.2.2/src/pyastgrep/
--rw-r--r--   0 luke      (1000) luke      (1000)       22 2023-06-27 15:38:08.000000 pyastgrep-1.2.2/src/pyastgrep/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1854 2023-06-22 08:42:51.000000 pyastgrep-1.2.2/src/pyastgrep/ast_utils.py
--rw-r--r--   0 luke      (1000) luke      (1000)     3851 2023-06-27 07:16:37.000000 pyastgrep-1.2.2/src/pyastgrep/asts.py
--rw-r--r--   0 luke      (1000) luke      (1000)     6555 2023-06-26 13:47:54.000000 pyastgrep-1.2.2/src/pyastgrep/cli.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1273 2023-06-22 09:46:09.000000 pyastgrep-1.2.2/src/pyastgrep/context.py
--rw-r--r--   0 luke      (1000) luke      (1000)      890 2022-11-25 07:36:32.000000 pyastgrep-1.2.2/src/pyastgrep/dump.py
--rw-r--r--   0 luke      (1000) luke      (1000)     4037 2023-06-26 13:47:54.000000 pyastgrep-1.2.2/src/pyastgrep/files.py
--rw-r--r--   0 luke      (1000) luke      (1000)    10840 2023-06-21 10:04:58.000000 pyastgrep-1.2.2/src/pyastgrep/ignores.py
--rw-r--r--   0 luke      (1000) luke      (1000)    10566 2023-06-22 09:21:14.000000 pyastgrep-1.2.2/src/pyastgrep/printer.py
--rw-r--r--   0 luke      (1000) luke      (1000)     4563 2023-06-26 14:10:33.000000 pyastgrep-1.2.2/src/pyastgrep/search.py
--rw-r--r--   0 luke      (1000) luke      (1000)      696 2022-11-14 14:54:35.000000 pyastgrep-1.2.2/src/pyastgrep/xml.py
--rw-r--r--   0 luke      (1000) luke      (1000)      366 2022-11-06 20:21:35.000000 pyastgrep-1.2.2/src/pyastgrep/xpath2.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-27 15:41:42.807281 pyastgrep-1.2.2/src/pyastgrep.egg-info/
--rw-r-----   0 luke      (1000) luke      (1000)    15748 2023-06-27 15:41:42.000000 pyastgrep-1.2.2/src/pyastgrep.egg-info/PKG-INFO
--rw-r-----   0 luke      (1000) luke      (1000)      750 2023-06-27 15:41:42.000000 pyastgrep-1.2.2/src/pyastgrep.egg-info/SOURCES.txt
--rw-r-----   0 luke      (1000) luke      (1000)        1 2023-06-27 15:41:42.000000 pyastgrep-1.2.2/src/pyastgrep.egg-info/dependency_links.txt
--rw-r-----   0 luke      (1000) luke      (1000)       81 2023-06-27 15:41:42.000000 pyastgrep-1.2.2/src/pyastgrep.egg-info/entry_points.txt
--rw-r-----   0 luke      (1000) luke      (1000)       58 2023-06-27 15:41:42.000000 pyastgrep-1.2.2/src/pyastgrep.egg-info/requires.txt
--rw-r-----   0 luke      (1000) luke      (1000)       10 2023-06-27 15:41:42.000000 pyastgrep-1.2.2/src/pyastgrep.egg-info/top_level.txt
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-27 15:41:42.811281 pyastgrep-1.2.2/tests/
--rw-r--r--   0 luke      (1000) luke      (1000)     6529 2023-06-21 08:40:28.000000 pyastgrep-1.2.2/tests/test_cli.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1558 2023-06-26 19:56:42.000000 pyastgrep-1.2.2/tests/test_encodings.py
--rw-r--r--   0 luke      (1000) luke      (1000)      648 2022-11-07 12:52:05.000000 pyastgrep-1.2.2/tests/test_errors.py
--rw-r--r--   0 luke      (1000) luke      (1000)     5325 2023-06-21 09:44:46.000000 pyastgrep-1.2.2/tests/test_ignores.py
--rw-r--r--   0 luke      (1000) luke      (1000)      449 2022-11-25 08:08:17.000000 pyastgrep-1.2.2/tests/test_parsing.py
--rw-r--r--   0 luke      (1000) luke      (1000)     7058 2023-06-22 09:50:58.000000 pyastgrep-1.2.2/tests/test_printing.py
--rw-r--r--   0 luke      (1000) luke      (1000)      410 2023-02-20 15:45:50.000000 pyastgrep-1.2.2/tests/test_symlinks.py
--rw-r--r--   0 luke      (1000) luke      (1000)    12211 2023-06-27 07:05:06.000000 pyastgrep-1.2.2/tests/test_xml.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-07-18 22:22:00.292992 pyastgrep-1.3/
+-rw-r--r--   0 luke      (1000) luke      (1000)      378 2022-10-17 13:09:58.000000 pyastgrep-1.3/.gitattributes
+-rw-r--r--   0 luke      (1000) luke      (1000)     1771 2022-11-07 12:01:43.000000 pyastgrep-1.3/.gitignore
+-rw-rw-rw-   0 luke      (1000) luke      (1000)    15965 2023-07-18 22:22:00.296992 pyastgrep-1.3/PKG-INFO
+-rw-r--r--   0 luke      (1000) luke      (1000)    15145 2023-06-28 14:16:41.000000 pyastgrep-1.3/README.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      806 2023-07-18 21:14:43.000000 pyastgrep-1.3/pyproject.toml
+-rw-r--r--   0 luke      (1000) luke      (1000)     1164 2023-07-18 22:22:00.296992 pyastgrep-1.3/setup.cfg
+-rw-r--r--   0 luke      (1000) luke      (1000)       38 2022-10-21 16:01:47.000000 pyastgrep-1.3/setup.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-07-18 22:22:00.288992 pyastgrep-1.3/src/
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-07-18 22:22:00.292992 pyastgrep-1.3/src/pyastgrep/
+-rw-r--r--   0 luke      (1000) luke      (1000)       20 2023-07-18 22:21:25.000000 pyastgrep-1.3/src/pyastgrep/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     2100 2023-07-10 13:19:56.000000 pyastgrep-1.3/src/pyastgrep/ast_utils.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     3851 2023-07-18 12:48:04.000000 pyastgrep-1.3/src/pyastgrep/asts.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     7443 2023-07-18 21:58:41.000000 pyastgrep-1.3/src/pyastgrep/cli.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     2989 2023-07-18 22:02:02.000000 pyastgrep-1.3/src/pyastgrep/color.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1273 2023-06-22 09:46:09.000000 pyastgrep-1.3/src/pyastgrep/context.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      890 2022-11-25 07:36:32.000000 pyastgrep-1.3/src/pyastgrep/dump.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     4055 2023-07-18 12:54:44.000000 pyastgrep-1.3/src/pyastgrep/files.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    10840 2023-07-18 12:54:58.000000 pyastgrep-1.3/src/pyastgrep/ignores.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    11324 2023-07-18 21:56:25.000000 pyastgrep-1.3/src/pyastgrep/printer.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     4378 2023-07-18 21:04:48.000000 pyastgrep-1.3/src/pyastgrep/search.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      956 2023-07-18 21:36:26.000000 pyastgrep-1.3/src/pyastgrep/xml.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      397 2023-07-18 21:36:26.000000 pyastgrep-1.3/src/pyastgrep/xpath2.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-07-18 22:22:00.292992 pyastgrep-1.3/src/pyastgrep.egg-info/
+-rw-r-----   0 luke      (1000) luke      (1000)    15965 2023-07-18 22:22:00.000000 pyastgrep-1.3/src/pyastgrep.egg-info/PKG-INFO
+-rw-r-----   0 luke      (1000) luke      (1000)      773 2023-07-18 22:22:00.000000 pyastgrep-1.3/src/pyastgrep.egg-info/SOURCES.txt
+-rw-r-----   0 luke      (1000) luke      (1000)        1 2023-07-18 22:22:00.000000 pyastgrep-1.3/src/pyastgrep.egg-info/dependency_links.txt
+-rw-r-----   0 luke      (1000) luke      (1000)       81 2023-07-18 22:22:00.000000 pyastgrep-1.3/src/pyastgrep.egg-info/entry_points.txt
+-rw-r-----   0 luke      (1000) luke      (1000)      104 2023-07-18 22:22:00.000000 pyastgrep-1.3/src/pyastgrep.egg-info/requires.txt
+-rw-r-----   0 luke      (1000) luke      (1000)       10 2023-07-18 22:22:00.000000 pyastgrep-1.3/src/pyastgrep.egg-info/top_level.txt
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-07-18 22:22:00.292992 pyastgrep-1.3/tests/
+-rw-r--r--   0 luke      (1000) luke      (1000)     6529 2023-07-18 12:44:48.000000 pyastgrep-1.3/tests/test_cli.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1559 2023-07-18 12:44:48.000000 pyastgrep-1.3/tests/test_encodings.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      648 2022-11-07 12:52:05.000000 pyastgrep-1.3/tests/test_errors.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     5325 2023-07-18 12:44:48.000000 pyastgrep-1.3/tests/test_ignores.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      449 2022-11-25 08:08:17.000000 pyastgrep-1.3/tests/test_parsing.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     8409 2023-07-18 21:55:34.000000 pyastgrep-1.3/tests/test_printing.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      411 2023-07-18 12:44:48.000000 pyastgrep-1.3/tests/test_symlinks.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    12211 2023-07-18 12:44:48.000000 pyastgrep-1.3/tests/test_xml.py
```

### Comparing `pyastgrep-1.2.2/.gitignore` & `pyastgrep-1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.2.2/PKG-INFO` & `pyastgrep-1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastgrep
-Version: 1.2.2
+Version: 1.3
 Summary: A query tool for Python abstract syntax trees
 Home-page: https://github.com/spookylukey/pyastgrep
 Author: Luke Plant
 License: MIT
 Keywords: xpath xml ast asts syntax query css grep
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -373,14 +373,21 @@
 a ``target`` node that is a parent of a ``Name`` node with attribute ``id``
 equal to ``"foo"``:
 
 .. code:: bash
 
    $ pyastgrep './/Assign[./targets//Name[@id="foo"]]' --xml
 
+Bugs
+----
+
+Due to limitations in what characters can be stored in an XML document, null
+bytes (``\x00``) and other characters such as escape codes in string and byte
+literals get stripped, and can’t be searched for.
+
 Limitations and other tools
 ---------------------------
 
 pyastgrep is useful for grepping Python code at a fairly low level. It can be
 used for various refactoring or linting tasks. Some linting tasks require higher
 level understanding of a code base. For example, to detect use of a certain
 function, you need to cope with various ways that the function may be imported
```

### Comparing `pyastgrep-1.2.2/README.rst` & `pyastgrep-1.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -351,14 +351,21 @@
 a ``target`` node that is a parent of a ``Name`` node with attribute ``id``
 equal to ``"foo"``:
 
 .. code:: bash
 
    $ pyastgrep './/Assign[./targets//Name[@id="foo"]]' --xml
 
+Bugs
+----
+
+Due to limitations in what characters can be stored in an XML document, null
+bytes (``\x00``) and other characters such as escape codes in string and byte
+literals get stripped, and can’t be searched for.
+
 Limitations and other tools
 ---------------------------
 
 pyastgrep is useful for grepping Python code at a fairly low level. It can be
 used for various refactoring or linting tasks. Some linting tasks require higher
 level understanding of a code base. For example, to detect use of a certain
 function, you need to cope with various ways that the function may be imported
```

### Comparing `pyastgrep-1.2.2/pyproject.toml` & `pyastgrep-1.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -8,24 +8,26 @@
 line_length = 120
 profile = "black"
 multi_line_output = 3
 
 
 [tool.ruff]
 line-length = 120
-target-version = 'py310'
+target-version = 'py38'
+select = ["E", "F", "I", "UP", "FLY"]
 
 
 [tool.mypy]
 ignore_missing_imports = true
 check_untyped_defs = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 show_error_codes = true
+strict = true
 exclude = ['dist', 'build']
 
 
 [[tool.mypy.overrides]]
 module = "tests.examples.*"
 ignore_errors = true
 disallow_untyped_calls = false
```

### Comparing `pyastgrep-1.2.2/setup.cfg` & `pyastgrep-1.3/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 python_requires = >=3.8
 install_requires = 
 	lxml>=3.3.5
 	elementpath
 	astpretty
 	pathspec
 	cssselect>=1.2
+	backports.strenum; python_version < "3.11"
 
 [options.entry_points]
 console_scripts = 
 	pyastgrep = pyastgrep.cli:main
 	pyastdump = pyastgrep.dump:main
 
 [options.packages.find]
```

### Comparing `pyastgrep-1.2.2/src/pyastgrep/ast_utils.py` & `pyastgrep-1.3/src/pyastgrep/ast_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 For changes between Python versions, try this one liner in bash/zsh:
 
 diff -u <(python3.10 -c 'import ast; print("\n".join(sorted(dir(ast))))') \
         <(python3.11 -c 'import ast; print("\n".join(sorted(dir(ast))))')
 """
 
 
+# BLOCK_AST and STATEMENT_AST together are based on the 'stmt' rule in the
+# Python grammar, plus others that have `body` attributes like Module and
+# ExceptHandler. BLOCK_AST are the ones that have a 'body' attribute.
 BLOCK_AST = tuple(
     i
     for i in [
         ast.FunctionDef,
         ast.AsyncFunctionDef,
         ast.ClassDef,
         ast.Module,
@@ -25,14 +28,15 @@
         ast.AsyncFor,
         ast.While,
         ast.If,
         ast.With,
         ast.Try,
         getattr(ast, "TryStar", None),
         getattr(ast, "match_case", None),
+        ast.ExceptHandler,
     ]
     if i
 )
 
 STATEMENT_AST = BLOCK_AST + tuple(
     i
     for i in [
```

### Comparing `pyastgrep-1.2.2/src/pyastgrep/asts.py` & `pyastgrep-1.3/src/pyastgrep/asts.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.2.2/src/pyastgrep/cli.py` & `pyastgrep-1.3/src/pyastgrep/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,22 +11,25 @@
 import argparse
 import sys
 from pathlib import Path
 from typing import BinaryIO
 
 from lxml.etree import XPathEvalError
 
-from pyastgrep import __version__
-from pyastgrep.printer import StatementContext, StaticContext, print_results
-from pyastgrep.search import search_python_files
+from . import __version__
+from .color import Colorer, NullColorer, UseColor, make_default_colorer
+from .context import StatementContext, StaticContext
+from .printer import print_results
+from .search import search_python_files
 
 NAME_AND_VERSION = "pyastgrep " + __version__
 parser = argparse.ArgumentParser(
     prog=NAME_AND_VERSION,
     description="Grep Python files uses XPath expressions against the AST",
+    formatter_class=argparse.RawTextHelpFormatter,
 )
 
 
 def context_parameter(param: str) -> int | StatementContext:
     if param == "statement":
         return StatementContext()
     return int(param)  # Will raise ValueError if invalid, which is handled by argparse
@@ -65,52 +68,68 @@
     help="Lines of context to display after matching line",
     type=int,
     default=0,
 )
 parser.add_argument(
     "-C",
     "--context",
-    help="Lines of context to display before and after matching line, as an integer. "
-    "You can also use '--context=statement' to print the complete statement of a given match. "
-    "When combined with --heading, this has some extra behaviour:"
-    " code is automatically dedented;"
-    " multiple matches within the same statement won't be printed twice.",
+    help="""Lines of context to display before and after matching line, as an integer.
+You can also use '--context=statement' to print the complete statement of a match.
+When combined with --heading, this has some extra behaviour:
+  - code is automatically dedented
+  - multiple matches within the same statement won't be printed twice.
+  - matches are not colored
+    """,
     type=context_parameter,
     default=0,
 )
 parser.add_argument(
+    "--color",
+    help="""Controls when to use colors. Possible values are:
+    never    Colors will never be used.
+    auto     Use colors if a terminal is detected as the output (default)
+    always   Colors will always be used regardless of where output is sent.
+    """,
+    type=UseColor,
+    default=UseColor.AUTO,
+    choices=list(UseColor),
+)
+parser.add_argument(
     "--css",
     help="Interpret expression as a CSS selector",
     action="store_true",
 )
 parser.add_argument(
     "--xpath2",
-    help="Use XPath 2.0 functions and selectors. This currently makes matching significantly slower, "
-    "and re:match and re:search functions are not supported",
+    help="""Use XPath 2.0 functions and selectors. This currently makes matching
+significantly slower, and re:match and re:search functions are not supported""",
     action="store_true",
     default=False,
 )
 parser.add_argument(
     "--heading",
-    help="Print the file path and line number as a heading (formatted as a Python comment) above the results.",
+    help="""Print the file path and line number as a heading (formatted as a Python
+comment) above the results.""",
     action="store_true",
     default=False,
 )
 parser.add_argument(
     "-.",
     "--hidden",
-    help="Search hidden files and directories, which are skipped by default. A file "
-    "or directory is considered hidden if its base name starts with a dot character ('.').",
+    help="""Search hidden files and directories, which are skipped by default.
+A file or directory is considered hidden if its base name starts with
+a dot character ('.').""",
     action="store_true",
     default=False,
 )
 parser.add_argument(
     "--no-ignore-global",
-    help="Don't respect ignore files that come from \"global\" sources such as git's "
-    "`core.excludesFile` configuration option (typically ~/.config/git/ignore` or ~/.gitignore)).",
+    help="""Don't respect ignore files that come from \"global\" sources such as
+git's `core.excludesFile` configuration option, which is typically
+~/.config/git/ignore or ~/.gitignore""",
     action="store_true",
     default=False,
 )
 parser.add_argument(
     "--no-ignore-vcs",
     help="Don't respect version control ignore files (.gitignore, etc.). ",
     action="store_true",
@@ -124,15 +143,16 @@
 )
 parser.add_argument(
     "expr",
     help="XPath search expression",
 )
 parser.add_argument(
     "path",
-    help="Zero or more files or directory to search. Search defaults to current directory if omitted. Use - for stdin",
+    help="""Zero or more files or directory to search. Search defaults to current directory if omitted.
+Use - for stdin""",
     nargs="*",
 )
 
 MATCH_FOUND = 0
 NO_MATCH_FOUND = 1
 ERROR = 2
 
@@ -182,14 +202,26 @@
 
         try:
             expr = cssselect.GenericTranslator().css_to_xpath(expr, prefix=".//")
         except cssselect.SelectorError:
             print(f"Invalid CSS selector: {expr}", file=sys.stderr)
             return ERROR
 
+    colorer: Colorer
+    color: UseColor = args.color
+    if color == UseColor.AUTO:
+        if sys.stdout.isatty():
+            colorer = make_default_colorer()
+        else:
+            colorer = NullColorer()
+    elif color == UseColor.NEVER:
+        colorer = NullColorer()
+    elif color == UseColor.ALWAYS:
+        colorer = make_default_colorer()
+
     try:
         matches, errors = print_results(
             search_python_files(
                 paths,
                 expr,
                 xpath2=args.xpath2,
                 include_hidden=args.hidden,
@@ -197,14 +229,15 @@
                 respect_vcs_ignores=not args.no_ignore_vcs,
             ),
             print_xml=args.xml,
             print_ast=args.ast,
             quiet=args.quiet,
             context=context,
             heading=args.heading,
+            colorer=colorer,
         )
     except XPathEvalError:
         print(f"Invalid XPath expression: {expr}", file=sys.stderr)
         return ERROR
     except KeyboardInterrupt:
         sys.exit(1)
     # Match ripgrep:
```

### Comparing `pyastgrep-1.2.2/src/pyastgrep/context.py` & `pyastgrep-1.3/src/pyastgrep/context.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.2.2/src/pyastgrep/dump.py` & `pyastgrep-1.3/src/pyastgrep/dump.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.2.2/src/pyastgrep/files.py` & `pyastgrep-1.3/src/pyastgrep/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
 
 def parse_python_file(contents: bytes, filename: str | Path, *, auto_dedent: bool) -> tuple[str, ast.AST]:
     if auto_dedent:
         contents = auto_dedent_code(contents)
 
     parsed_ast: ast.AST = ast.parse(contents, str(filename))
-    # Needed for StatementContext and for position_from_node
+    # Need `parent` backlinks for StatementContext and for position_from_node:
     for node in ast.walk(parsed_ast):
         for child in ast.iter_child_nodes(node):
             child.parent = node  # type: ignore
 
     # ast.parse does it's own encoding detection, which we have to replicate
     # here since we can't assume utf-8
     encoding = get_encoding(contents)
```

### Comparing `pyastgrep-1.2.2/src/pyastgrep/ignores.py` & `pyastgrep-1.3/src/pyastgrep/ignores.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.2.2/src/pyastgrep/printer.py` & `pyastgrep-1.3/src/pyastgrep/printer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
 import sys
 import textwrap
 from typing import Callable, Iterable, Protocol, TextIO
 
 from . import xml
+from .color import Colorer, NullColorer
 from .context import ContextType, StatementContext, StaticContext
-from .search import FileFinished, Match, MissingPath, NonElementReturned, Pathlike, ReadError
+from .files import MissingPath
+from .search import FileFinished, Match, NonElementReturned, Pathlike, ReadError
 
 
 class Formatter(Protocol):
     def format_header(self, path: Pathlike, context_line_index: int) -> str | None:
         pass
 
     def format_context_line(self, result: Match, context_line: str, context_line_index: int) -> str:
@@ -36,45 +38,50 @@
     print_xml: bool = False,
     print_ast: bool = False,
     context: ContextType = StaticContext(before=0, after=0),
     stdout: TextIO | None = None,
     stderr: TextIO | None = None,
     quiet: bool = False,
     heading: bool = False,
+    colorer: Colorer | None = None,
 ) -> tuple[int, int]:
     if print_ast:
         # Don't import unless needed
         import astpretty
 
     if stdout is None:
         stdout = sys.stdout
     if stderr is None:
         stderr = sys.stderr
+    if colorer is None:
+        colorer = NullColorer()
     matches = 0
     errors = 0
 
     def do_error(message: str) -> None:
         nonlocal errors
         print(message, file=stderr)
         errors += 1
 
     def line_printer(line: str) -> None:
         print(line, file=stdout)
 
     context_handler: ContextHandler
     if heading:
         if isinstance(context, StatementContext):
-            context_handler = StatementWithHeadingContextHandler(line_printer=line_printer)
+            context_handler = StatementWithHeadingContextHandler(
+                line_printer=line_printer, formatter=HeadingFormatter(colorer=colorer)
+            )
         else:
             context_handler = DefaultContextHandler(
-                context_type=context, line_printer=line_printer, formatter=HeadingFormatter()
+                context_type=context, line_printer=line_printer, formatter=HeadingFormatter(colorer=colorer)
             )
     else:
         context_handler = DefaultContextHandler(
-            context_type=context, line_printer=line_printer, formatter=DefaultFormatter()
+            context_type=context, line_printer=line_printer, formatter=DefaultFormatter(colorer=colorer)
         )
 
     for result in results:
         if isinstance(result, MissingPath):
             do_error(f"{result.path}: No such file or directory")
             continue
         elif isinstance(result, ReadError):
@@ -216,18 +223,18 @@
 
     # This requires a different strategy, because we need to dedent the whole
     # statement at once. We don't have the issues with needing to wait for the
     # next result, because context lines are not formatted different to matches.
     # For cases of overlapping or nested matches, we don't print the same lines
     # multiple times.
 
-    def __init__(self, *, line_printer: LinePrinter):
+    def __init__(self, *, line_printer: LinePrinter, formatter: Formatter):
         # Configuration from outside:
         self.line_printer = line_printer
-        self.formatter = HeadingFormatter()
+        self.formatter = formatter
         self.context_type = StatementContext()
 
         # Managed state:
         self.printed_context_lines: set[tuple[Pathlike, int]] = set()
 
     def handle_result(self, result: Match) -> None:
         line_index = result.position.lineno - 1
@@ -257,36 +264,50 @@
         pass
 
 
 # Formatters
 
 
 class DefaultFormatter:
+    def __init__(self, colorer: Colorer):
+        self.colorer = colorer
+
     # Same formatting as ripgrep:
     def format_header(self, path: Pathlike, context_line_index: int) -> str | None:
         return None
 
     def format_context_line(self, result: Match, context_line: str, context_line_index: int) -> str:
-        return f"{result.path}-{context_line_index + 1}-{context_line}"
+        c = self.colorer
+        path_s = c.color_path(str(result.path))
+        lineno_s = c.color_lineno(context_line_index + 1)
+        return f"{path_s}-{lineno_s}-{context_line}"
 
     def format_match_line(self, result: Match) -> str:
-        return f"{result.path}:{result.position.lineno}:{result.position.col_offset + 1}:{result.matching_line}"
+        c = self.colorer
+        path_s = c.color_path(str(result.path))
+        lineno_s = c.color_lineno(result.position.lineno)
+        match_s = c.color_match(result)
+        return f"{path_s}:{lineno_s}:{result.position.col_offset + 1}:{match_s}"
 
 
 class HeadingFormatter:
-    def __init__(self) -> None:
+    def __init__(self, colorer: Colorer):
+        self.colorer = colorer
         self.first_result_printed = False
 
     def format_header(self, path: Pathlike, context_line_index: int) -> str | None:
         # Start with hash like a Python comment, for integration with tools that
         # consume Python code
 
         # Gap between results, for all but very first
         spacer = "\n" if self.first_result_printed else ""
         self.first_result_printed = True
-        return spacer + f"# {path}:{context_line_index + 1}:"
+        c = self.colorer
+        path_s = c.color_path(str(path))
+        lineno_s = c.color_lineno(context_line_index + 1)
+        return spacer + f"# {path_s}:{lineno_s}:"
 
     def format_context_line(self, result: Match, context_line: str, context_line_index: int) -> str:
         return context_line
 
     def format_match_line(self, result: Match) -> str:
-        return result.matching_line
+        return self.colorer.color_match(result)
```

### Comparing `pyastgrep-1.2.2/src/pyastgrep/search.py` & `pyastgrep-1.3/src/pyastgrep/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,22 @@
 """Functions for searching the XML from file, file contents, or directory."""
 from __future__ import annotations
 
 import ast
 from dataclasses import dataclass
 from pathlib import Path
-from typing import TYPE_CHECKING, BinaryIO, Callable, Generator, Iterable, Sequence
+from typing import BinaryIO, Callable, Generator, Iterable, Literal, Sequence, Union
 
 from lxml.etree import _Element
 
 from . import xml
 from .asts import ast_to_xml
 from .files import MissingPath, get_files_to_search, parse_python_file
 
-if TYPE_CHECKING:
-    from typing import Literal
-
-    Pathlike = Path | Literal["<stdin>"]
-else:
-    # `|` not supported on older Python versions we support,
-    # and Literal is only available in Python 3.8+
-    Pathlike = Path
+Pathlike = Union[Path, Literal["<stdin>"]]
 
 
 @dataclass(frozen=True)
 class Match:
     path: Pathlike
     file_lines: list[str]
     xml_element: _Element
```

### Comparing `pyastgrep-1.2.2/src/pyastgrep/xml.py` & `pyastgrep-1.3/src/pyastgrep/xml.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 from __future__ import annotations
 
 import re
+from typing import TYPE_CHECKING, Callable
 
 from lxml import etree
 from lxml.etree import _Element, _ElementUnicodeResult, tostring
 
 __all__ = ["tostring", "lxml_query"]
 
+if TYPE_CHECKING:
+    from typing import ParamSpec, TypeVar
+
+    P = ParamSpec("P")
+    R = TypeVar("R")
+
 
 def lxml_query(element: _Element, expression: str) -> list[_Element | _ElementUnicodeResult]:
-    return element.xpath(expression)
+    return element.xpath(expression)  # type: ignore[no-any-return]
 
 
-regex_ns = etree.FunctionNamespace("https://github.com/spookylukey/pyastgrep")
-regex_ns.prefix = "re"
+regex_ns: Callable[[Callable[P, R]], Callable[P, R]] = etree.FunctionNamespace(
+    "https://github.com/spookylukey/pyastgrep"
+)
+regex_ns.prefix = "re"  # type: ignore[attr-defined]
 
 
 @regex_ns
 def match(ctx: None, pattern: str, strings: list[str]) -> bool:
     return any(re.match(pattern, s) is not None for s in strings)
```

### Comparing `pyastgrep-1.2.2/src/pyastgrep.egg-info/PKG-INFO` & `pyastgrep-1.3/src/pyastgrep.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastgrep
-Version: 1.2.2
+Version: 1.3
 Summary: A query tool for Python abstract syntax trees
 Home-page: https://github.com/spookylukey/pyastgrep
 Author: Luke Plant
 License: MIT
 Keywords: xpath xml ast asts syntax query css grep
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -373,14 +373,21 @@
 a ``target`` node that is a parent of a ``Name`` node with attribute ``id``
 equal to ``"foo"``:
 
 .. code:: bash
 
    $ pyastgrep './/Assign[./targets//Name[@id="foo"]]' --xml
 
+Bugs
+----
+
+Due to limitations in what characters can be stored in an XML document, null
+bytes (``\x00``) and other characters such as escape codes in string and byte
+literals get stripped, and can’t be searched for.
+
 Limitations and other tools
 ---------------------------
 
 pyastgrep is useful for grepping Python code at a fairly low level. It can be
 used for various refactoring or linting tasks. Some linting tasks require higher
 level understanding of a code base. For example, to detect use of a certain
 function, you need to cope with various ways that the function may be imported
```

### Comparing `pyastgrep-1.2.2/src/pyastgrep.egg-info/SOURCES.txt` & `pyastgrep-1.3/src/pyastgrep.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyproject.toml
 setup.cfg
 setup.py
 src/pyastgrep/__init__.py
 src/pyastgrep/ast_utils.py
 src/pyastgrep/asts.py
 src/pyastgrep/cli.py
+src/pyastgrep/color.py
 src/pyastgrep/context.py
 src/pyastgrep/dump.py
 src/pyastgrep/files.py
 src/pyastgrep/ignores.py
 src/pyastgrep/printer.py
 src/pyastgrep/search.py
 src/pyastgrep/xml.py
```

### Comparing `pyastgrep-1.2.2/tests/test_cli.py` & `pyastgrep-1.3/tests/test_cli.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import io
 import subprocess
 from pathlib import Path
 
 import pytest
-
 from pyastgrep.cli import main
+
 from tests.utils import chdir
 
 DIR = Path(__file__).parent / "examples" / "test_cli"
 
 
 def assert_output(
     capsys,
```

### Comparing `pyastgrep-1.2.2/tests/test_encodings.py` & `pyastgrep-1.3/tests/test_encodings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import io
 from pathlib import Path
 
 from pyastgrep.files import get_encoding
+
 from tests.utils import run_print
 
 DIR = Path(__file__).parent / "examples" / "test_encodings"
 
 
 def test_empty():
     assert get_encoding(b"") == "utf-8"
```

### Comparing `pyastgrep-1.2.2/tests/test_errors.py` & `pyastgrep-1.3/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.2.2/tests/test_ignores.py` & `pyastgrep-1.3/tests/test_ignores.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from unittest.mock import patch
 
-from pathspec.gitignore import GitIgnoreSpec
-
 import pyastgrep.ignores
+from pathspec.gitignore import GitIgnoreSpec
 from pyastgrep.files import get_files_to_search
 from pyastgrep.ignores import DirectoryPathSpec, find_gitignore_files
+
 from tests.utils import chdir, run_print
 
 DIR = Path(__file__).resolve().parent / "examples" / "test_ignores"
 REPO_ROOT = Path(__file__).resolve().parent.parent
 DIR_FROM_ROOT = DIR.relative_to(REPO_ROOT)
```

### Comparing `pyastgrep-1.2.2/tests/test_printing.py` & `pyastgrep-1.3/tests/test_printing.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import io
 from pathlib import Path
 
 import pytest
+from pyastgrep.color import Colors, Styles, make_default_colorer
+from pyastgrep.context import StatementContext, StaticContext
 
-from pyastgrep.printer import StatementContext, StaticContext
 from tests.utils import run_print
 
 DIR = Path(__file__).parent / "examples" / "test_printing"
 
 
 def test_before_context():
     output = run_print(DIR, './/Name[@id="a_name"]', ["context_example.py"], context=StaticContext(before=1)).stdout
@@ -282,7 +283,42 @@
 out_of_order.py-3-
 out_of_order.py:4:11:@dec(param=1)
 out_of_order.py:5:17:def function(arg=2):
 out_of_order.py:6:5:    3
 out_of_order.py-7-
 """.lstrip()
     )
+
+
+def test_coloring():
+    output = run_print(
+        DIR, ".//arg", ["colors.py"], context=StaticContext(before=0, after=0), colorer=make_default_colorer()
+    ).stdout
+    assert output == (
+        f"{Colors.MAGENTA}colors.py{Styles.END}:{Colors.GREEN}1{Styles.END}:9:"
+        f"def foo({Colors.RED}{Styles.BOLD}arg1{Styles.END}, arg2):\n"
+        f"{Colors.MAGENTA}colors.py{Styles.END}:{Colors.GREEN}1{Styles.END}:15:"
+        f"def foo(arg1, {Colors.RED}{Styles.BOLD}arg2{Styles.END}):\n"
+    )
+
+
+def test_coloring_function_def():
+    # See comment in AnsiColorer.color_match
+    output = run_print(
+        DIR, ".//FunctionDef", ["colors.py"], context=StaticContext(before=0, after=0), colorer=make_default_colorer()
+    ).stdout
+    assert output == (f"{Colors.MAGENTA}colors.py{Styles.END}:{Colors.GREEN}1{Styles.END}:1:def foo(arg1, arg2):\n")
+
+
+def test_coloring_heading():
+    output = run_print(
+        DIR,
+        ".//arg[@arg='arg1']",
+        ["colors.py"],
+        context=StaticContext(before=0, after=0),
+        colorer=make_default_colorer(),
+        heading=True,
+    ).stdout
+    assert output == (
+        f"# {Colors.MAGENTA}colors.py{Styles.END}:{Colors.GREEN}1{Styles.END}:\n"
+        f"def foo({Colors.RED}{Styles.BOLD}arg1{Styles.END}, arg2):\n"
+    )
```

### Comparing `pyastgrep-1.2.2/tests/test_xml.py` & `pyastgrep-1.3/tests/test_xml.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 from pathlib import Path
 
 import lxml.etree
 import pytest
-
 from pyastgrep.asts import ast_to_xml
 from pyastgrep.files import parse_python_file
+
 from tests.utils import run_print
 
 DIR = Path(__file__).parent / "examples" / "test_xml"
 
 
 def test_literals():
     # We need a way to distinguish between different literals
```

