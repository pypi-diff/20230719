# Comparing `tmp/py4web_debug_tools-1.0.0.tar.gz` & `tmp/py4web_debug_tools-1.1.0.tar.gz`

## Comparing `py4web_debug_tools-1.0.0.tar` & `py4web_debug_tools-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/py4web_debug/__about__.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/py4web_debug/__init__.py
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/py4web_debug/core.py
--rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/py4web_debug/debugbar.py
--rw-r--r--   0        0        0     3443 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/py4web_debug/dumping.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/py4web_debug/env.py
--rw-r--r--   0        0        0     4250 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/py4web_debug/internals.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/py4web_debug/wsgi.py
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/py4web_debug/templates/debugbar.html
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/py4web_debug/templates/dumpdie.html
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/py4web_debug/templates/error_default.html
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/py4web_debug/templates/fancy_dumpdie.html
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/.gitignore
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/README.md
--rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 py4web_debug_tools-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.0/src/py4web_debug/__about__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.0/src/py4web_debug/__init__.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.0/src/py4web_debug/_internals.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.0/src/py4web_debug/core.py
+-rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.0/src/py4web_debug/debugbar.py
+-rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.0/src/py4web_debug/dumping.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.0/src/py4web_debug/env.py
+-rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.0/src/py4web_debug/internals.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.0/src/py4web_debug/py.typed
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.0/src/py4web_debug/wsgi.py
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.0/src/py4web_debug/templates/debugbar.html
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.0/src/py4web_debug/templates/dumpdie.html
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.0/src/py4web_debug/templates/error_default.html
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.0/src/py4web_debug/templates/fancy_dumpdie.html
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.0/.gitignore
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.0/README.md
+-rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 py4web_debug_tools-1.1.0/PKG-INFO
```

### Comparing `py4web_debug_tools-1.0.0/CHANGELOG.md` & `py4web_debug_tools-1.1.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.1.0 (2023-07-19)
+
+
 ## v1.0.0 (2023-07-17)
 ### Feature
 * **config:** Multiple minor changes: ([`bb14fec`](https://github.com/trialandsuccess/py4web-debug-tools/commit/bb14fec07780826eb7f550cb9c5d0ed24df1f8b3))
 * **debugbar:** Added required files ([`afc690f`](https://github.com/trialandsuccess/py4web-debug-tools/commit/afc690fb96ec2c9d54547434caffe7c1469302b1))
 * **p4w-debug:** Initial module setup ([`b36c53c`](https://github.com/trialandsuccess/py4web-debug-tools/commit/b36c53c30206189bfcfcbea1c7236f12ae8becab))
 
 ### Fix
```

### Comparing `py4web_debug_tools-1.0.0/py4web_debug/core.py` & `py4web_debug_tools-1.1.0/src/py4web_debug/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import typing
 from dataclasses import dataclass
 
 from py4web import DAL as P4WDAL
 
 from .debugbar import DebugBar, DummyDebugBar
 from .env import is_debug
-from .internals import patch_py4
+from .internals import ContextDict, patch_py4
 
 # in: context, out: string
-RendererMethod = typing.Callable[[typing.Dict[str, typing.Any]], str]
+RendererMethod = typing.Callable[[ContextDict], str]
 
 
 @dataclass
 class ErrorpageSettings:
     enabled: bool
 
 
@@ -49,58 +49,61 @@
         errorpage_enabled: bool = None,  # value of 'enabled' is used by default
         errorpage_renderer: RendererMethod = None,
         # debugbar settings:
         debugbar_enabled: bool = None,  # value of 'enabled' is used by default
         debugbar_fancy_rendering: bool = True,
         debugbar_style: typing.Literal["bootstrap"] = "bootstrap",
         debugbar_slow_threshold_ms: int = 10,
-    ):
+    ) -> None:
         """
         By default, on_off looks at PY4WEB_DEBUG_MODE in the env
 
         @todo: debugbar style (bootstrap/default, bulma, ...)
         """
         if enabled is None:
             enabled = is_debug()
 
         self.db = db
         self.enabled = enabled
 
         self.IS_DEBUG = enabled
 
         self.config = InternalConfig(
-            errorpage=ErrorpageSettings(enabled=errorpage_enabled in (True, None)),
+            errorpage=ErrorpageSettings(enabled=errorpage_enabled in {True, None}),
             # todo: more
-            debugbar=DebugbarSettings(enabled=debugbar_enabled in (True, None)),
+            debugbar=DebugbarSettings(enabled=debugbar_enabled in {True, None}),
             # todo: more
         )
 
         if enabled:
             if self.config.errorpage.enabled:
                 patch_py4(errorpage_renderer)
 
             if self.config.debugbar.enabled:
                 if not db:
                     raise ValueError("`db` variable should be provided when using the debug bar!")
+
                 self.debug_bar = DebugBar(
                     db,
                     debugbar_fancy_rendering,
                     debugbar_style,
                     debugbar_slow_threshold_ms,
                 )
 
             if set_env_var:
                 # will change the result of is_debug (hopefully)
                 os.environ["PY4WEB_DEBUG_MODE"] = "1"
         else:
             self.debug_bar = DummyDebugBar()
 
-    def set_renderer(self, cb: RendererMethod):
+    def set_renderer(self, cb: RendererMethod) -> None:
         # swap the errorpage_renderer
         if not (self.enabled and self.config.errorpage.enabled):
             # do nothing
             return
 
         patch_py4.renderer = cb
 
 
 tools = DebugTools()
+
+__all__ = ["tools", "patch_py4", "ContextDict"]
```

### Comparing `py4web_debug_tools-1.0.0/py4web_debug/debugbar.py` & `py4web_debug_tools-1.1.0/src/py4web_debug/debugbar.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 import os
 import typing
 import warnings
 from collections import Counter
+from inspect import FrameInfo
 
 import yatl
 from py4web import request
 from py4web.core import Fixture, Template
+from pydal import DAL
 from yatl import XML
 
+from ._internals import TypedFixture
 from .dumping import dump
 from .env import is_debug
 
 
-def _fmt_callframe(cf):
+def _fmt_callframe(cf: FrameInfo) -> str:
     # 0: frame
     # 1: file
     # 2: lineno
     # 3: function
     # 4: context
     filename = cf[1].split("/")[-1]
     function = cf[3]
     return f"{filename}:{function}"
 
 
-def catch(*context, levels=3, _from=1):
+def catch(*context: typing.Any, levels: int = 3, _from: int = 1) -> None:
     """
     Log usages of this method
     """
     _ = "You should only use catch() while debugging!!!!"
 
     if not is_debug():
         warnings.warn(_)
@@ -48,15 +51,15 @@
             "callframes": cfl,
             "context": context,
         }
     )
     setattr(request, "_catch", c)
 
 
-def _debugbar(data, template="templates/debugbar.html", fancy=True):
+def _debugbar(data: dict[str, typing.Any], template: str = "templates/debugbar.html", fancy: bool = True) -> str:
     fname = os.path.join(os.path.dirname(__file__), template)
 
     if not data.get("queries"):
         data["queries"] = []
 
     if not data.get("duplicate_queries"):
         data["duplicate_queries"] = []
@@ -68,43 +71,44 @@
         data["catch"] = []
 
     if not data.get("json_context"):
         data["json_context"] = []
 
     data["fancy"] = fancy
 
-    return yatl.render(
+    result = yatl.render(
         filename=fname,
         context={"BEAUTIFY": yatl.BEAUTIFY, **data},
         delimiters="[[ ]]",
     )
+    return typing.cast(str, result)
 
 
-def render_debugbar(*contexts, fancy=True):
+def render_debugbar(*contexts: typing.Any, fancy: bool = True) -> str:
     """
     Contexts should be:
     1. debug data (filled in the Debug Bar Fixture)
     2. on_success context, after rendering (so output = html), including other info such as fixtures
     3. context['output'] from before it is rendered by the template
     """
 
     debug_data, _, input_data = contexts
-    return _debugbar(debug_data, fancy=fancy) + "</html>"
+    return f"{_debugbar(debug_data, fancy=fancy)}</html>"
 
 
-def debugbar_template(_: Fixture, debug_data: dict, fancy=True):
+def debugbar_template(_: Fixture, debug_data: dict[str, typing.Any], fancy: bool = True) -> None:
     """
     debug_data is reset and filled every request
     """
 
     if not hasattr(Template, "_on_success"):
         # DON'T overwrite existing _on_success because that will lead to recursion...
         Template._on_success = Template.on_success
 
-    def _on_request(self, context: dict):
+    def _on_request(self: Template, context: dict[str, typing.Any]) -> None:
         if not (context and context.get("output")):
             # do nothing
             return
 
         pre_render_output = context["output"].copy() if isinstance(context.get("output"), dict) else {}
 
         Template._on_success(self, context)
@@ -112,15 +116,15 @@
         # only replace actual templates (= end in /html)
         if (output := context["output"]) and isinstance(output, str):
             context["output"] = output.replace(
                 "</html>",
                 render_debugbar(debug_data, context, pre_render_output, fancy=fancy),
             )
 
-    def on_success(self, context: dict):
+    def on_success(self: Template, context: dict[str, typing.Any]) -> None:
         try:
             _on_request(self, context)
         finally:
             # after output has been rendered, reset to original on_success (so next request will reset):
             Template.on_success = Template._on_success
 
     Template.on_success = on_success
@@ -143,92 +147,86 @@
             value[key] = _prune_long_values(item)
     elif isinstance(value, str | bytes) and len(value) > 50:
         return "[pruned due to length]"
 
     return value
 
 
-def convert_for_debugbar(value):
+def convert_for_debugbar(value: typing.Any) -> str:
     """
     Returns: a dict or list that can be converted to json
     """
     # deprecated: as dict is now managed by dump()
-    # if hasattr(value, "as_dict"):
-    #     value = value.as_dict()
-    #
-    # elif hasattr(value, "_asdict"):
-    #     value = value._asdict()
 
-    value = _prune_long_values(value)
-    return value
+    return _prune_long_values(value)
 
 
-class DummyDebugBar(Fixture):
+class DummyDebugBar(TypedFixture):
     ...
 
 
-class DebugBar(Fixture):
+class DebugBar(TypedFixture):
     queries: typing.ClassVar[list[str]] = []  # mutable but DONT OVERWRITE !!!
     debug_data: typing.ClassVar[dict[str, typing.Any]] = {}  # mutable but DON'T OVERWRITE!!
 
     def __init__(
         self,
-        db,
+        db: DAL,
         fancy_rendering: bool,
         bar_style: typing.Literal["bootstrap"],
         slow_threshold_ms: int,
     ):
         self.__prerequisites__ = [db]
         self.db = db
         self.fancy = fancy_rendering
         self.style = bar_style
         self.threshold_ms = slow_threshold_ms
 
-    def _find_duplicate_queries(self, timings):
+    def _find_duplicate_queries(self, timings: list[tuple[str, float]]) -> dict[str, int]:
         """
         Returns: a dict of queries (+ count as value) that are executed more than once
         """
         counts = Counter(query for query, _ in timings)
 
         return {query: count for query, count in counts.items() if count > 1}
 
-    def _find_slow_queries(self, timings: list[tuple[str, float]], threshold_ms: int):
+    def _find_slow_queries(self, timings: list[tuple[str, float]], threshold_ms: int) -> list[dict[str, str]]:
         """
         Returns: a list of queries that took longer than threshold_ms
         """
         return [{q: f"{round(t * 1000, 5)}ms"} for q, t in timings if t > threshold_ms / 1000]
 
-    def on_request(self, _: dict[str, typing.Any]):
+    def on_request(self, _: dict[str, typing.Any]) -> None:
         db = self.db
         # these two are scoped to the request
         self.queries.clear()  # DON'T OVERWRITE WITH = [] !!!
         self.debug_data.clear()  # idem
         db._timings.clear()
 
         self.debug_data["queries"] = db._timings
         setattr(request, "_catch", [])
 
         # empty before debug_pydal adds new queries
         # patch the Template.on_success:
         debugbar_template(self, self.debug_data, fancy=self.fancy)
 
-    def filter_context(self, input_data: dict):
+    def filter_context(self, input_data: dict[str, typing.Any]) -> dict[str, str]:
         """
         Returns: a dict with all keys that are not in __ignored \
          and it's values shortened (nested long values are pruned).
         """
         if not input_data or not isinstance(input_data, dict):
             return {}
 
         __ignored = input_data.get("__ignore", [])
 
         # remove common helper methods etc.
         return {k: convert_for_debugbar(v) for k, v in input_data.items() if k not in __ignored}
 
-    def on_success(self, context):
+    def on_success(self, context: dict[str, typing.Any]) -> None:
         self.debug_data["duplicate_queries"] = self._find_duplicate_queries(self.debug_data["queries"])
         self.debug_data["slow_queries"] = self._find_slow_queries(
             self.debug_data["queries"], threshold_ms=self.threshold_ms
         )
 
         try:
             json_context = dump(self.filter_context(context["output"]), with_headers=False)
```

### Comparing `py4web_debug_tools-1.0.0/py4web_debug/dumping.py` & `py4web_debug_tools-1.1.0/src/py4web_debug/dumping.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,17 +5,49 @@
 import pydal.objects
 from configurablejson import ConfigurableJsonEncoder, JSONRule
 from py4web import response
 
 from .env import is_debug
 
 
+class PossiblyAsDict(typing.Protocol):
+    def as_dict(self) -> dict[str, typing.Any]:
+        ...
+
+    def asdict(self) -> dict[str, typing.Any]:
+        ...
+
+    def _asdict(self) -> dict[str, typing.Any]:
+        ...
+
+    def _as_dict(self) -> dict[str, typing.Any]:
+        ...
+
+    def to_dict(self) -> dict[str, typing.Any]:
+        ...
+
+    def todict(self) -> dict[str, typing.Any]:
+        ...
+
+    def _todict(self) -> dict[str, typing.Any]:
+        ...
+
+    def _to_dict(self) -> dict[str, typing.Any]:
+        ...
+
+    def __json__(self) -> dict[str, typing.Any]:
+        ...
+
+    def as_list(self) -> list[typing.Any]:
+        ...
+
+
 class DDJsonEncoder(ConfigurableJsonEncoder):
     @staticmethod
-    def _default(o) -> str:
+    def _default(o: PossiblyAsDict) -> dict[str, typing.Any] | list[typing.Any] | str:
         if hasattr(o, "as_list"):
             # note: prefer as_list now as not every Rows may have an id (= default key of as_dict)
             return o.as_list()
         # more as list stuff?
 
         if hasattr(o, "as_dict"):
             return o.as_dict()
@@ -41,33 +73,41 @@
     @staticmethod
     def is_probably_namedtuple(o: typing.Any) -> bool:
         """
         Try to guess if 'o' is a Named Tuple or something else.
         """
         return isinstance(o, tuple) and hasattr(o, "_fields")
 
-    def rules(self, o, with_default=True) -> JSONRule:
+    def rules(self, o: typing.Any, with_default: bool = True) -> JSONRule:
         """
         Custom rules for the DD json: set to list and namedtuple to dict
         # NOTE: with_default is (probably) false anyway!!!!
         """
 
         _type = typing.NamedTuple if self.is_probably_namedtuple(o) else type(o)
 
-        return {
+        rules: dict[type, JSONRule] = {
             # convert set to list
             set: JSONRule(preprocess=lambda o: list(o)),
             # convert namedtuple to dict
             typing.NamedTuple: JSONRule(preprocess=self._default),
             pydal.objects.Row: JSONRule(preprocess=lambda row: row.as_dict()),
             pydal.objects.Rows: JSONRule(preprocess=lambda row: row.as_list()),
-        }.get(_type, JSONRule(transform=self._default) if with_default else None)
+        }
+
+        if rule := rules.get(typing.cast(type, _type)):
+            return rule
+        elif rule is None and with_default:
+            return JSONRule(transform=self._default)
+        else:
+            # empty rule:
+            return JSONRule()
 
 
-def dump(data: typing.Iterable, with_headers=True) -> str:
+def dump(data: typing.Iterable[typing.Any], with_headers: bool = True) -> str:
     """
     Helper to json dump some data with custom converter and headers
     """
     if with_headers:
         response.headers["Content-Type"] = "application/json"
 
     return json.dumps(data, indent=2, cls=DDJsonEncoder)
@@ -94,15 +134,15 @@
     """
     Custom Exception used to catch dd() in py4web error page -> JSON only output
     """
 
     pass
 
 
-def dd(*data, fancy=True, api=False):
+def dd(*data: typing.Any, fancy: bool = True, api: bool = False) -> None:
     """
     Dump and Die:
     Show args as JSON an halt the rest of the request
     (useful for debugging fifty levels deep in some helper method)
 
     """
     if len(data) == 1:
```

### Comparing `py4web_debug_tools-1.0.0/py4web_debug/internals.py` & `py4web_debug_tools-1.1.0/src/py4web_debug/internals.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,80 @@
 import functools
 import http.client
 import json
 import logging
 import os
 import re
-import traceback
+import traceback as tb
 import typing
 
 import ombott as bottle
 import yatl
 from py4web import HTTP, action, response
 from py4web.core import (
     REGEX_APPJSON,
     Template,
     dumps,
     error_logger,
     get_error_snapshot,
     request,
 )
+from typing_extensions import NotRequired
 from yatl import XML
 
 
+class ContextDict(typing.TypedDict):
+    code: int
+    message: typing.Optional[str]
+    button_text: typing.Optional[str]
+    href: str
+    color: typing.Optional[str]
+    traceback: str
+    err_type: str
+    exception: typing.Optional[Exception]
+
+    XML: NotRequired[typing.Type[XML]]
+
+
+T_Renderer = typing.Callable[[ContextDict], str]
+AnyFunc = typing.Callable[..., typing.Any]
+
+
 def custom_error_page(
-    code,
-    button_text=None,
-    href="#",
-    color=None,
-    message=None,
-    traceback="",
-    err_type: str | typing.Type | None = None,
-    bare_exception=None,
-    renderer=None,
-):
+    code: int,
+    button_text: str = None,
+    href: str = "#",
+    color: str = None,
+    message: str = None,
+    traceback: str = "",
+    err_type: str | typing.Type[Exception] | None = None,
+    bare_exception: Exception = None,
+    renderer: T_Renderer = None,
+) -> str:
     if err_type and not isinstance(err_type, str):
         err_type = err_type.__name__
 
     # make sure the name is a string (but it probably already is:)
     err_type_name = str(err_type)
 
     if hasattr(Template, "_on_success"):
         # reset here on error, because on_error might not be called!
         Template.on_success = Template._on_success
         del Template._on_success
 
     message = http.client.responses[code].upper() if message is None else message
     color = color or {"4": "#F44336", "5": "#607D8B"}.get(str(code)[0], "#2196F3")
-    context = dict(
+    context: ContextDict = dict(
         code=code,
         message=message,
         button_text=button_text,
         href=href,
         color=color,
         traceback=traceback,
-        err_type=err_type,
+        err_type=err_type_name,
         exception=bare_exception,
     )
     # if client accepts 'application/json' - return json
     if re.search(REGEX_APPJSON, request.headers.get("accept", "")):
         response.status = code
         return json.dumps(context)
     # else - return html error-page
@@ -77,66 +95,69 @@
         # just bare exception
         return str(context["exception"])
 
     context["XML"] = XML
 
     fname = os.path.join(os.path.dirname(__file__), "templates", _tmpl)
     with open(fname) as f:
-        return yatl.render(
+        result = yatl.render(
             stream=f,
             context=context,
             delimiters="[[ ]]",
         )
+    return typing.cast(str, result)
 
 
-def patch_py4(renderer=None):
+class patch_py4:
     # THIS IS ONLY CALLED ONCE, WHEN tools.enable IS CALLED OR py4web_debug.wsgi IS USED!
+    renderer: T_Renderer | None = None
 
-    def custom_catch_errors(app_name, func):
-        """Catches and logs errors in an action; also sets request.app_name"""
-
-        # ^ THIS METHOD IS CALLED FOR EVERY ACTION DEFIFINED WITH @action
-
-        # v METHOD BELOW IS CALLED ON EVERY ERROR
-
-        @functools.wraps(func)
-        def wrapper(*func_args, **func_kwargs):
-            try:
-                request.app_name = app_name
-                ret = func(*func_args, **func_kwargs)
-                if isinstance(ret, dict):
-                    response.headers["Content-Type"] = "application/json"
-                    ret = dumps(ret)
-                return ret
-            except HTTP as http:
-                response.status = http.status
-                response.headers.update(http.headers)
-                return http.body
-            except bottle.HTTPResponse:
-                raise
-            except Exception as e:
-                snapshot = get_error_snapshot()
-                logging.error(snapshot["traceback"])
-                ticket_uuid = error_logger.log(request.app_name, snapshot) or "unknown"
-                response.status = 500
-
-                raise bottle.HTTPResponse(
-                    body=custom_error_page(
-                        500,
-                        button_text=ticket_uuid,
-                        href="/_dashboard/ticket/" + ticket_uuid,
-                        traceback=traceback.format_exc(),
-                        err_type=type(e),
-                        bare_exception=e,
-                        renderer=getattr(patch_py4, "renderer", None),
-                    ),
-                    status=500,
-                )
-
-        return wrapper
-
-    # prevent duplicate enabling:
-    if action.catch_errors.__qualname__ == "action.catch_errors":
-        action.catch_errors = custom_catch_errors
+    def __init__(self, renderer: T_Renderer = None):
+        def custom_catch_errors(app_name: str, func: AnyFunc) -> typing.Callable[..., str]:
+            """Catches and logs errors in an action; also sets request.app_name"""
+
+            # ^ THIS METHOD IS CALLED FOR EVERY ACTION DEFIFINED WITH @action
+
+            # v METHOD BELOW IS CALLED ON EVERY ERROR
+
+            @functools.wraps(func)
+            def wrapper(*func_args: typing.Any, **func_kwargs: typing.Any) -> str:
+                try:
+                    request.app_name = app_name
+                    ret = func(*func_args, **func_kwargs)
+                    if isinstance(ret, dict):
+                        response.headers["Content-Type"] = "application/json"
+                        ret = dumps(ret)
+                    return str(ret)
+                except HTTP as http:
+                    response.status = http.status
+                    response.headers.update(http.headers)
+                    return str(http.body)
+                except bottle.HTTPResponse:
+                    raise
+                except Exception as e:
+                    snapshot = get_error_snapshot()
+                    logging.error(snapshot["traceback"])
+                    ticket_uuid = error_logger.log(request.app_name, snapshot) or "unknown"
+                    response.status = 500
+
+                    raise bottle.HTTPResponse(
+                        body=custom_error_page(
+                            500,
+                            button_text=ticket_uuid,
+                            href=f"/_dashboard/ticket/{ticket_uuid}",
+                            traceback=tb.format_exc(),
+                            err_type=type(e),
+                            bare_exception=e,
+                            renderer=getattr(patch_py4, "renderer", None),
+                        ),
+                        status=500,
+                    )
+
+            return wrapper
+
+        # prevent duplicate enabling:
+        if action.catch_errors.__qualname__ == "action.catch_errors":
+            action.catch_errors = custom_catch_errors
 
-    # allows swapping renderer on the fly with tools.set_renderer():
-    patch_py4.renderer = renderer
+        # allows swapping renderer on the fly with tools.set_renderer():
+        patch_py4.renderer = renderer
```

### Comparing `py4web_debug_tools-1.0.0/py4web_debug/templates/debugbar.html` & `py4web_debug_tools-1.1.0/src/py4web_debug/templates/debugbar.html`

 * *Files identical despite different names*

### Comparing `py4web_debug_tools-1.0.0/py4web_debug/templates/error_default.html` & `py4web_debug_tools-1.1.0/src/py4web_debug/templates/error_default.html`

 * *Files identical despite different names*

### Comparing `py4web_debug_tools-1.0.0/py4web_debug/templates/fancy_dumpdie.html` & `py4web_debug_tools-1.1.0/src/py4web_debug/templates/fancy_dumpdie.html`

 * *Files identical despite different names*

### Comparing `py4web_debug_tools-1.0.0/README.md` & `py4web_debug_tools-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `py4web_debug_tools-1.0.0/pyproject.toml` & `py4web_debug_tools-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
+[template.plugins.default]
+src-layout = true
+
+[tool.setuptools.package-data]
+"py4web_debug" = ["py.typed"]
+
+[tool.hatch.build.targets.wheel]
+packages = ["src/py4web_debug"]
+
 [tool.hatch.build]
 artifacts = [
-    "py4web_debug/templates/*.html"
+    "src/py4web_debug/templates/*.html"
 ]
 
 [project]
 name = "py4web-debug-tools"
 dynamic = ["version"]
 description = 'Debug Tools for py4web'
 readme = "README.md"
@@ -39,35 +48,31 @@
 dev = [
     "su6[all]",
     "hatch",
 ]
 
 
 [tool.hatch.version]
-path = "py4web_debug/__about__.py"
+path = "src/py4web_debug/__about__.py"
 
 [tool.semantic_release]
 branch = "master"
-version_variable = "py4web_debug/__about__.py:__version__"
+version_variable = "src/py4web_debug/__about__.py:__version__"
 change_log = "CHANGELOG.md"
 upload_to_repository = false
 upload_to_release = false
 build_command = "hatch build"
 
 
 [tool.su6]
-directory = "py4web_debug"
+directory = "src"
 include = []
 exclude = ["pytest"]
 stop-after-first-failure = true
 
-[tool.su6.svelte-check]
-target = "pytest_examples/no_issues"
-node_modules = "pytest_examples/node_modules"
-
 [tool.black]
 target-version = ["py311"]
 line-length = 120
 # 'extend-exclude' excludes files or directories in addition to the defaults
 extend-exclude = '''
 # A regex preceded with ^/ will apply only to files and directories
 # in the root of the project.
```

### Comparing `py4web_debug_tools-1.0.0/PKG-INFO` & `py4web_debug_tools-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web-debug-tools
-Version: 1.0.0
+Version: 1.1.0
 Summary: Debug Tools for py4web
 Project-URL: Documentation, https://github.com/trialandsuccess/py4web-debug-tools#readme
 Project-URL: Issues, https://github.com/trialandsuccess/py4web-debug-tools/issues
 Project-URL: Source, https://github.com/trialandsuccess/py4web-debug-tools
 Author-email: Robin van der Noord <contact@trialandsuccess.nl>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
```

