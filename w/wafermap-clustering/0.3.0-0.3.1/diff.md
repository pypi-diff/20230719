# Comparing `tmp/wafermap-clustering-0.3.0.tar.gz` & `tmp/wafermap-clustering-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wafermap-clustering-0.3.0.tar", last modified: Tue Jun 27 15:59:43 2023, max compression
+gzip compressed data, was "wafermap-clustering-0.3.1.tar", last modified: Wed Jul 19 09:51:45 2023, max compression
```

## Comparing `wafermap-clustering-0.3.0.tar` & `wafermap-clustering-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 15:59:43.130680 wafermap-clustering-0.3.0/
--rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0      568 2023-06-27 15:59:43.126688 wafermap-clustering-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 15:59:43.131682 wafermap-clustering-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      990 2023-06-27 15:59:06.000000 wafermap-clustering-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 15:59:43.012990 wafermap-clustering-0.3.0/tests/
--rw-rw-rw-   0        0        0     8837 2023-06-27 12:35:52.000000 wafermap-clustering-0.3.0/tests/test_clustering.py
-drwxrwxrwx   0        0        0        0 2023-06-27 15:59:43.019913 wafermap-clustering-0.3.0/wafermap_clustering/
-drwxrwxrwx   0        0        0        0 2023-06-27 15:59:43.080497 wafermap-clustering-0.3.0/wafermap_clustering/configs/
--rw-rw-rw-   0        0        0     3472 2023-06-27 08:34:33.000000 wafermap-clustering-0.3.0/wafermap_clustering/configs/config.py
--rw-rw-rw-   0        0        0      913 2023-06-27 08:34:33.000000 wafermap-clustering-0.3.0/wafermap_clustering/configs/logging_config.py
-drwxrwxrwx   0        0        0        0 2023-06-27 15:59:43.094012 wafermap-clustering-0.3.0/wafermap_clustering/libs/
--rw-rw-rw-   0        0        0     5710 2023-06-27 15:58:56.000000 wafermap-clustering-0.3.0/wafermap_clustering/libs/klarf_lib.py
-drwxrwxrwx   0        0        0        0 2023-06-27 15:59:43.116482 wafermap-clustering-0.3.0/wafermap_clustering/models/
--rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.3.0/wafermap_clustering/models/clustered_defect.py
--rw-rw-rw-   0        0        0      521 2023-04-06 11:28:53.000000 wafermap-clustering-0.3.0/wafermap_clustering/models/clustering_performance.py
--rw-rw-rw-   0        0        0      854 2023-06-27 08:43:17.000000 wafermap-clustering-0.3.0/wafermap_clustering/models/clustering_result.py
--rw-rw-rw-   0        0        0     5588 2023-06-27 08:44:43.000000 wafermap-clustering-0.3.0/wafermap_clustering/wafermap_clustering.py
-drwxrwxrwx   0        0        0        0 2023-06-27 15:59:43.064984 wafermap-clustering-0.3.0/wafermap_clustering.egg-info/
--rw-rw-rw-   0        0        0      568 2023-06-27 15:59:42.000000 wafermap-clustering-0.3.0/wafermap_clustering.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      582 2023-06-27 15:59:42.000000 wafermap-clustering-0.3.0/wafermap_clustering.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 15:59:42.000000 wafermap-clustering-0.3.0/wafermap_clustering.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-06-27 15:59:42.000000 wafermap-clustering-0.3.0/wafermap_clustering.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-27 15:59:42.000000 wafermap-clustering-0.3.0/wafermap_clustering.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 09:51:45.272672 wafermap-clustering-0.3.1/
+-rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      568 2023-07-19 09:51:45.270732 wafermap-clustering-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-19 09:51:45.273460 wafermap-clustering-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      990 2023-07-19 09:51:12.000000 wafermap-clustering-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:51:45.223244 wafermap-clustering-0.3.1/tests/
+-rw-rw-rw-   0        0        0     9509 2023-07-19 09:46:50.000000 wafermap-clustering-0.3.1/tests/test_clustering.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:51:45.227244 wafermap-clustering-0.3.1/wafermap_clustering/
+drwxrwxrwx   0        0        0        0 2023-07-19 09:51:45.251235 wafermap-clustering-0.3.1/wafermap_clustering/configs/
+-rw-rw-rw-   0        0        0     3472 2023-06-27 08:34:33.000000 wafermap-clustering-0.3.1/wafermap_clustering/configs/config.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:51:45.255366 wafermap-clustering-0.3.1/wafermap_clustering/libs/
+-rw-rw-rw-   0        0        0     4479 2023-07-19 09:07:18.000000 wafermap-clustering-0.3.1/wafermap_clustering/libs/klarf_lib.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:51:45.267732 wafermap-clustering-0.3.1/wafermap_clustering/models/
+-rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.3.1/wafermap_clustering/models/clustered_defect.py
+-rw-rw-rw-   0        0        0      468 2023-07-19 09:50:06.000000 wafermap-clustering-0.3.1/wafermap_clustering/models/clustering_performance.py
+-rw-rw-rw-   0        0        0      854 2023-06-27 08:43:17.000000 wafermap-clustering-0.3.1/wafermap_clustering/models/clustering_result.py
+-rw-rw-rw-   0        0        0     5621 2023-07-19 09:43:06.000000 wafermap-clustering-0.3.1/wafermap_clustering/wafermap_clustering.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:51:45.247276 wafermap-clustering-0.3.1/wafermap_clustering.egg-info/
+-rw-rw-rw-   0        0        0      568 2023-07-19 09:51:45.000000 wafermap-clustering-0.3.1/wafermap_clustering.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2023-07-19 09:51:45.000000 wafermap-clustering-0.3.1/wafermap_clustering.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 09:51:45.000000 wafermap-clustering-0.3.1/wafermap_clustering.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-07-19 09:51:45.000000 wafermap-clustering-0.3.1/wafermap_clustering.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-19 09:51:45.000000 wafermap-clustering-0.3.1/wafermap_clustering.egg-info/top_level.txt
```

### Comparing `wafermap-clustering-0.3.0/LICENSE.txt` & `wafermap-clustering-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.0/PKG-INFO` & `wafermap-clustering-0.3.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.3.0
+Version: 0.3.1
 Summary: A project to apply clustering on wafermaps
 Home-page: https://github.com/Impro02/wafermap-clustering
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.0.tar.gz
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.1.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.3.0/setup.py` & `wafermap-clustering-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.3.0"
+version = "0.3.1"
 
 setup(
     name="wafermap-clustering",
     version=version,
     packages=[
         "wafermap_clustering",
         "wafermap_clustering.configs",
```

### Comparing `wafermap-clustering-0.3.0/tests/test_clustering.py` & `wafermap-clustering-0.3.1/tests/test_clustering.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # MODULES
+import logging
+from logging.handlers import TimedRotatingFileHandler
 from pathlib import Path
 from collections import Counter
 
 # UNITTEST
 import unittest
 
 # WAFERMAP_CLUSTERING
@@ -13,25 +15,55 @@
     KlarfFormat,
 )
 
 ASSETS_PATH: Path = Path(__file__).parent / "assets"
 ASSETS_OUPUT_PATH: Path = ASSETS_PATH / "clustering" / "output"
 
 
+def setup_logger(name: str, directory: Path):
+    logger = logging.getLogger(name=name)
+
+    if not logger.hasHandlers():
+        logger.setLevel(logging.INFO)
+
+        formatter = logging.Formatter(
+            "%(asctime)s - %(levelname)s - %(message)s", datefmt="%Y-%m-%d %H:%M:%S"
+        )
+
+        # Add a file handler to log messages to a file
+        directory.mkdir(parents=True, exist_ok=True)
+
+        time_rotating_handler = TimedRotatingFileHandler(
+            filename=directory / f"{name}.log",
+            when="midnight",
+            interval=1,
+            backupCount=10,
+        )
+        time_rotating_handler.setLevel(logging.INFO)
+        time_rotating_handler.setFormatter(formatter)
+        logger.addHandler(time_rotating_handler)
+
+    return logger
+
+
 class TestClustering(unittest.TestCase):
     def setUp(self) -> None:
         self.path_klarf_single_wafer = ASSETS_PATH / "J052SBN_8196_J052SBN-01.000"
         self.path_klarf_multi_wafers = ASSETS_PATH / "J237DTA_3236.000"
         self.path_klarf_single_wafer_large_klarf = ASSETS_PATH / "LARGE_KLARF.000"
 
         self.config = Config(
             platform="windows",
             conf_path=ASSETS_PATH / "conf" / "config.json",
         )
 
+        self.logger = setup_logger(
+            name="clustering", directory=Path(self.config.directories.logs)
+        )
+
     def assertFileEqual(self, first: Path, second: Path, ignore_rows: list[str]):
         with open(first, "r") as file1, open(second, "r") as file2:
             for line1, line2 in zip(file1, file2):
                 if any(
                     line.lower().startswith(row.lower())
                     for row in ignore_rows
                     for line in [line1, line2]
@@ -56,15 +88,15 @@
                     0: 10580,
                     1: 1670,
                 },
             }
         ]
 
         # WHEN
