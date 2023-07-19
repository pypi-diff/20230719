# Comparing `tmp/pynisher-1.0.6.tar.gz` & `tmp/pynisher-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynisher-1.0.6.tar", last modified: Mon Jul 17 09:42:30 2023, max compression
+gzip compressed data, was "pynisher-1.0.7.tar", last modified: Wed Jul 19 09:30:54 2023, max compression
```

## Comparing `pynisher-1.0.6.tar` & `pynisher-1.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-07-17 09:42:29.996314 pynisher-1.0.6/
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1076 2023-03-13 20:53:22.000000 pynisher-1.0.6/LICENSE
--rw-r--r--   0 skantify  (1000) skantify  (1000)       37 2023-03-13 20:53:22.000000 pynisher-1.0.6/MANIFEST.in
--rw-r--r--   0 skantify  (1000) skantify  (1000)    14596 2023-07-17 09:42:29.996314 pynisher-1.0.6/PKG-INFO
--rw-r--r--   0 skantify  (1000) skantify  (1000)    13803 2023-03-13 20:53:22.000000 pynisher-1.0.6/README.md
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-07-17 09:42:29.996314 pynisher-1.0.6/pynisher/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      723 2023-03-13 20:53:22.000000 pynisher-1.0.6/pynisher/__init__.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)      545 2023-03-13 20:53:22.000000 pynisher-1.0.6/pynisher/exceptions.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-07-17 09:42:29.996314 pynisher-1.0.6/pynisher/limiters/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      213 2023-03-13 20:53:22.000000 pynisher-1.0.6/pynisher/limiters/__init__.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)    11791 2023-07-17 09:27:44.000000 pynisher-1.0.6/pynisher/limiters/limiter.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2625 2023-07-17 09:31:11.000000 pynisher-1.0.6/pynisher/limiters/linux.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     3214 2023-03-13 20:53:22.000000 pynisher-1.0.6/pynisher/limiters/mac.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     4995 2023-07-17 09:27:44.000000 pynisher-1.0.6/pynisher/limiters/windows.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)        0 2023-03-13 20:53:22.000000 pynisher-1.0.6/pynisher/py.typed
--rw-r--r--   0 skantify  (1000) skantify  (1000)    26577 2023-07-17 09:14:39.000000 pynisher-1.0.6/pynisher/pynisher.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     3181 2023-03-13 20:53:22.000000 pynisher-1.0.6/pynisher/support.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     6757 2023-03-14 15:30:00.000000 pynisher-1.0.6/pynisher/util.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)      924 2023-03-13 20:53:22.000000 pynisher-1.0.6/pynisher/win_errcodes.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-07-17 09:42:29.996314 pynisher-1.0.6/pynisher.egg-info/
--rw-r--r--   0 skantify  (1000) skantify  (1000)    14596 2023-07-17 09:42:29.000000 pynisher-1.0.6/pynisher.egg-info/PKG-INFO
--rw-r--r--   0 skantify  (1000) skantify  (1000)      497 2023-07-17 09:42:29.000000 pynisher-1.0.6/pynisher.egg-info/SOURCES.txt
--rw-r--r--   0 skantify  (1000) skantify  (1000)        1 2023-07-17 09:42:29.000000 pynisher-1.0.6/pynisher.egg-info/dependency_links.txt
--rw-r--r--   0 skantify  (1000) skantify  (1000)      171 2023-07-17 09:42:29.000000 pynisher-1.0.6/pynisher.egg-info/requires.txt
--rw-r--r--   0 skantify  (1000) skantify  (1000)        9 2023-07-17 09:42:29.000000 pynisher-1.0.6/pynisher.egg-info/top_level.txt
--rw-r--r--   0 skantify  (1000) skantify  (1000)     3029 2023-07-17 09:28:49.000000 pynisher-1.0.6/pyproject.toml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       38 2023-07-17 09:42:29.996314 pynisher-1.0.6/setup.cfg
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1600 2023-07-17 09:14:50.000000 pynisher-1.0.6/setup.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-07-19 09:30:54.340418 pynisher-1.0.7/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1076 2023-03-13 20:53:22.000000 pynisher-1.0.7/LICENSE
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       37 2023-03-13 20:53:22.000000 pynisher-1.0.7/MANIFEST.in
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    14610 2023-07-19 09:30:54.340418 pynisher-1.0.7/PKG-INFO
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    13817 2023-07-19 09:28:17.000000 pynisher-1.0.7/README.md
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-07-19 09:30:54.340418 pynisher-1.0.7/pynisher/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      723 2023-03-13 20:53:22.000000 pynisher-1.0.7/pynisher/__init__.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      545 2023-03-13 20:53:22.000000 pynisher-1.0.7/pynisher/exceptions.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-07-19 09:30:54.340418 pynisher-1.0.7/pynisher/limiters/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      213 2023-03-13 20:53:22.000000 pynisher-1.0.7/pynisher/limiters/__init__.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    11791 2023-07-17 09:27:44.000000 pynisher-1.0.7/pynisher/limiters/limiter.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2625 2023-07-17 09:31:11.000000 pynisher-1.0.7/pynisher/limiters/linux.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     3214 2023-03-13 20:53:22.000000 pynisher-1.0.7/pynisher/limiters/mac.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     4995 2023-07-17 09:27:44.000000 pynisher-1.0.7/pynisher/limiters/windows.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)        0 2023-03-13 20:53:22.000000 pynisher-1.0.7/pynisher/py.typed
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    26738 2023-07-19 09:29:55.000000 pynisher-1.0.7/pynisher/pynisher.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     3181 2023-03-13 20:53:22.000000 pynisher-1.0.7/pynisher/support.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     6757 2023-03-14 15:30:00.000000 pynisher-1.0.7/pynisher/util.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      924 2023-03-13 20:53:22.000000 pynisher-1.0.7/pynisher/win_errcodes.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-07-19 09:30:54.340418 pynisher-1.0.7/pynisher.egg-info/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    14610 2023-07-19 09:30:54.000000 pynisher-1.0.7/pynisher.egg-info/PKG-INFO
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      497 2023-07-19 09:30:54.000000 pynisher-1.0.7/pynisher.egg-info/SOURCES.txt
+-rw-r--r--   0 skantify  (1000) skantify  (1000)        1 2023-07-19 09:30:54.000000 pynisher-1.0.7/pynisher.egg-info/dependency_links.txt
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      171 2023-07-19 09:30:54.000000 pynisher-1.0.7/pynisher.egg-info/requires.txt
+-rw-r--r--   0 skantify  (1000) skantify  (1000)        9 2023-07-19 09:30:54.000000 pynisher-1.0.7/pynisher.egg-info/top_level.txt
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     3029 2023-07-17 09:28:49.000000 pynisher-1.0.7/pyproject.toml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       38 2023-07-19 09:30:54.340418 pynisher-1.0.7/setup.cfg
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1600 2023-07-19 09:28:03.000000 pynisher-1.0.7/setup.py
```

### Comparing `pynisher-1.0.6/LICENSE` & `pynisher-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.6/PKG-INFO` & `pynisher-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynisher
-Version: 1.0.6
+Version: 1.0.7
 Summary: A library to limit the resources used by functions using subprocesses
 Home-page: https://github.com/automl/pynisher
 Author: ('Stefan Falkner, Christina Hernandez-Wunsch, Samuel Mueller,Matthias Feurer, Francisco Rivera, Eddie Bergman and Rene Sass',)
 Author-email: feurerm@informatik.uni-freiburg.de
 License: MIT
 Keywords: resources
 Classifier: License :: OSI Approved :: BSD License
