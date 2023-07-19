# Comparing `tmp/faasmctl-0.6.1.tar.gz` & `tmp/faasmctl-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faasmctl-0.6.1.tar", last modified: Wed Jul 19 08:43:04 2023, max compression
+gzip compressed data, was "faasmctl-0.6.2.tar", last modified: Wed Jul 19 08:56:51 2023, max compression
```

## Comparing `faasmctl-0.6.1.tar` & `faasmctl-0.6.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:43:04.232673 faasmctl-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-19 08:40:24.000000 faasmctl-0.6.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-19 08:43:04.232673 faasmctl-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-19 08:40:24.000000 faasmctl-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:43:04.224673 faasmctl-0.6.1/faasmctl/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:43:04.228673 faasmctl-0.6.1/faasmctl/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/tasks/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/tasks/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/tasks/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/tasks/flush.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/tasks/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/tasks/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/tasks/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/tasks/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/tasks/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:43:04.228673 faasmctl-0.6.1/faasmctl/util/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/util/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/util/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/util/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/util/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/util/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/util/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/util/faasm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/util/flush.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:43:04.232673 faasmctl-0.6.1/faasmctl/util/gen_proto/
--rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-19 08:42:54.000000 faasmctl-0.6.1/faasmctl/util/gen_proto/faabric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-19 08:42:54.000000 faasmctl-0.6.1/faasmctl/util/gen_proto/planner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/util/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/util/k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/util/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/util/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/util/planner.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/util/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/util/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-19 08:40:24.000000 faasmctl-0.6.1/faasmctl/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:43:04.224673 faasmctl-0.6.1/faasmctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-19 08:43:04.000000 faasmctl-0.6.1/faasmctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-19 08:43:04.000000 faasmctl-0.6.1/faasmctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 08:43:04.000000 faasmctl-0.6.1/faasmctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-19 08:43:04.000000 faasmctl-0.6.1/faasmctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-19 08:43:04.000000 faasmctl-0.6.1/faasmctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 08:43:04.000000 faasmctl-0.6.1/faasmctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-19 08:40:24.000000 faasmctl-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-19 08:43:04.232673 faasmctl-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:56:51.631293 faasmctl-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-19 08:54:51.000000 faasmctl-0.6.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-19 08:56:51.631293 faasmctl-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-19 08:54:51.000000 faasmctl-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:56:51.623293 faasmctl-0.6.2/faasmctl/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:56:51.627293 faasmctl-0.6.2/faasmctl/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/tasks/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/tasks/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/tasks/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/tasks/flush.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/tasks/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/tasks/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/tasks/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/tasks/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/tasks/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:56:51.631293 faasmctl-0.6.2/faasmctl/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/faasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/flush.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:56:51.631293 faasmctl-0.6.2/faasmctl/util/gen_proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-19 08:56:42.000000 faasmctl-0.6.2/faasmctl/util/gen_proto/faabric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-19 08:56:42.000000 faasmctl-0.6.2/faasmctl/util/gen_proto/planner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:56:51.623293 faasmctl-0.6.2/faasmctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-19 08:56:51.000000 faasmctl-0.6.2/faasmctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-19 08:56:51.000000 faasmctl-0.6.2/faasmctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 08:56:51.000000 faasmctl-0.6.2/faasmctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-19 08:56:51.000000 faasmctl-0.6.2/faasmctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-19 08:56:51.000000 faasmctl-0.6.2/faasmctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 08:56:51.000000 faasmctl-0.6.2/faasmctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-19 08:54:51.000000 faasmctl-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-19 08:56:51.631293 faasmctl-0.6.2/setup.cfg
```

### Comparing `faasmctl-0.6.1/LICENSE.md` & `faasmctl-0.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.1/PKG-INFO` & `faasmctl-0.6.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.6.1
+Version: 0.6.2
 Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,15 +17,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.6.1
+pip install faasmctl==0.6.2
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.6.1/README.md` & `faasmctl-0.6.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.6.1
+pip install faasmctl==0.6.2
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.6.1/faasmctl/tasks/cli.py` & `faasmctl-0.6.2/faasmctl/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.1/faasmctl/tasks/delete.py` & `faasmctl-0.6.2/faasmctl/tasks/delete.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.1/faasmctl/tasks/deploy.py` & `faasmctl-0.6.2/faasmctl/tasks/deploy.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.1/faasmctl/tasks/flush.py` & `faasmctl-0.6.2/faasmctl/tasks/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.1/faasmctl/tasks/invoke.py` & `faasmctl-0.6.2/faasmctl/tasks/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.1/faasmctl/tasks/logs.py` & `faasmctl-0.6.2/faasmctl/tasks/logs.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.1/faasmctl/tasks/restart.py` & `faasmctl-0.6.2/faasmctl/tasks/restart.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.1/faasmctl/tasks/status.py` & `faasmctl-0.6.2/faasmctl/tasks/status.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.1/faasmctl/util/compose.py` & `faasmctl-0.6.2/faasmctl/util/compose.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.1/faasmctl/util/config.py` & `faasmctl-0.6.2/faasmctl/util/config.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.1/faasmctl/util/deploy.py` & `faasmctl-0.6.2/faasmctl/util/deploy.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.1/faasmctl/util/docker.py` & `faasmctl-0.6.2/faasmctl/util/docker.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.1/faasmctl/util/flush.py` & `faasmctl-0.6.2/faasmctl/util/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.1/faasmctl/util/gen_proto/faabric_pb2.py` & `faasmctl-0.6.2/faasmctl/util/gen_proto/faabric_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.1/faasmctl/util/gen_proto/planner_pb2.py` & `faasmctl-0.6.2/faasmctl/util/gen_proto/planner_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.1/faasmctl/util/invoke.py` & `faasmctl-0.6.2/faasmctl/util/invoke.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,15 +79,18 @@
         if response.status_code != 200:
             # FIXME: temporary workaround while the planner does not control
             # batch scheduling (and thus doesn't keep track of the apps in
             # flight). We may query for an app result before it is finished.
             # In this case, by default, the planner endpoint fails. But it is
             # not an error (it will be in the future)
             if response.text == "App not registered in results":
-                print("WARNING: app not registered in results")
+                # FIXME: we will have to emit a warning eventually, for now
+                # we pass
+                # print("WARNING: app not registered in results")
+                pass
             else:
                 print(
                     "POST request failed (code: {}): {}".format(
                         response.status_code, response.text
                     )
                 )
                 break
```

### Comparing `faasmctl-0.6.1/faasmctl/util/k8s.py` & `faasmctl-0.6.2/faasmctl/util/k8s.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.1/faasmctl/util/network.py` & `faasmctl-0.6.2/faasmctl/util/network.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.1/faasmctl/util/planner.py` & `faasmctl-0.6.2/faasmctl/util/planner.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.1/faasmctl/util/upload.py` & `faasmctl-0.6.2/faasmctl/util/upload.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.1/faasmctl.egg-info/PKG-INFO` & `faasmctl-0.6.2/faasmctl.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.6.1
+Version: 0.6.2
 Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,15 +17,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.6.1
+pip install faasmctl==0.6.2
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.6.1/faasmctl.egg-info/SOURCES.txt` & `faasmctl-0.6.2/faasmctl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.1/pyproject.toml` & `faasmctl-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faasmctl"
-version = "0.6.1"
+version = "0.6.2"
 authors = [
   { name="Faasm Team", email="foo@bar.com" },
 ]
 description = "Command line tool to deploy, manage, and interact with Faasm"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

