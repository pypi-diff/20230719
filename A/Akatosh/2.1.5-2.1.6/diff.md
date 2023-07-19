# Comparing `tmp/Akatosh-2.1.5.tar.gz` & `tmp/Akatosh-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Akatosh-2.1.5.tar", last modified: Tue Jul 18 06:12:28 2023, max compression
+gzip compressed data, was "Akatosh-2.1.6.tar", last modified: Wed Jul 19 04:57:01 2023, max compression
```

## Comparing `Akatosh-2.1.5.tar` & `Akatosh-2.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 06:12:28.896546 Akatosh-2.1.5/
-drwxrwxrwx   0        0        0        0 2023-07-18 06:12:28.838981 Akatosh-2.1.5/Akatosh/
--rw-rw-rw-   0        0        0      242 2023-07-12 05:21:53.000000 Akatosh-2.1.5/Akatosh/__init__.py
--rw-rw-rw-   0        0        0    14879 2023-07-18 06:06:44.000000 Akatosh-2.1.5/Akatosh/entity.py
--rw-rw-rw-   0        0        0    13327 2023-07-12 07:37:05.000000 Akatosh-2.1.5/Akatosh/event.py
--rw-rw-rw-   0        0        0      384 2023-07-12 04:33:32.000000 Akatosh-2.1.5/Akatosh/logger.py
--rw-rw-rw-   0        0        0     9111 2023-07-12 04:33:32.000000 Akatosh-2.1.5/Akatosh/resource.py
--rw-rw-rw-   0        0        0      201 2023-07-12 04:33:32.000000 Akatosh-2.1.5/Akatosh/states.py
--rw-rw-rw-   0        0        0     6148 2023-07-18 03:07:53.000000 Akatosh-2.1.5/Akatosh/universe.py
-drwxrwxrwx   0        0        0        0 2023-07-18 06:12:28.884548 Akatosh-2.1.5/Akatosh.egg-info/
--rw-rw-rw-   0        0        0     2830 2023-07-18 06:12:28.000000 Akatosh-2.1.5/Akatosh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-07-18 06:12:28.000000 Akatosh-2.1.5/Akatosh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 06:12:28.000000 Akatosh-2.1.5/Akatosh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-18 06:12:28.000000 Akatosh-2.1.5/Akatosh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2830 2023-07-18 06:12:28.893546 Akatosh-2.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2238 2023-07-12 04:33:32.000000 Akatosh-2.1.5/README.md
--rw-rw-rw-   0        0        0      635 2023-07-18 06:11:53.000000 Akatosh-2.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-18 06:12:28.896546 Akatosh-2.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-19 04:57:01.648851 Akatosh-2.1.6/
+drwxrwxrwx   0        0        0        0 2023-07-19 04:57:01.634853 Akatosh-2.1.6/Akatosh/
+-rw-rw-rw-   0        0        0      242 2023-07-13 05:05:39.000000 Akatosh-2.1.6/Akatosh/__init__.py
+-rw-rw-rw-   0        0        0    14879 2023-07-19 04:52:07.000000 Akatosh-2.1.6/Akatosh/entity.py
+-rw-rw-rw-   0        0        0    13327 2023-07-17 05:10:45.000000 Akatosh-2.1.6/Akatosh/event.py
+-rw-rw-rw-   0        0        0      384 2023-07-11 12:42:40.000000 Akatosh-2.1.6/Akatosh/logger.py
+-rw-rw-rw-   0        0        0     9111 2023-07-11 12:42:40.000000 Akatosh-2.1.6/Akatosh/resource.py
+-rw-rw-rw-   0        0        0      201 2023-07-11 12:42:40.000000 Akatosh-2.1.6/Akatosh/states.py
+-rw-rw-rw-   0        0        0     6365 2023-07-19 04:55:41.000000 Akatosh-2.1.6/Akatosh/universe.py
+drwxrwxrwx   0        0        0        0 2023-07-19 04:57:01.644852 Akatosh-2.1.6/Akatosh.egg-info/
+-rw-rw-rw-   0        0        0     2830 2023-07-19 04:57:01.000000 Akatosh-2.1.6/Akatosh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-07-19 04:57:01.000000 Akatosh-2.1.6/Akatosh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 04:57:01.000000 Akatosh-2.1.6/Akatosh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-19 04:57:01.000000 Akatosh-2.1.6/Akatosh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2830 2023-07-19 04:57:01.646852 Akatosh-2.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2238 2023-07-11 12:42:40.000000 Akatosh-2.1.6/README.md
+-rw-rw-rw-   0        0        0      635 2023-07-19 04:56:29.000000 Akatosh-2.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-19 04:57:01.649852 Akatosh-2.1.6/setup.cfg
```

### Comparing `Akatosh-2.1.5/Akatosh/entity.py` & `Akatosh-2.1.6/Akatosh/entity.py`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.5/Akatosh/event.py` & `Akatosh-2.1.6/Akatosh/event.py`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.5/Akatosh/resource.py` & `Akatosh-2.1.6/Akatosh/resource.py`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.5/Akatosh/universe.py` & `Akatosh-2.1.6/Akatosh/universe.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 if TYPE_CHECKING:
     from .event import Event
 
 
 class Universe:
     def __init__(self) -> None:
         """The Simulation Universe."""
-        self._resolution = (
-            1  # the resolution of the time. 1 means minimum time unit is 0.1 second.
-        )
+        self._resolution = 15  # the resolution of the time. 1 means minimum time unit is 0.1 second.
         self._now: int | float = -1  # the current time of the simulated universe.
         self._future_events: List[Event] = list()  # the future events queue.
         self._current_events: List[Event] = list()  # the current events queue.
         self._past_events: List[Event] = list()  # the past events queue.
         self._alduin: bool = False  # trigger to stop the simulation.
         self.set_logger(logging.ERROR)  # set the default logger level to ERROR.
 
@@ -127,14 +125,21 @@
         """Set the logger level."""
         logger.setLevel(level)
 
     @property
     def resolution(self) -> int:
         """Return  the resolution of the time."""
         return self._resolution
+    
+    @resolution.setter
+    def resolution(self, value: int):
+        """Set the resolution of the time."""
+        if value <= 0:
+            raise ValueError("Resolution must be greater than 0.")
+        self._resolution = value
 
     @property
     def now(self) -> int | float:
         """Return the current time of the simulated universe."""
         return self._now
 
     @property
```

### Comparing `Akatosh-2.1.5/Akatosh.egg-info/PKG-INFO` & `Akatosh-2.1.6/Akatosh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 2.1.5
+Version: 2.1.6
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Documentation, https://ulfaric.github.io/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Akatosh-2.1.5/PKG-INFO` & `Akatosh-2.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 2.1.5
+Version: 2.1.6
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Documentation, https://ulfaric.github.io/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Akatosh-2.1.5/README.md` & `Akatosh-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.5/pyproject.toml` & `Akatosh-2.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Akatosh"
-version = "2.1.5"
+version = "2.1.6"
 authors = [{ name = "Yifei Ren", email = "ryf0510@live.com" }]
 description = "A simple implement for discrete events simulation."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

