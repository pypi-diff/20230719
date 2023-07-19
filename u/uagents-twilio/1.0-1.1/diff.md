# Comparing `tmp/uagents_twilio-1.0.tar.gz` & `tmp/uagents_twilio-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uagents_twilio-1.0.tar", max compression
+gzip compressed data, was "uagents_twilio-1.1.tar", max compression
```

## Comparing `uagents_twilio-1.0.tar` & `uagents_twilio-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1073 2023-07-19 05:51:51.560628 uagents_twilio-1.0/LICENSE
--rw-r--r--   0        0        0      576 2023-07-19 05:51:51.560628 uagents_twilio-1.0/README.rst
--rw-r--r--   0        0        0      870 2023-07-19 05:52:12.353499 uagents_twilio-1.0/pyproject.toml
--rw-r--r--   0        0        0       68 2023-07-19 05:51:51.564628 uagents_twilio-1.0/uagents_twilio/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 05:51:51.564628 uagents_twilio-1.0/uagents_twilio/gc_integration/__init__.py
--rw-r--r--   0        0        0     1727 2023-07-19 05:51:51.564628 uagents_twilio-1.0/uagents_twilio/gc_integration/constants.py
--rw-r--r--   0        0        0    14304 2023-07-19 05:51:51.564628 uagents_twilio-1.0/uagents_twilio/gc_integration/google_calendar.py
--rw-r--r--   0        0        0     1229 2023-07-19 05:51:51.564628 uagents_twilio-1.0/uagents_twilio/gc_integration/utils.py
--rw-r--r--   0        0        0      125 2023-07-19 05:51:51.564628 uagents_twilio-1.0/uagents_twilio/models.py
--rw-r--r--   0        0        0        0 2023-07-19 05:51:51.564628 uagents_twilio-1.0/uagents_twilio/protocols/__init__.py
--rw-r--r--   0        0        0     1878 2023-07-19 05:51:51.564628 uagents_twilio-1.0/uagents_twilio/protocols/message.py
--rw-r--r--   0        0        0      555 2023-07-19 05:51:51.564628 uagents_twilio-1.0/uagents_twilio/webhook.py
--rw-r--r--   0        0        0        0 2023-07-19 05:51:51.564628 uagents_twilio-1.0/uagents_twilio/wrappers/__init__.py
--rw-r--r--   0        0        0     1964 2023-07-19 05:51:51.564628 uagents_twilio-1.0/uagents_twilio/wrappers/messageWrapper.py
--rw-r--r--   0        0        0     1582 1970-01-01 00:00:00.000000 uagents_twilio-1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-19 07:23:47.980330 uagents_twilio-1.1/LICENSE
+-rw-r--r--   0        0        0      576 2023-07-19 07:23:47.980330 uagents_twilio-1.1/README.rst
+-rw-r--r--   0        0        0      870 2023-07-19 07:24:04.428514 uagents_twilio-1.1/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-07-19 07:23:47.984330 uagents_twilio-1.1/uagents_twilio/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 07:23:47.984330 uagents_twilio-1.1/uagents_twilio/gc_integration/__init__.py
+-rw-r--r--   0        0        0     1727 2023-07-19 07:23:47.984330 uagents_twilio-1.1/uagents_twilio/gc_integration/constants.py
+-rw-r--r--   0        0        0    14304 2023-07-19 07:23:47.984330 uagents_twilio-1.1/uagents_twilio/gc_integration/google_calendar.py
+-rw-r--r--   0        0        0     1229 2023-07-19 07:23:47.984330 uagents_twilio-1.1/uagents_twilio/gc_integration/utils.py
+-rw-r--r--   0        0        0      125 2023-07-19 07:23:47.984330 uagents_twilio-1.1/uagents_twilio/models.py
+-rw-r--r--   0        0        0        0 2023-07-19 07:23:47.984330 uagents_twilio-1.1/uagents_twilio/protocols/__init__.py
+-rw-r--r--   0        0        0     1909 2023-07-19 07:23:47.984330 uagents_twilio-1.1/uagents_twilio/protocols/message.py
+-rw-r--r--   0        0        0      555 2023-07-19 07:23:47.984330 uagents_twilio-1.1/uagents_twilio/webhook.py
+-rw-r--r--   0        0        0        0 2023-07-19 07:23:47.984330 uagents_twilio-1.1/uagents_twilio/wrappers/__init__.py
+-rw-r--r--   0        0        0     1964 2023-07-19 07:23:47.984330 uagents_twilio-1.1/uagents_twilio/wrappers/messageWrapper.py
+-rw-r--r--   0        0        0     1582 1970-01-01 00:00:00.000000 uagents_twilio-1.1/PKG-INFO
```

### Comparing `uagents_twilio-1.0/LICENSE` & `uagents_twilio-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uagents_twilio-1.0/README.rst` & `uagents_twilio-1.1/README.rst`

 * *Files identical despite different names*

### Comparing `uagents_twilio-1.0/pyproject.toml` & `uagents_twilio-1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "uagents-twilio"
 #
-version = "1.0"
+version = "1.1"
 #
 description = ""
 authors = ["Harsh <harsh@gmail.com>"]
 readme = "README.rst"
 repository = "https://github.com/Github User/uagents-twilio"
 packages = [{include = "uagents_twilio"}]
 classifiers=[
```

### Comparing `uagents_twilio-1.0/uagents_twilio/gc_integration/constants.py` & `uagents_twilio-1.1/uagents_twilio/gc_integration/constants.py`

 * *Files identical despite different names*

### Comparing `uagents_twilio-1.0/uagents_twilio/gc_integration/google_calendar.py` & `uagents_twilio-1.1/uagents_twilio/gc_integration/google_calendar.py`

 * *Files identical despite different names*

### Comparing `uagents_twilio-1.0/uagents_twilio/gc_integration/utils.py` & `uagents_twilio-1.1/uagents_twilio/gc_integration/utils.py`

 * *Files identical despite different names*

### Comparing `uagents_twilio-1.0/uagents_twilio/protocols/message.py` & `uagents_twilio-1.1/uagents_twilio/protocols/message.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from decouple import config
-from models import WhatsAppMsg
 from uagents import Context, Protocol
-from wrappers.messageWrapper import WhatsappClient
+
+from uagents_twilio.models import WhatsAppMsg
+from uagents_twilio.wrappers.messageWrapper import WhatsappClient
 
 service_agent = Protocol()
 
 AGENT1_EMAIL = config("AGENT1_EMAIL")
 AGENT2_EMAIL = config("AGENT2_EMAIL")
 
 # gc = GoogleCalendar(
```

### Comparing `uagents_twilio-1.0/uagents_twilio/webhook.py` & `uagents_twilio-1.1/uagents_twilio/webhook.py`

 * *Files identical despite different names*

### Comparing `uagents_twilio-1.0/uagents_twilio/wrappers/messageWrapper.py` & `uagents_twilio-1.1/uagents_twilio/wrappers/messageWrapper.py`

 * *Files identical despite different names*

### Comparing `uagents_twilio-1.0/PKG-INFO` & `uagents_twilio-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uagents-twilio
-Version: 1.0
+Version: 1.1
 Summary: 
 Home-page: https://github.com/Github User/uagents-twilio
 Author: Harsh
 Author-email: harsh@gmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

