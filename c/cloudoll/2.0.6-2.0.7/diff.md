# Comparing `tmp/cloudoll-2.0.6.tar.gz` & `tmp/cloudoll-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudoll-2.0.6.tar", last modified: Wed Jul 19 07:16:42 2023, max compression
+gzip compressed data, was "cloudoll-2.0.7.tar", last modified: Wed Jul 19 08:18:46 2023, max compression
```

## Comparing `cloudoll-2.0.6.tar` & `cloudoll-2.0.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 07:16:42.178459 cloudoll-2.0.6/
--rw-r--r--   0 xiaobei    (501) staff       (20)     1059 2023-03-15 06:24:14.000000 cloudoll-2.0.6/LICENSE
--rw-r--r--   0 xiaobei    (501) staff       (20)     7235 2023-07-19 07:16:42.178063 cloudoll-2.0.6/PKG-INFO
--rw-r--r--   0 xiaobei    (501) staff       (20)     6601 2023-07-10 08:09:57.000000 cloudoll-2.0.6/README.md
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 07:16:42.163613 cloudoll-2.0.6/cloudoll/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.6/cloudoll/__init__.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 07:16:42.168146 cloudoll-2.0.6/cloudoll/error/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.6/cloudoll/error/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     3501 2023-03-15 06:24:14.000000 cloudoll-2.0.6/cloudoll/error/errors.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 07:16:42.168998 cloudoll-2.0.6/cloudoll/logging/
--rw-r--r--   0 xiaobei    (501) staff       (20)     4581 2023-07-11 02:48:07.000000 cloudoll-2.0.6/cloudoll/logging/__init__.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 07:16:42.169990 cloudoll-2.0.6/cloudoll/mail/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.6/cloudoll/mail/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     5741 2023-05-23 03:27:31.000000 cloudoll-2.0.6/cloudoll/mail/smtp.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 07:16:42.171299 cloudoll-2.0.6/cloudoll/orm/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.6/cloudoll/orm/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)    27939 2023-07-03 04:38:49.000000 cloudoll-2.0.6/cloudoll/orm/mysql.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 07:16:42.173609 cloudoll-2.0.6/cloudoll/robot/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.6/cloudoll/robot/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     6380 2023-03-22 06:00:15.000000 cloudoll-2.0.6/cloudoll/robot/dingtalk.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     3114 2023-03-22 06:01:06.000000 cloudoll-2.0.6/cloudoll/robot/feishu.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 07:16:42.177317 cloudoll-2.0.6/cloudoll/web/
--rw-r--r--   0 xiaobei    (501) staff       (20)    15142 2023-07-19 07:14:54.000000 cloudoll-2.0.6/cloudoll/web/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     2077 2023-03-15 06:24:14.000000 cloudoll-2.0.6/cloudoll/web/html.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     3541 2023-05-23 03:27:31.000000 cloudoll-2.0.6/cloudoll/web/http.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     1097 2023-06-05 02:36:30.000000 cloudoll-2.0.6/cloudoll/web/jwt.py
--rw-r--r--   0 xiaobei    (501) staff       (20)      298 2023-04-24 09:13:28.000000 cloudoll-2.0.6/cloudoll/web/settings.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 07:16:42.166791 cloudoll-2.0.6/cloudoll.egg-info/
--rw-r--r--   0 xiaobei    (501) staff       (20)     7235 2023-07-19 07:16:42.000000 cloudoll-2.0.6/cloudoll.egg-info/PKG-INFO
--rw-r--r--   0 xiaobei    (501) staff       (20)      573 2023-07-19 07:16:42.000000 cloudoll-2.0.6/cloudoll.egg-info/SOURCES.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)        1 2023-07-19 07:16:42.000000 cloudoll-2.0.6/cloudoll.egg-info/dependency_links.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)      127 2023-07-19 07:16:42.000000 cloudoll-2.0.6/cloudoll.egg-info/requires.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)        9 2023-07-19 07:16:42.000000 cloudoll-2.0.6/cloudoll.egg-info/top_level.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)       38 2023-07-19 07:16:42.178568 cloudoll-2.0.6/setup.cfg
--rw-r--r--   0 xiaobei    (501) staff       (20)     4187 2023-07-19 07:16:37.000000 cloudoll-2.0.6/setup.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 08:18:46.446815 cloudoll-2.0.7/
+-rw-r--r--   0 xiaobei    (501) staff       (20)     1059 2023-03-15 06:24:14.000000 cloudoll-2.0.7/LICENSE
+-rw-r--r--   0 xiaobei    (501) staff       (20)     7278 2023-07-19 08:18:46.446397 cloudoll-2.0.7/PKG-INFO
+-rw-r--r--   0 xiaobei    (501) staff       (20)     6644 2023-07-19 08:17:48.000000 cloudoll-2.0.7/README.md
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 08:18:46.432034 cloudoll-2.0.7/cloudoll/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.7/cloudoll/__init__.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 08:18:46.436914 cloudoll-2.0.7/cloudoll/error/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.7/cloudoll/error/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     3501 2023-03-15 06:24:14.000000 cloudoll-2.0.7/cloudoll/error/errors.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 08:18:46.437552 cloudoll-2.0.7/cloudoll/logging/
+-rw-r--r--   0 xiaobei    (501) staff       (20)     4608 2023-07-19 08:14:53.000000 cloudoll-2.0.7/cloudoll/logging/__init__.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 08:18:46.438848 cloudoll-2.0.7/cloudoll/mail/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.7/cloudoll/mail/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     5741 2023-05-23 03:27:31.000000 cloudoll-2.0.7/cloudoll/mail/smtp.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 08:18:46.440312 cloudoll-2.0.7/cloudoll/orm/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.7/cloudoll/orm/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)    27939 2023-07-03 04:38:49.000000 cloudoll-2.0.7/cloudoll/orm/mysql.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 08:18:46.442259 cloudoll-2.0.7/cloudoll/robot/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.0.7/cloudoll/robot/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     6380 2023-03-22 06:00:15.000000 cloudoll-2.0.7/cloudoll/robot/dingtalk.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     3114 2023-03-22 06:01:06.000000 cloudoll-2.0.7/cloudoll/robot/feishu.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 08:18:46.445624 cloudoll-2.0.7/cloudoll/web/
+-rw-r--r--   0 xiaobei    (501) staff       (20)    14109 2023-07-19 07:31:20.000000 cloudoll-2.0.7/cloudoll/web/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     2077 2023-03-15 06:24:14.000000 cloudoll-2.0.7/cloudoll/web/html.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     3541 2023-05-23 03:27:31.000000 cloudoll-2.0.7/cloudoll/web/http.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     1097 2023-06-05 02:36:30.000000 cloudoll-2.0.7/cloudoll/web/jwt.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)      298 2023-04-24 09:13:28.000000 cloudoll-2.0.7/cloudoll/web/settings.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2023-07-19 08:18:46.435597 cloudoll-2.0.7/cloudoll.egg-info/
+-rw-r--r--   0 xiaobei    (501) staff       (20)     7278 2023-07-19 08:18:46.000000 cloudoll-2.0.7/cloudoll.egg-info/PKG-INFO
+-rw-r--r--   0 xiaobei    (501) staff       (20)      573 2023-07-19 08:18:46.000000 cloudoll-2.0.7/cloudoll.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)        1 2023-07-19 08:18:46.000000 cloudoll-2.0.7/cloudoll.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)      127 2023-07-19 08:18:46.000000 cloudoll-2.0.7/cloudoll.egg-info/requires.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)        9 2023-07-19 08:18:46.000000 cloudoll-2.0.7/cloudoll.egg-info/top_level.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)       38 2023-07-19 08:18:46.446929 cloudoll-2.0.7/setup.cfg
+-rw-r--r--   0 xiaobei    (501) staff       (20)     4183 2023-07-19 08:18:40.000000 cloudoll-2.0.7/setup.py
```

### Comparing `cloudoll-2.0.6/LICENSE` & `cloudoll-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.6/PKG-INFO` & `cloudoll-2.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudoll
-Version: 2.0.6
+Version: 2.0.7
 Summary: 辅助快速创建可分布的微服务。
 Home-page: https://gitee.com/chuchur/cloudoll-py
 Author: chuchur
 Author-email: chuchur@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -16,14 +16,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # cloudoll 云端玩具
 
 ## 更新日志
