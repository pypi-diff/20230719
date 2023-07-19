# Comparing `tmp/autometrics-0.6.tar.gz` & `tmp/autometrics-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autometrics-0.6.tar", max compression
+gzip compressed data, was "autometrics-0.7.tar", max compression
```

## Comparing `autometrics-0.6.tar` & `autometrics-0.7.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1022 2023-04-12 17:23:29.278864 autometrics-0.6/LICENSE
--rw-r--r--   0        0        0     9529 2023-06-23 15:57:11.581730 autometrics-0.6/README.md
--rw-r--r--   0        0        0     2081 2023-06-23 15:57:11.584556 autometrics-0.6/pyproject.toml
--rw-r--r--   0        0        0       53 2023-05-16 18:06:49.422047 autometrics-0.6/src/autometrics/__init__.py
--rw-r--r--   0        0        0       84 2023-06-20 09:32:43.127205 autometrics-0.6/src/autometrics/admin_panel/__init__.py
--rw-r--r--   0        0        0      574 2023-06-20 09:32:43.127678 autometrics-0.6/src/autometrics/admin_panel/function_registry.py
--rw-r--r--   0        0        0     1489 2023-06-23 15:57:11.585010 autometrics-0.6/src/autometrics/constants.py
--rw-r--r--   0        0        0     4967 2023-06-23 15:57:11.585208 autometrics-0.6/src/autometrics/decorator.py
--rw-r--r--   0        0        0     3050 2023-04-13 12:18:19.449416 autometrics-0.6/src/autometrics/objectives.py
--rw-r--r--   0        0        0     2197 2023-05-11 12:02:53.378737 autometrics-0.6/src/autometrics/prometheus_url.py
--rw-r--r--   0        0        0    12055 2023-06-23 15:57:11.585450 autometrics-0.6/src/autometrics/test_decorator.py
--rw-r--r--   0        0        0     3065 2023-05-11 12:02:53.378981 autometrics-0.6/src/autometrics/test_prometheus_url.py
--rw-r--r--   0        0        0       23 2023-05-05 10:51:08.826284 autometrics-0.6/src/autometrics/tracker/__init__.py
--rw-r--r--   0        0        0      680 2023-06-15 09:09:44.376855 autometrics-0.6/src/autometrics/tracker/exemplar.py
--rw-r--r--   0        0        0     5982 2023-06-23 15:57:11.585695 autometrics-0.6/src/autometrics/tracker/opentelemetry.py
--rw-r--r--   0        0        0     4347 2023-06-23 15:57:11.585945 autometrics-0.6/src/autometrics/tracker/prometheus.py
--rw-r--r--   0        0        0     2319 2023-06-23 15:57:11.586326 autometrics-0.6/src/autometrics/tracker/test_concurrency.py
--rw-r--r--   0        0        0     3027 2023-06-16 11:01:50.465190 autometrics-0.6/src/autometrics/tracker/test_tracker.py
--rw-r--r--   0        0        0     2615 2023-06-23 15:57:11.586581 autometrics-0.6/src/autometrics/tracker/tracker.py
--rw-r--r--   0        0        0     1820 2023-05-10 15:25:28.523451 autometrics-0.6/src/autometrics/utils.py
--rw-r--r--   0        0        0    10678 1970-01-01 00:00:00.000000 autometrics-0.6/PKG-INFO
+-rw-r--r--   0        0        0     1022 2023-04-12 17:23:29.278864 autometrics-0.7/LICENSE
+-rw-r--r--   0        0        0     9181 2023-07-19 14:50:31.112596 autometrics-0.7/README.md
+-rw-r--r--   0        0        0     2081 2023-07-19 15:57:15.109845 autometrics-0.7/pyproject.toml
+-rw-r--r--   0        0        0       25 2023-06-28 13:42:06.860107 autometrics-0.7/src/autometrics/__init__.py
+-rw-r--r--   0        0        0     1489 2023-06-26 13:25:13.436175 autometrics-0.7/src/autometrics/constants.py
+-rw-r--r--   0        0        0     5672 2023-07-19 14:50:31.113087 autometrics-0.7/src/autometrics/decorator.py
+-rw-r--r--   0        0        0     3050 2023-04-13 12:18:19.449416 autometrics-0.7/src/autometrics/objectives.py
+-rw-r--r--   0        0        0     2197 2023-05-11 12:02:53.378737 autometrics-0.7/src/autometrics/prometheus_url.py
+-rw-r--r--   0        0        0     1125 2023-07-19 14:50:31.113230 autometrics-0.7/src/autometrics/test_caller.py
+-rw-r--r--   0        0        0    16117 2023-07-19 14:50:31.113444 autometrics-0.7/src/autometrics/test_decorator.py
+-rw-r--r--   0        0        0     3065 2023-05-11 12:02:53.378981 autometrics-0.7/src/autometrics/test_prometheus_url.py
+-rw-r--r--   0        0        0       23 2023-05-05 10:51:08.826284 autometrics-0.7/src/autometrics/tracker/__init__.py
+-rw-r--r--   0        0        0      680 2023-06-15 09:09:44.376855 autometrics-0.7/src/autometrics/tracker/exemplar.py
+-rw-r--r--   0        0        0     6397 2023-07-19 15:54:12.041119 autometrics-0.7/src/autometrics/tracker/opentelemetry.py
+-rw-r--r--   0        0        0     4767 2023-06-28 13:42:06.860732 autometrics-0.7/src/autometrics/tracker/prometheus.py
+-rw-r--r--   0        0        0     2462 2023-07-19 14:50:31.114279 autometrics-0.7/src/autometrics/tracker/test_concurrency.py
+-rw-r--r--   0        0        0     3027 2023-06-16 11:01:50.465190 autometrics-0.7/src/autometrics/tracker/test_tracker.py
+-rw-r--r--   0        0        0     2824 2023-06-28 13:42:06.860895 autometrics-0.7/src/autometrics/tracker/tracker.py
+-rw-r--r--   0        0        0     1551 2023-07-19 14:50:31.114920 autometrics-0.7/src/autometrics/utils.py
+-rw-r--r--   0        0        0    10330 1970-01-01 00:00:00.000000 autometrics-0.7/PKG-INFO
```

### Comparing `autometrics-0.6/LICENSE` & `autometrics-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `autometrics-0.6/README.md` & `autometrics-0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ![GitHub_headerImage](https://user-images.githubusercontent.com/3262610/221191767-73b8a8d9-9f8b-440e-8ab6-75cb3c82f2bc.png)
 
+[![Tests](https://github.com/autometrics-dev/autometrics-py/actions/workflows/main.yml/badge.svg)](https://github.com/autometrics-dev/autometrics-py/actions/workflows/main.yml)
 [![Discord Shield](https://discordapp.com/api/guilds/950489382626951178/widget.png?style=shield)](https://discord.gg/kHtwcH8As9)
 
 > A Python port of the Rust
 > [autometrics-rs](https://github.com/fiberplane/autometrics-rs) library
 
 **Autometrics is a library that exports a decorator that makes it easy to understand the error rate, response time, and production usage of any function in your code.** Jump straight from your IDE to live Prometheus charts for each HTTP/RPC handler, database method, or other piece of application logic.
 
@@ -20,15 +21,15 @@
   most useful metrics
 - 💡 Writes Prometheus queries so you can understand the data generated without
   knowing PromQL
 - 🔗 Create links to live Prometheus charts directly into each function's docstring
 - [🔍 Identify commits](#identifying-commits-that-introduced-problems) that introduced errors or increased latency
 - [🚨 Define alerts](#alerts--slos) using SLO best practices directly in your source code
 - [📊 Grafana dashboards](#dashboards) work out of the box to visualize the performance of instrumented functions & SLOs
-- [⚙️ Configurable](#metrics-libraries) metric collection library (`opentelemetry`, `prometheus`, or `metrics`)
+- [⚙️ Configurable](#metrics-libraries) metric collection library (`opentelemetry` or `prometheus`)
 - [📍 Attach exemplars](#exemplars) to connect metrics with traces
 - ⚡ Minimal runtime overhead
 
 ## Using autometrics-py
 
 - Set up a [Prometheus instance](https://prometheus.io/download/)
 - Configure prometheus to scrape your application ([check our instructions if you need help](https://github.com/autometrics-dev#5-configuring-prometheus))
@@ -82,47 +83,15 @@
 )
 
 @autometrics(objective=API_SLO_HIGH_SUCCESS)
 def api_handler():
   # ...
 ```
 
