# Comparing `tmp/cachetoolz-0.1.2.tar.gz` & `tmp/cachetoolz-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachetoolz-0.1.2.tar", max compression
+gzip compressed data, was "cachetoolz-0.1.3.tar", max compression
```

## Comparing `cachetoolz-0.1.2.tar` & `cachetoolz-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1077 2023-07-19 02:08:29.819918 cachetoolz-0.1.2/LICENSE
--rw-r--r--   0        0        0    11147 2023-07-19 02:22:48.443807 cachetoolz-0.1.2/README.md
--rw-r--r--   0        0        0      394 2023-07-19 02:08:29.819918 cachetoolz-0.1.2/cachetoolz/__init__.py
--rw-r--r--   0        0        0      223 2023-07-19 02:08:29.819918 cachetoolz-0.1.2/cachetoolz/abc/__init__.py
--rw-r--r--   0        0        0     2181 2023-07-19 02:08:29.819918 cachetoolz-0.1.2/cachetoolz/abc/backend.py
--rw-r--r--   0        0        0      618 2023-07-19 02:08:29.819918 cachetoolz-0.1.2/cachetoolz/abc/coder.py
--rw-r--r--   0        0        0      623 2023-07-19 02:08:29.819918 cachetoolz-0.1.2/cachetoolz/abc/serializer.py
--rw-r--r--   0        0        0      315 2023-07-19 02:08:29.819918 cachetoolz-0.1.2/cachetoolz/backend/__init__.py
--rw-r--r--   0        0        0     4619 2023-07-19 02:08:29.819918 cachetoolz-0.1.2/cachetoolz/backend/inmemory.py
--rw-r--r--   0        0        0     6595 2023-07-19 02:08:29.819918 cachetoolz-0.1.2/cachetoolz/backend/mongo.py
--rw-r--r--   0        0        0     4212 2023-07-19 02:08:29.819918 cachetoolz-0.1.2/cachetoolz/backend/redis.py
--rw-r--r--   0        0        0     2151 2023-07-19 02:08:29.819918 cachetoolz-0.1.2/cachetoolz/coder/__init__.py
--rw-r--r--   0        0        0     2413 2023-07-19 02:08:29.819918 cachetoolz-0.1.2/cachetoolz/coder/decoder.py
--rw-r--r--   0        0        0     3733 2023-07-19 02:08:29.819918 cachetoolz-0.1.2/cachetoolz/coder/encoder.py
--rw-r--r--   0        0        0     3907 2023-07-19 02:08:29.819918 cachetoolz-0.1.2/cachetoolz/decorator.py
--rw-r--r--   0        0        0      250 2023-07-19 02:08:29.819918 cachetoolz-0.1.2/cachetoolz/exceptions.py
--rw-r--r--   0        0        0      702 2023-07-19 02:08:29.819918 cachetoolz-0.1.2/cachetoolz/log.py
--rw-r--r--   0        0        0      633 2023-07-19 02:08:29.819918 cachetoolz-0.1.2/cachetoolz/types.py
--rw-r--r--   0        0        0     3194 2023-07-19 02:08:29.819918 cachetoolz-0.1.2/cachetoolz/utils.py
--rw-r--r--   0        0        0     3063 2023-07-19 02:24:44.948254 cachetoolz-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    12688 1970-01-01 00:00:00.000000 cachetoolz-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/LICENSE
+-rw-r--r--   0        0        0    11121 2023-07-19 02:27:25.148763 cachetoolz-0.1.3/README.md
+-rw-r--r--   0        0        0      394 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/__init__.py
+-rw-r--r--   0        0        0      223 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/abc/__init__.py
+-rw-r--r--   0        0        0     2181 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/abc/backend.py
+-rw-r--r--   0        0        0      618 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/abc/coder.py
+-rw-r--r--   0        0        0      623 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/abc/serializer.py
+-rw-r--r--   0        0        0      315 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/backend/__init__.py
+-rw-r--r--   0        0        0     4619 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/backend/inmemory.py
+-rw-r--r--   0        0        0     6595 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/backend/mongo.py
+-rw-r--r--   0        0        0     4212 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/backend/redis.py
+-rw-r--r--   0        0        0     2151 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/coder/__init__.py
+-rw-r--r--   0        0        0     2413 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/coder/decoder.py
+-rw-r--r--   0        0        0     3733 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/coder/encoder.py
+-rw-r--r--   0        0        0     3907 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/decorator.py
+-rw-r--r--   0        0        0      250 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/exceptions.py
+-rw-r--r--   0        0        0      702 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/log.py
+-rw-r--r--   0        0        0      633 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/types.py
+-rw-r--r--   0        0        0     3194 2023-07-19 02:08:29.819918 cachetoolz-0.1.3/cachetoolz/utils.py
+-rw-r--r--   0        0        0     3063 2023-07-19 02:27:34.736790 cachetoolz-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    12662 1970-01-01 00:00:00.000000 cachetoolz-0.1.3/PKG-INFO
```

### Comparing `cachetoolz-0.1.2/LICENSE` & `cachetoolz-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.2/README.md` & `cachetoolz-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,18 +53,16 @@
 You can specify these in your requirements or on the pip command-line by using brackets. Multiple bundles can be specified by separating them by commas.
 ```bash
 pip install cachetoolz[redis]
 pip install cachetoolz[redis,mongo]
 ```
 
 The following bundles are available:
