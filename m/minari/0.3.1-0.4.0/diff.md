# Comparing `tmp/minari-0.3.1.tar.gz` & `tmp/minari-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minari-0.3.1.tar", last modified: Fri May 19 03:57:36 2023, max compression
+gzip compressed data, was "minari-0.4.0.tar", last modified: Wed Jul 19 13:34:21 2023, max compression
```

## Comparing `minari-0.3.1.tar` & `minari-0.4.0.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:57:36.166160 minari-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-05-19 03:57:21.000000 minari-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-19 03:57:36.166160 minari-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-19 03:57:21.000000 minari-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:57:36.158160 minari-0.3.1/minari/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-19 03:57:21.000000 minari-0.3.1/minari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-05-19 03:57:21.000000 minari-0.3.1/minari/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:57:36.162160 minari-0.3.1/minari/data_collector/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-19 03:57:21.000000 minari-0.3.1/minari/data_collector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:57:36.162160 minari-0.3.1/minari/data_collector/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-19 03:57:21.000000 minari-0.3.1/minari/data_collector/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-19 03:57:21.000000 minari-0.3.1/minari/data_collector/callbacks/episode_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-05-19 03:57:21.000000 minari-0.3.1/minari/data_collector/callbacks/step_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    19889 2023-05-19 03:57:21.000000 minari-0.3.1/minari/data_collector/data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:57:36.162160 minari-0.3.1/minari/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 03:57:21.000000 minari-0.3.1/minari/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-05-19 03:57:21.000000 minari-0.3.1/minari/dataset/minari_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-19 03:57:21.000000 minari-0.3.1/minari/dataset/minari_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:57:36.162160 minari-0.3.1/minari/storage/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-19 03:57:21.000000 minari-0.3.1/minari/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-19 03:57:21.000000 minari-0.3.1/minari/storage/datasets_root_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-05-19 03:57:21.000000 minari-0.3.1/minari/storage/hosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-19 03:57:21.000000 minari-0.3.1/minari/storage/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    15749 2023-05-19 03:57:21.000000 minari-0.3.1/minari/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:57:36.162160 minari-0.3.1/minari.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-19 03:57:36.000000 minari-0.3.1/minari.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-19 03:57:36.000000 minari-0.3.1/minari.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 03:57:36.000000 minari-0.3.1/minari.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-19 03:57:36.000000 minari-0.3.1/minari.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-19 03:57:36.000000 minari-0.3.1/minari.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 03:57:36.000000 minari-0.3.1/minari.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-19 03:57:21.000000 minari-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 03:57:36.166160 minari-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-19 03:57:21.000000 minari-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 03:57:36.166160 minari-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-05-19 03:57:21.000000 minari-0.3.1/tests/test_dataset_combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-05-19 03:57:21.000000 minari-0.3.1/tests/test_dataset_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-19 03:57:21.000000 minari-0.3.1/tests/test_dataset_download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:34:21.716521 minari-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-07-19 13:34:05.000000 minari-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-19 13:34:21.716521 minari-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-19 13:34:05.000000 minari-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:34:21.712520 minari-0.4.0/minari/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-19 13:34:05.000000 minari-0.4.0/minari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-07-19 13:34:05.000000 minari-0.4.0/minari/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:34:21.716521 minari-0.4.0/minari/data_collector/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-19 13:34:05.000000 minari-0.4.0/minari/data_collector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:34:21.716521 minari-0.4.0/minari/data_collector/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-19 13:34:05.000000 minari-0.4.0/minari/data_collector/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-19 13:34:05.000000 minari-0.4.0/minari/data_collector/callbacks/episode_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-19 13:34:05.000000 minari-0.4.0/minari/data_collector/callbacks/step_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22904 2023-07-19 13:34:05.000000 minari-0.4.0/minari/data_collector/data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:34:21.716521 minari-0.4.0/minari/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 13:34:05.000000 minari-0.4.0/minari/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12389 2023-07-19 13:34:05.000000 minari-0.4.0/minari/dataset/minari_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-07-19 13:34:05.000000 minari-0.4.0/minari/dataset/minari_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-07-19 13:34:05.000000 minari-0.4.0/minari/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:34:21.716521 minari-0.4.0/minari/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-19 13:34:05.000000 minari-0.4.0/minari/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-19 13:34:05.000000 minari-0.4.0/minari/storage/datasets_root_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-07-19 13:34:05.000000 minari-0.4.0/minari/storage/hosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-19 13:34:05.000000 minari-0.4.0/minari/storage/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32015 2023-07-19 13:34:05.000000 minari-0.4.0/minari/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:34:21.716521 minari-0.4.0/minari.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-19 13:34:21.000000 minari-0.4.0/minari.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-19 13:34:21.000000 minari-0.4.0/minari.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 13:34:21.000000 minari-0.4.0/minari.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-19 13:34:21.000000 minari-0.4.0/minari.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-19 13:34:21.000000 minari-0.4.0/minari.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-19 13:34:21.000000 minari-0.4.0/minari.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-19 13:34:05.000000 minari-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 13:34:21.716521 minari-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-19 13:34:05.000000 minari-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:34:21.716521 minari-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-19 13:34:05.000000 minari-0.4.0/tests/test_serialization.py
```

### Comparing `minari-0.3.1/LICENSE` & `minari-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `minari-0.3.1/PKG-INFO` & `minari-0.4.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,28 @@
-Metadata-Version: 2.1
-Name: minari
-Version: 0.3.1
-Summary: A standard format for offline reinforcement learning datasets, with popular reference datasets and related utilities.
-Author-email: Farama Foundation <contact@farama.org>
-License: MIT License
-Project-URL: Homepage, https://farama.org
-Project-URL: Repository, https://github.com/Farama-Foundation/Minari
-Project-URL: Documentation, https://minari.farama.org/
-Project-URL: Bug Report, https://github.com/Farama-Foundation/Minari/issues
-Keywords: Reinforcement Learning,Offline RL,RL,AI,gymnasium,Farama
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-License-File: LICENSE
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) 
+
 
 <p align="center">
     <img src="minari-text.png" width="500px"/>
 </p>
 
 Minari is a Python library for conducting research in offline reinforcement learning, akin to an offline version of Gymnasium or an offline RL version of HuggingFace's datasets library. This library is currently in beta.
 
 The documentation website is at [minari.farama.org](https://minari.farama.org/main/). We also have a public discord server (which we use for Q&A and to coordinate development work) that you can join here: https://discord.gg/bnJ6kubTg6.
 
 Note: Minari was previously developed under the name Kabuki.
 
 
 ## Installation
+To install Minari from [PyPI](https://pypi.org/project/minari/):
+```
+pip install minari
+```
 
-Currently the beta release is under development. If you'd like to start testing or contribute to Minari please install this project from source with: 
+Note that currently Minari is under a beta release. If you'd like to start testing or contribute to Minari please install this project from source with: 
 
 ```bash
 git clone https://github.com/Farama-Foundation/Minari.git
 cd Minari
 pip install -e .
 ```
 
@@ -68,18 +49,26 @@
 ```
 
 To download a dataset:
 
 ```python
 import minari
 
-dataset = minari.download_dataset("LunarLander_v2_remote-test-dataset")
+minari.download_dataset("door-cloned-v1")
+```
+
+To load a dataset:
+
+```python
+import minari
+
+dataset = minari.load_dataset("door-cloned-v1")
 ```
 
 ## Project Maintainers
