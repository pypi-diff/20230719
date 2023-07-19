# Comparing `tmp/mine-3.1.1.tar.gz` & `tmp/mine-4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mine-3.1.1.tar", max compression
+gzip compressed data, was "mine-4.0a1.tar", max compression
```

## Comparing `mine-3.1.1.tar` & `mine-4.0a1.tar`

### file list

```diff
@@ -1,32 +1,31 @@
--rw-r--r--   0        0        0     1088 2019-05-21 02:49:19.000000 mine-3.1.1/LICENSE.md
--rw-r--r--   0        0        0     2840 2023-04-16 19:11:58.196023 mine-3.1.1/README.md
--rw-r--r--   0        0        0      340 2023-04-16 19:25:03.010573 mine-3.1.1/mine/__init__.py
--rw-r--r--   0        0        0     6624 2023-04-16 19:11:58.197283 mine-3.1.1/mine/cli.py
--rw-r--r--   0        0        0     2865 2023-04-16 19:11:58.197615 mine-3.1.1/mine/common.py
--rw-r--r--   0        0        0     6669 2023-04-16 19:18:48.322162 mine-3.1.1/mine/manager.py
--rw-r--r--   0        0        0      232 2019-05-21 02:49:19.000000 mine-3.1.1/mine/models/__init__.py
--rw-r--r--   0        0        0      424 2021-06-02 19:31:21.821486 mine-3.1.1/mine/models/_bases.py
--rw-r--r--   0        0        0     1803 2019-05-21 02:49:19.000000 mine-3.1.1/mine/models/application.py
--rw-r--r--   0        0        0     4801 2023-07-15 20:16:13.642291 mine-3.1.1/mine/models/computer.py
--rw-r--r--   0        0        0      501 2019-05-21 02:49:19.000000 mine-3.1.1/mine/models/config.py
--rw-r--r--   0        0        0     5145 2020-05-16 16:13:05.000000 mine-3.1.1/mine/models/data.py
--rw-r--r--   0        0        0     6544 2022-09-08 17:31:06.428139 mine-3.1.1/mine/models/status.py
--rw-r--r--   0        0        0     1052 2019-05-21 02:49:19.000000 mine-3.1.1/mine/models/timestamp.py
--rwxr-xr-x   0        0        0     2667 2023-04-16 19:11:58.198225 mine-3.1.1/mine/services.py
--rw-r--r--   0        0        0      573 2023-04-16 19:13:26.811463 mine-3.1.1/mine/settings.py
--rw-r--r--   0        0        0       34 2016-09-23 05:48:42.000000 mine-3.1.1/mine/tests/__init__.py
--rw-r--r--   0        0        0     1038 2023-04-16 19:11:58.198685 mine-3.1.1/mine/tests/conftest.py
--rw-r--r--   0        0        0        9 2016-09-23 02:41:14.000000 mine-3.1.1/mine/tests/files/.gitignore
--rw-r--r--   0        0        0      513 2016-09-23 02:41:14.000000 mine-3.1.1/mine/tests/files/mine-in.yml
--rw-r--r--   0        0        0      587 2016-09-23 02:41:14.000000 mine-3.1.1/mine/tests/files/mine-out.yml
--rw-r--r--   0        0        0     3996 2023-04-16 19:11:58.199066 mine-3.1.1/mine/tests/test_cli.py
--rw-r--r--   0        0        0     3506 2023-04-16 19:11:58.199194 mine-3.1.1/mine/tests/test_manager.py
--rw-r--r--   0        0        0     1489 2023-04-16 19:11:58.199324 mine-3.1.1/mine/tests/test_models_application.py
--rw-r--r--   0        0        0     4244 2023-07-15 19:53:23.376622 mine-3.1.1/mine/tests/test_models_computer.py
--rw-r--r--   0        0        0      316 2023-04-16 19:11:58.199968 mine-3.1.1/mine/tests/test_models_config.py
--rw-r--r--   0        0        0      682 2023-04-16 19:11:58.200223 mine-3.1.1/mine/tests/test_models_data.py
--rw-r--r--   0        0        0     4961 2023-04-16 19:11:58.200402 mine-3.1.1/mine/tests/test_models_status.py
--rw-r--r--   0        0        0     1750 2023-04-16 19:11:58.200536 mine-3.1.1/mine/tests/test_models_timestamp.py
--rw-r--r--   0        0        0     3211 2023-04-16 19:21:47.166045 mine-3.1.1/mine/tests/test_services.py
--rw-r--r--   0        0        0     2294 2023-07-15 20:13:11.614336 mine-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     4366 1970-01-01 00:00:00.000000 mine-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2019-05-21 02:49:19.000000 mine-4.0a1/LICENSE.md
+-rw-r--r--   0        0        0     2840 2023-04-16 19:11:58.196023 mine-4.0a1/README.md
+-rw-r--r--   0        0        0      340 2023-04-16 19:25:03.010573 mine-4.0a1/mine/__init__.py
+-rw-r--r--   0        0        0     6860 2023-07-19 02:52:07.566131 mine-4.0a1/mine/cli.py
+-rw-r--r--   0        0        0     2889 2023-07-19 02:12:18.943946 mine-4.0a1/mine/common.py
+-rw-r--r--   0        0        0     6660 2023-07-19 03:21:57.599480 mine-4.0a1/mine/manager.py
+-rw-r--r--   0        0        0      217 2023-07-19 02:12:18.944037 mine-4.0a1/mine/models/__init__.py
+-rw-r--r--   0        0        0     1095 2023-07-19 03:18:20.515733 mine-4.0a1/mine/models/application.py
+-rw-r--r--   0        0        0     2121 2023-07-19 02:18:02.802475 mine-4.0a1/mine/models/computer.py
+-rw-r--r--   0        0        0     3721 2023-07-19 02:28:44.644217 mine-4.0a1/mine/models/config.py
+-rw-r--r--   0        0        0     5413 2023-07-19 02:28:30.879778 mine-4.0a1/mine/models/data.py
+-rw-r--r--   0        0        0     5863 2023-07-19 03:18:32.152880 mine-4.0a1/mine/models/status.py
+-rw-r--r--   0        0        0      882 2023-07-19 02:12:18.944631 mine-4.0a1/mine/models/timestamp.py
+-rwxr-xr-x   0        0        0     2720 2023-07-19 02:46:39.336705 mine-4.0a1/mine/services.py
+-rw-r--r--   0        0        0      578 2023-07-19 02:12:18.944827 mine-4.0a1/mine/settings.py
+-rw-r--r--   0        0        0       34 2016-09-23 05:48:42.000000 mine-4.0a1/mine/tests/__init__.py
+-rw-r--r--   0        0        0     1043 2023-07-19 02:12:18.944974 mine-4.0a1/mine/tests/conftest.py
+-rw-r--r--   0        0        0        9 2016-09-23 02:41:14.000000 mine-4.0a1/mine/tests/files/.gitignore
+-rw-r--r--   0        0        0      513 2016-09-23 02:41:14.000000 mine-4.0a1/mine/tests/files/mine-in.yml
+-rw-r--r--   0        0        0      587 2016-09-23 02:41:14.000000 mine-4.0a1/mine/tests/files/mine-out.yml
+-rw-r--r--   0        0        0     3994 2023-07-19 02:20:06.563001 mine-4.0a1/mine/tests/test_cli.py
+-rw-r--r--   0        0        0     3506 2023-04-16 19:11:58.199194 mine-4.0a1/mine/tests/test_manager.py
+-rw-r--r--   0        0        0     1002 2023-07-19 01:11:50.938610 mine-4.0a1/mine/tests/test_models_application.py
+-rw-r--r--   0        0        0     2193 2023-07-19 01:11:50.938810 mine-4.0a1/mine/tests/test_models_computer.py
+-rw-r--r--   0        0        0     3086 2023-07-19 02:12:18.936287 mine-4.0a1/mine/tests/test_models_config.py
+-rw-r--r--   0        0        0      682 2023-04-16 19:11:58.200223 mine-4.0a1/mine/tests/test_models_data.py
+-rw-r--r--   0        0        0     4961 2023-04-16 19:11:58.200402 mine-4.0a1/mine/tests/test_models_status.py
+-rw-r--r--   0        0        0     1750 2023-04-16 19:11:58.200536 mine-4.0a1/mine/tests/test_models_timestamp.py
+-rw-r--r--   0        0        0     3226 2023-07-19 02:41:25.796394 mine-4.0a1/mine/tests/test_services.py
+-rw-r--r--   0        0        0     2248 2023-07-19 03:18:38.846415 mine-4.0a1/pyproject.toml
+-rw-r--r--   0        0        0     4176 1970-01-01 00:00:00.000000 mine-4.0a1/PKG-INFO
```

### Comparing `mine-3.1.1/LICENSE.md` & `mine-4.0a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mine-3.1.1/README.md` & `mine-4.0a1/README.md`

 * *Files identical despite different names*

### Comparing `mine-3.1.1/mine/cli.py` & `mine-4.0a1/mine/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 
 import argparse
 import subprocess
 import sys
 import time
 
 import log
