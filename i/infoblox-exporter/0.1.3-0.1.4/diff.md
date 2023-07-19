# Comparing `tmp/infoblox-exporter-0.1.3.tar.gz` & `tmp/infoblox-exporter-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infoblox-exporter-0.1.3.tar", last modified: Tue Jul 18 15:13:26 2023, max compression
+gzip compressed data, was "infoblox-exporter-0.1.4.tar", last modified: Wed Jul 19 08:46:23 2023, max compression
```

## Comparing `infoblox-exporter-0.1.3.tar` & `infoblox-exporter-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:13:26.206365 infoblox-exporter-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34570 2023-07-18 15:12:52.000000 infoblox-exporter-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-18 15:13:26.202365 infoblox-exporter-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-18 15:12:52.000000 infoblox-exporter-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:13:26.202365 infoblox-exporter-0.1.3/infoblox_exporter/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-18 15:12:52.000000 infoblox-exporter-0.1.3/infoblox_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-18 15:12:52.000000 infoblox-exporter-0.1.3/infoblox_exporter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-18 15:12:52.000000 infoblox-exporter-0.1.3/infoblox_exporter/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-18 15:12:52.000000 infoblox-exporter-0.1.3/infoblox_exporter/dhcp_utilization.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-18 15:12:52.000000 infoblox-exporter-0.1.3/infoblox_exporter/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-18 15:12:52.000000 infoblox-exporter-0.1.3/infoblox_exporter/infoblox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-18 15:12:52.000000 infoblox-exporter-0.1.3/infoblox_exporter/infoblox_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-07-18 15:12:52.000000 infoblox-exporter-0.1.3/infoblox_exporter/node_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-07-18 15:12:52.000000 infoblox-exporter-0.1.3/infoblox_exporter/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-18 15:12:52.000000 infoblox-exporter-0.1.3/infoblox_exporter/server_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-18 15:12:52.000000 infoblox-exporter-0.1.3/infoblox_exporter/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:13:26.202365 infoblox-exporter-0.1.3/infoblox_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-18 15:13:26.000000 infoblox-exporter-0.1.3/infoblox_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-18 15:13:26.000000 infoblox-exporter-0.1.3/infoblox_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:13:26.000000 infoblox-exporter-0.1.3/infoblox_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:13:26.000000 infoblox-exporter-0.1.3/infoblox_exporter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-18 15:13:26.000000 infoblox-exporter-0.1.3/infoblox_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-18 15:13:26.000000 infoblox-exporter-0.1.3/infoblox_exporter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 15:13:26.206365 infoblox-exporter-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-18 15:12:52.000000 infoblox-exporter-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:13:26.202365 infoblox-exporter-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-18 15:12:52.000000 infoblox-exporter-0.1.3/tests/test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:46:23.051273 infoblox-exporter-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34570 2023-07-19 08:45:39.000000 infoblox-exporter-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-07-19 08:46:23.051273 infoblox-exporter-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10287 2023-07-19 08:45:39.000000 infoblox-exporter-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:46:23.047273 infoblox-exporter-0.1.4/infoblox_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-19 08:45:39.000000 infoblox-exporter-0.1.4/infoblox_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-19 08:45:39.000000 infoblox-exporter-0.1.4/infoblox_exporter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-19 08:45:39.000000 infoblox-exporter-0.1.4/infoblox_exporter/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-19 08:45:39.000000 infoblox-exporter-0.1.4/infoblox_exporter/dhcp_utilization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-19 08:45:39.000000 infoblox-exporter-0.1.4/infoblox_exporter/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-19 08:45:39.000000 infoblox-exporter-0.1.4/infoblox_exporter/infoblox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-19 08:45:39.000000 infoblox-exporter-0.1.4/infoblox_exporter/infoblox_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-07-19 08:45:39.000000 infoblox-exporter-0.1.4/infoblox_exporter/node_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-07-19 08:45:39.000000 infoblox-exporter-0.1.4/infoblox_exporter/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-19 08:45:39.000000 infoblox-exporter-0.1.4/infoblox_exporter/server_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-19 08:45:39.000000 infoblox-exporter-0.1.4/infoblox_exporter/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:46:23.051273 infoblox-exporter-0.1.4/infoblox_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-07-19 08:46:23.000000 infoblox-exporter-0.1.4/infoblox_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-19 08:46:23.000000 infoblox-exporter-0.1.4/infoblox_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 08:46:23.000000 infoblox-exporter-0.1.4/infoblox_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 08:46:23.000000 infoblox-exporter-0.1.4/infoblox_exporter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-19 08:46:23.000000 infoblox-exporter-0.1.4/infoblox_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-19 08:46:23.000000 infoblox-exporter-0.1.4/infoblox_exporter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 08:46:23.051273 infoblox-exporter-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-19 08:45:39.000000 infoblox-exporter-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:46:23.051273 infoblox-exporter-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-19 08:45:39.000000 infoblox-exporter-0.1.4/tests/test_dummy.py
```

### Comparing `infoblox-exporter-0.1.3/LICENSE` & `infoblox-exporter-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `infoblox-exporter-0.1.3/infoblox_exporter/__init__.py` & `infoblox-exporter-0.1.4/infoblox_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `infoblox-exporter-0.1.3/infoblox_exporter/__main__.py` & `infoblox-exporter-0.1.4/infoblox_exporter/__main__.py`

 * *Files identical despite different names*

### Comparing `infoblox-exporter-0.1.3/infoblox_exporter/api.py` & `infoblox-exporter-0.1.4/infoblox_exporter/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,10 +64,8 @@
 
     async def get_infoblox_dhcp_utilization(self, network: str) -> int:
         try:
             return_fields_range = ['network', 'dhcp_utilization', 'dhcp_utilization_status']
             range = self.conn.get_object('range', {'network': network}, return_fields=return_fields_range)
             return range[0]['dhcp_utilization']
         except Exception as err:
-            raise InfobloxException("Not a valid network",status=400)
-
-
+            raise InfobloxException("Not a valid network", status=400)
```

### Comparing `infoblox-exporter-0.1.3/infoblox_exporter/dhcp_utilization.py` & `infoblox-exporter-0.1.4/infoblox_exporter/dhcp_utilization.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,18 +15,19 @@
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with infoblox_exporter.  If not, see <http://www.gnu.org/licenses/>.
 
 """
 
-from typing import Dict, Any, List
+import logging
+
 from prometheus_client.core import GaugeMetricFamily
+
 from infoblox_exporter.transform import Transform
-import logging
 
 
 class DHCPUtilization(Transform):
     prefix = "infoblox_"
 
     def __init__(self, network: str, utilization: int):
         super().__init__()
```

### Comparing `infoblox-exporter-0.1.3/infoblox_exporter/exceptions.py` & `infoblox-exporter-0.1.4/infoblox_exporter/exceptions.py`

 * *Files identical despite different names*

### Comparing `infoblox-exporter-0.1.3/infoblox_exporter/infoblox.py` & `infoblox-exporter-0.1.4/infoblox_exporter/infoblox.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,46 +35,46 @@
 from infoblox_exporter.node_info import NodeInfo
 from infoblox_exporter.dhcp_utilization import DHCPUtilization
 
 disable_warnings(InsecureRequestWarning)
 
 
 class Modules(Enum):
-    NODES = 'nodes'
+    MEMBER_SERVICES = 'member_services'
     DHCP_UTILIZATION = 'dhcp_utilization'
 
 
 def to_list(metric_generator):
     metrics = []
     for metric in metric_generator:
         if metric.samples:
             # Only append if the metric has a list of Samples
             metrics.append(metric)
     return metrics
 
 
 class InfobloxCollector:
-    def __init__(self, connection: Dict[str, str], target: str, module: str = Modules.NODES.value):
+    def __init__(self, connection: Dict[str, str], target: str, module: str = Modules.MEMBER_SERVICES.value):
         self.target = target
         self.module = module
         self.connector = InfoBlox(connection)
 
     async def collect(self):
         start = time.perf_counter()
         all_module_metrics = []
         status = {"up": 1}
         try:
             all_tasks = []
 
-            if self.module == Modules.NODES.value:
+            if self.module == Modules.MEMBER_SERVICES.value:
                 all_tasks.append(asyncio.create_task(self._collect_node_info()))
             elif self.module == Modules.DHCP_UTILIZATION.value:
                 all_tasks.append(asyncio.create_task(self._collect_dhcp_ranges()))
             else:
-                raise InfobloxException(message=f"Not a valid module {self.module}",status=400)
+                raise InfobloxException(message=f"Not a valid module {self.module}", status=400)
 
             await asyncio.gather(*all_tasks)
             for task in all_tasks:
                 all_module_metrics.extend(task.result())
 
         except InfobloxException as err:
             status['up'] = 0
```

### Comparing `infoblox-exporter-0.1.3/infoblox_exporter/infoblox_status.py` & `infoblox-exporter-0.1.4/infoblox_exporter/infoblox_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,18 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with fortigate_exporter.  If not, see <http://www.gnu.org/licenses/>.
 
 """
