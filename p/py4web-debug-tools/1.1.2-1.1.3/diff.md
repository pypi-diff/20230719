# Comparing `tmp/py4web_debug_tools-1.1.2.tar.gz` & `tmp/py4web_debug_tools-1.1.3.tar.gz`

## Comparing `py4web_debug_tools-1.1.2.tar` & `py4web_debug_tools-1.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/CHANGELOG.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/__about__.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/__init__.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/_internals.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/core.py
--rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/debugbar.py
--rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/dumping.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/env.py
--rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/internals.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/py.typed
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/wsgi.py
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/templates/debugbar.html
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/templates/dumpdie.html
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/templates/error_default.html
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/src/py4web_debug/templates/fancy_dumpdie.html
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/.gitignore
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/README.md
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.3/src/py4web_debug/__about__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.3/src/py4web_debug/__init__.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.3/src/py4web_debug/_internals.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.3/src/py4web_debug/core.py
+-rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.3/src/py4web_debug/debugbar.py
+-rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.3/src/py4web_debug/dumping.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.3/src/py4web_debug/env.py
+-rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.3/src/py4web_debug/internals.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.3/src/py4web_debug/py.typed
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.3/src/py4web_debug/wsgi.py
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.3/src/py4web_debug/templates/debugbar.html
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.3/src/py4web_debug/templates/dumpdie.html
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.3/src/py4web_debug/templates/error_default.html
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.3/src/py4web_debug/templates/fancy_dumpdie.html
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.3/.gitignore
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.3/README.md
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.3/PKG-INFO
```

### Comparing `py4web_debug_tools-1.1.2/CHANGELOG.md` & `py4web_debug_tools-1.1.3/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.1.3 (2023-07-19)
+### Fix
+* Error page renderer can also be False (in addition to None or a method) ([`41d33aa`](https://github.com/trialandsuccess/py4web-debug-tools/commit/41d33aae9e307034b2818641c041f1dd6c8364fc))
+
 ## v1.1.2 (2023-07-19)
 ### Fix
 * Wrapper can also return an HTTP response! ([`4431d80`](https://github.com/trialandsuccess/py4web-debug-tools/commit/4431d8094162dc9100aab2798571b87e5a076ed4))
 
 ## v1.1.1 (2023-07-19)
 ### Fix
 * Bump `configurable-json` to new typed version ([`52fa55a`](https://github.com/trialandsuccess/py4web-debug-tools/commit/52fa55a3eb0d8e95064ddb9ecae820a2fa229a9a))
```

### Comparing `py4web_debug_tools-1.1.2/src/py4web_debug/_internals.py` & `py4web_debug_tools-1.1.3/src/py4web_debug/_internals.py`

 * *Files identical despite different names*

### Comparing `py4web_debug_tools-1.1.2/src/py4web_debug/core.py` & `py4web_debug_tools-1.1.3/src/py4web_debug/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,18 +3,15 @@
 import typing
 from dataclasses import dataclass
 
 from py4web import DAL as P4WDAL
 
 from .debugbar import DebugBar, DummyDebugBar
 from .env import is_debug
-from .internals import ContextDict, patch_py4
-
-# in: context, out: string
-RendererMethod = typing.Callable[[ContextDict], str]
+from .internals import T_Renderer, patch_py4
 
 
 @dataclass
 class ErrorpageSettings:
     enabled: bool
 
 
@@ -43,15 +40,15 @@
         self,
         # general settings:
         db: P4WDAL = None,
         enabled: bool | None = None,  # OVERWRITES errorpage_enabled and debugbar_enabled
         set_env_var: bool = True,
         # error screen settings:
         errorpage_enabled: bool = None,  # value of 'enabled' is used by default
-        errorpage_renderer: RendererMethod = None,
+        errorpage_renderer: T_Renderer = None,
         # debugbar settings:
         debugbar_enabled: bool = None,  # value of 'enabled' is used by default
         debugbar_fancy_rendering: bool = True,
         debugbar_style: typing.Literal["bootstrap"] = "bootstrap",
         debugbar_slow_threshold_ms: int = 10,
     ) -> None:
         """
@@ -91,19 +88,19 @@
 
             if set_env_var:
                 # will change the result of is_debug (hopefully)
                 os.environ["PY4WEB_DEBUG_MODE"] = "1"
         else:
             self.debug_bar = DummyDebugBar()
 
-    def set_renderer(self, cb: RendererMethod) -> None:
+    def set_renderer(self, cb: T_Renderer) -> None:
         # swap the errorpage_renderer
         if not (self.enabled and self.config.errorpage.enabled):
             # do nothing
             return
 
         patch_py4.renderer = cb
 
 
 tools = DebugTools()
 
-__all__ = ["tools", "patch_py4", "ContextDict"]
+__all__ = ["tools", "patch_py4"]
```

### Comparing `py4web_debug_tools-1.1.2/src/py4web_debug/debugbar.py` & `py4web_debug_tools-1.1.3/src/py4web_debug/debugbar.py`

 * *Files identical despite different names*

### Comparing `py4web_debug_tools-1.1.2/src/py4web_debug/dumping.py` & `py4web_debug_tools-1.1.3/src/py4web_debug/dumping.py`

 * *Files identical despite different names*

### Comparing `py4web_debug_tools-1.1.2/src/py4web_debug/internals.py` & `py4web_debug_tools-1.1.3/src/py4web_debug/internals.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     traceback: str
     err_type: str
     exception: typing.Optional[Exception]
 
     XML: NotRequired[typing.Type[XML]]
 
 
-T_Renderer = typing.Callable[[ContextDict], str]
+T_Renderer = typing.Callable[[ContextDict], str] | typing.Literal[False]
 AnyFunc = typing.Callable[..., typing.Any]
 
 
 def custom_error_page(
     code: int,
     button_text: str = None,
     href: str = "#",
```

### Comparing `py4web_debug_tools-1.1.2/src/py4web_debug/templates/debugbar.html` & `py4web_debug_tools-1.1.3/src/py4web_debug/templates/debugbar.html`

 * *Files identical despite different names*

### Comparing `py4web_debug_tools-1.1.2/src/py4web_debug/templates/error_default.html` & `py4web_debug_tools-1.1.3/src/py4web_debug/templates/error_default.html`

 * *Files identical despite different names*

### Comparing `py4web_debug_tools-1.1.2/src/py4web_debug/templates/fancy_dumpdie.html` & `py4web_debug_tools-1.1.3/src/py4web_debug/templates/fancy_dumpdie.html`

 * *Files identical despite different names*

### Comparing `py4web_debug_tools-1.1.2/README.md` & `py4web_debug_tools-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `py4web_debug_tools-1.1.2/pyproject.toml` & `py4web_debug_tools-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py4web_debug_tools-1.1.2/PKG-INFO` & `py4web_debug_tools-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web-debug-tools
-Version: 1.1.2
+Version: 1.1.3
 Summary: Debug Tools for py4web
 Project-URL: Documentation, https://github.com/trialandsuccess/py4web-debug-tools#readme
 Project-URL: Issues, https://github.com/trialandsuccess/py4web-debug-tools/issues
 Project-URL: Source, https://github.com/trialandsuccess/py4web-debug-tools
 Author-email: Robin van der Noord <contact@trialandsuccess.nl>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
```