-import yorm
+from datafiles import frozen
+from datafiles.model import create_model
 from startfile import startfile
 
 from . import CLI, DESCRIPTION, VERSION, common, services
-from .manager import get_manager
-from .models import Application, Data
+from .manager import BaseManager, get_manager
+from .models import Application, Data, Versions
 
-daemon = Application(CLI, filename=CLI)
+daemon = Application(CLI, versions=Versions(mac="mine", windows="mine", linux="mine"))
 
 
 def main(args=None):
     """Process command-line arguments and run the program."""
 
     # Shared options
     debug = argparse.ArgumentParser(add_help=False)
@@ -165,47 +166,47 @@
     manager = get_manager()
     if not manager.is_running(services.APPLICATION):
         manager.start(services.APPLICATION)
 
     root = services.find_root()
     path = path or services.find_config_path(root=root)
 
-    data = Data()
-    yorm.sync(data, path)
+    data = create_model(Data, pattern=path, defaults=True)()
 
     config = data.config
     status = data.status
 
     log.info("Identifying current computer...")
-    computer = config.computers.get_current()
+    computer = config.get_current_computer()
     log.info("Current computer: %s", computer)
 
     if edit:
         return startfile(path)
     if delete:
         return services.delete_conflicts(root, force=force)
 
     if switch is True:
         switch = computer
     elif switch is False:
         data.close_all_applications(config, manager)
     elif switch:
