# Comparing `tmp/cloudoll-2.0.5.tar.gz` & `tmp/cloudoll-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudoll-2.0.5.tar", last modified: Mon Jul 10 07:11:52 2023, max compression
+gzip compressed data, was "cloudoll-2.0.6.tar", last modified: Wed Jul 19 07:16:42 2023, max compression
```

## Comparing `cloudoll-2.0.5.tar` & `cloudoll-2.0.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-10 07:11:52.056258 cloudoll-2.0.5/
--rw-r--r--   0 xiaobei    (501) staff       (20)     1059 2023-03-15 06:24:14.000000 cloudoll-2.0.5/LICENSE
--rw-r--r--   0 xiaobei    (501) staff       (20)     7131 2023-07-10 07:11:52.055413 cloudoll-2.0.5/PKG-INFO
--rw-r--r--   0 xiaobei    (501) staff       (20)     6497 2023-07-06 01:49:11.000000 cloudoll-2.0.5/README.md
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-10 07:11:52.040408 cloudoll-2.0.5/cloudoll/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.5/cloudoll/__init__.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-10 07:11:52.045844 cloudoll-2.0.5/cloudoll/error/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.5/cloudoll/error/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     3501 2023-03-15 06:24:14.000000 cloudoll-2.0.5/cloudoll/error/errors.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-10 07:11:52.046697 cloudoll-2.0.5/cloudoll/logging/
--rw-r--r--   0 xiaobei    (501) staff       (20)     3818 2023-07-10 07:06:42.000000 cloudoll-2.0.5/cloudoll/logging/__init__.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-10 07:11:52.047944 cloudoll-2.0.5/cloudoll/mail/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.5/cloudoll/mail/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     5741 2023-05-23 03:27:31.000000 cloudoll-2.0.5/cloudoll/mail/smtp.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-10 07:11:52.049305 cloudoll-2.0.5/cloudoll/orm/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.5/cloudoll/orm/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)    27939 2023-07-03 04:38:49.000000 cloudoll-2.0.5/cloudoll/orm/mysql.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-10 07:11:52.051468 cloudoll-2.0.5/cloudoll/robot/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.5/cloudoll/robot/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     6380 2023-03-22 06:00:15.000000 cloudoll-2.0.5/cloudoll/robot/dingtalk.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     3114 2023-03-22 06:01:06.000000 cloudoll-2.0.5/cloudoll/robot/feishu.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-10 07:11:52.054548 cloudoll-2.0.5/cloudoll/web/
--rw-r--r--   0 xiaobei    (501) staff       (20)    13999 2023-07-10 07:06:42.000000 cloudoll-2.0.5/cloudoll/web/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     2077 2023-03-15 06:24:14.000000 cloudoll-2.0.5/cloudoll/web/html.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     3541 2023-05-23 03:27:31.000000 cloudoll-2.0.5/cloudoll/web/http.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     1097 2023-06-05 02:36:30.000000 cloudoll-2.0.5/cloudoll/web/jwt.py
--rw-r--r--   0 xiaobei    (501) staff       (20)      298 2023-04-24 09:13:28.000000 cloudoll-2.0.5/cloudoll/web/settings.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-10 07:11:52.044484 cloudoll-2.0.5/cloudoll.egg-info/
--rw-r--r--   0 xiaobei    (501) staff       (20)     7131 2023-07-10 07:11:51.000000 cloudoll-2.0.5/cloudoll.egg-info/PKG-INFO
--rw-r--r--   0 xiaobei    (501) staff       (20)      573 2023-07-10 07:11:51.000000 cloudoll-2.0.5/cloudoll.egg-info/SOURCES.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)        1 2023-07-10 07:11:51.000000 cloudoll-2.0.5/cloudoll.egg-info/dependency_links.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)      127 2023-07-10 07:11:51.000000 cloudoll-2.0.5/cloudoll.egg-info/requires.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)        9 2023-07-10 07:11:51.000000 cloudoll-2.0.5/cloudoll.egg-info/top_level.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)       38 2023-07-10 07:11:52.056451 cloudoll-2.0.5/setup.cfg
--rw-r--r--   0 xiaobei    (501) staff       (20)     4183 2023-07-10 07:07:38.000000 cloudoll-2.0.5/setup.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 07:16:42.178459 cloudoll-2.0.6/
+-rw-r--r--   0 xiaobei    (501) staff       (20)     1059 2023-03-15 06:24:14.000000 cloudoll-2.0.6/LICENSE
+-rw-r--r--   0 xiaobei    (501) staff       (20)     7235 2023-07-19 07:16:42.178063 cloudoll-2.0.6/PKG-INFO
+-rw-r--r--   0 xiaobei    (501) staff       (20)     6601 2023-07-10 08:09:57.000000 cloudoll-2.0.6/README.md
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 07:16:42.163613 cloudoll-2.0.6/cloudoll/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.6/cloudoll/__init__.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 07:16:42.168146 cloudoll-2.0.6/cloudoll/error/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.6/cloudoll/error/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     3501 2023-03-15 06:24:14.000000 cloudoll-2.0.6/cloudoll/error/errors.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 07:16:42.168998 cloudoll-2.0.6/cloudoll/logging/
+-rw-r--r--   0 xiaobei    (501) staff       (20)     4581 2023-07-11 02:48:07.000000 cloudoll-2.0.6/cloudoll/logging/__init__.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 07:16:42.169990 cloudoll-2.0.6/cloudoll/mail/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.6/cloudoll/mail/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     5741 2023-05-23 03:27:31.000000 cloudoll-2.0.6/cloudoll/mail/smtp.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 07:16:42.171299 cloudoll-2.0.6/cloudoll/orm/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.6/cloudoll/orm/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)    27939 2023-07-03 04:38:49.000000 cloudoll-2.0.6/cloudoll/orm/mysql.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 07:16:42.173609 cloudoll-2.0.6/cloudoll/robot/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.6/cloudoll/robot/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     6380 2023-03-22 06:00:15.000000 cloudoll-2.0.6/cloudoll/robot/dingtalk.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     3114 2023-03-22 06:01:06.000000 cloudoll-2.0.6/cloudoll/robot/feishu.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 07:16:42.177317 cloudoll-2.0.6/cloudoll/web/
+-rw-r--r--   0 xiaobei    (501) staff       (20)    15142 2023-07-19 07:14:54.000000 cloudoll-2.0.6/cloudoll/web/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     2077 2023-03-15 06:24:14.000000 cloudoll-2.0.6/cloudoll/web/html.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     3541 2023-05-23 03:27:31.000000 cloudoll-2.0.6/cloudoll/web/http.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     1097 2023-06-05 02:36:30.000000 cloudoll-2.0.6/cloudoll/web/jwt.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)      298 2023-04-24 09:13:28.000000 cloudoll-2.0.6/cloudoll/web/settings.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 07:16:42.166791 cloudoll-2.0.6/cloudoll.egg-info/
+-rw-r--r--   0 xiaobei    (501) staff       (20)     7235 2023-07-19 07:16:42.000000 cloudoll-2.0.6/cloudoll.egg-info/PKG-INFO
+-rw-r--r--   0 xiaobei    (501) staff       (20)      573 2023-07-19 07:16:42.000000 cloudoll-2.0.6/cloudoll.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)        1 2023-07-19 07:16:42.000000 cloudoll-2.0.6/cloudoll.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)      127 2023-07-19 07:16:42.000000 cloudoll-2.0.6/cloudoll.egg-info/requires.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)        9 2023-07-19 07:16:42.000000 cloudoll-2.0.6/cloudoll.egg-info/top_level.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)       38 2023-07-19 07:16:42.178568 cloudoll-2.0.6/setup.cfg
+-rw-r--r--   0 xiaobei    (501) staff       (20)     4187 2023-07-19 07:16:37.000000 cloudoll-2.0.6/setup.py
```

### Comparing `cloudoll-2.0.5/LICENSE` & `cloudoll-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.5/PKG-INFO` & `cloudoll-2.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudoll
-Version: 2.0.5
+Version: 2.0.6
 Summary: 辅助快速创建可分布的微服务。
 Home-page: https://gitee.com/chuchur/cloudoll-py
 Author: chuchur
 Author-email: chuchur@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -16,14 +16,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # cloudoll 云端玩具
 
 ## 更新日志
