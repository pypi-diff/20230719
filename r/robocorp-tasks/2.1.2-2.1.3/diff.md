# Comparing `tmp/robocorp_tasks-2.1.2.tar.gz` & `tmp/robocorp_tasks-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_tasks-2.1.2.tar", max compression
+gzip compressed data, was "robocorp_tasks-2.1.3.tar", max compression
```

## Comparing `robocorp_tasks-2.1.2.tar` & `robocorp_tasks-2.1.3.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0     5432 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/README.md
--rw-r--r--   0        0        0     1240 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     3502 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/__init__.py
--rw-r--r--   0        0        0       79 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/__main__.py
--rw-r--r--   0        0        0     4495 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_argdispatch.py
--rw-r--r--   0        0        0     1467 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_callback.py
--rw-r--r--   0        0        0     5121 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_collect_tasks.py
--rw-r--r--   0        0        0    10273 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_commands.py
--rw-r--r--   0        0        0     2245 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_config.py
--rw-r--r--   0        0        0      182 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_exceptions.py
--rw-r--r--   0        0        0     1122 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_hooks.py
--rw-r--r--   0        0        0     1367 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_lifecycle.py
--rw-r--r--   0        0        0     5084 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_log_auto_setup.py
--rw-r--r--   0        0        0     2160 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_log_output_setup.py
--rw-r--r--   0        0        0     4201 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_protocols.py
--rw-r--r--   0        0        0     5489 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_task.py
--rw-r--r--   0        0        0     2436 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_toml_settings.py
--rw-r--r--   0        0        0      869 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/cli.py
--rw-r--r--   0        0        0        0 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/py.typed
--rw-r--r--   0        0        0     6211 1970-01-01 00:00:00.000000 robocorp_tasks-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     5721 2023-07-19 12:49:50.239060 robocorp_tasks-2.1.3/README.md
+-rw-r--r--   0        0        0     1240 2023-07-19 12:49:50.239060 robocorp_tasks-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3502 2023-07-19 12:49:50.239060 robocorp_tasks-2.1.3/src/robocorp/tasks/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-19 12:49:50.239060 robocorp_tasks-2.1.3/src/robocorp/tasks/__main__.py
+-rw-r--r--   0        0        0     4495 2023-07-19 12:49:50.239060 robocorp_tasks-2.1.3/src/robocorp/tasks/_argdispatch.py
+-rw-r--r--   0        0        0     1467 2023-07-19 12:49:50.239060 robocorp_tasks-2.1.3/src/robocorp/tasks/_callback.py
+-rw-r--r--   0        0        0     5121 2023-07-19 12:49:50.239060 robocorp_tasks-2.1.3/src/robocorp/tasks/_collect_tasks.py
+-rw-r--r--   0        0        0    10475 2023-07-19 12:49:50.239060 robocorp_tasks-2.1.3/src/robocorp/tasks/_commands.py
+-rw-r--r--   0        0        0     2245 2023-07-19 12:49:50.239060 robocorp_tasks-2.1.3/src/robocorp/tasks/_config.py
+-rw-r--r--   0        0        0      182 2023-07-19 12:49:50.239060 robocorp_tasks-2.1.3/src/robocorp/tasks/_exceptions.py
+-rw-r--r--   0        0        0     1122 2023-07-19 12:49:50.239060 robocorp_tasks-2.1.3/src/robocorp/tasks/_hooks.py
+-rw-r--r--   0        0        0     1367 2023-07-19 12:49:50.239060 robocorp_tasks-2.1.3/src/robocorp/tasks/_lifecycle.py
+-rw-r--r--   0        0        0     1022 2023-07-19 12:49:50.239060 robocorp_tasks-2.1.3/src/robocorp/tasks/_log_auto_setup.py
+-rw-r--r--   0        0        0     2160 2023-07-19 12:49:50.239060 robocorp_tasks-2.1.3/src/robocorp/tasks/_log_output_setup.py
+-rw-r--r--   0        0        0     4089 2023-07-19 12:49:50.239060 robocorp_tasks-2.1.3/src/robocorp/tasks/_protocols.py
+-rw-r--r--   0        0        0     5489 2023-07-19 12:49:50.239060 robocorp_tasks-2.1.3/src/robocorp/tasks/_task.py
+-rw-r--r--   0        0        0      869 2023-07-19 12:49:50.239060 robocorp_tasks-2.1.3/src/robocorp/tasks/cli.py
+-rw-r--r--   0        0        0        0 2023-07-19 12:49:50.239060 robocorp_tasks-2.1.3/src/robocorp/tasks/py.typed
+-rw-r--r--   0        0        0     6500 1970-01-01 00:00:00.000000 robocorp_tasks-2.1.3/PKG-INFO
```

### Comparing `robocorp_tasks-2.1.2/README.md` & `robocorp_tasks-2.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -60,36 +60,45 @@
 3. View the log results in `output/log.html`.
 
 
 ## Auto logging customization
 
 
 Following the initial steps outlined above should be sufficient to get comprehensive 
