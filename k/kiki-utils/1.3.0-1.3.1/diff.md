# Comparing `tmp/kiki_utils-1.3.0.tar.gz` & `tmp/kiki_utils-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiki_utils-1.3.0.tar", last modified: Sat Feb  4 08:48:19 2023, max compression
+gzip compressed data, was "kiki_utils-1.3.1.tar", last modified: Wed Jul 19 07:16:33 2023, max compression
```

## Comparing `kiki_utils-1.3.0.tar` & `kiki_utils-1.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-02-04 08:48:19.767185 kiki_utils-1.3.0/
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1066 2022-11-28 02:36:38.000000 kiki_utils-1.3.0/LICENSE.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      240 2023-02-04 08:48:19.767185 kiki_utils-1.3.0/PKG-INFO
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2022-11-28 02:36:38.000000 kiki_utils-1.3.0/README.md
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-02-04 08:48:19.767185 kiki_utils-1.3.0/kiki_utils.egg-info/
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      240 2023-02-04 08:48:19.000000 kiki_utils-1.3.0/kiki_utils.egg-info/PKG-INFO
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      569 2023-02-04 08:48:19.000000 kiki_utils-1.3.0/kiki_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-02-04 08:48:19.000000 kiki_utils-1.3.0/kiki_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      160 2023-02-04 08:48:19.000000 kiki_utils-1.3.0/kiki_utils.egg-info/requires.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       10 2023-02-04 08:48:19.000000 kiki_utils-1.3.0/kiki_utils.egg-info/top_level.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-02-04 08:48:19.000000 kiki_utils-1.3.0/kiki_utils.egg-info/zip-safe
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-02-04 08:48:19.767185 kiki_utils-1.3.0/kikiutils/
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)       13 2022-11-28 02:36:38.000000 kiki_utils-1.3.0/kikiutils/__init__.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1952 2023-02-04 08:39:18.000000 kiki_utils-1.3.0/kikiutils/aes.py
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     1874 2023-02-04 08:39:42.000000 kiki_utils-1.3.0/kikiutils/aiofile.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1748 2023-02-04 08:32:01.000000 kiki_utils-1.3.0/kikiutils/check.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      188 2022-11-28 02:36:38.000000 kiki_utils-1.3.0/kikiutils/cookie.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     2256 2023-01-05 10:12:29.000000 kiki_utils-1.3.0/kikiutils/decorators.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     2206 2023-02-04 08:39:46.000000 kiki_utils-1.3.0/kikiutils/file.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      769 2023-02-04 08:44:11.000000 kiki_utils-1.3.0/kikiutils/hash.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      152 2022-11-28 02:36:38.000000 kiki_utils-1.3.0/kikiutils/import_utils.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      979 2023-02-04 08:44:34.000000 kiki_utils-1.3.0/kikiutils/json.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      313 2022-11-28 02:36:38.000000 kiki_utils-1.3.0/kikiutils/log.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      573 2023-01-22 12:55:32.000000 kiki_utils-1.3.0/kikiutils/network.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     3265 2023-02-04 08:35:20.000000 kiki_utils-1.3.0/kikiutils/requests.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1285 2023-02-04 08:45:08.000000 kiki_utils-1.3.0/kikiutils/string.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1613 2022-12-11 02:05:07.000000 kiki_utils-1.3.0/kikiutils/time.py
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      106 2023-02-04 08:43:27.000000 kiki_utils-1.3.0/kikiutils/typehint.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      592 2023-02-04 08:36:34.000000 kiki_utils-1.3.0/kikiutils/uuid.py
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       38 2023-02-04 08:48:19.767185 kiki_utils-1.3.0/setup.cfg
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      673 2023-02-04 08:47:27.000000 kiki_utils-1.3.0/setup.py
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-07-19 07:16:33.928846 kiki_utils-1.3.1/
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1066 2023-07-19 07:09:04.000000 kiki_utils-1.3.1/LICENSE.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      240 2023-07-19 07:16:33.928846 kiki_utils-1.3.1/PKG-INFO
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)       48 2023-07-19 07:08:23.000000 kiki_utils-1.3.1/README.md
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-07-19 07:16:33.924845 kiki_utils-1.3.1/kiki_utils.egg-info/
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      240 2023-07-19 07:16:33.000000 kiki_utils-1.3.1/kiki_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      569 2023-07-19 07:16:33.000000 kiki_utils-1.3.1/kiki_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-07-19 07:16:33.000000 kiki_utils-1.3.1/kiki_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      160 2023-07-19 07:16:33.000000 kiki_utils-1.3.1/kiki_utils.egg-info/requires.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       10 2023-07-19 07:16:33.000000 kiki_utils-1.3.1/kiki_utils.egg-info/top_level.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-07-19 07:14:37.000000 kiki_utils-1.3.1/kiki_utils.egg-info/zip-safe
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-07-19 07:16:33.928846 kiki_utils-1.3.1/kikiutils/
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)       13 2022-11-28 02:36:38.000000 kiki_utils-1.3.1/kikiutils/__init__.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1952 2023-02-04 08:39:18.000000 kiki_utils-1.3.1/kikiutils/aes.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1874 2023-02-04 08:39:42.000000 kiki_utils-1.3.1/kikiutils/aiofile.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1830 2023-06-23 04:31:52.000000 kiki_utils-1.3.1/kikiutils/check.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      188 2022-11-28 02:36:38.000000 kiki_utils-1.3.1/kikiutils/cookie.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     3431 2023-07-19 07:14:09.000000 kiki_utils-1.3.1/kikiutils/decorators.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     2206 2023-02-04 08:39:46.000000 kiki_utils-1.3.1/kikiutils/file.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      769 2023-02-04 08:44:11.000000 kiki_utils-1.3.1/kikiutils/hash.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      152 2022-11-28 02:36:38.000000 kiki_utils-1.3.1/kikiutils/import_utils.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      979 2023-02-04 08:44:34.000000 kiki_utils-1.3.1/kikiutils/json.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      313 2022-11-28 02:36:38.000000 kiki_utils-1.3.1/kikiutils/log.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      573 2023-01-22 12:55:32.000000 kiki_utils-1.3.1/kikiutils/network.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     3265 2023-02-04 08:35:20.000000 kiki_utils-1.3.1/kikiutils/requests.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1285 2023-02-04 08:45:08.000000 kiki_utils-1.3.1/kikiutils/string.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1613 2022-12-11 02:05:07.000000 kiki_utils-1.3.1/kikiutils/time.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      106 2023-02-04 08:43:27.000000 kiki_utils-1.3.1/kikiutils/typehint.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      592 2023-02-04 08:36:34.000000 kiki_utils-1.3.1/kikiutils/uuid.py
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       38 2023-07-19 07:16:33.928846 kiki_utils-1.3.1/setup.cfg
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      673 2023-07-19 07:07:57.000000 kiki_utils-1.3.1/setup.py
```

### Comparing `kiki_utils-1.3.0/LICENSE.txt` & `kiki_utils-1.3.1/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 kiki-kanri
+Copyright (c) 2023 kiki-kanri
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `kiki_utils-1.3.0/kiki_utils.egg-info/SOURCES.txt` & `kiki_utils-1.3.1/kiki_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiki_utils-1.3.0/kikiutils/aes.py` & `kiki_utils-1.3.1/kikiutils/aes.py`

 * *Files identical despite different names*