-Autometrics by default will try to store information on which function calls a decorated function. As such you may want to place the autometrics in the top/first decorator, as otherwise you may get `inner` or `wrapper` as the caller function.
-
-So instead of writing:
-
-```py
-from functools import wraps
-from typing import Any, TypeVar, Callable
-
-R = TypeVar("R")
-
-def noop(func: Callable[..., R]) -> Callable[..., R]:
-    """A noop decorator that does nothing."""
-
-    @wraps(func)
-    def inner(*args: Any, **kwargs: Any) -> Any:
-        return func(*args, **kwargs)
-
-    return inner
-
-@noop
-@autometrics
-def api_handler():
-  # ...
-```
-
-You may want to switch the order of the decorator
-
-```py
-@autometrics
-@noop
-def api_handler():
-  # ...
-```
+Autometrics keeps track of instrumented functions calling each other. If you have a function that calls another function, metrics for later will include `caller` label set to the name of the autometricised function that called it.
 
 #### Metrics Libraries
 
 Configure the package that autometrics will use to produce metrics with the `AUTOMETRICS_TRACKER` environment variable.
 
 - `opentelemetry` - Enabled by default, can also be explicitly set using the env var `AUTOMETRICS_TRACKER="OPEN_TELEMETERY"`. Look in `pyproject.toml` for the versions of the OpenTelemetry packages that will be used.
 - `prometheus` - Can be set using the env var `AUTOMETRICS_TRACKER="PROMETHEUS"`. Look in `pyproject.toml` for the version of the `prometheus-client` package that will be used.
