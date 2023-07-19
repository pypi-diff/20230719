# Comparing `tmp/pygbop-0.2.0.3.tar.gz` & `tmp/pygbop-0.2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pygbop-0.2.0.3.tar", last modified: Thu Jul  6 02:05:17 2023, max compression
+gzip compressed data, was "dist\pygbop-0.2.0.5.tar", last modified: Wed Jul 19 05:56:19 2023, max compression
```

## Comparing `pygbop-0.2.0.3.tar` & `pygbop-0.2.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 02:05:17.000000 pygbop-0.2.0.3/
--rw-rw-rw-   0        0        0      207 2023-07-05 07:13:48.000000 pygbop-0.2.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2522 2023-07-06 02:05:17.000000 pygbop-0.2.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-06 02:05:17.000000 pygbop-0.2.0.3/pygbop/
--rw-rw-rw-   0        0        0      467 2023-06-14 03:13:50.000000 pygbop-0.2.0.3/pygbop/common.py
--rw-rw-rw-   0        0        0     2776 2023-07-06 02:01:12.000000 pygbop-0.2.0.3/pygbop/event_push.py
--rw-rw-rw-   0        0        0     4199 2023-07-05 06:47:47.000000 pygbop-0.2.0.3/pygbop/gbop.py
--rw-rw-rw-   0        0        0      601 2023-07-05 07:08:15.000000 pygbop-0.2.0.3/pygbop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 02:05:17.000000 pygbop-0.2.0.3/pygbop.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-06 02:05:17.000000 pygbop-0.2.0.3/pygbop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2522 2023-07-06 02:05:17.000000 pygbop-0.2.0.3/pygbop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-07-06 02:05:17.000000 pygbop-0.2.0.3/pygbop.egg-info/requires.txt
--rw-rw-rw-   0        0        0      278 2023-07-06 02:05:17.000000 pygbop-0.2.0.3/pygbop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-06 02:05:17.000000 pygbop-0.2.0.3/pygbop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1564 2023-07-06 02:02:34.000000 pygbop-0.2.0.3/readme.md
--rw-rw-rw-   0        0        0       16 2022-07-08 06:38:50.000000 pygbop-0.2.0.3/requirements.txt
--rw-rw-rw-   0        0        0       64 2023-07-06 02:05:17.000000 pygbop-0.2.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1274 2023-07-06 02:04:44.000000 pygbop-0.2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 05:56:19.000000 pygbop-0.2.0.5/
+-rw-rw-rw-   0        0        0      207 2023-07-05 07:13:48.000000 pygbop-0.2.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     3245 2023-07-19 05:56:19.000000 pygbop-0.2.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-19 05:56:19.000000 pygbop-0.2.0.5/pygbop/
+-rw-rw-rw-   0        0        0      480 2023-07-19 05:43:19.000000 pygbop-0.2.0.5/pygbop/common.py
+-rw-rw-rw-   0        0        0     3950 2023-07-19 05:43:41.000000 pygbop-0.2.0.5/pygbop/event_push.py
+-rw-rw-rw-   0        0        0     4199 2023-07-05 06:47:47.000000 pygbop-0.2.0.5/pygbop/gbop.py
+-rw-rw-rw-   0        0        0      601 2023-07-05 07:08:15.000000 pygbop-0.2.0.5/pygbop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 05:56:19.000000 pygbop-0.2.0.5/pygbop.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-19 05:56:19.000000 pygbop-0.2.0.5/pygbop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     3245 2023-07-19 05:56:19.000000 pygbop-0.2.0.5/pygbop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2023-07-19 05:56:19.000000 pygbop-0.2.0.5/pygbop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      278 2023-07-19 05:56:19.000000 pygbop-0.2.0.5/pygbop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-19 05:56:19.000000 pygbop-0.2.0.5/pygbop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2287 2023-07-19 05:53:06.000000 pygbop-0.2.0.5/readme.md
+-rw-rw-rw-   0        0        0       16 2022-07-08 06:38:50.000000 pygbop-0.2.0.5/requirements.txt
+-rw-rw-rw-   0        0        0       64 2023-07-19 05:56:19.000000 pygbop-0.2.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1274 2023-07-19 05:56:15.000000 pygbop-0.2.0.5/setup.py
```

### Comparing `pygbop-0.2.0.3/PKG-INFO` & `pygbop-0.2.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygbop
-Version: 0.2.0.3
+Version: 0.2.0.5
 Summary: Geely GBOP Client
 Home-page: https://pypi.python.org/pypi/GbopApiClient
 Author: huang.xiaogang
 Author-email: huang.xiaogang@geely.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -66,8 +66,28 @@
     "message": "hello 喵啪斯"
 }
 response = event_push_client.push_message(data=data,
                                           source='xx.cmdb',
                                           type_='xx:cmdb:InstanceChanged')
 print(response.decode('utf-8'))
 ```
+or
+```python
+from pygbop import CloudEventBasicAuth, EventPushClient
+
+auth = CloudEventBasicAuth(producer_group='xxxxxxx',
+                           subject='persistent://Information_Technology/xxxx/XXXX_EVENT',
+                           secret_token='xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx')
+event_push_client = EventPushClient(auth=auth, base_url='http://xxxx.dev.xxxxx.com')
+data = {
+    "message": "hello 喵啪斯"
+}
+response = event_push_client.push(data=data,
+                                  source='xx.cmdb',
+                                  type_='xx:cmdb:InstanceChanged')
+if response.result:
+    message_id = response.data
+else:
+    code = response.code
+    fail_message = response.message
+```
```

