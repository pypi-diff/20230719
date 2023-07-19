# Comparing `tmp/rabbitbus-0.1.1.tar.gz` & `tmp/rabbitbus-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rabbitbus-0.1.1.tar", last modified: Wed Oct 28 13:05:30 2020, max compression
+gzip compressed data, was "rabbitbus-0.1.2.tar", last modified: Wed Jul 19 10:05:37 2023, max compression
```

## Comparing `rabbitbus-0.1.1.tar` & `rabbitbus-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-28 13:05:30.000000 rabbitbus-0.1.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)       34 2020-10-28 13:05:14.000000 rabbitbus-0.1.1/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)       17 2020-10-28 13:05:14.000000 rabbitbus-0.1.1/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2712 2020-10-28 13:05:30.000000 rabbitbus-0.1.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1518 2020-10-28 13:05:14.000000 rabbitbus-0.1.1/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-28 13:05:30.000000 rabbitbus-0.1.1/rabbitbus/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-28 13:05:30.000000 rabbitbus-0.1.1/rabbitbus/acks/
--rw-rw-r--   0 travis    (2000) travis    (2000)      647 2020-10-28 13:05:14.000000 rabbitbus-0.1.1/rabbitbus/acks/requests.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-28 13:05:14.000000 rabbitbus-0.1.1/rabbitbus/acks/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      527 2020-10-28 13:05:14.000000 rabbitbus-0.1.1/rabbitbus/acks/responses.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11866 2020-10-28 13:05:14.000000 rabbitbus-0.1.1/rabbitbus/manager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       36 2020-10-28 13:05:14.000000 rabbitbus-0.1.1/rabbitbus/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-28 13:05:30.000000 rabbitbus-0.1.1/rabbitbus.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2712 2020-10-28 13:05:30.000000 rabbitbus-0.1.1/rabbitbus.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-10-28 13:05:30.000000 rabbitbus-0.1.1/rabbitbus.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2020-10-28 13:05:30.000000 rabbitbus-0.1.1/rabbitbus.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      336 2020-10-28 13:05:30.000000 rabbitbus-0.1.1/rabbitbus.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2020-10-28 13:05:30.000000 rabbitbus-0.1.1/rabbitbus.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-10-28 13:05:30.000000 rabbitbus-0.1.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     3786 2020-10-28 13:05:14.000000 rabbitbus-0.1.1/setup.py
+drwxr-xr-x   0 shadrus   (1000) shadrus   (1000)        0 2023-07-19 10:05:37.216935 rabbitbus-0.1.2/
+-rw-r--r--   0 shadrus   (1000) shadrus   (1000)     1068 2023-07-19 08:12:49.000000 rabbitbus-0.1.2/LICENSE
+-rw-r--r--   0 shadrus   (1000) shadrus   (1000)       34 2023-07-19 08:12:49.000000 rabbitbus-0.1.2/MANIFEST.in
+-rw-r--r--   0 shadrus   (1000) shadrus   (1000)     2733 2023-07-19 10:05:37.216935 rabbitbus-0.1.2/PKG-INFO
+-rw-r--r--   0 shadrus   (1000) shadrus   (1000)     1941 2023-07-19 08:12:49.000000 rabbitbus-0.1.2/README.md
+drwxr-xr-x   0 shadrus   (1000) shadrus   (1000)        0 2023-07-19 10:05:37.216935 rabbitbus-0.1.2/rabbitbus/
+-rw-r--r--   0 shadrus   (1000) shadrus   (1000)       36 2023-07-19 08:12:49.000000 rabbitbus-0.1.2/rabbitbus/__init__.py
+drwxr-xr-x   0 shadrus   (1000) shadrus   (1000)        0 2023-07-19 10:05:37.216935 rabbitbus-0.1.2/rabbitbus/acks/
+-rw-r--r--   0 shadrus   (1000) shadrus   (1000)        0 2023-07-19 08:12:49.000000 rabbitbus-0.1.2/rabbitbus/acks/__init__.py
+-rw-r--r--   0 shadrus   (1000) shadrus   (1000)      647 2023-07-19 08:12:49.000000 rabbitbus-0.1.2/rabbitbus/acks/requests.py
+-rw-r--r--   0 shadrus   (1000) shadrus   (1000)      527 2023-07-19 08:12:49.000000 rabbitbus-0.1.2/rabbitbus/acks/responses.py
+-rw-r--r--   0 shadrus   (1000) shadrus   (1000)    11837 2023-07-19 08:32:16.000000 rabbitbus-0.1.2/rabbitbus/manager.py
+drwxr-xr-x   0 shadrus   (1000) shadrus   (1000)        0 2023-07-19 10:05:37.216935 rabbitbus-0.1.2/rabbitbus.egg-info/
+-rw-r--r--   0 shadrus   (1000) shadrus   (1000)     2733 2023-07-19 10:05:37.000000 rabbitbus-0.1.2/rabbitbus.egg-info/PKG-INFO
+-rw-r--r--   0 shadrus   (1000) shadrus   (1000)      344 2023-07-19 10:05:37.000000 rabbitbus-0.1.2/rabbitbus.egg-info/SOURCES.txt
+-rw-r--r--   0 shadrus   (1000) shadrus   (1000)        1 2023-07-19 10:05:37.000000 rabbitbus-0.1.2/rabbitbus.egg-info/dependency_links.txt
+-rw-r--r--   0 shadrus   (1000) shadrus   (1000)       16 2023-07-19 10:05:37.000000 rabbitbus-0.1.2/rabbitbus.egg-info/requires.txt
+-rw-r--r--   0 shadrus   (1000) shadrus   (1000)       10 2023-07-19 10:05:37.000000 rabbitbus-0.1.2/rabbitbus.egg-info/top_level.txt
+-rw-r--r--   0 shadrus   (1000) shadrus   (1000)       17 2023-07-19 08:27:35.000000 rabbitbus-0.1.2/requirements.txt
+-rw-r--r--   0 shadrus   (1000) shadrus   (1000)       38 2023-07-19 10:05:37.216935 rabbitbus-0.1.2/setup.cfg
+-rw-r--r--   0 shadrus   (1000) shadrus   (1000)     3836 2023-07-19 08:29:00.000000 rabbitbus-0.1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rabbitbus-0.1.1/PKG-INFO` & `rabbitbus-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,98 @@
 Metadata-Version: 2.1
 Name: rabbitbus
