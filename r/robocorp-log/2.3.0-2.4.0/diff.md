# Comparing `tmp/robocorp_log-2.3.0.tar.gz` & `tmp/robocorp_log-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_log-2.3.0.tar", max compression
+gzip compressed data, was "robocorp_log-2.4.0.tar", max compression
```

## Comparing `robocorp_log-2.3.0.tar` & `robocorp_log-2.4.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0    10142 2023-07-10 19:37:10.488717 robocorp_log-2.3.0/LICENSE
--rw-r--r--   0        0        0     5557 2023-07-10 19:37:10.488717 robocorp_log-2.3.0/README.md
--rw-r--r--   0        0        0     1297 2023-07-10 19:37:10.492717 robocorp_log-2.3.0/pyproject.toml
--rw-r--r--   0        0        0    38636 2023-07-10 19:37:10.492717 robocorp_log-2.3.0/src/robocorp/log/__init__.py
--rw-r--r--   0        0        0    17963 2023-07-10 19:37:10.492717 robocorp_log-2.3.0/src/robocorp/log/_ast_utils.py
--rw-r--r--   0        0        0    15297 2023-07-10 19:37:10.492717 robocorp_log-2.3.0/src/robocorp/log/_auto_logging_setup.py
--rw-r--r--   0        0        0    14416 2023-07-10 19:37:10.492717 robocorp_log-2.3.0/src/robocorp/log/_config.py
--rw-r--r--   0        0        0      696 2023-07-10 19:37:10.492717 robocorp_log-2.3.0/src/robocorp/log/_convert_units.py
--rw-r--r--   0        0        0     7143 2023-07-10 19:37:10.492717 robocorp_log-2.3.0/src/robocorp/log/_decoder.py
--rw-r--r--   0        0        0     7193 2023-07-10 19:37:10.496717 robocorp_log-2.3.0/src/robocorp/log/_decoder_spec.py
--rw-r--r--   0        0        0   805892 2023-07-10 19:38:04.712192 robocorp_log-2.3.0/src/robocorp/log/_index_v3.py
--rw-r--r--   0        0        0     7077 2023-07-10 19:37:10.496717 robocorp_log-2.3.0/src/robocorp/log/_lifecycle_hooks.py
--rw-r--r--   0        0        0     1128 2023-07-10 19:37:10.496717 robocorp_log-2.3.0/src/robocorp/log/_logger_instances.py
--rw-r--r--   0        0        0     1208 2023-07-10 19:37:10.496717 robocorp_log-2.3.0/src/robocorp/log/_null.py
--rw-r--r--   0        0        0      886 2023-07-10 19:37:10.496717 robocorp_log-2.3.0/src/robocorp/log/_obj_info_repr.py
--rw-r--r--   0        0        0      396 2023-07-10 19:37:10.496717 robocorp_log-2.3.0/src/robocorp/log/_on_exit_context_manager.py
--rw-r--r--   0        0        0    32317 2023-07-10 19:37:10.496717 robocorp_log-2.3.0/src/robocorp/log/_rewrite_ast_add_callbacks.py
--rw-r--r--   0        0        0     9227 2023-07-10 19:37:10.496717 robocorp_log-2.3.0/src/robocorp/log/_rewrite_filtering.py
--rw-r--r--   0        0        0    12755 2023-07-10 19:37:10.496717 robocorp_log-2.3.0/src/robocorp/log/_rewrite_importhook.py
--rw-r--r--   0        0        0    11687 2023-07-10 19:37:10.496717 robocorp_log-2.3.0/src/robocorp/log/_robo_logger.py
--rw-r--r--   0        0        0    67873 2023-07-10 19:37:10.496717 robocorp_log-2.3.0/src/robocorp/log/_robo_output_impl.py
--rw-r--r--   0        0        0     1436 2023-07-10 19:37:10.496717 robocorp_log-2.3.0/src/robocorp/log/_sensitive_variable_names.py
--rw-r--r--   0        0        0     1915 2023-07-10 19:37:10.496717 robocorp_log-2.3.0/src/robocorp/log/_suppress_helper.py
--rw-r--r--   0        0        0     7900 2023-07-10 19:37:10.496717 robocorp_log-2.3.0/src/robocorp/log/console.py
--rw-r--r--   0        0        0     1413 2023-07-10 19:37:10.496717 robocorp_log-2.3.0/src/robocorp/log/protocols.py
--rw-r--r--   0        0        0        0 2023-07-10 19:37:10.496717 robocorp_log-2.3.0/src/robocorp/log/py.typed
--rw-r--r--   0        0        0     8035 2023-07-10 19:37:10.496717 robocorp_log-2.3.0/src/robocorp/log/redirect.py
--rw-r--r--   0        0        0     6424 1970-01-01 00:00:00.000000 robocorp_log-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-07-19 12:36:32.625527 robocorp_log-2.4.0/LICENSE
+-rw-r--r--   0        0        0     5557 2023-07-19 12:36:32.625527 robocorp_log-2.4.0/README.md
+-rw-r--r--   0        0        0     1297 2023-07-19 12:36:32.629527 robocorp_log-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0    38636 2023-07-19 12:36:32.629527 robocorp_log-2.4.0/src/robocorp/log/__init__.py
+-rw-r--r--   0        0        0    17963 2023-07-19 12:36:32.633527 robocorp_log-2.4.0/src/robocorp/log/_ast_utils.py
+-rw-r--r--   0        0        0    15297 2023-07-19 12:36:32.633527 robocorp_log-2.4.0/src/robocorp/log/_auto_logging_setup.py
+-rw-r--r--   0        0        0    14416 2023-07-19 12:36:32.633527 robocorp_log-2.4.0/src/robocorp/log/_config.py
+-rw-r--r--   0        0        0      696 2023-07-19 12:36:32.633527 robocorp_log-2.4.0/src/robocorp/log/_convert_units.py
+-rw-r--r--   0        0        0     7143 2023-07-19 12:36:32.633527 robocorp_log-2.4.0/src/robocorp/log/_decoder.py
+-rw-r--r--   0        0        0     7193 2023-07-19 12:36:32.633527 robocorp_log-2.4.0/src/robocorp/log/_decoder_spec.py
+-rw-r--r--   0        0        0   805892 2023-07-19 12:37:29.592748 robocorp_log-2.4.0/src/robocorp/log/_index_v3.py
+-rw-r--r--   0        0        0     7077 2023-07-19 12:36:32.633527 robocorp_log-2.4.0/src/robocorp/log/_lifecycle_hooks.py
+-rw-r--r--   0        0        0     1128 2023-07-19 12:36:32.633527 robocorp_log-2.4.0/src/robocorp/log/_logger_instances.py
+-rw-r--r--   0        0        0     1208 2023-07-19 12:36:32.633527 robocorp_log-2.4.0/src/robocorp/log/_null.py
+-rw-r--r--   0        0        0      886 2023-07-19 12:36:32.633527 robocorp_log-2.4.0/src/robocorp/log/_obj_info_repr.py
+-rw-r--r--   0        0        0      396 2023-07-19 12:36:32.633527 robocorp_log-2.4.0/src/robocorp/log/_on_exit_context_manager.py
+-rw-r--r--   0        0        0    32317 2023-07-19 12:36:32.633527 robocorp_log-2.4.0/src/robocorp/log/_rewrite_ast_add_callbacks.py
+-rw-r--r--   0        0        0     9227 2023-07-19 12:36:32.633527 robocorp_log-2.4.0/src/robocorp/log/_rewrite_filtering.py
+-rw-r--r--   0        0        0    12755 2023-07-19 12:36:32.633527 robocorp_log-2.4.0/src/robocorp/log/_rewrite_importhook.py
+-rw-r--r--   0        0        0    11687 2023-07-19 12:36:32.633527 robocorp_log-2.4.0/src/robocorp/log/_robo_logger.py
+-rw-r--r--   0        0        0    67873 2023-07-19 12:36:32.633527 robocorp_log-2.4.0/src/robocorp/log/_robo_output_impl.py
+-rw-r--r--   0        0        0     1436 2023-07-19 12:36:32.633527 robocorp_log-2.4.0/src/robocorp/log/_sensitive_variable_names.py
+-rw-r--r--   0        0        0     1915 2023-07-19 12:36:32.633527 robocorp_log-2.4.0/src/robocorp/log/_suppress_helper.py
+-rw-r--r--   0        0        0     7900 2023-07-19 12:36:32.633527 robocorp_log-2.4.0/src/robocorp/log/console.py
+-rw-r--r--   0        0        0     1505 2023-07-19 12:36:32.633527 robocorp_log-2.4.0/src/robocorp/log/protocols.py
+-rw-r--r--   0        0        0        0 2023-07-19 12:36:32.633527 robocorp_log-2.4.0/src/robocorp/log/py.typed
+-rw-r--r--   0        0        0     7268 2023-07-19 12:36:32.633527 robocorp_log-2.4.0/src/robocorp/log/pyproject_config.py
+-rw-r--r--   0        0        0     8035 2023-07-19 12:36:32.633527 robocorp_log-2.4.0/src/robocorp/log/redirect.py
+-rw-r--r--   0        0        0     6424 1970-01-01 00:00:00.000000 robocorp_log-2.4.0/PKG-INFO
```

### Comparing `robocorp_log-2.3.0/LICENSE` & `robocorp_log-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robocorp_log-2.3.0/README.md` & `robocorp_log-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_log-2.3.0/pyproject.toml` & `robocorp_log-2.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-log"
-version = "2.3.0"
+version = "2.4.0"
 description = "Automatic trace logging for Python"
 authors = [
     "Fabio Zadrozny <fabio@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robo/"
 license = "Apache-2.0"
```

### Comparing `robocorp_log-2.3.0/src/robocorp/log/__init__.py` & `robocorp_log-2.4.0/src/robocorp/log/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from .protocols import IReadLines, LogHTMLStyle, OptExcInfo, Status
 import enum
 from types import TracebackType
 
 if typing.TYPE_CHECKING:
     from ._robo_logger import _RoboLogger
 
-__version__ = "2.3.0"
+__version__ = "2.4.0"
 version_info = [int(x) for x in __version__.split(".")]
 
 from . import _config
 
 # --- Export parts of the public API below (imports above aren't part of
 # the public API).
```

### Comparing `robocorp_log-2.3.0/src/robocorp/log/_ast_utils.py` & `robocorp_log-2.4.0/src/robocorp/log/_ast_utils.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-2.3.0/src/robocorp/log/_auto_logging_setup.py` & `robocorp_log-2.4.0/src/robocorp/log/_auto_logging_setup.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-2.3.0/src/robocorp/log/_config.py` & `robocorp_log-2.4.0/src/robocorp/log/_config.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-2.3.0/src/robocorp/log/_convert_units.py` & `robocorp_log-2.4.0/src/robocorp/log/_convert_units.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-2.3.0/src/robocorp/log/_decoder.py` & `robocorp_log-2.4.0/src/robocorp/log/_decoder.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-2.3.0/src/robocorp/log/_decoder_spec.py` & `robocorp_log-2.4.0/src/robocorp/log/_decoder_spec.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-2.3.0/src/robocorp/log/_index_v3.py` & `robocorp_log-2.4.0/src/robocorp/log/_index_v3.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-2.3.0/src/robocorp/log/_lifecycle_hooks.py` & `robocorp_log-2.4.0/src/robocorp/log/_lifecycle_hooks.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-2.3.0/src/robocorp/log/_logger_instances.py` & `robocorp_log-2.4.0/src/robocorp/log/_logger_instances.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-2.3.0/src/robocorp/log/_null.py` & `robocorp_log-2.4.0/src/robocorp/log/_null.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-2.3.0/src/robocorp/log/_obj_info_repr.py` & `robocorp_log-2.4.0/src/robocorp/log/_obj_info_repr.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-2.3.0/src/robocorp/log/_rewrite_ast_add_callbacks.py` & `robocorp_log-2.4.0/src/robocorp/log/_rewrite_ast_add_callbacks.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-2.3.0/src/robocorp/log/_rewrite_filtering.py` & `robocorp_log-2.4.0/src/robocorp/log/_rewrite_filtering.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-2.3.0/src/robocorp/log/_rewrite_importhook.py` & `robocorp_log-2.4.0/src/robocorp/log/_rewrite_importhook.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-2.3.0/src/robocorp/log/_robo_logger.py` & `robocorp_log-2.4.0/src/robocorp/log/_robo_logger.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-2.3.0/src/robocorp/log/_robo_output_impl.py` & `robocorp_log-2.4.0/src/robocorp/log/_robo_output_impl.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-2.3.0/src/robocorp/log/_sensitive_variable_names.py` & `robocorp_log-2.4.0/src/robocorp/log/_sensitive_variable_names.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-2.3.0/src/robocorp/log/_suppress_helper.py` & `robocorp_log-2.4.0/src/robocorp/log/_suppress_helper.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-2.3.0/src/robocorp/log/console.py` & `robocorp_log-2.4.0/src/robocorp/log/console.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-2.3.0/src/robocorp/log/protocols.py` & `robocorp_log-2.4.0/src/robocorp/log/protocols.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from types import TracebackType
-from typing import Literal, Protocol, Union, Sequence
+from typing import Literal, Protocol, Sequence, Union
 
 ExcInfo = tuple[type[BaseException], BaseException, TracebackType]
 OptExcInfo = Union[ExcInfo, tuple[None, None, None]]
 
 LogHTMLStyle = Literal["standalone", "vscode"]
 
 
 class IReadLines(Protocol):
     def readlines(self) -> Sequence[str]:
         pass
 
 
+class IContextErrorReport(Protocol):
+    def show_error(self, message: str):
+        pass
+
+
 # Note: this is a bit messy as we're mixing task states with log levels.
 # Note2: This is for the log.html and not really for user APIs.
 class Status:
     NOT_RUN = "NOT_RUN"  # Initial status for a task which is not run.
     PASS = "PASS"  # Used for task pass
     FAIL = "FAIL"  # Used for task failure
```

### Comparing `robocorp_log-2.3.0/src/robocorp/log/redirect.py` & `robocorp_log-2.4.0/src/robocorp/log/redirect.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-2.3.0/PKG-INFO` & `robocorp_log-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-log
-Version: 2.3.0
+Version: 2.4.0
 Summary: Automatic trace logging for Python
 Home-page: https://github.com/robocorp/robo/
 License: Apache-2.0
 Author: Fabio Zadrozny
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

