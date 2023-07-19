# Comparing `tmp/bchmnn.poodle-0.2.4.tar.gz` & `tmp/bchmnn.poodle-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bchmnn.poodle-0.2.4.tar", last modified: Mon Jul 17 15:52:58 2023, max compression
+gzip compressed data, was "bchmnn.poodle-0.2.5.tar", last modified: Wed Jul 19 10:22:24 2023, max compression
```

## Comparing `bchmnn.poodle-0.2.4.tar` & `bchmnn.poodle-0.2.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:52:58.595575 bchmnn.poodle-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44286 2023-07-17 15:52:58.595575 bchmnn.poodle-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:52:58.595575 bchmnn.poodle-0.2.4/bchmnn.poodle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44286 2023-07-17 15:52:58.000000 bchmnn.poodle-0.2.4/bchmnn.poodle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-17 15:52:58.000000 bchmnn.poodle-0.2.4/bchmnn.poodle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:52:58.000000 bchmnn.poodle-0.2.4/bchmnn.poodle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 15:52:58.000000 bchmnn.poodle-0.2.4/bchmnn.poodle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 15:52:58.000000 bchmnn.poodle-0.2.4/bchmnn.poodle.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:52:58.595575 bchmnn.poodle-0.2.4/poodle/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/corews.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/poodle.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:52:58.595575 bchmnn.poodle-0.2.4/poodle/types/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26959 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/types/assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/types/course.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/types/courses.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/types/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/types/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/types/jsonable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/types/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/types/site.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/types/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/types/ws.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:52:58.595575 bchmnn.poodle-0.2.4/poodle/util/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/util/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/util/loggable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/util/parse_form.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/poodle/util/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-17 15:52:20.000000 bchmnn.poodle-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:52:58.595575 bchmnn.poodle-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:22:24.279823 bchmnn.poodle-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44286 2023-07-19 10:22:24.279823 bchmnn.poodle-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:22:24.271823 bchmnn.poodle-0.2.5/bchmnn.poodle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44286 2023-07-19 10:22:24.000000 bchmnn.poodle-0.2.5/bchmnn.poodle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-19 10:22:24.000000 bchmnn.poodle-0.2.5/bchmnn.poodle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 10:22:24.000000 bchmnn.poodle-0.2.5/bchmnn.poodle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-19 10:22:24.000000 bchmnn.poodle-0.2.5/bchmnn.poodle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-19 10:22:24.000000 bchmnn.poodle-0.2.5/bchmnn.poodle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:22:24.275823 bchmnn.poodle-0.2.5/poodle/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/poodle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/poodle/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/poodle/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/poodle/corews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/poodle/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/poodle/poodle.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/poodle/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:22:24.279823 bchmnn.poodle-0.2.5/poodle/typedefs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/poodle/typedefs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26959 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/poodle/typedefs/assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/poodle/typedefs/course.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/poodle/typedefs/courses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/poodle/typedefs/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/poodle/typedefs/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/poodle/typedefs/jsonable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/poodle/typedefs/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/poodle/typedefs/site.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/poodle/typedefs/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/poodle/typedefs/ws.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:22:24.279823 bchmnn.poodle-0.2.5/poodle/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/poodle/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/poodle/util/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/poodle/util/loggable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/poodle/util/parse_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/poodle/util/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-19 10:21:44.000000 bchmnn.poodle-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 10:22:24.279823 bchmnn.poodle-0.2.5/setup.cfg
```

### Comparing `bchmnn.poodle-0.2.4/LICENSE` & `bchmnn.poodle-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.4/PKG-INFO` & `bchmnn.poodle-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bchmnn.poodle
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python Moodle SDK
 Author-email: Jacob Bachmann <jacob.bachmann@posteo.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bchmnn.poodle-0.2.4/README.md` & `bchmnn.poodle-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.4/bchmnn.poodle.egg-info/PKG-INFO` & `bchmnn.poodle-0.2.5/bchmnn.poodle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bchmnn.poodle
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python Moodle SDK
 Author-email: Jacob Bachmann <jacob.bachmann@posteo.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bchmnn.poodle-0.2.4/bchmnn.poodle.egg-info/SOURCES.txt` & `bchmnn.poodle-0.2.5/bchmnn.poodle.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 poodle/__init__.py
 poodle/auth.py
 poodle/constants.py
 poodle/corews.py
 poodle/credentials.py
 poodle/poodle.py
 poodle/py.typed
