# Comparing `tmp/pypomes_scheduling-0.1.8.tar.gz` & `tmp/pypomes_scheduling-0.1.9.tar.gz`

## Comparing `pypomes_scheduling-0.1.8.tar` & `pypomes_scheduling-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.8/src/pypomes_scheduling/__init__.py
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.8/src/pypomes_scheduling/__threaded_scheduler.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.8/src/pypomes_scheduling/scheduling_pomes.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.8/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.8/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.8/README.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.9/src/pypomes_scheduling/__init__.py
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.9/src/pypomes_scheduling/__threaded_scheduler.py
+-rw-r--r--   0        0        0     5128 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.9/src/pypomes_scheduling/scheduling_pomes.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.9/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.9/README.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pypomes_scheduling-0.1.9/PKG-INFO
```

### Comparing `pypomes_scheduling-0.1.8/src/pypomes_scheduling/__threaded_scheduler.py` & `pypomes_scheduling-0.1.9/src/pypomes_scheduling/__threaded_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,12 +99,11 @@
                                 name=job_name)
         if self._logger is not None:
             self._logger.info(f"Job '{job_name}' scheduled, with CRON '{job_cron}'")
 
     def stop(self):
         """
         Stop the scheduler.
-        :return:
         """
         if self._logger is not None:
             self._logger.info("Finishing...")
         self._stopped = True
```

### Comparing `pypomes_scheduling-0.1.8/src/pypomes_scheduling/scheduling_pomes.py` & `pypomes_scheduling-0.1.9/src/pypomes_scheduling/scheduling_pomes.py`

 * *Files 5% similar despite different names*

```diff
@@ -106,21 +106,35 @@
         # add to the return valiable, if scheduling was successful
         if scheduler_add_job(errors, job[0], job[1], job[2], job_cron, job_start, job_args, job_kwargs):
             result += 1
 
     return result
 
 
-def scheduler_start():
+def scheduler_start(errors: list[str]):
     """
     Start the scheduler.
+
+    :param errors: incidental errors
+    :return: True if the scheduler has started, False otherwise
     """
     global __scheduler
-    __scheduler.start()
+
+    # initialize the return variable
+    result: bool = False
+
+    try:
+        __scheduler.start()
+        result = True
+    except Exception as e:
+        errors.append(f"Error starting the scheduler': {exc_format(e, sys.exc_info())}")
+
+    return result
 
 
 def scheduler_stop():
     """
     Stop the scheduler.
     """
     global __scheduler
+
     __scheduler.stop()
```

### Comparing `pypomes_scheduling-0.1.8/LICENSE` & `pypomes_scheduling-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_scheduling-0.1.8/pyproject.toml` & `pypomes_scheduling-0.1.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_scheduling"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (scheduling module)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_scheduling-0.1.8/PKG-INFO` & `pypomes_scheduling-0.1.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypomes_scheduling
-Version: 0.1.8
+Version: 0.1.9
 Summary: A collection of Python pomes, pennyeach (scheduling module)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Scheduling
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Scheduling/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