```

### Comparing `autometrics-0.6/pyproject.toml` & `autometrics-0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autometrics"
-version = "0.6"
+version = "0.7"
 description = "Easily add metrics to your system – and actually understand them using automatically customized Prometheus queries"
 authors = ["Fiberplane <info@fiberplane.com>"]
 license = "MIT OR Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/autometrics-dev/autometrics-py"
 homepage = "https://github.com/autometrics-dev/autometrics-py"
 keywords = ["metrics", "telemetry", "prometheus", "monitoring", "observability", "instrumentation"]
```

### Comparing `autometrics-0.6/src/autometrics/constants.py` & `autometrics-0.7/src/autometrics/constants.py`

 * *Files identical despite different names*

### Comparing `autometrics-0.6/src/autometrics/decorator.py` & `autometrics-0.7/src/autometrics/decorator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 """Autometrics module."""
+from contextvars import ContextVar
 import time
 import inspect
 
 from functools import wraps
 from typing import overload, TypeVar, Callable, Optional, Awaitable
 from typing_extensions import ParamSpec
+
 from .objectives import Objective
 from .tracker import get_tracker, Result
-from .admin_panel import register_function_info
-from .utils import get_module_name, get_caller_function, append_docs_to_docstring
+from .utils import (
+    get_function_name,
+    get_module_name,
+    append_docs_to_docstring,
+)
 
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
+caller_var: ContextVar[str] = ContextVar("caller", default="")
+
+
 # Bare decorator usage
 @overload
 def autometrics(func: Callable[P, T]) -> Callable[P, T]:
     ...
 
 
 @overload
@@ -38,14 +46,22 @@
     func: Optional[Callable] = None,
     *,
     objective: Optional[Objective] = None,
     track_concurrency: Optional[bool] = False,
 ):
     """Decorator for tracking function calls and duration. Supports synchronous and async functions."""
 
