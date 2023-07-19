# Comparing `tmp/eotdl-2023.6.27.tar.gz` & `tmp/eotdl-2023.7.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eotdl-2023.6.27.tar", max compression
+gzip compressed data, was "eotdl-2023.7.19.tar", max compression
```

## Comparing `eotdl-2023.6.27.tar` & `eotdl-2023.7.19.tar`

### file list

```diff
@@ -1,56 +1,60 @@
--rw-r--r--   0        0        0       55 2023-06-14 11:11:09.535553 eotdl-2023.6.27/README.md
--rw-r--r--   0        0        0      936 2023-06-14 11:29:35.346126 eotdl-2023.6.27/eotdl/__init__.py
--rw-r--r--   0        0        0      292 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/access/__init__.py
--rw-r--r--   0        0        0      363 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/access/parameters.py
--rw-r--r--   0        0        0      252 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/access/sentinelhub/__init__.py
--rw-r--r--   0        0        0     7605 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/access/sentinelhub/client.py
--rw-r--r--   0        0        0     6595 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/access/sentinelhub/utils.py
--rw-r--r--   0        0        0       66 2023-06-14 12:47:21.260036 eotdl-2023.6.27/eotdl/auth/__init__.py
--rw-r--r--   0        0        0      857 2023-06-14 12:49:25.712094 eotdl-2023.6.27/eotdl/auth/main.py
--rw-r--r--   0        0        0      193 2023-06-14 12:17:22.982144 eotdl-2023.6.27/eotdl/cli.py
--rw-r--r--   0        0        0        0 2023-06-14 10:24:15.563978 eotdl-2023.6.27/eotdl/commands/__init__.py
--rw-r--r--   0        0        0      937 2023-06-14 13:05:32.317534 eotdl-2023.6.27/eotdl/commands/auth.py
--rw-r--r--   0        0        0     1298 2023-06-19 14:16:48.822880 eotdl-2023.6.27/eotdl/commands/datasets.py
--rw-r--r--   0        0        0      270 2023-06-14 10:33:31.353776 eotdl-2023.6.27/eotdl/curation/__init__.py
--rw-r--r--   0        0        0     2929 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/curation/formatters.py
--rw-r--r--   0        0        0     1552 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/curation/metadata.py
--rw-r--r--   0        0        0      201 2023-06-14 09:35:56.383873 eotdl-2023.6.27/eotdl/curation/stac/__init__.py
--rw-r--r--   0        0        0     8495 2023-06-14 10:12:58.941969 eotdl-2023.6.27/eotdl/curation/stac/dataframe.py
--rw-r--r--   0        0        0     5231 2023-06-14 09:10:22.117884 eotdl-2023.6.27/eotdl/curation/stac/extensions.py
--rw-r--r--   0        0        0     1380 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/curation/stac/parsers.py
--rw-r--r--   0        0        0    17796 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/curation/stac/stac.py
--rw-r--r--   0        0        0     1855 2023-06-14 09:09:09.621596 eotdl-2023.6.27/eotdl/curation/stac/utils.py
--rw-r--r--   0        0        0      159 2023-06-19 14:05:03.242426 eotdl-2023.6.27/eotdl/datasets/__init__.py
--rw-r--r--   0        0        0      481 2023-06-16 12:06:24.332346 eotdl-2023.6.27/eotdl/datasets/download.py
--rw-r--r--   0        0        0     1583 2023-06-16 10:46:33.504518 eotdl-2023.6.27/eotdl/datasets/ingest.py
--rw-r--r--   0        0        0      534 2023-06-14 12:41:38.606725 eotdl-2023.6.27/eotdl/datasets/retrieve.py
--rw-r--r--   0        0        0       74 2023-04-18 14:58:49.560135 eotdl-2023.6.27/eotdl/hello.py
--rw-r--r--   0        0        0        0 2023-06-14 10:24:20.807993 eotdl-2023.6.27/eotdl/src/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 10:24:20.811993 eotdl-2023.6.27/eotdl/src/errors/__init__.py
--rw-r--r--   0        0        0      306 2023-06-14 10:24:20.811993 eotdl-2023.6.27/eotdl/src/errors/auth.py
--rw-r--r--   0        0        0    10025 2023-06-19 14:50:31.920344 eotdl-2023.6.27/eotdl/src/repos/APIRepo.py
--rw-r--r--   0        0        0      987 2023-06-14 12:53:43.856124 eotdl-2023.6.27/eotdl/src/repos/AuthRepo.py
--rw-r--r--   0        0        0       59 2023-06-14 10:24:20.815993 eotdl-2023.6.27/eotdl/src/repos/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 10:24:20.815993 eotdl-2023.6.27/eotdl/src/usecases/__init__.py
--rw-r--r--   0        0        0     1587 2023-06-14 10:24:20.815993 eotdl-2023.6.27/eotdl/src/usecases/auth/Auth.py
--rw-r--r--   0        0        0      332 2023-06-14 10:24:20.815993 eotdl-2023.6.27/eotdl/src/usecases/auth/IsLogged.py
--rw-r--r--   0        0        0      420 2023-06-14 10:24:20.815993 eotdl-2023.6.27/eotdl/src/usecases/auth/Logout.py
--rw-r--r--   0        0        0       81 2023-06-14 12:28:54.159966 eotdl-2023.6.27/eotdl/src/usecases/auth/__init__.py
--rw-r--r--   0        0        0     1908 2023-06-16 12:03:45.195900 eotdl-2023.6.27/eotdl/src/usecases/datasets/DownloadDataset.py
--rw-r--r--   0        0        0      940 2023-06-16 11:34:57.062552 eotdl-2023.6.27/eotdl/src/usecases/datasets/DownloadFile.py
--rw-r--r--   0        0        0      953 2023-06-14 12:59:21.144637 eotdl-2023.6.27/eotdl/src/usecases/datasets/IngestDataset.py
--rw-r--r--   0        0        0     1943 2023-06-19 14:49:41.092104 eotdl-2023.6.27/eotdl/src/usecases/datasets/IngestFile.py
--rw-r--r--   0        0        0     1337 2023-06-16 11:23:06.416437 eotdl-2023.6.27/eotdl/src/usecases/datasets/IngestFolder.py
--rw-r--r--   0        0        0     1428 2023-06-14 12:59:27.016649 eotdl-2023.6.27/eotdl/src/usecases/datasets/IngestLargeDataset.py
--rw-r--r--   0        0        0     1595 2023-06-14 10:24:20.819993 eotdl-2023.6.27/eotdl/src/usecases/datasets/IngestLargeDatasetParallel.py
--rw-r--r--   0        0        0      421 2023-06-14 10:24:20.819993 eotdl-2023.6.27/eotdl/src/usecases/datasets/RetrieveDataset.py
--rw-r--r--   0        0        0      455 2023-06-16 11:29:50.861680 eotdl-2023.6.27/eotdl/src/usecases/datasets/RetrieveDatasets.py
--rw-r--r--   0        0        0      303 2023-06-16 12:06:29.796362 eotdl-2023.6.27/eotdl/src/usecases/datasets/__init__.py
--rw-r--r--   0        0        0      479 2023-06-16 09:41:47.694244 eotdl-2023.6.27/eotdl/src/utils.py
--rw-r--r--   0        0        0      277 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/tools/__init__.py
--rw-r--r--   0        0        0      215 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/tools/sen12floods/__init__.py
--rw-r--r--   0        0        0     8124 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/tools/sen12floods/tools.py
--rw-r--r--   0        0        0      636 2023-06-14 08:30:42.023737 eotdl-2023.6.27/eotdl/tools/stac.py
--rw-r--r--   0        0        0      642 2023-06-27 10:43:26.613664 eotdl-2023.6.27/pyproject.toml
--rw-r--r--   0        0        0     1207 1970-01-01 00:00:00.000000 eotdl-2023.6.27/setup.py
--rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 eotdl-2023.6.27/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-06-14 11:11:09.535553 eotdl-2023.7.19/README.md
+-rw-r--r--   0        0        0      936 2023-06-14 11:29:35.346126 eotdl-2023.7.19/eotdl/__init__.py
+-rw-r--r--   0        0        0      292 2023-06-14 08:30:42.023737 eotdl-2023.7.19/eotdl/access/__init__.py
+-rw-r--r--   0        0        0      363 2023-06-14 08:30:42.023737 eotdl-2023.7.19/eotdl/access/parameters.py
+-rw-r--r--   0        0        0      252 2023-06-14 08:30:42.023737 eotdl-2023.7.19/eotdl/access/sentinelhub/__init__.py
+-rw-r--r--   0        0        0     7605 2023-06-14 08:30:42.023737 eotdl-2023.7.19/eotdl/access/sentinelhub/client.py
+-rw-r--r--   0        0        0     6595 2023-06-14 08:30:42.023737 eotdl-2023.7.19/eotdl/access/sentinelhub/utils.py
+-rw-r--r--   0        0        0       66 2023-06-14 12:47:21.260036 eotdl-2023.7.19/eotdl/auth/__init__.py
+-rw-r--r--   0        0        0      857 2023-06-14 12:49:25.712094 eotdl-2023.7.19/eotdl/auth/main.py
+-rw-r--r--   0        0        0      192 2023-07-18 14:00:04.010046 eotdl-2023.7.19/eotdl/cli.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:24:15.563978 eotdl-2023.7.19/eotdl/commands/__init__.py
+-rw-r--r--   0        0        0      937 2023-06-14 13:05:32.317534 eotdl-2023.7.19/eotdl/commands/auth.py
+-rw-r--r--   0        0        0     1555 2023-07-18 14:19:51.122330 eotdl-2023.7.19/eotdl/commands/datasets.py
+-rw-r--r--   0        0        0      270 2023-06-14 10:33:31.353776 eotdl-2023.7.19/eotdl/curation/__init__.py
+-rw-r--r--   0        0        0     2929 2023-06-14 08:30:42.023737 eotdl-2023.7.19/eotdl/curation/formatters.py
+-rw-r--r--   0        0        0     1552 2023-06-14 08:30:42.023737 eotdl-2023.7.19/eotdl/curation/metadata.py
+-rw-r--r--   0        0        0      199 2023-06-28 08:52:45.310651 eotdl-2023.7.19/eotdl/curation/stac/__init__.py
+-rw-r--r--   0        0        0     4801 2023-06-28 13:34:13.295928 eotdl-2023.7.19/eotdl/curation/stac/dataframe.py
+-rw-r--r--   0        0        0     8495 2023-06-28 08:51:21.786391 eotdl-2023.7.19/eotdl/curation/stac/dataframe_bck.py
+-rw-r--r--   0        0        0     5231 2023-06-14 09:10:22.117884 eotdl-2023.7.19/eotdl/curation/stac/extensions.py
+-rw-r--r--   0        0        0     1380 2023-06-14 08:30:42.023737 eotdl-2023.7.19/eotdl/curation/stac/parsers.py
+-rw-r--r--   0        0        0    17796 2023-06-14 08:30:42.023737 eotdl-2023.7.19/eotdl/curation/stac/stac.py
+-rw-r--r--   0        0        0     1855 2023-06-28 13:43:55.318745 eotdl-2023.7.19/eotdl/curation/stac/utils.py
+-rw-r--r--   0        0        0      183 2023-06-28 11:49:25.556463 eotdl-2023.7.19/eotdl/datasets/__init__.py
+-rw-r--r--   0        0        0      481 2023-06-16 12:06:24.332346 eotdl-2023.7.19/eotdl/datasets/download.py
+-rw-r--r--   0        0        0     1306 2023-07-18 11:25:08.852060 eotdl-2023.7.19/eotdl/datasets/ingest.py
+-rw-r--r--   0        0        0      534 2023-06-14 12:41:38.606725 eotdl-2023.7.19/eotdl/datasets/retrieve.py
+-rw-r--r--   0        0        0       74 2023-04-18 14:58:49.560135 eotdl-2023.7.19/eotdl/hello.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:24:20.807993 eotdl-2023.7.19/eotdl/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:24:20.811993 eotdl-2023.7.19/eotdl/src/errors/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-14 10:24:20.811993 eotdl-2023.7.19/eotdl/src/errors/auth.py
+-rw-r--r--   0        0        0       31 2023-07-18 10:22:04.473804 eotdl-2023.7.19/eotdl/src/models/__init__.py
+-rw-r--r--   0        0        0      390 2023-07-18 10:54:03.697537 eotdl-2023.7.19/eotdl/src/models/metadata.py
+-rw-r--r--   0        0        0     9455 2023-07-18 14:20:55.282554 eotdl-2023.7.19/eotdl/src/repos/APIRepo.py
+-rw-r--r--   0        0        0      987 2023-06-14 12:53:43.856124 eotdl-2023.7.19/eotdl/src/repos/AuthRepo.py
+-rw-r--r--   0        0        0       59 2023-06-14 10:24:20.815993 eotdl-2023.7.19/eotdl/src/repos/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:24:20.815993 eotdl-2023.7.19/eotdl/src/usecases/__init__.py
+-rw-r--r--   0        0        0     1587 2023-06-14 10:24:20.815993 eotdl-2023.7.19/eotdl/src/usecases/auth/Auth.py
+-rw-r--r--   0        0        0      332 2023-06-14 10:24:20.815993 eotdl-2023.7.19/eotdl/src/usecases/auth/IsLogged.py
+-rw-r--r--   0        0        0      420 2023-06-14 10:24:20.815993 eotdl-2023.7.19/eotdl/src/usecases/auth/Logout.py
+-rw-r--r--   0        0        0       81 2023-06-14 12:28:54.159966 eotdl-2023.7.19/eotdl/src/usecases/auth/__init__.py
+-rw-r--r--   0        0        0     2920 2023-07-18 14:20:38.662496 eotdl-2023.7.19/eotdl/src/usecases/datasets/DownloadDataset.py
+-rw-r--r--   0        0        0      940 2023-06-16 11:34:57.062552 eotdl-2023.7.19/eotdl/src/usecases/datasets/DownloadFile.py
+-rw-r--r--   0        0        0      953 2023-06-14 12:59:21.144637 eotdl-2023.7.19/eotdl/src/usecases/datasets/IngestDataset.py
+-rw-r--r--   0        0        0     2136 2023-07-18 11:55:02.486656 eotdl-2023.7.19/eotdl/src/usecases/datasets/IngestFile.py
+-rw-r--r--   0        0        0     4025 2023-07-18 13:41:37.178001 eotdl-2023.7.19/eotdl/src/usecases/datasets/IngestFolder.py
+-rw-r--r--   0        0        0     1428 2023-06-14 12:59:27.016649 eotdl-2023.7.19/eotdl/src/usecases/datasets/IngestLargeDataset.py
+-rw-r--r--   0        0        0     1595 2023-06-14 10:24:20.819993 eotdl-2023.7.19/eotdl/src/usecases/datasets/IngestLargeDatasetParallel.py
+-rw-r--r--   0        0        0     1518 2023-06-28 13:45:56.007478 eotdl-2023.7.19/eotdl/src/usecases/datasets/IngestSTAC.py
+-rw-r--r--   0        0        0      421 2023-06-14 10:24:20.819993 eotdl-2023.7.19/eotdl/src/usecases/datasets/RetrieveDataset.py
+-rw-r--r--   0        0        0      455 2023-06-16 11:29:50.861680 eotdl-2023.7.19/eotdl/src/usecases/datasets/RetrieveDatasets.py
+-rw-r--r--   0        0        0      338 2023-06-28 11:43:48.855484 eotdl-2023.7.19/eotdl/src/usecases/datasets/__init__.py
+-rw-r--r--   0        0        0      479 2023-06-28 09:13:04.844752 eotdl-2023.7.19/eotdl/src/utils.py
+-rw-r--r--   0        0        0      277 2023-06-14 08:30:42.023737 eotdl-2023.7.19/eotdl/tools/__init__.py
+-rw-r--r--   0        0        0      215 2023-06-14 08:30:42.023737 eotdl-2023.7.19/eotdl/tools/sen12floods/__init__.py
+-rw-r--r--   0        0        0     8124 2023-06-14 08:30:42.023737 eotdl-2023.7.19/eotdl/tools/sen12floods/tools.py
+-rw-r--r--   0        0        0      636 2023-06-14 08:30:42.023737 eotdl-2023.7.19/eotdl/tools/stac.py
+-rw-r--r--   0        0        0      642 2023-07-19 10:50:06.960451 eotdl-2023.7.19/pyproject.toml
+-rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 eotdl-2023.7.19/setup.py
+-rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 eotdl-2023.7.19/PKG-INFO
```

### Comparing `eotdl-2023.6.27/eotdl/__init__.py` & `eotdl-2023.7.19/eotdl/__init__.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.27/eotdl/access/sentinelhub/client.py` & `eotdl-2023.7.19/eotdl/access/sentinelhub/client.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.27/eotdl/access/sentinelhub/utils.py` & `eotdl-2023.7.19/eotdl/access/sentinelhub/utils.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.27/eotdl/auth/main.py` & `eotdl-2023.7.19/eotdl/auth/main.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.27/eotdl/commands/auth.py` & `eotdl-2023.7.19/eotdl/commands/auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.27/eotdl/curation/formatters.py` & `eotdl-2023.7.19/eotdl/curation/formatters.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.27/eotdl/curation/metadata.py` & `eotdl-2023.7.19/eotdl/curation/metadata.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.27/eotdl/curation/stac/dataframe.py` & `eotdl-2023.7.19/eotdl/curation/stac/dataframe_bck.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.27/eotdl/curation/stac/extensions.py` & `eotdl-2023.7.19/eotdl/curation/stac/extensions.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.27/eotdl/curation/stac/parsers.py` & `eotdl-2023.7.19/eotdl/curation/stac/parsers.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.27/eotdl/curation/stac/stac.py` & `eotdl-2023.7.19/eotdl/curation/stac/stac.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.27/eotdl/curation/stac/utils.py` & `eotdl-2023.7.19/eotdl/curation/stac/utils.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.27/eotdl/datasets/ingest.py` & `eotdl-2023.7.19/eotdl/datasets/ingest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,61 +1,52 @@
+import os
+
 from ..src.repos import APIRepo