-Main Contributors: [Rodrigo Perez-Vicente](https://github.com/rodrigodelazcano), [Omar Younis](https://github.com/younik)
+Main Contributors: [Rodrigo Perez-Vicente](https://github.com/rodrigodelazcano), [Omar Younis](https://github.com/younik), [John Balis](https://github.com/balisujohn)
 
 Maintenance for this project is also contributed by the broader Farama team: [farama.org/team](https://farama.org/team).
 
 ___
 
 _Minari is a shortening of Minarai, the Japanese word for "learning by observation"._
```

### Comparing `minari-0.3.1/minari/__init__.py` & `minari-0.4.0/minari/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     upload_dataset,
 )
 from minari.storage.local import delete_dataset, list_local_datasets, load_dataset
 from minari.utils import (
     combine_datasets,
     create_dataset_from_buffers,
     create_dataset_from_collector_env,
+    get_normalized_score,
     split_dataset,
 )
 
 
 __all__ = [
     # Minari Dataset
     "MinariDataset",
@@ -30,10 +31,11 @@
     "delete_dataset",
     "list_local_datasets",
     "load_dataset",
     "combine_datasets",
     "create_dataset_from_buffers",
     "create_dataset_from_collector_env",
     "split_dataset",
+    "get_normalized_score",
 ]
 
-__version__ = "0.3.1"
+__version__ = "0.4.0"
```

### Comparing `minari-0.3.1/minari/cli.py` & `minari-0.4.0/minari/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Minari CLI commands."""
+import os
 from typing import List, Optional
+from typing_extensions import Annotated
 
 import typer
 from rich import print
 from rich.table import Table
 from rich.tree import Tree
 
 from minari import __version__
@@ -47,45 +49,68 @@
         )
 
     print(table)
 
 
 @app.callback()
 def common(
-    version: Optional[bool] = typer.Option(
-        None,
-        "--version",
-        "-v",
-        callback=_version_callback,
-        help="Show installed Minari version.",
-    )
+    version: Annotated[
+        Optional[bool],
+        typer.Option(
+            "--version",
+            "-v",
+            callback=_version_callback,
+            help="Show installed Minari version.",
+        ),
+    ] = None,
 ):
     """Minari is a tool for collecting and hosting Offline datasets for Reinforcement Learning environments based on the Gymnaisum API."""
     pass
 
 
 @list_app.command("remote")
-def list_remote():
+def list_remote(
+    all: Annotated[
+        bool, typer.Option("--all", "-a", help="Show all dataset versions.")
+    ] = False
+):
     """List Minari datasets hosted in the Farama server."""
-    datasets = hosting.list_remote_datasets()
+    if all:
+        datasets = hosting.list_remote_datasets()
+    else:
+        datasets = hosting.list_remote_datasets(
+            latest_version=True, compatible_minari_version=True
+        )
     table_title = "Minari datasets in Farama server"
     _show_dataset_table(datasets, table_title)
 
 
 @list_app.command("local")
-def list_local():
+def list_local(
+    all: Annotated[
+        bool, typer.Option("--all", "-a", help="Show all dataset versions.")
+    ] = False
+):
     """List local Minari datasets."""
-    datasets = local.list_local_datasets()
-    dataset_dir = "home/rodrigo/.minari/"
+    if all:
+        datasets = local.list_local_datasets()
+    else:
+        datasets = local.list_local_datasets(
+            latest_version=True, compatible_minari_version=True
+        )
+    dataset_dir = os.environ.get(
+        "MINARI_DATASETS_PATH",
+        os.path.join(os.path.expanduser("~"), ".minari/datasets/"),
+    )
     table_title = f"Local Minari datasets('{dataset_dir}')"
     _show_dataset_table(datasets, table_title)
 
 
 @app.command()
-def delete(datasets: List[str]):
+def delete(datasets: Annotated[List[str], typer.Argument()]):
     """Delete datasets from local database."""
     # check that the given local datasets exist
     local_dsts = local.list_local_datasets()
     non_matching_local = [dst for dst in datasets if dst not in local_dsts]
     if len(non_matching_local) > 0:
         local_dataset_path = get_dataset_path("")
         tree = Tree(
@@ -107,18 +132,24 @@
     typer.confirm("Are you sure you want to delete these local datasets?", abort=True)
 
     for dst in datasets:
         local.delete_dataset(dst)
 
 
 @app.command()
-def download(datasets: List[str]):
+def download(
+    datasets: Annotated[List[str], typer.Argument()],
+    force: Annotated[
+        bool, typer.Option("--force", "-f", help="Perform a force download.")
+    ] = False,
+):
     """Download Minari datasets from Farama server."""
     # check if datasets exist in remote server
     remote_dsts = hosting.list_remote_datasets()
+
     non_matching_remote = [dst for dst in datasets if dst not in remote_dsts]
     if len(non_matching_remote) > 0:
         tree = Tree(
             "The following datasets can't be found in the remote Farama server",
             style="red",
         )
         for dst in non_matching_remote:
@@ -130,28 +161,31 @@
     local_dsts = local.list_local_datasets()
     datasets_to_override = {
         local_name: local_dsts[local_name]
         for local_name in local_dsts.keys()
         if local_name in datasets
     }
 
-    if len(datasets_to_override) > 0:
+    if len(datasets_to_override) > 0 and not force:
         _show_dataset_table(datasets_to_override, "Download remote Minari datasets")
         typer.confirm(
             "Are you sure you want to download and override these local datasets?",
             abort=True,
         )
 
     # download datastets
     for dst in datasets:
-        hosting.download_dataset(dst)
+        hosting.download_dataset(dst, force_download=force)
 
 
 @app.command()
-def upload(datasets: List[str], key_path: str = typer.Option(...)):
+def upload(
+    datasets: Annotated[List[str], typer.Argument()],
+    key_path: Annotated[str, typer.Option()],
+):
     """Upload Minari datasets to the remote Farama server."""
     local_dsts = local.list_local_datasets()
     remote_dsts = hosting.list_remote_datasets()
 
     # check that the given local datasets exist
     non_matching_local = [dst for dst in datasets if dst not in local_dsts]
     if len(non_matching_local) > 0:
@@ -180,15 +214,18 @@
 
     # Upload datasets
     for dst in datasets:
         hosting.upload_dataset(dst, key_path)
 
 
 @app.command()
-def combine(datasets: List[str], dataset_id: str = typer.Option(...)):
+def combine(
+    datasets: Annotated[List[str], typer.Argument()],
+    dataset_id: Annotated[str, typer.Option()],
+):
     """Combine multiple datasets into a single Minari dataset."""
     local_dsts = local.list_local_datasets()
     # check dataset name doesn't exist locally
     if dataset_id in local_dsts:
         print(
             f"[red]Dataset name {dataset_id} already exist in the local Minari datasets.[/red]",
         )
```

### Comparing `minari-0.3.1/minari/data_collector/callbacks/episode_metadata.py` & `minari-0.4.0/minari/data_collector/callbacks/episode_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
         """
         eps_group["rewards"].attrs["sum"] = np.sum(eps_group["rewards"])
         eps_group["rewards"].attrs["mean"] = np.mean(eps_group["rewards"])
         eps_group["rewards"].attrs["std"] = np.std(eps_group["rewards"])
         eps_group["rewards"].attrs["max"] = np.max(eps_group["rewards"])
         eps_group["rewards"].attrs["min"] = np.min(eps_group["rewards"])
 
-        eps_group.attrs["total_steps"] = eps_group["actions"].shape[0]
+        eps_group.attrs["total_steps"] = eps_group["rewards"].shape[0]
```

### Comparing `minari-0.3.1/minari/data_collector/data_collector.py` & `minari-0.4.0/minari/data_collector/data_collector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from __future__ import annotations
 
 import os
 import shutil
 import tempfile
-from typing import Any, Dict, List, Optional, SupportsFloat, Type, TypeVar, Union
+from collections import OrderedDict
+from typing import Any, Dict, List, Optional, SupportsFloat, Type, Union
 
 import gymnasium as gym
 import h5py
 import numpy as np
 from gymnasium.core import ActType, ObsType
 
 from minari.data_collector.callbacks import (
     STEP_DATA_KEYS,
     EpisodeMetadataCallback,
     StepData,
     StepDataCallback,
 )
+from minari.serialization import serialize_space
 
 
-EpisodeBufferValues = TypeVar("EpisodeBufferValues", List[Any], "EpisodeBuffer")
-EpisodeBuffer = Dict[str, EpisodeBufferValues]
+EpisodeBuffer = Dict[str, Any]  # TODO: narrow this down
 
 
 class DataCollectorV0(gym.Wrapper):
     r"""Gymnasium environment wrapper that collects step data.
 
     This wrapper is meant to work as a temporary buffer of the environment data before creating a Minari dataset. The creation of the buffers
     that will be convert to a Minari dataset is agnostic to the user:
@@ -68,42 +69,52 @@
         step_data_callback: Type[StepDataCallback] = StepDataCallback,
         episode_metadata_callback: Type[
             EpisodeMetadataCallback
         ] = EpisodeMetadataCallback,
         record_infos: bool = False,
         max_buffer_steps: Optional[int] = None,
         max_buffer_episodes: Optional[int] = None,
+        observation_space=None,
+        action_space=None,
     ):
         """Initialize the data colletor attributes and create the temporary directory for caching.
 
         Args:
             env (gym.Env): Gymnasium environment
             step_data_callback (type[StepDataCallback], optional): Callback class to edit/update step databefore storing to buffer. Defaults to StepDataCallback.
             episode_metadata_callback (type[EpisodeMetadataCallback], optional): Callback class to add custom metadata to episode group in HDF5 file. Defaults to EpisodeMetadataCallback.
             record_infos (bool, optional): If True record the info return key of each step. Defaults to False.
             max_buffer_steps (Optional[int], optional): number of steps saved in-memory buffers before dumping to HDF5 file in disk. Defaults to None.
             max_buffer_episodes (Optional[int], optional): number of episodes saved in-memory buffers before dumping to HDF5 file in disk. Defaults to None.
 
         Raises:
             ValueError: `max_buffer_steps` and `max_buffer_episodes` can't be passed at the same time
         """
-        self.env = env
-        self._step_data_callback = step_data_callback(env)
+        super().__init__(env)
+        self._step_data_callback = step_data_callback()
+
+        if observation_space is None:
+            observation_space = self.env.observation_space
+        self.dataset_observation_space = observation_space
+
+        if action_space is None:
+            action_space = self.env.action_space
+        self.dataset_action_space = action_space
 
         self._episode_metadata_callback = episode_metadata_callback()
         self._record_infos = record_infos
 
         if max_buffer_steps is not None and max_buffer_episodes is not None:
             raise ValueError("Choose step or episode scheduler not both")
 
         self.max_buffer_episodes = max_buffer_episodes
         self.max_buffer_steps = max_buffer_steps
 
         # Initialzie empty buffer
-        self._buffer: List[EpisodeBuffer] = [{key: [] for key in STEP_DATA_KEYS}]
+        self._buffer: List[EpisodeBuffer] = [{}]
 
         self._current_seed: Union[int, str] = str(None)
         self._new_episode = False
 
         self._step_id = 0
 
         # get path to minari datasets directory
@@ -117,22 +128,19 @@
             os.makedirs(self.datasets_path)
 
         self._tmp_dir = tempfile.TemporaryDirectory(dir=self.datasets_path)
         self._tmp_f = h5py.File(
             os.path.join(self._tmp_dir.name, "tmp_dataset.hdf5"), "a", track_order=True
         )  # track insertion order of groups ('episodes_i')
 
-        assert self.env.spec is not None
+        assert self.env.spec is not None, "Env Spec is None"
         self._tmp_f.attrs["env_spec"] = self.env.spec.to_json()
-        self._tmp_f.attrs[
-            "flatten_observation"
-        ] = self._step_data_callback.flatten_observation
-        self._tmp_f.attrs["flatten_action"] = self._step_data_callback.flatten_action
 
         self._new_episode = False
+        self._reset_called = False
 
         # Initialize first episode group in temporary hdf5 file
         self._episode_id = 0
         self._eps_group: h5py.Group = self._tmp_f.create_group("episode_0")
         self._eps_group.attrs["id"] = 0
 
         self._last_episode_group_term_or_trunc = False
@@ -142,15 +150,15 @@
         self,
         episode_buffer: EpisodeBuffer,
         step_data: Union[StepData, Dict[str, StepData]],
     ) -> EpisodeBuffer:
         """Add step data dictionary to episode buffer.
 
         Args:
-            buffer (Dict): dictionary episode buffer
+            episode_buffer (Dict): dictionary episode buffer
             step_data (Dict): dictionary with data for a single step
 
         Returns:
             Dict: new dictionary episode buffer with added values from step_data
         """
         for key, value in step_data.items():
             if (not self._record_infos and key == "infos") or (value is None):
@@ -161,19 +169,25 @@
             if key not in episode_buffer:
                 if isinstance(value, dict):
                     episode_buffer[key] = self._add_to_episode_buffer({}, value)
                 else:
                     episode_buffer[key] = [value]
             else:
                 if isinstance(value, dict):
-                    assert isinstance(episode_buffer[key], dict)
+                    assert isinstance(
+                        episode_buffer[key], dict
+                    ), f"Element to be inserted is type 'dict', but buffer accepts type {type(episode_buffer[key])}"
+
                     episode_buffer[key] = self._add_to_episode_buffer(
                         episode_buffer[key], value
                     )
                 else:
+                    assert isinstance(
+                        episode_buffer[key], list
+                    ), f"Element to be inserted is type 'list', but buffer accepts type {type(episode_buffer[key])}"
                     episode_buffer[key].append(value)
 
         return episode_buffer
 
     def step(
         self, action: ActType
     ) -> tuple[ObsType, SupportsFloat, bool, bool, dict[str, Any]]:
@@ -186,93 +200,114 @@
             obs=obs,
             info=info,
             action=action,
             rew=rew,
             terminated=terminated,
             truncated=truncated,
         )
-
-        # force step data dicitonary to include keys corresponding to Gymnasium step returns:
-        # actions, observations, rewards, terminations, truncatins, and infos
-        assert STEP_DATA_KEYS.issubset(step_data.keys())
+        # Force step data dictionary to include keys corresponding to Gymnasium step returns:
+        # actions, observations, rewards, terminations, truncations, and infos
+        assert STEP_DATA_KEYS.issubset(
+            step_data.keys()
+        ), "One or more required keys is missing from 'step-data'."
+        # Check that the saved observation and action belong to the dataset's observation/action spaces
+        assert self.dataset_observation_space.contains(
+            step_data["observations"]
+        ), "Observations are not in observation space."
+        assert self.dataset_action_space.contains(
+            step_data["actions"]
+        ), "Actions are not in action space."
 
         self._step_id += 1
 
         clear_buffers = False
         # check if buffer needs to be cleared to temp file due to maximum step scheduler
         if self.max_buffer_steps is not None:
             clear_buffers = (
                 self._step_id % self.max_buffer_steps == 0 and self._step_id != 0
             )
 
-        # Get initial observation from previous episode if reset has not been called after termination or truncation
-        # This may happen if the step_data_callback truncates or terminates the episode under certain conditions.
+        # Get initial observation/info from previous episode if reset has not been called after termination
+        # or truncation. This may happen if the step_data_callback truncates or terminates the episode under
+        # certain conditions.
         if self._new_episode and not self._reset_called:
-            self._buffer[-1]["observations"] = [self._previous_eps_final_obs]
+            if isinstance(self._previous_eps_final_obs, dict):
+                self._buffer[-1]["observations"] = self._add_to_episode_buffer(
+                    {}, self._previous_eps_final_obs
+                )
+            else:
+                self._buffer[-1]["observations"] = [self._previous_eps_final_obs]
+            if self._record_infos:
+                self._buffer[-1]["infos"] = self._add_to_episode_buffer(
+                    {}, self._previous_eps_final_info
+                )
+
             self._new_episode = False
 
         # add step data to last episode buffer
         self._buffer[-1] = self._add_to_episode_buffer(self._buffer[-1], step_data)
 
         if step_data["terminations"] or step_data["truncations"]:
+            # Save last observation/info to use as initial observation/info in the next episode
             self._previous_eps_final_obs = step_data["observations"]
+            if self._record_infos:
+                self._previous_eps_final_info = step_data["infos"]
             self._reset_called = False
             self._new_episode = True
-            self._buffer[-1]["seed"] = self._current_seed
+            self._buffer[-1]["seed"] = self._current_seed  # type: ignore
             # Only check episode scheduler to save in-memory data to temp HDF5 file when episode is done
             if self.max_buffer_episodes is not None:
                 clear_buffers = (self._episode_id + 1) % self.max_buffer_episodes == 0
 
         if clear_buffers:
             self.clear_buffer_to_tmp_file()
 
-        # add new episode buffer to global buffer when episode finishes with truncation or termination
         if clear_buffers or step_data["terminations"] or step_data["truncations"]:
-            self._buffer.append({key: [] for key in STEP_DATA_KEYS})
+            self._buffer.append({})
 
-        # Increase episode count when step is term/trunc and only after clearing buffers to tmp file
         if step_data["terminations"] or step_data["truncations"]:
-            # New episode
             self._episode_id += 1
 
         return obs, rew, terminated, truncated, info
 
     def reset(
         self,
         *,
         seed: int | None = None,
         options: dict[str, Any] | None = None,
     ) -> tuple[ObsType, dict[str, Any]]:
         """Gymnasium environment reset."""
         obs, info = self.env.reset(seed=seed, options=options)
         step_data = self._step_data_callback(env=self, obs=obs, info=info)
 
-        assert STEP_DATA_KEYS.issubset(step_data.keys())
+        assert STEP_DATA_KEYS.issubset(
+            step_data.keys()
+        ), "One or more required keys is missing from 'step-data'"
 
         # If last episode in global buffer has saved steps, we need to check if it was truncated or terminated
-        # If not, then we need to auto-truncate the episode
-        if len(self._buffer[-1]["actions"]) > 0:
+        # If the last element in the buffer is not an empty dictionary, then we need to auto-truncate the episode.
+        if self._buffer[-1]:
             if (
                 not self._buffer[-1]["terminations"][-1]
                 and not self._buffer[-1]["truncations"][-1]
             ):
                 self._buffer[-1]["truncations"][-1] = True
-                self._buffer[-1]["seed"] = self._current_seed
+                self._buffer[-1]["seed"] = self._current_seed  # type: ignore
 
                 # New episode
                 self._episode_id += 1
 
                 if (
                     self.max_buffer_episodes is not None
                     and self._episode_id % self.max_buffer_episodes == 0
                 ):
                     self.clear_buffer_to_tmp_file()
 
                 # add new episode buffer
-                self._buffer.append({key: [] for key in STEP_DATA_KEYS})
+                self._buffer.append({})
         else:
             # In the case that the past episode is already stored in the tmp hdf5 file because of caching,
             # we need to check if it was truncated or terminated, if not then auto-truncate
             if (
                 len(self._buffer) == 1
                 and not self._last_episode_group_term_or_trunc
                 and self._episode_id != 0
@@ -301,71 +336,94 @@
     def clear_buffer_to_tmp_file(self, truncate_last_episode: bool = False):
         """Save the global buffer in-memory to a temporary HDF5 file in disk.
 
         Args:
             truncate_last_episode (bool, optional): If True the last episode from the buffer will be truncated before saving to disk. Defaults to False.
         """
 
+        def get_h5py_subgroup(group: h5py.Group, name: str) -> h5py.Group:
+            """Get a subgroup from an h5py group.
+
+            If the subgroup does not exist, create and return and empty group with the given name.
+
+            Args:
+                group (h5py.Group): the h5py group object to look for/create the subgroup.
+                name (str): name of the subgroup.
+
+            Returns:
+                subgroup (h5py.Group)
+            """
+            if name in group:
+                subgroup = group.get(name)
+                assert isinstance(subgroup, h5py.Group)
+            else:
+                subgroup = group.create_group(name)
+
+            return subgroup
+
         def clear_buffer(dictionary_buffer: EpisodeBuffer, episode_group: h5py.Group):
             """Inner function to recursively save the nested data dictionaries in an episode buffer.
 
             Args:
                 dictionary_buffer (EpisodeBuffer): ditionary with keys to store as independent HDF5 datasets if the value is a list buffer
                 or create another group if value is a dictionary.
                 episode_group (h5py.Group): HDF5 group to store the datasets from the dictionary_buffer.
             """
             for key, data in dictionary_buffer.items():
                 if isinstance(data, dict):
-                    if key in episode_group:
-                        eps_group_to_clear = episode_group[key]
-                    else:
-                        eps_group_to_clear = episode_group.create_group(key)
+                    eps_group_to_clear = get_h5py_subgroup(episode_group, key)
                     clear_buffer(data, eps_group_to_clear)
+                elif all(map(lambda elem: isinstance(elem, tuple), data)):
+                    # we have a list of tuples, so we need to act appropriately
+                    dict_data = {
+                        f"_index_{str(i)}": [entry[i] for entry in data]
+                        for i, _ in enumerate(data[0])
+                    }
+                    eps_group_to_clear = get_h5py_subgroup(episode_group, key)
+                    clear_buffer(dict_data, eps_group_to_clear)
+                elif all(map(lambda elem: isinstance(elem, OrderedDict), data)):
+                    # we have a list of OrderedDicts, so we need to act appropriately
+                    dict_data = {
+                        key: [entry[key] for entry in data]
+                        for key, value in data[0].items()
+                    }
+                    eps_group_to_clear = get_h5py_subgroup(episode_group, key)
+                    clear_buffer(dict_data, eps_group_to_clear)
                 else:
-                    # convert data to numpy
-                    np_data = np.asarray(data)
-                    assert np.all(np.logical_not(np.isnan(np_data)))
+                    if all(map(lambda elem: isinstance(elem, str), data)):
+                        data_shape = (len(data),)
+                        dtype = h5py.string_dtype(encoding="utf-8")
+                    else:
+                        data = np.asarray(data)
+                        data_shape = data.shape
+                        dtype = data.dtype
+                        assert np.all(
+                            np.logical_not(np.isnan(data))
+                        ), "Nan found after cast to nump array, check the type of 'data'."
 
-                    # Check if last episode group is terminated or truncated
                     if (
                         not self._last_episode_group_term_or_trunc
                         and key in episode_group
                     ):
-                        # Append to last episode group datasets
-                        if key not in STEP_DATA_KEYS and key != "infos":
-                            # check current dataset size directly from hdf5 since
-                            # non step data (actions, obs, rew, term, trunc) may not be
-                            # added in a per-step/sequential basis, including "infos"
-                            current_dataset_shape = episode_group[key].shape[0]
-                        else:
-                            current_dataset_shape = self._last_episode_n_steps
-                            if key == "observations":
-                                current_dataset_shape += (
-                                    1  # include initial observation
-                                )
+                        current_dataset_shape = episode_group[key].shape[0]
                         episode_group[key].resize(
                             current_dataset_shape + len(data), axis=0
                         )
-                        episode_group[key][-len(data) :] = np_data
+                        episode_group[key][-len(data) :] = data
                     else:
                         if not current_episode_group_term_or_trunc:
-                            # Create resizable datasets
-                            episode_group.create_dataset(
-                                key,
-                                data=np_data,
-                                maxshape=(None,) + np_data.shape[1:],
-                                chunks=True,
-                            )
-                        else:
-                            # Dump everything to episode group
-                            episode_group.create_dataset(key, data=np_data, chunks=True)
+                            data_shape = (None,) + data_shape[1:]  # resizable dataset
+
+                        episode_group.create_dataset(
+                            key, data=data, maxshape=data_shape, dtype=dtype
+                        )
 
         for i, eps_buff in enumerate(self._buffer):
-            if len(eps_buff["actions"]) == 0:
-                # Make sure that the episode has stepped
+            # Make sure that the episode has stepped, by checking if the 'actions' key has been added to the episode buffer.
+            if "actions" not in eps_buff:
                 continue
 
             current_episode_group_term_or_trunc = (
                 eps_buff["terminations"][-1] or eps_buff["truncations"][-1]
             )
 
             # Check if last episode group is terminated or truncated
@@ -404,28 +462,46 @@
 
             # Compute metadata, use episode dataset in hdf5 file
             self._episode_metadata_callback(self._eps_group)
 
         # Clear in-memory buffers
         self._buffer.clear()
 
-    def save_to_disk(self, path: str, dataset_metadata: Dict = {}):
+    def save_to_disk(
+        self, path: str, dataset_metadata: Optional[Dict[str, Any]] = None
+    ):
         """Save all in-memory buffer data and move temporary HDF5 file to a permanent location in disk.
 
         Args:
             path (str): path to store permanent HDF5, i.e: '/home/foo/datasets/data.hdf5'
             dataset_metadata (Dict, optional): additional metadata to add to HDF5 dataset file as attributes. Defaults to {}.
         """
+        if dataset_metadata is None:
+            dataset_metadata = {}
+
         # Dump everything in memory buffers to tmp_dataset.hdf5 and truncate last episode
         self.clear_buffer_to_tmp_file(truncate_last_episode=True)
 
         for key, value in dataset_metadata.items():
             self._tmp_f.attrs[key] = value
 
-        self._buffer.append({key: [] for key in STEP_DATA_KEYS})
+        assert (
+            "observation_space" not in dataset_metadata.keys()
+        ), "'observation_space' is not allowed as an optional key."
+        assert (
+            "action_space" not in dataset_metadata.keys()
+        ), "'action_space' is not allowed as an optional key."
+
+        action_space_str = serialize_space(self.dataset_action_space)
+        observation_space_str = serialize_space(self.dataset_observation_space)
+
+        self._tmp_f.attrs["action_space"] = action_space_str
+        self._tmp_f.attrs["observation_space"] = observation_space_str
+
+        self._buffer.append({})
 
         # Reset episode count
         self._episode_id = 0
 
         self._tmp_f.attrs["total_episodes"] = len(self._tmp_f.keys())
         self._tmp_f.attrs["total_steps"] = sum(
             [
```

### Comparing `minari-0.3.1/minari/dataset/minari_dataset.py` & `minari-0.4.0/minari/dataset/minari_dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from __future__ import annotations
 
 import os
 import re
 from dataclasses import dataclass, field
-from typing import Callable, Dict, Iterable, Iterator, List, NamedTuple, Optional, Union
+from typing import Callable, Iterable, Iterator, List, Optional, Union
 
 import gymnasium as gym
-import h5py
 import numpy as np
 from gymnasium import error
 from gymnasium.envs.registration import EnvSpec
 
 from minari.data_collector import DataCollectorV0
 from minari.dataset.minari_storage import MinariStorage, PathLike
 
 
 DATASET_ID_RE = re.compile(
     r"(?:(?P<environment>[\w]+?))?(?:-(?P<dataset>[\w:.-]+?))(?:-v(?P<version>\d+))?$"
 )
 
 
-def parse_dataset_id(dataset_id: str) -> tuple[str | None, str, int | None]:
+def parse_dataset_id(dataset_id: str) -> tuple[str | None, str, int]:
     """Parse dataset ID string format - ``(env_name-)(dataset_name)(-v(version))``.
 
     Args:
         dataset_id: The dataset id to parse
     Returns:
         A tuple of environment name, dataset name and version number
     Raises:
@@ -32,74 +31,79 @@
     """
     match = DATASET_ID_RE.fullmatch(dataset_id)
     if not match:
         raise error.Error(
             f"Malformed dataset ID: {dataset_id}. (Currently all IDs must be of the form (env_name-)(dataset_name)-v(version). (namespace is optional))"
         )
     env_name, dataset_name, version = match.group("environment", "dataset", "version")
-    if version is not None:
-        version = int(version)
 
-    return env_name, dataset_name, version
-
-
-def clear_episode_buffer(episode_buffer: Dict, eps_group: h5py.Group) -> h5py.Group:
-    """Save an episode dictionary buffer into an HDF5 episode group recursively.
+    version = int(version)
 
-    Args:
-        episode_buffer (dict): episode buffer
-        eps_group (h5py.Group): HDF5 group to store the episode datasets
-
-    Returns:
-        episode group: filled HDF5 episode group
-    """
-    for key, data in episode_buffer.items():
-        if isinstance(data, dict):
-            if key in eps_group:
-                eps_group_to_clear = eps_group[key]
-            else:
-                eps_group_to_clear = eps_group.create_group(key)
-            clear_episode_buffer(data, eps_group_to_clear)
-        else:
-            # assert data is numpy array
-            assert np.all(np.logical_not(np.isnan(data)))
-            # add seed to attributes
-            eps_group.create_dataset(key, data=data, chunks=True)
-
-    return eps_group
+    return env_name, dataset_name, version
 
 
-class EpisodeData(NamedTuple):
+@dataclass(frozen=True)
+class EpisodeData:
     """Contains the datasets data for a single episode.
 
     This is the object returned by :class:`minari.MinariDataset.sample_episodes`.
     """
 
     id: int
     seed: Optional[int]
     total_timesteps: int
     observations: np.ndarray
     actions: np.ndarray
     rewards: np.ndarray
     terminations: np.ndarray
     truncations: np.ndarray
 
+    def __repr__(self) -> str:
+        return (
+            "EpisodeData("
+            f"id={repr(self.id)}, "
+            f"seed={repr(self.seed)}, "
+            f"total_timesteps={self.total_timesteps}, "
+            f"observations={EpisodeData._repr_space_values(self.observations)}, "
+            f"actions={EpisodeData._repr_space_values(self.actions)}, "
+            f"rewards=ndarray of {len(self.rewards)} floats, "
+            f"terminations=ndarray of {len(self.terminations)} bools, "
+            f"truncations=ndarray of {len(self.truncations)} bools"
+            ")"
+        )
+
+    @staticmethod
+    def _repr_space_values(value):
+        if isinstance(value, np.ndarray):
+            return f"ndarray of shape {value.shape} and dtype {value.dtype}"
+        elif isinstance(value, dict):
+            reprs = [
+                f"{k}: {EpisodeData._repr_space_values(v)}" for k, v in value.items()
+            ]
+            dict_repr = ", ".join(reprs)
+            return "{" + dict_repr + "}"
+        elif isinstance(value, tuple):
+            reprs = [EpisodeData._repr_space_values(v) for v in value]
+            values_repr = ", ".join(reprs)
+            return "(" + values_repr + ")"
+        else:
+            return repr(value)
+
 
 @dataclass
 class MinariDatasetSpec:
-    flatten_observations: bool
-    flatten_actions: bool
     env_spec: EnvSpec
     total_episodes: int
     total_steps: int
     dataset_id: str
     combined_datasets: List[str]
     observation_space: gym.Space
     action_space: gym.Space
     data_path: str
+    minari_version: str
 
     # post-init attributes
     env_name: str | None = field(init=False)
     dataset_name: str = field(init=False)
     version: int | None = field(init=False)
 
     def __post_init__(self):
@@ -133,107 +137,118 @@
             self._data = MinariStorage(data)
         else:
             raise ValueError(f"Unrecognized type {type(data)} for data")
 
         self._additional_data_id = 0
         if episode_indices is None:
             episode_indices = np.arange(self._data.total_episodes)
+
         self._episode_indices = episode_indices
 
+        assert self._episode_indices is not None
+
+        total_steps = sum(
+            self._data.apply(
+                lambda episode: episode["total_timesteps"],
+                episode_indices=self._episode_indices,
+            )
+        )
+
         self.spec = MinariDatasetSpec(
-            flatten_observations=self._data.flatten_observations,
-            flatten_actions=self._data.flatten_actions,
             env_spec=self._data.env_spec,
-            total_episodes=self._data.total_episodes,
-            total_steps=self._data.total_steps,
+            total_episodes=self._episode_indices.size,
+            total_steps=total_steps,
             dataset_id=self._data.id,
             combined_datasets=self._data.combined_datasets,
             observation_space=self._data.observation_space,
             action_space=self._data.action_space,
             data_path=str(self._data.data_path),
+            minari_version=str(self._data.minari_version),
         )
-        self._total_steps = None
+        self._total_steps = total_steps
         self._generator = np.random.default_rng()
 
     @property
     def total_episodes(self):
         """Total episodes recorded in the Minari dataset."""
         assert self._episode_indices is not None
-        return len(self._episode_indices)
+        return self._episode_indices.size
 
     @property
     def total_steps(self):
         """Total episodes steps in the Minari dataset."""
-        if self._total_steps is None:
-            t_steps = self._data.apply(
-                lambda episode: episode["total_steps"],
-                episode_indices=self._episode_indices,
-            )
-            self._total_steps = sum(t_steps)
         return self._total_steps
 
     @property
-    def episode_indices(self):
+    def episode_indices(self) -> np.ndarray:
         """Indices of the available episodes to sample within the Minari dataset."""
         return self._episode_indices
 
-    def recover_environment(self):
+    def recover_environment(self) -> gym.Env:
         """Recover the Gymnasium environment used to create the dataset.
 
         Returns:
             environment: Gymnasium environment
         """
         return gym.make(self._data.env_spec)
 
     def set_seed(self, seed: int):
         """Set seed for random episode sampling generator."""
         self._generator = np.random.default_rng(seed)
 
-    def filter_episodes(self, condition: Callable[[h5py.Group], bool]) -> MinariDataset:
+    def filter_episodes(
+        self, condition: Callable[[EpisodeData], bool]
+    ) -> MinariDataset:
         """Filter the dataset episodes with a condition.
 
-        The condition must be a callable with  a single argument, the episode HDF5 group.
+        The condition must be a callable which takes an `EpisodeData` instance and retutrns a bool.
         The callable must return a `bool` True if the condition is met and False otherwise.
         i.e filtering for episodes that terminate:
 
         ```
         dataset.filter(condition=lambda x: x['terminations'][-1] )
         ```
 
         Args:
-            condition (Callable[[h5py.Group], bool]): callable that accepts an episode group and returns True if certain condition is met.
+            condition (Callable[[EpisodeData], bool]): callable that accepts any type(For our current backend, an h5py episode group) and returns True if certain condition is met.
         """
-        mask = self._data.apply(condition, episode_indices=self._episode_indices)
+
+        def dict_to_episode_data_condition(episode: dict) -> bool:
+            return condition(EpisodeData(**episode))
+
+        mask = self._data.apply(
+            dict_to_episode_data_condition, episode_indices=self._episode_indices
+        )
         assert self._episode_indices is not None
         return MinariDataset(self._data, episode_indices=self._episode_indices[mask])
 
     def sample_episodes(self, n_episodes: int) -> Iterable[EpisodeData]:
         """Sample n number of episodes from the dataset.
 
         Args:
             n_episodes (Optional[int], optional): number of episodes to sample.
         """
         indices = self._generator.choice(
-            self._episode_indices, size=n_episodes, replace=False
+            self.episode_indices, size=n_episodes, replace=False
         )
         episodes = self._data.get_episodes(indices)
         return list(map(lambda data: EpisodeData(**data), episodes))
 
     def iterate_episodes(
         self, episode_indices: Optional[List[int]] = None
     ) -> Iterator[EpisodeData]:
         """Iterate over episodes from the dataset.
 
         Args:
             episode_indices (Optional[List[int]], optional): episode indices to iterate over.
         """
         if episode_indices is None:
-            assert self._episode_indices is not None
-            assert self._episode_indices.ndim == 1
-            episode_indices = self._episode_indices.tolist()
+            assert self.episode_indices is not None
+            assert self.episode_indices.ndim == 1
+            episode_indices = self.episode_indices.tolist()
 
         assert episode_indices is not None
 
         for episode_index in episode_indices:
             data = self._data.get_episodes([episode_index])[0]
             yield EpisodeData(**data)
 
@@ -250,39 +265,36 @@
         """
         # check that collector env has the same characteristics as self._env_spec
         new_data_file_path = os.path.join(
             os.path.split(self.spec.data_path)[0],
             f"additional_data_{self._additional_data_id}.hdf5",
         )
 
-        collector_env.save_to_disk(path=new_data_file_path)
+        old_total_episodes = self._data.total_episodes
+
+        self._data.update_from_collector_env(
+            collector_env, new_data_file_path, self._additional_data_id
+        )
+
+        new_total_episodes = self._data._total_episodes
 
-        with h5py.File(new_data_file_path, "r", track_order=True) as new_data_file:
-            new_data_total_episodes = new_data_file.attrs["total_episodes"]
-            new_data_total_steps = new_data_file.attrs["total_steps"]
-
-        with h5py.File(self._data.data_path, "a", track_order=True) as file:
-            last_episode_id = file.attrs["total_episodes"]
-            for id in range(new_data_total_episodes):
-                file[f"episode_{last_episode_id + id}"] = h5py.ExternalLink(
-                    f"additional_data_{self._additional_data_id}.hdf5", f"/episode_{id}"
-                )
-                file[f"episode_{last_episode_id + id}"].attrs.modify(
-                    "id", last_episode_id + id
-                )
-
-            # Update metadata of minari dataset
-            file.attrs.modify(
-                "total_episodes", last_episode_id + new_data_total_episodes
-            )
-            file.attrs.modify(
-                "total_steps", file.attrs["total_steps"] + new_data_total_steps
-            )
         self._additional_data_id += 1
 
+        self._episode_indices = np.append(
+            self._episode_indices, np.arange(old_total_episodes, new_total_episodes)
+        )  # ~= np.append(self._episode_indices,np.arange(self._data.total_episodes))
+
+        self.spec.total_episodes = self._episode_indices.size
+        self.spec.total_steps = sum(
+            self._data.apply(
+                lambda episode: episode["total_timesteps"],
+                episode_indices=self._episode_indices,
+            )
+        )
+
     def update_dataset_from_buffer(self, buffer: List[dict]):
         """Additional data can be added to the Minari Dataset from a list of episode dictionary buffers.
 
         Each episode dictionary buffer must have the following items:
             * `observations`: np.ndarray of step observations. shape = (total_episode_steps + 1, (observation_shape)). Should include initial and final observation
             * `actions`: np.ndarray of step action. shape = (total_episode_steps + 1, (action_shape)).
             * `rewards`: np.ndarray of step rewards. shape = (total_episode_steps + 1, 1).
@@ -290,46 +302,36 @@
             * `truncations`: np.ndarray of step truncations. shape = (total_episode_steps + 1, 1).
 
         Other additional items can be added as long as the values are np.ndarray's or other nested dictionaries.
 
         Args:
             buffer (list[dict]): list of episode dictionary buffers to add to dataset
         """
-        additional_steps = 0
-        with h5py.File(self.spec.data_path, "a", track_order=True) as file:
-            last_episode_id = file.attrs["total_episodes"]
-            for i, eps_buff in enumerate(buffer):
-                episode_id = last_episode_id + i
-                # check episode terminated or truncated
-                assert (
-                    eps_buff["terminations"][-1] or eps_buff["truncations"][-1]
-                ), "Each episode must be terminated or truncated before adding it to a Minari dataset"
-                assert len(eps_buff["actions"]) + 1 == len(
-                    eps_buff["observations"]
-                ), f"Number of observations {len(eps_buff['observations'])} must have an additional \
-                                                                                        element compared to the number of action steps {len(eps_buff['actions'])} \
-                                                                                        The initial and final observation must be included"
-                seed = eps_buff.pop("seed", None)
-                eps_group = clear_episode_buffer(
-                    eps_buff, file.create_group(f"episode_{episode_id}")
-                )
-
-                eps_group.attrs["id"] = episode_id
-                total_steps = len(eps_buff["actions"])
-                eps_group.attrs["total_steps"] = total_steps
-                additional_steps += total_steps
-
-                if seed is None:
-                    eps_group.attrs["seed"] = str(None)
-                else:
-                    assert isinstance(seed, int)
-                    eps_group.attrs["seed"] = seed
-
-                # TODO: save EpisodeMetadataCallback callback in MinariDataset and update new episode group metadata
-
-            file.attrs.modify("total_episodes", last_episode_id + len(buffer))
-            file.attrs.modify(
-                "total_steps", file.attrs["total_steps"] + additional_steps
+        old_total_episodes = self._data.total_episodes
+
+        self._data.update_from_buffer(buffer, self.spec.data_path)
+
+        new_total_episodes = self._data._total_episodes
+
+        self._episode_indices = np.append(
+            self._episode_indices, np.arange(old_total_episodes, new_total_episodes)
+        )  # ~= np.append(self._episode_indices,np.arange(self._data.total_episodes))
+
+        self.spec.total_episodes = self._episode_indices.size
+
+        self.spec.total_steps = sum(
+            self._data.apply(
+                lambda episode: episode["total_timesteps"],
+                episode_indices=self._episode_indices,
             )
+        )
 
     def __iter__(self):
         return self.iterate_episodes()
+
+    def __getitem__(self, idx: int) -> EpisodeData:
+        episodes_data = self._data.get_episodes([self.episode_indices[idx]])
+        assert len(episodes_data) == 1
+        return EpisodeData(**episodes_data[0])
+
+    def __len__(self) -> int:
+        return self.total_episodes
```

### Comparing `minari-0.3.1/minari/utils.py` & `minari-0.4.0/minari/storage/hosting.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,351 +1,295 @@
 from __future__ import annotations
 
+import glob
+import importlib.metadata
 import os
 import warnings
-from typing import Dict, List, Optional, Union
+from typing import Dict, List
 
-import gymnasium as gym
 import h5py
-import numpy as np
-from gymnasium.envs.registration import EnvSpec
+from google.cloud import storage  # pyright: ignore [reportGeneralTypeIssues]
+from gymnasium import logger
+from packaging.specifiers import SpecifierSet
+from tqdm.auto import tqdm  # pyright: ignore [reportMissingModuleSource]
 
-from minari import DataCollectorV0
-from minari.dataset.minari_dataset import MinariDataset, clear_episode_buffer
+from minari.dataset.minari_dataset import parse_dataset_id
 from minari.storage.datasets_root_dir import get_dataset_path
+from minari.storage.local import load_dataset
 
 
-def combine_datasets(datasets_to_combine: List[MinariDataset], new_dataset_id: str):
-    """Combine a group of MinariDataset in to a single dataset with its own name id.
+# Use importlib due to circular import when: "from minari import __version__"
+__version__ = importlib.metadata.version("minari")
 
-    A new HDF5 metadata attribute will be added to the new dataset called `combined_datasets`. This will
-    contain a list of strings with the dataset names that were combined to form this new Minari dataset.
+
+def upload_dataset(dataset_id: str, path_to_private_key: str):
+    """Upload a Minari dataset to the remote Farama server.
+
+    If you would like to upload a dataset please first get in touch with the Farama team at contact@farama.org.
 
     Args:
-        datasets_to_combine (list[MinariDataset]): list of datasets to be combined
-        new_dataset_id (str): name id for the newly created dataset
+        dataset_id (str): name id of the local Minari dataset
+        path_to_private_key (str): path to the GCP bucket json credentials. Reach out to the Farama team.
     """
-    new_dataset_path = get_dataset_path(new_dataset_id)
 
-    # Check if dataset already exists
-    if not os.path.exists(new_dataset_path):
-        new_dataset_path = os.path.join(new_dataset_path, "data")
-        os.makedirs(new_dataset_path)
-        new_data_path = os.path.join(new_dataset_path, "main_data.hdf5")
-    else:
-        raise ValueError(
-            f"A Minari dataset with ID {new_dataset_id} already exists and it cannot be overridden. Please use a different dataset name or version."
+    def _upload_local_directory_to_gcs(local_path, bucket, gcs_path):
+        assert os.path.isdir(local_path)
+        for local_file in glob.glob(local_path + "/**"):
+            if not os.path.isfile(local_file):
+                _upload_local_directory_to_gcs(
+                    local_file, bucket, gcs_path + "/" + os.path.basename(local_file)
+                )
+            else:
+                remote_path = os.path.join(gcs_path, local_file[1 + len(local_path) :])
+                blob = bucket.blob(remote_path)
+                # add metadata to main data file of dataset
+                if blob.name.endswith("main_data.hdf5"):
+                    blob.metadata = metadata
+                blob.upload_from_filename(local_file)
+
+    file_path = get_dataset_path(dataset_id)
+    remote_datasets = list_remote_datasets()
+    if dataset_id not in remote_datasets.keys():
+        storage_client = storage.Client.from_service_account_json(
+            json_credentials_path=path_to_private_key
         )
+        bucket = storage.Bucket(storage_client, "minari-datasets")
 
-    with h5py.File(new_data_path, "a", track_order=True) as combined_data_file:
-        combined_data_file.attrs["total_episodes"] = 0
-        combined_data_file.attrs["total_steps"] = 0
-        combined_data_file.attrs["dataset_id"] = new_dataset_id
-
-        combined_data_file.attrs["combined_datasets"] = [
-            dataset.spec.dataset_id for dataset in datasets_to_combine
-        ]
-
-        current_env_spec = None
-
-        for dataset in datasets_to_combine:
-            if not isinstance(dataset, MinariDataset):
-                raise ValueError(f"The dataset {dataset} is not of type MinariDataset.")
-            dataset_env_spec = dataset.spec.env_spec
-
-            assert isinstance(dataset_env_spec, EnvSpec)
-            # We have to check that all datasets can be merged by checking that they come from the same
-            # environments. However, we override the time limit max_episode_steps with the max among all
-            # the datasets to be combined. Then we check if the rest of the env_spec attributes are from
-            # the same environment.
-            if current_env_spec is None:
-                current_env_spec = dataset_env_spec
-            elif dataset_env_spec.max_episode_steps is not None:
-                if current_env_spec.max_episode_steps is None:
-                    current_env_spec.max_episode_steps = (
-                        dataset_env_spec.max_episode_steps
-                    )
-                else:
-                    if (
-                        current_env_spec.max_episode_steps
-                        < dataset_env_spec.max_episode_steps
-                    ):
-                        current_env_spec.max_episode_steps = (
-                            dataset_env_spec.max_episode_steps
-                        )
-                    else:
-                        dataset_env_spec.max_episode_steps = (
-                            current_env_spec.max_episode_steps
-                        )
-
-            if current_env_spec != dataset_env_spec:
-                raise ValueError(
-                    "The datasets to be combined have different values for `env_spec` attribute."
-                )
+        dataset = load_dataset(dataset_id)
 
-            if combined_data_file.attrs.get("flatten_action") is None:
-                combined_data_file.attrs[
-                    "flatten_action"
-                ] = dataset.spec.flatten_actions
-            else:
-                if (
-                    combined_data_file.attrs["flatten_action"]
-                    != dataset.spec.flatten_actions
-                ):
-                    raise ValueError(
-                        "The datasets to be combined have different values for `flatten_action` attribute."
-                    )
-
-            if combined_data_file.attrs.get("flatten_observation") is None:
-                combined_data_file.attrs[
-                    "flatten_observation"
-                ] = dataset.spec.flatten_observations
-            else:
-                if (
-                    combined_data_file.attrs["flatten_observation"]
-                    != dataset.spec.flatten_observations
-                ):
-                    raise ValueError(
-                        "The datasets to be combined have different values for `flatten_observation` attribute."
-                    )
-
-            last_episode_id = combined_data_file.attrs["total_episodes"]
-
-            for id in range(dataset.total_episodes):
-                combined_data_file[
-                    f"episode_{last_episode_id + id}"
-                ] = h5py.ExternalLink(dataset.spec.data_path, f"/episode_{id}")
-                combined_data_file[f"episode_{last_episode_id + id}"].attrs.modify(
-                    "id", last_episode_id + id
-                )
+        with h5py.File(dataset.spec.data_path, "r") as f:
+            metadata = dict(f.attrs.items())
 
-            # Update metadata of minari dataset
-            combined_data_file.attrs.modify(
-                "total_episodes", last_episode_id + dataset.total_episodes
-            )
-            combined_data_file.attrs.modify(
-                "total_steps",
-                combined_data_file.attrs["total_steps"] + dataset.spec.total_steps,
-            )
+        # See https://github.com/googleapis/python-storage/issues/27 for discussion on progress bars
+        _upload_local_directory_to_gcs(str(file_path), bucket, dataset_id)
 
-            # TODO: list of authors, and emails
-            with h5py.File(dataset.spec.data_path, "r") as dataset_file:
-                combined_data_file.attrs.modify("author", dataset_file.attrs["author"])
-                combined_data_file.attrs.modify(
-                    "author_email", dataset_file.attrs["author_email"]
-                )
+        print(f"Dataset {dataset_id} uploaded!")
 
-        assert current_env_spec is not None
-        combined_data_file.attrs["env_spec"] = current_env_spec.to_json()
+        combined_datasets = dataset.spec.combined_datasets
 
-    return MinariDataset(new_data_path)
+        if len(combined_datasets) > 0:
+            print(
+                f"Dataset {dataset_id} is formed by a combination of the following datasets:"
+            )
+            for name in combined_datasets:
+                print(f"\t{name}")
+            for dataset in combined_datasets:
+                print(f"Uploading dataset {dataset}")
+                upload_dataset(
+                    dataset_id=dataset, path_to_private_key=path_to_private_key
+                )
+    else:
+        print(
+            f"Stopped upload of dataset {dataset_id}. {dataset_id} is already in the Farama servers."
+        )
 
 
-def split_dataset(
-    dataset: MinariDataset, sizes: List[int], seed: Optional[int] = None
-) -> List[MinariDataset]:
-    """Split a MinariDataset in multiple datasets.
+def download_dataset(dataset_id: str, force_download: bool = False):
+    """Download dataset from remote Farama server.
 
-    Args:
-        dataset (MinariDataset): the MinariDataset to split
-        sizes (List[int]): sizes of the resulting datasets
-        seed (Optiona[int]): random seed
+    An error will be raised if the dataset version is not compatible with the local installed version of Minari.
+    This error can be skipped and the download continued with the `force_download` argument. Also, with `force_download`,
+    any local datasets that match the id of the downloading dataset will be overridden.
 
-    Returns:
-        datasets (List[MinariDataset]): resulting list of datasets
+    Args:
+        dataset_id (str): name id of the Minari dataset
+        force_download (bool): boolean flag for force downloading the dataset. Default Value = False
     """
-    if sum(sizes) > dataset.total_episodes:
+    download_env_name, download_dataset_name, download_version = parse_dataset_id(
+        dataset_id
+    )
+
+    all_dataset_versions = get_remote_dataset_versions(
+        download_env_name, download_dataset_name
+    )
+
+    # 1. Check if there are any remote versions of the dataset at all
+    if not all_dataset_versions:
         raise ValueError(
-            "Incompatible arguments: the sum of sizes exceeds ",
-            f"the number of episodes in the dataset ({dataset.total_episodes})",
+            f"Couldn't find any version for dataset {download_env_name}-{download_dataset_name} in the remote Farama server."
         )
-    generator = np.random.default_rng(seed=seed)
-    indices = generator.permutation(dataset.episode_indices)
-    out_datasets = []
-    start_idx = 0
-    for length in sizes:
-        end_idx = start_idx + length
-        slice_dataset = MinariDataset(
-            dataset.spec.data_path, indices[start_idx:end_idx]
+
+    # 2. Check if there are any remote compatible versions with the local installed Minari version
+    max_version = get_remote_dataset_versions(
+        download_env_name, download_dataset_name, True, True
+    )
+    if not max_version:
+        if not force_download:
+            raise ValueError(
+                f"Couldn't find any compatible version of dataset {download_env_name}-{download_dataset_name} with the local installed version of Minari, {__version__}."
+            )
+        else:
+            logger.warn(
+                f"Couldn't find any compatible version of dataset {download_env_name}-{download_dataset_name} with the local installed version of Minari, {__version__}."
+            )
+
+    # 3. Check that the dataset version exists
+    if download_version not in all_dataset_versions:
+        e_msg = f"The dataset version, {dataset_id}, doesn't exist in the remote Farama server."
+        if not max_version:
+            raise ValueError(
+                e_msg
+                + f", and no other compatible versions with the local installed Minari version {__version__} were found."
+            )
+        else:
+            raise ValueError(
+                e_msg
+                + f" We suggest you download the latest compatible version of this dataset: {download_env_name}-{download_dataset_name}-v{max_version[0]}"
+            )
+
+    # 4. Check that the dataset version is compatible with the local installed Minari version
+    compatible_dataset_versions = get_remote_dataset_versions(
+        download_env_name, download_dataset_name, True
+    )
+    if download_version not in compatible_dataset_versions:
+        e_msg = f"The version you are trying to download for dataset, {dataset_id}, is not compatible with\
+                                    your local installed version of Minari, {__version__}."
+        if not force_download:
+            raise ValueError(
+                e_msg
+                + f" You can download the latest compatible version of this dataset: {download_env_name}-{download_dataset_name}-v{max_version[0]}."
+            )
+        # Only a warning and force download incompatible dataset
+        else:
+            logger.warn(
+                e_msg
+                + f" {dataset_id} will be FORCE download but you can download the latest compatible version of this dataset: {download_env_name}-{download_dataset_name}-v{max_version}."
+            )
+
+    # 5. Warning to recommend downloading the latest compatible version of the dataset
+    elif max_version[0] is not None and download_version < max_version[0]:
+        logger.warn(
+            f"We recommend you install a higher dataset version available and compatible with your local installed Minari version: {download_env_name}-{download_dataset_name}-v{max_version}."
         )
-        out_datasets.append(slice_dataset)
-        start_idx = end_idx
 
-    return out_datasets
+    file_path = get_dataset_path(dataset_id)
+    if os.path.exists(file_path):
+        if not force_download:
+            logger.warn(
+                f"Skipping Download. Dataset {dataset_id} found locally at {file_path}, Use force_download=True to download the dataset again.\n"
+            )
+            return
 
+    print(f"\nDownloading {dataset_id} from Farama servers...")
+    storage_client = storage.Client.create_anonymous_client()
 
-def create_dataset_from_buffers(
-    dataset_id: str,
-    env: gym.Env,
-    buffer: List[Dict[str, Union[list, Dict]]],
-    algorithm_name: Optional[str] = None,
-    author: Optional[str] = None,
-    author_email: Optional[str] = None,
-    code_permalink: Optional[str] = None,
-):
-    """Create Minari dataset from a list of episode dictionary buffers.
-
-    The ``dataset_id`` parameter corresponds to the name of the dataset, with the syntax as follows:
-    ``(env_name-)(dataset_name)(-v(version))`` where ``env_name`` identifies the name of the environment used to generate the dataset ``dataset_name``.
-    This ``dataset_id`` is used to load the Minari datasets with :meth:`minari.load_dataset`.
-
-    Each episode dictionary buffer must have the following items:
-        * `observations`: np.ndarray of step observations. shape = (total_episode_steps + 1, (observation_shape)). Should include initial and final observation
-        * `actions`: np.ndarray of step action. shape = (total_episode_steps + 1, (action_shape)).
-        * `rewards`: np.ndarray of step rewards. shape = (total_episode_steps + 1, 1).
-        * `terminations`: np.ndarray of step terminations. shape = (total_episode_steps + 1, 1).
-        * `truncations`: np.ndarray of step truncations. shape = (total_episode_steps + 1, 1).
+    bucket = storage_client.bucket(bucket_name="minari-datasets")
+    # Construct a client side representation of a blob.
+    # Note `Bucket.blob` differs from `Bucket.get_blob` as it doesn't retrieve
+    # any content from Google Cloud Storage. As we don't need additional data,
+    # using `Bucket.blob` is preferred here.
+    blobs = bucket.list_blobs(prefix=dataset_id)  # Get list of files
+    for blob in blobs:
+        print(f"\n * Downloading data file '{blob.name}' ...\n")
+        blob_dir, file_name = os.path.split(blob.name)
+        # If the object blob path is a directory continue searching for files
+        if file_name == "":
+            continue
+        blob_local_dir = os.path.join(os.path.dirname(file_path), blob_dir)
+        if not os.path.exists(blob_local_dir):
+            os.makedirs(blob_local_dir)
+        # Download progress bar:
+        # https://stackoverflow.com/questions/62811608/how-to-show-progress-bar-when-we-are-downloading-a-file-from-cloud-bucket-using
+        with open(os.path.join(blob_local_dir, file_name), "wb") as f:
+            with tqdm.wrapattr(f, "write", total=blob.size) as file_obj:
+                storage_client.download_blob_to_file(blob, file_obj)
+
+    print(f"\nDataset {dataset_id} downloaded to {file_path}")
+
+    # Skip a force download of an incompatible dataset versino
+    if download_dataset in compatible_dataset_versions:
+        combined_datasets = load_dataset(dataset_id).spec.combined_datasets
+
+        # If the dataset is a combination of other datasets download the subdatasets recursively
+        if len(combined_datasets) > 0:
+            print(
+                f"\nDataset {dataset_id} is formed by a combination of the following datasets:"
+            )
+            for name in combined_datasets:
+                print(f"  * {name}")
+            print("\nDownloading extra datasets ...")
+            for dataset in combined_datasets:
+                download_dataset(dataset_id=dataset)
 
-    Other additional items can be added as long as the values are np.ndarray's or other nested dictionaries.
+
+def list_remote_datasets(
+    latest_version: bool = False,
+    compatible_minari_version: bool = False,
+) -> Dict[str, Dict[str, str]]:
+    """Get the names and metadata of all the Minari datasets in the remote Farama server.
 
     Args:
-        dataset_id (str): name id to identify Minari dataset
-        env (gym.Env): Gymnasium environment used to collect the buffer data
-        buffer (list[Dict[str, Union[list, Dict]]]): list of episode dictionaries with data
-        algorithm_name (Optional[str], optional): name of the algorithm used to collect the data. Defaults to None.
-        author (Optional[str], optional): author that generated the dataset. Defaults to None.
-        author_email (Optional[str], optional): email of the author that generated the dataset. Defaults to None.
-        code_permalink (Optional[str], optional): link to relevant code used to generate the dataset. Defaults to None.
+        latest_version (bool): if `True` only the latest version of the datasets are returned i.e. from ['door-human-v0', 'door-human-v1`], only the metadata for v1 is returned. Default to `False`.
+        compatible_minari_version (bool): if `True` only the datasets compatible with the current Minari version are returned. Default to `False`.
 
     Returns:
-        MinariDataset
+       Dict[str, Dict[str, str]]: keys the names of the Minari datasets and values the metadata
     """
-    # NoneType warnings
-    if code_permalink is None:
-        warnings.warn(
-            "`code_permalink` is set to None. For reproducibility purposes it is highly recommended to link your dataset to versioned code.",
-            UserWarning,
-        )
-    if author is None:
-        warnings.warn(
-            "`author` is set to None. For longevity purposes it is highly recommended to provide an author name.",
-            UserWarning,
-        )
-    if author_email is None:
-        warnings.warn(
-            "`author_email` is set to None. For longevity purposes it is highly recommended to provide an author email, or some other obvious contact information.",
-            UserWarning,
+    client = storage.Client.create_anonymous_client()
+    bucket = client.bucket("minari-datasets")
+    blobs = bucket.list_blobs(delimiter="main_data.hdf5")
+
+    # Necessary to get prefixes iterable
+    next(blobs)
+
+    # Generate dict = {'env_name-dataset_name': (version, metadata)}
+    remote_datasets = {}
+    for prefix in sorted(blobs.prefixes):
+        blob = bucket.get_blob(prefix)
+        try:
+            metadata = blob.metadata
+            if compatible_minari_version and __version__ not in SpecifierSet(
+                metadata["minari_version"]
+            ):
+                continue
+            dataset_id = metadata["dataset_id"]
+            env_name, dataset_name, version = parse_dataset_id(dataset_id)
+            dataset = f"{env_name}-{dataset_name}"
+            if latest_version:
+                if (
+                    dataset not in remote_datasets
+                    or version > remote_datasets[dataset][0]
+                ):
+                    remote_datasets[dataset] = (version, metadata)
+            else:
+                remote_datasets[dataset_id] = metadata
+        except Exception:
+            warnings.warn(f"Misconfigured dataset named {blob.name} on remote")
+
+    if latest_version:
+        # Return dict = {'dataset_id': metadata}
+        return dict(
+            map(lambda x: (f"{x[0]}-v{x[1][0]}", x[1][1]), remote_datasets.items())
         )
-
-    dataset_path = get_dataset_path(dataset_id)
-
-    # Check if dataset already exists
-    if not os.path.exists(dataset_path):
-        dataset_path = os.path.join(dataset_path, "data")
-        os.makedirs(dataset_path)
-        data_path = os.path.join(dataset_path, "main_data.hdf5")
-
-        total_steps = 0
-        with h5py.File(data_path, "w", track_order=True) as file:
-            for i, eps_buff in enumerate(buffer):
-                # check episode terminated or truncated
-                assert (
-                    eps_buff["terminations"][-1] or eps_buff["truncations"][-1]
-                ), "Each episode must be terminated or truncated before adding it to a Minari dataset"
-                assert len(eps_buff["actions"]) + 1 == len(
-                    eps_buff["observations"]
-                ), f"Number of observations {len(eps_buff['observations'])} must have an additional \
-                                                                                        element compared to the number of action steps {len(eps_buff['actions'])} \
-                                                                                        The initial and final observation must be included"
-                seed = eps_buff.pop("seed", None)
-                eps_group = clear_episode_buffer(
-                    eps_buff, file.create_group(f"episode_{i}")
-                )
-
-                eps_group.attrs["id"] = i
-                total_steps = len(eps_buff["actions"])
-                eps_group.attrs["total_steps"] = total_steps
-                total_steps += total_steps
-
-                if seed is None:
-                    eps_group.attrs["seed"] = str(None)
-                else:
-                    assert isinstance(seed, int)
-                    eps_group.attrs["seed"] = seed
-
-                # TODO: save EpisodeMetadataCallback callback in MinariDataset and update new episode group metadata
-
-            file.attrs["total_episodes"] = len(buffer)
-            file.attrs["total_steps"] = total_steps
-
-            # TODO: check if observation/action have been flatten and update
-            file.attrs["flatten_observation"] = False
-            file.attrs["flatten_action"] = False
-
-            file.attrs[
-                "env_spec"
-            ] = env.spec.to_json()  # pyright: ignore [reportOptionalMemberAccess]
-            file.attrs["dataset_id"] = dataset_id
-
-        return MinariDataset(data_path)
     else:
-        raise ValueError(
-            f"A Minari dataset with ID {dataset_id} already exists and it cannot be overridden. Please use a different dataset name or version."
-        )
+        return remote_datasets
 
 
-def create_dataset_from_collector_env(
-    dataset_id: str,
-    collector_env: DataCollectorV0,
-    algorithm_name: Optional[str] = None,
-    author: Optional[str] = None,
-    author_email: Optional[str] = None,
-    code_permalink: Optional[str] = None,
-):
-    """Create a Minari dataset using the data collected from stepping with a Gymnasium environment wrapped with a `DataCollectorV0` Minari wrapper.
-
-    The ``dataset_id`` parameter corresponds to the name of the dataset, with the syntax as follows:
-    ``(env_name-)(dataset_name)(-v(version))`` where ``env_name`` identifies the name of the environment used to generate the dataset ``dataset_name``.
-    This ``dataset_id`` is used to load the Minari datasets with :meth:`minari.load_dataset`.
+def get_remote_dataset_versions(
+    env_name: str | None,
+    dataset_name: str,
+    latest_version: bool = False,
+    compatible_minari_version: bool = False,
+) -> List[int]:
+    """Finds all registered versions in the remote Farama server of the dataset given.
 
     Args:
-        dataset_id (str): name id to identify Minari dataset
-        collector_env (DataCollectorV0): Gymnasium environment used to collect the buffer data
-        buffer (list[Dict[str, Union[list, Dict]]]): list of episode dictionaries with data
-        algorithm_name (Optional[str], optional): name of the algorithm used to collect the data. Defaults to None.
-        author (Optional[str], optional): author that generated the dataset. Defaults to None.
-        author_email (Optional[str], optional): email of the author that generated the dataset. Defaults to None.
-        code_permalink (Optional[str], optional): link to relevant code used to generate the dataset. Defaults to None.
-
+        env_name (str): name to identigy the environment of the dataset
+        dataset_name (str): name of the dataset within the ``env_name``
+        latest_version (bool): if `True` only the latest version of the datasets is returned. Default to `False`.
+        compatible_minari_version: only return highest version among the datasets compatible with the local installed version of Minari. Default to `False`
     Returns:
-        MinariDataset
+        A list of integer versions of the dataset with the specified requirements.
     """
-    # NoneType warnings
-    if code_permalink is None:
-        warnings.warn(
-            "`code_permalink` is set to None. For reproducibility purposes it is highly recommended to link your dataset to versioned code.",
-            UserWarning,
-        )
-    if author is None:
-        warnings.warn(
-            "`author` is set to None. For longevity purposes it is highly recommended to provide an author name.",
-            UserWarning,
-        )
-    if author_email is None:
-        warnings.warn(
-            "`author_email` is set to None. For longevity purposes it is highly recommended to provide an author email, or some other obvious contact information.",
-            UserWarning,
+    versions: list[int] = []
+
+    for dataset_id in list_remote_datasets(
+        latest_version, compatible_minari_version
+    ).keys():
+        remote_env_name, remote_dataset_name, remote_version = parse_dataset_id(
+            dataset_id
         )
 
-    assert collector_env.datasets_path is not None
-    dataset_path = os.path.join(collector_env.datasets_path, dataset_id)
+        if remote_env_name == env_name and remote_dataset_name == dataset_name:
+            versions.append(remote_version)
 
-    # Check if dataset already exists
-    if not os.path.exists(dataset_path):
-        dataset_path = os.path.join(dataset_path, "data")
-        os.makedirs(dataset_path)
-        data_path = os.path.join(dataset_path, "main_data.hdf5")
-        collector_env.save_to_disk(
-            data_path,
-            dataset_metadata={
-                "dataset_id": str(dataset_id),
-                "algorithm_name": str(algorithm_name),
-                "author": str(author),
-                "author_email": str(author_email),
-                "code_permalink": str(code_permalink),
-            },
-        )
-        return MinariDataset(data_path)
-    else:
-        raise ValueError(
-            f"A Minari dataset with ID {dataset_id} already exists and it cannot be overridden. Please use a different dataset name or version."
-        )
+    return versions
```

### Comparing `minari-0.3.1/minari.egg-info/PKG-INFO` & `minari-0.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 Metadata-Version: 2.1
 Name: minari
-Version: 0.3.1
+Version: 0.4.0
 Summary: A standard format for offline reinforcement learning datasets, with popular reference datasets and related utilities.
 Author-email: Farama Foundation <contact@farama.org>
 License: MIT License
 Project-URL: Homepage, https://farama.org
 Project-URL: Repository, https://github.com/Farama-Foundation/Minari
 Project-URL: Documentation, https://minari.farama.org/
 Project-URL: Bug Report, https://github.com/Farama-Foundation/Minari/issues
 Keywords: Reinforcement Learning,Offline RL,RL,AI,gymnasium,Farama
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) 
+
+
 <p align="center">
     <img src="minari-text.png" width="500px"/>
 </p>
 
 Minari is a Python library for conducting research in offline reinforcement learning, akin to an offline version of Gymnasium or an offline RL version of HuggingFace's datasets library. This library is currently in beta.
 
 The documentation website is at [minari.farama.org](https://minari.farama.org/main/). We also have a public discord server (which we use for Q&A and to coordinate development work) that you can join here: https://discord.gg/bnJ6kubTg6.
 
 Note: Minari was previously developed under the name Kabuki.
 
 
 ## Installation
+To install Minari from [PyPI](https://pypi.org/project/minari/):
+```
+pip install minari
+```
 
-Currently the beta release is under development. If you'd like to start testing or contribute to Minari please install this project from source with: 
+Note that currently Minari is under a beta release. If you'd like to start testing or contribute to Minari please install this project from source with: 
 
 ```bash
 git clone https://github.com/Farama-Foundation/Minari.git
 cd Minari
 pip install -e .
 ```
 
@@ -68,18 +74,26 @@
 ```
 
 To download a dataset:
 
 ```python
 import minari
 
-dataset = minari.download_dataset("LunarLander_v2_remote-test-dataset")
+minari.download_dataset("door-cloned-v1")
+```
+
+To load a dataset:
+
+```python
+import minari
+
+dataset = minari.load_dataset("door-cloned-v1")
 ```
 
 ## Project Maintainers
-Main Contributors: [Rodrigo Perez-Vicente](https://github.com/rodrigodelazcano), [Omar Younis](https://github.com/younik)
+Main Contributors: [Rodrigo Perez-Vicente](https://github.com/rodrigodelazcano), [Omar Younis](https://github.com/younik), [John Balis](https://github.com/balisujohn)
 
 Maintenance for this project is also contributed by the broader Farama team: [farama.org/team](https://farama.org/team).
 
 ___
 
 _Minari is a shortening of Minarai, the Japanese word for "learning by observation"._
```

### Comparing `minari-0.3.1/minari.egg-info/SOURCES.txt` & `minari-0.4.0/minari.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 minari/__init__.py
 minari/cli.py
+minari/serialization.py
 minari/utils.py
 minari.egg-info/PKG-INFO
 minari.egg-info/SOURCES.txt
 minari.egg-info/dependency_links.txt
 minari.egg-info/entry_points.txt
 minari.egg-info/requires.txt
 minari.egg-info/top_level.txt
@@ -19,10 +20,8 @@
 minari/dataset/__init__.py
 minari/dataset/minari_dataset.py
 minari/dataset/minari_storage.py
 minari/storage/__init__.py
 minari/storage/datasets_root_dir.py
 minari/storage/hosting.py
 minari/storage/local.py
-tests/test_dataset_combine.py
-tests/test_dataset_creation.py
-tests/test_dataset_download.py
+tests/test_serialization.py
```

### Comparing `minari-0.3.1/pyproject.toml` & `minari-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,38 +4,38 @@
 requires = ["setuptools >= 61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "minari"
 description = "A standard format for offline reinforcement learning datasets, with popular reference datasets and related utilities."
 readme = "README.md"
-requires-python = ">= 3.7"
+requires-python = ">= 3.8"
 authors = [{ name = "Farama Foundation", email = "contact@farama.org" }]
 license = { text = "MIT License" }
 keywords = ["Reinforcement Learning", "Offline RL", "RL", "AI", "gymnasium", "Farama"]
 classifiers = [
     "Development Status :: 4 - Beta",  # change to `5 - Production/Stable` when ready
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     'Intended Audience :: Science/Research',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
 ]
 dependencies = [
     "numpy >=1.21.0",
-    "h5py==3.7.0",
+    "h5py>=3.8.0",
     "tqdm>=4.65.0",
     "typing_extensions==4.4.0",
     "google-cloud-storage==2.5.0",
-    "typer[all]==0.7.0",
+    "typer[all]==0.9.0",
     "gymnasium>=0.28.1",
+    "portion==2.4.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 testing = [
     "pytest ==7.1.3",
     "gymnasium-robotics>=1.2.1",
@@ -74,15 +74,15 @@
 
 [tool.pyright]
 include = ["minari/**", "tests/**"]
 exclude = ["**/node_modules", "**/__pycache__"]
 strict = []
 
 typeCheckingMode = "basic"
-pythonVersion = "3.7"
+pythonVersion = "3.8"
 pythonPlatform = "All"
 typeshedPath = "typeshed"
 enableTypeIgnoreComments = true
 
 # This is required as the CI pre-commit does not download the module (i.e. numpy, pygame, box2d)
 #   Therefore, we have to ignore missing imports
 reportMissingImports = "none"
```

### Comparing `minari-0.3.1/setup.py` & `minari-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup
 
 
 CWD = pathlib.Path(__file__).absolute().parent
 
 
 def get_version():
-    """Gets the gymnasium version."""
+    """Gets the Minari version."""
     path = CWD / "minari" / "__init__.py"
     content = path.read_text()
 
     for line in content.splitlines():
         if line.startswith("__version__"):
             return line.strip().split()[-1].strip().strip('"')
     raise RuntimeError("bad version data in __init__.py")
```