+`2.0.5` 2023-07-04
+- 修复redis在 3.11+环境下的问题
+
+`2.0.4` 2023-07-04
+- 切换热更为adev
+
+
 `2.0.2` 2023-07-03
 - 优化一系列问题
 - 可以热加载
 
 `2.0.0` 2023-06-09
 - 优化一系列问题
 - orm 执行更优雅
```

### Comparing `cloudoll-2.0.5/README.md` & `cloudoll-2.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 # cloudoll 云端玩具
 
 ## 更新日志
+`2.0.5` 2023-07-04
+- 修复redis在 3.11+环境下的问题
+
+`2.0.4` 2023-07-04
+- 切换热更为adev
+
+
 `2.0.2` 2023-07-03
 - 优化一系列问题
 - 可以热加载
 
 `2.0.0` 2023-06-09
 - 优化一系列问题
 - orm 执行更优雅
```

### Comparing `cloudoll-2.0.5/cloudoll/error/errors.py` & `cloudoll-2.0.6/cloudoll/error/errors.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.5/cloudoll/mail/smtp.py` & `cloudoll-2.0.6/cloudoll/mail/smtp.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.5/cloudoll/orm/mysql.py` & `cloudoll-2.0.6/cloudoll/orm/mysql.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.5/cloudoll/robot/dingtalk.py` & `cloudoll-2.0.6/cloudoll/robot/dingtalk.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.5/cloudoll/robot/feishu.py` & `cloudoll-2.0.6/cloudoll/robot/feishu.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.5/cloudoll/web/__init__.py` & `cloudoll-2.0.6/cloudoll/web/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 # -*- coding: utf-8 -*-
 
 __author__ = "chuchur/chuchur.com"
 
 import argparse
 import asyncio
 import hashlib
