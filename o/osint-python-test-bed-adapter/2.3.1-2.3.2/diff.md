# Comparing `tmp/osint-python-test-bed-adapter-2.3.1.tar.gz` & `tmp/osint-python-test-bed-adapter-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osint-python-test-bed-adapter-2.3.1.tar", last modified: Fri Jun 23 00:54:39 2023, max compression
+gzip compressed data, was "osint-python-test-bed-adapter-2.3.2.tar", last modified: Wed Jul 19 11:49:17 2023, max compression
```

## Comparing `osint-python-test-bed-adapter-2.3.1.tar` & `osint-python-test-bed-adapter-2.3.2.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-23 00:54:39.646283 osint-python-test-bed-adapter-2.3.1/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-test-bed-adapter-2.3.1/LICENSE
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3592 2023-06-23 00:54:39.646283 osint-python-test-bed-adapter-2.3.1/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3165 2023-06-13 08:56:50.000000 osint-python-test-bed-adapter-2.3.1/README.md
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-23 00:54:39.646283 osint-python-test-bed-adapter-2.3.1/osint_python_test_bed_adapter.egg-info/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3592 2023-06-23 00:54:39.000000 osint-python-test-bed-adapter-2.3.1/osint_python_test_bed_adapter.egg-info/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      703 2023-06-23 00:54:39.000000 osint-python-test-bed-adapter-2.3.1/osint_python_test_bed_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-06-23 00:54:39.000000 osint-python-test-bed-adapter-2.3.1/osint_python_test_bed_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       39 2023-06-23 00:54:39.000000 osint-python-test-bed-adapter-2.3.1/osint_python_test_bed_adapter.egg-info/requires.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       17 2023-06-23 00:54:39.000000 osint-python-test-bed-adapter-2.3.1/osint_python_test_bed_adapter.egg-info/top_level.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-06-23 00:54:39.646283 osint-python-test-bed-adapter-2.3.1/setup.cfg
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      758 2023-06-23 00:50:22.000000 osint-python-test-bed-adapter-2.3.1/setup.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-23 00:54:39.646283 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1389 2023-06-17 00:32:44.000000 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/__init__.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-23 00:54:39.646283 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/kafka/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       68 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/kafka/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3897 2023-06-23 00:52:25.000000 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/kafka/consumer_manager.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1699 2023-06-16 22:08:43.000000 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/kafka/heartbeat_manager.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3074 2023-06-23 00:54:19.000000 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/kafka/log_manager.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2102 2023-06-17 00:23:16.000000 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/kafka/producer_manager.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-23 00:54:39.646283 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/options/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       31 2022-04-23 22:07:41.000000 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/options/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3486 2023-06-01 22:28:40.000000 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/options/test_bed_options.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-23 00:54:39.646283 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/utils/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       22 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/utils/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      598 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/utils/helpers.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1005 2023-03-16 17:51:41.000000 osint-python-test-bed-adapter-2.3.1/test_bed_adapter/utils/key.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-07-19 11:49:17.841630 osint-python-test-bed-adapter-2.3.2/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-test-bed-adapter-2.3.2/LICENSE
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3592 2023-07-19 11:49:17.841630 osint-python-test-bed-adapter-2.3.2/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3165 2023-06-13 08:56:50.000000 osint-python-test-bed-adapter-2.3.2/README.md
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-07-19 11:49:17.841630 osint-python-test-bed-adapter-2.3.2/osint_python_test_bed_adapter.egg-info/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3592 2023-07-19 11:49:17.000000 osint-python-test-bed-adapter-2.3.2/osint_python_test_bed_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      747 2023-07-19 11:49:17.000000 osint-python-test-bed-adapter-2.3.2/osint_python_test_bed_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-07-19 11:49:17.000000 osint-python-test-bed-adapter-2.3.2/osint_python_test_bed_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       39 2023-07-19 11:49:17.000000 osint-python-test-bed-adapter-2.3.2/osint_python_test_bed_adapter.egg-info/requires.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       29 2023-07-19 11:49:17.000000 osint-python-test-bed-adapter-2.3.2/osint_python_test_bed_adapter.egg-info/top_level.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-07-19 11:49:17.841630 osint-python-test-bed-adapter-2.3.2/setup.cfg
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      758 2023-07-19 11:48:44.000000 osint-python-test-bed-adapter-2.3.2/setup.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-07-19 11:49:17.841630 osint-python-test-bed-adapter-2.3.2/test_bed_adapter/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1389 2023-06-17 00:32:44.000000 osint-python-test-bed-adapter-2.3.2/test_bed_adapter/__init__.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-07-19 11:49:17.841630 osint-python-test-bed-adapter-2.3.2/test_bed_adapter/kafka/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       68 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.3.2/test_bed_adapter/kafka/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     4477 2023-07-19 11:47:27.000000 osint-python-test-bed-adapter-2.3.2/test_bed_adapter/kafka/consumer_manager.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1699 2023-06-16 22:08:43.000000 osint-python-test-bed-adapter-2.3.2/test_bed_adapter/kafka/heartbeat_manager.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3074 2023-06-23 00:54:19.000000 osint-python-test-bed-adapter-2.3.2/test_bed_adapter/kafka/log_manager.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2102 2023-06-17 00:23:16.000000 osint-python-test-bed-adapter-2.3.2/test_bed_adapter/kafka/producer_manager.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-07-19 11:49:17.841630 osint-python-test-bed-adapter-2.3.2/test_bed_adapter/options/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       31 2022-04-23 22:07:41.000000 osint-python-test-bed-adapter-2.3.2/test_bed_adapter/options/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3486 2023-06-01 22:28:40.000000 osint-python-test-bed-adapter-2.3.2/test_bed_adapter/options/test_bed_options.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-07-19 11:49:17.841630 osint-python-test-bed-adapter-2.3.2/test_bed_adapter/utils/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       22 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.3.2/test_bed_adapter/utils/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      598 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.3.2/test_bed_adapter/utils/helpers.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1005 2023-03-16 17:51:41.000000 osint-python-test-bed-adapter-2.3.2/test_bed_adapter/utils/key.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-07-19 11:49:17.841630 osint-python-test-bed-adapter-2.3.2/url_checker/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-07-10 03:35:36.000000 osint-python-test-bed-adapter-2.3.2/url_checker/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1260 2023-07-10 05:06:40.000000 osint-python-test-bed-adapter-2.3.2/url_checker/main.py
```

### Comparing `osint-python-test-bed-adapter-2.3.1/LICENSE` & `osint-python-test-bed-adapter-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.3.1/PKG-INFO` & `osint-python-test-bed-adapter-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-test-bed-adapter
-Version: 2.3.1
+Version: 2.3.2
 Summary: Python adapter for Kafka
 Home-page: https://github.com/OSINT-VDU-TNO/python-adapter
 Author: TimovdK
 Author-email: timo_kuil@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `osint-python-test-bed-adapter-2.3.1/README.md` & `osint-python-test-bed-adapter-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.3.1/osint_python_test_bed_adapter.egg-info/PKG-INFO` & `osint-python-test-bed-adapter-2.3.2/osint_python_test_bed_adapter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-test-bed-adapter
-Version: 2.3.1
+Version: 2.3.2
 Summary: Python adapter for Kafka
 Home-page: https://github.com/OSINT-VDU-TNO/python-adapter
 Author: TimovdK
 Author-email: timo_kuil@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `osint-python-test-bed-adapter-2.3.1/osint_python_test_bed_adapter.egg-info/SOURCES.txt` & `osint-python-test-bed-adapter-2.3.2/osint_python_test_bed_adapter.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -12,8 +12,10 @@
 test_bed_adapter/kafka/heartbeat_manager.py
 test_bed_adapter/kafka/log_manager.py
 test_bed_adapter/kafka/producer_manager.py
 test_bed_adapter/options/__init__.py
 test_bed_adapter/options/test_bed_options.py
 test_bed_adapter/utils/__init__.py
 test_bed_adapter/utils/helpers.py
