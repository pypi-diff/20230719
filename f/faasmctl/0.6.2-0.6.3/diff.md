# Comparing `tmp/faasmctl-0.6.2.tar.gz` & `tmp/faasmctl-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faasmctl-0.6.2.tar", last modified: Wed Jul 19 08:56:51 2023, max compression
+gzip compressed data, was "faasmctl-0.6.3.tar", last modified: Wed Jul 19 09:42:40 2023, max compression
```

## Comparing `faasmctl-0.6.2.tar` & `faasmctl-0.6.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:56:51.631293 faasmctl-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-19 08:54:51.000000 faasmctl-0.6.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-19 08:56:51.631293 faasmctl-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-19 08:54:51.000000 faasmctl-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:56:51.623293 faasmctl-0.6.2/faasmctl/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:56:51.627293 faasmctl-0.6.2/faasmctl/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/tasks/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/tasks/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/tasks/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/tasks/flush.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/tasks/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/tasks/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/tasks/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/tasks/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/tasks/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:56:51.631293 faasmctl-0.6.2/faasmctl/util/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/faasm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/flush.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:56:51.631293 faasmctl-0.6.2/faasmctl/util/gen_proto/
--rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-19 08:56:42.000000 faasmctl-0.6.2/faasmctl/util/gen_proto/faabric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-19 08:56:42.000000 faasmctl-0.6.2/faasmctl/util/gen_proto/planner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/planner.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-19 08:54:51.000000 faasmctl-0.6.2/faasmctl/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:56:51.623293 faasmctl-0.6.2/faasmctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-19 08:56:51.000000 faasmctl-0.6.2/faasmctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-19 08:56:51.000000 faasmctl-0.6.2/faasmctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 08:56:51.000000 faasmctl-0.6.2/faasmctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-19 08:56:51.000000 faasmctl-0.6.2/faasmctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-19 08:56:51.000000 faasmctl-0.6.2/faasmctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 08:56:51.000000 faasmctl-0.6.2/faasmctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-19 08:54:51.000000 faasmctl-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-19 08:56:51.631293 faasmctl-0.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:42:40.933650 faasmctl-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-19 09:40:42.000000 faasmctl-0.6.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-19 09:42:40.933650 faasmctl-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-19 09:40:42.000000 faasmctl-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:42:40.921650 faasmctl-0.6.3/faasmctl/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:42:40.925650 faasmctl-0.6.3/faasmctl/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/tasks/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/tasks/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/tasks/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/tasks/flush.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/tasks/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/tasks/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/tasks/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/tasks/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/tasks/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:42:40.929650 faasmctl-0.6.3/faasmctl/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/util/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/util/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/util/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/util/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/util/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/util/faasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/util/flush.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:42:40.933650 faasmctl-0.6.3/faasmctl/util/gen_proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-19 09:42:31.000000 faasmctl-0.6.3/faasmctl/util/gen_proto/faabric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-19 09:42:31.000000 faasmctl-0.6.3/faasmctl/util/gen_proto/planner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/util/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/util/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/util/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/util/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/util/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/util/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/util/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-19 09:40:42.000000 faasmctl-0.6.3/faasmctl/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:42:40.921650 faasmctl-0.6.3/faasmctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-19 09:42:40.000000 faasmctl-0.6.3/faasmctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-19 09:42:40.000000 faasmctl-0.6.3/faasmctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 09:42:40.000000 faasmctl-0.6.3/faasmctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-19 09:42:40.000000 faasmctl-0.6.3/faasmctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-19 09:42:40.000000 faasmctl-0.6.3/faasmctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 09:42:40.000000 faasmctl-0.6.3/faasmctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-19 09:40:42.000000 faasmctl-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-19 09:42:40.933650 faasmctl-0.6.3/setup.cfg
```

### Comparing `faasmctl-0.6.2/LICENSE.md` & `faasmctl-0.6.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.2/PKG-INFO` & `faasmctl-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.6.2
+Version: 0.6.3
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
-pip install faasmctl==0.6.2
+pip install faasmctl==0.6.3
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.6.2/README.md` & `faasmctl-0.6.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.6.2
+pip install faasmctl==0.6.3
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.6.2/faasmctl/tasks/cli.py` & `faasmctl-0.6.3/faasmctl/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.2/faasmctl/tasks/delete.py` & `faasmctl-0.6.3/faasmctl/tasks/delete.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.2/faasmctl/tasks/deploy.py` & `faasmctl-0.6.3/faasmctl/tasks/deploy.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.2/faasmctl/tasks/flush.py` & `faasmctl-0.6.3/faasmctl/tasks/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.2/faasmctl/tasks/invoke.py` & `faasmctl-0.6.3/faasmctl/tasks/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.2/faasmctl/tasks/logs.py` & `faasmctl-0.6.3/faasmctl/tasks/logs.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.2/faasmctl/tasks/restart.py` & `faasmctl-0.6.3/faasmctl/tasks/restart.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.2/faasmctl/tasks/status.py` & `faasmctl-0.6.3/faasmctl/tasks/status.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.2/faasmctl/util/compose.py` & `faasmctl-0.6.3/faasmctl/util/compose.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from faasmctl.util.config import get_faasm_ini_value
 from faasmctl.util.deploy import generate_ini_file
 from faasmctl.util.network import get_next_bindable_port
 from faasmctl.util.random import generate_gid
