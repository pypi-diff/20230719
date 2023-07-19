# Comparing `tmp/py4web_debug_tools-1.1.1.tar.gz` & `tmp/py4web_debug_tools-1.1.2.tar.gz`

## Comparing `py4web_debug_tools-1.1.1.tar` & `py4web_debug_tools-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.1/CHANGELOG.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.1/src/py4web_debug/__about__.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.1/src/py4web_debug/__init__.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.1/src/py4web_debug/_internals.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.1/src/py4web_debug/core.py
--rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.1/src/py4web_debug/debugbar.py
--rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.1/src/py4web_debug/dumping.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.1/src/py4web_debug/env.py
--rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.1/src/py4web_debug/internals.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.1/src/py4web_debug/py.typed
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.1/src/py4web_debug/wsgi.py
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.1/src/py4web_debug/templates/debugbar.html
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.1/src/py4web_debug/templates/dumpdie.html
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.1/src/py4web_debug/templates/error_default.html
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.1/src/py4web_debug/templates/fancy_dumpdie.html
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.1/.gitignore
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.1/README.md
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/__about__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/__init__.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/_internals.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/core.py
+-rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/debugbar.py
+-rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/dumping.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/env.py
+-rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/internals.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/py.typed
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/wsgi.py
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/templates/debugbar.html
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/templates/dumpdie.html
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/templates/error_default.html
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/templates/fancy_dumpdie.html
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/.gitignore
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/README.md
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/PKG-INFO
```

### Comparing `py4web_debug_tools-1.1.1/CHANGELOG.md` & `py4web_debug_tools-1.1.2/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.1.2 (2023-07-19)
+### Fix
+* Wrapper can also return an HTTP response! ([`4431d80`](https://github.com/trialandsuccess/py4web-debug-tools/commit/4431d8094162dc9100aab2798571b87e5a076ed4))
+
 ## v1.1.1 (2023-07-19)
 ### Fix
 * Bump `configurable-json` to new typed version ([`52fa55a`](https://github.com/trialandsuccess/py4web-debug-tools/commit/52fa55a3eb0d8e95064ddb9ecae820a2fa229a9a))
 
 ### Documentation
 * Updated changelog ([`15a9517`](https://github.com/trialandsuccess/py4web-debug-tools/commit/15a9517f149b9bff272306c64165e9e62845e8d0))
```

### Comparing `py4web_debug_tools-1.1.1/src/py4web_debug/_internals.py` & `py4web_debug_tools-1.1.2/src/py4web_debug/_internals.py`

 * *Files identical despite different names*

### Comparing `py4web_debug_tools-1.1.1/src/py4web_debug/core.py` & `py4web_debug_tools-1.1.2/src/py4web_debug/core.py`

 * *Files identical despite different names*

### Comparing `py4web_debug_tools-1.1.1/src/py4web_debug/debugbar.py` & `py4web_debug_tools-1.1.2/src/py4web_debug/debugbar.py`

 * *Files identical despite different names*

### Comparing `py4web_debug_tools-1.1.1/src/py4web_debug/dumping.py` & `py4web_debug_tools-1.1.2/src/py4web_debug/dumping.py`

 * *Files identical despite different names*

### Comparing `py4web_debug_tools-1.1.1/src/py4web_debug/internals.py` & `py4web_debug_tools-1.1.2/src/py4web_debug/internals.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 import re
 import traceback as tb
 import typing
 
 import ombott as bottle
 import yatl
+from ombott import HTTPResponse
 from py4web import HTTP, action, response
 from py4web.core import (
     REGEX_APPJSON,
     Template,
     dumps,
     error_logger,
     get_error_snapshot,
@@ -116,26 +117,26 @@
             """Catches and logs errors in an action; also sets request.app_name"""
 
             # ^ THIS METHOD IS CALLED FOR EVERY ACTION DEFIFINED WITH @action
 
             # v METHOD BELOW IS CALLED ON EVERY ERROR
 
             @functools.wraps(func)
-            def wrapper(*func_args: typing.Any, **func_kwargs: typing.Any) -> str:
+            def wrapper(*func_args: typing.Any, **func_kwargs: typing.Any) -> str | HTTPResponse:
                 try:
                     request.app_name = app_name
                     ret = func(*func_args, **func_kwargs)
                     if isinstance(ret, dict):
                         response.headers["Content-Type"] = "application/json"
                         ret = dumps(ret)
-                    return str(ret)
+                    return ret
                 except HTTP as http:
                     response.status = http.status
                     response.headers.update(http.headers)
-                    return str(http.body)
+                    return http.body
                 except bottle.HTTPResponse:
                     raise
                 except Exception as e:
                     snapshot = get_error_snapshot()
                     logging.error(snapshot["traceback"])
                     ticket_uuid = error_logger.log(request.app_name, snapshot) or "unknown"
                     response.status = 500
```

### Comparing `py4web_debug_tools-1.1.1/src/py4web_debug/templates/debugbar.html` & `py4web_debug_tools-1.1.2/src/py4web_debug/templates/debugbar.html`

 * *Files identical despite different names*

### Comparing `py4web_debug_tools-1.1.1/src/py4web_debug/templates/error_default.html` & `py4web_debug_tools-1.1.2/src/py4web_debug/templates/error_default.html`

 * *Files identical despite different names*

### Comparing `py4web_debug_tools-1.1.1/src/py4web_debug/templates/fancy_dumpdie.html` & `py4web_debug_tools-1.1.2/src/py4web_debug/templates/fancy_dumpdie.html`

 * *Files identical despite different names*

### Comparing `py4web_debug_tools-1.1.1/README.md` & `py4web_debug_tools-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `py4web_debug_tools-1.1.1/pyproject.toml` & `py4web_debug_tools-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py4web_debug_tools-1.1.1/PKG-INFO` & `py4web_debug_tools-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web-debug-tools
-Version: 1.1.1
+Version: 1.1.2
 Summary: Debug Tools for py4web
 Project-URL: Documentation, https://github.com/trialandsuccess/py4web-debug-tools#readme
 Project-URL: Issues, https://github.com/trialandsuccess/py4web-debug-tools/issues
 Project-URL: Source, https://github.com/trialandsuccess/py4web-debug-tools
 Author-email: Robin van der Noord <contact@trialandsuccess.nl>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
```