+    def register_function_info(
+        function: str,
+        module: str,
+    ):
+        get_tracker().initialize_counters(
+            function=function, module=module, objective=objective
+        )
+
     def track_start(function: str, module: str):
         get_tracker().start(
             function=function, module=module, track_concurrency=track_concurrency
         )
 
     def track_result_ok(start_time: float, function: str, module: str, caller: str):
         get_tracker().finish(
@@ -74,23 +90,25 @@
             result=Result.ERROR,
         )
 
     def sync_decorator(func: Callable[P, T]) -> Callable[P, T]:
         """Helper for decorating synchronous functions, to track calls and duration."""
 
         module_name = get_module_name(func)
-        func_name = func.__name__
+        func_name = get_function_name(func)
         register_function_info(func_name, module_name)
 
         @wraps(func)
         def sync_wrapper(*args: P.args, **kwds: P.kwargs) -> T:
             start_time = time.time()
-            caller = get_caller_function()
+            caller = caller_var.get()
+            context_token = None
 
             try:
+                context_token = caller_var.set(func_name)
                 if track_concurrency:
                     track_start(module=module_name, function=func_name)
                 result = func(*args, **kwds)
                 track_result_ok(
                     start_time, function=func_name, module=module_name, caller=caller
                 )
 
@@ -100,32 +118,39 @@
                     start_time,
                     function=func_name,
                     module=module_name,
                     caller=caller,
                 )
                 # Reraise exception
                 raise exception
+
+            finally:
+                if context_token is not None:
+                    caller_var.reset(context_token)
+
             return result
 
         sync_wrapper.__doc__ = append_docs_to_docstring(func, func_name, module_name)
         return sync_wrapper
 
     def async_decorator(func: Callable[P, Awaitable[T]]) -> Callable[P, Awaitable[T]]:
         """Helper for decorating async functions, to track calls and duration."""
 
         module_name = get_module_name(func)
-        func_name = func.__name__
+        func_name = get_function_name(func)
         register_function_info(func_name, module_name)
 
         @wraps(func)
         async def async_wrapper(*args: P.args, **kwds: P.kwargs) -> T:
             start_time = time.time()
-            caller = get_caller_function()
+            caller = caller_var.get()
+            context_token = None
 
             try:
+                context_token = caller_var.set(func_name)
                 if track_concurrency:
                     track_start(module=module_name, function=func_name)
                 result = await func(*args, **kwds)
                 track_result_ok(
                     start_time, function=func_name, module=module_name, caller=caller
                 )
 
@@ -135,14 +160,19 @@
                     start_time,
                     function=func_name,
                     module=module_name,
                     caller=caller,
                 )
                 # Reraise exception
                 raise exception
+
+            finally:
+                if context_token is not None:
+                    caller_var.reset(context_token)
+
             return result
 
         async_wrapper.__doc__ = append_docs_to_docstring(func, func_name, module_name)
         return async_wrapper
 
     def pick_decorator(func: Callable) -> Callable:
         """Pick the correct decorator based on the function type."""
```

### Comparing `autometrics-0.6/src/autometrics/objectives.py` & `autometrics-0.7/src/autometrics/objectives.py`

 * *Files identical despite different names*

### Comparing `autometrics-0.6/src/autometrics/prometheus_url.py` & `autometrics-0.7/src/autometrics/prometheus_url.py`

 * *Files identical despite different names*

### Comparing `autometrics-0.6/src/autometrics/test_prometheus_url.py` & `autometrics-0.7/src/autometrics/test_prometheus_url.py`

 * *Files identical despite different names*

### Comparing `autometrics-0.6/src/autometrics/tracker/exemplar.py` & `autometrics-0.7/src/autometrics/tracker/exemplar.py`

 * *Files identical despite different names*

### Comparing `autometrics-0.6/src/autometrics/tracker/opentelemetry.py` & `autometrics-0.7/src/autometrics/tracker/opentelemetry.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,23 +79,24 @@
         self,
         function: str,
         module: str,
         caller: str,
         objective: Optional[Objective],
         exemplar: Optional[dict],
         result: Result,