### Comparing `kiki_utils-1.3.0/kikiutils/aiofile.py` & `kiki_utils-1.3.1/kikiutils/aiofile.py`

 * *Files identical despite different names*

### Comparing `kiki_utils-1.3.0/kikiutils/decorators.py` & `kiki_utils-1.3.1/kikiutils/decorators.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,54 @@
 import time
 
+from asyncio import create_task, sleep, Task
 from functools import wraps
 from inspect import iscoroutinefunction
+from threading import Timer
 from typing import Callable
 
 
+def debounce(delay: float | int):
+    """Defers the execution of a function until it is not called again within the specified time since the last call.
+
+    Supports async and sync function.
+    """
+
+    def decorator(view_func: Callable):
+        if iscoroutinefunction(view_func):
+            task: Task = None
+
+            @wraps(view_func)
+            async def awrapped_view(*args, **kwargs):
+                nonlocal task
+
+                if task is not None:
+                    task.cancel()
+
+                async def aexec():
+                    await sleep(delay)
+                    await view_func(*args, **kwargs)
+
+                task = create_task(aexec())
+            return awrapped_view
+
+        @wraps(view_func)
+        def wrapped_view(*args, **kwargs):
+            def exec():
+                view_func(*args, **kwargs)
+
+            if hasattr(wrapped_view, '_timer'):
+                wrapped_view._timer.cancel()
+
+            wrapped_view._timer = Timer(delay, exec)
+            wrapped_view._timer.start()
+        return wrapped_view
+    return decorator
+
+
 def show_cost_time(view_func: Callable):
     """Run the function and show cost time.
 
     Supports async and sync function.
     """
 
     if iscoroutinefunction(view_func):
