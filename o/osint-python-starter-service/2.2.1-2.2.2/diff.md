# Comparing `tmp/osint-python-starter-service-2.2.1.tar.gz` & `tmp/osint-python-starter-service-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osint-python-starter-service-2.2.1.tar", last modified: Tue Jun 27 14:10:22 2023, max compression
+gzip compressed data, was "osint-python-starter-service-2.2.2.tar", last modified: Wed Jul 19 12:32:52 2023, max compression
```

## Comparing `osint-python-starter-service-2.2.1.tar` & `osint-python-starter-service-2.2.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-27 14:10:22.040169 osint-python-starter-service-2.2.1/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-starter-service-2.2.1/LICENSE
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2202 2023-06-27 14:10:22.040169 osint-python-starter-service-2.2.1/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1731 2023-04-25 07:13:29.000000 osint-python-starter-service-2.2.1/README.md
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-27 14:10:22.040169 osint-python-starter-service-2.2.1/classes/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-22 23:18:15.000000 osint-python-starter-service-2.2.1/classes/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2841 2023-06-22 23:23:47.000000 osint-python-starter-service-2.2.1/classes/article_raw_en.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      909 2023-06-22 23:23:46.000000 osint-python-starter-service-2.2.1/classes/metadata_item_ner_en.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-27 14:10:22.040169 osint-python-starter-service-2.2.1/osint_python_starter_service.egg-info/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2202 2023-06-27 14:10:22.000000 osint-python-starter-service-2.2.1/osint_python_starter_service.egg-info/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1051 2023-06-27 14:10:22.000000 osint-python-starter-service-2.2.1/osint_python_starter_service.egg-info/SOURCES.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-06-27 14:10:22.000000 osint-python-starter-service-2.2.1/osint_python_starter_service.egg-info/dependency_links.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      108 2023-06-27 14:10:22.000000 osint-python-starter-service-2.2.1/osint_python_starter_service.egg-info/requires.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       24 2023-06-27 14:10:22.000000 osint-python-starter-service-2.2.1/osint_python_starter_service.egg-info/top_level.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-06-27 14:10:22.040169 osint-python-starter-service-2.2.1/setup.cfg
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      778 2023-06-27 14:09:32.000000 osint-python-starter-service-2.2.1/setup.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-27 14:10:22.040169 osint-python-starter-service-2.2.1/starter_service/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2022-06-04 21:05:58.000000 osint-python-starter-service-2.2.1/starter_service/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      973 2023-04-06 22:41:55.000000 osint-python-starter-service-2.2.1/starter_service/api.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6309 2023-06-23 01:20:47.000000 osint-python-starter-service-2.2.1/starter_service/api_server.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     5774 2023-06-03 20:59:13.000000 osint-python-starter-service-2.2.1/starter_service/avro_parser.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     4278 2023-06-27 14:08:38.000000 osint-python-starter-service-2.2.1/starter_service/base_service.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1837 2023-06-07 19:08:41.000000 osint-python-starter-service-2.2.1/starter_service/env.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-27 14:10:22.040169 osint-python-starter-service-2.2.1/starter_service/examples/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-29 02:03:27.000000 osint-python-starter-service-2.2.1/starter_service/examples/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      602 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.1/starter_service/examples/error.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1595 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.1/starter_service/examples/manual_api.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1282 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.1/starter_service/examples/manual_kafka.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1220 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.1/starter_service/examples/multi.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1332 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.1/starter_service/examples/offset_kafka.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1164 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.1/starter_service/examples/single.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6117 2023-06-23 01:28:24.000000 osint-python-starter-service-2.2.1/starter_service/kafka_adapter.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     7571 2023-04-25 06:06:55.000000 osint-python-starter-service-2.2.1/starter_service/schemas.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      788 2023-06-23 00:39:02.000000 osint-python-starter-service-2.2.1/starter_service/sub_process.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-27 14:10:22.040169 osint-python-starter-service-2.2.1/starter_service/tests/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-05-18 14:40:43.000000 osint-python-starter-service-2.2.1/starter_service/tests/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      560 2023-05-18 15:14:53.000000 osint-python-starter-service-2.2.1/starter_service/tests/employee.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      699 2023-06-03 20:55:03.000000 osint-python-starter-service-2.2.1/starter_service/tests/teet.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2885 2023-06-03 20:45:37.000000 osint-python-starter-service-2.2.1/starter_service/tests/test_avro_parser.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      194 2023-05-18 14:41:17.000000 osint-python-starter-service-2.2.1/starter_service/tests/tst.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-07-19 12:32:52.539366 osint-python-starter-service-2.2.2/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-starter-service-2.2.2/LICENSE
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2202 2023-07-19 12:32:52.536032 osint-python-starter-service-2.2.2/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1731 2023-04-25 07:13:29.000000 osint-python-starter-service-2.2.2/README.md
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-07-19 12:32:52.536032 osint-python-starter-service-2.2.2/classes/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-22 23:18:15.000000 osint-python-starter-service-2.2.2/classes/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2841 2023-06-22 23:23:47.000000 osint-python-starter-service-2.2.2/classes/article_raw_en.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      909 2023-06-22 23:23:46.000000 osint-python-starter-service-2.2.2/classes/metadata_item_ner_en.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-07-19 12:32:52.536032 osint-python-starter-service-2.2.2/osint_python_starter_service.egg-info/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2202 2023-07-19 12:32:52.000000 osint-python-starter-service-2.2.2/osint_python_starter_service.egg-info/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1051 2023-07-19 12:32:52.000000 osint-python-starter-service-2.2.2/osint_python_starter_service.egg-info/SOURCES.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-07-19 12:32:52.000000 osint-python-starter-service-2.2.2/osint_python_starter_service.egg-info/dependency_links.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      108 2023-07-19 12:32:52.000000 osint-python-starter-service-2.2.2/osint_python_starter_service.egg-info/requires.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       24 2023-07-19 12:32:52.000000 osint-python-starter-service-2.2.2/osint_python_starter_service.egg-info/top_level.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-07-19 12:32:52.539366 osint-python-starter-service-2.2.2/setup.cfg
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      778 2023-07-19 12:31:07.000000 osint-python-starter-service-2.2.2/setup.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-07-19 12:32:52.536032 osint-python-starter-service-2.2.2/starter_service/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2022-06-04 21:05:58.000000 osint-python-starter-service-2.2.2/starter_service/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      973 2023-04-06 22:41:55.000000 osint-python-starter-service-2.2.2/starter_service/api.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6309 2023-06-23 01:20:47.000000 osint-python-starter-service-2.2.2/starter_service/api_server.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     5774 2023-06-03 20:59:13.000000 osint-python-starter-service-2.2.2/starter_service/avro_parser.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     4758 2023-07-19 12:29:04.000000 osint-python-starter-service-2.2.2/starter_service/base_service.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1837 2023-06-07 19:08:41.000000 osint-python-starter-service-2.2.2/starter_service/env.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-07-19 12:32:52.536032 osint-python-starter-service-2.2.2/starter_service/examples/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-29 02:03:27.000000 osint-python-starter-service-2.2.2/starter_service/examples/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      602 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.2/starter_service/examples/error.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1595 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.2/starter_service/examples/manual_api.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1282 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.2/starter_service/examples/manual_kafka.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1220 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.2/starter_service/examples/multi.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1332 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.2/starter_service/examples/offset_kafka.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1164 2023-06-23 01:24:07.000000 osint-python-starter-service-2.2.2/starter_service/examples/single.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6963 2023-07-19 12:29:30.000000 osint-python-starter-service-2.2.2/starter_service/kafka_adapter.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     7571 2023-04-25 06:06:55.000000 osint-python-starter-service-2.2.2/starter_service/schemas.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      788 2023-06-23 00:39:02.000000 osint-python-starter-service-2.2.2/starter_service/sub_process.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-07-19 12:32:52.536032 osint-python-starter-service-2.2.2/starter_service/tests/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-05-18 14:40:43.000000 osint-python-starter-service-2.2.2/starter_service/tests/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      560 2023-05-18 15:14:53.000000 osint-python-starter-service-2.2.2/starter_service/tests/employee.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      699 2023-06-03 20:55:03.000000 osint-python-starter-service-2.2.2/starter_service/tests/teet.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2885 2023-06-03 20:45:37.000000 osint-python-starter-service-2.2.2/starter_service/tests/test_avro_parser.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      194 2023-05-18 14:41:17.000000 osint-python-starter-service-2.2.2/starter_service/tests/tst.py
```

### Comparing `osint-python-starter-service-2.2.1/LICENSE` & `osint-python-starter-service-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.1/PKG-INFO` & `osint-python-starter-service-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-starter-service
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python starter service
 Home-page: https://github.com/OSINT-VDU-TNO/python-starter-service
 Author: mindpetk
 Author-email: petkeviciusm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `osint-python-starter-service-2.2.1/README.md` & `osint-python-starter-service-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.1/classes/article_raw_en.py` & `osint-python-starter-service-2.2.2/classes/article_raw_en.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.1/classes/metadata_item_ner_en.py` & `osint-python-starter-service-2.2.2/classes/metadata_item_ner_en.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.1/osint_python_starter_service.egg-info/PKG-INFO` & `osint-python-starter-service-2.2.2/osint_python_starter_service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-starter-service
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python starter service
 Home-page: https://github.com/OSINT-VDU-TNO/python-starter-service
 Author: mindpetk
 Author-email: petkeviciusm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `osint-python-starter-service-2.2.1/osint_python_starter_service.egg-info/SOURCES.txt` & `osint-python-starter-service-2.2.2/osint_python_starter_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.1/setup.py` & `osint-python-starter-service-2.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 setuptools.setup(
     name="osint-python-starter-service",
-    version="2.2.1",
+    version="2.2.2",
     author="mindpetk",
     author_email="petkeviciusm@gmail.com",
     description="Python starter service",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OSINT-VDU-TNO/python-starter-service",
     include_package_data=True,
```

### Comparing `osint-python-starter-service-2.2.1/starter_service/api.py` & `osint-python-starter-service-2.2.2/starter_service/api.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.1/starter_service/api_server.py` & `osint-python-starter-service-2.2.2/starter_service/api_server.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.1/starter_service/avro_parser.py` & `osint-python-starter-service-2.2.2/starter_service/avro_parser.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.1/starter_service/base_service.py` & `osint-python-starter-service-2.2.2/starter_service/base_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,17 +21,14 @@
         self.logger = logging.getLogger(__name__)
         self.running = True
 
         # Initialize services
         self.kafka = None
         self.api = None
 
-        self.kafka_error = None
-        self.api_error = None
-
         self._initialize()
 
     @abstractmethod
     def ready(self) -> bool:
         """Return True if service is ready to receive messages, False otherwise."""
         pass
 
@@ -41,67 +38,82 @@
         pass
 
     def _initialize(self):
         """Initialize services"""
         self.name = ENV.CLIENT_ID = ENV.CLIENT_ID or self.name or self.__class__.__name__
         # Initialize schema registry
         SchemaRegistry.initialize(self.path)
-        try:
-            self.kafka = KafkaAdapter()
-            self.kafka.callback = self.kafka_callback
-            self.kafka.base_service = self
-            self.logger.info(f"Kafka initialized.")
-        except Exception as e:
-            self.kafka_error = f'Error initializing kafka: {e}'
-            self.logger.error(f'Error initializing kafka: {e}')
-            self.kafka_callback(error=e)
+        # Initialize services
+        self._init_kafka()
+        # Initialize API
+        self._init_api()
 
+    def _init_api(self):
         try:
             self.api = APIServer(name=self.name, ready=self.ready, health=self.health)
             self.api.callback = self.api_callback
             self.api.base_service = self
             self.logger.info(f"API initialized.")
         except Exception as e:
-            self.api_error = f'Error initializing API: {e}'
             self.logger.error(f'Error initializing API: {e}')
             self.api_callback(error=e)
 
+    def _init_kafka(self):
+        try:
+            self.kafka = KafkaAdapter()
+            self.kafka.callback = self.kafka_callback
+            self.kafka.base_service = self
+            self.logger.info(f"Kafka initialized.")
+        except Exception as e:
+            self.logger.error(f'Error initializing kafka: {e}')
+            self.kafka_callback(error=e)
+
     def start(self):
         """Start the service"""
         try:
+            # Start Kafka
             if self.kafka:
                 self.logger.info("Starting service Kafka...")
                 self.kafka.start()
-            self.logger.info("Starting service API...")
             # Wait for kafka to start and register schemas
+            self.logger.info("Waiting for Kafka to start and register schemas...")
             sleep(3)
-
-            # Callback
-            self.callback(kafka_error=self.kafka_error, api_error=self.api_error)
-            # Async callback
+            # Synchronous callback
+            self.callback()
+            # Asynchronous callback
             threading.Thread(target=self.async_callback, daemon=True).start()
-
+            # Start API
             if self.api:
+                self.logger.info("Starting service API...")
                 self.api.run()
-
+            # Check if services are initialized
             if self.kafka is None and self.api is None:
                 raise Exception('No services initialized. Shutting down.')
 
         except Exception as e:
             self.logger.info(f"Error starting services: {e}")
             self.stop()
 
     def stop(self):
         """Stop the service"""
         self.logger.info("Stopping service...")
-        if self.kafka:
-            self.kafka.stop()
-            self.kafka.join()
-        if self.api:
-            self.api.stop()
+        try:
+            self.logger.info("Stopping Kafka...")
+            if self.kafka:
+                self.kafka.stop()
+                # self.kafka.join()
+        except Exception as e:
+            self.logger.error(f"Error stopping Kafka: {e}")
+        try:
+            self.logger.info("Stopping API...")
+            if self.api:
+                self.api.stop()
+                # self.api.join()
+        except Exception as e:
+            self.logger.error(f"Error stopping API: {e}")
         sys.exit(0)
 
     def send_message(self, message, topic, testing=True):
         """Send message to Kafka"""
         if self.kafka is None:
             raise Exception("Kafka is not initialized")
         self.kafka.send_message(message, topics=topic, testing=testing)
```

### Comparing `osint-python-starter-service-2.2.1/starter_service/env.py` & `osint-python-starter-service-2.2.2/starter_service/env.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.1/starter_service/examples/error.py` & `osint-python-starter-service-2.2.2/starter_service/examples/error.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.1/starter_service/examples/manual_api.py` & `osint-python-starter-service-2.2.2/starter_service/examples/manual_api.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.1/starter_service/examples/manual_kafka.py` & `osint-python-starter-service-2.2.2/starter_service/examples/manual_kafka.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.1/starter_service/examples/multi.py` & `osint-python-starter-service-2.2.2/starter_service/examples/multi.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.1/starter_service/examples/offset_kafka.py` & `osint-python-starter-service-2.2.2/starter_service/examples/offset_kafka.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.1/starter_service/examples/single.py` & `osint-python-starter-service-2.2.2/starter_service/examples/single.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.1/starter_service/kafka_adapter.py` & `osint-python-starter-service-2.2.2/starter_service/kafka_adapter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 from time import sleep
 
 from starter_service.api import API
 from starter_service.env import ENV
 from starter_service.schemas import SchemaRegistry
 from starter_service.sub_process import SubProcess
-from test_bed_adapter import TestBedOptions, TestBedAdapter
+from test_bed_adapter import TestBedAdapter
+from test_bed_adapter import TestBedOptions
 from test_bed_adapter.kafka.consumer_manager import ConsumerManager
 from test_bed_adapter.kafka.log_manager import LogManager
 from test_bed_adapter.kafka.producer_manager import ProducerManager
 
 logging.basicConfig(level=logging.INFO, format='%(asctime)s %(levelname)s %(name)s %(message)s')
 
 
@@ -25,17 +26,34 @@
         # Validate environment variables
         self._validate_params()
         # Initialize test bed options
         self._init_options()
         # Initialize producers and consumers
         self._producers = {}
         self._consumers = {}
+        # Initialize logger
+        self.logger = logging.getLogger(__name__)
+        self.error_msg = None
 
     def run(self):
         """Start the service"""
+        try:
+            self._test_bed_adapter = TestBedAdapter(self._test_bed_options)
+            self.logger = LogManager(options=self._test_bed_options)
+            self.logger.info(f"Kafka ClientId[{ENV.CLIENT_ID}], Consume[{ENV.CONSUME}], Produce[{ENV.PRODUCE}]")
+            self.connect()
+            self.error_msg = None
+        except Exception as e:
+            self.error_msg = f"Error starting service: {e}"
+            self.logger.error(f"Error starting service: {e}, Restarting... in 30 seconds")
+            sleep(30)
+            self.run()
+
+    def connect(self):
+        """Start the service"""
         self._init_producers()
         self._test_bed_adapter.initialize()
         self._init_logger()
         # Create threads for each consume topic
         for topic in ENV.CONSUME.split(','):
             topic = topic.strip()
             if not topic:
@@ -61,19 +79,30 @@
             try:
                 consumer.start()
                 self.logger.info(f"Initializing listener for topic {topic}")
             except:
                 self.logger.error("Could not start consumer")
 
         while self.running:
-            sleep(1)
+            for consumer in self._consumers.values():
+                if not consumer.is_alive():
+                    self.logger.error("Consumer thread died, exiting...")
+                    self.running = False
+                    break
+            sleep(10)
 
         for consumer in self._consumers.values():
-            consumer.stop()
-            consumer.join()
+            try:
+                consumer.stop()
+                consumer.join()
+            except:
+                self.logger.error("Could not stop consumer")
+
+        self.logger.info("Stopping service...")
+        self.base_service.stop()
 
     def send_message(self, message, topics=None, testing=False):
         """Send message to kafka topic"""
         if testing:
             self.logger.info(f"Sending test message to {topics}\n{message}")
             return
 
@@ -130,19 +159,14 @@
             "offset_type": ENV.OFFSET_TYPE,
             "heartbeat_interval": ENV.HEARTBEAT_INTERVAL,
             "string_based_keys": ENV.STRING_BASED_KEYS,
             "ignore_timeout": ENV.IGNORE_TIMEOUT,
             "use_latest": ENV.USE_LATEST
         }
         self._test_bed_options = TestBedOptions(_options)