-test_bed_adapter/utils/key.py
+test_bed_adapter/utils/key.py
+url_checker/__init__.py
+url_checker/main.py
```

### Comparing `osint-python-test-bed-adapter-2.3.1/setup.py` & `osint-python-test-bed-adapter-2.3.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="osint-python-test-bed-adapter",
-    version="2.3.1",
+    version="2.3.2",
     author="TimovdK",
     author_email="timo_kuil@hotmail.com",
     description="Python adapter for Kafka",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OSINT-VDU-TNO/python-adapter",
     include_package_data=True,
```

### Comparing `osint-python-test-bed-adapter-2.3.1/test_bed_adapter/__init__.py` & `osint-python-test-bed-adapter-2.3.2/test_bed_adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.3.1/test_bed_adapter/kafka/consumer_manager.py` & `osint-python-test-bed-adapter-2.3.2/test_bed_adapter/kafka/consumer_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from threading import Thread
 from time import time, sleep
 
-from confluent_kafka import DeserializingConsumer
+from confluent_kafka import DeserializingConsumer, KafkaError
 from confluent_kafka.schema_registry import SchemaRegistryClient
 from confluent_kafka.schema_registry.avro import AvroDeserializer
 
 from ..options.test_bed_options import TestBedOptions
 
 
 class ConsumerManager(Thread):