-        clustering = Clustering(config=self.config, autocreate_logger=True)
+        clustering = Clustering(config=self.config, logger=self.logger)
         results = clustering.apply(self.path_klarf_single_wafer)
 
         summary = [
             {
                 "result_timestamp": res.result_timestamp,
                 "lot_id": res.lot_id,
                 "step_id": res.step_id,
@@ -100,15 +132,15 @@
                     6: 4,
                     7: 3,
                 },
             }
         ]
 
         # WHEN
-        clustering = Clustering(config=self.config, autocreate_logger=True)
+        clustering = Clustering(config=self.config, logger=self.logger)
         results = clustering.apply(
             self.path_klarf_single_wafer_large_klarf,
             output_directory=ASSETS_OUPUT_PATH,
             klarf_format=KlarfFormat.FULL.value,
         )
 
         summary = [
@@ -131,15 +163,15 @@
     def test_clustering_hdbscan_single_wafer(self):
         # GIVEN
         output_path = ASSETS_OUPUT_PATH
 
         expected_clusters = [615]
 
         # WHEN
-        clustering = Clustering(config=self.config, autocreate_logger=True)
+        clustering = Clustering(config=self.config, logger=self.logger)
         results = clustering.apply(
             klarf_path=self.path_klarf_single_wafer,
             output_directory=output_path,
             klarf_format=KlarfFormat.FULL.value,
             clustering_mode=ClusteringMode.HDBSCAN.value,
         )
 
@@ -185,15 +217,15 @@
                     5: 5,
                     6: 3,
                 },
             },
         ]
 
         # WHEN
