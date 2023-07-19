# Comparing `tmp/types-python-crontab-2.7.0.6.tar.gz` & `tmp/types-python-crontab-3.0.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-python-crontab-2.7.0.6.tar", last modified: Wed Feb 22 09:17:18 2023, max compression
+gzip compressed data, was "types-python-crontab-3.0.0.0.tar", last modified: Wed Jul 19 12:29:39 2023, max compression
```

## Comparing `types-python-crontab-2.7.0.6.tar` & `types-python-crontab-3.0.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:17:18.493898 types-python-crontab-2.7.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-02-22 09:17:17.000000 types-python-crontab-2.7.0.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-22 09:17:17.000000 types-python-crontab-2.7.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-02-22 09:17:18.493898 types-python-crontab-2.7.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:17:18.493898 types-python-crontab-2.7.0.6/cronlog-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-22 09:17:17.000000 types-python-crontab-2.7.0.6/cronlog-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-02-22 09:17:17.000000 types-python-crontab-2.7.0.6/cronlog-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:17:18.493898 types-python-crontab-2.7.0.6/crontab-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-22 09:17:17.000000 types-python-crontab-2.7.0.6/crontab-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-02-22 09:17:17.000000 types-python-crontab-2.7.0.6/crontab-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:17:18.493898 types-python-crontab-2.7.0.6/crontabs-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-22 09:17:17.000000 types-python-crontab-2.7.0.6/crontabs-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-02-22 09:17:17.000000 types-python-crontab-2.7.0.6/crontabs-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 09:17:18.493898 types-python-crontab-2.7.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-02-22 09:17:17.000000 types-python-crontab-2.7.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:17:18.493898 types-python-crontab-2.7.0.6/types_python_crontab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-02-22 09:17:18.000000 types-python-crontab-2.7.0.6/types_python_crontab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-02-22 09:17:18.000000 types-python-crontab-2.7.0.6/types_python_crontab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 09:17:18.000000 types-python-crontab-2.7.0.6/types_python_crontab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-22 09:17:18.000000 types-python-crontab-2.7.0.6/types_python_crontab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:29:39.035303 types-python-crontab-3.0.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-19 12:29:37.000000 types-python-crontab-3.0.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 12:29:37.000000 types-python-crontab-3.0.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-19 12:29:39.035303 types-python-crontab-3.0.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:29:39.035303 types-python-crontab-3.0.0.0/cronlog-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-19 12:29:37.000000 types-python-crontab-3.0.0.0/cronlog-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-19 12:29:37.000000 types-python-crontab-3.0.0.0/cronlog-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:29:39.035303 types-python-crontab-3.0.0.0/crontab-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-19 12:29:37.000000 types-python-crontab-3.0.0.0/crontab-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-07-19 12:29:37.000000 types-python-crontab-3.0.0.0/crontab-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:29:39.035303 types-python-crontab-3.0.0.0/crontabs-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-19 12:29:37.000000 types-python-crontab-3.0.0.0/crontabs-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-19 12:29:37.000000 types-python-crontab-3.0.0.0/crontabs-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 12:29:39.035303 types-python-crontab-3.0.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-19 12:29:37.000000 types-python-crontab-3.0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:29:39.035303 types-python-crontab-3.0.0.0/types_python_crontab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-19 12:29:38.000000 types-python-crontab-3.0.0.0/types_python_crontab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-19 12:29:39.000000 types-python-crontab-3.0.0.0/types_python_crontab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:29:38.000000 types-python-crontab-3.0.0.0/types_python_crontab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-19 12:29:38.000000 types-python-crontab-3.0.0.0/types_python_crontab.egg-info/top_level.txt
```

### Comparing `types-python-crontab-2.7.0.6/CHANGELOG.md` & `types-python-crontab-3.0.0.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 3.0.0.0 (2023-07-19)
+
+Update `python-crontab` to `3.0.*` (#10475)
+
 ## 2.7.0.6 (2023-02-22)
 
 Update `Unused` parameters in `stubs/` (#9704)
 
 * Update _Unused TypeAlias
 
 * Update `object | None` params
```

### Comparing `types-python-crontab-2.7.0.6/PKG-INFO` & `types-python-crontab-3.0.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-python-crontab
-Version: 2.7.0.6
+Version: 3.0.0.0
 Summary: Typing stubs for python-crontab
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-crontab.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `python-crontab`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-crontab. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `078c6a095892e12c94462889fa43c2c2dc8280ad`.
+This package was generated from typeshed commit `032f9195f9e3788a6e5c7ecb086f173a3ac92a95` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-python-crontab-2.7.0.6/cronlog-stubs/__init__.pyi` & `types-python-crontab-3.0.0.0/cronlog-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-python-crontab-2.7.0.6/crontab-stubs/__init__.pyi` & `types-python-crontab-3.0.0.0/crontab-stubs/__init__.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import re
 import subprocess
-from _typeshed import Incomplete, Unused
+from _typeshed import Incomplete
 from builtins import range as _range
 from collections import OrderedDict
 from collections.abc import Callable, Generator, Iterable, Iterator
 from datetime import datetime
 from logging import Logger
 from types import TracebackType
-from typing import Any
+from typing import Any, overload
 from typing_extensions import Self, SupportsIndex, TypeAlias
 
 from cronlog import CronLog
 
 _User: TypeAlias = str | bool | None
 
 __pkgname__: str
@@ -28,15 +28,26 @@
 SYSTEMV: bool
 ZERO_PAD: bool
 LOG: Logger
 CRON_COMMAND: str
 SHELL: str
 current_user: Callable[[], str | None]
 
-def open_pipe(cmd: str, *args: str, **flags: str) -> subprocess.Popen[Any]: ...
+class Process:
+    env: subprocess._ENV | None
+    args: tuple[str, ...]
+    has_run: bool
+    stdout: str | None
+    stderr: str | None
+    returncode: int | None
+    # `posix` and `env` are known special kwargs:
+    def __init__(self, cmd: str, *args: str, posix: bool = ..., env: subprocess._ENV | None = None, **flags: object) -> None: ...
+    def run(self) -> Self: ...
+    def __int__(self) -> int: ...  # technically, it can return `None` before `run` is called
+    def __eq__(self, other: object) -> bool: ...
 
 class CronTab:
     lines: list[str | CronItem] | None
     crons: list[CronItem] | None
     filen: str | None
     cron_command: str
     env: OrderedVariableList | None
@@ -65,16 +76,15 @@
         before: str | re.Pattern[str] | list[CronItem] | tuple[CronItem, ...] | Generator[CronItem, Any, Any] | None = ...,
     ) -> None: ...
     def write(self, filename: str | None = ..., user: _User = ..., errors: bool = ...) -> None: ...
     def write_to_user(self, user: bool | str = ...) -> None: ...
     # Usually `kwargs` are just `now: datetime | None`, but technically this can
     # work for `CronItem` subclasses, which might define other kwargs.
     def run_pending(self, **kwargs: Any) -> Iterator[str]: ...
-    # There are two known kwargs and others are unused:
-    def run_scheduler(self, timeout: int = ..., *, warp: object = ..., cadence: int = ..., **kwargs: Unused) -> Iterator[str]: ...
+    def run_scheduler(self, timeout: int = -1, cadence: int = 60, warp: bool = False) -> Iterator[str]: ...
     def render(self, errors: bool = ..., specials: bool | None = ...) -> str: ...
     def new(
         self,
         command: str = ...,
         comment: str = ...,
         user: str | None = ...,
         pre_comment: bool = ...,
@@ -128,14 +138,27 @@
     def every(self, unit: int = ...) -> Every: ...
     def setall(self, *args: Any) -> None: ...
     def clear(self) -> None: ...
     def frequency(self, year: int | None = ...) -> int: ...
     def frequency_per_year(self, year: int | None = ...) -> int: ...
     def frequency_per_day(self) -> int: ...
     def frequency_per_hour(self) -> int: ...
+    def frequency_at_year(self, year: int | None = None) -> int: ...
+    @overload
+    def frequency_at_month(self, year: int, month: int) -> int: ...
+    @overload
+    def frequency_at_month(self, year: None = None, month: None = None) -> int: ...
+    @overload
+    def frequency_at_day(self, year: int, month: int, day: int) -> int: ...
+    @overload
+    def frequency_at_day(self, year: None = None, month: None = None, day: None = None) -> int: ...
+    @overload
+    def frequency_at_hour(self, year: int, month: int, day: int, hour: int) -> int: ...
+    @overload
+    def frequency_at_hour(self, year: None = None, month: None = None, day: None = None, hour: None = None) -> int: ...
     def run_pending(self, now: datetime | None = ...) -> int | str: ...
     def run(self) -> str: ...
     # TODO: use types from `croniter` module here:
     def schedule(self, date_from: datetime | None = ...) -> Incomplete: ...
     # TODO: use types from `cron_descriptor` here:
     def description(self, **kw: Incomplete) -> Incomplete: ...
     @property
@@ -181,14 +204,27 @@
     def clean_render(self) -> str: ...
     def render(self, specials: bool = ...) -> str: ...
     def clear(self) -> None: ...
     def frequency(self, year: int | None = ...) -> int: ...
     def frequency_per_year(self, year: int | None = ...) -> int: ...
     def frequency_per_day(self) -> int: ...
     def frequency_per_hour(self) -> int: ...
+    def frequency_at_year(self, year: int | None = None) -> int: ...
+    @overload
+    def frequency_at_month(self, year: int, month: int) -> int: ...
+    @overload
+    def frequency_at_month(self, year: None = None, month: None = None) -> int: ...
+    @overload
+    def frequency_at_day(self, year: int, month: int, day: int) -> int: ...
+    @overload
+    def frequency_at_day(self, year: None = None, month: None = None, day: None = None) -> int: ...
+    @overload
+    def frequency_at_hour(self, year: int, month: int, day: int, hour: int) -> int: ...
+    @overload
+    def frequency_at_hour(self, year: None = None, month: None = None, day: None = None, hour: None = None) -> int: ...
     def __eq__(self, arg: object) -> bool: ...
 
 class SundayError(KeyError): ...
 
 class Also:
     obj: CronSlice
     def __init__(self, obj: CronSlice) -> None: ...
@@ -205,15 +241,15 @@
     max: int | None
     name: str | None
     enum: list[str | None] | None
     parts: list[_Part]
     def __init__(self, info: int | dict[str, Any], value: str | None = ...) -> None: ...
     def __hash__(self) -> int: ...
     def parse(self, value: str | None) -> None: ...
-    def render(self, resolve: bool = ..., specials: bool = ...) -> str: ...
+    def render(self, resolve: bool = False) -> str: ...
     def __eq__(self, arg: object) -> bool: ...
     def every(self, n_value: int, also: bool = ...) -> _Part: ...
     # The only known kwarg, others are unused,
     # `*args`` are passed to `parse_value`, so they are `Any`
     def on(self, *n_value: Any, also: bool = ...) -> list[_Part]: ...
     def during(self, vfrom: int | str, vto: int | str, also: bool = ...) -> _Part: ...
     @property
```

### Comparing `types-python-crontab-2.7.0.6/crontabs-stubs/__init__.pyi` & `types-python-crontab-3.0.0.0/crontabs-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-python-crontab-2.7.0.6/setup.py` & `types-python-crontab-3.0.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,32 +12,34 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `python-crontab`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-crontab. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `078c6a095892e12c94462889fa43c2c2dc8280ad`.
+This package was generated from typeshed commit `032f9195f9e3788a6e5c7ecb086f173a3ac92a95` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="2.7.0.6",
+      version="3.0.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-crontab.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
-      packages=['crontab-stubs', 'cronlog-stubs', 'crontabs-stubs'],
-      package_data={'crontab-stubs': ['__init__.pyi', 'METADATA.toml'], 'cronlog-stubs': ['__init__.pyi', 'METADATA.toml'], 'crontabs-stubs': ['__init__.pyi', 'METADATA.toml']},
+      packages=['cronlog-stubs', 'crontab-stubs', 'crontabs-stubs'],
+      package_data={'cronlog-stubs': ['__init__.pyi', 'METADATA.toml'], 'crontab-stubs': ['__init__.pyi', 'METADATA.toml'], 'crontabs-stubs': ['__init__.pyi', 'METADATA.toml']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-python-crontab-2.7.0.6/types_python_crontab.egg-info/PKG-INFO` & `types-python-crontab-3.0.0.0/types_python_crontab.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-python-crontab
-Version: 2.7.0.6
+Version: 3.0.0.0
 Summary: Typing stubs for python-crontab
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-crontab.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `python-crontab`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-crontab. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `078c6a095892e12c94462889fa43c2c2dc8280ad`.
+This package was generated from typeshed commit `032f9195f9e3788a6e5c7ecb086f173a3ac92a95` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