-poodle/types/__init__.py
-poodle/types/assign.py
-poodle/types/course.py
-poodle/types/courses.py
-poodle/types/exception.py
-poodle/types/groups.py
-poodle/types/jsonable.py
-poodle/types/methods.py
-poodle/types/site.py
-poodle/types/tag.py
-poodle/types/ws.py
+poodle/typedefs/__init__.py
+poodle/typedefs/assign.py
+poodle/typedefs/course.py
+poodle/typedefs/courses.py
+poodle/typedefs/exception.py
+poodle/typedefs/groups.py
+poodle/typedefs/jsonable.py
+poodle/typedefs/methods.py
+poodle/typedefs/site.py
+poodle/typedefs/tag.py
+poodle/typedefs/ws.py
 poodle/util/__init__.py
 poodle/util/cache.py
 poodle/util/loggable.py
 poodle/util/parse_form.py
 poodle/util/tokens.py
```

### Comparing `bchmnn.poodle-0.2.4/poodle/auth.py` & `bchmnn.poodle-0.2.5/poodle/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import logging
 import random
 from abc import abstractmethod
 from typing import List, Optional
 
 import aiohttp
 
-from .types.exception import AuthError
-from .types.site import CoreSitePublicConfig
+from .typedefs.exception import AuthError
+from .typedefs.site import CoreSitePublicConfig
 from .util.loggable import Loggable
 from .util.tokens import Tokens
 
 
 class AbstractSSOHandler(Loggable):
     _priority: int
     # supported id provider workflows
```

### Comparing `bchmnn.poodle-0.2.4/poodle/corews.py` & `bchmnn.poodle-0.2.5/poodle/corews.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import typing
 from typing import Dict, Mapping, Optional
 from urllib import parse
 
 import aiohttp
 
 from .constants import CONTENT_TYPE, X_WWW_FORM_URLENCODED
-from .types.exception import CoreAjaxWSError, CoreConnectionError, CoreWSError
+from .typedefs.exception import (CoreAjaxWSError, CoreConnectionError,
+                                 CoreWSError)
 from .util.parse_form import parse_form
 from .util.tokens import Tokens
 
 
 class CoreWS(aiohttp.ClientSession):
     _url: str
     _tokens: Tokens
```

### Comparing `bchmnn.poodle-0.2.4/poodle/credentials.py` & `bchmnn.poodle-0.2.5/poodle/credentials.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.4/poodle/poodle.py` & `bchmnn.poodle-0.2.5/poodle/poodle.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import inspect
 import logging
 import re
 from typing import Any, List, Optional
 
 from .auth import AbstractSSOHandler, BrowserSSOHandler
 from .corews import CoreWS
-from .types.exception import (AuthError, CourseNotFoundError,
-                              MissingPrivateAccessKeyError)
-from .types.methods import DataTypeT, MoodleMethod, MoodleMethods, ReturnTypeT
-from .types.site import CoreSitePublicConfig
+from .typedefs.exception import (AuthError, CourseNotFoundError,
+                                 MissingPrivateAccessKeyError)
+from .typedefs.methods import (DataTypeT, MoodleMethod, MoodleMethods,
+                               ReturnTypeT)
+from .typedefs.site import CoreSitePublicConfig
 from .util.cache import Cache, CacheItem
 from .util.loggable import Loggable
+from .util.parse_form import parse_form
 from .util.tokens import Tokens
 
 
 class Poodle(Loggable, CoreWS):
     cache: Cache = Cache()
     _auth_handlers: List[AbstractSSOHandler]
 
@@ -68,16 +70,17 @@
         self,
         method: MoodleMethod[Any, ReturnTypeT, DataTypeT],
         data: Optional[DataTypeT] = None,
         usecache=True,
         refetch=False,
     ) -> ReturnTypeT:
         key = method["key"]
+        cachekey = key if data is None else key + parse_form(dict(data))
         return_type = method["type"]
-        cacheitem: CacheItem = {"key": key, "type": return_type}
+        cacheitem: CacheItem = {"key": cachekey, "type": return_type}
         if usecache and not refetch:
             _item = self.cache.get(cacheitem)
             if _item is not None:
                 return _item
         self.logger.debug("Fetching %s ...", key)
         item = return_type(**await self.call(key, data))  # type: ignore
         if usecache:
@@ -88,16 +91,17 @@
         self,
         method: MoodleMethod[List, ReturnTypeT, DataTypeT],
         data: Optional[DataTypeT] = None,
         usecache=True,
         refetch=False,
     ) -> List[ReturnTypeT]:
         key = method["key"]
+        cachekey = key if data is None else key + parse_form(dict(data))
         return_type = method["type"]
-        cacheitem: CacheItem = {"key": key, "type": return_type}
+        cacheitem: CacheItem = {"key": cachekey, "type": return_type}
         if usecache and not refetch:
             _item = self.cache.get(cacheitem)
             if _item is not None:
                 return _item
         self.logger.debug("Fetching %s ...", key)
         item = [return_type(**entry) for entry in await self.call(key, data)]
         if usecache:
@@ -134,83 +138,87 @@
         token = (await self.core_webservice_get_site_info()).userprivateaccesskey
         if token is None:
             raise MissingPrivateAccessKeyError(
                 "Current site is missing userprivateaccesskey"
             )
         return await self.get(self.fix_file_url(url, token))
 
-    async def core_enrol_get_users_courses(self, userid: Optional[int] = None):
+    async def core_enrol_get_users_courses(
+        self, userid: Optional[int] = None, refetch=False
+    ):
         if userid is None:
             userid = (await self.core_webservice_get_site_info()).userid
         return await self.fetch_list(
             MoodleMethods.CORE_ENROL_GET_USERS_COURSES,
             {"userid": userid, "returnusercount": 0},
-            usecache=False,
+            refetch,
         )
 
-    async def get_user_courses(self, name: str, userid: Optional[int] = None):
-        courses = await self.core_enrol_get_users_courses(userid)
+    async def get_user_courses(
+        self, name: str, userid: Optional[int] = None, refetch=False
+    ):
+        courses = await self.core_enrol_get_users_courses(userid, refetch)
         return [item for item in courses if name.lower() in item.fullname.lower()]
 
-    async def get_user_course(self, name: str, userid: Optional[int] = None):
-        courses = await self.get_user_courses(name, userid)
+    async def get_user_course(
+        self, name: str, userid: Optional[int] = None, refetch=False
+    ):
+        courses = await self.get_user_courses(name, userid, refetch)
         if len(courses) == 0:
             raise CourseNotFoundError(f"Could not find course: '{name}'")
         return courses[0]
 
-    async def core_course_get_contents(self, courseid: int):
+    async def core_course_get_contents(self, courseid: int, refetch=False):
         return await self.fetch_list(
             MoodleMethods.CORE_COURSE_GET_CONTENTS,
             {"courseid": courseid},
-            usecache=False,
+            refetch,
         )
 
-    async def mod_assign_get_assignments(self, courseids: List[int]):
+    async def mod_assign_get_assignments(self, courseids: List[int], refetch=False):
         return await self.fetch(
-            MoodleMethods.MOD_ASSIGN_GET_ASSIGNMENTS,
-            {"courseids": courseids},
-            usecache=False,
+            MoodleMethods.MOD_ASSIGN_GET_ASSIGNMENTS, {"courseids": courseids}, refetch
         )
 
-    async def get_assignments(self, courseid: int):
+    async def get_assignments(self, courseid: int, refetch=False):
         return (
-            (await self.mod_assign_get_assignments([courseid])).courses[0].assignments
+            (await self.mod_assign_get_assignments([courseid], refetch))
+            .courses[0]
+            .assignments
         )
 
-    async def get_assignment(self, courseid: int, index: int = 0):
-        assignments = await self.get_assignments(courseid)
+    async def get_assignment(self, courseid: int, index: int = 0, refetch=False):
+        assignments = await self.get_assignments(courseid, refetch)
         if (
             index >= 0
             and index >= len(assignments)
             or index < 0
             and -index >= len(assignments)
         ):
             raise IndexError("Index out of bounds")
         return assignments[index]
 
-    async def mod_assign_get_submissions(self, assignmentids: List[int]):
+    async def mod_assign_get_submissions(self, assignmentids: List[int], refetch=False):
         return await self.fetch(
             MoodleMethods.MOD_ASSIGN_GET_SUBMISSIONS,
             {"assignmentids": assignmentids},
-            usecache=False,
+            refetch,
         )
 
-    async def get_submissions(self, assignmentid: int):
+    async def get_submissions(self, assignmentid: int, refetch=False):
         return (
-            (await self.mod_assign_get_submissions([assignmentid]))
+            (await self.mod_assign_get_submissions([assignmentid], refetch))
             .assignments[0]
             .submissions
         )
 
