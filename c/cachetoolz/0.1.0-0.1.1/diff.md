# Comparing `tmp/cachetoolz-0.1.0.tar.gz` & `tmp/cachetoolz-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachetoolz-0.1.0.tar", max compression
+gzip compressed data, was "cachetoolz-0.1.1.tar", max compression
```

## Comparing `cachetoolz-0.1.0.tar` & `cachetoolz-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1077 2023-07-15 00:00:01.404142 cachetoolz-0.1.0/LICENSE
--rw-r--r--   0        0        0     9978 2023-07-19 01:22:12.109287 cachetoolz-0.1.0/README.md
--rw-r--r--   0        0        0      394 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/__init__.py
--rw-r--r--   0        0        0      223 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/abc/__init__.py
--rw-r--r--   0        0        0     2181 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/abc/backend.py
--rw-r--r--   0        0        0      618 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/abc/coder.py
--rw-r--r--   0        0        0      623 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/abc/serializer.py
--rw-r--r--   0        0        0      315 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/backend/__init__.py
--rw-r--r--   0        0        0     4619 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/backend/inmemory.py
--rw-r--r--   0        0        0     6595 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/backend/mongo.py
--rw-r--r--   0        0        0     4212 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/backend/redis.py
--rw-r--r--   0        0        0     2151 2023-07-19 00:56:58.493490 cachetoolz-0.1.0/cachetoolz/coder/__init__.py
--rw-r--r--   0        0        0     2423 2023-07-19 01:21:14.345496 cachetoolz-0.1.0/cachetoolz/coder/decoder.py
--rw-r--r--   0        0        0     3761 2023-07-19 00:55:36.997518 cachetoolz-0.1.0/cachetoolz/coder/encoder.py
--rw-r--r--   0        0        0     3907 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/decorator.py
--rw-r--r--   0        0        0      250 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/exceptions.py
--rw-r--r--   0        0        0      697 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/log.py
--rw-r--r--   0        0        0      633 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/types.py
--rw-r--r--   0        0        0     3194 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/utils.py
--rw-r--r--   0        0        0     3063 2023-07-19 01:00:36.969226 cachetoolz-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    11519 1970-01-01 00:00:00.000000 cachetoolz-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-15 00:00:01.404142 cachetoolz-0.1.1/LICENSE
+-rw-r--r--   0        0        0    10565 2023-07-19 01:45:34.070630 cachetoolz-0.1.1/README.md
+-rw-r--r--   0        0        0      394 2023-07-18 19:29:39.465545 cachetoolz-0.1.1/cachetoolz/__init__.py
+-rw-r--r--   0        0        0      223 2023-07-18 19:29:39.465545 cachetoolz-0.1.1/cachetoolz/abc/__init__.py
+-rw-r--r--   0        0        0     2181 2023-07-18 19:29:39.465545 cachetoolz-0.1.1/cachetoolz/abc/backend.py
+-rw-r--r--   0        0        0      618 2023-07-18 19:29:39.465545 cachetoolz-0.1.1/cachetoolz/abc/coder.py
+-rw-r--r--   0        0        0      623 2023-07-18 19:29:39.465545 cachetoolz-0.1.1/cachetoolz/abc/serializer.py
+-rw-r--r--   0        0        0      315 2023-07-18 19:29:39.465545 cachetoolz-0.1.1/cachetoolz/backend/__init__.py
+-rw-r--r--   0        0        0     4619 2023-07-18 19:29:39.465545 cachetoolz-0.1.1/cachetoolz/backend/inmemory.py
+-rw-r--r--   0        0        0     6595 2023-07-18 19:29:39.465545 cachetoolz-0.1.1/cachetoolz/backend/mongo.py
+-rw-r--r--   0        0        0     4212 2023-07-18 19:29:39.465545 cachetoolz-0.1.1/cachetoolz/backend/redis.py
+-rw-r--r--   0        0        0     2151 2023-07-19 00:56:58.493490 cachetoolz-0.1.1/cachetoolz/coder/__init__.py
+-rw-r--r--   0        0        0     2413 2023-07-19 01:29:30.131293 cachetoolz-0.1.1/cachetoolz/coder/decoder.py
+-rw-r--r--   0        0        0     3733 2023-07-19 01:29:30.135293 cachetoolz-0.1.1/cachetoolz/coder/encoder.py
+-rw-r--r--   0        0        0     3907 2023-07-18 19:29:39.465545 cachetoolz-0.1.1/cachetoolz/decorator.py
+-rw-r--r--   0        0        0      250 2023-07-18 19:29:39.465545 cachetoolz-0.1.1/cachetoolz/exceptions.py
+-rw-r--r--   0        0        0      702 2023-07-19 01:55:43.832002 cachetoolz-0.1.1/cachetoolz/log.py
+-rw-r--r--   0        0        0      633 2023-07-18 19:29:39.465545 cachetoolz-0.1.1/cachetoolz/types.py
+-rw-r--r--   0        0        0     3194 2023-07-18 19:29:39.465545 cachetoolz-0.1.1/cachetoolz/utils.py
+-rw-r--r--   0        0        0     3063 2023-07-19 01:56:10.351889 cachetoolz-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    12106 1970-01-01 00:00:00.000000 cachetoolz-0.1.1/PKG-INFO
```

### Comparing `cachetoolz-0.1.0/LICENSE` & `cachetoolz-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.0/README.md` & `cachetoolz-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,33 @@
 
 The decorator provided by this library automatically checks if the function has been called with the same set of arguments before. If it has, instead of executing the function again, it returns the cached result, saving valuable processing time. However, if the function is called with new or different arguments, it will execute normally and cache the result for future use.
 
 By incorporating this caching decorator into your code, you can optimize the execution of functions that involve complex computations, database queries, API calls, or any other operations that could benefit from caching.
 
 Overall, this library simplifies the implementation of caching in your applications, allowing you to enhance performance and reduce resource consumption effectively.
 
