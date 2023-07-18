# Comparing `tmp/nvidia_tao-4.0.1-py3-none-any.whl.zip` & `tmp/nvidia_tao-5.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,28 +1,26 @@
-Zip file size: 155453 bytes, number of entries: 26
--rw-rw-r--  2.0 unx      306 b- defN 22-Apr-06 19:19 tlt/__init__.py
--rw-rw-r--  2.0 unx     1297 b- defN 23-Mar-06 15:37 tlt/version.py
--rw-rw-r--  2.0 unx      242 b- defN 21-Nov-06 18:23 tlt/components/__init__.py
--rw-rw-r--  2.0 unx      235 b- defN 21-Nov-06 18:23 tlt/components/docker_handler/__init__.py
--rw-rw-r--  2.0 unx    13152 b- defN 22-Nov-10 06:56 tlt/components/docker_handler/docker_handler.py
--rw-rw-r--  2.0 unx      281 b- defN 21-Nov-06 18:23 tlt/components/instance_handler/__init__.py
--rw-rw-r--  2.0 unx     1311 b- defN 22-Nov-10 06:56 tlt/components/instance_handler/base_instance.py
--rw-rw-r--  2.0 unx     1090 b- defN 22-Nov-10 06:56 tlt/components/instance_handler/builder.py
--rw-rw-r--  2.0 unx    13543 b- defN 22-Aug-21 22:48 tlt/components/instance_handler/local_instance.py
--rw-rw-r--  2.0 unx     5630 b- defN 22-Nov-10 06:56 tlt/components/instance_handler/utils.py
--rw-rw-r--  2.0 unx     5512 b- defN 22-Nov-10 06:56 tlt/components/instance_handler/whl_instance.py
--rw-rw-r--  2.0 unx      122 b- defN 21-Nov-06 18:23 tlt/components/types/__init__.py
--rw-rw-r--  2.0 unx     2444 b- defN 22-Nov-10 06:56 tlt/components/types/task.py
--rw-rw-r--  2.0 unx      217 b- defN 21-Nov-06 18:23 tlt/config/__init__.py
--rw-rw-r--  2.0 unx     2284 b- defN 23-Mar-06 15:37 tlt/config/config.json
--rw-rw-r--  2.0 unx      934 b- defN 23-Mar-06 15:37 tlt/config/config_deploy.json
--rw-rw-r--  2.0 unx      225 b- defN 21-Nov-06 18:23 tlt/entrypoint/__init__.py
--rw-rw-r--  2.0 unx     3930 b- defN 22-Nov-10 06:56 tlt/entrypoint/tao.py
--rw-rw-r--  2.0 unx     3972 b- defN 22-Nov-10 06:56 tlt/entrypoint/tao_deploy.py
--rw-rw-r--  2.0 unx   136701 b- defN 22-Jan-21 20:18 tlt/license/EULA.pdf
--rw-rw-r--  2.0 unx      208 b- defN 21-Nov-06 18:23 tlt/license/__init__.py
--rw-rw-r--  2.0 unx    18014 b- defN 23-Mar-06 15:38 nvidia_tao-4.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-06 15:38 nvidia_tao-4.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-06 15:38 nvidia_tao-4.0.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        4 b- defN 23-Mar-06 15:38 nvidia_tao-4.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2263 b- defN 23-Mar-06 15:38 nvidia_tao-4.0.1.dist-info/RECORD
-26 files, 214101 bytes uncompressed, 151763 bytes compressed:  29.1%
+Zip file size: 35256 bytes, number of entries: 24
+-rw-rw-r--  2.0 unx      858 b- defN 23-Jun-22 23:36 nvidia_tao_cli/__init__.py
+-rw-rw-r--  2.0 unx     1827 b- defN 23-Jul-14 19:47 nvidia_tao_cli/version.py
+-rw-rw-r--  2.0 unx      783 b- defN 23-Jun-22 23:36 nvidia_tao_cli/components/__init__.py
+-rw-rw-r--  2.0 unx      776 b- defN 23-Jun-22 23:36 nvidia_tao_cli/components/docker_handler/__init__.py
+-rw-rw-r--  2.0 unx    16529 b- defN 23-Jun-22 23:36 nvidia_tao_cli/components/docker_handler/docker_handler.py
+-rw-rw-r--  2.0 unx      822 b- defN 23-Jun-22 23:36 nvidia_tao_cli/components/instance_handler/__init__.py
+-rw-rw-r--  2.0 unx     1852 b- defN 23-Jun-22 23:36 nvidia_tao_cli/components/instance_handler/base_instance.py
+-rw-rw-r--  2.0 unx     1664 b- defN 23-Jun-22 23:36 nvidia_tao_cli/components/instance_handler/builder.py
+-rw-rw-r--  2.0 unx    16850 b- defN 23-Jun-22 23:36 nvidia_tao_cli/components/instance_handler/local_instance.py
+-rw-rw-r--  2.0 unx     6412 b- defN 23-Jun-22 23:36 nvidia_tao_cli/components/instance_handler/utils.py
+-rw-rw-r--  2.0 unx     8645 b- defN 23-Jun-22 23:36 nvidia_tao_cli/components/instance_handler/whl_instance.py
+-rw-rw-r--  2.0 unx      663 b- defN 23-Jun-22 23:36 nvidia_tao_cli/components/types/__init__.py
+-rw-rw-r--  2.0 unx     2990 b- defN 23-Jun-22 23:36 nvidia_tao_cli/components/types/task.py
+-rw-rw-r--  2.0 unx      759 b- defN 23-Jun-22 23:36 nvidia_tao_cli/config/__init__.py
+-rw-rw-r--  2.0 unx     4010 b- defN 23-Jul-18 18:44 nvidia_tao_cli/config/config.json
+-rw-rw-r--  2.0 unx      998 b- defN 23-Jun-18 00:10 nvidia_tao_cli/config/config_deploy.json
+-rw-rw-r--  2.0 unx      766 b- defN 23-Jun-22 23:36 nvidia_tao_cli/entrypoint/__init__.py
+-rw-rw-r--  2.0 unx     5615 b- defN 23-Jun-22 23:36 nvidia_tao_cli/entrypoint/tao_launcher.py
+-rw-rw-r--  2.0 unx    11356 b- defN 23-Jul-18 18:45 nvidia_tao-5.0.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     7970 b- defN 23-Jul-18 18:45 nvidia_tao-5.0.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-18 18:45 nvidia_tao-5.0.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       68 b- defN 23-Jul-18 18:45 nvidia_tao-5.0.0.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       15 b- defN 23-Jul-18 18:45 nvidia_tao-5.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2319 b- defN 23-Jul-18 18:45 nvidia_tao-5.0.0.dist-info/RECORD
+24 files, 94639 bytes uncompressed, 31378 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -1,79 +1,73 @@
-Filename: tlt/__init__.py
+Filename: nvidia_tao_cli/__init__.py
 Comment: 
 