-        switch = config.computers.match(switch)
+        switch = config.match_computer(switch)
 
     if switch:
         if switch != computer:
             data.close_all_applications(config, manager)
         data.queue_all_applications(config, status, switch)
 
     while True:
         services.delete_conflicts(root, config_only=True, force=True)
-        data.launch_queued_applications(config, status, computer, manager)
-        data.update_status(config, status, computer, manager)
+        with frozen(data):
+            data.launch_queued_applications(config, status, computer, manager)
+            data.update_status(config, status, computer, manager)
 
-        if delay is None:
+        if delay is None or delay <= 0:
             break
 
         log.info("Delaying %s seconds for files to sync...", delay)
         time.sleep(delay)
 
         step = 5
         elapsed = 0
@@ -215,23 +216,24 @@
             elapsed += step
 
         short_delay = 30
         log.info("Delaying %s seconds for files to sync...", short_delay)
         time.sleep(short_delay)
 
     if cleanup:
-        data.prune_status(config, status)
+        with frozen(data):
+            data.prune_status(config, status)
 
     if delay is None:
         return _restart_daemon(manager)
 
     return True
 
 
-def _restart_daemon(manager):
+def _restart_daemon(manager: BaseManager):
     cmd = "nohup {} --daemon --verbose >> /tmp/mine.log 2>&1 &".format(CLI)
     if daemon and not manager.is_running(daemon):
         log.warning("Daemon is not running, attempting to restart...")
 
         log.info("$ %s", cmd)
         subprocess.call(cmd, shell=True)
         if manager.is_running(daemon):
