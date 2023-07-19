# Comparing `tmp/terminal_manager-0.8.2.tar.gz` & `tmp/terminal_manager-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal_manager-0.8.2.tar", last modified: Mon Jul 17 08:30:40 2023, max compression
+gzip compressed data, was "terminal_manager-0.8.3.tar", last modified: Wed Jul 19 07:55:12 2023, max compression
```

## Comparing `terminal_manager-0.8.2.tar` & `terminal_manager-0.8.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 08:30:40.466247 terminal_manager-0.8.2/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:30.000000 terminal_manager-0.8.2/LICENSE
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-17 08:30:40.466247 terminal_manager-0.8.2/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      107 2023-07-11 04:42:30.000000 terminal_manager-0.8.2/README.md
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      706 2023-07-17 08:27:15.000000 terminal_manager-0.8.2/pyproject.toml
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-17 08:30:40.466247 terminal_manager-0.8.2/setup.cfg
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 08:30:40.458247 terminal_manager-0.8.2/src/
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 08:30:40.462247 terminal_manager-0.8.2/src/terminal_manager/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     7006 2023-07-17 07:25:30.000000 terminal_manager-0.8.2/src/terminal_manager/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3352 2023-07-17 07:25:30.000000 terminal_manager-0.8.2/src/terminal_manager/collection.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     6322 2023-07-17 07:25:30.000000 terminal_manager-0.8.2/src/terminal_manager/command.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 08:30:40.466247 terminal_manager-0.8.2/src/terminal_manager/default_collections/
--rw-r--r--   0 adrian    (1000) adrian    (1000)      161 2023-07-17 07:25:30.000000 terminal_manager-0.8.2/src/terminal_manager/default_collections/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1084 2023-07-17 07:25:30.000000 terminal_manager-0.8.2/src/terminal_manager/default_collections/const.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     4359 2023-07-17 08:14:03.000000 terminal_manager-0.8.2/src/terminal_manager/default_collections/linux.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5206 2023-07-17 07:25:30.000000 terminal_manager-0.8.2/src/terminal_manager/default_collections/windows_cmd.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5374 2023-07-17 07:25:30.000000 terminal_manager-0.8.2/src/terminal_manager/default_collections/windows_ps.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)       94 2023-07-17 07:25:30.000000 terminal_manager-0.8.2/src/terminal_manager/errors.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      617 2023-07-17 07:25:30.000000 terminal_manager-0.8.2/src/terminal_manager/event.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      222 2023-07-17 07:25:30.000000 terminal_manager-0.8.2/src/terminal_manager/helpers.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8387 2023-07-17 07:25:30.000000 terminal_manager-0.8.2/src/terminal_manager/sensor.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1248 2023-07-17 07:25:30.000000 terminal_manager-0.8.2/src/terminal_manager/synchronizer.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-17 08:30:40.466247 terminal_manager-0.8.2/src/terminal_manager.egg-info/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-17 08:30:40.000000 terminal_manager-0.8.2/src/terminal_manager.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      776 2023-07-17 08:30:40.000000 terminal_manager-0.8.2/src/terminal_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-17 08:30:40.000000 terminal_manager-0.8.2/src/terminal_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       22 2023-07-17 08:30:40.000000 terminal_manager-0.8.2/src/terminal_manager.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       17 2023-07-17 08:30:40.000000 terminal_manager-0.8.2/src/terminal_manager.egg-info/top_level.txt
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-19 07:55:12.733609 terminal_manager-0.8.3/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:30.000000 terminal_manager-0.8.3/LICENSE
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-19 07:55:12.733609 terminal_manager-0.8.3/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      107 2023-07-11 04:42:30.000000 terminal_manager-0.8.3/README.md
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      706 2023-07-19 07:53:42.000000 terminal_manager-0.8.3/pyproject.toml
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-19 07:55:12.733609 terminal_manager-0.8.3/setup.cfg
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-19 07:55:12.725609 terminal_manager-0.8.3/src/
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-19 07:55:12.729609 terminal_manager-0.8.3/src/terminal_manager/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     7006 2023-07-17 08:57:09.000000 terminal_manager-0.8.3/src/terminal_manager/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     3352 2023-07-17 08:57:09.000000 terminal_manager-0.8.3/src/terminal_manager/collection.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     6319 2023-07-19 07:46:27.000000 terminal_manager-0.8.3/src/terminal_manager/command.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-19 07:55:12.729609 terminal_manager-0.8.3/src/terminal_manager/default_collections/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      161 2023-07-17 08:57:09.000000 terminal_manager-0.8.3/src/terminal_manager/default_collections/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1084 2023-07-17 08:57:09.000000 terminal_manager-0.8.3/src/terminal_manager/default_collections/const.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     4371 2023-07-19 07:37:33.000000 terminal_manager-0.8.3/src/terminal_manager/default_collections/linux.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5206 2023-07-17 08:57:09.000000 terminal_manager-0.8.3/src/terminal_manager/default_collections/windows_cmd.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5368 2023-07-19 07:26:17.000000 terminal_manager-0.8.3/src/terminal_manager/default_collections/windows_ps.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)       94 2023-07-17 08:57:09.000000 terminal_manager-0.8.3/src/terminal_manager/errors.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      617 2023-07-17 08:57:09.000000 terminal_manager-0.8.3/src/terminal_manager/event.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      222 2023-07-17 08:57:09.000000 terminal_manager-0.8.3/src/terminal_manager/helpers.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8387 2023-07-17 08:57:09.000000 terminal_manager-0.8.3/src/terminal_manager/sensor.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1248 2023-07-17 08:57:09.000000 terminal_manager-0.8.3/src/terminal_manager/synchronizer.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-19 07:55:12.729609 terminal_manager-0.8.3/src/terminal_manager.egg-info/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-19 07:55:12.000000 terminal_manager-0.8.3/src/terminal_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      776 2023-07-19 07:55:12.000000 terminal_manager-0.8.3/src/terminal_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-19 07:55:12.000000 terminal_manager-0.8.3/src/terminal_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       22 2023-07-19 07:55:12.000000 terminal_manager-0.8.3/src/terminal_manager.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       17 2023-07-19 07:55:12.000000 terminal_manager-0.8.3/src/terminal_manager.egg-info/top_level.txt
```

### Comparing `terminal_manager-0.8.2/LICENSE` & `terminal_manager-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.2/PKG-INFO` & `terminal_manager-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal_manager
-Version: 0.8.2
+Version: 0.8.3
 Summary: Use terminal commands to control and monitor devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
 Keywords: terminal,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `terminal_manager-0.8.2/pyproject.toml` & `terminal_manager-0.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "terminal_manager"
-version = "0.8.2"
+version = "0.8.3"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Use terminal commands to control and monitor devices"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `terminal_manager-0.8.2/src/terminal_manager/__init__.py` & `terminal_manager-0.8.3/src/terminal_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.2/src/terminal_manager/collection.py` & `terminal_manager-0.8.3/src/terminal_manager/collection.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.2/src/terminal_manager/command.py` & `terminal_manager-0.8.3/src/terminal_manager/command.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import annotations
 
