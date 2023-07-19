# Comparing `tmp/faasmctl-0.5.6.tar.gz` & `tmp/faasmctl-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faasmctl-0.5.6.tar", last modified: Mon Jul 17 21:59:27 2023, max compression
+gzip compressed data, was "faasmctl-0.6.0.tar", last modified: Wed Jul 19 08:35:05 2023, max compression
```

## Comparing `faasmctl-0.5.6.tar` & `faasmctl-0.6.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:59:27.295498 faasmctl-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-17 21:56:53.000000 faasmctl-0.5.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-17 21:59:27.295498 faasmctl-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-17 21:56:53.000000 faasmctl-0.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:59:27.291498 faasmctl-0.5.6/faasmctl/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:59:27.291498 faasmctl-0.5.6/faasmctl/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/tasks/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/tasks/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/tasks/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/tasks/flush.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/tasks/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/tasks/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/tasks/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/tasks/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/tasks/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:59:27.295498 faasmctl-0.5.6/faasmctl/util/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/util/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/util/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/util/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/util/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/util/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/util/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/util/faasm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/util/flush.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:59:27.295498 faasmctl-0.5.6/faasmctl/util/gen_proto/
--rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-17 21:59:17.000000 faasmctl-0.5.6/faasmctl/util/gen_proto/faabric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-17 21:59:17.000000 faasmctl-0.5.6/faasmctl/util/gen_proto/planner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/util/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/util/k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/util/message.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/util/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/util/planner.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/util/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/util/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 21:56:53.000000 faasmctl-0.5.6/faasmctl/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:59:27.291498 faasmctl-0.5.6/faasmctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-17 21:59:27.000000 faasmctl-0.5.6/faasmctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-17 21:59:27.000000 faasmctl-0.5.6/faasmctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 21:59:27.000000 faasmctl-0.5.6/faasmctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 21:59:27.000000 faasmctl-0.5.6/faasmctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 21:59:27.000000 faasmctl-0.5.6/faasmctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 21:59:27.000000 faasmctl-0.5.6/faasmctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-17 21:56:53.000000 faasmctl-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 21:59:27.295498 faasmctl-0.5.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:35:05.777988 faasmctl-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-19 08:32:51.000000 faasmctl-0.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-19 08:35:05.777988 faasmctl-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-19 08:32:51.000000 faasmctl-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:35:05.773987 faasmctl-0.6.0/faasmctl/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:35:05.777988 faasmctl-0.6.0/faasmctl/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/tasks/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/tasks/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/tasks/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/tasks/flush.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/tasks/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/tasks/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/tasks/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/tasks/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/tasks/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:35:05.777988 faasmctl-0.6.0/faasmctl/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/util/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/util/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/util/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/util/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/util/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/util/faasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/util/flush.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:35:05.777988 faasmctl-0.6.0/faasmctl/util/gen_proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-19 08:34:55.000000 faasmctl-0.6.0/faasmctl/util/gen_proto/faabric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-19 08:34:55.000000 faasmctl-0.6.0/faasmctl/util/gen_proto/planner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/util/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/util/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/util/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/util/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/util/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/util/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/util/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-19 08:32:51.000000 faasmctl-0.6.0/faasmctl/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:35:05.777988 faasmctl-0.6.0/faasmctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-19 08:35:05.000000 faasmctl-0.6.0/faasmctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-19 08:35:05.000000 faasmctl-0.6.0/faasmctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 08:35:05.000000 faasmctl-0.6.0/faasmctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-19 08:35:05.000000 faasmctl-0.6.0/faasmctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-19 08:35:05.000000 faasmctl-0.6.0/faasmctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 08:35:05.000000 faasmctl-0.6.0/faasmctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-19 08:32:51.000000 faasmctl-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-19 08:35:05.781988 faasmctl-0.6.0/setup.cfg
```

### Comparing `faasmctl-0.5.6/LICENSE.md` & `faasmctl-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.6/PKG-INFO` & `faasmctl-0.6.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.5.6
+Version: 0.6.0
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
-pip install faasmctl==0.5.6
+pip install faasmctl==0.6.0
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.5.6/README.md` & `faasmctl-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.5.6
+pip install faasmctl==0.6.0
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.5.6/faasmctl/tasks/cli.py` & `faasmctl-0.6.0/faasmctl/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.6/faasmctl/tasks/delete.py` & `faasmctl-0.6.0/faasmctl/tasks/delete.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.6/faasmctl/tasks/deploy.py` & `faasmctl-0.6.0/faasmctl/tasks/deploy.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.6/faasmctl/tasks/flush.py` & `faasmctl-0.6.0/faasmctl/tasks/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.6/faasmctl/tasks/invoke.py` & `faasmctl-0.6.0/faasmctl/tasks/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.6/faasmctl/tasks/logs.py` & `faasmctl-0.6.0/faasmctl/tasks/logs.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.6/faasmctl/tasks/restart.py` & `faasmctl-0.6.0/faasmctl/tasks/restart.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.6/faasmctl/tasks/status.py` & `faasmctl-0.6.0/faasmctl/tasks/status.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.6/faasmctl/util/compose.py` & `faasmctl-0.6.0/faasmctl/util/compose.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from faasmctl.util.config import get_faasm_ini_value
 from faasmctl.util.deploy import generate_ini_file
+from faasmctl.util.network import get_next_bindable_port
 from faasmctl.util.random import generate_gid
 from os import environ, makedirs
 from os.path import exists, isfile, join
 from shutil import rmtree
 from subprocess import run
 from time import sleep
 