```

### Comparing `mine-3.1.1/mine/common.py` & `mine-4.0a1/mine/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,15 +68,17 @@
     # Set a custom formatter
     logging.basicConfig(level=level)
     logging.captureWarnings(True)
     formatter = WarningFormatter(
         default_format, verbose_format, datefmt=settings.LOGGING_DATEFMT
     )
     logging.root.handlers[0].setFormatter(formatter)
-    logging.getLogger("yorm").setLevel(max(level, settings.YORM_LOGGING_LEVEL))
+    logging.getLogger("datafiles").setLevel(
+        max(level, settings.DATAFILES_LOGGING_LEVEL)
+    )
 
     # Warn about excessive verbosity
     global verbosity
     if count > MAX_VERBOSITY:
         msg = "Maximum verbosity level is {}".format(MAX_VERBOSITY)
         logging.warning(msg)
         verbosity = MAX_VERBOSITY
```

### Comparing `mine-3.1.1/mine/manager.py` & `mine-4.0a1/mine/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import abc
 import functools
 import glob
 import os
 import platform
 import time
-from typing import List
 
 import log
 import psutil
 
 # TODO: delete this after implementing `BaseManager`
 # https://github.com/jacebrowning/mine/issues/8
 # https://github.com/jacebrowning/mine/issues/9
@@ -59,15 +58,15 @@
 
 
 class BaseManager(metaclass=abc.ABCMeta):  # pragma: no cover (abstract)
     """Base application manager."""
 
     NAME = FRIENDLY = ""
 
-    IGNORED_APPLICATION_NAMES: List[str] = []
+    IGNORED_APPLICATION_NAMES: list[str] = []
 
     def __str__(self):
         return self.FRIENDLY
 
     @abc.abstractmethod
     def is_running(self, application):
         """Determine if an application is currently running."""
@@ -217,15 +216,15 @@
     def start(self, application):
         pass
 
     def stop(self, application):
         pass
 
 
-def get_manager(name=None):
+def get_manager(name=None) -> BaseManager:
     """Return an application manager for the current operating system."""
     log.info("Detecting the current system...")
     name = name or platform.system()
     manager = {  # type: ignore
         WindowsManager.NAME: WindowsManager,
         MacManager.NAME: MacManager,
         LinuxManager.NAME: LinuxManager,
```

### Comparing `mine-3.1.1/mine/models/data.py` & `mine-4.0a1/mine/models/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,66 +1,70 @@
 """Data structures that combine all program data."""
 
+from dataclasses import dataclass, field
+
 import crayons
 import log
-import yorm
 
+from ..manager import BaseManager
 from .config import ProgramConfig
 from .status import ProgramStatus
 
 
-@yorm.attr(config=ProgramConfig)
-@yorm.attr(status=ProgramStatus)
+@dataclass
 class Data:
     """Primary wrapper for all settings."""
 
-    def __init__(self):
-        self.config = ProgramConfig()
-        self.status = ProgramStatus()
+    config: ProgramConfig = field(default_factory=ProgramConfig)
+    status: ProgramStatus = field(default_factory=ProgramStatus)
+
+    def __post_init__(self):
         self._last_counter = self.status.counter
 
     def __repr__(self):
         return "settings"
 
     @property
     def modified(self):
         changed = self.status.counter != self._last_counter
         self._last_counter = self.status.counter
         return changed
 
     @staticmethod
-    def prune_status(config, status):
+    def prune_status(config: ProgramConfig, status: ProgramStatus):
         """Remove undefined applications and computers."""
         log.info("Cleaning up applications and computers...")
         for appstatus in status.applications.copy():
-            if not config.applications.find(appstatus.application):
+            if not config.find_application(appstatus.application):
                 status.applications.remove(appstatus)
                 log.info("Removed application: %s", appstatus)
             else:
                 for computerstate in appstatus.computers.copy():
-                    if not config.computers.find(computerstate.computer):
+                    if not config.find_computer(computerstate.computer):
                         appstatus.computers.remove(computerstate)
                         log.info("Removed computer: %s", computerstate)
 
     @staticmethod
-    def queue_all_applications(config, status, computer):
+    def queue_all_applications(config: ProgramConfig, status: ProgramStatus, computer):
         """Queue applications for launch."""
         log.info("Queuing applications for launch...")
         for application in config.applications:
             if application.auto_queue:
                 log.debug("Queuing %s on %s...", application, computer)
                 status.queue(application, computer)
 
     @staticmethod
-    def launch_queued_applications(config, status, computer, manager):
+    def launch_queued_applications(
+        config: ProgramConfig, status: ProgramStatus, computer, manager: BaseManager
+    ):
         """Launch applications that have been queued."""
         log.info("Launching queued applications...")
         for app_status in status.applications:
             if app_status.next:
-                application = config.applications.get(app_status.application)
+                application = config.get_application(app_status.application)
                 print(crayons.yellow(f"{application} is queued for {app_status.next}"))
                 if app_status.next == computer:
                     latest = status.get_latest(application)
                     if latest in (computer, None) or application.no_wait:
                         if not manager.is_running(application):
                             manager.start(application)
                         app_status.next = None
@@ -70,22 +74,24 @@
                                 f"{application} is still running on {latest}"
                             )
                         )
                 elif manager.is_running(application):
                     manager.stop(application)
 
     @staticmethod
