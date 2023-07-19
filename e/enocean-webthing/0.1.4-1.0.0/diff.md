# Comparing `tmp/enocean_webthing-0.1.4.tar.gz` & `tmp/enocean_webthing-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/enocean_webthing-0.1.4.tar", last modified: Sat Jul 15 13:32:50 2023, max compression
+gzip compressed data, was "dist/enocean_webthing-1.0.0.tar", last modified: Wed Jul 19 05:28:50 2023, max compression
```

## Comparing `enocean_webthing-0.1.4.tar` & `enocean_webthing-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:32:50.000000 enocean_webthing-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-15 13:32:50.000000 enocean_webthing-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-15 13:32:35.000000 enocean_webthing-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:32:50.000000 enocean_webthing-0.1.4/enocean_webthing/
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-15 13:32:35.000000 enocean_webthing-0.1.4/enocean_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-15 13:32:35.000000 enocean_webthing-0.1.4/enocean_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-15 13:32:35.000000 enocean_webthing-0.1.4/enocean_webthing/enocean_thing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-07-15 13:32:35.000000 enocean_webthing-0.1.4/enocean_webthing/enocean_webthing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:32:50.000000 enocean_webthing-0.1.4/enocean_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-15 13:32:49.000000 enocean_webthing-0.1.4/enocean_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-15 13:32:50.000000 enocean_webthing-0.1.4/enocean_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 13:32:49.000000 enocean_webthing-0.1.4/enocean_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-15 13:32:49.000000 enocean_webthing-0.1.4/enocean_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-15 13:32:49.000000 enocean_webthing-0.1.4/enocean_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-15 13:32:49.000000 enocean_webthing-0.1.4/enocean_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 13:32:50.000000 enocean_webthing-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-15 13:32:35.000000 enocean_webthing-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:28:50.000000 enocean_webthing-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-19 05:28:50.000000 enocean_webthing-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-19 05:28:39.000000 enocean_webthing-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:28:50.000000 enocean_webthing-1.0.0/enocean_webthing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-19 05:28:39.000000 enocean_webthing-1.0.0/enocean_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-19 05:28:39.000000 enocean_webthing-1.0.0/enocean_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-19 05:28:39.000000 enocean_webthing-1.0.0/enocean_webthing/enocean_thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-07-19 05:28:39.000000 enocean_webthing-1.0.0/enocean_webthing/enocean_webthing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:28:50.000000 enocean_webthing-1.0.0/enocean_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-19 05:28:50.000000 enocean_webthing-1.0.0/enocean_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-19 05:28:50.000000 enocean_webthing-1.0.0/enocean_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 05:28:50.000000 enocean_webthing-1.0.0/enocean_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-19 05:28:50.000000 enocean_webthing-1.0.0/enocean_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-19 05:28:50.000000 enocean_webthing-1.0.0/enocean_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-19 05:28:50.000000 enocean_webthing-1.0.0/enocean_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 05:28:50.000000 enocean_webthing-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-19 05:28:39.000000 enocean_webthing-1.0.0/setup.py
```

### Comparing `enocean_webthing-0.1.4/PKG-INFO` & `enocean_webthing-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enocean_webthing
-Version: 0.1.4
+Version: 1.0.0
 Summary: A web connected enocean gateway
 Home-page: https://github.com/grro/enocean_webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: UNKNOWN
 Description: # enocean_webthing
         A web connected enocean gateway. This project provides a [webthing API](https://iot.mozilla.org/wot/) to an enocean gateway such as the  [EnOcean USB 300 USB-Gateway](https://www.enocean.com/de/produkt/usb-300-500u-400j/)
```

### Comparing `enocean_webthing-0.1.4/README.md` & `enocean_webthing-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `enocean_webthing-0.1.4/enocean_webthing/__init__.py` & `enocean_webthing-1.0.0/enocean_webthing/__init__.py`

 * *Files identical despite different names*

### Comparing `enocean_webthing-0.1.4/enocean_webthing/app.py` & `enocean_webthing-1.0.0/enocean_webthing/app.py`

 * *Files identical despite different names*

### Comparing `enocean_webthing-0.1.4/enocean_webthing/enocean_thing.py` & `enocean_webthing-1.0.0/enocean_webthing/enocean_thing.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,18 @@
         self.sender = enocean_id.upper()
         self.sender_hex_string: List[int] = enocean.utils.from_hex_string(self.sender)
         self.eep_id = eep_id.upper()
         self.eep_id_hex_string: List[int] = enocean.utils.from_hex_string(self.eep_id)
         logging.info("window handle (eep_id: " + eep_id + ", enocean_id: " + enocean_id +")")
 
     @property
+    def closed(self) -> bool:
+        return self.state_text == "CLOSED"
+
+    @property
     def state(self) -> int:
         return self.db.get("state", 3)
 
     @property
     def state_text(self) -> str:
         if self.state == 1:
             return "TILTED"
@@ -60,15 +64,15 @@
         is_handled = False
         try:
             if self.eep_id_hex_string[0] == 0xf6 and packet.packet_type == PACKET.RADIO_ERP1 and packet.rorg == RORG.RPS:
                 packet.parse_eep(self.eep_id_hex_string[1], self.eep_id_hex_string[2])
                 state = packet.parsed['WIN']['raw_value']  #  WIN: {'description': 'Window handle', 'unit': '', 'value': 'Moved from vertical to down', 'raw_value': 3}
                 if self.sender == packet.sender_hex:
                     self.db.put("state", state)
-                    logging.info(self.name + " state updated " + self.state_text)
+                    logging.info(self.name + " state updated " + str(self.state) + " (" + self.state_text + ")")
                     self.listener.on_updated(self)
                     is_handled = True
         except Exception as e:
             logging.warning("error occurred by handling packet", e)
         return is_handled
```

### Comparing `enocean_webthing-0.1.4/enocean_webthing/enocean_webthing.py` & `enocean_webthing-1.0.0/enocean_webthing/enocean_webthing.py`

 * *Files 24% similar despite different names*

```diff
@@ -56,44 +56,57 @@
                      metadata={
                          'title': 'enocean id',
                          "type": "string",
                          'description': '"The enocean id',
                          'readOnly': True,
                      }))
 