-import os, base64, datetime
+import os, base64
 import importlib
 import inspect
 import json
 import pkgutil
 import sys
 import socket
 from urllib import parse
-import aiomcache
+import aiomcache, aiojobs
 from redis import asyncio as aioredis
 from aiohttp import web
 from aiohttp.web_exceptions import *
 from aiohttp.web_ws import WebSocketResponse as WebSocket, WSMsgType
 from aiohttp_session import (
     get_session,
     setup,
@@ -29,14 +29,16 @@
 from jinja2 import Environment, FileSystemLoader
 from setuptools import find_packages
 from .settings import get_config
 
 from ..logging import logging
 from ..orm.mysql import sa
 from . import jwt
+from decimal import Decimal
+from datetime import datetime
 
 
 class _Handler(object):
     def __init__(self, cls, fn):
         self.cls = cls
         self.fn = fn
 
@@ -139,14 +141,16 @@
         self.mysql = None
         self.env = None
         self.app = None
         self._route_table = web.RouteTableDef()
         self._middleware = []
         self.config = {}
         self._args = None
+        self.tasks = None
+        self._run_tasks = {}
 
     def create(self):
         loop = asyncio.get_event_loop()
         if loop is None:
             loop = asyncio.new_event_loop()
         self._loop = loop
 
@@ -180,14 +184,21 @@
         self.app.config = config
         self.app.jwt_encode = self.jwt_encode
         self.app.jwt_decode = self.jwt_decode
         # session
         self._init_session()
         #  router:
         self._reg_router()
+        # start task
+        # self.tasks = await aiojobs.create_scheduler()
+        # await scheduler.close()
+        # await scheduler.join()
+        
+        # self._init_task()
+        # self.app.on_cleanup.append(self._free_task)
 
         # static
         if conf_server is not None:
             conf_st = conf_server.get("static")
             if conf_st:
                 temp = os.path.join(os.path.abspath("."), "static")
                 self.app.router.add_static(**conf_st, path=temp)
@@ -235,15 +246,15 @@
                     path = f"{username}:{password}@{path}"
                 redis_url = f"{protocol}://{path}"
 
             max_age = redis_conf.get("max_age")
             secure = redis_conf.get("secure")
             httponly = redis_conf.get("httponly")
             cookie_name = redis_conf.get("key", _SESSION_KEY)
-            
+
             redis = aioredis.from_url(redis_url)
             self.app.redis = redis
             storage = redis_storage.RedisStorage(
                 redis,
                 cookie_name=cookie_name,
                 max_age=_int(max_age),
                 httponly=httponly,
@@ -295,24 +306,48 @@
             # print(module, router)
             importlib.import_module(module, fd)
 
         self.app.add_routes(self._route_table)
         # for route in self._routes:
         #     self.app.router.add_route(**route)
 
+    def _create_task(self, fun):
+        if not callable(fun):
+            raise ValueError("Task must be function.")
+
+        def inner():
+            fun_name = getattr(fun, "__name__")
+            self._run_tasks[fun_name] = asyncio.create_task(fun())
+
+        return inner
+
+    def _init_task(self):
+        for task in self.tasks:
+            fun = self._create_task(task)
+            self.on_startup.append(fun)
+
+    def _free_task(self):
+        for task in self.tasks:
+            self.free_task(task)
+
+    async def free_task(self, fun: function):
+        fun_name = getattr(fun, "__name__")
+        task = self._run_tasks[fun_name]
+        if task:
+            del self._ran_tasks[fun_name]
+            task.cancel()
+            await task
+
     def run(self, *args, **kw):
         """
         run app
         :params prot default  9001
         :params host default 127.0.0.1
         """
         conf = self.config.get("server", {})
-        # if conf.get('reload',False) is True:
-        # import aioreloader
-        # aioreloader.start()
         conf.update(args)
         args = {k: v for k, v in vars(self._args).items() if v is not None}
         conf.update(args)
         host = conf.get("host", "127.0.0.1")
         port = conf.get("port", 9001)
         path = conf.get("path")
         _check_address(host, port)
@@ -402,42 +437,46 @@
 
     def __str__(self):
         return self.key
 
 
 class JsonEncoder(json.JSONEncoder):
     def default(self, obj):
-        if isinstance(obj, datetime.datetime) or isinstance(obj, datetime.date):
+        if isinstance(obj, datetime) or isinstance(obj, datetime.date):
             return obj.__str__()
+        elif isinstance(obj, Decimal):
+            return str(obj)
+        elif isinstance(obj, set):
+            return list(obj)
         else:
             return super(JsonEncoder, self).default(obj)
 
 
-def get(path, name=None):
+def get(path: str, name=None):
     return app.add_router(path, "GET", name)
 
 
-def post(path, name=None):
+def post(path: str, name=None):
     return app.add_router(path, "POST", name)
 
 
-def put(path, name=None):
+def put(path: str, name=None):
     return app.add_router(path, "PUT", name)
 
 
-def delete(path, name=None):
+def delete(path: str, name=None):
     return app.add_router(path, "DELETE", name)
 
 
-def all(path):
+def all(path: str):
     #     return app._actions(path, 'GET')
     return app.route_table.view(path)
 
 
-def jsons(data, **kw):
+def jsons(data, **kw) -> web.Response:
     res = {}
     if isinstance(data, list):
         res["data"] = data
     elif isinstance(data, dict):
         res.update(data)
     elif isinstance(data, tuple):
         data = dict(data)
```

### Comparing `cloudoll-2.0.5/cloudoll/web/html.py` & `cloudoll-2.0.6/cloudoll/web/html.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.5/cloudoll/web/http.py` & `cloudoll-2.0.6/cloudoll/web/http.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.5/cloudoll/web/jwt.py` & `cloudoll-2.0.6/cloudoll/web/jwt.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.5/cloudoll.egg-info/PKG-INFO` & `cloudoll-2.0.6/cloudoll.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudoll
-Version: 2.0.5
+Version: 2.0.6
 Summary: 辅助快速创建可分布的微服务。
 Home-page: https://gitee.com/chuchur/cloudoll-py
 Author: chuchur
 Author-email: chuchur@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -16,14 +16,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # cloudoll 云端玩具
 
 ## 更新日志
+`2.0.5` 2023-07-04
+- 修复redis在 3.11+环境下的问题
+
+`2.0.4` 2023-07-04
+- 切换热更为adev
+
+
 `2.0.2` 2023-07-03
 - 优化一系列问题
 - 可以热加载
 
 `2.0.0` 2023-06-09
 - 优化一系列问题
 - orm 执行更优雅
```

### Comparing `cloudoll-2.0.5/cloudoll.egg-info/SOURCES.txt` & `cloudoll-2.0.6/cloudoll.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.5/setup.py` & `cloudoll-2.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = "cloudoll"
 DESCRIPTION = "辅助快速创建可分布的微服务。"
 URL = "https://gitee.com/chuchur/cloudoll-py"
 EMAIL = "chuchur@qq.com"
 AUTHOR = "chuchur"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "2.0.5"
+VERSION = "2.0.6"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "requests",
     "colorlog",
     "aiomysql",
     "aiopg",
@@ -93,16 +93,16 @@
         self.status("Building Source and Wheel (universal) distribution…")
         os.system("{0} setup.py sdist bdist_wheel --universal".format(sys.executable))
 
         self.status("Uploading the package to PyPI via Twine…")
         os.system("twine upload dist/*")
 
         self.status("Pushing git tags…")
-        os.system("git tag v{0}".format(about["__version__"]))
-        os.system("git push --tags")
+        # os.system("git tag v{0}".format(about["__version__"]))
+        # os.system("git push --tags")
 
         sys.exit()
 
 
 # Where the magic happens:
 setup(
     name=NAME,
```