+---
+# Summary
+* **[Installation](#installation)**
+* **[How to use](#how-to-use)**
+  * **[Cache parameters](#cache-parameters)**
+    * **[Key generator](#key-generator)**
+  * **[Cache clear](#cache-clear)**
+  * **[Backends](#backends)**
+    * **[In Memory](#in-memory)**
+    * **[Remote Backends](#remote-backends)**
+        * **[Redis](#redis)**
+        * **[Mongo](#mongo)**
+  * **[Coder](#coder)**
+    * **[Supported Types](#supported-types)**
+    * **[Register Coder](#register-coder)**
+    * **[Register Encode](#register-encode)**
+    * **[Register Decode](#register-decode)**
+---
+
 # Installation
 cachetoolz is available from [PyPI](https://pypi.org/project/cachetoolz/) and can be installed by running
 
 ```bash
 pip install cachetoolz
 ```
 
@@ -284,15 +303,15 @@
 
     def decode(self, value):
         return deque(val['iterable'], val['maxlen'])
 
 coder.register(DequeCoder(foo='bar'))
 ```
 
-### Redister Encode
+### Register Encode
 If you have no need to decode the result or prefer to add it separately, you have the option to register a single encoder.
 
 ```python
 from collections import deque
 
 from cachetoolz.coder import encoder
```

### Comparing `cachetoolz-0.1.0/cachetoolz/abc/backend.py` & `cachetoolz-0.1.1/cachetoolz/abc/backend.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.0/cachetoolz/abc/coder.py` & `cachetoolz-0.1.1/cachetoolz/abc/coder.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.0/cachetoolz/abc/serializer.py` & `cachetoolz-0.1.1/cachetoolz/abc/serializer.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.0/cachetoolz/backend/inmemory.py` & `cachetoolz-0.1.1/cachetoolz/backend/inmemory.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.0/cachetoolz/backend/mongo.py` & `cachetoolz-0.1.1/cachetoolz/backend/mongo.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.0/cachetoolz/backend/redis.py` & `cachetoolz-0.1.1/cachetoolz/backend/redis.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.0/cachetoolz/coder/__init__.py` & `cachetoolz-0.1.1/cachetoolz/coder/__init__.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.0/cachetoolz/coder/decoder.py` & `cachetoolz-0.1.1/cachetoolz/coder/decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     IPv4Network,
     IPv6Address,
     IPv6Interface,
     IPv6Network,
 )
 from json import JSONDecoder
 from pathlib import Path
-from typing import Any, ClassVar, Dict, Optional
+from typing import Any, ClassVar, Dict
 from uuid import UUID
 
 from .. import types
 from ..exceptions import RegistryError, UnknownDecoderError
 
 
 class Decoder(JSONDecoder):
```

### Comparing `cachetoolz-0.1.0/cachetoolz/coder/encoder.py` & `cachetoolz-0.1.1/cachetoolz/coder/encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     IPv4Network,
     IPv6Address,
     IPv6Interface,
     IPv6Network,
 )
 from json import JSONEncoder
 from pathlib import PosixPath
-from typing import Optional
 from uuid import UUID
 
 try:
     from inspect import get_annotations
 except ImportError:
     from get_annotations import get_annotations
```

### Comparing `cachetoolz-0.1.0/cachetoolz/decorator.py` & `cachetoolz-0.1.1/cachetoolz/decorator.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.0/cachetoolz/log.py` & `cachetoolz-0.1.1/cachetoolz/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Logging implemetation."""
 
 import logging
 
 
-def get_logger(name='cache') -> logging.Logger:
+def get_logger(name='cachetoolz') -> logging.Logger:
     """Get a logger.
 
     Parameters
     ----------
     name
         logger name
```

### Comparing `cachetoolz-0.1.0/cachetoolz/types.py` & `cachetoolz-0.1.1/cachetoolz/types.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.0/cachetoolz/utils.py` & `cachetoolz-0.1.1/cachetoolz/utils.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.0/pyproject.toml` & `cachetoolz-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cachetoolz"
-version = "0.1.0"
+version = "0.1.1"
 description = "This library provides a decorator for caching functions"
 license = "MIT"
 authors = ["Igor Taconi <igor.taconi@protonmail.com>"]
 maintainers = ["Igor Taconi <igor.taconi@protonmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/taconi/cachetoolz/#readme"
 repository = "https://github.com/taconi/cachetoolz/"
```

### Comparing `cachetoolz-0.1.0/PKG-INFO` & `cachetoolz-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachetoolz
-Version: 0.1.0
+Version: 0.1.1
 Summary: This library provides a decorator for caching functions
 Home-page: https://github.com/taconi/cachetoolz/#readme
 License: MIT
 Keywords: python,cache,async,redis,mongo
 Author: Igor Taconi
 Author-email: igor.taconi@protonmail.com
 Maintainer: Igor Taconi
@@ -52,14 +52,33 @@
 
 The decorator provided by this library automatically checks if the function has been called with the same set of arguments before. If it has, instead of executing the function again, it returns the cached result, saving valuable processing time. However, if the function is called with new or different arguments, it will execute normally and cache the result for future use.
 
 By incorporating this caching decorator into your code, you can optimize the execution of functions that involve complex computations, database queries, API calls, or any other operations that could benefit from caching.
 
 Overall, this library simplifies the implementation of caching in your applications, allowing you to enhance performance and reduce resource consumption effectively.
 
+---
+# Summary
+* **[Installation](#installation)**
+* **[How to use](#how-to-use)**
+  * **[Cache parameters](#cache-parameters)**
+    * **[Key generator](#key-generator)**
+  * **[Cache clear](#cache-clear)**
+  * **[Backends](#backends)**
+    * **[In Memory](#in-memory)**
+    * **[Remote Backends](#remote-backends)**
+        * **[Redis](#redis)**
+        * **[Mongo](#mongo)**
+  * **[Coder](#coder)**
+    * **[Supported Types](#supported-types)**
+    * **[Register Coder](#register-coder)**
+    * **[Register Encode](#register-encode)**
+    * **[Register Decode](#register-decode)**
+---
+
 # Installation
 cachetoolz is available from [PyPI](https://pypi.org/project/cachetoolz/) and can be installed by running
 
 ```bash
 pip install cachetoolz
 ```
 
@@ -321,15 +340,15 @@
 
     def decode(self, value):
         return deque(val['iterable'], val['maxlen'])
 
 coder.register(DequeCoder(foo='bar'))
 ```
 
-### Redister Encode
+### Register Encode
 If you have no need to decode the result or prefer to add it separately, you have the option to register a single encoder.
 
 ```python
 from collections import deque
 
 from cachetoolz.coder import encoder
```