-        self.state = Value(3)
+        self.state = Value(self.device.state)
         self.add_property(
             Property(self,
                      'state',
                      self.state,
                      metadata={
                          'title': 'State',
                          "type": "integer",
                          'description': 'The state of the handle',
                          'readOnly': True,
                      }))
 
-        self.state_text = Value("CLOSED")
+        self.state_text = Value(self.device.state_text)
         self.add_property(
             Property(self,
                      'state_text',
                      self.state_text,
                      metadata={
                          'title': 'State Description',
                          "type": "string",
                          'description': 'The state description',
                          'readOnly': True,
                      }))
 
+        self.closed = Value(self.device.closed)
+        self.add_property(
+            Property(self,
+                     'closed',
+                     self.closed,
+                     metadata={
+                         'title': 'Closed state',
+                         "type": "boolean",
+                         'description': 'True, if closed',
+                         'readOnly': True,
+                     }))
+
     def on_updated(self, device: WindowHandle):
         self.ioloop.add_callback(self.__update_state, device)
 
     def __update_state(self, device: WindowHandle):
         self.state.notify_of_external_update(device.state)
         self.state_text.notify_of_external_update(device.state_text)
+        self.closed.notify_of_external_update(device.closed)
 
 def run_server(port: int, description: str, path: str, addresses: List[str]):
     enocean_webthings = []
     for address in sorted(addresses):
         name, eep_id, enocean_id = address.split("/")
         if WindowHandle.supports(eep_id):
             enocean_webthings.append(WindowHandleWebThing(description, name, eep_id, enocean_id))
```

### Comparing `enocean_webthing-0.1.4/enocean_webthing.egg-info/PKG-INFO` & `enocean_webthing-1.0.0/enocean_webthing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enocean-webthing
-Version: 0.1.4
+Version: 1.0.0
 Summary: A web connected enocean gateway
 Home-page: https://github.com/grro/enocean_webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: UNKNOWN
 Description: # enocean_webthing
         A web connected enocean gateway. This project provides a [webthing API](https://iot.mozilla.org/wot/) to an enocean gateway such as the  [EnOcean USB 300 USB-Gateway](https://www.enocean.com/de/produkt/usb-300-500u-400j/)
```

### Comparing `enocean_webthing-0.1.4/setup.py` & `enocean_webthing-1.0.0/setup.py`

 * *Files identical despite different names*