-        self._test_bed_adapter = TestBedAdapter(self._test_bed_options)
-        self.logger = LogManager(options=self._test_bed_options)
-        self.logger.info(
-            f"Initializing kafka: ClientId[{ENV.CLIENT_ID}], Consume[{ENV.CONSUME}], Produce[{ENV.PRODUCE}]")
-        self.logger.info(f"Connected to kafka: {_options}")
 
     def _handle_message(self, message, topic):
         self.logger.info(f"Received message for topic {topic}")
         if ENV.DEBUG:
             self.logger.info(f"Message {message}")
 
         funcs = API.get_func_by_consumer(topic)
```

### Comparing `osint-python-starter-service-2.2.1/starter_service/schemas.py` & `osint-python-starter-service-2.2.2/starter_service/schemas.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.1/starter_service/sub_process.py` & `osint-python-starter-service-2.2.2/starter_service/sub_process.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.1/starter_service/tests/employee.py` & `osint-python-starter-service-2.2.2/starter_service/tests/employee.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.1/starter_service/tests/teet.py` & `osint-python-starter-service-2.2.2/starter_service/tests/teet.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.2.1/starter_service/tests/test_avro_parser.py` & `osint-python-starter-service-2.2.2/starter_service/tests/test_avro_parser.py`

 * *Files identical despite different names*

