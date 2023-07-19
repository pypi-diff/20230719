# Comparing `tmp/mctech_actuator-1.0.3.tar.gz` & `tmp/mctech_actuator-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mctech_actuator-1.0.3.tar", last modified: Fri Jun 16 07:48:23 2023, max compression
+gzip compressed data, was "mctech_actuator-1.0.4.tar", last modified: Wed Jul 19 07:58:46 2023, max compression
```

## Comparing `mctech_actuator-1.0.3.tar` & `mctech_actuator-1.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 07:48:23.806776 mctech_actuator-1.0.3/
--rw-rw-rw-   0        0        0       62 2023-06-16 07:48:23.805774 mctech_actuator-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      529 2023-06-16 07:43:18.000000 mctech_actuator-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 07:48:23.773434 mctech_actuator-1.0.3/mctech_actuator/
--rw-rw-rw-   0        0        0      391 2023-06-16 07:43:18.000000 mctech_actuator-1.0.3/mctech_actuator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 07:48:23.796184 mctech_actuator-1.0.3/mctech_actuator/actuator/
--rw-rw-rw-   0        0        0        0 2023-06-16 07:43:18.000000 mctech_actuator-1.0.3/mctech_actuator/actuator/__init__.py
--rw-rw-rw-   0        0        0     1205 2023-06-16 07:43:18.000000 mctech_actuator-1.0.3/mctech_actuator/actuator/actuator_router.py
-drwxrwxrwx   0        0        0        0 2023-06-16 07:48:23.800189 mctech_actuator-1.0.3/mctech_actuator/actuator/route/
--rw-rw-rw-   0        0        0        0 2023-06-16 07:43:18.000000 mctech_actuator-1.0.3/mctech_actuator/actuator/route/__init__.py
--rw-rw-rw-   0        0        0      439 2023-06-16 07:43:18.000000 mctech_actuator-1.0.3/mctech_actuator/actuator/route/health_route.py
--rw-rw-rw-   0        0        0      213 2023-06-16 07:43:18.000000 mctech_actuator-1.0.3/mctech_actuator/actuator/route/info_route.py
--rw-rw-rw-   0        0        0      229 2023-06-16 07:43:18.000000 mctech_actuator-1.0.3/mctech_actuator/actuator/route/metrics_routes.py
-drwxrwxrwx   0        0        0        0 2023-06-16 07:48:23.804770 mctech_actuator-1.0.3/mctech_actuator/health/
--rw-rw-rw-   0        0        0      173 2023-06-16 07:43:18.000000 mctech_actuator-1.0.3/mctech_actuator/health/__init__.py
--rw-rw-rw-   0        0        0     2036 2023-06-16 07:43:18.000000 mctech_actuator-1.0.3/mctech_actuator/health/composite_health_indicator.py
--rw-rw-rw-   0        0        0     2582 2023-06-16 07:43:18.000000 mctech_actuator-1.0.3/mctech_actuator/health/health.py
--rw-rw-rw-   0        0        0      936 2023-06-16 07:43:18.000000 mctech_actuator-1.0.3/mctech_actuator/health/health_manager.py
--rw-rw-rw-   0        0        0      169 2023-06-16 07:43:18.000000 mctech_actuator-1.0.3/mctech_actuator/health/indicator.py
-drwxrwxrwx   0        0        0        0 2023-06-16 07:48:23.794183 mctech_actuator-1.0.3/mctech_actuator.egg-info/
--rw-rw-rw-   0        0        0       62 2023-06-16 07:48:23.000000 mctech_actuator-1.0.3/mctech_actuator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      719 2023-06-16 07:48:23.000000 mctech_actuator-1.0.3/mctech_actuator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 07:48:23.000000 mctech_actuator-1.0.3/mctech_actuator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-16 07:48:23.000000 mctech_actuator-1.0.3/mctech_actuator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-16 07:48:23.000000 mctech_actuator-1.0.3/mctech_actuator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      257 2023-06-16 07:43:18.000000 mctech_actuator-1.0.3/mctech_actuator_setup.py
--rw-rw-rw-   0        0        0       42 2023-06-16 07:48:23.806776 mctech_actuator-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-19 07:58:46.572762 mctech_actuator-1.0.4/
+-rw-rw-rw-   0        0        0      150 2023-07-19 07:58:46.571750 mctech_actuator-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      497 2023-07-19 07:47:00.000000 mctech_actuator-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 07:58:46.465205 mctech_actuator-1.0.4/mctech_actuator/
+-rw-rw-rw-   0        0        0      373 2022-10-08 03:15:48.000000 mctech_actuator-1.0.4/mctech_actuator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:58:46.527203 mctech_actuator-1.0.4/mctech_actuator/actuator/
+-rw-rw-rw-   0        0        0        0 2023-05-12 06:58:39.000000 mctech_actuator-1.0.4/mctech_actuator/actuator/__init__.py
+-rw-rw-rw-   0        0        0     1175 2023-05-12 08:46:37.000000 mctech_actuator-1.0.4/mctech_actuator/actuator/actuator_router.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:58:46.541202 mctech_actuator-1.0.4/mctech_actuator/actuator/route/
+-rw-rw-rw-   0        0        0        0 2023-05-12 06:58:39.000000 mctech_actuator-1.0.4/mctech_actuator/actuator/route/__init__.py
+-rw-rw-rw-   0        0        0      421 2022-10-08 03:15:48.000000 mctech_actuator-1.0.4/mctech_actuator/actuator/route/health_route.py
+-rw-rw-rw-   0        0        0      203 2022-10-08 03:15:48.000000 mctech_actuator-1.0.4/mctech_actuator/actuator/route/info_route.py
+-rw-rw-rw-   0        0        0      219 2023-05-12 08:22:20.000000 mctech_actuator-1.0.4/mctech_actuator/actuator/route/metrics_routes.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:58:46.568750 mctech_actuator-1.0.4/mctech_actuator/health/
+-rw-rw-rw-   0        0        0      169 2022-10-08 03:15:48.000000 mctech_actuator-1.0.4/mctech_actuator/health/__init__.py
+-rw-rw-rw-   0        0        0     1971 2023-05-12 06:58:39.000000 mctech_actuator-1.0.4/mctech_actuator/health/composite_health_indicator.py
+-rw-rw-rw-   0        0        0     2484 2022-10-08 03:15:48.000000 mctech_actuator-1.0.4/mctech_actuator/health/health.py
+-rw-rw-rw-   0        0        0      899 2023-05-12 06:58:39.000000 mctech_actuator-1.0.4/mctech_actuator/health/health_manager.py
+-rw-rw-rw-   0        0        0      157 2022-10-08 03:15:48.000000 mctech_actuator-1.0.4/mctech_actuator/health/indicator.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:58:46.504204 mctech_actuator-1.0.4/mctech_actuator.egg-info/
+-rw-rw-rw-   0        0        0      150 2023-07-19 07:58:46.000000 mctech_actuator-1.0.4/mctech_actuator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      719 2023-07-19 07:58:46.000000 mctech_actuator-1.0.4/mctech_actuator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 07:58:46.000000 mctech_actuator-1.0.4/mctech_actuator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-19 07:58:46.000000 mctech_actuator-1.0.4/mctech_actuator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-19 07:58:46.000000 mctech_actuator-1.0.4/mctech_actuator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      284 2023-07-19 07:58:45.000000 mctech_actuator-1.0.4/mctech_actuator_setup.py
+-rw-rw-rw-   0        0        0       42 2023-07-19 07:58:46.573755 mctech_actuator-1.0.4/setup.cfg
```

### Comparing `mctech_actuator-1.0.3/mctech_actuator/actuator/actuator_router.py` & `mctech_actuator-1.0.4/mctech_actuator/actuator/actuator_router.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-
-from fastapi import FastAPI
-from fastapi.responses import PlainTextResponse
-from .route.info_route import create_info_route
-from .route.health_route import create_health_route
-from .route.metrics_routes import create_metrics_routers
-
-
-def create_actuator_route(configure, app: FastAPI):
-    async def empty():
-        res = PlainTextResponse('Actuator Not Found')
-        res.status_code = 404
-        return res
-
-    management = configure.get_config('management')
-    prefix = management.get('context-path') or \
-        management.get('contextPath') or '/actuator'
-
-    app.add_api_route(f"{prefix}/info", endpoint=create_info_route(configure))
-    app.add_api_route(f"{prefix}/health",
-                      endpoint=create_health_route(configure))
-    app.add_api_route(f"{prefix}/env", endpoint=empty)
-    app.add_api_route(f"{prefix}/shutdown", endpoint=empty)
-
-    app.add_api_route(f"{prefix}/loggers", endpoint=empty)
-    app.add_api_route(f"{prefix}/loggers", endpoint=empty)
-    app.add_api_route(f"{prefix}/loggers/:category", endpoint=empty)
-
-    for path, endpoint in create_metrics_routers():
-        app.add_api_route(f"{prefix}/{path}", endpoint=endpoint)
+
+from fastapi import FastAPI
+from fastapi.responses import PlainTextResponse
+from .route.info_route import create_info_route
+from .route.health_route import create_health_route
+from .route.metrics_routes import create_metrics_routers
+
+
+def create_actuator_route(configure, app: FastAPI):
+    async def empty():
+        res = PlainTextResponse('Actuator Not Found')
+        res.status_code = 404
+        return res
+
+    management = configure.get_config('management')
+    prefix = management.get('context-path') or \
+        management.get('contextPath') or '/actuator'
+
+    app.add_api_route(f"{prefix}/info", endpoint=create_info_route(configure))
+    app.add_api_route(f"{prefix}/health",
+                      endpoint=create_health_route(configure))
+    app.add_api_route(f"{prefix}/env", endpoint=empty)
+    app.add_api_route(f"{prefix}/shutdown", endpoint=empty)
+
+    app.add_api_route(f"{prefix}/loggers", endpoint=empty)
+    app.add_api_route(f"{prefix}/loggers", endpoint=empty)
+    app.add_api_route(f"{prefix}/loggers/:category", endpoint=empty)
+
+    for path, endpoint in create_metrics_routers():
+        app.add_api_route(f"{prefix}/{path}", endpoint=endpoint)
```

### Comparing `mctech_actuator-1.0.3/mctech_actuator/health/health.py` & `mctech_actuator-1.0.4/mctech_actuator/health/health.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-from typing import Any, Union
-
-
-class Status:
-    def __init__(self, code: int, description: str):
-        self.code = code
-        self.description = description
-
-    def compareTo(self, s):
-        if self == s:
-            return 0
-
-        if not s:
-            return 1
-        if self.code < s.code:
-            return -1
-        elif self.code < s.code:
-            return 1
-        return 0
-
-
-Status.UP = 'UP'
-Status.DOWN = 'DOWN'
-Status.SARTING = 'STARTING'
-Status.OUT_OF_SERVICE = 'OUT_OF_SERVICE'
-Status.UNKNOWN = 'UNKNOWN'
-
-
-class Health:
-    def __init__(self, status: Status, details: dict):
-        self.status = status
-        self.details = dict(details) if details else {}
-
-    def to_json(self):
-        json = {
-            'status': self.status.code,
-            'description': self.status.description
-        }
-
-        for key, value in self.details.items():
-            if 'to_json' in value:
-                json[key] = value.to_json()
-            else:
-                json[key] = value
-        return json
-
-    @staticmethod
-    def unknown(description: str):
-        status = Status(Status.UNKNOWN, description)
-        return HealthBuilder(status)
-
-    @staticmethod
-    def down(description: str):
-        status = Status(Status.DOWN, description)
-        return HealthBuilder(status)
-
-    @staticmethod
-    def up(description: str):
-        status = Status(Status.UP, description)
-        return HealthBuilder(status)
-
-    @staticmethod
-    def out_of_service(description: str):
-        status = Status(Status.OUT_OF_SERVICE, description)
-        return HealthBuilder(status)
-
-    @staticmethod
-    def status(code: str, description: str):
-        _status = Status(code, description)
-        return HealthBuilder(_status)
-
-
-class HealthBuilder:
-    def __init__(self, status: Union[str, Status], details):
-        self.status(status)
-        self._details = dict(details) if details else {}
-
-    def status(self, status: Union[str, Status] = None):
-        if status:
-            if isinstance(status, Status):
-                self._status = status
-            else:
-                self._status = Status(status)
-        return self
-
-    def down(self, message: str):
-        self._status = Status(Status.DOWN, message)
-        return self
-
-    def add_detail(self, name: str, item: Any):
-        self._details.set(name, item)
-        return self
-
-    def build(self):
-        return Health(self._status, self._details)
-
-
-Health.Builder = HealthBuilder
+from typing import Any, Union
+
+
+class Status:
+    def __init__(self, code: int, description: str):
+        self.code = code
+        self.description = description
+
+    def compareTo(self, s):
+        if self == s:
+            return 0
+
+        if not s:
+            return 1
+        if self.code < s.code:
+            return -1
+        elif self.code < s.code:
+            return 1
+        return 0
+
+
+Status.UP = 'UP'
+Status.DOWN = 'DOWN'
+Status.SARTING = 'STARTING'
+Status.OUT_OF_SERVICE = 'OUT_OF_SERVICE'
+Status.UNKNOWN = 'UNKNOWN'
+
+
+class Health:
+    def __init__(self, status: Status, details: dict):
+        self.status = status
+        self.details = dict(details) if details else {}
+
+    def to_json(self):
+        json = {
+            'status': self.status.code,
+            'description': self.status.description
+        }
+
+        for key, value in self.details.items():
+            if 'to_json' in value:
+                json[key] = value.to_json()
+            else:
+                json[key] = value
+        return json
+
+    @staticmethod
+    def unknown(description: str):
+        status = Status(Status.UNKNOWN, description)
+        return HealthBuilder(status)
+
+    @staticmethod
+    def down(description: str):
+        status = Status(Status.DOWN, description)
+        return HealthBuilder(status)
+
+    @staticmethod
+    def up(description: str):
+        status = Status(Status.UP, description)
+        return HealthBuilder(status)
+
+    @staticmethod
+    def out_of_service(description: str):
+        status = Status(Status.OUT_OF_SERVICE, description)
+        return HealthBuilder(status)
+
+    @staticmethod
+    def status(code: str, description: str):
+        _status = Status(code, description)
+        return HealthBuilder(_status)
+
+
+class HealthBuilder:
+    def __init__(self, status: Union[str, Status], details):
+        self.status(status)
+        self._details = dict(details) if details else {}
+
+    def status(self, status: Union[str, Status] = None):
+        if status:
+            if isinstance(status, Status):
+                self._status = status
+            else:
+                self._status = Status(status)
+        return self
+
+    def down(self, message: str):
+        self._status = Status(Status.DOWN, message)
+        return self
+
+    def add_detail(self, name: str, item: Any):
+        self._details.set(name, item)
+        return self
+
+    def build(self):
+        return Health(self._status, self._details)
+
+
+Health.Builder = HealthBuilder
```

### Comparing `mctech_actuator-1.0.3/mctech_actuator/health/health_manager.py` & `mctech_actuator-1.0.4/mctech_actuator/health/health_manager.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from .composite_health_indicator import CompositeHealthIndicator
-from .health import Health
-
-
-class HealthManager:
-    def __init__(self):
-        self._indicator = CompositeHealthIndicator()
-        self._metrics = []
-
-    def get_metrics(self):
-        return self._metrics
-
-    def add_metric(self, metric):
-        self._metrics.append(metric)
-
-    def get_health(self):
-        return self._indicator.health()
-
-    def add_indicator(self, indicator):
-        holder = IndicatorHolder(indicator)
-        self._indicator.add_indicator(indicator.name, holder)
-
-
-class IndicatorHolder:
-    def __init__(self, indicator):
-        self.name = None
-        self.indicator = indicator
-
-    def health(self):
-        try:
-            h = self.indicator.health()
-        except RuntimeError as e:
-            h = Health.down(e.name + ':' + e.message).build()
-        return h
-
-
-manager = HealthManager()
+from .composite_health_indicator import CompositeHealthIndicator
+from .health import Health
+
+
+class HealthManager:
+    def __init__(self):
+        self._indicator = CompositeHealthIndicator()
+        self._metrics = []
+
+    def get_metrics(self):
+        return self._metrics
+
+    def add_metric(self, metric):
+        self._metrics.append(metric)
+
+    def get_health(self):
+        return self._indicator.health()
+
+    def add_indicator(self, indicator):
+        holder = IndicatorHolder(indicator)
+        self._indicator.add_indicator(indicator.name, holder)
+
+
+class IndicatorHolder:
+    def __init__(self, indicator):
+        self.name = None
+        self.indicator = indicator
+
+    def health(self):
+        try:
+            h = self.indicator.health()
+        except RuntimeError as e:
+            h = Health.down(e.name + ':' + e.message).build()
+        return h
+
+
+manager = HealthManager()
```

### Comparing `mctech_actuator-1.0.3/mctech_actuator.egg-info/SOURCES.txt` & `mctech_actuator-1.0.4/mctech_actuator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