-logging for all user code executed. However, note that it won't log calls from 
-libraries by default, as it may be difficult to separate the libraries that are 
-important for a project from those that are just noise.
+logging for all user code executed and calls into libraries in site-packges and python libs (which by default are
+configured to show just when called from user code and will not show internal calls
+inside the library itself).
 
-To add custom logging for libraries like `rpaframework`, `Selenium` and others, create a 
-`pyproject.toml` file and place it in the root of your project. 
-Then, customize the `[tool.robocorp.log]` section to add `log_filter_rules`.
+It's possible to change how libraries or user code is logged by customizing `log_filter_rules`
+by creating a `[tool.robocorp.log]` in `pyproject.toml`.
 
 
-`log_filter_rules` is a list of dictionaries where entries may be added to specify
-how to handle logging for a particular module.
+There are three different logging configurations that may be applied for each module:
 
-There are three different logging configurations that may be applied:
-
-- `exclude`: skips logging a module.
+- `exclude`: excludes a module from logging.
 - `full_log` (default for user code): logs a module with full information, such as method calls, arguments, yields, local assigns, and more.
-- `log_on_project_call` (default for library code -- since 2.0): logs only method calls, arguments, return values and exceptions, but only when a library method is called from user code. This configuration is meant to be used for library logging.
+- `log_on_project_call` (default for library code -- since 2.0): logs only method calls, arguments, return values and exceptions, but only when a library method is called from user code. This configuration is meant to be used for libraries (modules in site-packages or python lib) logging.
+
+
+Example showing how to exclude from logging any user module which ends with `producer`:
+
+
+```
+[tool.robocorp.log]
+
+log_filter_rules = [
+    {name = "*producer", kind = "exclude"},
+]
+```
 
-Note that the default for the library code may be configured through `default_library_filter_kind`.
+By default libraries in site-packages and python lib will be configured as `log_on_project_call`, but
+it's possible to change its default through `default_library_filter_kind`.
 
 Example of `pyproject.toml` where the `rpaframework` and `selenium` 
