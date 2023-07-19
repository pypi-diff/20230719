# Comparing `tmp/types-mock-5.0.0.7.tar.gz` & `tmp/types-mock-5.1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-mock-5.0.0.7.tar", last modified: Wed Jun 21 01:22:55 2023, max compression
+gzip compressed data, was "types-mock-5.1.0.0.tar", last modified: Wed Jul 19 12:29:46 2023, max compression
```

## Comparing `types-mock-5.0.0.7.tar` & `types-mock-5.1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:22:55.282034 types-mock-5.0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-21 01:22:53.000000 types-mock-5.0.0.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 01:22:53.000000 types-mock-5.0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-21 01:22:55.282034 types-mock-5.0.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:22:55.282034 types-mock-5.0.0.7/mock-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 01:22:53.000000 types-mock-5.0.0.7/mock-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-21 01:22:41.000000 types-mock-5.0.0.7/mock-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-21 01:22:41.000000 types-mock-5.0.0.7/mock-stubs/backports.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-06-21 01:22:41.000000 types-mock-5.0.0.7/mock-stubs/mock.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 01:22:55.282034 types-mock-5.0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-21 01:22:53.000000 types-mock-5.0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:22:55.282034 types-mock-5.0.0.7/types_mock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-21 01:22:55.000000 types-mock-5.0.0.7/types_mock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-21 01:22:55.000000 types-mock-5.0.0.7/types_mock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 01:22:55.000000 types-mock-5.0.0.7/types_mock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 01:22:55.000000 types-mock-5.0.0.7/types_mock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:29:46.791357 types-mock-5.1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-19 12:29:46.000000 types-mock-5.1.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 12:29:46.000000 types-mock-5.1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-19 12:29:46.791357 types-mock-5.1.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:29:46.787357 types-mock-5.1.0.0/mock-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-19 12:29:46.000000 types-mock-5.1.0.0/mock-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-19 12:29:24.000000 types-mock-5.1.0.0/mock-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-19 12:29:24.000000 types-mock-5.1.0.0/mock-stubs/backports.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13541 2023-07-19 12:29:24.000000 types-mock-5.1.0.0/mock-stubs/mock.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 12:29:46.791357 types-mock-5.1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-19 12:29:46.000000 types-mock-5.1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:29:46.791357 types-mock-5.1.0.0/types_mock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-19 12:29:46.000000 types-mock-5.1.0.0/types_mock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-19 12:29:46.000000 types-mock-5.1.0.0/types_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:29:46.000000 types-mock-5.1.0.0/types_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-19 12:29:46.000000 types-mock-5.1.0.0/types_mock.egg-info/top_level.txt
```

### Comparing `types-mock-5.0.0.7/CHANGELOG.md` & `types-mock-5.1.0.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 5.1.0.0 (2023-07-19)
+
+Add a more precise signature for `AsyncMock.reset_mock()` (#10481)
+
+Update `mock` to `5.1.*` (#10472)
+
 ## 5.0.0.7 (2023-06-21)
 
 [mock] take an iterable of calls for assert_has_awaits(#10337)
 
 use ParamSpec in patch in mock stubs (#10338)
 
 ## 5.0.0.6 (2023-03-27)
```

### Comparing `types-mock-5.0.0.7/PKG-INFO` & `types-mock-5.1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-mock
-Version: 5.0.0.7
+Version: 5.1.0.0
 Summary: Typing stubs for mock
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/mock.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,10 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `mock`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/mock. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a46fe434772d105c1f8204565b2b8636c5bb108b` and was tested
-with mypy 1.3.0, pyright 1.1.314, and
-pytype 2023.6.2.
+This package was generated from typeshed commit `032f9195f9e3788a6e5c7ecb086f173a3ac92a95` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-mock-5.0.0.7/mock-stubs/mock.pyi` & `types-mock-5.1.0.0/mock-stubs/mock.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from _typeshed import Incomplete
 from collections.abc import Callable, Coroutine, Iterable, Mapping, Sequence
 from contextlib import AbstractContextManager
 from types import TracebackType
-from typing import Any, Generic, TypeVar, overload
+from typing import Any, ClassVar, Generic, TypeVar, overload
 from typing_extensions import Literal, ParamSpec, Self
 
 _F = TypeVar("_F", bound=Callable[..., Any])
 _AF = TypeVar("_AF", bound=Callable[..., Coroutine[Any, Any, Any]])
 _T = TypeVar("_T")
 _TT = TypeVar("_TT", bound=type[Any])
 _R = TypeVar("_R")
@@ -18,14 +18,15 @@
     "patch",
     "sentinel",
     "DEFAULT",
     "ANY",
     "call",
     "create_autospec",
     "AsyncMock",
+    "ThreadingMock",
     "FILTER_DIR",
     "NonCallableMock",
     "NonCallableMagicMock",
     "mock_open",
     "PropertyMock",
     "seal",
 )
@@ -324,15 +325,20 @@
     await_args_list: _CallList
     __name__: str
     __defaults__: tuple[Any, ...]
     __kwdefaults__: dict[str, Any]
     __annotations__: dict[str, Any] | None  # type: ignore[assignment]
 
 class AsyncMagicMixin(MagicMixin): ...
-class AsyncMock(AsyncMockMixin, AsyncMagicMixin, Mock): ...
+
+class AsyncMock(AsyncMockMixin, AsyncMagicMixin, Mock):
+    # Improving the `reset_mock` signature.
+    # It is defined on `AsyncMockMixin` with `*args, **kwargs`, which is not ideal.
+    # But, `NonCallableMock` super-class has the better version.
+    def reset_mock(self, visited: Any = None, *, return_value: bool = False, side_effect: bool = False) -> None: ...
 
 class MagicProxy(Base):
     name: str
     parent: Any
     def __init__(self, name: str, parent: Any) -> None: ...
     def create_mock(self) -> Any: ...
     def __get__(self, obj: Any, _type: Incomplete | None = None) -> Any: ...
@@ -374,7 +380,21 @@
 def mock_open(mock: Incomplete | None = None, read_data: Any = "") -> Any: ...
 
 class PropertyMock(Mock):
     def __get__(self, obj: _T, obj_type: type[_T] | None = None) -> Self: ...
     def __set__(self, obj: Any, value: Any) -> None: ...
 
 def seal(mock: Any) -> None: ...
+
+class ThreadingMixin(Base):
+    DEFAULT_TIMEOUT: ClassVar[float | None]
+
+    def __init__(self, *args: Any, timeout: float | None = ..., **kwargs: Any) -> None: ...
+    def reset_mock(self, *args: Any, **kwargs: Any) -> None: ...
+    def wait_until_called(self, *, timeout: float | None = ...) -> None: ...
+    def wait_until_any_call_with(self, *args: Any, **kwargs: Any) -> None: ...
+
+class ThreadingMock(ThreadingMixin, MagicMixin, Mock):
+    # Improving the `reset_mock` signature.
+    # It is defined on `ThreadingMixin` with `*args, **kwargs`, which is not ideal.
+    # But, `NonCallableMock` super-class has the better version.
+    def reset_mock(self, visited: Any = None, *, return_value: bool = False, side_effect: bool = False) -> None: ...
```

### Comparing `types-mock-5.0.0.7/setup.py` & `types-mock-5.1.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `mock`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/mock. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a46fe434772d105c1f8204565b2b8636c5bb108b` and was tested
-with mypy 1.3.0, pyright 1.1.314, and
-pytype 2023.6.2.
+This package was generated from typeshed commit `032f9195f9e3788a6e5c7ecb086f173a3ac92a95` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="5.0.0.7",
+      version="5.1.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/mock.md",
```

### Comparing `types-mock-5.0.0.7/types_mock.egg-info/PKG-INFO` & `types-mock-5.1.0.0/types_mock.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-mock
-Version: 5.0.0.7
+Version: 5.1.0.0
 Summary: Typing stubs for mock
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/mock.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,10 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `mock`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/mock. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a46fe434772d105c1f8204565b2b8636c5bb108b` and was tested
-with mypy 1.3.0, pyright 1.1.314, and
-pytype 2023.6.2.
+This package was generated from typeshed commit `032f9195f9e3788a6e5c7ecb086f173a3ac92a95` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