@@ -24,14 +25,26 @@
         env["FAASM_BUILD_DIR"] = join(faasm_checkout, "dev/faasm/build")
         env["FAASM_BUILD_MOUNT"] = "/host_dev/build"
         env["FAASM_CODE_MOUNT"] = "/host_dev/code"
         env["FAASM_CONAN_MOUNT"] = "/host_dev/conan"
         env["FAASM_LOCAL_MOUNT"] = "/host_dev/faasm-local"
         env["PLANNER_BUILD_MOUNT"] = "/build/faabric/static"
 
+    # Set network env. variables
+    env["PLANNER_DOCKER_PORT"] = "8080"
+    env["PLANNER_HOST_PORT"] = str(
+        get_next_bindable_port(int(env["PLANNER_DOCKER_PORT"]))
+    )
+    env["MINIO_DOCKER_PORT"] = "9000"
+    env["MINIO_HOST_PORT"] = str(get_next_bindable_port(int(env["MINIO_DOCKER_PORT"])))
+    env["UPLOAD_DOCKER_PORT"] = "8002"
+    env["UPLOAD_HOST_PORT"] = str(
+        get_next_bindable_port(int(env["UPLOAD_DOCKER_PORT"]))
+    )
+
     # Get Faasm version
     with open(join(faasm_checkout, "VERSION"), "r") as fh:
         faasm_ver = fh.read()
         faasm_ver = faasm_ver.strip()
 
     # Whitelist env. variables that we recognise
     if "WASM_VM" in environ:
@@ -82,14 +95,18 @@
     # Finally, generate the faasm.ini file to interact with the cluster
     return generate_ini_file(
         "compose",
         out_file=ini_file,
         name=env["COMPOSE_PROJECT_NAME"],
         cwd=faasm_checkout,
         mount_source=mount_source,
+        planner_host_port=env["PLANNER_HOST_PORT"],
+        planner_docker_port=env["PLANNER_DOCKER_PORT"],
+        upload_host_port=env["UPLOAD_HOST_PORT"],
+        upload_docker_port=env["UPLOAD_DOCKER_PORT"],
     )
 
 
 def delete_compose_cluster(ini_file):
     """
     Delete a cluster running on docker compose
```

### Comparing `faasmctl-0.5.6/faasmctl/util/config.py` & `faasmctl-0.6.0/faasmctl/util/config.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.6/faasmctl/util/deploy.py` & `faasmctl-0.6.0/faasmctl/util/deploy.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,17 +84,17 @@
     if backend == "compose":
         if "name" not in kwargs or "cwd" not in kwargs:
             raise RuntimeError("Not enough compose arguments provided!")
         cluster_name = kwargs["name"]
         working_dir = kwargs["cwd"]
 
         upload_ip = LOCALHOST_IP
-        upload_port = "8002"
+        upload_port = kwargs["upload_host_port"]
         planner_ip = LOCALHOST_IP
-        planner_port = "8080"
+        planner_port = kwargs["planner_host_port"]
         worker_names = []
         worker_ips = []
     elif backend == "k8s":
         working_dir = kwargs["cwd"]
         k8s_config = kwargs["k8s_config"]
         k8s_namespace = kwargs["k8s_namespace"]
 
@@ -127,18 +127,26 @@
             fh.write("cluster_name = {}\n".format(cluster_name))
         elif backend == "k8s":
             fh.write("k8s_namespace = {}\n".format(k8s_namespace))
         fh.write("upload_host = {}\n".format(upload_ip))
         if backend == "compose":
             fh.write("upload_host_in_docker = upload\n")
         fh.write("upload_port = {}\n".format(upload_port))
+        if backend == "compose":
+            fh.write(
+                "upload_port_in_docker = {}\n".format(kwargs["upload_docker_port"])
+            )
         fh.write("planner_host = {}\n".format(planner_ip))
         if backend == "compose":
             fh.write("planner_host_in_docker = planner\n")
         fh.write("planner_port = {}\n".format(planner_port))
+        if backend == "compose":
+            fh.write(
+                "planner_port_in_docker = {}\n".format(kwargs["planner_docker_port"])
+            )
         if backend == "k8s":
             fh.write("worker_names = {}\n".format(",".join(worker_names)))
             fh.write("worker_ips = {}\n".format(",".join(worker_ips)))
 
     with open(out_file, "r") as fh:
         print(fh.read())
```

### Comparing `faasmctl-0.5.6/faasmctl/util/docker.py` & `faasmctl-0.6.0/faasmctl/util/docker.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.6/faasmctl/util/flush.py` & `faasmctl-0.6.0/faasmctl/util/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.6/faasmctl/util/gen_proto/faabric_pb2.py` & `faasmctl-0.6.0/faasmctl/util/gen_proto/faabric_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.6/faasmctl/util/gen_proto/planner_pb2.py` & `faasmctl-0.6.0/faasmctl/util/gen_proto/planner_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.6/faasmctl/util/invoke.py` & `faasmctl-0.6.0/faasmctl/util/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.6/faasmctl/util/k8s.py` & `faasmctl-0.6.0/faasmctl/util/k8s.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.6/faasmctl/util/planner.py` & `faasmctl-0.6.0/faasmctl/util/planner.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.6/faasmctl/util/upload.py` & `faasmctl-0.6.0/faasmctl/util/upload.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.6/faasmctl.egg-info/PKG-INFO` & `faasmctl-0.6.0/faasmctl.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.5.6
+Version: 0.6.0
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
-pip install faasmctl==0.5.6
+pip install faasmctl==0.6.0
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.5.6/faasmctl.egg-info/SOURCES.txt` & `faasmctl-0.6.0/faasmctl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `faasmctl-0.5.6/pyproject.toml` & `faasmctl-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faasmctl"
-version = "0.5.6"
+version = "0.6.0"
 authors = [
   { name="Faasm Team", email="foo@bar.com" },
 ]
 description = "Command line tool to deploy, manage, and interact with Faasm"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