-import logging
 from typing import Dict, Any
 
 from prometheus_client import Metric
-from prometheus_client.core import CounterMetricFamily, GaugeMetricFamily
+from prometheus_client.core import GaugeMetricFamily
 
 from infoblox_exporter.transform import Transform, LabelsBase
 
 
 class Config:
     prefix = 'infoblox_'
     help_prefix = ''
```

### Comparing `infoblox-exporter-0.1.3/infoblox_exporter/node_info.py` & `infoblox-exporter-0.1.4/infoblox_exporter/node_info.py`

 * *Files identical despite different names*

### Comparing `infoblox-exporter-0.1.3/infoblox_exporter/proxy.py` & `infoblox-exporter-0.1.4/infoblox_exporter/proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                 "mapping": {"level": "levelname", "timestamp": "asctime"},
                 "datefmt": TIME_FORMAT
             }
         },
         "handlers": {
             "console": {"class": "logging.StreamHandler", "formatter": "logfmt"}
         },
-        "loggers": {"": {"handlers": ["console"], "level": "INFO"}},
+        "loggers": {"": {"handlers": ["console"], "level": os.getenv('EXPORTER_LOG_LEVEL', 'INFO')}},
     }
 )
 
 app = FastAPI()
 security = HTTPBasic()
 global_settings = Settings()
 
@@ -187,26 +187,26 @@
 
 @app.get('/')
 def alive():
     return Response("infoblox_exporter alive!", status_code=200, media_type=MIME_TYPE)
 
 
 @app.get("/probe")
-async def probe(target: str, type: str):
+async def probe(target: str, module: str, auth: str = Depends(authorize)):
     start_time = time.time()
 
     if not target or target == "":
         return Response("Target must be specified", status_code=400, media_type=MIME_TYPE)
 
     # If target do not include a port number
 
     registry = CollectorRegistry()
     try:
 
-        collector = InfobloxCollector(connection=global_settings.infoblox, target=target, module=type)
+        collector = InfobloxCollector(connection=global_settings.infoblox, target=target, module=module)
         registry.register(collector)
 
         duration = Gauge('infoblox_scrape_duration_seconds', 'Time spent processing request', registry=registry)
 
         duration.set(time.time() - start_time)
 
         infoblox_response = generate_latest(await collector.collect())
```

### Comparing `infoblox-exporter-0.1.3/infoblox_exporter/server_config.py` & `infoblox-exporter-0.1.4/infoblox_exporter/server_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 import logging
 from functools import lru_cache
 
 from pydantic import AnyUrl, BaseSettings
 
 
 class Settings(BaseSettings):
-    basic_auth_username: str = os.getenv("BASIC_AUTH_USERNAME", "mother")
-    basic_auth_password: str = os.getenv("BASIC_AUTH_PASSWORD", "mother")
+    basic_auth_username: str = os.getenv("BASIC_AUTH_USERNAME")
+    basic_auth_password: str = os.getenv("BASIC_AUTH_PASSWORD")
     infoblox = {"master": os.getenv("INFOBLOX_MASTER"),
                 "wapi_version": os.getenv("INFOBLOX_WAPI_VERSION"),
                 "username": os.getenv("INFOBLOX_USERNAME"),
                 "password": os.getenv("INFOBLOX_PASSWORD")}
 
 
 @lru_cache()
```

### Comparing `infoblox-exporter-0.1.3/infoblox_exporter/transform.py` & `infoblox-exporter-0.1.4/infoblox_exporter/transform.py`

 * *Files identical despite different names*

### Comparing `infoblox-exporter-0.1.3/infoblox_exporter.egg-info/SOURCES.txt` & `infoblox-exporter-0.1.4/infoblox_exporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `infoblox-exporter-0.1.3/setup.py` & `infoblox-exporter-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `infoblox-exporter-0.1.3/tests/test_dummy.py` & `infoblox-exporter-0.1.4/tests/test_dummy.py`

 * *Files identical despite different names*