-Filename: tlt/version.py
+Filename: nvidia_tao_cli/version.py
 Comment: 
 
-Filename: tlt/components/__init__.py
+Filename: nvidia_tao_cli/components/__init__.py
 Comment: 
 
-Filename: tlt/components/docker_handler/__init__.py
+Filename: nvidia_tao_cli/components/docker_handler/__init__.py
 Comment: 
 
-Filename: tlt/components/docker_handler/docker_handler.py
+Filename: nvidia_tao_cli/components/docker_handler/docker_handler.py
 Comment: 
 
-Filename: tlt/components/instance_handler/__init__.py
+Filename: nvidia_tao_cli/components/instance_handler/__init__.py
 Comment: 
 
-Filename: tlt/components/instance_handler/base_instance.py
+Filename: nvidia_tao_cli/components/instance_handler/base_instance.py
 Comment: 
 
-Filename: tlt/components/instance_handler/builder.py
+Filename: nvidia_tao_cli/components/instance_handler/builder.py
 Comment: 
 
-Filename: tlt/components/instance_handler/local_instance.py
+Filename: nvidia_tao_cli/components/instance_handler/local_instance.py
 Comment: 
 
-Filename: tlt/components/instance_handler/utils.py
+Filename: nvidia_tao_cli/components/instance_handler/utils.py
 Comment: 
 
-Filename: tlt/components/instance_handler/whl_instance.py
+Filename: nvidia_tao_cli/components/instance_handler/whl_instance.py
 Comment: 
 
-Filename: tlt/components/types/__init__.py
+Filename: nvidia_tao_cli/components/types/__init__.py
 Comment: 
 
-Filename: tlt/components/types/task.py
+Filename: nvidia_tao_cli/components/types/task.py
 Comment: 
 
-Filename: tlt/config/__init__.py
+Filename: nvidia_tao_cli/config/__init__.py
 Comment: 
 
-Filename: tlt/config/config.json
+Filename: nvidia_tao_cli/config/config.json
 Comment: 
 
-Filename: tlt/config/config_deploy.json
+Filename: nvidia_tao_cli/config/config_deploy.json
 Comment: 
 
-Filename: tlt/entrypoint/__init__.py
+Filename: nvidia_tao_cli/entrypoint/__init__.py
 Comment: 
 
-Filename: tlt/entrypoint/tao.py
+Filename: nvidia_tao_cli/entrypoint/tao_launcher.py
 Comment: 
 
-Filename: tlt/entrypoint/tao_deploy.py
+Filename: nvidia_tao-5.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: tlt/license/EULA.pdf
+Filename: nvidia_tao-5.0.0.dist-info/METADATA
 Comment: 
 
-Filename: tlt/license/__init__.py
+Filename: nvidia_tao-5.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: nvidia_tao-4.0.1.dist-info/METADATA
+Filename: nvidia_tao-5.0.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: nvidia_tao-4.0.1.dist-info/WHEEL
+Filename: nvidia_tao-5.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: nvidia_tao-4.0.1.dist-info/entry_points.txt
-Comment: 
-
-Filename: nvidia_tao-4.0.1.dist-info/top_level.txt
-Comment: 
-
-Filename: nvidia_tao-4.0.1.dist-info/RECORD
+Filename: nvidia_tao-5.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `tlt/version.py` & `nvidia_tao_cli/version.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,27 @@
-# Copyright (c) 2017-2021, NVIDIA CORPORATION.  All rights reserved.
+# Copyright (c) 2023, NVIDIA CORPORATION.  All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 """Launcher SDK version."""
 
-MAJOR = 4
-MINOR = 0
-PATCH = 1
-PRE_RELEASE = ""
+MAJOR = "5"
+MINOR = "0"
+PATCH = "0"
+PRE_RELEASE = ''
 
 
 # Getting the build number.
 def get_build_info():
     """Get the build version number."""
     # required since setup.py runs a version string and global imports aren't executed.
     import os  # noqa pylint: disable=import-outside-toplevel
@@ -41,8 +53,8 @@
 __package_name__ = "nvidia-tao"
 __description__ = "NVIDIA's Launcher for TAO Toolkit."
 __keywords__ = "nvidia, tao, launcher"
 
 __contact_names__ = "Varun Praveen"
 __contact_emails__ = "vpraveen@nvidia.com"
 
-__license__ = "NVIDIA Proprietary Software"
+__license__ = "Apache 2.0"
```