+        inc_by: int = 1,
     ):
         objective_name = "" if objective is None else objective.name
         percentile = (
             ""
             if objective is None or objective.success_rate is None
             else objective.success_rate.value
         )
         self.__counter_instance.add(
-            1,
+            inc_by,
             attributes={
                 "function": function,
                 "module": module,
                 "result": result.value,
                 "caller": caller,
                 OBJECTIVE_NAME: objective_name,
                 OBJECTIVE_PERCENTILE: percentile,
@@ -118,15 +119,15 @@
         threshold = ""
 
         if latency is not None:
             threshold = latency[0].value
             percentile = latency[1].value
 
         self.__histogram_instance.record(
-            duration * 1000,
+            duration,
             attributes={
                 "function": function,
                 "module": module,
                 OBJECTIVE_NAME: objective_name,
                 OBJECTIVE_PERCENTILE: percentile,
                 OBJECTIVE_LATENCY_THRESHOLD: threshold,
             },
@@ -180,7 +181,18 @@
             self.__up_down_counter_concurrency_instance.add(
                 -1.0,
                 attributes={
                     "function": function,
                     "module": module,
                 },
             )
+
+    def initialize_counters(
+        self,
+        function: str,
+        module: str,
+        objective: Optional[Objective] = None,
+    ):
+        """Initialize tracking metrics for a function call at zero."""
+        caller = ""
+        self.__count(function, module, caller, objective, None, Result.OK, 0)
+        self.__count(function, module, caller, objective, None, Result.ERROR, 0)
```

### Comparing `autometrics-0.6/src/autometrics/tracker/prometheus.py` & `autometrics-0.7/src/autometrics/tracker/prometheus.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,14 +65,15 @@
         self,
         func_name: str,
         module_name: str,
         caller: str,
         objective: Optional[Objective] = None,
         exemplar: Optional[dict] = None,
         result: Result = Result.OK,
+        inc_by: int = 1,
     ):
         """Increment the counter for the function call."""
         objective_name = "" if objective is None else objective.name
         percentile = (
             ""
             if objective is None or objective.success_rate is None
             else objective.success_rate.value
@@ -81,15 +82,15 @@
         self.prom_counter.labels(
             func_name,
             module_name,
             result.value,
             caller,
             objective_name,
             percentile,
-        ).inc(1, exemplar)
+        ).inc(inc_by, exemplar)
 
     def _histogram(
         self,
         func_name: str,
         module_name: str,
         start_time: float,
         objective: Optional[Objective] = None,
@@ -142,7 +143,18 @@
             exemplar = get_exemplar()
 
         self._count(function, module, caller, objective, exemplar, result)
         self._histogram(function, module, start_time, objective, exemplar)
 
         if track_concurrency:
             self.prom_gauge_concurrency.labels(function, module).dec()
+
+    def initialize_counters(
+        self,
+        function: str,
+        module: str,
+        objective: Optional[Objective] = None,
+    ):
+        """Initialize tracking metrics for a function call at zero."""
+        caller = ""
+        self._count(function, module, caller, objective, None, Result.OK, 0)
+        self._count(function, module, caller, objective, None, Result.ERROR, 0)
```

### Comparing `autometrics-0.6/src/autometrics/tracker/test_concurrency.py` & `autometrics-0.7/src/autometrics/tracker/test_concurrency.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,42 +2,46 @@
 import asyncio
 import pytest
 
 
 from .tracker import set_tracker, TrackerType
 
 from ..decorator import autometrics
+from ..utils import get_function_name, get_module_name
 
 
 @autometrics(track_concurrency=True)
 async def sleep(time):
     await asyncio.sleep(time)
 
 
 @pytest.mark.asyncio
 async def test_concurrency_tracking_prometheus(monkeypatch):
     # HACK - We need to set the tracker explicitly here, instead of using `init_tracker`
     #        because the library was already initialized with the OpenTelemetry tracker
     set_tracker(TrackerType.PROMETHEUS)
 
+    func_name = get_function_name(sleep)
+    module_name = get_module_name(sleep)
+
     # Create a 200ms async task
     loop = asyncio.get_event_loop()
     task = loop.create_task(sleep(0.2))
 
     # Await a separate 100ms async task.
     # This way, the 200ms task will still running once this task is done.
     # We have to do this to ensure that the 200ms task is kicked off before we call `generate_latest`
     await sleep(0.1)
     blob = generate_latest()
     await task
     assert blob is not None
     data = blob.decode("utf-8")
-    print(data)
+
     assert (
-        f"""# TYPE function_calls_concurrent gauge\nfunction_calls_concurrent{{function="sleep",module="test_concurrency"}} 1.0"""
+        f"""# TYPE function_calls_concurrent gauge\nfunction_calls_concurrent{{function="sleep",module="autometrics.tracker.test_concurrency"}} 1.0"""
         in data
     )
 
 
 # NOTE - Gauges are not supported by the OTEL collector (yet)
 #        https://github.com/open-telemetry/opentelemetry-python/pull/3306
 #
```

### Comparing `autometrics-0.6/src/autometrics/tracker/test_tracker.py` & `autometrics-0.7/src/autometrics/tracker/test_tracker.py`

 * *Files identical despite different names*

### Comparing `autometrics-0.6/src/autometrics/tracker/tracker.py` & `autometrics-0.7/src/autometrics/tracker/tracker.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,14 +32,22 @@
         caller: str,
         result: Result = Result.OK,
         objective: Optional[Objective] = None,
         track_concurrency: Optional[bool] = False,
     ):
         """Finish tracking metrics for a function call."""
 
+    def initialize_counters(
+        self,
+        function: str,
+        module: str,
+        objective: Optional[Objective] = None,
+    ):
+        """Initialize (counter) metrics for a function at zero."""
+
 
 class TrackerType(Enum):
     """Type of tracker."""
 
     OPENTELEMETRY = "opentelemetry"
     PROMETHEUS = "prometheus"
```

### Comparing `autometrics-0.6/src/autometrics/utils.py` & `autometrics-0.7/src/autometrics/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import inspect
 import os
 from collections.abc import Callable
+
 from .prometheus_url import Generator
 
 
 def get_module_name(func: Callable) -> str:
     """Get the name of the module that contains the function."""
-    func_name = func.__name__
-    fullname = func.__qualname__
-    filename = get_filename_as_module(func)
-    if fullname == func_name:
-        return filename
-
-    classname = func.__qualname__.rsplit(".", 1)[0]
-    return f"{filename}.{classname}"
+    module = inspect.getmodule(func)
+    if module is None:
+        return get_filename_as_module(func)
+    return module.__name__
 
 
 def get_filename_as_module(func: Callable) -> str:
     """Get the filename of the module that contains the function."""
     fullpath = inspect.getsourcefile(func)
     if fullpath is None:
         return ""
 
     filename = os.path.basename(fullpath)
     module_part = os.path.splitext(filename)[0]
     return module_part
 
 
+def get_function_name(func: Callable) -> str:
+    """Get the name of the function."""
+    return func.__qualname__ or func.__name__
+
+
 def write_docs(func_name: str, module_name: str):
     """Write the prometheus query urls to the function docstring."""
     generator = Generator(func_name, module_name)
     docs = f"Prometheus Query URLs for Function - {func_name} and Module - {module_name}: \n\n"
 
     urls = generator.create_urls()
     for key, value in urls.items():
@@ -42,14 +44,7 @@
 
 def append_docs_to_docstring(func, func_name, module_name):
     """Helper for appending docs to a function's docstring."""
     if func.__doc__ is None:
         return write_docs(func_name, module_name)
     else:
         return f"{func.__doc__}\n{write_docs(func_name, module_name)}"
-
-
-def get_caller_function(depth: int = 2):
-    """Get the name of the function. Default depth is 2 to get the caller of the caller of the function being decorated."""
-    caller_frame = inspect.stack()[depth]
-    caller_function_name = caller_frame[3]
-    return caller_function_name
```

### Comparing `autometrics-0.6/PKG-INFO` & `autometrics-0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autometrics
-Version: 0.6
+Version: 0.7
 Summary: Easily add metrics to your system – and actually understand them using automatically customized Prometheus queries
 Home-page: https://github.com/autometrics-dev/autometrics-py
 License: MIT OR Apache-2.0
 Keywords: metrics,telemetry,prometheus,monitoring,observability,instrumentation
 Author: Fiberplane
 Author-email: info@fiberplane.com
 Requires-Python: >=3.8,<4.0
@@ -21,14 +21,15 @@
 Requires-Dist: python-dotenv (==1.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Project-URL: Repository, https://github.com/autometrics-dev/autometrics-py
 Description-Content-Type: text/markdown
 
 ![GitHub_headerImage](https://user-images.githubusercontent.com/3262610/221191767-73b8a8d9-9f8b-440e-8ab6-75cb3c82f2bc.png)
 
+[![Tests](https://github.com/autometrics-dev/autometrics-py/actions/workflows/main.yml/badge.svg)](https://github.com/autometrics-dev/autometrics-py/actions/workflows/main.yml)
 [![Discord Shield](https://discordapp.com/api/guilds/950489382626951178/widget.png?style=shield)](https://discord.gg/kHtwcH8As9)
 
 > A Python port of the Rust
 > [autometrics-rs](https://github.com/fiberplane/autometrics-rs) library
 
 **Autometrics is a library that exports a decorator that makes it easy to understand the error rate, response time, and production usage of any function in your code.** Jump straight from your IDE to live Prometheus charts for each HTTP/RPC handler, database method, or other piece of application logic.
 
@@ -45,15 +46,15 @@
   most useful metrics
 - 💡 Writes Prometheus queries so you can understand the data generated without
   knowing PromQL
 - 🔗 Create links to live Prometheus charts directly into each function's docstring
 - [🔍 Identify commits](#identifying-commits-that-introduced-problems) that introduced errors or increased latency
 - [🚨 Define alerts](#alerts--slos) using SLO best practices directly in your source code
 - [📊 Grafana dashboards](#dashboards) work out of the box to visualize the performance of instrumented functions & SLOs
-- [⚙️ Configurable](#metrics-libraries) metric collection library (`opentelemetry`, `prometheus`, or `metrics`)
+- [⚙️ Configurable](#metrics-libraries) metric collection library (`opentelemetry` or `prometheus`)
 - [📍 Attach exemplars](#exemplars) to connect metrics with traces
 - ⚡ Minimal runtime overhead
 
 ## Using autometrics-py
 
 - Set up a [Prometheus instance](https://prometheus.io/download/)
 - Configure prometheus to scrape your application ([check our instructions if you need help](https://github.com/autometrics-dev#5-configuring-prometheus))
@@ -107,47 +108,15 @@
 )
 
 @autometrics(objective=API_SLO_HIGH_SUCCESS)
 def api_handler():
   # ...
 ```
 
-Autometrics by default will try to store information on which function calls a decorated function. As such you may want to place the autometrics in the top/first decorator, as otherwise you may get `inner` or `wrapper` as the caller function.
-
-So instead of writing:
-
-```py
-from functools import wraps
-from typing import Any, TypeVar, Callable
-
-R = TypeVar("R")
-
-def noop(func: Callable[..., R]) -> Callable[..., R]:
-    """A noop decorator that does nothing."""
-
-    @wraps(func)
-    def inner(*args: Any, **kwargs: Any) -> Any:
-        return func(*args, **kwargs)
-
-    return inner
-
-@noop
-@autometrics
-def api_handler():
-  # ...
-```
-
-You may want to switch the order of the decorator
-
-```py
-@autometrics
-@noop
-def api_handler():
-  # ...
-```
+Autometrics keeps track of instrumented functions calling each other. If you have a function that calls another function, metrics for later will include `caller` label set to the name of the autometricised function that called it.
 
 #### Metrics Libraries
 
 Configure the package that autometrics will use to produce metrics with the `AUTOMETRICS_TRACKER` environment variable.
 
 - `opentelemetry` - Enabled by default, can also be explicitly set using the env var `AUTOMETRICS_TRACKER="OPEN_TELEMETERY"`. Look in `pyproject.toml` for the versions of the OpenTelemetry packages that will be used.
 - `prometheus` - Can be set using the env var `AUTOMETRICS_TRACKER="PROMETHEUS"`. Look in `pyproject.toml` for the version of the `prometheus-client` package that will be used.
```

