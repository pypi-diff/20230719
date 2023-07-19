# Comparing `tmp/cachetoolz-0.0.1.tar.gz` & `tmp/cachetoolz-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachetoolz-0.0.1.tar", max compression
+gzip compressed data, was "cachetoolz-0.1.0.tar", max compression
```

## Comparing `cachetoolz-0.0.1.tar` & `cachetoolz-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1077 2023-07-15 00:00:01.404142 cachetoolz-0.0.1/LICENSE
--rw-r--r--   0        0        0     2840 2023-07-18 18:57:10.052212 cachetoolz-0.0.1/README.md
--rw-r--r--   0        0        0      394 2023-07-15 20:28:16.920819 cachetoolz-0.0.1/cachetoolz/__init__.py
--rw-r--r--   0        0        0      223 2023-07-15 00:22:02.122353 cachetoolz-0.0.1/cachetoolz/abc/__init__.py
--rw-r--r--   0        0        0     2181 2023-07-18 16:39:46.482306 cachetoolz-0.0.1/cachetoolz/abc/backend.py
--rw-r--r--   0        0        0      618 2023-07-15 00:22:02.122353 cachetoolz-0.0.1/cachetoolz/abc/coder.py
--rw-r--r--   0        0        0      623 2023-07-15 00:22:02.122353 cachetoolz-0.0.1/cachetoolz/abc/serializer.py
--rw-r--r--   0        0        0      315 2023-07-15 20:28:16.920819 cachetoolz-0.0.1/cachetoolz/backend/__init__.py
--rw-r--r--   0        0        0     4619 2023-07-18 16:39:46.482306 cachetoolz-0.0.1/cachetoolz/backend/inmemory.py
--rw-r--r--   0        0        0     6599 2023-07-15 20:28:16.920819 cachetoolz-0.0.1/cachetoolz/backend/mongo.py
--rw-r--r--   0        0        0     4214 2023-07-15 20:28:16.920819 cachetoolz-0.0.1/cachetoolz/backend/redis.py
--rw-r--r--   0        0        0     2160 2023-07-18 16:39:46.482306 cachetoolz-0.0.1/cachetoolz/coder/__init__.py
--rw-r--r--   0        0        0     2486 2023-07-18 16:39:46.482306 cachetoolz-0.0.1/cachetoolz/coder/decoder.py
--rw-r--r--   0        0        0     3821 2023-07-18 16:39:46.482306 cachetoolz-0.0.1/cachetoolz/coder/encoder.py
--rw-r--r--   0        0        0     3907 2023-07-18 16:39:46.482306 cachetoolz-0.0.1/cachetoolz/decorator.py
--rw-r--r--   0        0        0      250 2023-07-15 00:22:02.122353 cachetoolz-0.0.1/cachetoolz/exceptions.py
--rw-r--r--   0        0        0      697 2023-07-15 00:22:02.122353 cachetoolz-0.0.1/cachetoolz/log.py
--rw-r--r--   0        0        0      633 2023-07-18 16:39:46.482306 cachetoolz-0.0.1/cachetoolz/types.py
--rw-r--r--   0        0        0     3194 2023-07-18 16:39:46.482306 cachetoolz-0.0.1/cachetoolz/utils.py
--rw-r--r--   0        0        0     3063 2023-07-18 18:56:39.232375 cachetoolz-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4381 1970-01-01 00:00:00.000000 cachetoolz-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-15 00:00:01.404142 cachetoolz-0.1.0/LICENSE
+-rw-r--r--   0        0        0     9978 2023-07-19 01:22:12.109287 cachetoolz-0.1.0/README.md
+-rw-r--r--   0        0        0      394 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/__init__.py
+-rw-r--r--   0        0        0      223 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/abc/__init__.py
+-rw-r--r--   0        0        0     2181 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/abc/backend.py
+-rw-r--r--   0        0        0      618 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/abc/coder.py
+-rw-r--r--   0        0        0      623 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/abc/serializer.py
+-rw-r--r--   0        0        0      315 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/backend/__init__.py
+-rw-r--r--   0        0        0     4619 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/backend/inmemory.py
+-rw-r--r--   0        0        0     6595 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/backend/mongo.py
+-rw-r--r--   0        0        0     4212 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/backend/redis.py
+-rw-r--r--   0        0        0     2151 2023-07-19 00:56:58.493490 cachetoolz-0.1.0/cachetoolz/coder/__init__.py
+-rw-r--r--   0        0        0     2423 2023-07-19 01:21:14.345496 cachetoolz-0.1.0/cachetoolz/coder/decoder.py
+-rw-r--r--   0        0        0     3761 2023-07-19 00:55:36.997518 cachetoolz-0.1.0/cachetoolz/coder/encoder.py
+-rw-r--r--   0        0        0     3907 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/decorator.py
+-rw-r--r--   0        0        0      250 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/exceptions.py
+-rw-r--r--   0        0        0      697 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/log.py
+-rw-r--r--   0        0        0      633 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/types.py
+-rw-r--r--   0        0        0     3194 2023-07-18 19:29:39.465545 cachetoolz-0.1.0/cachetoolz/utils.py
+-rw-r--r--   0        0        0     3063 2023-07-19 01:00:36.969226 cachetoolz-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    11519 1970-01-01 00:00:00.000000 cachetoolz-0.1.0/PKG-INFO
```

### Comparing `cachetoolz-0.0.1/LICENSE` & `cachetoolz-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.0.1/cachetoolz/abc/backend.py` & `cachetoolz-0.1.0/cachetoolz/abc/backend.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.0.1/cachetoolz/abc/coder.py` & `cachetoolz-0.1.0/cachetoolz/abc/coder.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.0.1/cachetoolz/abc/serializer.py` & `cachetoolz-0.1.0/cachetoolz/abc/serializer.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.0.1/cachetoolz/backend/inmemory.py` & `cachetoolz-0.1.0/cachetoolz/backend/inmemory.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.0.1/cachetoolz/backend/mongo.py` & `cachetoolz-0.1.0/cachetoolz/backend/mongo.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 
 from ..abc import AsyncBackendABC, BackendABC
 
 
 class MongoBackend(BackendABC):
     """MongoDB cache."""
 