-Version: 0.1.1
+Version: 0.1.2
 Summary: RabbitMQ app framework
 Home-page: https://github.com/shadrus/rabbitbus
 Author: KrylovYS
 Author-email: krylov.ys@malltech.ru
 License: MIT
-Description: 
-        ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rabbitbus)
-        [![Build Status](https://travis-ci.org/shadrus/rabbitbus.svg?branch=master)](https://travis-ci.org/shadrus/rabbitbus)
-        # RabbitBus
-        
-        Feel RabbitMQ like HTTP
-        
-          - Custom CorrelationManagers
-          - Regexp routes
-        
-        
-        ### Installation
-        
-        RabbitBus requires Python 3.6 >, aioamqp.
-        
-        Install the dependencies and library.
-        
-        ```sh
-        $ pip install rabbitbus
-        ```
-        
-        Example:
-        
-        ```python
-        import asyncio
-        from rabbitbus.manager import DatabusApp, Configuration
-        from rabbitbus.acks.requests import AmqpRequest
-        from rabbitbus.acks.responses import AckResponse
-        
-        async def my_view(request: AmqpRequest):
-            # Write your code here
-            return AckResponse(request)
-        
-        def serve():
-            loop = asyncio.get_event_loop()
-            # Inherit from CorrelationManager for custom correlation storages
-            app = DatabusApp(conf=Configuration())
-            app.add_route(r'^CASH_REGISTER_EQUIPMENTS[a-zA-Z_]{4}$', my_view)
-            app.start(loop)
-        
-        
-        if __name__ == '__main__':
-            serve()
-        ```
-        
-        If message has reply_to property, you can make response like
-        
-        ```python
-        from rabbitbus.acks.requests import AmqpRequest
-        from rabbitbus.acks.responses import AckResponse
-        
-        async def my_view(request: AmqpRequest):
-            # Write your code here
-            return AckResponse(request, data={"result": 1})
-        ```
-        
-        "reply_to" will be converted to the "routing_key" and message will be published to the app exchange.
-        More about RPC you can read [in RabbitMQ documentation](https://www.rabbitmq.com/tutorials/tutorial-six-python.html)
-        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6.0
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rabbitbus)
+[![Build Status](https://travis-ci.org/shadrus/rabbitbus.svg?branch=master)](https://travis-ci.org/shadrus/rabbitbus)
+# RabbitBus
+
+Feel RabbitMQ like HTTP
+
+  - Custom CorrelationManagers
+  - Regexp routes
+
+
+### Installation
+
+RabbitBus requires Python 3.6 >, aioamqp.
+
+Install the dependencies and library.
+
+```sh
+$ pip install rabbitbus
+```
+
+Example:
+
+```python
+import asyncio
+from rabbitbus.manager import DatabusApp, Configuration
+from rabbitbus.acks.requests import AmqpRequest
+from rabbitbus.acks.responses import AckResponse
+
+async def my_view(request: AmqpRequest):
+    # Write your code here
+    return AckResponse(request)
+
+def serve():
+    loop = asyncio.get_event_loop()
+    # Inherit from CorrelationManager for custom correlation storages
+    app = DatabusApp(conf=Configuration())
+    app.add_route(r'^CASH_REGISTER_EQUIPMENTS[a-zA-Z_]{4}$', my_view)
+    app.start(loop)
+
+
+if __name__ == '__main__':
+    serve()
+```
+
+If message has reply_to property, you can make response like:
+
+```python
+from rabbitbus.acks.requests import AmqpRequest
+from rabbitbus.acks.responses import AckResponse
+
+async def my_view(request: AmqpRequest):
+    # Write your code here
+    return AckResponse(request, data={"result": 1})
+```
+
+"reply_to" will be converted to the "routing_key" and message will be published to the app exchange.
+More about RPC you can read [in RabbitMQ documentation](https://www.rabbitmq.com/tutorials/tutorial-six-python.html)
+
+Sometimes you may need to pause consuming.
+Three method are to your needs:
+
+```python
+app.pause_consuming()
+app.continue_consuming()
+app.is_paused() #bool to test if your app is paused
+```
+
+To send message from any view you can also use:
+```python
+async def my_view(request: AmqpRequest):
+    # Write your code here
+    request.app.send_message(data={"test": True}, routing_key="TEST")
+    return AckResponse(request)
+```
+
```

### Comparing `rabbitbus-0.1.1/README.md` & `rabbitbus-0.1.2/rabbitbus.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: rabbitbus
+Version: 0.1.2
+Summary: RabbitMQ app framework
+Home-page: https://github.com/shadrus/rabbitbus
+Author: KrylovYS
+Author-email: krylov.ys@malltech.ru
+License: MIT
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rabbitbus)
 [![Build Status](https://travis-ci.org/shadrus/rabbitbus.svg?branch=master)](https://travis-ci.org/shadrus/rabbitbus)
 # RabbitBus
 
 Feel RabbitMQ like HTTP
 
   - Custom CorrelationManagers
@@ -38,20 +61,38 @@
     app.start(loop)
 
 
 if __name__ == '__main__':
     serve()
 ```
 
-If message has reply_to property, you can make response like
+If message has reply_to property, you can make response like:
 
 ```python
 from rabbitbus.acks.requests import AmqpRequest
 from rabbitbus.acks.responses import AckResponse
 
 async def my_view(request: AmqpRequest):
     # Write your code here
     return AckResponse(request, data={"result": 1})
 ```
 
 "reply_to" will be converted to the "routing_key" and message will be published to the app exchange.
 More about RPC you can read [in RabbitMQ documentation](https://www.rabbitmq.com/tutorials/tutorial-six-python.html)
+
+Sometimes you may need to pause consuming.
+Three method are to your needs:
+
+```python
+app.pause_consuming()
+app.continue_consuming()
+app.is_paused() #bool to test if your app is paused
+```
+
+To send message from any view you can also use:
+```python
+async def my_view(request: AmqpRequest):
+    # Write your code here
+    request.app.send_message(data={"test": True}, routing_key="TEST")
+    return AckResponse(request)
+```
+
```

### Comparing `rabbitbus-0.1.1/rabbitbus/acks/requests.py` & `rabbitbus-0.1.2/rabbitbus/acks/requests.py`

 * *Files identical despite different names*

### Comparing `rabbitbus-0.1.1/rabbitbus/acks/responses.py` & `rabbitbus-0.1.2/rabbitbus/acks/responses.py`

 * *Files identical despite different names*

### Comparing `rabbitbus-0.1.1/rabbitbus/manager.py` & `rabbitbus-0.1.2/rabbitbus/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         route = await self.correlation_manager.find_request_by_correlation_id(
             correlation_id)
         if route:
             return route
         else:
             logger.warning(f"Got unknown correlation_id: {correlation_id}")
 
-    def __prepare_data(self, data):
+    def __prepare_data(self, data) -> str:
         if isinstance(data, list) or isinstance(data, dict):
             return json.dumps(data)
         else:
             return str(data)
 
     async def send_message(self, data, routing_key: str, properties: Properties):
         await self.channel.publish(payload=self.__prepare_data(data),
@@ -209,15 +209,15 @@
                                                         virtualhost=self.__conf.virtualhost)
             self.channel = await protocol.channel()
             await self.channel.basic_qos(prefetch_count=self.__max_workers)
             await self.channel.basic_consume(self.__serve_message,
                                              queue_name=self.__conf.queue_name,
                                              no_ack=False)
         except aioamqp.AmqpClosedConnection:
-            logging.debug("AmqpClosedConnection, will call on_error")
+            logging.warning("AmqpClosedConnection, will call on_error")
         except (OSError, ConnectionRefusedError) as e:
             if transport and not transport.is_closing():
                 await transport.close()
             if reconnect:
                 logger.warning(str(e))
                 await asyncio.sleep(reconnect_wait_period)
                 await self.__receive(reconnect, reconnect_wait_period)
@@ -227,16 +227,15 @@
     async def __set_response(self, request: AmqpRequest,
                              response: Union[AckResponse, NackResponse, None],
                              worker_id):
         if isinstance(response, AckResponse):
             if request.properties.reply_to:
                 await self.send_message(response.data,
                                         routing_key=request.properties.reply_to,
-                                        properties={
-                                            "correlation_id": request.properties.correlation_id}
+                                        properties=Properties(correlation_id=request.properties.correlation_id)
                                         )
             if request.envelope.delivery_tag:
                 await request.channel.basic_client_ack(
                     delivery_tag=request.envelope.delivery_tag)
             logger.debug("Worker %s completed the task" % worker_id)
         else:
             logger.warning(
```

### Comparing `rabbitbus-0.1.1/setup.py` & `rabbitbus-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 
 # Package meta-data.
 NAME = 'rabbitbus'
 DESCRIPTION = 'RabbitMQ app framework'
 URL = 'https://github.com/shadrus/rabbitbus'
 EMAIL = 'krylov.ys@malltech.ru'
 AUTHOR = 'KrylovYS'
-REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.1'
+REQUIRES_PYTHON = '>=3.7.0'
+VERSION = '0.1.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
-    'aioamqp==0.14.0'
+    'aioamqp==0.15.0'
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
@@ -116,17 +116,18 @@
     license='MIT',
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy'
     ],
     # $ setup.py publish support.
     cmdclass={
         'upload': UploadCommand,
     },
```

