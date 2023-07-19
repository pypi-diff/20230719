# Comparing `tmp/pykebab-0.7.12.tar.gz` & `tmp/pykebab-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykebab-0.7.12.tar", max compression
+gzip compressed data, was "pykebab-0.7.8.tar", max compression
```

## Comparing `pykebab-0.7.12.tar` & `pykebab-0.7.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      821 2022-11-06 03:32:21.214628 pykebab-0.7.12/kebab/__init__.py
--rw-r--r--   0        0        0     3920 2022-11-06 03:32:21.214802 pykebab-0.7.12/kebab/aws.py
--rw-r--r--   0        0        0       40 2022-11-06 03:32:21.214897 pykebab-0.7.12/kebab/cli/__init__.py
--rw-r--r--   0        0        0     1801 2023-01-05 03:45:44.147407 pykebab-0.7.12/kebab/cli/cli.py
--rw-r--r--   0        0        0      902 2023-07-17 05:23:30.671130 pykebab-0.7.12/kebab/constants.py
--rw-r--r--   0        0        0       42 2022-11-06 03:32:21.215088 pykebab-0.7.12/kebab/exceptions.py
--rw-r--r--   0        0        0     2586 2023-07-15 08:49:23.404276 pykebab-0.7.12/kebab/k8s.py
--rw-r--r--   0        0        0      744 2023-07-17 05:24:19.989267 pykebab-0.7.12/kebab/loaders.py
--rw-r--r--   0        0        0     2368 2023-06-26 02:47:04.851901 pykebab-0.7.12/kebab/magic.py
--rw-r--r--   0        0        0     1575 2023-07-15 08:49:38.763057 pykebab-0.7.12/kebab/openers.py
--rw-r--r--   0        0        0    22604 2023-07-18 08:40:12.186718 pykebab-0.7.12/kebab/sources.py
--rw-r--r--   0        0        0     4825 2023-01-05 03:45:44.148106 pykebab-0.7.12/kebab/utils.py
--rw-r--r--   0        0        0     1066 2023-07-18 12:20:01.784990 pykebab-0.7.12/pyproject.toml
--rw-r--r--   0        0        0      924 1970-01-01 00:00:00.000000 pykebab-0.7.12/PKG-INFO
+-rw-r--r--   0        0        0      821 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/__init__.py
+-rw-r--r--   0        0        0     3920 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/aws.py
+-rw-r--r--   0        0        0       40 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/cli/__init__.py
+-rw-r--r--   0        0        0     1801 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/cli/cli.py
+-rw-r--r--   0        0        0      798 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/constants.py
+-rw-r--r--   0        0        0       42 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/exceptions.py
+-rw-r--r--   0        0        0     2587 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/k8s.py
+-rw-r--r--   0        0        0      773 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/loader.py
+-rw-r--r--   0        0        0     2368 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/magic.py
+-rw-r--r--   0        0        0     2108 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/openers.py
+-rw-r--r--   0        0        0    22564 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/sources.py
+-rw-r--r--   0        0        0     4825 2023-06-26 04:27:04.825862 pykebab-0.7.8/kebab/utils.py
+-rw-r--r--   0        0        0     1025 2023-06-26 04:27:04.825862 pykebab-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 pykebab-0.7.8/PKG-INFO
```

### Comparing `pykebab-0.7.12/kebab/__init__.py` & `pykebab-0.7.8/kebab/__init__.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.12/kebab/aws.py` & `pykebab-0.7.8/kebab/aws.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.12/kebab/cli/cli.py` & `pykebab-0.7.8/kebab/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.12/kebab/k8s.py` & `pykebab-0.7.8/kebab/k8s.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         return self._api
 
     def __init__(self):
         self._lock = threading.Lock()
         self._api = None
 
     def k8s_open(self, req):
+
         url = req.get_full_url()
         pu = _ParsedUrl(url)
 
         if pu.resource_type in ["secret", "secrets"]:
             stream = self._read_secret(pu)
         elif pu.resource_type in ["cm", "configmap", "configmaps"]:
             stream = self._read_configmap(pu)
```

### Comparing `pykebab-0.7.12/kebab/loaders.py` & `pykebab-0.7.8/kebab/loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # coding=utf-8
 import abc
 from configparser import ConfigParser
-
 # from typing import List, Dict
 
 import yaml
 
+
 # Context = Dict[str, 'Context'] | List['Context'] | str | int | float | bool | None
 
 
+# noinspection PyUnusedLocal
 class StrLoader(object):
     @abc.abstractmethod
     def load(self, content: str):
         return {}
 
 
 class YamlLoader(StrLoader):
```

### Comparing `pykebab-0.7.12/kebab/magic.py` & `pykebab-0.7.8/kebab/magic.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.12/kebab/openers.py` & `pykebab-0.7.8/kebab/openers.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,20 +7,40 @@
     BaseHandler,
     FileHandler,
     HTTPHandler,
     HTTPSHandler,
 )
 from urllib.response import addinfourl
 