-    def __init__(self, url: str, database: str = '.cache_tools'):
+    def __init__(self, url: str, database: str = '.cachetoolz'):
         """Initialize the instance.
 
         Parameters
         ----------
         url
             Mongo url
         database
             Cache database name
 
         """
         try:
             from pymongo import MongoClient
         except ImportError as exc:
             raise RuntimeError(
-                "Install cache_tools with the 'mongo' extra in order "
+                "Install cachetoolz with the 'mongo' extra in order "
                 "to use mongo backend."
             ) from exc
 
         self._client_cls = MongoClient
 
         self._url = url
         self._database = database
@@ -123,30 +123,30 @@
         with self._get_database_or_collection() as database:
             database.drop_collection(namespace)
 
 
 class AsyncMongoBackend(AsyncBackendABC):
     """Async MongoDB cache."""
 
-    def __init__(self, url: str, database: str = '.cache_tools'):
+    def __init__(self, url: str, database: str = '.cachetoolz'):
         """Initialize the instance.
 
         Parameters
         ----------
         url
             Mongo url
         database
             Cache database name
 
         """
         try:
             from motor.motor_asyncio import AsyncIOMotorClient
         except ImportError as exc:
             raise RuntimeError(
-                "Install cache_tools with the 'mongo' extra in order "
+                "Install cachetoolz with the 'mongo' extra in order "
                 "to use mongo backend."
             ) from exc
 
         self._client_cls = AsyncIOMotorClient
 
         self._url = url
         self._database = database
```

### Comparing `cachetoolz-0.0.1/cachetoolz/backend/redis.py` & `cachetoolz-0.1.0/cachetoolz/backend/redis.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             Redis url
 
         """
         try:
             from redis import Redis
         except ImportError as exc:
             raise RuntimeError(
-                "Install cache_tools with the 'redis' extra in order "
+                "Install cachetoolz with the 'redis' extra in order "
                 "to use redis backend."
             ) from exc
 
         self._url = url
         self._backend = Redis.from_url(self._url, decode_responses=True)
 
     def __repr__(self):
@@ -102,15 +102,15 @@
             Redis url
 
         """
         try:
             from redis.asyncio import Redis
         except ImportError as exc:
             raise RuntimeError(
-                "Install cache_tools with the 'redis' extra in order "
+                "Install cachetoolz with the 'redis' extra in order "
                 "to use redis backend."
             ) from exc
 
         self._url = url
         self._backend = Redis.from_url(self._url, decode_responses=True)
 
     def __repr__(self):
```

### Comparing `cachetoolz-0.0.1/cachetoolz/coder/__init__.py` & `cachetoolz-0.1.0/cachetoolz/coder/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,16 @@
             raise RegistryError(
                 'Sereliazador is not valid, the class must have implemented '
                 'the `encode(value: type)` and `decode(value)` methods'
             )
 
         instance = serializer() if isclass(serializer) else serializer
 
-        decoder = decoder_name(instance).replace('serializer', '').strip('_')
+        name = decoder_name(instance).replace('serializer', '').strip('_')
 