+`2.0.7` 2023-07-04
+- 修复logging 问题
+
 `2.0.5` 2023-07-04
 - 修复redis在 3.11+环境下的问题
 
 `2.0.4` 2023-07-04
 - 切换热更为adev
```

### Comparing `cloudoll-2.0.6/README.md` & `cloudoll-2.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # cloudoll 云端玩具
 
 ## 更新日志
+`2.0.7` 2023-07-04
+- 修复logging 问题
+
 `2.0.5` 2023-07-04
 - 修复redis在 3.11+环境下的问题
 
 `2.0.4` 2023-07-04
 - 切换热更为adev
```

### Comparing `cloudoll-2.0.6/cloudoll/error/errors.py` & `cloudoll-2.0.7/cloudoll/error/errors.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.6/cloudoll/logging/__init__.py` & `cloudoll-2.0.7/cloudoll/logging/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 __author__ = "chuchur/chuchur.com"
 
 import logging
 import os
 from datetime import datetime
 from logging.handlers import RotatingFileHandler
-
+from logging import INFO, DEBUG, ERROR, CRITICAL, DEBUG
 import colorlog
 
 _COLORS = {
     # 终端输出日志颜色配置
     "DEBUG": "white",
     "INFO": "green",
     "WARNING": "yellow",
@@ -30,15 +30,15 @@
 _LOG_FILES_COUNT = 3  # 最多保留3个日志文件
 
 
 class HandleLog:
     """
     建日志记录器(logging.getLogger)
     设置日志级别(logger.setLevel)
-    接着创建日志文件(logging.FileHandler)
+    创建日志文件(logging.FileHandler)
     设置日志格式(logging.Formatter)
     日志处理程序记录到记录器(addHandler)
     """
 
     def __init__(self):
         # cur_path = os.path.dirname(os.path.realpath(__file__))  # 当前项目路径
         # log_path = os.path.join(os.path.normpath(os.getcwd() + os.sep + os.pardir), 'logs')
@@ -50,29 +50,29 @@
             os.mkdir(log_path)  # 若不存在logs文件夹，则自动创建
         self.log_path = log_path
         self.log_path_prefix = None  # 当前日期格式化
         self.all_handle = None
         self.error_handle = None
 
         # console
-        if __debug__:
-            console_handle = colorlog.StreamHandler()
-            console_fmt = colorlog.ColoredFormatter(
-                _FORMATS["console_format"], log_colors=_COLORS
-            )
-            console_handle.setFormatter(console_fmt)
-            console_handle.setLevel(logging.DEBUG)
-            self.__logger.addHandler(console_handle)
+        # if __debug__:
+        console_handle = colorlog.StreamHandler()
+        console_fmt = colorlog.ColoredFormatter(
+            _FORMATS["console_format"], log_colors=_COLORS
+        )
+        console_handle.setFormatter(console_fmt)
+        console_handle.setLevel(DEBUG)
+        self.__logger.addHandler(console_handle)
 
     def setLevel(self, level):
         self.__logger.setLevel(level)
 
-    def getLogger(self, __file):
+    def getLogger(self, __file=None):
         self.__logger = logging.getLogger(__file)  # 创建日志记录器
-
+        self.__logger.setLevel(INFO)
         # self._set_handle()
         return self.__logger
 
     def __create_handler(self, log_path, level):
         handler = RotatingFileHandler(
             log_path,
             maxBytes=_LOG_SIZE,
@@ -107,20 +107,19 @@
             error_log_path = os.path.join(
                 self.log_path, "%s-error.log" % log_path_prefix
             )
 
             # set handle
             # self.__logger.setLevel(logging.INFO)  # 设置默认日志记录器记录级别
             # all
-            self.all_handle = self.__create_handler(all_log_path, logging.INFO)
+            self.all_handle = self.__create_handler(all_log_path, INFO)
             # error
-            self.error_handle = self.__create_handler(error_log_path, logging.ERROR)
+            self.error_handle = self.__create_handler(error_log_path, ERROR)
 
-        log = getattr(logger, method, None)
-        return log
+        return getattr(logger, method, None)
 
 
 _handler = None
 
 
 def _get_handle():
     global _handler
@@ -130,15 +129,15 @@
 
 
 def setLevel(level: int):
     _get_handle().setLevel(level)
 
 
 def getLogger(name=None):
-    return _get_handle().getLogger(name)
+    return _get_handle().getLogger(name=name)
 
 
 debug = _get_handle().log("debug")
 
 info = _get_handle().log("info")
 
 warning = _get_handle().log("warning")
```

### Comparing `cloudoll-2.0.6/cloudoll/mail/smtp.py` & `cloudoll-2.0.7/cloudoll/mail/smtp.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.6/cloudoll/orm/mysql.py` & `cloudoll-2.0.7/cloudoll/orm/mysql.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.6/cloudoll/robot/dingtalk.py` & `cloudoll-2.0.7/cloudoll/robot/dingtalk.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.6/cloudoll/robot/feishu.py` & `cloudoll-2.0.7/cloudoll/robot/feishu.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.6/cloudoll/web/__init__.py` & `cloudoll-2.0.7/cloudoll/web/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import importlib
 import inspect
 import json
 import pkgutil
 import sys
 import socket
 from urllib import parse
-import aiomcache, aiojobs
+import aiomcache
 from redis import asyncio as aioredis
 from aiohttp import web
 from aiohttp.web_exceptions import *
 from aiohttp.web_ws import WebSocketResponse as WebSocket, WSMsgType
 from aiohttp_session import (
     get_session,
     setup,
@@ -86,15 +86,15 @@
     request.session = session
 
 
 def _get_modules(fd):
     modules = set()
     temp = os.path.join(os.path.abspath("."), fd)
     if not os.path.exists(temp):
-        return
+        return modules
     s = find_packages(temp)
     for pkg in s:
         # modules.add(pkg)
         pkg_path = temp + "/" + pkg.replace(".", "/")
         if sys.version_info.major == 2 or (
             sys.version_info.major == 3 and sys.version_info.minor < 6
         ):
@@ -141,16 +141,14 @@
         self.mysql = None
         self.env = None
         self.app = None
         self._route_table = web.RouteTableDef()
         self._middleware = []
         self.config = {}
         self._args = None
-        self.tasks = None
-        self._run_tasks = {}
 
     def create(self):
         loop = asyncio.get_event_loop()
         if loop is None:
             loop = asyncio.new_event_loop()
         self._loop = loop
 
@@ -184,22 +182,15 @@
         self.app.config = config
         self.app.jwt_encode = self.jwt_encode
         self.app.jwt_decode = self.jwt_decode
         # session
         self._init_session()
         #  router:
         self._reg_router()
-        # start task
-        # self.tasks = await aiojobs.create_scheduler()
-        # await scheduler.close()
-        # await scheduler.join()
         
-        # self._init_task()
-        # self.app.on_cleanup.append(self._free_task)
-
         # static
         if conf_server is not None:
             conf_st = conf_server.get("static")
             if conf_st:
                 temp = os.path.join(os.path.abspath("."), "static")
                 self.app.router.add_static(**conf_st, path=temp)
                 logging.warning("Suggest using nginx or others instead.")
@@ -306,40 +297,14 @@
             # print(module, router)
             importlib.import_module(module, fd)
 
         self.app.add_routes(self._route_table)
         # for route in self._routes:
         #     self.app.router.add_route(**route)
 
-    def _create_task(self, fun):
-        if not callable(fun):
-            raise ValueError("Task must be function.")
-
-        def inner():
-            fun_name = getattr(fun, "__name__")
-            self._run_tasks[fun_name] = asyncio.create_task(fun())
-
-        return inner
-
-    def _init_task(self):
-        for task in self.tasks:
-            fun = self._create_task(task)
-            self.on_startup.append(fun)
-
-    def _free_task(self):
-        for task in self.tasks:
-            self.free_task(task)
-
-    async def free_task(self, fun: function):
-        fun_name = getattr(fun, "__name__")
-        task = self._run_tasks[fun_name]
-        if task:
-            del self._ran_tasks[fun_name]
-            task.cancel()
-            await task
 
     def run(self, *args, **kw):
         """
         run app
         :params prot default  9001
         :params host default 127.0.0.1
         """
```

### Comparing `cloudoll-2.0.6/cloudoll/web/html.py` & `cloudoll-2.0.7/cloudoll/web/html.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.6/cloudoll/web/http.py` & `cloudoll-2.0.7/cloudoll/web/http.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.6/cloudoll/web/jwt.py` & `cloudoll-2.0.7/cloudoll/web/jwt.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.6/cloudoll.egg-info/PKG-INFO` & `cloudoll-2.0.7/cloudoll.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudoll
-Version: 2.0.6
+Version: 2.0.7
 Summary: 辅助快速创建可分布的微服务。
 Home-page: https://gitee.com/chuchur/cloudoll-py
 Author: chuchur
 Author-email: chuchur@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -16,14 +16,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # cloudoll 云端玩具
 
 ## 更新日志
+`2.0.7` 2023-07-04
+- 修复logging 问题
+
 `2.0.5` 2023-07-04
 - 修复redis在 3.11+环境下的问题
 
 `2.0.4` 2023-07-04
 - 切换热更为adev
```

### Comparing `cloudoll-2.0.6/cloudoll.egg-info/SOURCES.txt` & `cloudoll-2.0.7/cloudoll.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudoll-2.0.6/setup.py` & `cloudoll-2.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = "cloudoll"
 DESCRIPTION = "辅助快速创建可分布的微服务。"
 URL = "https://gitee.com/chuchur/cloudoll-py"
 EMAIL = "chuchur@qq.com"
 AUTHOR = "chuchur"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "2.0.6"
+VERSION = "2.0.7"
 
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
-        # os.system("git tag v{0}".format(about["__version__"]))
-        # os.system("git push --tags")
+        os.system("git tag v{0}".format(about["__version__"]))
+        os.system("git push --tags")
 
         sys.exit()
 
 
 # Where the magic happens:
 setup(
     name=NAME,
```