+import re as _re
 from collections.abc import Callable
 from dataclasses import KW_ONLY, dataclass, field
 from string import Template
 from time import time
 from typing import TYPE_CHECKING
 
 from .errors import CommandError
 from .helpers import name_to_key
 from .sensor import Sensor
 
 if TYPE_CHECKING:
     from . import CommandOutput, Manager
 
-SENSOR_DELIMITER = "@sensor"
-VARIABLE_DELIMITER = "@variable"
-SHORTCUTS = ["id", "value"]
+SENSOR_DELIMITER = "#"
+VARIABLE_DELIMITER = "@"
 PLACEHOLDER_KEY = "_"
 
 
 # Not needed anymore after python 3.11
 class Template(Template):
     def get_identifiers(self):
         ids = []
@@ -34,41 +34,50 @@
             ):
                 raise ValueError("Unrecognized named group in pattern", self.pattern)
         return ids
 
 
 class SensorTemplate(Template):
     delimiter = SENSOR_DELIMITER
+    pattern = rf"""
+    {_re.escape(delimiter)}{{(?:
+      (?P<braced>{Template.idpattern})|
+      (?P<invalid>)|
+      (?P<named>)|
+      (?P<escaped>)
+    )}}
+    """
 
 
 class VariableTemplate(Template):
     delimiter = VARIABLE_DELIMITER
+    pattern = rf"""
+    {_re.escape(delimiter)}{{(?:
+      (?P<braced>{Template.idpattern})|
+      (?P<invalid>)|
+      (?P<named>)|
+      (?P<escaped>)
+    )}}
+    """
 
 
 @dataclass
 class Command:
     string: str
     _: KW_ONLY
     timeout: float | None = None
     renderer: Callable[[str], str] | None = None
 
     @property
     def required_variables(self) -> set[str]:
-        string = self._replace_shortcuts(self.string)
-        return set(VariableTemplate(string).get_identifiers())
+        return set(VariableTemplate(self.string).get_identifiers())
 
     @property
     def required_sensors(self) -> set[str]:
-        string = self._replace_shortcuts(self.string)
-        return set(SensorTemplate(string).get_identifiers())
-
-    def _replace_shortcuts(self, string: str) -> str:
-        for name in SHORTCUTS:
-            string = string.replace(f"@{name}", f"{VARIABLE_DELIMITER}{{{name}}}")
-        return string
+        return set(SensorTemplate(self.string).get_identifiers())
 
     def _render(self, string: str) -> str:
         if self.renderer:
             string = self.renderer(string)
         return string
 
     async def async_generate_string(
@@ -79,20 +88,20 @@
         """Generate the string.
 
         Raises:
             CommandError
         """
         variables = variables or {}
         sensor_values_by_key = {}
-        string = self._replace_shortcuts(self.string)
+        string = self.string
 
         try:
             string = VariableTemplate(string).substitute(variables)
         except Exception as exc:
-            raise CommandError(f"Failed to substitute variables ({exc})")
+            raise CommandError(f"Failed to substitute variable ({exc})")
 
         try:
             sensors = await manager.async_poll_sensors(self.required_sensors)
         except Exception as exc:
             raise CommandError(f"Failed to poll sensors ({exc})")
 
         for sensor in sensors:
@@ -100,15 +109,15 @@
                 sensor_values_by_key[sensor.key] = sensor.value
             else:
                 raise CommandError(f"Value of sensor {sensor.key} is None")
 
         try:
             string = SensorTemplate(string).substitute(sensor_values_by_key)
         except Exception as exc:
-            raise CommandError(f"Failed to substitute sensors ({exc})") from exc
+            raise CommandError(f"Failed to substitute sensor ({exc})") from exc
 
         try:
             return self._render(string)
         except Exception as exc:
             raise CommandError(f"Failed to render string ({exc})")
 
     async def async_execute(
```

### Comparing `terminal_manager-0.8.2/src/terminal_manager/default_collections/const.py` & `terminal_manager-0.8.3/src/terminal_manager/default_collections/const.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.2/src/terminal_manager/default_collections/linux.py` & `terminal_manager-0.8.3/src/terminal_manager/default_collections/linux.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,24 +25,24 @@
                 TextSensor(
                     SensorName.NETWORK_INTERFACE,
                     SensorKey.NETWORK_INTERFACE,
                 )
             ],
         ),
         SensorCommand(
-            "cat /sys/class/net/@sensor{network_interface}/address",
+            "cat /sys/class/net/#{network_interface}/address",
             sensors=[
                 TextSensor(
                     SensorName.MAC_ADDRESS,
                     SensorKey.MAC_ADDRESS,
                 )
             ],
         ),
         SensorCommand(
-            "cat /sys/class/net/@sensor{network_interface}/device/power/wakeup 2>/dev/null",
+            "cat /sys/class/net/#{network_interface}/device/power/wakeup 2>/dev/null",
             sensors=[
                 BinarySensor(
                     SensorName.WAKE_ON_LAN,
                     SensorKey.WAKE_ON_LAN,
                 )
             ],
         ),
@@ -101,16 +101,18 @@
                     SensorKey.FREE_MEMORY,
                     unit="KiB",
                 )
             ],
         ),
         SensorCommand(
             "df -k | awk '/^\/dev\// {"
-            + 'x=$0; sub(/^[^ ]+ +[^ ]+ +[^ ]+ +[^ ]+ +[^ ]+ /,"",x); '
-            + 'print x "|" $4}\'',
+            + "x=$4; "
+            + '$1=$2=$3=$4=$5=""; '
+            + 'sub(/^ +/, "", $0); '
+            + 'print $0 "|" x}\'',
             interval=60,
             sensors=[
                 NumberSensor(
                     SensorName.FREE_DISK_SPACE,
                     SensorKey.FREE_DISK_SPACE,
                     dynamic=True,
                     separator="|",
```

### Comparing `terminal_manager-0.8.2/src/terminal_manager/default_collections/windows_cmd.py` & `terminal_manager-0.8.3/src/terminal_manager/default_collections/windows_cmd.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.2/src/terminal_manager/default_collections/windows_ps.py` & `terminal_manager-0.8.3/src/terminal_manager/default_collections/windows_ps.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             ActionName.RESTART,
             ActionKey.RESTART,
         ),
     ],
     [
         SensorCommand(
             "$x = Get-NetAdapterPowerManagement "
-            + '-Name "@sensor{network_interface}" | '
+            + '-Name "#{network_interface}" | '
             + "Select WakeOnMagicPacket; "
             + "$x.WakeOnMagicPacket",
             sensors=[
                 BinarySensor(
                     SensorName.WAKE_ON_LAN,
                     SensorKey.WAKE_ON_LAN,
                 )
```

### Comparing `terminal_manager-0.8.2/src/terminal_manager/event.py` & `terminal_manager-0.8.3/src/terminal_manager/event.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.2/src/terminal_manager/sensor.py` & `terminal_manager-0.8.3/src/terminal_manager/sensor.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.2/src/terminal_manager/synchronizer.py` & `terminal_manager-0.8.3/src/terminal_manager/synchronizer.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.8.2/src/terminal_manager.egg-info/PKG-INFO` & `terminal_manager-0.8.3/src/terminal_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal-manager
-Version: 0.8.2
+Version: 0.8.3
 Summary: Use terminal commands to control and monitor devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
 Keywords: terminal,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `terminal_manager-0.8.2/src/terminal_manager.egg-info/SOURCES.txt` & `terminal_manager-0.8.3/src/terminal_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