-        clustering = Clustering(config=self.config, autocreate_logger=True)
+        clustering = Clustering(config=self.config, logger=self.logger)
         results = clustering.apply(self.path_klarf_multi_wafers)
 
         summary = [
             {
                 "result_timestamp": res.result_timestamp,
                 "lot_id": res.lot_id,
                 "step_id": res.step_id,
@@ -216,15 +248,15 @@
                 ASSETS_PATH / "saved" / "klarf_baby" / "J237DTA_3236_01_dbscan.000",
                 ASSETS_PATH / "saved" / "klarf_baby" / "J237DTA_3236_02_dbscan.000",
                 ASSETS_PATH / "saved" / "klarf_baby" / "J237DTA_3236_06_dbscan.000",
             ]
         )
 
         # WHEN
-        clustering = Clustering(config=self.config, autocreate_logger=True)
+        clustering = Clustering(config=self.config, logger=self.logger)
         results = clustering.apply(
             klarf_path=self.path_klarf_multi_wafers,
             output_directory=ASSETS_OUPUT_PATH,
             klarf_format=KlarfFormat.BABY.value,
         )
         results = sorted(results, key=lambda x: x.output_filename)
 
@@ -235,32 +267,27 @@
                 saved_klarf_paths[index],
                 result.output_filename,
                 ignore_rows=["FileTimestamp"],
             )
 
     def test_clustering_dbscan_multi_wafers_with_full_klarf_returned(self):
         # GIVEN