+import pkg_resources
+
 
 class _FileLikeKey(BufferedIOBase):
     def __init__(self, key):
         self.read = key.read
 
 
+class ResourceHandler(BaseHandler):
+    def __init__(self):
+        pass
+
+    # noinspection PyMethodMayBeStatic
+    def resource_open(self, req):
+        try:
+            selector = req.selector
+        except AttributeError:
+            selector = req.get_selector()
+        resource_name = selector.lstrip("/")
+        pkg_name = req.host
+
+        stream = pkg_resources.resource_stream(pkg_name, resource_name)
+
+        return addinfourl(_FileLikeKey(stream), [], req.get_full_url())
+
+
 class PythonPathHandler(BaseHandler):
     """
     a filename with relative path to the pythonpath
     """
 
     def __init__(self):
         pass
@@ -41,14 +61,15 @@
 
 
 handlers = [
     FileHandler,
     HTTPHandler,
     HTTPSHandler,
     PythonPathHandler,
+    ResourceHandler,
 ]
 
 try:
     # noinspection PyUnresolvedReferences
     from . import k8s
 
     handlers.append(k8s.K8SHandler)
```

### Comparing `pykebab-0.7.12/kebab/sources.py` & `pykebab-0.7.8/kebab/sources.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,20 +6,19 @@
 import queue  # using python-future for 2/3 compatibility
 import threading
 import time
 from typing import Any, List, Dict, get_type_hints, Type, TypeVar, Callable
 from urllib.request import OpenerDirector
 
 import deprecation
-
 # noinspection PyPackageRequirements
 from pydantic import BaseModel
 
 from kebab.constants import DEFAULT_URL_ENVVAR, DISABLE_RELOAD
-from kebab.loaders import YamlLoader, StrLoader
+from kebab.loader import YamlLoader, StrLoader
 from kebab.openers import DEFAULT_OPENER
 from kebab.utils import (
     update_recursively,
     lookup_recursively,
     fill_recursively,
     deprecated_alias,
 )
@@ -46,30 +45,29 @@
     def register_extension(cls, extension):
         if issubclass(extension, ContextExtension):
             extension = extension()
         if isinstance(extension, ContextExtension):
             KebabSource._context_extensions[extension.keyword] = extension
 
     @property
-    def str_loader(
-        self,
-    ) -> StrLoader:
+    def str_loader(self, ) -> StrLoader:
         return self._str_loader
 
     @str_loader.setter
     def str_loader(self, loader):
         self._str_loader = loader
 
     def __init__(self, **kwargs):
         # Variables for sources reload (first load is also a reload).
         super(KebabSource, self).__init__(**kwargs)
         self._last_reload_timestamp = 0  # type: float
         self._reload_lock = threading.RLock()
         self._reload_timer = None
         self._reload_disabled = threading.Event()
+        self._last_cached_timestamp = 0  # type: float
         self._cached_context = {}
         self._str_loader = YamlLoader()
 
     def __repr__(self):
         return self.__class__.__name__
 
     def __getitem__(self, key):
@@ -97,25 +95,17 @@
         return item in self.get()
 
     def __iter__(self):
         return iter(self.get())
 
     @abc.abstractmethod
     def _load_context(self):
-        """
-        Load the context from the source.
-        This method should be implemented by subclasses.
-        """
         return {}
 
     def _load_context_recursively(self):
-        """
-        Load the context from the source and recursively update the context from
-        the extensions.
-        """
         _logger.debug(f"loading {self}")
 
         _context = self._load_context()
 
         for keyword, extension in KebabSource._context_extensions.items():
             if keyword in _context:
                 extension_context = _context.pop(keyword)
@@ -182,57 +172,66 @@
                 )
                 self._reload_timer.daemon = True
                 self._reload_timer.start()
 
         return self
 
     def _get_context(self):
-        if not self._cached_context:
+        if (
+            not self._cached_context
+            or self._last_cached_timestamp < self.last_reload_timestamp
+        ):
             self.reload()
+            self._last_cached_timestamp = time.time()
 
         return self._cached_context
 
     @property
     def last_reload_timestamp(self):
         return self._last_reload_timestamp
 
-    T = TypeVar("T")
+    T = TypeVar('T')
 
     # noinspection PyMethodParameters
     def proxy(source, f: Callable[[], T], expected_type: Type[T]) -> T:
-        if expected_type in (int, str, float, bool, list, tuple, dict, set, type(None)):
+        if expected_type in (
+            int, str, float, bool, list, tuple, dict, set, type(None)
+        ):
             return f()
 
         # not thread safe
         class KebabProxy:
             def __init__(self):
                 self.__value = f()
                 self.__last_eval_timestamp = time.time()
 
-            def _reload_getattr(self, name):
+            def reload_if_necessary(self):
                 if self.__last_eval_timestamp < source.last_reload_timestamp:
                     self.__value = f()
                     self.__last_eval_timestamp = time.time()