@@ -92,13 +92,26 @@
         if self.latest_message and self.options.use_latest:
             self.handle_message(self.latest_message.value(), self.latest_message.topic())
 
     def listen(self):
         """Listen for messages on the topic and handle them with the provided callback"""
         # Continue to listen for messages
         while self.running:
-            msg = self.consumer.poll(1)
-            if msg is None:
-                continue
-            self.handle_message(msg.value(), msg.topic())
-        # Close down consumer to commit final offsets.
+            try:
+                msg = self.consumer.poll(1)  # Adjust the timeout as needed
+                if msg is None:
+                    continue
+                if msg.error():
+                    if msg.error().code() == KafkaError._PARTITION_EOF:
+                        # Handle end of partition
+                        continue
+                    else:
+                        # Handle other Kafka errors
+                        self.logger.error(f"Kafka error: {msg.error()}")
+                        break
+                self.handle_message(msg.value(), msg.topic())
+            except Exception as e:
+                self.logger.error(f"Exception occurred: {e}")
+                break
+
+        self.logger.error(f"Consumer for {self.kafka_topic} stopped")
         self.consumer.close()
```

### Comparing `osint-python-test-bed-adapter-2.3.1/test_bed_adapter/kafka/heartbeat_manager.py` & `osint-python-test-bed-adapter-2.3.2/test_bed_adapter/kafka/heartbeat_manager.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.3.1/test_bed_adapter/kafka/log_manager.py` & `osint-python-test-bed-adapter-2.3.2/test_bed_adapter/kafka/log_manager.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.3.1/test_bed_adapter/kafka/producer_manager.py` & `osint-python-test-bed-adapter-2.3.2/test_bed_adapter/kafka/producer_manager.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.3.1/test_bed_adapter/options/test_bed_options.py` & `osint-python-test-bed-adapter-2.3.2/test_bed_adapter/options/test_bed_options.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.3.1/test_bed_adapter/utils/helpers.py` & `osint-python-test-bed-adapter-2.3.2/test_bed_adapter/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.3.1/test_bed_adapter/utils/key.py` & `osint-python-test-bed-adapter-2.3.2/test_bed_adapter/utils/key.py`

 * *Files identical despite different names*