-        saved_klarf_paths = sorted(
-            [
-                ASSETS_PATH / "saved" / "klarf_full" / "J237DTA_3236_01_dbscan.000",
-                ASSETS_PATH / "saved" / "klarf_full" / "J237DTA_3236_02_dbscan.000",
-                ASSETS_PATH / "saved" / "klarf_full" / "J237DTA_3236_06_dbscan.000",
-            ]
+        saved_klarf_path = (
+            ASSETS_PATH / "saved" / "klarf_full" / "J237DTA_3236_dbscan.000"
         )
 
         # WHEN
-        clustering = Clustering(config=self.config, autocreate_logger=True)
+        clustering = Clustering(config=self.config, logger=self.logger)
         results = clustering.apply(
             klarf_path=self.path_klarf_multi_wafers,
             output_directory=ASSETS_OUPUT_PATH,
             klarf_format=KlarfFormat.FULL.value,
         )
         results = sorted(results, key=lambda x: x.output_filename)
 
         # THEN
-        self.assertEqual(len(results), len(saved_klarf_paths))
-        for index, result in enumerate(results):
+        for result in results:
             self.assertFileEqual(
-                saved_klarf_paths[index],
+                saved_klarf_path,
                 result.output_filename,
                 ignore_rows=["FileTimestamp"],
             )
```

### Comparing `wafermap-clustering-0.3.0/wafermap_clustering/configs/config.py` & `wafermap-clustering-0.3.1/wafermap_clustering/configs/config.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.0/wafermap_clustering/models/clustering_result.py` & `wafermap-clustering-0.3.1/wafermap_clustering/models/clustering_result.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.0/wafermap_clustering/wafermap_clustering.py` & `wafermap-clustering-0.3.1/wafermap_clustering/wafermap_clustering.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,84 +23,68 @@
 from .models.clustering_result import ClusteringResult
 
 # LIBS
 from .libs import klarf_lib
 
 # CONFIGS
 from .configs.config import ClusteringMode, Config, KlarfFormat
-from .configs.logging_config import setup_logger
 
 
 class Clustering:
     def __init__(
         self,
         config: Config,
         logger: Logger = None,
-        autocreate_logger: bool = False,
     ) -> None:
         self.config = config
-        self.logger = (
-            setup_logger(
-                name="clustering",
-                directory=Path(self.config.directories.logs),
-            )
-            if autocreate_logger and logger is None
-            else logger
-        )
+        self.logger = logger
 
     def apply(
         self,
         klarf_path: Path,
         output_directory: Path = None,
         klarf_format=KlarfFormat.BABY.value,
         clustering_mode=ClusteringMode.DBSCAN.value,
     ) -> List[ClusteringResult]:
 
         klarf_content, raw_content = Klarf.load_from_file_with_raw_content(
             filepath=klarf_path
         )
 
+        match clustering_mode:
+            case ClusteringMode.DBSCAN.value:
+                clustering = DBSCAN(
+                    eps=self.config.clustering.dbscan.eps,
+                    min_samples=self.config.clustering.dbscan.min_samples,
+                )
+            case ClusteringMode.HDBSCAN.value:
+                clustering = HDBSCAN(
+                    min_samples=self.config.clustering.hdbscan.min_samples,
+                    min_cluster_size=self.config.clustering.hdbscan.min_cluster_size,
+                )
+            case _:
+                raise ValueError(f"{clustering_mode=} is not supported")
+
         results: List[ClusteringResult] = []
         for index, wafer in enumerate(klarf_content.wafers):
             tic = time.time()
 
             single_klarf = klarf_convert.convert_to_single_klarf_content(
                 klarf_content=klarf_content, wafer_index=index
             )
 
-            output_filename = (
-                (
-                    output_directory
-                    / f"{single_klarf.lot_id}_{single_klarf.step_id}_{single_klarf.wafer.id}_{clustering_mode}.000"
-                )
-                if output_directory is not None
-                else None
-            )
-
             defect_ids = np.array([defect.id for defect in wafer.defects])
             defect_points = np.array(
                 [
                     (defect.point[0] / 1000, defect.point[1] / 1000)
                     for defect in wafer.defects
                 ]
             )
 
-            match clustering_mode:
-                case ClusteringMode.DBSCAN.value:
-                    clustering = DBSCAN(
-                        eps=self.config.clustering.dbscan.eps,
-                        min_samples=self.config.clustering.dbscan.min_samples,
-                    )
-                    labels = clustering.fit_predict(defect_points)
-                case ClusteringMode.HDBSCAN.value:
-                    hdbscan = HDBSCAN(
-                        min_samples=self.config.clustering.hdbscan.min_samples,
-                        min_cluster_size=self.config.clustering.hdbscan.min_cluster_size,
-                    )
-                    labels = hdbscan.fit_predict(defect_points)
+            labels = clustering.fit_predict(defect_points)
 
             clustering_values = np.column_stack((defect_ids, labels))
             clusters = len(np.unique(labels, axis=0))
 
             clustered_defects = [
                 ClusteredDefect(
                     defect_id=defect_id,
@@ -116,42 +100,62 @@
                 result_timestamp=single_klarf.result_timestamp,
                 lot_id=single_klarf.lot_id,
                 device_id=single_klarf.device_id,
                 step_id=single_klarf.step_id,
                 wafer_id=single_klarf.wafer.id,
                 clusters=clusters,
                 clustered_defects=clustered_defects,
-                output_filename=output_filename,
+                performance=ClusteringPerformance(
+                    clustering_timestamp=round(clustering_timestamp, 3)
+                ),
             )
 
             output_timestamp = None
-            match klarf_format:
-                case KlarfFormat.BABY.value if output_directory is not None:
-                    output_timestamp = klarf_lib.write_baby_klarf(
-                        single_klarf=single_klarf,
-                        clustering_result=clustering_result,
-                        attribute=self.config.attribute,
-                        output_filename=output_filename,
-                    )
-                case KlarfFormat.FULL.value if output_directory is not None:
-                    output_timestamp = klarf_lib.write_full_klarf(
-                        single_klarf=single_klarf,
-                        clustering_result=clustering_result,
-                        attribute=self.config.attribute,
-                        output_filename=output_filename,
-                    )
-
-            clustering_result.performance = ClusteringPerformance(
-                clustering_timestamp=round(clustering_timestamp, 3),
-                output_timestamp=round(output_timestamp, 3)
-                if output_timestamp is not None
-                else None,
-            )
+            if klarf_format == KlarfFormat.BABY.value and output_directory is not None:
+                output_filename = (
+                    output_directory
+                    / f"{single_klarf.lot_id}_{single_klarf.step_id}_{single_klarf.wafer.id}_{clustering_mode}.000"
+                )
+
+                output_timestamp = klarf_lib.write_baby_klarf(
+                    single_klarf=single_klarf,
+                    clustering_result=clustering_result,
+                    attribute=self.config.attribute,
+                    output_filename=output_filename,
+                )
+
+                clustering_result.output_filename = output_filename
+                clustering_result.performance.output_timestamp = round(
+                    output_timestamp, 3
+                )
 
             results.append(clustering_result)
 
-            if self.logger is not None:
+        if klarf_format == KlarfFormat.FULL.value and output_directory is not None:
+            output_filename = (
+                output_directory
+                / f"{klarf_path.stem}_{clustering_mode}{klarf_path.suffix}"
+            )
+
+            output_timestamp = klarf_lib.write_full_klarf(
+                raw_klarf=raw_content,
+                clustering_results=results,
+                attribute=self.config.attribute,
+                output_filename=output_filename,
+            )
+
+            for clustering_result in results:
+                clustering_result.output_filename = output_filename
+                clustering_result.performance.output_timestamp = round(
+                    output_timestamp, 3
+                )
+
+        if self.logger is not None:
+            for clustering_result in results:
+                defects = len(clustering_result.clustered_defects)
+                clusters = clustering_result.clusters
+
                 self.logger.info(
-                    msg=f"({repr(clustering_result)}) was sucessfully processed [defects={len(defect_ids)}, {clusters=}] with ({repr(clustering_result.performance)}) "
+                    msg=f"({repr(clustering_result)}) was sucessfully processed [{defects=}, {clusters=}] with ({repr(clustering_result.performance)}) "
                 )
 
         return results
```

### Comparing `wafermap-clustering-0.3.0/wafermap_clustering.egg-info/PKG-INFO` & `wafermap-clustering-0.3.1/wafermap_clustering.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.3.0
+Version: 0.3.1
 Summary: A project to apply clustering on wafermaps
 Home-page: https://github.com/Impro02/wafermap-clustering
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.0.tar.gz
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.1.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.3.0/wafermap_clustering.egg-info/SOURCES.txt` & `wafermap-clustering-0.3.1/wafermap_clustering.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -5,12 +5,11 @@
 wafermap_clustering/wafermap_clustering.py
 wafermap_clustering.egg-info/PKG-INFO
 wafermap_clustering.egg-info/SOURCES.txt
 wafermap_clustering.egg-info/dependency_links.txt
 wafermap_clustering.egg-info/requires.txt
 wafermap_clustering.egg-info/top_level.txt
 wafermap_clustering/configs/config.py
-wafermap_clustering/configs/logging_config.py
 wafermap_clustering/libs/klarf_lib.py
 wafermap_clustering/models/clustered_defect.py
 wafermap_clustering/models/clustering_performance.py
 wafermap_clustering/models/clustering_result.py
```

