# Comparing `tmp/slurm-usage-1.0.0.tar.gz` & `tmp/slurm-usage-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurm-usage-1.0.0.tar", last modified: Wed Sep 21 18:00:37 2022, max compression
+gzip compressed data, was "slurm-usage-1.1.0.tar", last modified: Wed Jul 19 03:42:37 2023, max compression
```

## Comparing `slurm-usage-1.0.0.tar` & `slurm-usage-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2022-09-21 18:00:37.668468 slurm-usage-1.0.0/
--rw-r--r--   0 basnijholt   (501) staff       (20)     1068 2022-09-20 20:58:08.000000 slurm-usage-1.0.0/LICENSE
--rw-r--r--   0 basnijholt   (501) staff       (20)      224 2022-09-21 18:00:37.664005 slurm-usage-1.0.0/PKG-INFO
--rw-r--r--   0 basnijholt   (501) staff       (20)      175 2022-09-20 20:58:08.000000 slurm-usage-1.0.0/README.md
--rw-r--r--   0 basnijholt   (501) staff       (20)       38 2022-09-21 18:00:37.668522 slurm-usage-1.0.0/setup.cfg
--rw-r--r--   0 basnijholt   (501) staff       (20)      414 2022-09-21 18:00:16.000000 slurm-usage-1.0.0/setup.py
-drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2022-09-21 18:00:37.662612 slurm-usage-1.0.0/slurm_usage.egg-info/
--rw-r--r--   0 basnijholt   (501) staff       (20)      224 2022-09-21 18:00:37.000000 slurm-usage-1.0.0/slurm_usage.egg-info/PKG-INFO
--rw-r--r--   0 basnijholt   (501) staff       (20)      253 2022-09-21 18:00:37.000000 slurm-usage-1.0.0/slurm_usage.egg-info/SOURCES.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)        1 2022-09-21 18:00:37.000000 slurm-usage-1.0.0/slurm_usage.egg-info/dependency_links.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)       74 2022-09-21 18:00:37.000000 slurm-usage-1.0.0/slurm_usage.egg-info/entry_points.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)        5 2022-09-21 18:00:37.000000 slurm-usage-1.0.0/slurm_usage.egg-info/requires.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)       12 2022-09-21 18:00:37.000000 slurm-usage-1.0.0/slurm_usage.egg-info/top_level.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)     2671 2022-09-21 17:59:53.000000 slurm-usage-1.0.0/slurm_usage.py
+drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2023-07-19 03:42:37.013386 slurm-usage-1.1.0/
+-rw-r--r--   0 basnijholt   (501) staff       (20)     1068 2021-09-01 11:17:48.000000 slurm-usage-1.1.0/LICENSE
+-rw-r--r--   0 basnijholt   (501) staff       (20)      224 2023-07-19 03:42:37.013256 slurm-usage-1.1.0/PKG-INFO
+-rw-r--r--   0 basnijholt   (501) staff       (20)      175 2021-09-01 11:17:48.000000 slurm-usage-1.1.0/README.md
+-rw-r--r--   0 basnijholt   (501) staff       (20)       38 2023-07-19 03:42:37.013429 slurm-usage-1.1.0/setup.cfg
+-rw-r--r--   0 basnijholt   (501) staff       (20)      414 2023-07-19 03:42:08.000000 slurm-usage-1.1.0/setup.py
+drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2023-07-19 03:42:37.013041 slurm-usage-1.1.0/slurm_usage.egg-info/
+-rw-r--r--   0 basnijholt   (501) staff       (20)      224 2023-07-19 03:42:37.000000 slurm-usage-1.1.0/slurm_usage.egg-info/PKG-INFO
+-rw-r--r--   0 basnijholt   (501) staff       (20)      253 2023-07-19 03:42:37.000000 slurm-usage-1.1.0/slurm_usage.egg-info/SOURCES.txt
+-rw-r--r--   0 basnijholt   (501) staff       (20)        1 2023-07-19 03:42:37.000000 slurm-usage-1.1.0/slurm_usage.egg-info/dependency_links.txt
+-rw-r--r--   0 basnijholt   (501) staff       (20)       74 2023-07-19 03:42:37.000000 slurm-usage-1.1.0/slurm_usage.egg-info/entry_points.txt
+-rw-r--r--   0 basnijholt   (501) staff       (20)        5 2023-07-19 03:42:37.000000 slurm-usage-1.1.0/slurm_usage.egg-info/requires.txt
+-rw-r--r--   0 basnijholt   (501) staff       (20)       12 2023-07-19 03:42:37.000000 slurm-usage-1.1.0/slurm_usage.egg-info/top_level.txt
+-rw-r--r--   0 basnijholt   (501) staff       (20)     2672 2023-07-19 03:41:57.000000 slurm-usage-1.1.0/slurm_usage.py
```

### Comparing `slurm-usage-1.0.0/LICENSE` & `slurm-usage-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slurm-usage-1.0.0/slurm_usage.py` & `slurm-usage-1.1.0/slurm_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from collections import defaultdict
 
 from rich.console import Console
 from rich.table import Table
 
 
 def squeue_output():
-    cmd = [f"squeue -o '%u/%t/%D/%P'"]
+    cmd = [f"squeue -ro '%u/%t/%D/%P'"]
     return subprocess.getoutput(cmd).split("\n")[1:]
 
 
 def process_data(output, cores_or_nodes):
     data = defaultdict(lambda: defaultdict(lambda: defaultdict(int)))
     total_partition = defaultdict(lambda: defaultdict(int))
     totals = defaultdict(int)
```

