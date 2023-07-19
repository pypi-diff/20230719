# Comparing `tmp/eotdl-2023.7.19.post2.tar.gz` & `tmp/eotdl-2023.7.19.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eotdl-2023.7.19.post2.tar", max compression
+gzip compressed data, was "eotdl-2023.7.19.post3.tar", max compression
```

## Comparing `eotdl-2023.7.19.post2.tar` & `eotdl-2023.7.19.post3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0       55 2023-06-14 11:11:09.535553 eotdl-2023.7.19.post2/README.md
--rw-r--r--   0        0        0      936 2023-06-14 11:29:35.346126 eotdl-2023.7.19.post2/eotdl/__init__.py
--rw-r--r--   0        0        0      292 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post2/eotdl/access/__init__.py
--rw-r--r--   0        0        0      363 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post2/eotdl/access/parameters.py
--rw-r--r--   0        0        0      252 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post2/eotdl/access/sentinelhub/__init__.py
--rw-r--r--   0        0        0     7605 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post2/eotdl/access/sentinelhub/client.py
--rw-r--r--   0        0        0     6595 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post2/eotdl/access/sentinelhub/utils.py
--rw-r--r--   0        0        0       66 2023-06-14 12:47:21.260036 eotdl-2023.7.19.post2/eotdl/auth/__init__.py
--rw-r--r--   0        0        0      857 2023-06-14 12:49:25.712094 eotdl-2023.7.19.post2/eotdl/auth/main.py
--rw-r--r--   0        0        0      192 2023-07-18 14:00:04.010046 eotdl-2023.7.19.post2/eotdl/cli.py
--rw-r--r--   0        0        0        0 2023-06-14 10:24:15.563978 eotdl-2023.7.19.post2/eotdl/commands/__init__.py
--rw-r--r--   0        0        0      937 2023-06-14 13:05:32.317534 eotdl-2023.7.19.post2/eotdl/commands/auth.py
--rw-r--r--   0        0        0     1555 2023-07-18 14:19:51.122330 eotdl-2023.7.19.post2/eotdl/commands/datasets.py
--rw-r--r--   0        0        0      270 2023-06-14 10:33:31.353776 eotdl-2023.7.19.post2/eotdl/curation/__init__.py
--rw-r--r--   0        0        0     2929 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post2/eotdl/curation/formatters.py
--rw-r--r--   0        0        0     1552 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post2/eotdl/curation/metadata.py
--rw-r--r--   0        0        0      199 2023-06-28 08:52:45.310651 eotdl-2023.7.19.post2/eotdl/curation/stac/__init__.py
--rw-r--r--   0        0        0     4801 2023-06-28 13:34:13.295928 eotdl-2023.7.19.post2/eotdl/curation/stac/dataframe.py
--rw-r--r--   0        0        0     8495 2023-06-28 08:51:21.786391 eotdl-2023.7.19.post2/eotdl/curation/stac/dataframe_bck.py
--rw-r--r--   0        0        0     5231 2023-06-14 09:10:22.117884 eotdl-2023.7.19.post2/eotdl/curation/stac/extensions.py
--rw-r--r--   0        0        0     1380 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post2/eotdl/curation/stac/parsers.py
--rw-r--r--   0        0        0    17796 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post2/eotdl/curation/stac/stac.py
--rw-r--r--   0        0        0     1855 2023-06-28 13:43:55.318745 eotdl-2023.7.19.post2/eotdl/curation/stac/utils.py
--rw-r--r--   0        0        0      183 2023-06-28 11:49:25.556463 eotdl-2023.7.19.post2/eotdl/datasets/__init__.py
--rw-r--r--   0        0        0      481 2023-06-16 12:06:24.332346 eotdl-2023.7.19.post2/eotdl/datasets/download.py
--rw-r--r--   0        0        0     1306 2023-07-18 11:25:08.852060 eotdl-2023.7.19.post2/eotdl/datasets/ingest.py
--rw-r--r--   0        0        0      534 2023-06-14 12:41:38.606725 eotdl-2023.7.19.post2/eotdl/datasets/retrieve.py
--rw-r--r--   0        0        0       74 2023-04-18 14:58:49.560135 eotdl-2023.7.19.post2/eotdl/hello.py
--rw-r--r--   0        0        0        0 2023-06-14 10:24:20.807993 eotdl-2023.7.19.post2/eotdl/src/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 10:24:20.811993 eotdl-2023.7.19.post2/eotdl/src/errors/__init__.py
--rw-r--r--   0        0        0      306 2023-06-14 10:24:20.811993 eotdl-2023.7.19.post2/eotdl/src/errors/auth.py
--rw-r--r--   0        0        0       31 2023-07-18 10:22:04.473804 eotdl-2023.7.19.post2/eotdl/src/models/__init__.py
--rw-r--r--   0        0        0      390 2023-07-18 10:54:03.697537 eotdl-2023.7.19.post2/eotdl/src/models/metadata.py
--rw-r--r--   0        0        0     9455 2023-07-18 14:20:55.282554 eotdl-2023.7.19.post2/eotdl/src/repos/APIRepo.py
--rw-r--r--   0        0        0      987 2023-06-14 12:53:43.856124 eotdl-2023.7.19.post2/eotdl/src/repos/AuthRepo.py
--rw-r--r--   0        0        0       59 2023-06-14 10:24:20.815993 eotdl-2023.7.19.post2/eotdl/src/repos/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 10:24:20.815993 eotdl-2023.7.19.post2/eotdl/src/usecases/__init__.py
--rw-r--r--   0        0        0     1587 2023-06-14 10:24:20.815993 eotdl-2023.7.19.post2/eotdl/src/usecases/auth/Auth.py
--rw-r--r--   0        0        0      332 2023-06-14 10:24:20.815993 eotdl-2023.7.19.post2/eotdl/src/usecases/auth/IsLogged.py
--rw-r--r--   0        0        0      420 2023-06-14 10:24:20.815993 eotdl-2023.7.19.post2/eotdl/src/usecases/auth/Logout.py
--rw-r--r--   0        0        0       81 2023-06-14 12:28:54.159966 eotdl-2023.7.19.post2/eotdl/src/usecases/auth/__init__.py
--rw-r--r--   0        0        0     2920 2023-07-18 14:20:38.662496 eotdl-2023.7.19.post2/eotdl/src/usecases/datasets/DownloadDataset.py
--rw-r--r--   0        0        0      940 2023-06-16 11:34:57.062552 eotdl-2023.7.19.post2/eotdl/src/usecases/datasets/DownloadFile.py
--rw-r--r--   0        0        0      953 2023-06-14 12:59:21.144637 eotdl-2023.7.19.post2/eotdl/src/usecases/datasets/IngestDataset.py
--rw-r--r--   0        0        0     2136 2023-07-18 11:55:02.486656 eotdl-2023.7.19.post2/eotdl/src/usecases/datasets/IngestFile.py
--rw-r--r--   0        0        0     4025 2023-07-18 13:41:37.178001 eotdl-2023.7.19.post2/eotdl/src/usecases/datasets/IngestFolder.py
--rw-r--r--   0        0        0     1428 2023-06-14 12:59:27.016649 eotdl-2023.7.19.post2/eotdl/src/usecases/datasets/IngestLargeDataset.py
--rw-r--r--   0        0        0     1595 2023-06-14 10:24:20.819993 eotdl-2023.7.19.post2/eotdl/src/usecases/datasets/IngestLargeDatasetParallel.py
--rw-r--r--   0        0        0     1518 2023-06-28 13:45:56.007478 eotdl-2023.7.19.post2/eotdl/src/usecases/datasets/IngestSTAC.py
--rw-r--r--   0        0        0      421 2023-06-14 10:24:20.819993 eotdl-2023.7.19.post2/eotdl/src/usecases/datasets/RetrieveDataset.py
--rw-r--r--   0        0        0      455 2023-06-16 11:29:50.861680 eotdl-2023.7.19.post2/eotdl/src/usecases/datasets/RetrieveDatasets.py
--rw-r--r--   0        0        0      338 2023-06-28 11:43:48.855484 eotdl-2023.7.19.post2/eotdl/src/usecases/datasets/__init__.py
--rw-r--r--   0        0        0      479 2023-06-28 09:13:04.844752 eotdl-2023.7.19.post2/eotdl/src/utils.py
--rw-r--r--   0        0        0      277 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post2/eotdl/tools/__init__.py
--rw-r--r--   0        0        0      215 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post2/eotdl/tools/sen12floods/__init__.py
--rw-r--r--   0        0        0     8124 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post2/eotdl/tools/sen12floods/tools.py
--rw-r--r--   0        0        0      636 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post2/eotdl/tools/stac.py
--rw-r--r--   0        0        0      702 2023-07-19 11:05:03.443415 eotdl-2023.7.19.post2/pyproject.toml
--rw-r--r--   0        0        0     1314 1970-01-01 00:00:00.000000 eotdl-2023.7.19.post2/setup.py
--rw-r--r--   0        0        0      867 1970-01-01 00:00:00.000000 eotdl-2023.7.19.post2/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-06-14 11:11:09.535553 eotdl-2023.7.19.post3/README.md
+-rw-r--r--   0        0        0      936 2023-06-14 11:29:35.346126 eotdl-2023.7.19.post3/eotdl/__init__.py
+-rw-r--r--   0        0        0      292 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post3/eotdl/access/__init__.py
+-rw-r--r--   0        0        0      363 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post3/eotdl/access/parameters.py
+-rw-r--r--   0        0        0      252 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post3/eotdl/access/sentinelhub/__init__.py
+-rw-r--r--   0        0        0     7605 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post3/eotdl/access/sentinelhub/client.py
+-rw-r--r--   0        0        0     6595 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post3/eotdl/access/sentinelhub/utils.py
+-rw-r--r--   0        0        0       66 2023-06-14 12:47:21.260036 eotdl-2023.7.19.post3/eotdl/auth/__init__.py
+-rw-r--r--   0        0        0      857 2023-06-14 12:49:25.712094 eotdl-2023.7.19.post3/eotdl/auth/main.py
+-rw-r--r--   0        0        0      192 2023-07-18 14:00:04.010046 eotdl-2023.7.19.post3/eotdl/cli.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:24:15.563978 eotdl-2023.7.19.post3/eotdl/commands/__init__.py
+-rw-r--r--   0        0        0      937 2023-06-14 13:05:32.317534 eotdl-2023.7.19.post3/eotdl/commands/auth.py
+-rw-r--r--   0        0        0     1555 2023-07-18 14:19:51.122330 eotdl-2023.7.19.post3/eotdl/commands/datasets.py
+-rw-r--r--   0        0        0      270 2023-06-14 10:33:31.353776 eotdl-2023.7.19.post3/eotdl/curation/__init__.py
+-rw-r--r--   0        0        0     2929 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post3/eotdl/curation/formatters.py
+-rw-r--r--   0        0        0     1552 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post3/eotdl/curation/metadata.py
+-rw-r--r--   0        0        0      199 2023-06-28 08:52:45.310651 eotdl-2023.7.19.post3/eotdl/curation/stac/__init__.py
+-rw-r--r--   0        0        0     4801 2023-06-28 13:34:13.295928 eotdl-2023.7.19.post3/eotdl/curation/stac/dataframe.py
+-rw-r--r--   0        0        0     8495 2023-06-28 08:51:21.786391 eotdl-2023.7.19.post3/eotdl/curation/stac/dataframe_bck.py
+-rw-r--r--   0        0        0     5231 2023-06-14 09:10:22.117884 eotdl-2023.7.19.post3/eotdl/curation/stac/extensions.py
+-rw-r--r--   0        0        0     1380 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post3/eotdl/curation/stac/parsers.py
+-rw-r--r--   0        0        0    17796 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post3/eotdl/curation/stac/stac.py
+-rw-r--r--   0        0        0     1855 2023-06-28 13:43:55.318745 eotdl-2023.7.19.post3/eotdl/curation/stac/utils.py
+-rw-r--r--   0        0        0      183 2023-06-28 11:49:25.556463 eotdl-2023.7.19.post3/eotdl/datasets/__init__.py
+-rw-r--r--   0        0        0      481 2023-06-16 12:06:24.332346 eotdl-2023.7.19.post3/eotdl/datasets/download.py
+-rw-r--r--   0        0        0     1306 2023-07-18 11:25:08.852060 eotdl-2023.7.19.post3/eotdl/datasets/ingest.py
+-rw-r--r--   0        0        0      534 2023-06-14 12:41:38.606725 eotdl-2023.7.19.post3/eotdl/datasets/retrieve.py
+-rw-r--r--   0        0        0       74 2023-04-18 14:58:49.560135 eotdl-2023.7.19.post3/eotdl/hello.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:24:20.807993 eotdl-2023.7.19.post3/eotdl/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:24:20.811993 eotdl-2023.7.19.post3/eotdl/src/errors/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-14 10:24:20.811993 eotdl-2023.7.19.post3/eotdl/src/errors/auth.py
+-rw-r--r--   0        0        0       31 2023-07-18 10:22:04.473804 eotdl-2023.7.19.post3/eotdl/src/models/__init__.py
+-rw-r--r--   0        0        0      390 2023-07-18 10:54:03.697537 eotdl-2023.7.19.post3/eotdl/src/models/metadata.py
+-rw-r--r--   0        0        0     9455 2023-07-18 14:20:55.282554 eotdl-2023.7.19.post3/eotdl/src/repos/APIRepo.py
+-rw-r--r--   0        0        0      987 2023-06-14 12:53:43.856124 eotdl-2023.7.19.post3/eotdl/src/repos/AuthRepo.py
+-rw-r--r--   0        0        0       59 2023-06-14 10:24:20.815993 eotdl-2023.7.19.post3/eotdl/src/repos/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:24:20.815993 eotdl-2023.7.19.post3/eotdl/src/usecases/__init__.py
+-rw-r--r--   0        0        0     1587 2023-06-14 10:24:20.815993 eotdl-2023.7.19.post3/eotdl/src/usecases/auth/Auth.py
+-rw-r--r--   0        0        0      332 2023-06-14 10:24:20.815993 eotdl-2023.7.19.post3/eotdl/src/usecases/auth/IsLogged.py
+-rw-r--r--   0        0        0      420 2023-06-14 10:24:20.815993 eotdl-2023.7.19.post3/eotdl/src/usecases/auth/Logout.py
+-rw-r--r--   0        0        0       81 2023-06-14 12:28:54.159966 eotdl-2023.7.19.post3/eotdl/src/usecases/auth/__init__.py
+-rw-r--r--   0        0        0     2920 2023-07-18 14:20:38.662496 eotdl-2023.7.19.post3/eotdl/src/usecases/datasets/DownloadDataset.py
+-rw-r--r--   0        0        0      940 2023-06-16 11:34:57.062552 eotdl-2023.7.19.post3/eotdl/src/usecases/datasets/DownloadFile.py
+-rw-r--r--   0        0        0      953 2023-06-14 12:59:21.144637 eotdl-2023.7.19.post3/eotdl/src/usecases/datasets/IngestDataset.py
+-rw-r--r--   0        0        0     2136 2023-07-18 11:55:02.486656 eotdl-2023.7.19.post3/eotdl/src/usecases/datasets/IngestFile.py
+-rw-r--r--   0        0        0     3986 2023-07-19 12:52:07.876035 eotdl-2023.7.19.post3/eotdl/src/usecases/datasets/IngestFolder.py
+-rw-r--r--   0        0        0     1428 2023-06-14 12:59:27.016649 eotdl-2023.7.19.post3/eotdl/src/usecases/datasets/IngestLargeDataset.py
+-rw-r--r--   0        0        0     1595 2023-06-14 10:24:20.819993 eotdl-2023.7.19.post3/eotdl/src/usecases/datasets/IngestLargeDatasetParallel.py
+-rw-r--r--   0        0        0     1518 2023-06-28 13:45:56.007478 eotdl-2023.7.19.post3/eotdl/src/usecases/datasets/IngestSTAC.py
+-rw-r--r--   0        0        0      421 2023-06-14 10:24:20.819993 eotdl-2023.7.19.post3/eotdl/src/usecases/datasets/RetrieveDataset.py
+-rw-r--r--   0        0        0      455 2023-06-16 11:29:50.861680 eotdl-2023.7.19.post3/eotdl/src/usecases/datasets/RetrieveDatasets.py
+-rw-r--r--   0        0        0      338 2023-06-28 11:43:48.855484 eotdl-2023.7.19.post3/eotdl/src/usecases/datasets/__init__.py
+-rw-r--r--   0        0        0      479 2023-06-28 09:13:04.844752 eotdl-2023.7.19.post3/eotdl/src/utils.py
+-rw-r--r--   0        0        0      277 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post3/eotdl/tools/__init__.py
+-rw-r--r--   0        0        0      215 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post3/eotdl/tools/sen12floods/__init__.py
+-rw-r--r--   0        0        0     8124 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post3/eotdl/tools/sen12floods/tools.py
+-rw-r--r--   0        0        0      636 2023-06-14 08:30:42.023737 eotdl-2023.7.19.post3/eotdl/tools/stac.py
+-rw-r--r--   0        0        0      702 2023-07-19 12:53:19.908371 eotdl-2023.7.19.post3/pyproject.toml
+-rw-r--r--   0        0        0     1314 1970-01-01 00:00:00.000000 eotdl-2023.7.19.post3/setup.py
+-rw-r--r--   0        0        0      867 1970-01-01 00:00:00.000000 eotdl-2023.7.19.post3/PKG-INFO
```

### Comparing `eotdl-2023.7.19.post2/eotdl/__init__.py` & `eotdl-2023.7.19.post3/eotdl/__init__.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/access/sentinelhub/client.py` & `eotdl-2023.7.19.post3/eotdl/access/sentinelhub/client.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/access/sentinelhub/utils.py` & `eotdl-2023.7.19.post3/eotdl/access/sentinelhub/utils.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/auth/main.py` & `eotdl-2023.7.19.post3/eotdl/auth/main.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/commands/auth.py` & `eotdl-2023.7.19.post3/eotdl/commands/auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/commands/datasets.py` & `eotdl-2023.7.19.post3/eotdl/commands/datasets.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/curation/formatters.py` & `eotdl-2023.7.19.post3/eotdl/curation/formatters.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/curation/metadata.py` & `eotdl-2023.7.19.post3/eotdl/curation/metadata.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/curation/stac/dataframe.py` & `eotdl-2023.7.19.post3/eotdl/curation/stac/dataframe.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/curation/stac/dataframe_bck.py` & `eotdl-2023.7.19.post3/eotdl/curation/stac/dataframe_bck.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/curation/stac/extensions.py` & `eotdl-2023.7.19.post3/eotdl/curation/stac/extensions.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/curation/stac/parsers.py` & `eotdl-2023.7.19.post3/eotdl/curation/stac/parsers.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/curation/stac/stac.py` & `eotdl-2023.7.19.post3/eotdl/curation/stac/stac.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/curation/stac/utils.py` & `eotdl-2023.7.19.post3/eotdl/curation/stac/utils.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/datasets/ingest.py` & `eotdl-2023.7.19.post3/eotdl/datasets/ingest.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/datasets/retrieve.py` & `eotdl-2023.7.19.post3/eotdl/datasets/retrieve.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/src/repos/APIRepo.py` & `eotdl-2023.7.19.post3/eotdl/src/repos/APIRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/src/repos/AuthRepo.py` & `eotdl-2023.7.19.post3/eotdl/src/repos/AuthRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/src/usecases/auth/Auth.py` & `eotdl-2023.7.19.post3/eotdl/src/usecases/auth/Auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/src/usecases/datasets/DownloadDataset.py` & `eotdl-2023.7.19.post3/eotdl/src/usecases/datasets/DownloadDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/src/usecases/datasets/DownloadFile.py` & `eotdl-2023.7.19.post3/eotdl/src/usecases/datasets/DownloadFile.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/src/usecases/datasets/IngestDataset.py` & `eotdl-2023.7.19.post3/eotdl/src/usecases/datasets/IngestDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/src/usecases/datasets/IngestFile.py` & `eotdl-2023.7.19.post3/eotdl/src/usecases/datasets/IngestFile.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/src/usecases/datasets/IngestFolder.py` & `eotdl-2023.7.19.post3/eotdl/src/usecases/datasets/IngestFolder.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,15 +58,14 @@
             current_files = [item["name"] for item in data["files"]]
             if len(current_files) > 0 and not inputs.force:
                 self.logger(
                     "The following files already exist and will not be uploaded (use --f to force re-upload):"
                 )
                 for item in current_files:
                     self.logger(f"{item}")