-        encoder_register(instance.encode, decoder)
-        decoder_register(instance.decode, decoder)
+        encoder_register(name)(instance.encode)
+        decoder_register(name)(instance.decode)
 
         return serializer
 
 
 coder = Coder()
```

### Comparing `cachetoolz-0.0.1/cachetoolz/coder/decoder.py` & `cachetoolz-0.1.0/cachetoolz/coder/decoder.py`

 * *Files 14% similar despite different names*

```diff
@@ -59,33 +59,34 @@
 
         if decoder not in self.DECODERS:
             raise UnknownDecoderError(f'Decoder "{decoder}" not registered')
 
         return self.DECODERS[decoder](obj['__val'])
 
 
-def register(func: types.Decoder, decoder: Optional[str] = None):
+def register(name: str) -> types.Decorator:
     """Register a decoder.
 
     Parameters
     ----------
-    func
-        Decoder function.
-    key
-        Decoder key to keep de function.
+    name
+        Decoder name.
 
     Examples
     --------
     >>> from collections import deque
     >>> from typing import Any
     >>> @register('deque')
     ... def _(val: dict[str, Any]):
     ...     return deque(val['iterable'], val['maxlen'])
     ...
 
     """
-    if not callable(func):
-        raise RegistryError('decoder needs to be a callable')
 
-    decoder = decoder or re.sub(r'decode[r]?', '', func.__name__).strip('_')
-    Decoder.DECODERS[decoder] = func
-    return func
+    def wrapper(func: types.Decoder) -> types.Decoder:
+        if not callable(func):
+            raise RegistryError('decoder needs to be a callable')
+
+        Decoder.DECODERS[name] = func
+        return func
+
+    return wrapper
```

### Comparing `cachetoolz-0.0.1/cachetoolz/coder/encoder.py` & `cachetoolz-0.1.0/cachetoolz/coder/encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,50 +44,49 @@
         o
             Python object
 
         """
         return encode(o)
 
 
-def register(
-    func: types.Encoder, decoder: Optional[str] = None
-) -> types.Encoder:
+def register(name: str) -> types.Decorator:
     """Register a encoder.
 
     Parameters
     ----------
-    func
-        Encoder function.
-    decoder
-        Decoder key to keep de function.
+    name
+        Encoder name.
 
     Examples
     --------
     >>> from collections import deque
-    >>> @register
-    ... def deque_encoder(value: deque):
+    >>> @register('deque')
+    ... def _(value: deque):
     ...     return {'iterable': list(value), 'maxlen': value.maxlen}
     ...
 
     """
-    if not callable(func):
-        raise RegistryError('encoder needs to be a callable')
-    if 'value' not in (annotations := get_annotations(func)):
-        raise RegistryError(
-            'encoder needs to have a parameter named `value` '
-            'and it needs to have the type annotated'
-        )
 
-    _type = annotations['value']
-    decoder = decoder or re.sub('encode[r]?', '', func.__name__).strip('_')
+    def wrapper(func: types.Encoder) -> types.Encoder:
+        if not callable(func):
+            raise RegistryError('encoder needs to be a callable')
+        if 'value' not in (annotations := get_annotations(func)):
+            raise RegistryError(
+                'encoder needs to have a parameter named `value` '
+                'and it needs to have the type annotated'
+            )
+
+        _type = annotations['value']
+
+        encode.register(_type)(
+            lambda value: {'__val': func(value), '__decoder': name}
+        )
+        return func
 
-    encode.register(_type)(
-        lambda value: {'__val': func(value), '__decoder': decoder}
-    )
-    return func
+    return wrapper
 
 
 @singledispatch
 def encode(value):
     """Turns a python object into a json object.
 
     Parameters
```

### Comparing `cachetoolz-0.0.1/cachetoolz/decorator.py` & `cachetoolz-0.1.0/cachetoolz/decorator.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.0.1/cachetoolz/log.py` & `cachetoolz-0.1.0/cachetoolz/log.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.0.1/cachetoolz/types.py` & `cachetoolz-0.1.0/cachetoolz/types.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.0.1/cachetoolz/utils.py` & `cachetoolz-0.1.0/cachetoolz/utils.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.0.1/pyproject.toml` & `cachetoolz-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cachetoolz"
-version = "0.0.1"
+version = "0.1.0"
 description = "This library provides a decorator for caching functions"
 license = "MIT"
 authors = ["Igor Taconi <igor.taconi@protonmail.com>"]
 maintainers = ["Igor Taconi <igor.taconi@protonmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/taconi/cachetoolz/#readme"
 repository = "https://github.com/taconi/cachetoolz/"
```