-from ..src.usecases.datasets import IngestFile, IngestFolder
+from ..src.usecases.datasets import IngestFile, IngestFolder, IngestSTAC
 from ..auth import with_auth
 
+
 allowed_extensions = [
     ".zip",
     ".tar",
     ".tar.gz",
     ".csv",
     ".txt",
     ".json",
     ".pdf",
     ".md",
+    ".yml",
 ]
 
 
+def ingest_q1(dataset, stac_catalog):
+    print("hola")
+    return
+
+
 @with_auth
-def ingest_file(file, dataset, logger=None, user=None):
+def ingest_file(
+    file, dataset_id, logger=None, allowed_extensions=allowed_extensions, user=None
+):
     api_repo = APIRepo()
     ingest = IngestFile(api_repo, allowed_extensions, logger)
-    inputs = ingest.Inputs(file=file, dataset=dataset, user=user)
+    inputs = ingest.Inputs(file=file, dataset_id=dataset_id, user=user)
     outputs = ingest(inputs)
-    return outputs.dataset
+    return outputs.data
 
 
 @with_auth
-def ingest_folder(folder, dataset, logger=None, user=None):
+def ingest_folder(folder, force, delete, logger=None, user=None):
     api_repo = APIRepo()
     ingest = IngestFolder(api_repo, ingest_file, allowed_extensions, logger)