-    def close_all_applications(config, manager):
+    def close_all_applications(config: ProgramConfig, manager: BaseManager):
         """Close all applications running on this computer."""
         log.info("Closing all applications on this computer...")
         for application in config.applications:
             manager.stop(application)
 
     @staticmethod
-    def update_status(config, status, computer, manager):
+    def update_status(
+        config: ProgramConfig, status: ProgramStatus, computer, manager: BaseManager
+    ):
         """Update each application's status."""
         log.info("Recording application status...")
         for application in config.applications:
             latest = status.get_latest(application)
             if manager.is_running(application):
                 if computer != latest:
                     if status.is_running(application, computer):
```

### Comparing `mine-3.1.1/mine/models/status.py` & `mine-4.0a1/mine/models/status.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Data structures for application/computer status."""
 
 import functools
+from dataclasses import dataclass, field
 
 import log
-import yorm
 
+from .application import Application
+from .computer import Computer
 from .timestamp import Timestamp
 
 
 def log_running(func):
     @functools.wraps(func)
     def wrapped(self, application, computer):
         running = func(self, application, computer)
@@ -41,71 +43,49 @@
         result = func(self, application, computer)
         log.debug("%s marked as stopped on: %s", application, computer)
         return result
 
     return wrapped
 
 
-@yorm.attr(computer=yorm.types.String)
-@yorm.attr(timestamp=Timestamp)
-class State(yorm.types.AttributeDictionary):
+@dataclass
+class State:
     """Dictionary of computer state."""
 
-    def __init__(self, computer=None, timestamp=None):
-        super().__init__()
-        self.computer = computer
-        self.timestamp = timestamp or Timestamp()
+    computer: str
+    timestamp: Timestamp = field(default_factory=Timestamp)
 
     def __str__(self):
         return str(self.computer)
 
     def __lt__(self, other):
         return str(self.computer).lower() < str(other.computer).lower()
 
 
-@yorm.attr(all=State)
-class StateList(yorm.types.SortedList):
-    """List of computer states for an application."""
-
-
-@yorm.attr(application=yorm.types.String)
-@yorm.attr(computers=StateList)
-@yorm.attr(next=yorm.types.NullableString)
-class Status(yorm.types.AttributeDictionary):
+@dataclass
+class Status:
     """Dictionary of computers using an application."""
 
-    def __init__(
-        self, application=None, computers=None, next=None
-    ):  # pylint: disable=redefined-builtin
-        super().__init__()
-        self.application = application
-        self.computers = computers or StateList()
-        self.next = next
+    application: str
+    computers: list[State] = field(default_factory=list)
+    next: str | None = None
 
     def __str__(self):
         return str(self.application)
 
     def __lt__(self, other):
         return str(self.application).lower() < str(other.application).lower()
 
 
-@yorm.attr(all=Status)
-class StatusList(yorm.types.SortedList):
-    """List of application statuses."""
-
-
-@yorm.attr(applications=StatusList)
-@yorm.attr(counter=yorm.types.Integer)
-class ProgramStatus(yorm.types.AttributeDictionary):
+@dataclass
+class ProgramStatus:
     """Dictionary of current program status."""
 
-    def __init__(self, applications=None, counter=0):
-        super().__init__()
-        self.applications = applications or StatusList()
-        self.counter = counter
+    applications: list[Status] = field(default_factory=list)
+    counter: int = 0
 
     def find(self, application):
         """Return the application status for an application."""
         for app_status in self.applications:
             if app_status.application == application.name:
                 break
         else:
@@ -139,57 +119,57 @@
                 for state in status.computers:
                     if state.computer == computer.name:
                         return state.timestamp.active
 
         # Status not found, assume the application is not running
         return False
 
-    def queue(self, application, computer):
+    def queue(self, application: Application, computer: Computer):
         """Record an application as queued for launch on a computer."""
         status = self.find(application)
         status.next = computer.name
 
     @log_starting
-    def start(self, application, computer):
+    def start(self, application: Application, computer: Computer):
         """Record an application as running on a computer."""
         for status in self.applications:
             if status.application == application.name:
                 for state in status.computers:
                     if state.computer == computer.name:
                         self.counter += 1
                         state.timestamp.started = self.counter
                         return
                 break
         else:
-            status = None
+            status = None  # type: ignore
 
         # Status not found, add the application/computer as started
         self.counter += 1
         state = State(computer.name)
         state.timestamp.started = self.counter
         if status is None:
             status = Status(application.name)
             status.computers.append(state)
             self.applications.append(status)
         else:
             status.computers.append(state)
 
     @log_stopping
-    def stop(self, application, computer):
+    def stop(self, application: Application, computer: Computer):
         """Record an application as no longer running on a computer."""
         for status in self.applications:
             if status.application == application.name:
                 for state in status.computers:
                     if state.computer == computer.name:
                         self.counter += 1
                         state.timestamp.stopped = self.counter
                         return
                 break
         else:
-            status = None
+            status = None  # type: ignore
 
         # Status not found, add the application/computer as stopped
         self.counter += 1
         state = State(computer.name)
         state.timestamp.stopped = self.counter
         if status is None:
             status = Status(application.name)
```

### Comparing `mine-3.1.1/mine/services.py` & `mine-4.0a1/mine/services.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import log
 
 from .models.application import Application, Versions
 
 ROOTS = (r"C:\Users", r"/Users", r"/home")
 SERVICES = ("Dropbox", "Dropbox (Personal)")
-CONFIG = "mine.yml"
+CONFIG = "mine4.yml"  # TODO: Change back to "mine.yml" with 4.x release
 CONFLICT_BASE = r"{} \(.+'s conflicted copy \d+-\d+-\d+.*\).*"
 CONFLICT_ANY = CONFLICT_BASE.format(".+")
 CONFLICT_CONFIG = CONFLICT_BASE.format("mine")
 DEPTH = 3  # number of levels to search for the settings file
 APPLICATION = Application(
     "Dropbox",
     versions=Versions(mac="Dropbox.app", windows="Dropbox.exe", linux="dropbox"),
```

### Comparing `mine-3.1.1/mine/settings.py` & `mine-4.0a1/mine/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 QUIET_LOGGING_LEVEL = logging.WARNING
 DEFAULT_LOGGING_LEVEL = logging.WARNING
 VERBOSE_LOGGING_LEVEL = logging.INFO
 VERBOSE2_LOGGING_LEVEL = logging.DEBUG
 LOGGING_DATEFMT = "%Y-%m-%d %H:%M"
 
 # 3rd party settings
-YORM_LOGGING_LEVEL = logging.WARNING
+DATAFILES_LOGGING_LEVEL = logging.WARNING
```

### Comparing `mine-3.1.1/mine/tests/conftest.py` & `mine-4.0a1/mine/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 def pytest_configure(config):
     """Disable verbose output when running tests."""
     log.init(
         level=log.DEBUG, format="[%(levelname)-8s] (%(name)s @%(lineno)4d) %(message)s"
     )
-    log.silence("yorm", allow_warning=True)
+    log.silence("datafiles", allow_warning=True)
 
     terminal = config.pluginmanager.getplugin("terminal")
     terminal.TerminalReporter.showfspath = False
 
 
 def pytest_runtest_setup(item):
     if "linux_only" in item.keywords and platform.system() != "Linux":
```

### Comparing `mine-3.1.1/mine/tests/files/mine-in.yml` & `mine-4.0a1/mine/tests/files/mine-in.yml`

 * *Files identical despite different names*

### Comparing `mine-3.1.1/mine/tests/files/mine-out.yml` & `mine-4.0a1/mine/tests/files/mine-out.yml`

 * *Files identical despite different names*

### Comparing `mine-3.1.1/mine/tests/test_cli.py` & `mine-4.0a1/mine/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from mine import cli, common
 from mine.models import Application
 
 
 @pytest.fixture
 def tmp_path(tmpdir):
-    return tmpdir.join("custom.ext").strpath
+    return tmpdir.join("custom.yml").strpath
 
 
 class TestMain:
     """Unit tests for the `main` function."""
 
     @patch("mine.cli.run", Mock(return_value=True))
     def test_run(self):
@@ -61,15 +61,15 @@
         mock_run.assert_called_once_with(path=None, delay=300)
 
     @patch("mine.cli.run")
     def test_daemon_with_specific_delay(self, mock_run):
         cli.main(["--daemon", "42"])
         mock_run.assert_called_once_with(path=None, delay=42)
 
-    @patch("mine.cli.daemon", Application(None))
+    @patch("mine.cli.daemon", Application(""))
     def test_warning_when_daemon_is_not_running(self, tmp_path):
         with pytest.raises(SystemExit):
             cli.main(["--file", tmp_path])
 
 
 class TestSwitch:
     """Unit tests for the `switch` function."""
```

### Comparing `mine-3.1.1/mine/tests/test_manager.py` & `mine-4.0a1/mine/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `mine-3.1.1/mine/tests/test_models_application.py` & `mine-4.0a1/mine/tests/test_models_application.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from mine.models import Application, Applications
+from mine.models import Application
 
 
 class TestApplication:
     """Unit tests for the application class."""
 
     app1 = Application("iTunes")
     app1.versions.mac = "iTunes.app"
@@ -30,23 +30,7 @@
         assert self.app2 == self.app4
         assert self.app1 != self.app3
 
     def test_lt(self):
         """Verify applications can be sorted."""
         assert self.app2 < self.app1
         assert self.app3 > self.app2
-
-
-class TestApplications:
-    """Unit tests for lists of applications."""
-
-    apps = Applications([TestApplication.app1, TestApplication.app2])
-
-    def test_get(self):
-        """Verify an application can be found in a list."""
-        app = self.apps.get("itunes")
-        assert "iTunes" == app.name
-
-    def test_get_missing(self):
-        """Verify an invalid names raise an assertion."""
-        with pytest.raises(AssertionError):
-            self.apps.get("fake")
```

### Comparing `mine-3.1.1/mine/tests/test_models_data.py` & `mine-4.0a1/mine/tests/test_models_data.py`

 * *Files identical despite different names*

### Comparing `mine-3.1.1/mine/tests/test_models_status.py` & `mine-4.0a1/mine/tests/test_models_status.py`

 * *Files identical despite different names*

### Comparing `mine-3.1.1/mine/tests/test_models_timestamp.py` & `mine-4.0a1/mine/tests/test_models_timestamp.py`

 * *Files identical despite different names*

### Comparing `mine-3.1.1/mine/tests/test_services.py` & `mine-4.0a1/mine/tests/test_services.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,32 +39,32 @@
         with pytest.raises(EnvironmentError):
             services.find_root(top="mock/top")
 
 
 class TestFindConfigPath:
     def test_find_dropbox(self, tmp_dir):
         """Verify a settings file can be found in Dropbox."""
-        touch("Dropbox", "mine.yml")
+        touch("Dropbox", services.CONFIG)
 
         path = services.find_config_path(tmp_dir)
 
         assert os.path.isfile(path)
 
     def test_find_dropbox_personal(self, tmp_dir):
         """Verify a settings file can be found in Dropbox (Personal)."""
-        touch("Dropbox (Personal)", "mine.yml")
+        touch("Dropbox (Personal)", services.CONFIG)
 
         path = services.find_config_path(tmp_dir)
 
         assert os.path.isfile(path)
 
     @patch("mine.services.DEPTH", 2)
     def test_find_depth(self, tmp_dir):
         """Verify a settings file is not found below the maximum depth."""
-        touch("Dropbox", "a", "b", "mine.yml")
+        touch("Dropbox", "a", "b", services.CONFIG)
 
         with pytest.raises(OSError):
             services.find_config_path(tmp_dir)
 
     def test_find_no_share(self):
         """Verify an error occurs when no service directory is found."""
         with pytest.raises(EnvironmentError):
```

### Comparing `mine-3.1.1/pyproject.toml` & `mine-4.0a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "mine"
-version = "3.1.1"
+version = "4.0a1"
 description = "Share application state across computers using Dropbox."
 
 license = "MIT"
 
 authors = ["Jace Browning <jacebrowning@gmail.com>"]
 
 readme = "README.md"
@@ -21,28 +21,26 @@
     "Environment :: Console",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: System",
     "Topic :: System :: Monitoring",
     "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
 
-python = "^3.8"
+python = "^3.10"
 
-YORM = "^1.6"
+datafiles = "^2.1.2"
 psutil = ">=4.4,<6.0"
 crayons = "~0.1"
 minilog = "^2.1"
 universal-startfile = "^0.2"
 
 [tool.poetry.dev-dependencies]
 
@@ -95,14 +93,16 @@
 
 ignore_missing_imports = true
 no_implicit_optional = true
 check_untyped_defs = true
 
 cache_dir = ".cache/mypy/"
 
+plugins = "datafiles.plugins:mypy"
+
 [tool.pytest.ini_options]
 
 addopts = """
 --strict-markers
 
 -r sxX
 --show-capture=log
```

### Comparing `mine-3.1.1/PKG-INFO` & `mine-4.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 Metadata-Version: 2.1
 Name: mine
-Version: 3.1.1
+Version: 4.0a1
 Summary: Share application state across computers using Dropbox.
 Home-page: https://pypi.org/project/mine
 License: MIT
 Author: Jace Browning
 Author-email: jacebrowning@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Utilities
-Requires-Dist: YORM (>=1.6,<2.0)
 Requires-Dist: crayons (>=0.1,<0.2)
+Requires-Dist: datafiles (>=2.1.2,<3.0.0)
 Requires-Dist: minilog (>=2.1,<3.0)
 Requires-Dist: psutil (>=4.4,<6.0)
 Requires-Dist: universal-startfile (>=0.2,<0.3)
 Project-URL: Documentation, https://mine.readthedocs.io
 Project-URL: Repository, https://github.com/jacebrowning/mine
 Description-Content-Type: text/markdown
```

