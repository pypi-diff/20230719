# Comparing `tmp/mctech_cloud-1.0.1.tar.gz` & `tmp/mctech_cloud-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mctech_cloud-1.0.1.tar", last modified: Fri Jun 16 07:50:42 2023, max compression
+gzip compressed data, was "mctech_cloud-1.0.2.tar", last modified: Wed Jul 19 07:47:26 2023, max compression
```

## Comparing `mctech_cloud-1.0.1.tar` & `mctech_cloud-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 07:50:42.184494 mctech_cloud-1.0.1/
--rw-rw-rw-   0        0        0       59 2023-06-16 07:50:42.183493 mctech_cloud-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      529 2023-06-16 07:43:18.000000 mctech_cloud-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 07:50:42.164476 mctech_cloud-1.0.1/mctech_cloud/
--rw-rw-rw-   0        0        0       35 2023-06-16 07:43:18.000000 mctech_cloud-1.0.1/mctech_cloud/__init__.py
--rw-rw-rw-   0        0        0     1996 2023-06-16 07:43:18.000000 mctech_cloud-1.0.1/mctech_cloud/app_server.py
--rw-rw-rw-   0        0        0      962 2023-06-16 07:43:18.000000 mctech_cloud-1.0.1/mctech_cloud/header_filter.py
-drwxrwxrwx   0        0        0        0 2023-06-16 07:50:42.182492 mctech_cloud-1.0.1/mctech_cloud/middlewares/
--rw-rw-rw-   0        0        0      696 2023-06-16 07:43:18.000000 mctech_cloud-1.0.1/mctech_cloud/middlewares/__init__.py
--rw-rw-rw-   0        0        0     1429 2023-06-16 07:43:18.000000 mctech_cloud-1.0.1/mctech_cloud/middlewares/service_context_middleware.py
-drwxrwxrwx   0        0        0        0 2023-06-16 07:50:42.181491 mctech_cloud-1.0.1/mctech_cloud.egg-info/
--rw-rw-rw-   0        0        0       59 2023-06-16 07:50:42.000000 mctech_cloud-1.0.1/mctech_cloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-06-16 07:50:42.000000 mctech_cloud-1.0.1/mctech_cloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 07:50:42.000000 mctech_cloud-1.0.1/mctech_cloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-06-16 07:50:42.000000 mctech_cloud-1.0.1/mctech_cloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-16 07:50:42.000000 mctech_cloud-1.0.1/mctech_cloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      326 2023-06-16 07:43:18.000000 mctech_cloud-1.0.1/mctech_cloud_setup.py
--rw-rw-rw-   0        0        0       42 2023-06-16 07:50:42.184494 mctech_cloud-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-19 07:47:26.341568 mctech_cloud-1.0.2/
+-rw-rw-rw-   0        0        0      147 2023-07-19 07:47:26.339576 mctech_cloud-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      497 2023-07-19 07:47:00.000000 mctech_cloud-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 07:47:26.283381 mctech_cloud-1.0.2/mctech_cloud/
+-rw-rw-rw-   0        0        0       34 2022-10-08 03:15:48.000000 mctech_cloud-1.0.2/mctech_cloud/__init__.py
+-rw-rw-rw-   0        0        0     1930 2022-10-18 06:23:52.000000 mctech_cloud-1.0.2/mctech_cloud/app_server.py
+-rw-rw-rw-   0        0        0      927 2022-10-08 03:15:48.000000 mctech_cloud-1.0.2/mctech_cloud/header_filter.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:47:26.336569 mctech_cloud-1.0.2/mctech_cloud/middlewares/
+-rw-rw-rw-   0        0        0      674 2022-10-08 03:15:48.000000 mctech_cloud-1.0.2/mctech_cloud/middlewares/__init__.py
+-rw-rw-rw-   0        0        0     1385 2022-10-08 03:15:48.000000 mctech_cloud-1.0.2/mctech_cloud/middlewares/service_context_middleware.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:47:26.327566 mctech_cloud-1.0.2/mctech_cloud.egg-info/
+-rw-rw-rw-   0        0        0      147 2023-07-19 07:47:26.000000 mctech_cloud-1.0.2/mctech_cloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-07-19 07:47:26.000000 mctech_cloud-1.0.2/mctech_cloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 07:47:26.000000 mctech_cloud-1.0.2/mctech_cloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-07-19 07:47:26.000000 mctech_cloud-1.0.2/mctech_cloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-19 07:47:26.000000 mctech_cloud-1.0.2/mctech_cloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      355 2023-07-19 07:44:17.000000 mctech_cloud-1.0.2/mctech_cloud_setup.py
+-rw-rw-rw-   0        0        0       42 2023-07-19 07:47:26.341568 mctech_cloud-1.0.2/setup.cfg
```

### Comparing `mctech_cloud-1.0.1/mctech_cloud/app_server.py` & `mctech_cloud-1.0.2/mctech_cloud/app_server.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-import uvicorn
-import math
-
-from log4py import logging
-from fastapi import FastAPI
-from mctech_discovery.discovery import discovery_client, configure
-from . import middlewares
-
-log = logging.getLogger('python.cloud.appServer')
-
-
-def try_convert_number(val: str):
-    ret = int(val)
-    return val if math.isnan(ret)else ret
-
-
-def init_app_manager():
-    # log.info('开始初始化各部分组件......')
-    # #  配置合并完成，开始触发执行延迟初始化事件
-    # #  @ts-expect-error 未暴露方法
-    # appManager.onIniting(configure)
-    # log.info('组件初始化完成！')
-    pass
-
-
-class AppServer:
-    def __init__(self):
-        self._app = FastAPI()
-        self._converters = {
-            'x-tenant-id': try_convert_number,
-            'x-user-id': try_convert_number,
-            'x-id': try_convert_number,
-            'x-org-id': try_convert_number
-        }
-
-    @property
-    def app(self):
-        return self._app
-
-    def _init(self):
-        middlewares.create_actuator(configure, self._app)
-        init_app_manager()
-        middlewares.create_extras(self._converters, self._app)
-
-    def start(self):
-        # 启动eureka(当前应用不会注册到注册中心)
-        discovery_client.start()
-        #  通过注册中心找到配置服务，加载远程配置
-        discovery_client.load_config()
-        configure.merge()
-        #  初始化本地模块
-        self._init()
-        #  根据需要把当前应用注册到服务中心
-        discovery_client.register()
-
-        #  启动网站
-        info = configure.get_app_info()
-        port = info['port']
-
-        #  添加'0.0.0.0'的目的是要求ctx.ip返回的格式是ipv4
-        uvicorn.run(self._app, host="0.0.0.0", port=port, access_log=False)
-        if log.isInfoEnabled():
-            log.info("应用程序在端口 %s 启动完成." % port)
-
-    def stop(self):
-        discovery_client.unregister()
+import uvicorn
+import math
+
+from log4py import logging
+from fastapi import FastAPI
+from mctech_discovery.discovery import discovery_client, configure
+from . import middlewares
+
+log = logging.getLogger('python.cloud.appServer')
+
+
+def try_convert_number(val: str):
+    ret = int(val)
+    return val if math.isnan(ret)else ret
+
+
+def init_app_manager():
+    # log.info('开始初始化各部分组件......')
+    # #  配置合并完成，开始触发执行延迟初始化事件
+    # #  @ts-expect-error 未暴露方法
+    # appManager.onIniting(configure)
+    # log.info('组件初始化完成！')
+    pass
+
+
+class AppServer:
+    def __init__(self):
+        self._app = FastAPI()
+        self._converters = {
+            'x-tenant-id': try_convert_number,
+            'x-user-id': try_convert_number,
+            'x-id': try_convert_number,
+            'x-org-id': try_convert_number
+        }
+
+    @property
+    def app(self):
+        return self._app
+
+    def _init(self):
+        middlewares.create_actuator(configure, self._app)
+        init_app_manager()
+        middlewares.create_extras(self._converters, self._app)
+
+    def start(self):
+        # 启动eureka(当前应用不会注册到注册中心)
+        discovery_client.start()
+        #  通过注册中心找到配置服务，加载远程配置
+        discovery_client.load_config()
+        configure.merge()
+        #  初始化本地模块
+        self._init()
+        #  根据需要把当前应用注册到服务中心
+        discovery_client.register()
+
+        #  启动网站
+        info = configure.get_app_info()
+        port = info['port']
+
+        #  添加'0.0.0.0'的目的是要求ctx.ip返回的格式是ipv4
+        uvicorn.run(self._app, host="0.0.0.0", port=port, access_log=False)
+        if log.isInfoEnabled():
+            log.info("应用程序在端口 %s 启动完成." % port)
+
+    def stop(self):
+        discovery_client.unregister()
```

### Comparing `mctech_cloud-1.0.1/mctech_cloud/header_filter.py` & `mctech_cloud-1.0.2/mctech_cloud/header_filter.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from typing import List
-
-PATTERNS = [
-    {
-        'group': 'tracingHeaders',
-        'match': lambda name:
-        name == 'x-request-id' or name == 'x-ot-span-context'
-    },
-    {
-        'group': 'tracingHeaders',
-        'match': lambda name: name.startswith('x-b3-')
-    },
-    {
-        'group': 'miscHeaders',
-        'match': lambda name: name.startswith('x-forwarded-')
-    }]
-
-
-def process(headers: List):
-    result = {
-        # str[]
-        'tracingHeaders': [],
-        # str[]}
-        'extrasHeaders': [],
-        # str[]
-        'miscHeaders': []
-    }
-
-    # 排除所有不是以'x-'开头的key
-    for header in filter(lambda h: h.startswith('x-'), headers):
-        # 排除满足$excludes集合中条件的
-        pattern = next(filter(lambda p: p.match(header), PATTERNS), None)
-        group = pattern['group'] if pattern else 'extrasHeaders'
-        result[group].append(header)
-    return result
+from typing import List
+
+PATTERNS = [
+    {
+        'group': 'tracingHeaders',
+        'match': lambda name:
+        name == 'x-request-id' or name == 'x-ot-span-context'
+    },
+    {
+        'group': 'tracingHeaders',
+        'match': lambda name: name.startswith('x-b3-')
+    },
+    {
+        'group': 'miscHeaders',
+        'match': lambda name: name.startswith('x-forwarded-')
+    }]
+
+
+def process(headers: List):
+    result = {
+        # str[]
+        'tracingHeaders': [],
+        # str[]}
+        'extrasHeaders': [],
+        # str[]
+        'miscHeaders': []
+    }
+
+    # 排除所有不是以'x-'开头的key
+    for header in filter(lambda h: h.startswith('x-'), headers):
+        # 排除满足$excludes集合中条件的
+        pattern = next(filter(lambda p: p.match(header), PATTERNS), None)
+        group = pattern['group'] if pattern else 'extrasHeaders'
+        result[group].append(header)
+    return result
```

### Comparing `mctech_cloud-1.0.1/mctech_cloud/middlewares/__init__.py` & `mctech_cloud-1.0.2/mctech_cloud/middlewares/__init__.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from .service_context_middleware import ServiceContextMiddleware
-from log4py import logging
-from fastapi import FastAPI
-from mctech_actuator import create_actuator_route
-
-log = logging.getLogger('python.cloud.middlewares')
-
-
-def create_extras(converters, app: FastAPI):
-    """创建构建extras的middleware
-    """
-    app.add_middleware(ServiceContextMiddleware, converters=converters)
-    log.info('创建extras context middleware完成')
-
-
-def create_actuator(configure, app: FastAPI):
-    """创建用于Actuator服务治理相关api的router
-    """
-
-    # 设置actuator的router
-    create_actuator_route(configure, app)
-    log.info('创建actuator router完成')
+from .service_context_middleware import ServiceContextMiddleware
+from log4py import logging
+from fastapi import FastAPI
+from mctech_actuator import create_actuator_route
+
+log = logging.getLogger('python.cloud.middlewares')
+
+
+def create_extras(converters, app: FastAPI):
+    """创建构建extras的middleware
+    """
+    app.add_middleware(ServiceContextMiddleware, converters=converters)
+    log.info('创建extras context middleware完成')
+
+
+def create_actuator(configure, app: FastAPI):
+    """创建用于Actuator服务治理相关api的router
+    """
+
+    # 设置actuator的router
+    create_actuator_route(configure, app)
+    log.info('创建actuator router完成')
```

### Comparing `mctech_cloud-1.0.1/mctech_cloud/middlewares/service_context_middleware.py` & `mctech_cloud-1.0.2/mctech_cloud/middlewares/service_context_middleware.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import re
-from starlette.datastructures import Headers
-from starlette.types import Receive, Scope, Send
-from .. import header_filter as filter
-
-pattern = re.compile('-([a-z])', re.IGNORECASE)
-
-
-class ServiceContextMiddleware:
-    def __init__(self, app, converters):
-        self._app = app
-        self._converters = converters
-
-    async def __call__(self, scope: Scope, receive: Receive, send: Send):
-        headers = Headers(scope=scope)
-        headerNames = headers.keys()
-        processors = filter.process(headerNames)
-        tracingHeaders = processors['tracingHeaders']
-        extrasHeaders = processors['extrasHeaders']
-
-        tracing = {}
-        for header_name in tracingHeaders:
-            tracing[header_name] = headers[header_name]
-        scope['tracing'] = tracing
-
-        extras = {}
-        for header_name in extrasHeaders:
-            self._resolve_extras_value(extras, headers, header_name)
-
-        scope['extras'] = extras
-        await self._app(scope, receive, send)
-
-    def _resolve_extras_value(self, extras: dict, headers: Headers, name: str):
-        key = pattern.sub(to_upper, name.replace('x-', ''))
-        converter = self._converters.get(name)
-        value = headers[name]
-        if converter:
-            value = converter(value)
-        extras[key] = value
-
-
-def to_upper(matched):
-    text = matched.group(1)
-    return text.upper()
+import re
+from starlette.datastructures import Headers
+from starlette.types import Receive, Scope, Send
+from .. import header_filter as filter
+
+pattern = re.compile('-([a-z])', re.IGNORECASE)
+
+
+class ServiceContextMiddleware:
+    def __init__(self, app, converters):
+        self._app = app
+        self._converters = converters
+
+    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+        headers = Headers(scope=scope)
+        headerNames = headers.keys()
+        processors = filter.process(headerNames)
+        tracingHeaders = processors['tracingHeaders']
+        extrasHeaders = processors['extrasHeaders']
+
+        tracing = {}
+        for header_name in tracingHeaders:
+            tracing[header_name] = headers[header_name]
+        scope['tracing'] = tracing
+
+        extras = {}
+        for header_name in extrasHeaders:
+            self._resolve_extras_value(extras, headers, header_name)
+
+        scope['extras'] = extras
+        await self._app(scope, receive, send)
+
+    def _resolve_extras_value(self, extras: dict, headers: Headers, name: str):
+        key = pattern.sub(to_upper, name.replace('x-', ''))
+        converter = self._converters.get(name)
+        value = headers[name]
+        if converter:
+            value = converter(value)
+        extras[key] = value
+
+
+def to_upper(matched):
+    text = matched.group(1)
+    return text.upper()
```