## Comparing `tlt/components/docker_handler/docker_handler.py` & `nvidia_tao_cli/components/docker_handler/docker_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,20 @@
-# Copyright (c) 2017-2021, NVIDIA CORPORATION.  All rights reserved.
+# Copyright (c) 2023, NVIDIA CORPORATION.  All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 """A docker handler to interface with the docker.
 
 This component is responsible for:
 1. Interacting with the docker registry
 2. Pulling the docker from the registry
 3. Instantiating a docker locally.
 4. Executing the command locally.
@@ -16,29 +28,29 @@
 
 import docker
 from tabulate import tabulate
 
 DOCKER_COMMAND = "docker"
 DEFAULT_DOCKER_PATH = "unix://var/run/docker.sock"
 VALID_PORT_PROTOCOLS = ["tcp", "udp", "sctp"]
-VALID_DOCKER_ARGS = ["user", "ports", "shm_size", "ulimits", "privileged", "network"]
+VALID_DOCKER_ARGS = ["user", "ports", "shm_size", "ulimits", "privileged", "network", "tty"]
 
 logger = logging.getLogger(__name__)
 
 
 def get_default_mountsfile():
     """Get the default mounts file."""
     default_mounts = "~/.tao_mounts.json"
     if not os.path.exists(os.path.expanduser(default_mounts)):
         print(
             "~/.tao_mounts.json wasn't found. Falling back to obtain "
-            "mount points and docker configs from ~/.tlt_mounts.json.\n"
+            "mount points and docker configs from ~/.tao_mounts.json.\n"
             "Please note that this will be deprecated going forward."
         )
-        default_mounts = "~/.tlt_mounts.json"
+        default_mounts = "~/.tao_mounts.json"
     return default_mounts
 
 
 DOCKER_MOUNT_FILE = get_default_mountsfile()
 
 
 class DockerHandler(object):
@@ -62,30 +74,30 @@
         self._docker_client = docker.from_env()
         self._api_client = docker.APIClient(base_url=docker_env_path)
         self._docker_registry = docker_registry
         self._image_name = image_name
         self._docker_mount_file = os.path.expanduser(docker_mount_file)
         self._docker_tag = docker_tag
         self._docker_digest = docker_digest
-        self.docker_exec_command = "docker exec -it"
+        self.docker_exec_command = "docker exec"
         self.initialized = True
         self._container = None
 
     @staticmethod
     def _load_mounts_file(docker_mount_file):
         """Simple function to load the mount file."""
         with open(docker_mount_file, "r") as mfile:
             data = json.load(mfile)
         return data
 
     def _get_mount_env_data(self):
-        """Get the mounts from the tlt_mount.json file."""
+        """Get the mounts from the tao_mount.json file."""
         mount_points = []
         env_vars = []
-        docker_options = None
+        docker_options = dict()
         if not os.path.exists(self._docker_mount_file):
             logging.info(
                 "No mount points were found in the {} file.".format(self._docker_mount_file)
             )
             return mount_points, env_vars, docker_options
 
         # Load mounts file.
@@ -253,19 +265,23 @@
                 "\nDockerOptions portion of the \"{}\" file. You can obtain your"
                 "\nusers UID and GID by using the \"id -u\" and \"id -g\" commands on the"
                 "\nterminal.".format(self._docker_mount_file)
             )
         # Try instantiating a container and return error.
         try:
             logger.debug("Starting the TAO Toolkit Container: {}".format(self.docker_image))
+            tty = docker_args.get("tty", True)
+            if "tty" in docker_args.keys():
+                docker_args.pop("tty")
+            logger.info("Printing tty value {tty}".format(tty=tty))
             self._container = self._docker_client.containers.run(
                 "{}".format(self.docker_image),
                 command=None,
                 device_requests=self.get_device_requests(),
-                tty=True,
+                tty=tty,
                 stderr=True,
                 stdout=True,
                 detach=True,
                 volumes=volumes,
                 environment=env_vars,
                 remove=True,
                 **docker_args
@@ -282,42 +298,113 @@
                 "Pulling a new docker.")
             self.pull()
         mount_data, env_vars, docker_options = self._get_mount_env_data()
         volumes = self.formatted_mounts(mount_data)
         env_variables = self.formatted_envs(env_vars)
 
         # Start the container if the it isn't already.
+        tty = True
+        if "tty" in docker_options.keys():
+            tty = docker_options["tty"]
+
         self.start_container(volumes, env_variables, docker_options)
+        interactive_option = "-i"
+        if tty:
+            interactive_option = "-it"
 