-Transports and Backends
 
-
-#### Backends 
+#### Backends
 * `cachetoolz[redis]`: for using Redis as a backend.
 * `cachetoolz[mongo]`: for using Mongo as a backend.
 
 # How to use
 ```python
 from asyncio import Lock
 from dataclasses import asdict, dataclass, field
```

### Comparing `cachetoolz-0.1.2/cachetoolz/abc/backend.py` & `cachetoolz-0.1.3/cachetoolz/abc/backend.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.2/cachetoolz/abc/coder.py` & `cachetoolz-0.1.3/cachetoolz/abc/coder.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.2/cachetoolz/abc/serializer.py` & `cachetoolz-0.1.3/cachetoolz/abc/serializer.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.2/cachetoolz/backend/inmemory.py` & `cachetoolz-0.1.3/cachetoolz/backend/inmemory.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.2/cachetoolz/backend/mongo.py` & `cachetoolz-0.1.3/cachetoolz/backend/mongo.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.2/cachetoolz/backend/redis.py` & `cachetoolz-0.1.3/cachetoolz/backend/redis.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.2/cachetoolz/coder/__init__.py` & `cachetoolz-0.1.3/cachetoolz/coder/__init__.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.2/cachetoolz/coder/decoder.py` & `cachetoolz-0.1.3/cachetoolz/coder/decoder.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.2/cachetoolz/coder/encoder.py` & `cachetoolz-0.1.3/cachetoolz/coder/encoder.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.2/cachetoolz/decorator.py` & `cachetoolz-0.1.3/cachetoolz/decorator.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.2/cachetoolz/log.py` & `cachetoolz-0.1.3/cachetoolz/log.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.2/cachetoolz/types.py` & `cachetoolz-0.1.3/cachetoolz/types.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.2/cachetoolz/utils.py` & `cachetoolz-0.1.3/cachetoolz/utils.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.1.2/pyproject.toml` & `cachetoolz-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cachetoolz"
-version = "0.1.2"
+version = "0.1.3"
 description = "This library provides a decorator for caching functions"
 license = "MIT"
 authors = ["Igor Taconi <igor.taconi@protonmail.com>"]
 maintainers = ["Igor Taconi <igor.taconi@protonmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/taconi/cachetoolz/#readme"
 repository = "https://github.com/taconi/cachetoolz/"
```

### Comparing `cachetoolz-0.1.2/PKG-INFO` & `cachetoolz-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachetoolz
-Version: 0.1.2
+Version: 0.1.3
 Summary: This library provides a decorator for caching functions
 Home-page: https://github.com/taconi/cachetoolz/#readme
 License: MIT
 Keywords: python,cache,async,redis,mongo
 Author: Igor Taconi
 Author-email: igor.taconi@protonmail.com
 Maintainer: Igor Taconi
@@ -90,18 +90,16 @@
 You can specify these in your requirements or on the pip command-line by using brackets. Multiple bundles can be specified by separating them by commas.
 ```bash
 pip install cachetoolz[redis]
 pip install cachetoolz[redis,mongo]
 ```
 
 The following bundles are available:
-Transports and Backends
 
-
-#### Backends 
+#### Backends
 * `cachetoolz[redis]`: for using Redis as a backend.
 * `cachetoolz[mongo]`: for using Mongo as a backend.
 
 # How to use
 ```python
 from asyncio import Lock
 from dataclasses import asdict, dataclass, field
```