+from json import loads as json_loads
 from os import environ, makedirs
 from os.path import exists, isfile, join
 from shutil import rmtree
 from subprocess import run
 from time import sleep
 
 
@@ -99,14 +100,16 @@
         name=env["COMPOSE_PROJECT_NAME"],
         cwd=faasm_checkout,
         mount_source=mount_source,
         planner_host_port=env["PLANNER_HOST_PORT"],
         planner_docker_port=env["PLANNER_DOCKER_PORT"],
         upload_host_port=env["UPLOAD_HOST_PORT"],
         upload_docker_port=env["UPLOAD_DOCKER_PORT"],
+        worker_names=get_container_names_from_compose(),
+        worker_ips=get_container_ips_from_compose(),
     )
 
 
 def delete_compose_cluster(ini_file):
     """
     Delete a cluster running on docker compose
 
@@ -120,28 +123,41 @@
         "-p {}".format(cluster_name),
         "down",
     ]
     compose_cmd = " ".join(compose_cmd)
     run(compose_cmd, shell=True, check=True, cwd=working_dir)
 
 
-def run_compose_cmd(ini_file, cmd):
+def run_compose_cmd(ini_file, cmd, capture_out=False):
     cluster_name = get_faasm_ini_value(ini_file, "Faasm", "cluster_name")
     work_dir = get_faasm_ini_value(ini_file, "Faasm", "working_dir")
     mount_source = get_faasm_ini_value(ini_file, "Faasm", "mount_source")
     mount_source = mount_source == "True"
 
     compose_cmd = [
         "docker compose",
         "-p {}".format(cluster_name),
         cmd,
     ]
     compose_cmd = " ".join(compose_cmd)
 
     compose_env = get_compose_env_vars(work_dir, mount_source)
+    if capture_out:
+        return (
+            run(
+                compose_cmd,
+                shell=True,
+                capture_out=True,
+                cwd=work_dir,
+                env=compose_env,
+            )
+            .stdout.decode("utf-8")
+            .strip()
+        )
+
     run(
         compose_cmd,
         shell=True,
         check=True,
         cwd=work_dir,
         env=compose_env,
     )
@@ -249,7 +265,37 @@
     for image in dirs_to_copy:
         image_tag = [line.split("=")[1] for line in env_file if line.startswith(image)]
         assert len(image_tag) == 1
         image_tag = image_tag[0]
 
         for dir_path in dirs_to_copy[image]:
             copy_from_ctr_to_host(image_tag, dir_path)
+
+
+def get_container_names_from_compose(ini_file):
+    json_str = run_compose_cmd(ini_file, "ps --format json", capture_out=True)
+    json_dict = json_loads(json_str)
+    return [c["Name"] for c in json_dict if c["Service"] == "worker"]
+
+
+def get_container_ips_from_compose(ini_file):
+    container_ips = []
+    container_names = get_container_names_from_compose(ini_file)
+    for c in container_names:
+        ip_cmd = [
+            "docker inspect -f",
+            "'{{range.NetworkSettings.Networks}}{{.IPAddress}}{{end}}'",
+            c,
+        ]
+        ip_cmd = " ".join(ip_cmd)
+        c_ip = (
+            run(
+                ip_cmd,
+                shell=True,
+                check=True,
+                capture_output=True,
+            )
+            .stdout.decode("utf-8")
+            .strip()
+        )
+        container_ips.append(c_ip)
+    return container_ips
```

### Comparing `faasmctl-0.6.2/faasmctl/util/config.py` & `faasmctl-0.6.3/faasmctl/util/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -40,7 +40,27 @@
         host = get_faasm_ini_value(ini_file, "Faasm", "planner_host_in_docker")
         port = get_faasm_ini_value(ini_file, "Faasm", "planner_port_in_docker")
     else:
         host = get_faasm_ini_value(ini_file, "Faasm", "planner_host")
         port = get_faasm_ini_value(ini_file, "Faasm", "planner_port")
 
     return host, port
+
+
+def get_faasm_worker_names(ini_file=None):
+    if not ini_file:
+        ini_file = get_faasm_ini_file()
+
+    names = get_faasm_ini_value(ini_file, "Faasm", "worker_names")
+    names = [p.strip() for p in names.split(",") if p.strip()]
+
+    return names
+
+
+def get_faasm_worker_ips(ini_file=None):
+    if not ini_file:
+        ini_file = get_faasm_ini_file()
+
+    ips = get_faasm_ini_value(ini_file, "Faasm", "worker_ips")
+    ips = [p.strip() for p in ips.split(",") if p.strip()]
+
+    return ips
```

### Comparing `faasmctl-0.6.2/faasmctl/util/deploy.py` & `faasmctl-0.6.3/faasmctl/util/deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,16 +87,16 @@
         cluster_name = kwargs["name"]
         working_dir = kwargs["cwd"]
 
         upload_ip = LOCALHOST_IP
         upload_port = kwargs["upload_host_port"]
         planner_ip = LOCALHOST_IP
         planner_port = kwargs["planner_host_port"]
-        worker_names = []
-        worker_ips = []
+        worker_names = kwargs["worker_names"]
+        worker_ips = kwargs["worker_ips"]
     elif backend == "k8s":
         working_dir = kwargs["cwd"]
         k8s_config = kwargs["k8s_config"]
         k8s_namespace = kwargs["k8s_namespace"]
 
         upload_ip = kwargs["upload_ip"]
         upload_port = kwargs["upload_port"]
```

### Comparing `faasmctl-0.6.2/faasmctl/util/docker.py` & `faasmctl-0.6.3/faasmctl/util/docker.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.2/faasmctl/util/flush.py` & `faasmctl-0.6.3/faasmctl/util/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.2/faasmctl/util/gen_proto/faabric_pb2.py` & `faasmctl-0.6.3/faasmctl/util/gen_proto/faabric_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.2/faasmctl/util/gen_proto/planner_pb2.py` & `faasmctl-0.6.3/faasmctl/util/gen_proto/planner_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.2/faasmctl/util/invoke.py` & `faasmctl-0.6.3/faasmctl/util/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.2/faasmctl/util/k8s.py` & `faasmctl-0.6.3/faasmctl/util/k8s.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.2/faasmctl/util/network.py` & `faasmctl-0.6.3/faasmctl/util/network.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,9 +31,8 @@
         try:
             s.bind((LOCALHOST_IP, bind_port))
             s.close()
             break
         except socket_error:
             bind_port += 1
 
-    print("Picking port: {}".format(bind_port))
     return bind_port
```

### Comparing `faasmctl-0.6.2/faasmctl/util/planner.py` & `faasmctl-0.6.3/faasmctl/util/planner.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.2/faasmctl/util/upload.py` & `faasmctl-0.6.3/faasmctl/util/upload.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.2/faasmctl.egg-info/PKG-INFO` & `faasmctl-0.6.3/faasmctl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.6.2
+Version: 0.6.3
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
-pip install faasmctl==0.6.2
+pip install faasmctl==0.6.3
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.6.2/faasmctl.egg-info/SOURCES.txt` & `faasmctl-0.6.3/faasmctl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `faasmctl-0.6.2/pyproject.toml` & `faasmctl-0.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faasmctl"
-version = "0.6.2"
+version = "0.6.3"
 authors = [
   { name="Faasm Team", email="foo@bar.com" },
 ]
 description = "Command line tool to deploy, manage, and interact with Faasm"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