@@ -226,15 +226,15 @@
 # the controlling process. The exception to this are MemoryErrors which occur
 # in the subprocess, we convert these to MemoryLimitException.
 raises: bool = True
 
 
 # This is the multiprocess context used, please refer to their documentation
 # https://docs.python.org/3/library/multiprocessing.html#contexts-and-start-methods
-context: "fork" | "spawn" | "forkserver" | None = None
+context: "fork" | "spawn" | "forkserver" | BaseContext | None = None
 
 
 # Whether to emit warnings from  limit or not. The current warnings:
 # * When the memory limit is lower than the starting memory of a process
 # * When trying to remove the memory limit for sending back information
 #   from the subprocess to the main process
 warnings: bool = True
```

### Comparing `pynisher-1.0.6/README.md` & `pynisher-1.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
 # the controlling process. The exception to this are MemoryErrors which occur
 # in the subprocess, we convert these to MemoryLimitException.
 raises: bool = True
 
 
 # This is the multiprocess context used, please refer to their documentation
 # https://docs.python.org/3/library/multiprocessing.html#contexts-and-start-methods
-context: "fork" | "spawn" | "forkserver" | None = None
+context: "fork" | "spawn" | "forkserver" | BaseContext | None = None
 
 
 # Whether to emit warnings from  limit or not. The current warnings:
 # * When the memory limit is lower than the starting memory of a process
 # * When trying to remove the memory limit for sending back information
 #   from the subprocess to the main process
 warnings: bool = True