-    async def mod_assign_list_participants(self, assignid: int):
+    async def mod_assign_list_participants(self, assignid: int, refetch=False):
         return await self.fetch_list(
             MoodleMethods.MOD_ASSIGN_LIST_PARTICIPANTS,
             {"assignid": assignid, "groupid": 0, "filter": ""},
-            usecache=False,
+            refetch,
         )
 
-    async def core_group_get_course_groups(self, courseid: int):
+    async def core_group_get_course_groups(self, courseid: int, refetch=False):
         return await self.fetch_list(
-            MoodleMethods.CORE_GROUP_GET_COURSE_GROUPS,
-            {"courseid": courseid},
-            usecache=False,
+            MoodleMethods.CORE_GROUP_GET_COURSE_GROUPS, {"courseid": courseid}, refetch
         )
```

### Comparing `bchmnn.poodle-0.2.4/poodle/types/assign.py` & `bchmnn.poodle-0.2.5/poodle/typedefs/assign.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.4/poodle/types/course.py` & `bchmnn.poodle-0.2.5/poodle/typedefs/course.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.4/poodle/types/courses.py` & `bchmnn.poodle-0.2.5/poodle/typedefs/courses.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.4/poodle/types/exception.py` & `bchmnn.poodle-0.2.5/poodle/typedefs/exception.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,14 +21,18 @@
         self.errorcode = errorcode
 
 
 class CoreAjaxWSError(CoreWSError):
     pass
 
 
+class CredentialProviderError(PoodleError):
+    pass
+
+
 class AuthError(PoodleError):
     pass
 
 
 class MissingPrivateAccessKeyError(PoodleError):
     pass
```

### Comparing `bchmnn.poodle-0.2.4/poodle/types/methods.py` & `bchmnn.poodle-0.2.5/poodle/typedefs/methods.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.4/poodle/types/site.py` & `bchmnn.poodle-0.2.5/poodle/typedefs/site.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import IntEnum
 from typing import List, Optional
 
-from poodle.types.jsonable import Jsonable
-from poodle.types.ws import CoreWSExternalWarning
+from poodle.typedefs.jsonable import Jsonable
+from poodle.typedefs.ws import CoreWSExternalWarning
 
 
 class CoreSiteQRCodeType(Jsonable, IntEnum):
     QR_CODE_DISABLED = 0  # QR code disabled value
     QR_CODE_URL = 1  # QR code type URL value
     QR_CODE_LOGIN = 2  # QR code type login value
```

### Comparing `bchmnn.poodle-0.2.4/poodle/types/tag.py` & `bchmnn.poodle-0.2.5/poodle/typedefs/tag.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.4/poodle/types/ws.py` & `bchmnn.poodle-0.2.5/poodle/typedefs/ws.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from poodle.types.jsonable import Jsonable
+from poodle.typedefs.jsonable import Jsonable
 
 
 # Structure of warnings returned by WS.
 class CoreWSExternalWarning(Jsonable):
     item: Optional[str] = None
     itemid: Optional[int] = None
     warningcode: Optional[
```

### Comparing `bchmnn.poodle-0.2.4/poodle/util/cache.py` & `bchmnn.poodle-0.2.5/poodle/util/cache.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.4/poodle/util/loggable.py` & `bchmnn.poodle-0.2.5/poodle/util/loggable.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.4/poodle/util/parse_form.py` & `bchmnn.poodle-0.2.5/poodle/util/parse_form.py`

 * *Files identical despite different names*

### Comparing `bchmnn.poodle-0.2.4/pyproject.toml` & `bchmnn.poodle-0.2.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bchmnn.poodle"
-version = "0.2.4"
+version = "0.2.5"
 description = "Python Moodle SDK"
 readme = "README.md"
 authors = [{ name = "Jacob Bachmann", email = "jacob.bachmann@posteo.de" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -38,20 +38,23 @@
 [project.urls]
 Homepage = "https://github.com/bchmnn/poodle"
 
 [tool.setuptools.package-data]
 "poodle" = ["py.typed"]
 
 [tool.bumpver]
-current_version = "0.2.4"
+current_version = "0.2.5"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "feat: release v{new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
     'version = "{version}"'
 ]
 "poodle/__init__.py" = ["{version}"]
+
+[tool.mypy]
+files = "poodle/**/*.py"
```

