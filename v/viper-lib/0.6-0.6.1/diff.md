# Comparing `tmp/viper_lib-0.6.tar.gz` & `tmp/viper_lib-0.6.1.tar.gz`

## Comparing `viper_lib-0.6.tar` & `viper_lib-0.6.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper.pth
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/__init__.py
--rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/better_threading.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/exceptions.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/format.py
--rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/frozendict.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/interactive.py
--rw-r--r--   0        0        0     5329 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/io.py
--rw-r--r--   0        0        0    15408 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/pickle_utils.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/warnings.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/abc/__init__.py
--rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/abc/connection.py
--rw-r--r--   0        0        0    15818 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/abc/io.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/building/__init__.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/building/module_tools.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/compress/__init__.py
--rw-r--r--   0        0        0     8976 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/compress/flux.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/debugging/__init__.py
--rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/debugging/chrono.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/debugging/utils.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/meta/__init__.py
--rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/meta/decorators.py
--rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/meta/iterable.py
--rw-r--r--   0        0        0    17549 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/meta/procedural.py
--rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 viper_lib-0.6/Viper/meta/utils.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 viper_lib-0.6/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 viper_lib-0.6/LICENSE
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 viper_lib-0.6/README.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 viper_lib-0.6/pyproject.toml
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 viper_lib-0.6/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 viper_lib-0.6.1/Viper.pth
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 viper_lib-0.6.1/Viper/__init__.py
+-rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 viper_lib-0.6.1/Viper/better_threading.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 viper_lib-0.6.1/Viper/exceptions.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 viper_lib-0.6.1/Viper/format.py
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 viper_lib-0.6.1/Viper/frozendict.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 viper_lib-0.6.1/Viper/interactive.py
+-rw-r--r--   0        0        0     5329 2020-02-02 00:00:00.000000 viper_lib-0.6.1/Viper/io.py
+-rw-r--r--   0        0        0    15408 2020-02-02 00:00:00.000000 viper_lib-0.6.1/Viper/pickle_utils.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 viper_lib-0.6.1/Viper/warnings.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 viper_lib-0.6.1/Viper/abc/__init__.py
+-rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 viper_lib-0.6.1/Viper/abc/connection.py
+-rw-r--r--   0        0        0    15870 2020-02-02 00:00:00.000000 viper_lib-0.6.1/Viper/abc/io.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 viper_lib-0.6.1/Viper/building/__init__.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 viper_lib-0.6.1/Viper/building/module_tools.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 viper_lib-0.6.1/Viper/compress/__init__.py
+-rw-r--r--   0        0        0     8976 2020-02-02 00:00:00.000000 viper_lib-0.6.1/Viper/compress/flux.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 viper_lib-0.6.1/Viper/debugging/__init__.py
+-rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 viper_lib-0.6.1/Viper/debugging/chrono.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 viper_lib-0.6.1/Viper/debugging/utils.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 viper_lib-0.6.1/Viper/meta/__init__.py
+-rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 viper_lib-0.6.1/Viper/meta/decorators.py
+-rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 viper_lib-0.6.1/Viper/meta/iterable.py
+-rw-r--r--   0        0        0    17549 2020-02-02 00:00:00.000000 viper_lib-0.6.1/Viper/meta/procedural.py
+-rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 viper_lib-0.6.1/Viper/meta/utils.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 viper_lib-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 viper_lib-0.6.1/LICENSE
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 viper_lib-0.6.1/README.md
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 viper_lib-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 viper_lib-0.6.1/PKG-INFO
```

### Comparing `viper_lib-0.6/Viper/better_threading.py` & `viper_lib-0.6.1/Viper/better_threading.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.6/Viper/format.py` & `viper_lib-0.6.1/Viper/format.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.6/Viper/frozendict.py` & `viper_lib-0.6.1/Viper/frozendict.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.6/Viper/interactive.py` & `viper_lib-0.6.1/Viper/interactive.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.6/Viper/io.py` & `viper_lib-0.6.1/Viper/io.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.6/Viper/pickle_utils.py` & `viper_lib-0.6.1/Viper/pickle_utils.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.6/Viper/warnings.py` & `viper_lib-0.6.1/Viper/warnings.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.6/Viper/abc/connection.py` & `viper_lib-0.6.1/Viper/abc/connection.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.6/Viper/abc/io.py` & `viper_lib-0.6.1/Viper/abc/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,17 +233,18 @@
     def read_blocking(self) -> bool:
         """
         Returns True if the stream can block on reading when no data are available.
         """
         raise NotImplementedError
 
     @property
-    @abstractmethod
     def readable(self) -> int | float:
-        raise NotImplementedError
+        if self.closed:
+            return 0
+        return STREAM_PACKET_SIZE
     
     @abstractmethod
     def read(self, size : int | float = float("inf"), /) -> Buf:
         """
         Reads size pieces of data. If size is float("inf"), then reads as much data as possible.
         If not blocking and no data is available, returns empty data.
         If blocking and no data is available, it should block until enough data is available.
@@ -347,17 +348,18 @@
     def write_blocking(self) -> bool:
         """
         Returns True if the stream can block on writing when no data can be written.
         """
         raise NotImplementedError
 
     @property
-    @abstractmethod
     def writable(self) -> int | float:
-        raise NotImplementedError
+        if self.closed:
+            return 0
+        return STREAM_PACKET_SIZE
 
     def flush(self):
         """
         Flushes the write buffers of the stream if applicable. Does nothing by default.
         """
         if self.closed:
             raise IOClosedError("Cannot flush closed stream")
```

### Comparing `viper_lib-0.6/Viper/building/module_tools.py` & `viper_lib-0.6.1/Viper/building/module_tools.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.6/Viper/compress/flux.py` & `viper_lib-0.6.1/Viper/compress/flux.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.6/Viper/debugging/chrono.py` & `viper_lib-0.6.1/Viper/debugging/chrono.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.6/Viper/debugging/utils.py` & `viper_lib-0.6.1/Viper/debugging/utils.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.6/Viper/meta/decorators.py` & `viper_lib-0.6.1/Viper/meta/decorators.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.6/Viper/meta/iterable.py` & `viper_lib-0.6.1/Viper/meta/iterable.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.6/Viper/meta/procedural.py` & `viper_lib-0.6.1/Viper/meta/procedural.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.6/Viper/meta/utils.py` & `viper_lib-0.6.1/Viper/meta/utils.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.6/.gitignore` & `viper_lib-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `viper_lib-0.6/LICENSE` & `viper_lib-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `viper_lib-0.6/README.md` & `viper_lib-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `viper_lib-0.6/pyproject.toml` & `viper_lib-0.6.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "viper_lib"
-version = "0.6"
+version = "0.6.1"
 authors = [
   { name="Vincent Raulin", email="vincent.raulin.n7@gmail.com" },
 ]
 description = "A Python library full of useful Python tools."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
```

### Comparing `viper_lib-0.6/PKG-INFO` & `viper_lib-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viper_lib
-Version: 0.6
+Version: 0.6.1
 Summary: A Python library full of useful Python tools.
 Project-URL: Repository, https://github.com/MrVoustache/Viper
 Project-URL: Bug Tracker, https://github.com/MrVoustache/Viper/issues
 Author-email: Vincent Raulin <vincent.raulin.n7@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Vincent Raulin
```