-            # TODO: delete current_files that are not in filtered_items if --delete
             hanged_files = [
                 file
                 for file in current_files
                 if file not in [item.name for item in filtered_items]
             ]
             if len(hanged_files) > 0:
                 self.logger(
@@ -79,17 +78,18 @@
                         _, error = self.repo.delete_file(
                             data["dataset_id"], item, inputs.user["id_token"]
                         )
                         if error:
                             self.logger(error)
                         else:
                             self.logger("Done")
-            filtered_items = [
-                item for item in filtered_items if item.name not in current_files
-            ]
+            if not inputs.force:
+                filtered_items = [
+                    item for item in filtered_items if item.name not in current_files
+                ]
         dataset_id = data["dataset_id"]
         # upload files
         if len(filtered_items) == 0:
             raise Exception("No files to upload")
         self.logger("The following files will be uploaded:")
         for item in filtered_items:
             self.logger(f"{item.name}")
```

### Comparing `eotdl-2023.7.19.post2/eotdl/src/usecases/datasets/IngestLargeDataset.py` & `eotdl-2023.7.19.post3/eotdl/src/usecases/datasets/IngestLargeDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/src/usecases/datasets/IngestLargeDatasetParallel.py` & `eotdl-2023.7.19.post3/eotdl/src/usecases/datasets/IngestLargeDatasetParallel.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/src/usecases/datasets/IngestSTAC.py` & `eotdl-2023.7.19.post3/eotdl/src/usecases/datasets/IngestSTAC.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/tools/sen12floods/tools.py` & `eotdl-2023.7.19.post3/eotdl/tools/sen12floods/tools.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/eotdl/tools/stac.py` & `eotdl-2023.7.19.post3/eotdl/tools/stac.py`

 * *Files identical despite different names*

### Comparing `eotdl-2023.7.19.post2/pyproject.toml` & `eotdl-2023.7.19.post3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eotdl"
-version = "2023.07.19-2"
+version = "2023.07.19-3"
 description = "Earth Observation Training Data Lab"
 authors = ["EarthPulse <it@earthpulse.es>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "eotdl"}]
 
 [tool.poetry.scripts]
```

### Comparing `eotdl-2023.7.19.post2/setup.py` & `eotdl-2023.7.19.post3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['eotdl = eotdl.cli:app']}
 
 setup_kwargs = {
     'name': 'eotdl',
-    'version': '2023.7.19.post2',
+    'version': '2023.7.19.post3',
     'description': 'Earth Observation Training Data Lab',
     'long_description': '# eotdl \n\nThis is the main library and CLI for EOTDL.\n\n',
     'author': 'EarthPulse',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `eotdl-2023.7.19.post2/PKG-INFO` & `eotdl-2023.7.19.post3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eotdl
-Version: 2023.7.19.post2
+Version: 2023.7.19.post3
 Summary: Earth Observation Training Data Lab
 License: MIT
 Author: EarthPulse
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