-    inputs = ingest.Inputs(folder=folder, dataset=dataset, user=user)
+    inputs = ingest.Inputs(folder=folder, user=user, force=force, delete=delete)
     outputs = ingest(inputs)
     return outputs.dataset
 
 
-# @with_auth
-# def ingest_dataset(name, description, path, logger=None, user=None):
-#     api_repo = APIRepo()
-#     ingest = IngestDataset(
-#         api_repo,
-#     )
-#     inputs = ingest.Inputs(name=name, description=description, path=path, user=user)
-#     outputs = ingest(inputs)
-#     return outputs.dataset
-
-
-# @with_auth
-# def ingest_large_dataset(name, path, logger=None, user=None):
-#     api_repo = APIRepo()
-#     ingest = IngestLargeDataset(api_repo, logger)
-#     inputs = ingest.Inputs(name=name, path=path, user=user)
-#     outputs = ingest(inputs)
-#     return outputs.dataset
-
-
-# def ingest_q0(dataset, path):
-#     return ingest_large_dataset(dataset, path)
-
-
-# def ingest_q1(dataset, stac_catalog):
-#     print("holas")
-#     return
+@with_auth
+def ingest_stac(stac_catalog, dataset, logger=None, user=None):
+    api_repo = APIRepo()
+    ingest = IngestSTAC(api_repo, ingest_file, allowed_extensions)
+    inputs = ingest.Inputs(stac_catalog=stac_catalog, dataset=dataset, user=user)
+    outputs = ingest(inputs)
+    return outputs.dataset
```

### Comparing `eotdl-2023.6.27/eotdl/datasets/retrieve.py` & `eotdl-2023.7.19/eotdl/datasets/retrieve.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.27/eotdl/src/repos/AuthRepo.py` & `eotdl-2023.7.19/eotdl/src/repos/AuthRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.27/eotdl/src/usecases/auth/Auth.py` & `eotdl-2023.7.19/eotdl/src/usecases/auth/Auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.27/eotdl/src/usecases/datasets/DownloadDataset.py` & `eotdl-2023.7.19/eotdl/src/usecases/datasets/DownloadDataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from pydantic import BaseModel
 from ....src.utils import calculate_checksum