```

### Comparing `pynisher-1.0.6/pynisher/__init__.py` & `pynisher-1.0.7/pynisher/__init__.py`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.6/pynisher/exceptions.py` & `pynisher-1.0.7/pynisher/exceptions.py`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.6/pynisher/limiters/limiter.py` & `pynisher-1.0.7/pynisher/limiters/limiter.py`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.6/pynisher/limiters/linux.py` & `pynisher-1.0.7/pynisher/limiters/linux.py`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.6/pynisher/limiters/mac.py` & `pynisher-1.0.7/pynisher/limiters/mac.py`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.6/pynisher/limiters/windows.py` & `pynisher-1.0.7/pynisher/limiters/windows.py`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.6/pynisher/pynisher.py` & `pynisher-1.0.7/pynisher/pynisher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+from multiprocessing.context import BaseContext
 
 from typing import Any, Callable, Generic, Type, TypeVar, overload
 
 import multiprocessing
 import signal
 import sys
 from functools import wraps
@@ -54,15 +55,15 @@
         func: Callable[P, T],
         *,
         raises: Literal[True] = ...,
         name: str | None = ...,
         memory: int | tuple[int, str] | None = ...,
         cpu_time: int | tuple[float, str] | None = ...,
         wall_time: int | tuple[float, str] | None = ...,
-        context: str | None = ...,
+        context: str | BaseContext | None = ...,
         warnings: bool = ...,
         wrap_errors: bool | list[str | Type[Exception]] | dict[str, Any] = ...,
         terminate_child_processes: bool = ...,
         forceful_keyboard_interrupt: bool = ...,
     ) -> None:
         ...
 
@@ -74,15 +75,15 @@
         func: Callable[P, T],
         *,
         raises: bool,
         name: str | None = ...,
         memory: int | tuple[int, str] | None = ...,
         cpu_time: int | tuple[float, str] | None = ...,
         wall_time: int | tuple[float, str] | None = ...,
-        context: str | None = ...,
+        context: str | BaseContext | None = ...,
         warnings: bool = ...,
         wrap_errors: bool | list[str | Type[Exception]] | dict[str, Any] = ...,
         terminate_child_processes: bool = ...,
         forceful_keyboard_interrupt: bool = ...,
     ) -> None:
         ...
 
@@ -90,15 +91,15 @@
         self,
         func: Callable[P, T],
         *,
         name: str | None = None,
         memory: int | tuple[int, str] | None = None,
         cpu_time: int | tuple[float, str] | None = None,
         wall_time: int | tuple[float, str] | None = None,
-        context: str | None = None,
+        context: str | BaseContext | None = None,
         raises: bool = True,
         warnings: bool = True,
         wrap_errors: bool | list[str | Type[Exception]] | dict[str, Any] = False,
         terminate_child_processes: bool = True,
         forceful_keyboard_interrupt: bool = True,
     ) -> None:
         """
@@ -127,15 +128,15 @@
             Units available are "s", "m", "h".
 
         wall_time : int | tuple[float, str] | None = None
             The amount of total wall time in seconds to limit to
             Can provide in (time, units) such as (1.5, "h") to indicate one and a half hours.
             Units available are "s", "m", "h"
 
-        context : "fork" | "forkserver" | "spawn" | None = None
+        context : "fork" | "forkserver" | "spawn"  | BaseContext | None = None
             The context to use with multiprocessing.get_context()
             * https://docs.python.org/3/library/multiprocessing.html#multiprocessing.get_context
 
         raises : bool = True
             Whether any error from the subprocess should filter up and be raised.
 
         warnings : bool = True
@@ -570,15 +571,15 @@
 def restricted(
     name: str | None = ...,
     *,
     raises: Literal[True] = ...,
     memory: int | tuple[int, str] | None = ...,
     cpu_time: int | None = ...,
     wall_time: int | None = ...,
-    context: str | None = ...,
+    context: str | BaseContext | None = ...,
     warnings: bool = ...,
     wrap_errors: bool | list[str | Type[Exception]] | dict[str, Any] = ...,
     terminate_child_processes: bool = ...,
     forceful_keyboard_interrupt: bool = True,
 ) -> Callable[[Callable[P, T]], Callable[P, T]]:
     ...
 
@@ -587,15 +588,15 @@
 def restricted(
     name: str | None = ...,
     *,
     raises: bool,
     memory: int | tuple[int, str] | None = ...,
     cpu_time: int | None = ...,
     wall_time: int | None = ...,
-    context: str | None = ...,
+    context: str | BaseContext | None = ...,
     warnings: bool = ...,
     wrap_errors: bool | list[str | Type[Exception]] | dict[str, Any] = ...,
     terminate_child_processes: bool = ...,
     forceful_keyboard_interrupt: bool = True,
 ) -> Callable[[Callable[P, T]], Callable[P, T | _EMPTY]]:
     ...
 
@@ -619,15 +620,15 @@
 #
 def restricted(
     name: str | None = None,
     *,
     memory: int | tuple[int, str] | None = None,
     cpu_time: int | None = None,
     wall_time: int | None = None,
-    context: str | None = None,
+    context: str | BaseContext | None = None,
     raises: bool = True,
     warnings: bool = True,
     wrap_errors: bool | list[str | Type[Exception]] | dict[str, Any] = False,
     terminate_child_processes: bool = True,
     forceful_keyboard_interrupt: bool = True,
 ) -> Callable[[Callable[P, T]], Callable[P, T | _EMPTY]]:
     """Limit a function's resource consumption on each call