### Comparing `pygbop-0.2.0.3/pygbop/event_push.py` & `pygbop-0.2.0.5/pygbop/event_push.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 # ======================================================
 # @Project : GbopApiClient
 # @FileName: event_push
 # @Software: PyCharm
 import uuid
 import datetime
 import requests
+import json
+from .common import ResultStruct
 
 
 class CloudEventBasicAuth(object):
     PROTOCOL_TYPE = 'cloudevents'
     LANGUAGE = 'Python'
     CONTENT_TYPE = 'application/json;charset=utf-8'
 
@@ -68,7 +70,38 @@
             "type": type_,
             "specversion": "1.0",
             "subject": self.auth.subject,
             "data": data
         }
         response = requests.post(self.base_url, json=_data, headers=self._get_headers(), timeout=timeout).content
         return response
+
+    def push(self, data: dict, source: str, type_: str, id_: str = '', timeout: int = 30) -> str:
+        """
+        消息推送
+        :param timeout: 超时时间
+        :param data: 数据体
+        :param source: 数据来源
+        :param type_: 数据类型
+        :param id_: 自定义数据编号(不传使用uuid)
+        :return: response content
+        """
+        _data = {
+            "id": id_ if id_ else str(uuid.uuid1()),
+            "source": source,
+            "type": type_,
+            "specversion": "1.0",
+            "subject": self.auth.subject,
+            "data": data
+        }
+        response = requests.post(self.base_url, json=_data, headers=self._get_headers(), timeout=timeout).content
+        res_json = json.loads(response.decode('utf-8'))
+        code = res_json['retCode']
+        msg = res_json['retMsg']
+        if code == 0:
+            result = True
+            data = msg[msg.find('messageId=') + 10:-1]
+            msg = ''
+        else:
+            result = False
+            data = None
+        return ResultStruct(result, code, msg, data)
```

### Comparing `pygbop-0.2.0.3/pygbop/gbop.py` & `pygbop-0.2.0.5/pygbop/gbop.py`

 * *Files identical despite different names*

### Comparing `pygbop-0.2.0.3/pygbop/__init__.py` & `pygbop-0.2.0.5/pygbop/__init__.py`

 * *Files identical despite different names*

### Comparing `pygbop-0.2.0.3/pygbop.egg-info/PKG-INFO` & `pygbop-0.2.0.5/pygbop.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygbop
-Version: 0.2.0.3
+Version: 0.2.0.5
 Summary: Geely GBOP Client
 Home-page: https://pypi.python.org/pypi/GbopApiClient
 Author: huang.xiaogang
 Author-email: huang.xiaogang@geely.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -66,8 +66,28 @@
     "message": "hello 喵啪斯"
 }
 response = event_push_client.push_message(data=data,
                                           source='xx.cmdb',
                                           type_='xx:cmdb:InstanceChanged')
 print(response.decode('utf-8'))
 ```
+or
+```python
+from pygbop import CloudEventBasicAuth, EventPushClient
+
+auth = CloudEventBasicAuth(producer_group='xxxxxxx',
+                           subject='persistent://Information_Technology/xxxx/XXXX_EVENT',
+                           secret_token='xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx')
+event_push_client = EventPushClient(auth=auth, base_url='http://xxxx.dev.xxxxx.com')
+data = {
+    "message": "hello 喵啪斯"
+}
+response = event_push_client.push(data=data,
+                                  source='xx.cmdb',
+                                  type_='xx:cmdb:InstanceChanged')
+if response.result:
+    message_id = response.data
+else:
+    code = response.code
+    fail_message = response.message
+```
```

### Comparing `pygbop-0.2.0.3/readme.md` & `pygbop-0.2.0.5/readme.md`

 * *Files 19% similar despite different names*

```diff
@@ -40,8 +40,28 @@
 data = {
     "message": "hello 喵啪斯"
 }
 response = event_push_client.push_message(data=data,
                                           source='xx.cmdb',
                                           type_='xx:cmdb:InstanceChanged')
 print(response.decode('utf-8'))
+```
+or
+```python
+from pygbop import CloudEventBasicAuth, EventPushClient
+
+auth = CloudEventBasicAuth(producer_group='xxxxxxx',
+                           subject='persistent://Information_Technology/xxxx/XXXX_EVENT',
+                           secret_token='xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx')
+event_push_client = EventPushClient(auth=auth, base_url='http://xxxx.dev.xxxxx.com')
+data = {
+    "message": "hello 喵啪斯"
+}
+response = event_push_client.push(data=data,
+                                  source='xx.cmdb',
+                                  type_='xx:cmdb:InstanceChanged')
+if response.result:
+    message_id = response.data
+else:
+    code = response.code
+    fail_message = response.message
 ```
```

### Comparing `pygbop-0.2.0.3/setup.py` & `pygbop-0.2.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 from __future__ import print_function
 from setuptools import setup, find_packages
 
 setup(
     name="pygbop",
-    version="0.2.0.3",
+    version="0.2.0.5",
     author="huang.xiaogang",
     author_email="huang.xiaogang@geely.com",
     description="Geely GBOP Client",
     long_description=open("readme.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://pypi.python.org/pypi/GbopApiClient",
```

