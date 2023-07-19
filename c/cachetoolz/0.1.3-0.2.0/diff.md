# Comparing `tmp/cachetoolz-0.1.3.tar.gz` & `tmp/cachetoolz-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachetoolz-0.1.3.tar", max compression
+gzip compressed data, was "cachetoolz-0.2.0.tar", max compression
```

## Comparing `cachetoolz-0.1.3.tar` & `cachetoolz-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1077 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/LICENSE
--rw-r--r--   0        0        0    11121 2023-07-19 02:27:25.148763 cachetoolz-0.1.3/README.md
--rw-r--r--   0        0        0      394 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/__init__.py
--rw-r--r--   0        0        0      223 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/abc/__init__.py
--rw-r--r--   0        0        0     2181 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/abc/backend.py
--rw-r--r--   0        0        0      618 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/abc/coder.py
--rw-r--r--   0        0        0      623 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/abc/serializer.py
--rw-r--r--   0        0        0      315 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/backend/__init__.py
--rw-r--r--   0        0        0     4619 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/backend/inmemory.py
--rw-r--r--   0        0        0     6595 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/backend/mongo.py
--rw-r--r--   0        0        0     4212 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/backend/redis.py
--rw-r--r--   0        0        0     2151 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/coder/__init__.py
--rw-r--r--   0        0        0     2413 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/coder/decoder.py
--rw-r--r--   0        0        0     3733 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/coder/encoder.py
--rw-r--r--   0        0        0     3907 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/decorator.py
--rw-r--r--   0        0        0      250 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/exceptions.py
--rw-r--r--   0        0        0      702 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/log.py
--rw-r--r--   0        0        0      633 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/types.py
--rw-r--r--   0        0        0     3194 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/utils.py
--rw-r--r--   0        0        0     3063 2023-07-19 02:27:34.736790 cachetoolz-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    12662 1970-01-01 00:00:00.000000 cachetoolz-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/LICENSE
+-rw-r--r--   0        0        0    11097 2023-07-19 13:12:21.864253 cachetoolz-0.2.0/README.md
+-rw-r--r--   0        0        0      394 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/__init__.py
+-rw-r--r--   0        0        0      223 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/abc/__init__.py
+-rw-r--r--   0        0        0     2181 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/abc/backend.py
+-rw-r--r--   0        0        0      618 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/abc/coder.py
+-rw-r--r--   0        0        0      623 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/abc/serializer.py
+-rw-r--r--   0        0        0      315 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/backend/__init__.py
+-rw-r--r--   0        0        0     4619 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/backend/inmemory.py
+-rw-r--r--   0        0        0     6595 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/backend/mongo.py
+-rw-r--r--   0        0        0     4212 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/backend/redis.py
+-rw-r--r--   0        0        0     2151 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/coder/__init__.py
+-rw-r--r--   0        0        0     2413 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/coder/decoder.py
+-rw-r--r--   0        0        0     3733 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/coder/encoder.py
+-rw-r--r--   0        0        0     4260 2023-07-19 13:28:48.375536 cachetoolz-0.2.0/cachetoolz/decorator.py
+-rw-r--r--   0        0        0      250 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/exceptions.py
+-rw-r--r--   0        0        0      702 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/log.py
+-rw-r--r--   0        0        0      633 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/types.py
+-rw-r--r--   0        0        0     3194 2023-07-19 13:24:39.070373 cachetoolz-0.2.0/cachetoolz/utils.py
+-rw-r--r--   0        0        0     3063 2023-07-19 13:46:29.211552 cachetoolz-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    12638 1970-01-01 00:00:00.000000 cachetoolz-0.2.0/PKG-INFO
```

### Comparing `cachetoolz-0.1.3/LICENSE` & `cachetoolz-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.3/README.md` & `cachetoolz-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 Overall, this library simplifies the implementation of caching in your applications, allowing you to enhance performance and reduce resource consumption effectively.
 
 ---
 # Summary
 * **[Installation](#installation)**
   * **[Bundles](#bundles)**
-* **[How to use](#how-to-use)**
+* **[Quickstart](#quickstart)**
   * **[Cache parameters](#cache-parameters)**
     * **[Key generator](#key-generator)**
   * **[Cache clear](#cache-clear)**
   * **[Backends](#backends)**
     * **[In Memory](#in-memory)**
     * **[Remote Backends](#remote-backends)**
         * **[Redis](#redis)**
@@ -58,15 +58,15 @@
 
 The following bundles are available:
 
 #### Backends
 * `cachetoolz[redis]`: for using Redis as a backend.
 * `cachetoolz[mongo]`: for using Mongo as a backend.
 
-# How to use
+# Quickstart
 ```python
 from asyncio import Lock
 from dataclasses import asdict, dataclass, field
 from uuid import UUID, uui4
 
 from cachetoolz import AsyncRedisBackend, Cache
 from cachetoolz.coder import coder
@@ -117,19 +117,19 @@
     async with lock:
         if todo not in TODOS:
             TODOS.append(todo)
 ```
 
 ## Cache parameters
 The decorator may have configured it with some parameters.
-All parameters except `expire` need to be passed namely.
+All parameters need to be passed namely.
 
 | Parameter   | Description | Type | Default |
 | ----------- | ----------- | ---- | ------- |
-| `expire`    | cache expiration time in seconds | `int`, `float`, `timedelta` | `math.inf` |
+| `ttl`       | cache ttl (time to live) | `int`, `float`, `timedelta` | `math.inf` |
 | `namespace` | namespace to cache | `str` | `"default"` |
 | `typed`     | If typed is set to true, function arguments of different types will be cached separately | `bool` | `False` |
 | `keygen`    | function to generate a cache identifier key | `cachetoolz.types.KeyGenerator` | `cachetoolz.utils.default_keygen` |
 
 ### Key generator
 This must be the signature of a key generator function
 ```python
```

### Comparing `cachetoolz-0.1.3/cachetoolz/abc/backend.py` & `cachetoolz-0.2.0/cachetoolz/abc/backend.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.3/cachetoolz/abc/coder.py` & `cachetoolz-0.2.0/cachetoolz/abc/coder.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.3/cachetoolz/abc/serializer.py` & `cachetoolz-0.2.0/cachetoolz/abc/serializer.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.3/cachetoolz/backend/inmemory.py` & `cachetoolz-0.2.0/cachetoolz/backend/inmemory.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.3/cachetoolz/backend/mongo.py` & `cachetoolz-0.2.0/cachetoolz/backend/mongo.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.3/cachetoolz/backend/redis.py` & `cachetoolz-0.2.0/cachetoolz/backend/redis.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.3/cachetoolz/coder/__init__.py` & `cachetoolz-0.2.0/cachetoolz/coder/__init__.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.3/cachetoolz/coder/decoder.py` & `cachetoolz-0.2.0/cachetoolz/coder/decoder.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.3/cachetoolz/coder/encoder.py` & `cachetoolz-0.2.0/cachetoolz/coder/encoder.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.3/cachetoolz/decorator.py` & `cachetoolz-0.2.0/cachetoolz/decorator.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,45 +13,48 @@
 from .types import Decorator, Func, KeyGenerator, P, T
 from .utils import ensure_async, make_key, manipulate
 
 
 class Cache:
     """Caches a function call and stores it in the namespace.
 
+    Bare decorator, ``@cache``, is supported as well as a call with
+    keyword arguments ``@cache(ttl=7200)``.
+
     Parameters
     ----------
-    expire
-        cache expiration time in seconds
+    ttl
+        cache ttl (time to live)
     namespace
         namespace to cache
     typed
         If typed is set to true, function arguments of different types
         will be cached separately
     keygen
         function to generate a cache identifier key
 
     Examples
     --------
-    >>> @cache()
+    >>> @cache
     ... def foo(_id):
     ...     ...
     ...
 
     >>> @cache(namespace='bar')  # specific a namespace
     ... def bar(filters):
     ...     ...
     ...
 
-    >>> @cache(60)  # set an expiration time in seconds
+    >>> @cache(ttl=60)  # set an expiration time in seconds
     ... def foo_bar(filters):
     ...     ...
     ...
 
     >>> from datetime import timedelta
-    >>> @cache(timedelta(days=1))  # Use timedelta to set the expiration
+    >>> @cache(ttl=timedelta(days=1))  # Use timedelta to set the expiration
     ... def foobar(filters):
     ...     ...
     ...
 
     """
 
     def __init__(self, backend: Union[AsyncBackendABC, BackendABC]):
@@ -64,53 +67,59 @@
 
         """
         self.backend = backend
         self._logger = get_logger()
 
     async def _cache(
         self,
-        expire: timedelta,
+        ttl: timedelta,
         keygen: KeyGenerator,
         func: Func,
         *args: P.args,
         **kwargs: P.kwargs,
     ) -> T:
         key = await keygen(func, *args, **kwargs)
 
         if (result := await ensure_async(self.backend.get, key)) is not None:
             return coder.decode(result)
 
         result = coder.encode(await ensure_async(func, *args, **kwargs))
 
         try:
-            await ensure_async(self.backend.set, key, result, expire)
+            await ensure_async(self.backend.set, key, result, ttl)
         except Exception as exception:
             self._logger.error(
                 "Error to set cache 'key=%s': exception=%s", key, exception
             )
 
         return coder.decode(result)
 
     def __call__(
         self,
-        expire: Union[int, float, timedelta] = inf,
-        *,
+        *args,
+        ttl: Union[int, float, timedelta] = inf,
         namespace: str = 'default',
         typed: bool = False,
         keygen: Optional[KeyGenerator] = None,
     ) -> Decorator:
         """Caches a function call and stores it in the namespace."""
-        if isinf(expire):
-            expire = timedelta(weeks=20e3)
-        elif not isinstance(expire, timedelta):
-            expire = timedelta(seconds=expire)
+
+        if isinf(ttl):
+            ttl = timedelta(weeks=20e3)
+        elif not isinstance(ttl, timedelta):
+            ttl = timedelta(seconds=ttl)
 
         keygen = curry(make_key)(namespace, keygen, typed)
-        _cache = curry(Cache._cache)(self, expire, keygen)
-        return manipulate(_cache)
+        manipulator = manipulate(curry(Cache._cache)(self, ttl, keygen))
+
+        if args:
+            # @cache
+            return manipulator(args[0])
+        # @cache()
+        return manipulator
 
     async def _clear(
         self,
         namespaces: Sequence[str],
         func: Func,
         *args: P.args,
         **kwargs: P.kwargs,
@@ -125,24 +134,31 @@
                 namespaces,
                 exception,
             )
 
         result = coder.encode(await ensure_async(func, *args, **kwargs))
         return coder.decode(result)
 
-    def clear(self, namespaces: Sequence[str] = ('default',)) -> Decorator:
+    def clear(
+        self, *args, namespaces: Sequence[str] = ('default',)
+    ) -> Decorator:
         """Clears all caches for all namespaces.
 
         Parameters
         ----------
         namespaces
             namespace to be cleaned.
 
         Examples
         --------
         >>> @cache.clear(namespaces=['book'])
         ... def create_book(book):
         ...     ...
 
         """
-        _clear = curry(Cache._clear)(self, namespaces)
-        return manipulate(_clear)
+        manipulator = manipulate(curry(Cache._clear)(self, namespaces))
+
+        if args:
+            # @cache.clear
+            return manipulator(args[0])
+        # @cache.clear(namespaces=['ns1'])
+        return manipulator
```

### Comparing `cachetoolz-0.1.3/cachetoolz/log.py` & `cachetoolz-0.2.0/cachetoolz/log.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.3/cachetoolz/types.py` & `cachetoolz-0.2.0/cachetoolz/types.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.3/cachetoolz/utils.py` & `cachetoolz-0.2.0/cachetoolz/utils.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.3/pyproject.toml` & `cachetoolz-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cachetoolz"
-version = "0.1.3"
+version = "0.2.0"
 description = "This library provides a decorator for caching functions"
 license = "MIT"
 authors = ["Igor Taconi <igor.taconi@protonmail.com>"]
 maintainers = ["Igor Taconi <igor.taconi@protonmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/taconi/cachetoolz/#readme"
 repository = "https://github.com/taconi/cachetoolz/"
```

### Comparing `cachetoolz-0.1.3/PKG-INFO` & `cachetoolz-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachetoolz
-Version: 0.1.3
+Version: 0.2.0
 Summary: This library provides a decorator for caching functions
 Home-page: https://github.com/taconi/cachetoolz/#readme
 License: MIT
 Keywords: python,cache,async,redis,mongo
 Author: Igor Taconi
 Author-email: igor.taconi@protonmail.com
 Maintainer: Igor Taconi
@@ -56,15 +56,15 @@
 
 Overall, this library simplifies the implementation of caching in your applications, allowing you to enhance performance and reduce resource consumption effectively.
 
 ---
 # Summary
 * **[Installation](#installation)**
   * **[Bundles](#bundles)**
-* **[How to use](#how-to-use)**
+* **[Quickstart](#quickstart)**
   * **[Cache parameters](#cache-parameters)**
     * **[Key generator](#key-generator)**
   * **[Cache clear](#cache-clear)**
   * **[Backends](#backends)**
     * **[In Memory](#in-memory)**
     * **[Remote Backends](#remote-backends)**
         * **[Redis](#redis)**
@@ -95,15 +95,15 @@
 
 The following bundles are available:
 
 #### Backends
 * `cachetoolz[redis]`: for using Redis as a backend.
 * `cachetoolz[mongo]`: for using Mongo as a backend.
 
-# How to use
+# Quickstart
 ```python
 from asyncio import Lock
 from dataclasses import asdict, dataclass, field
 from uuid import UUID, uui4
 
 from cachetoolz import AsyncRedisBackend, Cache
 from cachetoolz.coder import coder
@@ -154,19 +154,19 @@
     async with lock:
         if todo not in TODOS:
             TODOS.append(todo)
 ```
 
 ## Cache parameters
 The decorator may have configured it with some parameters.
-All parameters except `expire` need to be passed namely.
+All parameters need to be passed namely.
 
 | Parameter   | Description | Type | Default |
 | ----------- | ----------- | ---- | ------- |
-| `expire`    | cache expiration time in seconds | `int`, `float`, `timedelta` | `math.inf` |
+| `ttl`       | cache ttl (time to live) | `int`, `float`, `timedelta` | `math.inf` |
 | `namespace` | namespace to cache | `str` | `"default"` |
 | `typed`     | If typed is set to true, function arguments of different types will be cached separately | `bool` | `False` |
 | `keygen`    | function to generate a cache identifier key | `cachetoolz.types.KeyGenerator` | `cachetoolz.utils.default_keygen` |
 
 ### Key generator
 This must be the signature of a key generator function
 ```python
```