-libraries are configured to be logged and all other libraries are
+libraries are configured to be logged and all other libraries in site-packages/python lib are
 excluded by default:
 
 
 ```
 [tool.robocorp.log]
 
 log_filter_rules = [
@@ -104,15 +113,16 @@
 Note that when specifying a module name to match in `log_filter_rules`, 
 the name may either match exactly or the module name must start with the 
 name followed by a dot.
 
 This means that, for example, `RPA` would match `RPA.Browser`,
 but not `RPAmodule` nor `another.RPA`.
 
-Also, as of `robocorp-tasks 2.0`, it's also possible to use `fnmatch` style names.
+As of `robocorp-tasks 2.0`, it's also possible to use `fnmatch` style names
+(where `*` matches anything and `?` matches any single char -- see: https://docs.python.org/3/library/fnmatch.html for more information).
 
 i.e.:
 
 ```
 [tool.robocorp.log]
 
 log_filter_rules = [
```

### Comparing `robocorp_tasks-2.1.2/pyproject.toml` & `robocorp_tasks-2.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-tasks"
-version = "2.1.2"
+version = "2.1.3"
 description = "The automation framework for Python"
 authors = [
 	"Fabio Zadrozny <fabio@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robo/"
 license = "Apache-2.0"
@@ -15,15 +15,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-robocorp-log = ">=2.2,<3"
+robocorp-log = ">=2.4,<3"
 
 [tool.poetry.group.dev.dependencies]
 robocorp-devutils = {path = "../devutils/", develop = true}
 
 [tool.mypy]
 mypy_path = "src:tests"
```

### Comparing `robocorp_tasks-2.1.2/src/robocorp/tasks/__init__.py` & `robocorp_tasks-2.1.3/src/robocorp/tasks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 automatically logged is not imported prior the the `cli.main` call.
 """
 from pathlib import Path
 from typing import Optional
 
 from ._protocols import ITask
 
-__version__ = "2.1.2"
+__version__ = "2.1.3"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 def task(func):
     """
     Decorator for tasks (entry points) which can be executed by `robocorp.tasks`.
```

### Comparing `robocorp_tasks-2.1.2/src/robocorp/tasks/_argdispatch.py` & `robocorp_tasks-2.1.3/src/robocorp/tasks/_argdispatch.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.2/src/robocorp/tasks/_callback.py` & `robocorp_tasks-2.1.3/src/robocorp/tasks/_callback.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.2/src/robocorp/tasks/_collect_tasks.py` & `robocorp_tasks-2.1.3/src/robocorp/tasks/_collect_tasks.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.2/src/robocorp/tasks/_commands.py` & `robocorp_tasks-2.1.3/src/robocorp/tasks/_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import os
 import sys
+import threading
 import traceback
 from pathlib import Path
 from typing import List, Sequence, Union
 
 from ._argdispatch import arg_dispatch as _arg_dispatch
-import threading
 
 
 # Note: the args must match the 'dest' on the configured argparser.
 @_arg_dispatch.register(name="list")
 def list_tasks(
     path: str,
 ) -> int:
@@ -97,43 +97,49 @@
 
     Returns:
         0 if everything went well.
         1 if there was some error running the task.
     """
     from robocorp.log import console, redirect
 
-    from robocorp.tasks._toml_settings import read_pyproject_toml
-
     from ._collect_tasks import collect_tasks
     from ._config import RunConfig, set_config
     from ._exceptions import RobocorpTasksCollectError
     from ._hooks import (
         after_all_tasks_run,
         after_task_run,
         before_all_tasks_run,
         before_task_run,
     )
-    from ._log_auto_setup import read_robocorp_log_config, setup_cli_auto_logging
+    from ._log_auto_setup import setup_cli_auto_logging
     from ._log_output_setup import setup_log_output, setup_log_output_to_port
     from ._protocols import ITask, Status
     from ._task import Context, set_current_task
+    from robocorp.log.pyproject_config import read_pyproject_toml
+    from robocorp.log.pyproject_config import read_robocorp_auto_log_config
 
     console.set_mode(console_colors)
 
     # Don't show internal machinery on tracebacks:
     # setting __tracebackhide__ will make it so that robocorp-log
     # won't show this frame onwards in the logging.
     __tracebackhide__ = 1
 
     p = Path(path).absolute()
     context = Context()
     if not p.exists():
         context.show_error(f"Path: {path} does not exist")
         return 1
 
+    # Enable faulthandler (writing to sys.stderr) early on in the
+    # task execution process.
+    import faulthandler
+
+    faulthandler.enable()
+
     from robocorp import log
 
     task_names: Sequence[str]
     if not task_name:
         task_names = []
         task_or_tasks = "tasks"
     elif isinstance(task_name, str):
@@ -147,15 +153,15 @@
     config: log.AutoLogConfigBase
     pyproject_path_and_contents = read_pyproject_toml(p)
     pyproject_toml_contents: dict
     if pyproject_path_and_contents is None:
         config = log.DefaultAutoLogConfig()
         pyproject_toml_contents = {}
     else:
-        config = read_robocorp_log_config(context, pyproject_path_and_contents)
+        config = read_robocorp_auto_log_config(context, pyproject_path_and_contents)
         pyproject_toml_contents = pyproject_path_and_contents.toml_contents
 
     run_config = RunConfig(
         Path(output_dir),
         p,
         task_names,
         max_log_files,
```

### Comparing `robocorp_tasks-2.1.2/src/robocorp/tasks/_config.py` & `robocorp_tasks-2.1.3/src/robocorp/tasks/_config.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.2/src/robocorp/tasks/_hooks.py` & `robocorp_tasks-2.1.3/src/robocorp/tasks/_hooks.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.2/src/robocorp/tasks/_lifecycle.py` & `robocorp_tasks-2.1.3/src/robocorp/tasks/_lifecycle.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.2/src/robocorp/tasks/_log_output_setup.py` & `robocorp_tasks-2.1.3/src/robocorp/tasks/_log_output_setup.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.2/src/robocorp/tasks/_protocols.py` & `robocorp_tasks-2.1.3/src/robocorp/tasks/_protocols.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import typing
-from dataclasses import dataclass
 from pathlib import Path
 from types import TracebackType
 from typing import Any, Callable, Optional, Sequence, Set, TypeVar, Union
 
 ExcInfo = tuple[type[BaseException], BaseException, TracebackType]
 OptExcInfo = Union[ExcInfo, tuple[None, None, None]]
 
@@ -38,20 +37,14 @@
 
     ERROR = "ERROR"  # log.critical
     INFO = "INFO"  # log.info
     WARN = "WARN"  # log.warn
     DEBUG = "DEBUG"  # log.debug
 
 
-@dataclass
-class PyProjectInfo:
-    pyproject: Path
-    toml_contents: dict
-
-
 class ITask(typing.Protocol):
     module_name: str
     filename: str
     method: typing.Callable
 
     status: str
     message: str
```

### Comparing `robocorp_tasks-2.1.2/src/robocorp/tasks/_task.py` & `robocorp_tasks-2.1.3/src/robocorp/tasks/_task.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.2/src/robocorp/tasks/cli.py` & `robocorp_tasks-2.1.3/src/robocorp/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.2/PKG-INFO` & `robocorp_tasks-2.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: robocorp-tasks
-Version: 2.1.2
+Version: 2.1.3
 Summary: The automation framework for Python
 Home-page: https://github.com/robocorp/robo/
 License: Apache-2.0
 Author: Fabio Zadrozny
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Dist: robocorp-log (>=2.2,<3)
+Requires-Dist: robocorp-log (>=2.4,<3)
 Project-URL: Repository, https://github.com/robocorp/robo/
 Description-Content-Type: text/markdown
 
 # robocorp-tasks
 
 `robocorp-tasks` is a Python framework designed to simplify the development 
 of Python automations.
@@ -80,36 +80,45 @@
 3. View the log results in `output/log.html`.
 
 
 ## Auto logging customization
 
 
 Following the initial steps outlined above should be sufficient to get comprehensive 
-logging for all user code executed. However, note that it won't log calls from 
-libraries by default, as it may be difficult to separate the libraries that are 
-important for a project from those that are just noise.
+logging for all user code executed and calls into libraries in site-packges and python libs (which by default are
+configured to show just when called from user code and will not show internal calls
+inside the library itself).
 
-To add custom logging for libraries like `rpaframework`, `Selenium` and others, create a 
-`pyproject.toml` file and place it in the root of your project. 
-Then, customize the `[tool.robocorp.log]` section to add `log_filter_rules`.
+It's possible to change how libraries or user code is logged by customizing `log_filter_rules`
+by creating a `[tool.robocorp.log]` in `pyproject.toml`.
 
 
-`log_filter_rules` is a list of dictionaries where entries may be added to specify
-how to handle logging for a particular module.
+There are three different logging configurations that may be applied for each module:
 
-There are three different logging configurations that may be applied:
-
-- `exclude`: skips logging a module.
+- `exclude`: excludes a module from logging.
 - `full_log` (default for user code): logs a module with full information, such as method calls, arguments, yields, local assigns, and more.
-- `log_on_project_call` (default for library code -- since 2.0): logs only method calls, arguments, return values and exceptions, but only when a library method is called from user code. This configuration is meant to be used for library logging.
+- `log_on_project_call` (default for library code -- since 2.0): logs only method calls, arguments, return values and exceptions, but only when a library method is called from user code. This configuration is meant to be used for libraries (modules in site-packages or python lib) logging.
+
+
+Example showing how to exclude from logging any user module which ends with `producer`:
+
+
+```
+[tool.robocorp.log]
+
+log_filter_rules = [
+    {name = "*producer", kind = "exclude"},
+]
+```
 
-Note that the default for the library code may be configured through `default_library_filter_kind`.
+By default libraries in site-packages and python lib will be configured as `log_on_project_call`, but
+it's possible to change its default through `default_library_filter_kind`.
 
 Example of `pyproject.toml` where the `rpaframework` and `selenium` 
-libraries are configured to be logged and all other libraries are
+libraries are configured to be logged and all other libraries in site-packages/python lib are
 excluded by default:
 
 
 ```
 [tool.robocorp.log]
 
 log_filter_rules = [
@@ -124,15 +133,16 @@
 Note that when specifying a module name to match in `log_filter_rules`, 
 the name may either match exactly or the module name must start with the 
 name followed by a dot.
 
 This means that, for example, `RPA` would match `RPA.Browser`,
 but not `RPAmodule` nor `another.RPA`.
 
-Also, as of `robocorp-tasks 2.0`, it's also possible to use `fnmatch` style names.
+As of `robocorp-tasks 2.0`, it's also possible to use `fnmatch` style names
+(where `*` matches anything and `?` matches any single char -- see: https://docs.python.org/3/library/fnmatch.html for more information).
 
 i.e.:
 
 ```
 [tool.robocorp.log]
 
 log_filter_rules = [
```