-                return getattr(self.__value, name)
 
             def __getattr__(self, name):
-                ret = self._reload_getattr(name)
-                return source.proxy(lambda: self._reload_getattr(name), type(ret))
+                self.reload_if_necessary()
+                ret = getattr(self.__value, name)
 
+                def reloader():
+                    self.reload_if_necessary()
+                    return getattr(self.__value, name)
+                return source.proxy(reloader, type(ret))
         return KebabProxy()
 
     @deprecated_alias(default_value="default")
     def get(
         self,
         config_name=".",
         default=None,
         required=False,
         expected_type=None,
         masked=False,
-        update_after_reload=False,
+        update_after_reload=False
     ):
         """
         :param str config_name: The key to retrieve the config value. If '.', return the
                         whole context
         :param object default: The default value to fall back to if config_name not
                         found
         :param bool required: When the required value is not found, throw exception if
@@ -265,18 +264,21 @@
         Note that the type of the default becomes the expected_type if presents,
         the original expected_type will be ignored in that case.
 
         The parameter `default_value` is deprecated, use `default` instead
         """
         if update_after_reload:
             # noinspection PyTypeChecker
-            return self.proxy(
-                lambda: self.get(config_name, default, required, expected_type, masked),
-                expected_type=expected_type,
-            )
+            return self.proxy(lambda: self.get(
+                config_name,
+                default,
+                required,
+                expected_type,
+                masked
+            ), expected_type=expected_type)
 
         if default is not None:
             # set expected type based on default value (and ignore the original
             # expected_type
             if expected_type is not None and not isinstance(default, expected_type):
                 raise ValueError(
                     "You specified default of type {}, but expected_type={}".format(
@@ -360,22 +362,20 @@
                 else:
                     return expected_type(config_value)
         return config_value
 
     @staticmethod
     def _to_dataclass(data_class_type: Type[T], data: Dict[str, Any]) -> T:
         field_types = get_type_hints(data_class_type)
-        return data_class_type(
-            **{
-                field: KebabSource._to_dataclass(field_types[field], data[field])
-                if dataclasses.is_dataclass(field_types[field])
-                else data[field]
-                for field in data
-            }
-        )
+        return data_class_type(**{
+            field: KebabSource._to_dataclass(field_types[field], data[field])
+            if dataclasses.is_dataclass(field_types[field])
+            else data[field]
+            for field in data
+        })
 
     def subsource(self, config_name):
         """
         Caveats:
 
         When parent KebabSource reloads, SubSource is not effected the updated values in
             KebabSource.
@@ -590,17 +590,14 @@
 
     def _load_context(self):
         return self._parent_source.get(
             self._source_name, required=True, expected_type=dict
         )
 
     def _get_context(self):
-        """
-        SubSource never caches, relies on parent source/cache
-        """
         return self._load_context()
 
     @property
     def last_reload_timestamp(self):
         return self._parent_source.last_reload_timestamp
 
 
@@ -664,14 +661,14 @@
 
     if len(sources) == 1:
         # for single url, do not read with union source so that self configured auto
         # reload will work
         source = sources[0]
     else:
         source = UnionSource(sources=sources)
-    source.reload(reload_interval_in_secs=reload_interval_in_secs, skip_first=True)
+    source.reload(reload_interval_in_secs=reload_interval_in_secs)
     return source
 
 
 KebabSource.register_extension(ImportExtension)
 KebabSource.register_extension(EnvVarSource)
 KebabSource.register_extension(ReloadExtension)
```

### Comparing `pykebab-0.7.12/kebab/utils.py` & `pykebab-0.7.8/kebab/utils.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.7.12/PKG-INFO` & `pykebab-0.7.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: pykebab
-Version: 0.7.12
+Version: 0.7.8
 Summary: 
 Author: Yangming Huang
 Author-email: leonmax@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: aws
 Provides-Extra: cli
 Provides-Extra: k8s
-Requires-Dist: boto3 (>=1.28.3,<2.0.0) ; extra == "aws"
-Requires-Dist: click (>=8.1.5,<9.0.0) ; extra == "cli"
+Requires-Dist: boto3 (>=1.26.99,<2.0.0) ; extra == "aws"
+Requires-Dist: click (>=8.1.3,<9.0.0) ; extra == "cli"
 Requires-Dist: configparser (>=5.3.0,<6.0.0)
 Requires-Dist: deprecation (>=2.1.0,<3.0.0)
 Requires-Dist: kubernetes (>=26.1.0,<27.0.0) ; extra == "k8s"
-Requires-Dist: pydantic (>=2.0.3,<3.0.0)
-Requires-Dist: pyxdg (>=0.28,<0.29)
+Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: setuptools (>=68.0.0,<69.0.0)
+Requires-Dist: setuptools (>=67.6.0,<68.0.0)
```