-        formatted_command = "bash -c \'{} {} {}\'".format(
+        formatted_command = "bash -c \'{} {} {} {}\'".format(
             self.docker_exec_command,
+            interactive_option,
             self._container.id,
             task_command
         )
         logger.debug("volumes: {}".format(volumes))
         logger.debug("formatted_command: {}\nExecuting the command.".format(formatted_command))
         try:
             subprocess.check_call(
                 formatted_command,
                 shell=True,
-                stdout=sys.stdout,
-                env=os.environ
+                stdout=sys.stdout
             )
         except subprocess.CalledProcessError as e:
             if e.output is not None:
-                print("TLT command run failed with error: {}".format(e.output))
+                print("TAO command run failed with error: {}".format(e.output))
                 if self._container:
                     logger.info("Stopping container post instantiation")
                     self.stop_container()
                 sys.exit(-1)
         finally:
             if self._container:
                 logger.info("Stopping container.")
                 self.stop_container()
 
+    def run_container_on_ci(self, task_command):
+        """Simple function to run command on gitlab-ci."""
+        # TODO: @vpraveen: This is a temporary WAR to make sure that the
+        # gitlab tty issue doesn't block CI automation of notebooks.
+        # will need to revisit this asap before the code freeze.
+        if not self._check_image_exists():
+            logger.info(
+                "The required docker doesn't exist locally/the manifest has changed. "
+                "Pulling a new docker.")
+            self.pull()
+        mount_data, env_vars, docker_options = self._get_mount_env_data()
+        volumes = self.formatted_mounts(mount_data)
+        env_variables = self.formatted_envs(env_vars)
+
+        volume_args = " ".join(
+            [f"-v {source}:{value['bind']}:{value['mode']}" for source, value in volumes.items()]
+        )
+        env_args = " ".join(
+            [f"-e {env_var}" for env_var in env_variables]
+        )
+
+        # Start the container if the it isn't already.
+        interactive_option = "-i"
+        if docker_options.get("tty", True):
+            interactive_option += "t"
+
+        docker_command = [
+            "docker run",
+            f"{interactive_option}",
+            "--rm",
+            "--gpus all",
+            f"{volume_args}",
+            f"{env_args}",
+        ]
+        options = []
+        for option, value in docker_options.items():
+            if option == "privileged" and value:
+                options.append("--privileged")
+            if option == "shm_size":
+                options.append(f"--shm-size {value}")
+        docker_command.extend(options)
+
+        formatted_command = "{} {} {}".format(
+            " ".join(docker_command),
+            self.docker_image,
+            task_command
+        )
+
+        logger.debug("volumes: {}".format(volumes))
+        logger.debug("formatted_command: {}\nExecuting the command.".format(formatted_command))
+        try:
+            subprocess.check_call(
+                formatted_command,
+                shell=True,
+                stdout=sys.stdout
+            )
+        except subprocess.CalledProcessError as e:
+            if e.output is not None:
+                print("TAO command run failed with error: {}".format(e.output))
+                if self._container:
+                    logger.info("Stopping container post instantiation")
+                    self.stop_container()
+                sys.exit(-1)
+
     def stop_container(self):
         """Stop an instantiated container."""
         logger.debug("Stopping the container: {}".format(
             self.container_id
         ))
         self._container.stop()
```

## Comparing `tlt/components/instance_handler/local_instance.py` & `nvidia_tao_cli/components/instance_handler/local_instance.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,53 @@
-# Copyright (c) 2017-2021, NVIDIA CORPORATION.  All rights reserved.
+# Copyright (c) 2023, NVIDIA CORPORATION.  All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 """TAO Toolkit instance handler for launching jobs locally."""
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 import argparse
+import json
 import logging
 import os
 import sys
 import textwrap
 
 from tabulate import tabulate
-from tlt.components.docker_handler.docker_handler import (
+from nvidia_tao_cli.components.docker_handler.docker_handler import (
     DOCKER_MOUNT_FILE,
     DockerHandler
 )
-from tlt.components.instance_handler.base_instance import TLTInstance
-from tlt.components.instance_handler.utils import (
+from nvidia_tao_cli.components.instance_handler.base_instance import TAOInstance
+from nvidia_tao_cli.components.instance_handler.utils import (
     docker_logged_in,
     load_config_file,
 )
-from tlt.components.types.task import Task
+from nvidia_tao_cli.components.types.task import Task
 
 logger = logging.getLogger(__name__)
 
+TAB_SPACE = 4
+TABS = " " * TAB_SPACE
 
-class LocalInstance(TLTInstance):
+
+class LocalInstance(TAOInstance):
     """Instance handler class to define a TAO Toolkit instance."""
 
     def __init__(self, task_map, docker_images, config_path):
         """Initialize a local TAO Toolkit instance.
 
         Args:
             task_map(dict): Dictionary of task name to Task data structure.
@@ -69,67 +85,105 @@
         Returns:
             task_map(dict): Dictionary of tasks mapped to the respective dockers.
         """
         if "format_version" not in config_data.keys():
             raise KeyError("format is a required key in the launcher config.")
 
         task_map = {}
+        docker_images = set()
         if config_data["format_version"] == 1.0:
+            local_map = {}
             for image in list(config_data["dockers"].keys()):
                 logger.debug("Processing {}".format(image))
                 docker_data = config_data["dockers"][image]
                 if "tasks" not in list(docker_data.keys()):
                     raise NotImplementedError(
                         "The config data must contain tasks associated with the "
                         "respective docker."
                     )
-                task_map.update({
+                local_map.update({
                     task: Task(
                         name=task,
                         docker_image=image,
                         docker_tag=docker_data["docker_tag"],
                         docker_registry=docker_data["docker_registry"],
                         docker_digest=docker_data["docker_digest"] if "docker_digest" in docker_data.keys() else None
                     ) for task in docker_data["tasks"]
                 })
+                docker_images.add(image)
+            task_map["container_actions"] = local_map
         elif config_data["format_version"] == 2.0:
+            local_map = {}
             for image in list(config_data["dockers"].keys()):
                 logger.debug("Processing {}".format(image))
                 docker_data = config_data["dockers"][image]
                 if not isinstance(docker_data, dict):
-                    raise("Invalid format.")
-                task_map.update({
+                    raise ValueError("Invalid format.")
+                local_map.update({
                     task: Task(
                         name=task,
                         docker_image=image,
                         docker_tag=tag,
                         docker_registry=docker_data[tag]["docker_registry"],
                         docker_digest=docker_data[tag]["docker_digest"] if "docker_digest" in docker_data[tag].keys() else None
                     ) for tag in docker_data.keys() for task in docker_data[tag]["tasks"]
                 })
+                docker_images.add(image)
+            task_map["container_actions"] = local_map
+        elif config_data["format_version"] == 3.0:
+            for task_group, group_data in config_data["task_group"].items():
+                logger.debug("Configuring task group {task_group}".format(
+                    task_group=task_group
+                ))
+                local_map = {}
+                for image, image_data in group_data["dockers"].items():
+                    logger.debug(
+                        "Extracting tasks from docker {image}".format(
+                            image=image
+                        )
+                    )
+                    if not isinstance(image_data, dict):
+                        raise ValueError(f"Invalid data format for images {type(image_data)} encountered.")
+                    logger.debug(json.dumps(image_data, indent=4))
+                    local_map.update({
+                        task: Task(
+                            name=task,
+                            docker_image=image,
+                            docker_tag=tag,
+                            docker_registry=image_data[tag]["docker_registry"],
+                            docker_digest=image_data[tag].get("docker_digest", None)
+                        ) for tag in image_data.keys() for task in image_data[tag]["tasks"]
+                    })
+                    docker_images.add(image)
+                task_map[task_group] = local_map
         else:
             raise NotImplementedError("Invalid format type: {}".format(config_data["format_version"]))
-        return task_map
+        return task_map, docker_images
 
     @classmethod
     def from_config(cls, config_path):
         """Instantiate a TAO Toolkit instance from a config file.
 
         Args:
             config_path(str): Path to the launcher config file.
 
         Returns:
             Initialized LocalInstance object.
         """
         config_data = cls.load_config(config_path)
-        docker_images = list(config_data["dockers"].keys())
-        task_map = cls.parse_launcher_config(config_data)
+        task_map, docker_images = cls.parse_launcher_config(config_data)
         debug_string = ""
         for task_name, task in task_map.items():
-            debug_string += f"{task_name}: {str(task)}\n"
+            if config_data["format_version"] == 3.0:
+                task_list = ""
+                for name, task_data in task.items():
+                    task_list += f"{name}: {str(task_data)}\n"
+                debug_string = f"{task_name}: {task_list}"
+            else:
+                debug_string += f"\n {task_name}: {str(task)}\n"
         logger.debug(debug_string)
         return LocalInstance(
             task_map,
             docker_images,
             config_path
         )
 
@@ -137,24 +191,26 @@
     def handler_map(self):
         """Get image to handler map."""
         handler_map = {}
         # Build a handler map for the local instance.
         assert bool(self.task_map), (
             "A valid task map wasn't provided."
         )
-        for _, map_val in self.task_map.items():
-            handler_key = f"{map_val.docker_image}:{map_val.docker_tag}"
-            if handler_key not in handler_map.keys():
-                handler_map[handler_key] = DockerHandler(
-                    docker_registry=map_val.docker_registry,
-                    image_name=map_val.docker_image,
-                    docker_tag=map_val.docker_tag,
-                    docker_digest=map_val.docker_digest,
-                    docker_mount_file=os.getenv("LAUNCHER_MOUNTS", DOCKER_MOUNT_FILE)
-                )
+        logger.debug("Acquiring handler map for dockers.")
+        for _, tasks_dict in self.task_map.items():
+            for _, map_val in tasks_dict.items():
+                handler_key = f"{map_val.docker_image}:{map_val.docker_tag}"
+                if handler_key not in handler_map.keys():
+                    handler_map[handler_key] = DockerHandler(
+                        docker_registry=map_val.docker_registry,
+                        image_name=map_val.docker_image,
+                        docker_tag=map_val.docker_tag,
+                        docker_digest=map_val.docker_digest,
+                        docker_mount_file=os.getenv("LAUNCHER_MOUNTS", DOCKER_MOUNT_FILE)
+                    )
         return handler_map
 
     @property
     def _docker_client(self):
         """Get a docker handler to interact with the docker client."""
         docker_handler = list(self.handler_map.values())[0]
         return docker_handler._docker_client
@@ -184,37 +240,39 @@
                       "Please run tao stop --help for more information.")
 
     def list_running_jobs(self):
         """Simple function to list all existing jobs in a container."""
         container_list = self._get_running_containers()
         command_per_container = {}
         # Map the commands to the containers.
-        for container in container_list:
-            procs_list = container.top()
-            command_per_container[container] = ""
-            for item in procs_list["Processes"]:
-                # Getting the command from the row returned by container top.
-                command = item[-1:][0]
-                # Extracting entrypoint from the running command.
-                task_point = command.split(" ")
-                if len(task_point) < 2:
-                    continue
-                task_point = task_point[1]
-                # Since only 1 entrypoint will be launched per container, we only care
-                # about finding the process for that entrypoint.
-                if task_point.split("/")[-1] in self.task_map.keys():
-                    command_per_container[container] = "{} {}".format(
-                        task_point.split("/")[-1],
-                        " ".join(command.split(" ")[2:])
-                    )
-                    # We break from here because the launcher is currently designed to
-                    # handle one command per container. And since we only expose the entrypoints
-                    # we only need to look for the entrypoints running in the container.
-                    # TODO @vpraveen: We may need to change this in the future.
-                    break
+        for task_group in self.task_map.keys():
+            tasks_per_group = self.task_map[task_group].keys()
+            for container in container_list:
+                procs_list = container.top()
+                command_per_container[container] = ""
+                for item in procs_list["Processes"]:
+                    # Getting the command from the row returned by container top.
+                    command = item[-1:][0]
+                    # Extracting entrypoint from the running command.
+                    task_point = command.split(" ")
+                    if len(task_point) < 2:
+                        continue
+                    task_point = task_point[1]
+                    # Since only 1 entrypoint will be launched per container, we only care
+                    # about finding the process for that entrypoint.
+                    if task_point.split("/")[-1] in tasks_per_group:
+                        command_per_container[container] = "{} {}".format(
+                            task_point.split("/")[-1],
+                            " ".join(command.split(" ")[2:])
+                        )
+                        # We break from here because the launcher is currently designed to
+                        # handle one command per container. And since we only expose the entrypoints
+                        # we only need to look for the entrypoints running in the container.
+                        # TODO @vpraveen: We may need to change this in the future.
+                        break
 
         # Tabulate and print out the processes.
         self.pretty_print(command_per_container)
 
     def print_information(self, verbose=False):
         """Print the information of the current TAO Toolkit."""
         print("Configuration of the TAO Toolkit Instance")
@@ -240,24 +298,24 @@
             dictionary (dict): Dictionary to recursive print
             nlevels (int): Tab indentation level.
 
         Returns:
             output_string (str): Formatted print string.
         """
         assert isinstance(dictionary, dict), ""
-        output_string = "{}".format("\t" * nlevels)
+        output_string = "{}".format(f"{TABS}" * nlevels)
         for key, value in dictionary.items():
-            output_string += "\n{}{}: ".format("\t" * nlevels, key)
+            output_string += "\n{}{}: ".format(f"{TABS}" * nlevels, key)
             if isinstance(value, dict):
-                output_string += "\t{}".format(
-                    self.dict_print(value, nlevels + 1)
+                output_string += "{}{}".format(
+                    TABS, self.dict_print(value, nlevels + 1)
                 )
             elif isinstance(value, list):
                 for idx, item in enumerate(value, start=1):
-                    output_string += "\n{}{}. {}".format("\t" * (nlevels + 1),
+                    output_string += "\n{}{}. {}".format(f"{TABS}" * (nlevels + 1),
                                                          idx,
                                                          item)
             else:
                 output_string += "{}".format(value)
         return output_string
 
     @staticmethod
@@ -272,65 +330,70 @@
             data.append([
                 container.short_id,
                 container.status,
                 textwrap.fill(container_string, width=100)]
             )
         print(tabulate(data, headers=headers, tablefmt="rst"))
 
-    def launch_command(self, task, args):
+    def launch_command(self, task_group, task, args):
         """Launch command in the respective docker.
 
         Args:
             task(str): Name of the task from the entrypoint.
             args(list): List of args to the task in the docker.
 
         Returns:
             No explicit returns.
         """
-        if task in list(self.task_map.keys()):
-            assert isinstance(args, list), (
-                "The arguments must be given as a list to be passed "
-                "to the docker. Got a {} instead".format(
-                    type(args)
+        if task_group in self.task_map.keys():
+            task_map = self.task_map[task_group]
+            if task in list(task_map.keys()):
+                assert isinstance(args, list), (
+                    "The arguments must be given as a list to be passed "
+                    "to the docker. Got a {} instead".format(
+                        type(args)
+                    )
                 )
-            )
-            docker_logged_in(required_registry=self.task_map[task].docker_registry)
-            docker_handler = self.handler_map[
-                f"{self.task_map[task].docker_image}:{self.task_map[task].docker_tag}"
-            ]
-            logger.info(
-                "Running command in container: {}".format(docker_handler.docker_image)
-            )
-            if args:
-                command = ""
-                if args[0] == "run":
-                    args.pop(0)
-                else:
-                    command = "{} ".format(task)
-                command += " ".join(args)
-            else:
+                docker_logged_in(required_registry=task_map[task].docker_registry)
+                docker_handler = self.handler_map[
+                    f"{task_map[task].docker_image}:{task_map[task].docker_tag}"
+                ]
                 logger.info(
-                    "No commands provided to the launcher\n"
-                    "Kicking off an interactive docker session.\n"
-                    "NOTE: This container instance will be terminated "
-                    "when you exit."
+                    "Running command in container: {}".format(docker_handler.docker_image)
                 )
-                command = "/bin/bash"
-            # Running command in the container.
-            docker_handler.run_container(command)
+                if args:
+                    command = ""
+                    if args[0] == "run":
+                        args.pop(0)
+                    else:
+                        command = "{} ".format(task)
+                    command += " ".join(args)
+                else:
+                    logger.info(
+                        "No commands provided to the launcher\n"
+                        "Kicking off an interactive docker session.\n"
+                        "NOTE: This container instance will be terminated "
+                        "when you exit."
+                    )
+                    command = "/bin/bash"
+                # Running command in the container.
+                if os.getenv("CI_PROJECT_DIR", None) is not None:
+                    docker_handler.run_container_on_ci(command)
+                else:
+                    docker_handler.run_container(command)
         else:
-            assert task in self.instance_handler_tasks, (
+            assert task_group in self.instance_handler_tasks, (
                 "The tasks provided must be in instance handlers tasks or supported DL tasks."
             )
             assert isinstance(args, argparse.Namespace), {
                 "The arguments passed to the instance tasks must be argpase.Namespace to a dictionary."
                 "Type got here is: {}".format(type(args))
             }
-            if task == "list":
+            if task_group == "list":
                 self.list_running_jobs()
-            elif task == "stop":
+            elif task_group == "stop":
                 self.kill_containers(args.container_id, args.all)
-            elif task == "info":
+            elif task_group == "info":
                 self.print_information(verbose=args.verbose)
             else:
                 raise NotImplementedError(
                     "Task asked for wasn't implemented. {}".format(task))
```

## Comparing `tlt/components/instance_handler/utils.py` & `nvidia_tao_cli/components/instance_handler/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,20 @@
-# Copyright (c) 2017-2021, NVIDIA CORPORATION.  All rights reserved.
+# Copyright (c) 2023, NVIDIA CORPORATION.  All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 """Utilities for the TAO Toolkit instance handler."""
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
@@ -13,16 +25,16 @@
 
 logger = logging.getLogger(__name__)
 
 # Setup default paths.
 DOCKER_CONFIG = os.path.expanduser("~/.docker/config.json")
 
 # Launcher config and drive maps.
-OVERRIDE_CONFIG = os.path.expanduser("~/.tlt/config.json")
-DEPLOY_OVERRIDE_CONFIG = os.path.expanduser("~/.tlt/config_deploy.json")
+OVERRIDE_CONFIG = os.path.expanduser("~/.tao/config.json")
+DEPLOY_OVERRIDE_CONFIG = os.path.expanduser("~/.tao/config_deploy.json")
 
 # Docker registries supported.
 INTERNAL = os.getenv("LAUNCHER_MODE_INTERNAL", "0") == "1"
 REQUIRED_REGISTRIES = ["nvcr.io"]
 if INTERNAL:
     REQUIRED_REGISTRIES.append("stg.nvcr.io")
 
@@ -130,30 +142,34 @@
         config_file_path
     )
     return True
 
 
 def docker_logged_in(docker_config=DOCKER_CONFIG, required_registry=REQUIRED_REGISTRIES):
     """Simple function to warn the user the docker registry required hasn't been logged in."""
-    data = load_config_file(docker_config)
-
-    if "auths" not in list(data.keys()):
-        raise ValueError(
-            "Docker CLI hasn't been logged in to a registry."
-            "Please run `docker login nvcr.io`"
-        )
-    if not isinstance(required_registry, list):
-        required_registry = [required_registry]
-    logging.info("Registry: {}".format(required_registry))
-    registry_status = [registry in list(data["auths"].keys()) for registry in required_registry]
-
-    def error_msg(registry_status):
-        emsg = ""
-        for idx, status in enumerate(registry_status):
-            if not status:
-                emsg += "\nDocker not logged in to {}. Please run docker login {}".format(
-                    required_registry[idx], required_registry[idx]
-                )
-        return emsg
-    assert all(
-        [registry in list(data["auths"].keys()) for registry in required_registry]
-    ), error_msg(registry_status)
+    override_registry = os.getenv("OVERRIDE_REGISTRY", None)
+    if override_registry is None:
+        data = load_config_file(docker_config)
+
+        if "auths" not in list(data.keys()):
+            raise ValueError(
+                "Docker CLI hasn't been logged in to a registry."
+                "Please run `docker login nvcr.io`"
+            )
+        if not isinstance(required_registry, list):
+            required_registry = [required_registry]
+        logging.info("Registry: {}".format(required_registry))
+        registry_status = [registry in list(data["auths"].keys()) for registry in required_registry]
+
+        def error_msg(registry_status):
+            emsg = ""
+            for idx, status in enumerate(registry_status):
+                if not status:
+                    emsg += "\nDocker not logged in to {}. Please run docker login {}".format(
+                        required_registry[idx], required_registry[idx]
+                    )
+            return emsg
+        assert all(
+            [registry in list(data["auths"].keys()) for registry in required_registry]
+        ), error_msg(registry_status)
+    else:
+        logger.info("Skipping docker login check.")
```

## Comparing `tlt/config/config.json` & `nvidia_tao_cli/config/config.json`

 * *Files 24% similar despite different names*

### Pretty-printed

 * *Similarity: 0.3%*

 * *Differences: {"'format_version'": '3.0',*

 * * "'published_date'": "'07/14/2023'",*

 * * "'task_group'": "OrderedDict([('model', OrderedDict([('dockers', "*

 * *                 "OrderedDict([('nvidia/tao/tao-toolkit', OrderedDict([('5.0.0-tf2.11.0', "*

 * *                 "OrderedDict([('docker_registry', 'nvcr.io'), ('tasks', ['classification_tf2', "*

 * *                 "'efficientdet_tf2'])])), ('5.0.0-tf1.15.5', OrderedDict([('docker_registry', "*

 * *                 "'nvcr.io'), ('tasks', ['bpnet', 'classification_tf1', 'converter', "*

 * *      […]*

```diff
@@ -1,72 +1,111 @@
 {
-    "dockers": {
-        "nvidia/tao/tao-toolkit": {
-            "4.0.0-pyt": {
-                "docker_registry": "nvcr.io",
-                "tasks": [
-                    "action_recognition",
-                    "deformable_detr",
-                    "segformer",
-                    "re_identification",
-                    "pointpillars",
-                    "pose_classification",
-                    "n_gram",
-                    "speech_to_text",
-                    "speech_to_text_citrinet",
-                    "speech_to_text_conformer",
-                    "spectro_gen",
-                    "vocoder",
-                    "text_classification",
-                    "question_answering",
-                    "token_classification",
-                    "intent_slot_classification",
-                    "punctuation_and_capitalization"
-                ]
-            },
-            "4.0.0-tf1.15.5": {
-                "docker_registry": "nvcr.io",
-                "tasks": [
-                    "augment",
-                    "bpnet",
-                    "classification_tf1",
-                    "detectnet_v2",
-                    "dssd",
-                    "emotionnet",
-                    "efficientdet_tf1",
-                    "faster_rcnn",
-                    "fpenet",
-                    "gazenet",
-                    "gesturenet",
-                    "heartratenet",
-                    "lprnet",
-                    "mask_rcnn",
-                    "multitask_classification",
-                    "retinanet",
-                    "ssd",
-                    "unet",
-                    "yolo_v3",
-                    "yolo_v4",
-                    "yolo_v4_tiny",
-                    "converter"
-                ]
-            },
-            "4.0.0-tf2.9.1": {
-                "docker_registry": "nvcr.io",
-                "tasks": [
-                    "classification_tf2",
-                    "efficientdet_tf2"
-                ]
-            },
-            "4.0.1-tf1.15.5": {
-                "docker_registry": "nvcr.io",
-                "tasks": [
-                    "mask_rcnn",
-                    "unet"
-                ]
+    "format_version": 3.0,
+    "published_date": "07/14/2023",
+    "task_group": {
+        "dataset": {
+            "dockers": {
+                "nvidia/tao/tao-toolkit": {
+                    "5.0.0-data-services": {
+                        "docker_registry": "nvcr.io",
+                        "tasks": [
+                            "augmentation",
+                            "auto_label",
+                            "annotations",
+                            "analytics"
+                        ]
+                    }
+                }
+            }
+        },
+        "deploy": {
+            "dockers": {
+                "nvidia/tao/tao-toolkit": {
+                    "5.0.0-deploy": {
+                        "docker_registry": "nvcr.io",
+                        "tasks": [
+                            "classification_pyt",
+                            "classification_tf1",
+                            "classification_tf2",
+                            "deformable_detr",
+                            "detectnet_v2",
+                            "dino",
+                            "dssd",
+                            "efficientdet_tf1",
+                            "efficientdet_tf2",
+                            "faster_rcnn",
+                            "lprnet",
+                            "mask_rcnn",
+                            "ml_recog",
+                            "multitask_classification",
+                            "ocdnet",
+                            "ocrnet",
+                            "optical_inspection",
+                            "retinanet",
+                            "segformer",
+                            "ssd",
+                            "trtexec",
+                            "unet",
+                            "yolo_v3",
+                            "yolo_v4",
+                            "yolo_v4_tiny"
+                        ]
+                    }
+                }
+            }
+        },
+        "model": {
+            "dockers": {
+                "nvidia/tao/tao-toolkit": {
+                    "5.0.0-pyt": {
+                        "docker_registry": "nvcr.io",
+                        "tasks": [
+                            "action_recognition",
+                            "classification_pyt",
+                            "deformable_detr",
+                            "dino",
+                            "mal",
+                            "ml_recog",
+                            "ocdnet",
+                            "ocrnet",
+                            "optical_inspection",
+                            "pointpillars",
+                            "pose_classification",
+                            "re_identification",
+                            "segformer"
+                        ]
+                    },
+                    "5.0.0-tf1.15.5": {
+                        "docker_registry": "nvcr.io",
+                        "tasks": [
+                            "bpnet",
+                            "classification_tf1",
+                            "converter",
+                            "detectnet_v2",
+                            "dssd",
+                            "efficientdet_tf1",
+                            "faster_rcnn",
+                            "fpenet",
+                            "lprnet",
+                            "mask_rcnn",
+                            "multitask_classification",
+                            "retinanet",
+                            "ssd",
+                            "unet",
+                            "yolo_v3",
+                            "yolo_v4",
+                            "yolo_v4_tiny"
+                        ]
+                    },
+                    "5.0.0-tf2.11.0": {
+                        "docker_registry": "nvcr.io",
+                        "tasks": [
+                            "classification_tf2",
+                            "efficientdet_tf2"
+                        ]
+                    }
+                }
             }
         }
     },
-    "format_version": 2.0,
-    "published_date": "03/06/2023",
-    "toolkit_version": "4.0.1"
+    "toolkit_version": "5.0.0"
 }
```

