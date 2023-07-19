# Comparing `tmp/rclone-python-0.1.7.tar.gz` & `tmp/rclone-python-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rclone-python-0.1.7.tar", last modified: Mon Jun 19 09:29:26 2023, max compression
+gzip compressed data, was "rclone-python-0.1.8.tar", last modified: Wed Jul 19 05:54:43 2023, max compression
```

## Comparing `rclone-python-0.1.7.tar` & `rclone-python-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:29:26.798952 rclone-python-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-19 09:29:14.000000 rclone-python-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-19 09:29:26.798952 rclone-python-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-19 09:29:14.000000 rclone-python-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:29:26.798952 rclone-python-0.1.7/rclone_python/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 09:29:14.000000 rclone-python-0.1.7/rclone_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-19 09:29:14.000000 rclone-python-0.1.7/rclone_python/extract_remotenames.py
--rw-r--r--   0 runner    (1001) docker     (123)    15185 2023-06-19 09:29:14.000000 rclone-python-0.1.7/rclone_python/rclone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-19 09:29:14.000000 rclone-python-0.1.7/rclone_python/remote_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-06-19 09:29:14.000000 rclone-python-0.1.7/rclone_python/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:29:26.798952 rclone-python-0.1.7/rclone_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-19 09:29:26.000000 rclone-python-0.1.7/rclone_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-19 09:29:26.000000 rclone-python-0.1.7/rclone_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 09:29:26.000000 rclone-python-0.1.7/rclone_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-19 09:29:26.000000 rclone-python-0.1.7/rclone_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 09:29:26.000000 rclone-python-0.1.7/rclone_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 09:29:26.798952 rclone-python-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-19 09:29:14.000000 rclone-python-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:54:43.910553 rclone-python-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-19 05:54:32.000000 rclone-python-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-19 05:54:43.910553 rclone-python-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-19 05:54:32.000000 rclone-python-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:54:43.910553 rclone-python-0.1.8/rclone_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-19 05:54:32.000000 rclone-python-0.1.8/rclone_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-19 05:54:32.000000 rclone-python-0.1.8/rclone_python/extract_remotenames.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12976 2023-07-19 05:54:32.000000 rclone-python-0.1.8/rclone_python/rclone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-19 05:54:32.000000 rclone-python-0.1.8/rclone_python/remote_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-07-19 05:54:32.000000 rclone-python-0.1.8/rclone_python/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:54:43.910553 rclone-python-0.1.8/rclone_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-19 05:54:43.000000 rclone-python-0.1.8/rclone_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-19 05:54:43.000000 rclone-python-0.1.8/rclone_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 05:54:43.000000 rclone-python-0.1.8/rclone_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-19 05:54:43.000000 rclone-python-0.1.8/rclone_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-19 05:54:43.000000 rclone-python-0.1.8/rclone_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 05:54:43.910553 rclone-python-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-19 05:54:32.000000 rclone-python-0.1.8/setup.py
```

### Comparing `rclone-python-0.1.7/LICENSE` & `rclone-python-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rclone-python-0.1.7/PKG-INFO` & `rclone-python-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclone-python
-Version: 0.1.7
+Version: 0.1.8
 Summary: A python wrapper for rclone.
 Home-page: https://github.com/Johannes11833/rclone_python
 Author: Johannes Gundlach
 Keywords: rclone,wrapper,cloud sync
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rclone-python-0.1.7/README.md` & `rclone-python-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `rclone-python-0.1.7/rclone_python/extract_remotenames.py` & `rclone-python-0.1.8/rclone_python/extract_remotenames.py`

 * *Files identical despite different names*

### Comparing `rclone-python-0.1.7/rclone_python/rclone.py` & `rclone-python-0.1.8/rclone_python/rclone.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import json
 import logging
-import re
-import subprocess
 from functools import wraps
-from pathlib import Path
 from shutil import which
-from typing import Union, List, Dict, Tuple, Callable, Any
+from typing import Union, List, Dict, Callable, Any
 
 from rclone_python import utils
 from rclone_python.remote_types import RemoteTypes
 
 
 def __check_installed(func):
     @wraps(func)
@@ -261,14 +258,47 @@
     if process.returncode == 0:
         logging.info(f"Successfully deleted {path}")
     else:
         raise Exception(
             f'Deleting path "{path}" failed with error message:\n{process.stderr}'
         )
 