@@ -668,15 +669,15 @@
         Units available are "s", "m", "h".
 
     wall_time : int | tuple[float, str] | None = None
         The amount of total wall time in seconds to limit to
         Can provide in (time, units) such as (1.5, "h") to indicate one and a half hours.
         Units available are "s", "m", "h"
 
-    context : "fork" | "forkserver" | "spawn" | None = None
+    context : "fork" | "forkserver" | "spawn" | BaseContext | None = None
         The context to use with multiprocessing.get_context()
         * https://docs.python.org/3/library/multiprocessing.html#multiprocessing.get_context
 
     raises : bool = True
         Whether any error from the subprocess should filter up and be raised.
 
     warnings : bool = True
```

### Comparing `pynisher-1.0.6/pynisher/support.py` & `pynisher-1.0.7/pynisher/support.py`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.6/pynisher/util.py` & `pynisher-1.0.7/pynisher/util.py`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.6/pynisher/win_errcodes.py` & `pynisher-1.0.7/pynisher/win_errcodes.py`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.6/pynisher.egg-info/PKG-INFO` & `pynisher-1.0.7/pynisher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynisher
-Version: 1.0.6
+Version: 1.0.7
 Summary: A library to limit the resources used by functions using subprocesses
 Home-page: https://github.com/automl/pynisher
 Author: ('Stefan Falkner, Christina Hernandez-Wunsch, Samuel Mueller,Matthias Feurer, Francisco Rivera, Eddie Bergman and Rene Sass',)
 Author-email: feurerm@informatik.uni-freiburg.de
 License: MIT
 Keywords: resources
 Classifier: License :: OSI Approved :: BSD License
@@ -226,15 +226,15 @@
 # the controlling process. The exception to this are MemoryErrors which occur
 # in the subprocess, we convert these to MemoryLimitException.
 raises: bool = True
 
 
 # This is the multiprocess context used, please refer to their documentation
 # https://docs.python.org/3/library/multiprocessing.html#contexts-and-start-methods
-context: "fork" | "spawn" | "forkserver" | None = None
+context: "fork" | "spawn" | "forkserver" | BaseContext | None = None
 
 
 # Whether to emit warnings from  limit or not. The current warnings:
 # * When the memory limit is lower than the starting memory of a process
 # * When trying to remove the memory limit for sending back information
 #   from the subprocess to the main process
 warnings: bool = True
```

### Comparing `pynisher-1.0.6/pyproject.toml` & `pynisher-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynisher-1.0.6/setup.py` & `pynisher-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 readme = Path(__file__).parent / "README.md"
 
 with readme.open("r") as fh:
     long_description = fh.read()
 
 setup(
     name="pynisher",
-    version="1.0.6",
+    version="1.0.7",
     packages=find_packages(where=".", include=["pynisher*"], exclude=["test*"]),
     include_package_data=True,
     install_requires=[
         "psutil",
         "typing_extensions",
         "pywin32; platform_system=='Windows'",
     ],
```

