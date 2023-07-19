# Comparing `tmp/mctech_discovery-1.0.4.tar.gz` & `tmp/mctech_discovery-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mctech_discovery-1.0.4.tar", last modified: Mon Jul 17 15:49:07 2023, max compression
+gzip compressed data, was "mctech_discovery-1.0.5.tar", last modified: Wed Jul 19 07:47:33 2023, max compression
```

## Comparing `mctech_discovery-1.0.4.tar` & `mctech_discovery-1.0.5.tar`

### file list

```diff
@@ -1,47 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 15:49:07.089281 mctech_discovery-1.0.4/
--rw-rw-rw-   0        0        0       63 2023-07-17 15:49:07.089281 mctech_discovery-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      461 2023-07-17 15:12:11.000000 mctech_discovery-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 15:49:06.977282 mctech_discovery-1.0.4/mctech_discovery/
--rw-rw-rw-   0        0        0        0 2020-05-31 14:29:40.000000 mctech_discovery-1.0.4/mctech_discovery/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:49:07.017286 mctech_discovery-1.0.4/mctech_discovery/config/
--rw-rw-rw-   0        0        0     1016 2022-02-12 12:24:55.000000 mctech_discovery-1.0.4/mctech_discovery/config/__init__.py
--rw-rw-rw-   0        0        0     8183 2023-02-24 15:34:39.000000 mctech_discovery-1.0.4/mctech_discovery/config/_configure.py
--rw-rw-rw-   0        0        0     8384 2023-04-26 15:25:28.000000 mctech_discovery-1.0.4/mctech_discovery/config/config_merger.py
--rw-rw-rw-   0        0        0     1997 2021-12-09 13:36:01.000000 mctech_discovery-1.0.4/mctech_discovery/config/config_value.py
--rw-rw-rw-   0        0        0     1464 2023-04-26 15:25:28.000000 mctech_discovery-1.0.4/mctech_discovery/config/yaml_loader.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:49:07.025286 mctech_discovery-1.0.4/mctech_discovery/discovery/
--rw-rw-rw-   0        0        0     1471 2021-12-09 13:36:01.000000 mctech_discovery-1.0.4/mctech_discovery/discovery/__init__.py
--rw-rw-rw-   0        0        0     8996 2023-02-24 15:34:39.000000 mctech_discovery-1.0.4/mctech_discovery/discovery/eureka_discovery_client.py
--rw-rw-rw-   0        0        0      868 2022-01-28 07:17:21.000000 mctech_discovery-1.0.4/mctech_discovery/discovery/local_discovery_client.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:49:07.033289 mctech_discovery-1.0.4/mctech_discovery/lifecycle/
--rw-rw-rw-   0        0        0        0 2022-02-12 07:46:11.000000 mctech_discovery-1.0.4/mctech_discovery/lifecycle/__init__.py
--rw-rw-rw-   0        0        0     1141 2023-07-17 15:48:30.000000 mctech_discovery-1.0.4/mctech_discovery/lifecycle/lifecycle.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:49:07.041283 mctech_discovery-1.0.4/mctech_discovery/rpc/
--rw-rw-rw-   0        0        0       71 2022-02-12 09:07:25.000000 mctech_discovery-1.0.4/mctech_discovery/rpc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:49:07.057280 mctech_discovery-1.0.4/mctech_discovery/rpc/ep/
--rw-rw-rw-   0        0        0        0 2020-05-31 07:53:09.000000 mctech_discovery-1.0.4/mctech_discovery/rpc/ep/__init__.py
--rw-rw-rw-   0        0        0      625 2022-10-16 06:15:30.000000 mctech_discovery-1.0.4/mctech_discovery/rpc/ep/ep_request.py
--rw-rw-rw-   0        0        0     5418 2023-02-24 15:34:39.000000 mctech_discovery-1.0.4/mctech_discovery/rpc/ep/internal_rpc.py
--rw-rw-rw-   0        0        0      676 2022-10-16 05:40:54.000000 mctech_discovery-1.0.4/mctech_discovery/rpc/ep/simple_ep_request.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:49:07.073284 mctech_discovery-1.0.4/mctech_discovery/rpc/lb/
--rw-rw-rw-   0        0        0     3255 2023-04-26 15:25:28.000000 mctech_discovery-1.0.4/mctech_discovery/rpc/lb/__init__.py
--rw-rw-rw-   0        0        0     1530 2023-04-26 15:25:28.000000 mctech_discovery-1.0.4/mctech_discovery/rpc/lb/direct_loadbalancer.py
--rw-rw-rw-   0        0        0     1879 2023-04-26 15:25:28.000000 mctech_discovery-1.0.4/mctech_discovery/rpc/lb/discovery_service_loadbalancer.py
--rw-rw-rw-   0        0        0     1179 2023-04-26 15:25:28.000000 mctech_discovery-1.0.4/mctech_discovery/rpc/lb/loadbalancer.py
--rw-rw-rw-   0        0        0     1156 2023-04-26 15:25:28.000000 mctech_discovery-1.0.4/mctech_discovery/rpc/lb/local_service_loadabalancer.py
--rw-rw-rw-   0        0        0     1048 2023-04-26 15:25:28.000000 mctech_discovery-1.0.4/mctech_discovery/rpc/lb/retry_loadbalancer.py
--rw-rw-rw-   0        0        0     7997 2023-02-24 15:34:39.000000 mctech_discovery-1.0.4/mctech_discovery/rpc/request_context.py
--rw-rw-rw-   0        0        0     3401 2023-02-24 15:34:39.000000 mctech_discovery-1.0.4/mctech_discovery/rpc/rpc_client.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:49:07.081285 mctech_discovery-1.0.4/mctech_discovery/rpc/rule/
--rw-rw-rw-   0        0        0        0 2022-02-12 09:07:52.000000 mctech_discovery-1.0.4/mctech_discovery/rpc/rule/__init__.py
--rw-rw-rw-   0        0        0     1080 2022-02-12 11:29:44.000000 mctech_discovery-1.0.4/mctech_discovery/rpc/rule/abstarct_rule.py
--rw-rw-rw-   0        0        0      494 2022-02-12 09:06:28.000000 mctech_discovery-1.0.4/mctech_discovery/rpc/rule/simple_rule.py
--rw-rw-rw-   0        0        0      467 2021-12-09 13:36:01.000000 mctech_discovery-1.0.4/mctech_discovery/rpc/web_error.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:49:07.001302 mctech_discovery-1.0.4/mctech_discovery.egg-info/
--rw-rw-rw-   0        0        0       63 2023-07-17 15:49:06.000000 mctech_discovery-1.0.4/mctech_discovery.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1387 2023-07-17 15:49:06.000000 mctech_discovery-1.0.4/mctech_discovery.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 15:49:06.000000 mctech_discovery-1.0.4/mctech_discovery.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-07-17 15:49:06.000000 mctech_discovery-1.0.4/mctech_discovery.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-17 15:49:06.000000 mctech_discovery-1.0.4/mctech_discovery.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      398 2023-07-17 15:48:42.000000 mctech_discovery-1.0.4/mctech_discovery_setup.py
--rw-rw-rw-   0        0        0       42 2023-07-17 15:49:07.089281 mctech_discovery-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-19 07:47:33.658794 mctech_discovery-1.0.5/
+-rw-rw-rw-   0        0        0      151 2023-07-19 07:47:33.657793 mctech_discovery-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      497 2023-07-19 07:47:00.000000 mctech_discovery-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 07:47:33.513746 mctech_discovery-1.0.5/mctech_discovery/
+-rw-rw-rw-   0        0        0        0 2020-06-01 07:50:38.000000 mctech_discovery-1.0.5/mctech_discovery/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:47:33.586259 mctech_discovery-1.0.5/mctech_discovery/config/
+-rw-rw-rw-   0        0        0      977 2022-10-08 03:15:48.000000 mctech_discovery-1.0.5/mctech_discovery/config/__init__.py
+-rw-rw-rw-   0        0        0     8183 2023-05-12 06:58:39.000000 mctech_discovery-1.0.5/mctech_discovery/config/_configure.py
+-rw-rw-rw-   0        0        0     8384 2023-05-12 06:58:39.000000 mctech_discovery-1.0.5/mctech_discovery/config/config_merger.py
+-rw-rw-rw-   0        0        0     1922 2022-10-08 03:15:48.000000 mctech_discovery-1.0.5/mctech_discovery/config/config_value.py
+-rw-rw-rw-   0        0        0     1464 2023-05-12 06:58:39.000000 mctech_discovery-1.0.5/mctech_discovery/config/yaml_loader.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:47:33.596259 mctech_discovery-1.0.5/mctech_discovery/discovery/
+-rw-rw-rw-   0        0        0     1420 2022-10-08 03:15:48.000000 mctech_discovery-1.0.5/mctech_discovery/discovery/__init__.py
+-rw-rw-rw-   0        0        0     8996 2023-05-17 02:51:55.000000 mctech_discovery-1.0.5/mctech_discovery/discovery/eureka_discovery_client.py
+-rw-rw-rw-   0        0        0      830 2022-10-08 03:15:48.000000 mctech_discovery-1.0.5/mctech_discovery/discovery/local_discovery_client.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:47:33.600266 mctech_discovery-1.0.5/mctech_discovery/lifecycle/
+-rw-rw-rw-   0        0        0        0 2023-05-12 06:58:39.000000 mctech_discovery-1.0.5/mctech_discovery/lifecycle/__init__.py
+-rw-rw-rw-   0        0        0     1173 2023-07-19 07:35:41.000000 mctech_discovery-1.0.5/mctech_discovery/lifecycle/lifecycle.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:47:33.611276 mctech_discovery-1.0.5/mctech_discovery/rpc/
+-rw-rw-rw-   0        0        0       68 2023-05-12 06:58:39.000000 mctech_discovery-1.0.5/mctech_discovery/rpc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:47:33.621798 mctech_discovery-1.0.5/mctech_discovery/rpc/ep/
+-rw-rw-rw-   0        0        0        0 2020-06-01 03:25:27.000000 mctech_discovery-1.0.5/mctech_discovery/rpc/ep/__init__.py
+-rw-rw-rw-   0        0        0      625 2023-05-12 06:58:39.000000 mctech_discovery-1.0.5/mctech_discovery/rpc/ep/ep_request.py
+-rw-rw-rw-   0        0        0     5418 2023-05-12 06:58:39.000000 mctech_discovery-1.0.5/mctech_discovery/rpc/ep/internal_rpc.py
+-rw-rw-rw-   0        0        0      676 2023-05-12 06:58:39.000000 mctech_discovery-1.0.5/mctech_discovery/rpc/ep/simple_ep_request.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:47:33.637789 mctech_discovery-1.0.5/mctech_discovery/rpc/lb/
+-rw-rw-rw-   0        0        0     3255 2023-05-12 06:58:39.000000 mctech_discovery-1.0.5/mctech_discovery/rpc/lb/__init__.py
+-rw-rw-rw-   0        0        0     1530 2023-05-12 06:58:39.000000 mctech_discovery-1.0.5/mctech_discovery/rpc/lb/direct_loadbalancer.py
+-rw-rw-rw-   0        0        0     1879 2023-05-12 06:58:39.000000 mctech_discovery-1.0.5/mctech_discovery/rpc/lb/discovery_service_loadbalancer.py
+-rw-rw-rw-   0        0        0     1179 2023-05-12 06:58:39.000000 mctech_discovery-1.0.5/mctech_discovery/rpc/lb/loadbalancer.py
+-rw-rw-rw-   0        0        0     1156 2023-05-12 06:58:39.000000 mctech_discovery-1.0.5/mctech_discovery/rpc/lb/local_service_loadabalancer.py
+-rw-rw-rw-   0        0        0     1048 2023-05-12 06:58:39.000000 mctech_discovery-1.0.5/mctech_discovery/rpc/lb/retry_loadbalancer.py
+-rw-rw-rw-   0        0        0     7997 2023-05-12 06:58:39.000000 mctech_discovery-1.0.5/mctech_discovery/rpc/request_context.py
+-rw-rw-rw-   0        0        0     3401 2023-05-12 06:58:39.000000 mctech_discovery-1.0.5/mctech_discovery/rpc/rpc_client.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:47:33.644793 mctech_discovery-1.0.5/mctech_discovery/rpc/rule/
+-rw-rw-rw-   0        0        0        0 2023-05-12 06:58:39.000000 mctech_discovery-1.0.5/mctech_discovery/rpc/rule/__init__.py
+-rw-rw-rw-   0        0        0     1041 2023-05-12 06:58:39.000000 mctech_discovery-1.0.5/mctech_discovery/rpc/rule/abstarct_rule.py
+-rw-rw-rw-   0        0        0      477 2023-05-12 06:58:39.000000 mctech_discovery-1.0.5/mctech_discovery/rpc/rule/simple_rule.py
+-rw-rw-rw-   0        0        0      451 2022-10-08 03:15:48.000000 mctech_discovery-1.0.5/mctech_discovery/rpc/web_error.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:47:33.655795 mctech_discovery-1.0.5/mctech_discovery/test/
+-rw-rw-rw-   0        0        0        0 2020-06-01 05:42:33.000000 mctech_discovery-1.0.5/mctech_discovery/test/__init__.py
+-rw-rw-rw-   0        0        0      196 2022-10-08 03:15:48.000000 mctech_discovery-1.0.5/mctech_discovery/test/config_test.py
+-rw-rw-rw-   0        0        0      491 2022-10-08 03:15:48.000000 mctech_discovery-1.0.5/mctech_discovery/test/crypto_text.py
+-rw-rw-rw-   0        0        0      734 2023-05-12 06:58:39.000000 mctech_discovery-1.0.5/mctech_discovery/test/eureka_test.py
+-rw-rw-rw-   0        0        0      650 2023-05-12 06:58:39.000000 mctech_discovery-1.0.5/mctech_discovery/test/pkg_test.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:47:33.559263 mctech_discovery-1.0.5/mctech_discovery.egg-info/
+-rw-rw-rw-   0        0        0      151 2023-07-19 07:47:33.000000 mctech_discovery-1.0.5/mctech_discovery.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1566 2023-07-19 07:47:33.000000 mctech_discovery-1.0.5/mctech_discovery.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 07:47:33.000000 mctech_discovery-1.0.5/mctech_discovery.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-07-19 07:47:33.000000 mctech_discovery-1.0.5/mctech_discovery.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-19 07:47:33.000000 mctech_discovery-1.0.5/mctech_discovery.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      435 2023-07-19 07:44:35.000000 mctech_discovery-1.0.5/mctech_discovery_setup.py
+-rw-rw-rw-   0        0        0       42 2023-07-19 07:47:33.659793 mctech_discovery-1.0.5/setup.cfg
```

### Comparing `mctech_discovery-1.0.4/mctech_discovery/config/_configure.py` & `mctech_discovery-1.0.5/mctech_discovery/config/_configure.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.0.4/mctech_discovery/config/config_merger.py` & `mctech_discovery-1.0.5/mctech_discovery/config/config_merger.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.0.4/mctech_discovery/config/yaml_loader.py` & `mctech_discovery-1.0.5/mctech_discovery/config/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.0.4/mctech_discovery/discovery/__init__.py` & `mctech_discovery-1.0.5/mctech_discovery/discovery/__init__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from __future__ import absolute_import
-import socket
-import netifaces
-from log4py import logging
-from .local_discovery_client import LocalDiscoveryClient
-from .eureka_discovery_client import EurekaDiscoveryClient
-from ..config import configure
-
-log = logging.getLogger('python.eureka.discoveryClient')
-
-
-def getIPAdress():
-    '''
-    获取本机ip
-    '''
-
-    result = []
-    for iface in netifaces.interfaces():
-        alias = netifaces.ifaddresses(iface)
-        ipv4 = alias.get(netifaces.AF_INET)
-        if ipv4 is None:
-            continue
-        for addr_info in ipv4:
-            address = addr_info["addr"]
-            if address == '127.0.0.1':
-                continue
-            result.append(addr_info["addr"])
-
-    if len(result) == 0:
-        raise RuntimeError('未找到合适的ipv4地址')
-
-    if len(result) > 1:
-        log.warning('找到多个符合条件的ipv4地址: %s' % result)
-
-    selected_address = result[0]
-    log.info('当前使用的ip地址: ' + selected_address)
-
-    return selected_address
-
-
-def __create_discovery_client():
-    eurekaConfig = configure.get_config('eureka', {'enabled': True})
-    DiscoveryClientCls = EurekaDiscoveryClient if eurekaConfig["enabled"] \
-        else LocalDiscoveryClient
-
-    ipAddress = getIPAdress()
-    hostName = socket.gethostname()
-    return DiscoveryClientCls(ipAddress, hostName)
-
-
-discovery_client = __create_discovery_client()
+from __future__ import absolute_import
+import socket
+import netifaces
+from log4py import logging
+from .local_discovery_client import LocalDiscoveryClient
+from .eureka_discovery_client import EurekaDiscoveryClient
+from ..config import configure
+
+log = logging.getLogger('python.eureka.discoveryClient')
+
+
+def getIPAdress():
+    '''
+    获取本机ip
+    '''
+
+    result = []
+    for iface in netifaces.interfaces():
+        alias = netifaces.ifaddresses(iface)
+        ipv4 = alias.get(netifaces.AF_INET)
+        if ipv4 is None:
+            continue
+        for addr_info in ipv4:
+            address = addr_info["addr"]
+            if address == '127.0.0.1':
+                continue
+            result.append(addr_info["addr"])
+
+    if len(result) == 0:
+        raise RuntimeError('未找到合适的ipv4地址')
+
+    if len(result) > 1:
+        log.warning('找到多个符合条件的ipv4地址: %s' % result)
+
+    selected_address = result[0]
+    log.info('当前使用的ip地址: ' + selected_address)
+
+    return selected_address
+
+
+def __create_discovery_client():
+    eurekaConfig = configure.get_config('eureka', {'enabled': True})
+    DiscoveryClientCls = EurekaDiscoveryClient if eurekaConfig["enabled"] \
+        else LocalDiscoveryClient
+
+    ipAddress = getIPAdress()
+    hostName = socket.gethostname()
+    return DiscoveryClientCls(ipAddress, hostName)
+
+
+discovery_client = __create_discovery_client()
```

### Comparing `mctech_discovery-1.0.4/mctech_discovery/discovery/eureka_discovery_client.py` & `mctech_discovery-1.0.5/mctech_discovery/discovery/eureka_discovery_client.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.0.4/mctech_discovery/lifecycle/lifecycle.py` & `mctech_discovery-1.0.5/mctech_discovery/lifecycle/lifecycle.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,23 +23,23 @@
     每秒检查一次， 每5秒输出一条日志
     """
 
     k8s = os.environ.get('KUBERNETES_SERVICE_HOST')
     sidecar = os.environ.get('ISTIO_INJECT_STATUS')
 
     if not k8s or not sidecar:
-        log.info("There's NO sidecar found!")
+        log.info("There's NO sidecar found. Skip checking sidecar status")
         return
 
     count = 0
     while True:
         try:
             url = 'http://localhost:15020/healthz/ready'
             res = requests.get(url, timeout=(0.1, 0.5))
             res.raise_for_status()
-            log.info('Sidecar is ready!!')
+            log.info("The sidecar is ready.")
             break
         except Exception:
             if count % 5 == 0:
                 log.info('Waiting for sidecar ready......')
             count = count + 1
             time.sleep(1)
```

### Comparing `mctech_discovery-1.0.4/mctech_discovery/rpc/ep/ep_request.py` & `mctech_discovery-1.0.5/mctech_discovery/rpc/ep/ep_request.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.0.4/mctech_discovery/rpc/ep/internal_rpc.py` & `mctech_discovery-1.0.5/mctech_discovery/rpc/ep/internal_rpc.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.0.4/mctech_discovery/rpc/ep/simple_ep_request.py` & `mctech_discovery-1.0.5/mctech_discovery/rpc/ep/simple_ep_request.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.0.4/mctech_discovery/rpc/lb/__init__.py` & `mctech_discovery-1.0.5/mctech_discovery/rpc/lb/__init__.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.0.4/mctech_discovery/rpc/lb/direct_loadbalancer.py` & `mctech_discovery-1.0.5/mctech_discovery/rpc/lb/direct_loadbalancer.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.0.4/mctech_discovery/rpc/lb/discovery_service_loadbalancer.py` & `mctech_discovery-1.0.5/mctech_discovery/rpc/lb/discovery_service_loadbalancer.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.0.4/mctech_discovery/rpc/lb/loadbalancer.py` & `mctech_discovery-1.0.5/mctech_discovery/rpc/lb/loadbalancer.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.0.4/mctech_discovery/rpc/lb/local_service_loadabalancer.py` & `mctech_discovery-1.0.5/mctech_discovery/rpc/lb/local_service_loadabalancer.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.0.4/mctech_discovery/rpc/lb/retry_loadbalancer.py` & `mctech_discovery-1.0.5/mctech_discovery/rpc/lb/retry_loadbalancer.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.0.4/mctech_discovery/rpc/request_context.py` & `mctech_discovery-1.0.5/mctech_discovery/rpc/request_context.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.0.4/mctech_discovery/rpc/rpc_client.py` & `mctech_discovery-1.0.5/mctech_discovery/rpc/rpc_client.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.0.4/mctech_discovery.egg-info/SOURCES.txt` & `mctech_discovery-1.0.5/mctech_discovery.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -28,8 +28,13 @@
 mctech_discovery/rpc/lb/direct_loadbalancer.py
 mctech_discovery/rpc/lb/discovery_service_loadbalancer.py
 mctech_discovery/rpc/lb/loadbalancer.py
 mctech_discovery/rpc/lb/local_service_loadabalancer.py
 mctech_discovery/rpc/lb/retry_loadbalancer.py
 mctech_discovery/rpc/rule/__init__.py
 mctech_discovery/rpc/rule/abstarct_rule.py
-mctech_discovery/rpc/rule/simple_rule.py
+mctech_discovery/rpc/rule/simple_rule.py
+mctech_discovery/test/__init__.py
+mctech_discovery/test/config_test.py
+mctech_discovery/test/crypto_text.py
+mctech_discovery/test/eureka_test.py
+mctech_discovery/test/pkg_test.py
```