@@ -25,15 +65,15 @@
         se = time.time()
         result = view_func(*args, **kwargs)
         print(f'Function {view_func.__name__} cost time is {time.time() - se} s')
         return result
     return wrapped_view
 
 
-def try_and_get_bool(view_func):
+def try_and_get_bool(view_func: Callable):
     """Run the function use try/catch.
 
     Returns False if there was an error. Otherwise return True.
 
     Supports async and sync function.
     """
 
@@ -54,15 +94,15 @@
             view_func(*args, **kwargs)
             return True
         except:
             return False
     return wrapped_view
 
 
-def try_and_get_data(view_func):
+def try_and_get_data(view_func: Callable):
     """Run the function use try/catch.
 
     Returns None if there was an error. Otherwise return the function result.
 
     Supports async and sync function.
     """
```

### Comparing `kiki_utils-1.3.0/kikiutils/file.py` & `kiki_utils-1.3.1/kikiutils/file.py`

 * *Files identical despite different names*

### Comparing `kiki_utils-1.3.0/kikiutils/hash.py` & `kiki_utils-1.3.1/kikiutils/hash.py`

 * *Files identical despite different names*

### Comparing `kiki_utils-1.3.0/kikiutils/json.py` & `kiki_utils-1.3.1/kikiutils/json.py`

 * *Files identical despite different names*

### Comparing `kiki_utils-1.3.0/kikiutils/network.py` & `kiki_utils-1.3.1/kikiutils/network.py`

 * *Files identical despite different names*

### Comparing `kiki_utils-1.3.0/kikiutils/requests.py` & `kiki_utils-1.3.1/kikiutils/requests.py`

 * *Files identical despite different names*

### Comparing `kiki_utils-1.3.0/kikiutils/string.py` & `kiki_utils-1.3.1/kikiutils/string.py`

 * *Files identical despite different names*

### Comparing `kiki_utils-1.3.0/kikiutils/time.py` & `kiki_utils-1.3.1/kikiutils/time.py`

 * *Files identical despite different names*

### Comparing `kiki_utils-1.3.0/kikiutils/uuid.py` & `kiki_utils-1.3.1/kikiutils/uuid.py`

 * *Files identical despite different names*

### Comparing `kiki_utils-1.3.0/setup.py` & `kiki_utils-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     name='kiki_utils',
     classifiers=[
         'License :: Freely Distributable'
     ],
     packages=find_packages(),
     include_package_data=True,
     zip_safe=True,
-    version='1.3.0',
+    version='1.3.1',
     description='Utils functions.',
     author='kiki-kanri',
     author_email='a470666@gmail.com',
     keywords=['Utils'],
     install_requires=[
         'aiofiles',
         'aioshutil',
```