+from ....curation.stac import STACDataFrame
+from pathlib import Path
+import os
 
 
 class DownloadDataset:
     def __init__(self, repo, retrieve_dataset, logger):
         self.repo = repo
         self.retrieve_dataset = retrieve_dataset
         self.logger = logger if logger else print
@@ -25,32 +28,52 @@
         if calculate_checksum(dst_path) != checksum:
             self.logger(f"Checksum for {file} does not match")
         self.logger(f"Done")
         return dst_path
 
     def __call__(self, inputs: Inputs) -> Outputs:
         dataset = self.retrieve_dataset(inputs.dataset)
-        if inputs.file:
-            files = [f for f in dataset["files"] if f["name"] == inputs.file]
-            if not files:
-                raise Exception(f"File {inputs.file} not found")
-            if len(files) > 1:
-                raise Exception(f"Multiple files with name {inputs.file} found")
-            dst_path = self.download(
-                inputs.dataset,
+        if inputs.path is None:
+            download_path = str(Path.home()) + "/.eotdl/datasets/" + inputs.dataset
+        else:
+            download_path = inputs.path + "/" + inputs.dataset
+        os.makedirs(download_path, exist_ok=True)
+        if dataset["quality"] == 0:
+            if inputs.file:
+                files = [f for f in dataset["files"] if f["name"] == inputs.file]
+                if not files:
+                    raise Exception(f"File {inputs.file} not found")
+                if len(files) > 1:
+                    raise Exception(f"Multiple files with name {inputs.file} found")
+                dst_path = self.download(
+                    inputs.dataset,
+                    dataset["id"],
+                    inputs.file,
+                    files[0]["checksum"],
+                    download_path,
+                    inputs.user,
+                )
+                return self.Outputs(dst_path=dst_path)
+            for file in dataset["files"]:
+                dst_path = self.download(
+                    inputs.dataset,
+                    dataset["id"],
+                    file["name"],
+                    file["checksum"],
+                    download_path,
+                    inputs.user,
+                )
+            return self.Outputs(dst_path="/".join(dst_path.split("/")[:-1]))
+        else:
+            gdf, error = self.repo.download_stac(
                 dataset["id"],
-                inputs.file,
-                files[0]["checksum"],
-                inputs.path,
-                inputs.user,
+                inputs.user["id_token"],
             )
-            return self.Outputs(dst_path=dst_path)
-        for file in dataset["files"]:
-            dst_path = self.download(
-                inputs.dataset,
-                dataset["id"],
-                file["name"],
-                file["checksum"],
-                inputs.path,
-                inputs.user,
-            )
-        return self.Outputs(dst_path="/".join(dst_path.split("/")[:-1]))
+            if error:
+                raise Exception(error)
+            df = STACDataFrame(gdf)
+            # df.geometry = df.geometry.apply(lambda x: Polygon() if x is None else x)
+            path = inputs.path
+            if path is None:
+                path = str(Path.home()) + "/.eotdl/datasets/" + dataset["name"]
+            df.to_stac(path)
+            return self.Outputs(dst_path=path)
```

### Comparing `eotdl-2023.6.27/eotdl/src/usecases/datasets/DownloadFile.py` & `eotdl-2023.7.19/eotdl/src/usecases/datasets/DownloadFile.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.27/eotdl/src/usecases/datasets/IngestDataset.py` & `eotdl-2023.7.19/eotdl/src/usecases/datasets/IngestDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.27/eotdl/src/usecases/datasets/IngestFile.py` & `eotdl-2023.7.19/eotdl/src/usecases/datasets/IngestFile.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,48 +9,52 @@
     def __init__(self, repo, allowed_extensions, logger):
         self.repo = repo
         self.allowed_extensions = allowed_extensions
         self.logger = logger if logger else print
 
     class Inputs(BaseModel):
         file: typing.Any
-        dataset: str = None
+        dataset_id: str
         user: dict
 
     class Outputs(BaseModel):
-        dataset: dict
+        data: dict
 
     def __call__(self, inputs: Inputs) -> Outputs:
         # validate file extension
         extension = os.path.splitext(inputs.file)[1]
         if extension not in self.allowed_extensions:
             raise Exception(
                 f"Only {', '.join(self.allowed_extensions)} files are allowed"
             )
+        id_token = inputs.user["id_token"]
         self.logger(f"Uploading file {inputs.file}...")
+        # if inputs.file.startswith("http://") or inputs.file.startswith("https://"):
+        #     data, error = self.repo.ingest_file_url(
+        #         inputs.file, inputs.metadata.name, id_token
+        #     )
+        # else:
         self.logger("Computing checksum...")
         checksum = calculate_checksum(inputs.file)
         self.logger(checksum)
-        self.logger("Ingesting dataset...")
-        id_token = inputs.user["id_token"]
+        self.logger("Ingesting file...")
         filesize = os.path.getsize(inputs.file)
         # ingest small file
         if filesize < 1024 * 1024 * 16:  # 16 MB
             data, error = self.repo.ingest_file(
-                inputs.file, inputs.dataset, id_token, checksum
+                inputs.file, inputs.dataset_id, id_token, checksum
             )
             if error:
                 raise Exception(error)
             self.logger("Done")
-            return self.Outputs(dataset=data)
+            return self.Outputs(data=data)
         # ingest large file
         upload_id, parts = self.repo.prepare_large_upload(
-            inputs.file, inputs.dataset, checksum, id_token
+            inputs.file, inputs.dataset_id, checksum, id_token
         )
-        print(upload_id, parts)
         self.repo.ingest_large_dataset(inputs.file, upload_id, id_token, parts)
         self.logger("\nCompleting upload...")
         data, error = self.repo.complete_upload(id_token, upload_id)
         if error:
             raise Exception(error)
         self.logger("Done")
-        return self.Outputs(dataset=data)
+        return self.Outputs(data=data)
```

### Comparing `eotdl-2023.6.27/eotdl/src/usecases/datasets/IngestLargeDataset.py` & `eotdl-2023.7.19/eotdl/src/usecases/datasets/IngestLargeDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.27/eotdl/src/usecases/datasets/IngestLargeDatasetParallel.py` & `eotdl-2023.7.19/eotdl/src/usecases/datasets/IngestLargeDatasetParallel.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.27/eotdl/tools/sen12floods/tools.py` & `eotdl-2023.7.19/eotdl/tools/sen12floods/tools.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.27/eotdl/tools/stac.py` & `eotdl-2023.7.19/eotdl/tools/stac.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.6.27/pyproject.toml` & `eotdl-2023.7.19/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eotdl"
-version = "2023.06.27"
+version = "2023.07.19"
 description = "Earth Observation Training Data Lab"
 authors = ["EarthPulse <it@earthpulse.es>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "eotdl"}]
 
 [tool.poetry.scripts]
```

### Comparing `eotdl-2023.6.27/setup.py` & `eotdl-2023.7.19/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
  'eotdl.auth',
  'eotdl.commands',
  'eotdl.curation',
  'eotdl.curation.stac',
  'eotdl.datasets',
  'eotdl.src',
  'eotdl.src.errors',
+ 'eotdl.src.models',
  'eotdl.src.repos',
  'eotdl.src.usecases',
  'eotdl.src.usecases.auth',
  'eotdl.src.usecases.datasets',
  'eotdl.tools',
  'eotdl.tools.sen12floods']
 
@@ -30,15 +31,15 @@
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['eotdl = eotdl.cli:app']}
 
 setup_kwargs = {
     'name': 'eotdl',
-    'version': '2023.6.27',
+    'version': '2023.7.19',
     'description': 'Earth Observation Training Data Lab',
     'long_description': '# eotdl \n\nThis is the main library and CLI for EOTDL.\n\n',
     'author': 'EarthPulse',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `eotdl-2023.6.27/PKG-INFO` & `eotdl-2023.7.19/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eotdl
-Version: 2023.6.27
+Version: 2023.7.19
 Summary: Earth Observation Training Data Lab
 License: MIT
 Author: EarthPulse
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