+@__check_installed
+def link(
+    path: str,
+    expire: Union[str, None] = None,
+    unlink=False,
+    args=None,
+) -> str:
+    """
+    Generates a public link to a file/directory.
+    :param path: The path to the file/directory that a public link should be created, retrieved or removed for.
+    :param expire: The amount of time that the link will be valid (not supported by all backends).
+    :param unlink: If true, remove existing public links to the file or directory (not supported by all backends).
+    :param args: List of additional arguments/ flags.
+    :return: The link to the given file or directory.
+    """
+    if args is None:
+        args = []
+
+    command = f'rclone link "{path}"'
+
+    # add optional parameters
+    if expire is not None:
+        args.append(f"--expire {expire}")
+    if unlink:
+        args.append(f"--unlink")
+
+    process = utils.run_cmd(command, args)
+
+    if process.returncode != 0:
+        raise Exception(process.stderr)
+    else:
+        return process.stdout
+
 
 @__check_installed
 def ls(
     path: str,
     max_depth: Union[int, None] = None,
     dirs_only=False,
     files_only=False,
@@ -367,112 +397,19 @@
     # out path
     command += f' "{out_path}"'
 
     # optional named arguments/flags
     command += utils.args2string(args)
 
     # execute the upload command
-    process = _rclone_progress(
+    process = utils.rclone_progress(
         command, prog_title, listener=listener, show_progress=show_progress
     )
 
     if process.wait() == 0:
         logging.info("Cloud upload completed.")
     else:
         _, err = process.communicate()
         raise Exception(
             f"Copy/Move operation from {in_path} to {out_path}"
             f' failed with error message:\n{err.decode("utf-8")}'
         )
-
-
-def _rclone_progress(
-    command: str,
-    pbar_title: str,
-    stderr=subprocess.PIPE,
-    show_progress=True,
-    listener: Callable[[Dict], None] = None,
-) -> subprocess.Popen:
-    buffer = ""
-    pbar = None
-    total_progress_id = None
-    subprocesses = {}
-
-    if show_progress:
-        pbar, total_progress_id = utils.create_progress_bar(pbar_title)
-
-    process = subprocess.Popen(
-        command, stdout=subprocess.PIPE, stderr=stderr, shell=True
-    )
-    for line in iter(process.stdout.readline, b""):
-        var = line.decode()
-
-        valid, update_dict = _extract_rclone_progress(buffer)
-
-        if valid:
-            if show_progress:
-                utils.update_tasks(pbar, total_progress_id, update_dict, subprocesses)
-
-            # call the listener
-            if listener:
-                listener(update_dict)
-
-            # reset the buffer
-            buffer = ""
-        else:
-            # buffer until we
-            buffer += var
-
-    if show_progress:
-        utils.complete_task(total_progress_id, pbar)
-        for _, task_id in subprocesses.items():
-            # hide all subprocesses
-            pbar.update(task_id=task_id, visible=False)
-        pbar.stop()
-
-    return process
-
-
-def _extract_rclone_progress(buffer: str) -> Tuple[bool, Union[Dict[str, Any], None]]:
-    # matcher that checks if the progress update block is completely buffered yet (defines start and stop)
-    # it gets the sent bits, total bits, progress, transfer-speed and eta
-    reg_transferred = re.findall(
-        r"Transferred:\s+(\d+.\d+ \w+) \/ (\d+.\d+ \w+), (\d{1,3})%, (\d+.\d+ \w+\/\w+), ETA (\S+)",
-        buffer,
-    )
-
-    if reg_transferred:  # transferred block is completely buffered
-        # get the progress of the individual files
-        # matcher gets the currently transferring files and their individual progress
-        # returns list of tuples: (name, progress, file_size, unit)
-        prog_transferring = []
-        prog_regex = re.findall(
-            r"\* +(\S+):[ ]+(\d{1,2})% \/(\d+.\d+)([a-zA-Z]+),", buffer
-        )
-        for item in prog_regex:
-            prog_transferring.append(
-                (
-                    item[0],
-                    int(item[1]),
-                    float(item[2]),
-                    # the suffix B of the unit is missing for subprocesses
-                    item[3] + "B",
-                )
-            )
-
-        out = {"prog_transferring": prog_transferring}
-        sent_bits, total_bits, progress, transfer_speed_str, eta = reg_transferred[0]
-        out["progress"] = float(progress.strip())
-        out["total_bits"] = float(re.findall(r"\d+.\d+", total_bits)[0])
-        out["sent_bits"] = float(re.findall(r"\d+.\d+", sent_bits)[0])
-        out["unit_sent"] = re.findall(r"[a-zA-Z]+", sent_bits)[0]
-        out["unit_total"] = re.findall(r"[a-zA-Z]+", total_bits)[0]
-        out["transfer_speed"] = float(re.findall(r"\d+.\d+", transfer_speed_str)[0])
-        out["transfer_speed_unit"] = re.findall(
-            r"[a-zA-Z]+/[a-zA-Z]+", transfer_speed_str
-        )[0]
-        out["eta"] = eta
-
-        return True, out
-
-    else:
-        return False, None
```

### Comparing `rclone-python-0.1.7/rclone_python/remote_types.py` & `rclone-python-0.1.8/rclone_python/remote_types.py`

 * *Files identical despite different names*

### Comparing `rclone-python-0.1.7/rclone_python.egg-info/PKG-INFO` & `rclone-python-0.1.8/rclone_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclone-python
-Version: 0.1.7
+Version: 0.1.8
 Summary: A python wrapper for rclone.
 Home-page: https://github.com/Johannes11833/rclone_python
 Author: Johannes Gundlach
 Keywords: rclone,wrapper,cloud sync
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rclone-python-0.1.7/setup.py` & `rclone-python-0.1.8/setup.py`

 * *Files identical despite different names*

