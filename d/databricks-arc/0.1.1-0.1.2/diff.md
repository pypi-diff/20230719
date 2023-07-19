# Comparing `tmp/databricks-arc-0.1.1.tar.gz` & `tmp/databricks-arc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks-arc-0.1.1.tar", last modified: Tue Apr 18 19:20:19 2023, max compression
+gzip compressed data, was "databricks-arc-0.1.2.tar", last modified: Wed Jul 19 13:30:02 2023, max compression
```

## Comparing `databricks-arc-0.1.1.tar` & `databricks-arc-0.1.2.tar`

### file list

```diff
@@ -1,37 +1,35 @@
-drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-04-18 19:20:19.008158 databricks-arc-0.1.1/
--rw-r--r--   0 milos.colic   (502) staff       (20)      616 2023-04-18 19:20:19.008400 databricks-arc-0.1.1/PKG-INFO
--rw-r--r--   0 milos.colic   (502) staff       (20)       12 2023-03-06 17:23:57.000000 databricks-arc-0.1.1/README.md
-drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-04-18 19:20:18.956431 databricks-arc-0.1.1/arc/
--rw-r--r--   0 milos.colic   (502) staff       (20)       51 2023-04-18 19:17:37.000000 databricks-arc-0.1.1/arc/__init__.py
-drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-04-18 19:20:18.960488 databricks-arc-0.1.1/arc/autolinker/
--rw-r--r--   0 milos.colic   (502) staff       (20)       55 2023-03-21 16:51:08.000000 databricks-arc-0.1.1/arc/autolinker/__init__.py
--rw-r--r--   0 milos.colic   (502) staff       (20)    37669 2023-04-14 16:24:50.000000 databricks-arc-0.1.1/arc/autolinker/autolinker.py
--rw-r--r--   0 milos.colic   (502) staff       (20)    12472 2023-03-18 11:32:06.000000 databricks-arc-0.1.1/arc/autolinker/splink_mlflow.py
-drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-04-18 19:20:18.988706 databricks-arc-0.1.1/arc/lib/
--rw-r--r--   0 milos.colic   (502) staff       (20)        0 2023-03-16 14:35:13.000000 databricks-arc-0.1.1/arc/lib/__init__.py
--rw-r--r--   0 milos.colic   (502) staff       (20)  5327450 2023-04-18 19:10:13.000000 databricks-arc-0.1.1/arc/lib/arc-0.0.1-jar-with-dependencies.jar
--rw-r--r--   0 milos.colic   (502) staff       (20)   104860 2023-04-18 19:10:13.000000 databricks-arc-0.1.1/arc/lib/arc-0.0.1.jar
--rw-r--r--   0 milos.colic   (502) staff       (20)  5327451 2023-04-18 19:19:27.000000 databricks-arc-0.1.1/arc/lib/arc-0.1.1-jar-with-dependencies.jar
--rw-r--r--   0 milos.colic   (502) staff       (20)   104861 2023-04-18 19:19:27.000000 databricks-arc-0.1.1/arc/lib/arc-0.1.1.jar
-drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-04-18 19:20:18.991100 databricks-arc-0.1.1/arc/sql/
--rw-r--r--   0 milos.colic   (502) staff       (20)       50 2023-03-21 10:57:09.000000 databricks-arc-0.1.1/arc/sql/__init__.py
--rw-r--r--   0 milos.colic   (502) staff       (20)      466 2023-03-21 16:51:08.000000 databricks-arc-0.1.1/arc/sql/enable_arc.py
-drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-04-18 19:20:18.994359 databricks-arc-0.1.1/arc/sql/functions/
--rw-r--r--   0 milos.colic   (502) staff       (20)       56 2023-03-21 11:00:23.000000 databricks-arc-0.1.1/arc/sql/functions/__init__.py
--rw-r--r--   0 milos.colic   (502) staff       (20)     2663 2023-04-14 15:50:48.000000 databricks-arc-0.1.1/arc/sql/functions/functions.py
--rw-r--r--   0 milos.colic   (502) staff       (20)     3561 2023-03-21 10:51:29.000000 databricks-arc-0.1.1/arc/sql/functions/library_handler.py
-drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-04-18 19:20:19.001293 databricks-arc-0.1.1/databricks_arc.egg-info/
--rw-r--r--   0 milos.colic   (502) staff       (20)      616 2023-04-18 19:20:18.000000 databricks-arc-0.1.1/databricks_arc.egg-info/PKG-INFO
--rw-r--r--   0 milos.colic   (502) staff       (20)      727 2023-04-18 19:20:18.000000 databricks-arc-0.1.1/databricks_arc.egg-info/SOURCES.txt
--rw-r--r--   0 milos.colic   (502) staff       (20)        1 2023-04-18 19:20:18.000000 databricks-arc-0.1.1/databricks_arc.egg-info/dependency_links.txt
--rw-r--r--   0 milos.colic   (502) staff       (20)       41 2023-04-18 19:20:18.000000 databricks-arc-0.1.1/databricks_arc.egg-info/requires.txt
--rw-r--r--   0 milos.colic   (502) staff       (20)        9 2023-04-18 19:20:18.000000 databricks-arc-0.1.1/databricks_arc.egg-info/top_level.txt
--rw-r--r--   0 milos.colic   (502) staff       (20)     1184 2023-04-18 19:20:19.009712 databricks-arc-0.1.1/setup.cfg
--rw-r--r--   0 milos.colic   (502) staff       (20)      104 2023-03-06 17:23:57.000000 databricks-arc-0.1.1/setup.py
-drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-04-18 19:20:19.003054 databricks-arc-0.1.1/test/
--rw-r--r--   0 milos.colic   (502) staff       (20)        0 2023-03-06 17:23:57.000000 databricks-arc-0.1.1/test/__init__.py
--rw-r--r--   0 milos.colic   (502) staff       (20)      667 2023-04-14 15:50:48.000000 databricks-arc-0.1.1/test/test_arc_sql.py
-drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-04-18 19:20:19.006795 databricks-arc-0.1.1/test/utils/
--rw-r--r--   0 milos.colic   (502) staff       (20)       55 2023-03-16 16:33:36.000000 databricks-arc-0.1.1/test/utils/__init__.py
--rw-r--r--   0 milos.colic   (502) staff       (20)      827 2023-03-16 15:12:28.000000 databricks-arc-0.1.1/test/utils/arc_test.py
--rw-r--r--   0 milos.colic   (502) staff       (20)     1160 2023-03-18 23:48:54.000000 databricks-arc-0.1.1/test/utils/spark_test_case.py
+drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-07-19 13:30:02.744210 databricks-arc-0.1.2/
+-rw-r--r--   0 milos.colic   (502) staff       (20)      616 2023-07-19 13:30:02.744303 databricks-arc-0.1.2/PKG-INFO
+-rw-r--r--   0 milos.colic   (502) staff       (20)       12 2023-07-19 13:23:31.000000 databricks-arc-0.1.2/README.md
+drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-07-19 13:30:02.729026 databricks-arc-0.1.2/arc/
+-rw-r--r--   0 milos.colic   (502) staff       (20)       51 2023-07-19 13:28:00.000000 databricks-arc-0.1.2/arc/__init__.py
+drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-07-19 13:30:02.729875 databricks-arc-0.1.2/arc/autolinker/
+-rw-r--r--   0 milos.colic   (502) staff       (20)       55 2023-07-19 13:23:31.000000 databricks-arc-0.1.2/arc/autolinker/__init__.py
+-rw-r--r--   0 milos.colic   (502) staff       (20)    37669 2023-07-19 13:23:31.000000 databricks-arc-0.1.2/arc/autolinker/autolinker.py
+-rw-r--r--   0 milos.colic   (502) staff       (20)    12476 2023-07-19 13:23:31.000000 databricks-arc-0.1.2/arc/autolinker/splink_mlflow.py
+drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-07-19 13:30:02.734844 databricks-arc-0.1.2/arc/lib/
+-rw-r--r--   0 milos.colic   (502) staff       (20)        0 2023-07-19 13:23:31.000000 databricks-arc-0.1.2/arc/lib/__init__.py
+-rw-r--r--   0 milos.colic   (502) staff       (20)  5327405 2023-07-19 13:28:47.000000 databricks-arc-0.1.2/arc/lib/arc-0.1.2-jar-with-dependencies.jar
+-rw-r--r--   0 milos.colic   (502) staff       (20)   104782 2023-07-19 13:28:47.000000 databricks-arc-0.1.2/arc/lib/arc-0.1.2.jar
+drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-07-19 13:30:02.740027 databricks-arc-0.1.2/arc/sql/
+-rw-r--r--   0 milos.colic   (502) staff       (20)       50 2023-07-19 13:23:31.000000 databricks-arc-0.1.2/arc/sql/__init__.py
+-rw-r--r--   0 milos.colic   (502) staff       (20)      466 2023-07-19 13:23:31.000000 databricks-arc-0.1.2/arc/sql/enable_arc.py
+drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-07-19 13:30:02.741092 databricks-arc-0.1.2/arc/sql/functions/
+-rw-r--r--   0 milos.colic   (502) staff       (20)       56 2023-07-19 13:23:31.000000 databricks-arc-0.1.2/arc/sql/functions/__init__.py
+-rw-r--r--   0 milos.colic   (502) staff       (20)     2663 2023-07-19 13:23:31.000000 databricks-arc-0.1.2/arc/sql/functions/functions.py
+-rw-r--r--   0 milos.colic   (502) staff       (20)     3561 2023-07-19 13:23:31.000000 databricks-arc-0.1.2/arc/sql/functions/library_handler.py
+drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-07-19 13:30:02.742507 databricks-arc-0.1.2/databricks_arc.egg-info/
+-rw-r--r--   0 milos.colic   (502) staff       (20)      616 2023-07-19 13:30:02.000000 databricks-arc-0.1.2/databricks_arc.egg-info/PKG-INFO
+-rw-r--r--   0 milos.colic   (502) staff       (20)      661 2023-07-19 13:30:02.000000 databricks-arc-0.1.2/databricks_arc.egg-info/SOURCES.txt
+-rw-r--r--   0 milos.colic   (502) staff       (20)        1 2023-07-19 13:30:02.000000 databricks-arc-0.1.2/databricks_arc.egg-info/dependency_links.txt
+-rw-r--r--   0 milos.colic   (502) staff       (20)       41 2023-07-19 13:30:02.000000 databricks-arc-0.1.2/databricks_arc.egg-info/requires.txt
+-rw-r--r--   0 milos.colic   (502) staff       (20)        9 2023-07-19 13:30:02.000000 databricks-arc-0.1.2/databricks_arc.egg-info/top_level.txt
+-rw-r--r--   0 milos.colic   (502) staff       (20)     1184 2023-07-19 13:30:02.744785 databricks-arc-0.1.2/setup.cfg
+-rw-r--r--   0 milos.colic   (502) staff       (20)      104 2023-07-19 13:23:31.000000 databricks-arc-0.1.2/setup.py
+drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-07-19 13:30:02.743003 databricks-arc-0.1.2/test/
+-rw-r--r--   0 milos.colic   (502) staff       (20)        0 2023-07-19 13:23:31.000000 databricks-arc-0.1.2/test/__init__.py
+-rw-r--r--   0 milos.colic   (502) staff       (20)      667 2023-07-19 13:23:31.000000 databricks-arc-0.1.2/test/test_arc_sql.py
+drwxr-xr-x   0 milos.colic   (502) staff       (20)        0 2023-07-19 13:30:02.743874 databricks-arc-0.1.2/test/utils/
+-rw-r--r--   0 milos.colic   (502) staff       (20)       55 2023-07-19 13:23:31.000000 databricks-arc-0.1.2/test/utils/__init__.py
+-rw-r--r--   0 milos.colic   (502) staff       (20)      827 2023-07-19 13:23:31.000000 databricks-arc-0.1.2/test/utils/arc_test.py
+-rw-r--r--   0 milos.colic   (502) staff       (20)     1160 2023-07-19 13:23:31.000000 databricks-arc-0.1.2/test/utils/spark_test_case.py
```

### Comparing `databricks-arc-0.1.1/PKG-INFO` & `databricks-arc-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-arc
-Version: 0.1.1
+Version: 0.1.2
 Summary: ARC: data linking solution for Databricks with Splink
 Home-page: https://github.com/databricks-industry-solutions/splink-public-sector-hackathon
 Author: Databricks
 License: Databricks License
 Classifier: License :: Other/Proprietary License
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Programming Language :: Python
```

### Comparing `databricks-arc-0.1.1/arc/autolinker/autolinker.py` & `databricks-arc-0.1.2/arc/autolinker/autolinker.py`

 * *Files identical despite different names*

### Comparing `databricks-arc-0.1.1/arc/autolinker/splink_mlflow.py` & `databricks-arc-0.1.2/arc/autolinker/splink_mlflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,16 +159,16 @@
     _log_splink_model_json(splink_model_json)
     _log_hyperparameters(splink_model_json)
     #_log_comparisons(splink_model_json)
     #_save_splink_model_to_mlflow(linker, model_name)
     model = SplinkMLFlowWrapper()
     model.set_spark_linker(linker)
     mlflow.pyfunc.log_model(model_name, python_model=model)
-    if log_profiling_charts or log_parameters_charts:
-        _log_linker_charts(linker, log_parameters_charts, log_profiling_charts)
+    # if log_profiling_charts or log_parameters_charts:
+        # _log_linker_charts(linker, log_parameters_charts, log_profiling_charts)
     if params:
         mlflow.log_params(params)
     if metrics:
         mlflow.log_metrics(metrics)
     if artifacts:
         mlflow.log_artifacts(artifacts)
```

### Comparing `databricks-arc-0.1.1/arc/lib/arc-0.0.1-jar-with-dependencies.jar` & `databricks-arc-0.1.2/arc/lib/arc-0.1.2-jar-with-dependencies.jar`

 * *Files 1% similar despite different names*

#### zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5327450 bytes, number of entries: 2594
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 META-INF/
--rw-r--r--  2.0 unx       60 b- defN 23-Apr-18 20:09 META-INF/MANIFEST.MF
+Zip file size: 5327405 bytes, number of entries: 2594
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 META-INF/
+-rw-r--r--  2.0 unx       60 b- defN 23-Jul-19 14:28 META-INF/MANIFEST.MF
 drwxr-xr-x  2.0 unx        0 b- stor 19-Sep-10 21:11 scala/
 drwxr-xr-x  2.0 unx        0 b- stor 19-Sep-10 21:11 scala/annotation/
 drwxr-xr-x  2.0 unx        0 b- stor 19-Sep-10 21:11 scala/annotation/meta/
 drwxr-xr-x  2.0 unx        0 b- stor 19-Sep-10 21:11 scala/annotation/unchecked/
 drwxr-xr-x  2.0 unx        0 b- stor 19-Sep-10 21:11 scala/beans/
 drwxr-xr-x  2.0 unx        0 b- stor 19-Sep-10 21:11 scala/collection/
 drwxr-xr-x  2.0 unx        0 b- stor 19-Sep-10 21:11 scala/collection/concurrent/
@@ -32,29 +32,29 @@
 drwxr-xr-x  2.0 unx        0 b- stor 19-Sep-10 21:11 scala/sys/
 drwxr-xr-x  2.0 unx        0 b- stor 19-Sep-10 21:11 scala/sys/process/
 drwxr-xr-x  2.0 unx        0 b- stor 19-Sep-10 21:11 scala/text/
 drwxr-xr-x  2.0 unx        0 b- stor 19-Sep-10 21:11 scala/util/
 drwxr-xr-x  2.0 unx        0 b- stor 19-Sep-10 21:11 scala/util/control/
 drwxr-xr-x  2.0 unx        0 b- stor 19-Sep-10 21:11 scala/util/hashing/
 drwxr-xr-x  2.0 unx        0 b- stor 19-Sep-10 21:11 scala/util/matching/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 org/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 org/apache/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 org/apache/spark/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 org/apache/spark/sql/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 org/apache/spark/sql/adapters/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 com/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 com/databricks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 com/databricks/industry/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 com/databricks/industry/solutions/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 com/databricks/industry/solutions/arc/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/base/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 META-INF/maven/com.databricks.industry.solutions/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 META-INF/maven/com.databricks.industry.solutions/arc/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 org/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 org/apache/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 org/apache/spark/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 org/apache/spark/sql/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 org/apache/spark/sql/adapters/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 com/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 com/databricks/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 com/databricks/industry/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 com/databricks/industry/solutions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 com/databricks/industry/solutions/arc/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/base/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 META-INF/maven/com.databricks.industry.solutions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 META-INF/maven/com.databricks.industry.solutions/arc/
 -rw-r--r--  2.0 unx    11357 b- defN 19-Sep-10 20:58 LICENSE
 -rw-r--r--  2.0 unx      646 b- defN 19-Sep-10 20:58 NOTICE
 -rw-r--r--  2.0 unx      385 b- defN 19-Sep-10 21:09 library.properties
 -rw-r--r--  2.0 unx     3898 b- defN 19-Sep-10 20:58 rootdoc.txt
 -rw-r--r--  2.0 unx      658 b- defN 19-Sep-10 21:11 scala/AnyVal.class
 -rw-r--r--  2.0 unx      384 b- defN 19-Sep-10 21:11 scala/AnyValCompanion.class
 -rw-r--r--  2.0 unx     5263 b- defN 19-Sep-10 21:11 scala/App.class
@@ -2555,42 +2555,42 @@
 -rw-r--r--  2.0 unx     1563 b- defN 19-Sep-10 21:11 scala/util/matching/Regex$MatchIterator$$anon$3.class
 -rw-r--r--  2.0 unx     2666 b- defN 19-Sep-10 21:11 scala/util/matching/Regex$MatchIterator$$anon$4.class
 -rw-r--r--  2.0 unx     6501 b- defN 19-Sep-10 21:11 scala/util/matching/Regex$MatchIterator.class
 -rw-r--r--  2.0 unx     1875 b- defN 19-Sep-10 21:11 scala/util/matching/Regex$Replacement.class
 -rw-r--r--  2.0 unx    15190 b- defN 19-Sep-10 21:11 scala/util/matching/Regex.class
 -rw-r--r--  2.0 unx     1478 b- defN 19-Sep-10 21:11 scala/util/matching/UnanchoredRegex.class
 -rw-r--r--  2.0 unx      637 b- defN 19-Sep-10 21:11 scala/volatile.class
--rw-r--r--  2.0 unx      800 b- defN 23-Apr-18 20:09 org/apache/spark/sql/adapters/Column.class
--rw-r--r--  2.0 unx      811 b- defN 23-Apr-18 20:09 org/apache/spark/sql/adapters/Column$.class
--rw-r--r--  2.0 unx     2609 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/ARC.class
--rw-r--r--  2.0 unx     3448 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/ARC$$typecreator5$1.class
--rw-r--r--  2.0 unx     4911 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/functions.class
--rw-r--r--  2.0 unx     3445 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/ARC$$typecreator1$1.class
--rw-r--r--  2.0 unx    11679 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/ARC$.class
--rw-r--r--  2.0 unx     3204 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_MergeCountMapAgg$.class
--rw-r--r--  2.0 unx    23909 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_EntropyAggExpression.class
--rw-r--r--  2.0 unx     3206 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_EstimateSquaredCountOR$.class
--rw-r--r--  2.0 unx     3158 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_GeneratePartialCombinations$.class
--rw-r--r--  2.0 unx    10831 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_ToSplinkRule.class
--rw-r--r--  2.0 unx     6401 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_Combinations$.class
--rw-r--r--  2.0 unx    14299 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_GenerateCombinations.class
--rw-r--r--  2.0 unx     3906 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_CombinatorialCountAgg$.class
--rw-r--r--  2.0 unx    13817 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_EstimateSquaredCountOR.class
--rw-r--r--  2.0 unx     2293 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_ToSplinkRule$.class
--rw-r--r--  2.0 unx     3826 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_GenerateCombinations$.class
--rw-r--r--  2.0 unx    20236 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_CombinatorialCountAgg.class
--rw-r--r--  2.0 unx     8978 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_Combinations.class
--rw-r--r--  2.0 unx    13472 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_MergeCountMapAgg.class
--rw-r--r--  2.0 unx     8027 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/base/EntropyCountNestedList.class
--rw-r--r--  2.0 unx     3939 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/base/EntropyCountNestedList$.class
--rw-r--r--  2.0 unx     4776 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/base/EntropyCountAccumulatorMap$.class
--rw-r--r--  2.0 unx     1772 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/base/Utils.class
--rw-r--r--  2.0 unx     5850 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/base/CountAccumulatorMap$.class
--rw-r--r--  2.0 unx     5448 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/base/Utils$.class
--rw-r--r--  2.0 unx     6750 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/base/EntropyCountAccumulatorMap.class
--rw-r--r--  2.0 unx     9856 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/base/CountAccumulatorMap.class
--rw-r--r--  2.0 unx     3742 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_EntropyAggExpression$.class
--rw-r--r--  2.0 unx    17902 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_GeneratePartialCombinations.class
--rw-r--r--  2.0 unx    10435 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/functions$.class
--rw-r--r--  2.0 unx    10008 b- defN 23-Mar-18 11:47 META-INF/maven/com.databricks.industry.solutions/arc/pom.xml
--rw-r--r--  2.0 unx      121 b- defN 23-Apr-18 20:09 META-INF/maven/com.databricks.industry.solutions/arc/pom.properties
-2594 files, 14144009 bytes uncompressed, 4913090 bytes compressed:  65.3%
+-rw-r--r--  2.0 unx      800 b- defN 23-Jul-19 14:28 org/apache/spark/sql/adapters/Column.class
+-rw-r--r--  2.0 unx      811 b- defN 23-Jul-19 14:28 org/apache/spark/sql/adapters/Column$.class
+-rw-r--r--  2.0 unx     2609 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/ARC.class
+-rw-r--r--  2.0 unx     3448 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/ARC$$typecreator5$1.class
+-rw-r--r--  2.0 unx     4911 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/functions.class
+-rw-r--r--  2.0 unx     3445 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/ARC$$typecreator1$1.class
+-rw-r--r--  2.0 unx    11679 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/ARC$.class
+-rw-r--r--  2.0 unx     3204 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_MergeCountMapAgg$.class
+-rw-r--r--  2.0 unx    23909 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_EntropyAggExpression.class
+-rw-r--r--  2.0 unx     3206 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_EstimateSquaredCountOR$.class
+-rw-r--r--  2.0 unx     3158 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_GeneratePartialCombinations$.class
+-rw-r--r--  2.0 unx    10831 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_ToSplinkRule.class
+-rw-r--r--  2.0 unx     6401 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_Combinations$.class
+-rw-r--r--  2.0 unx    14299 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_GenerateCombinations.class
+-rw-r--r--  2.0 unx     3906 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_CombinatorialCountAgg$.class
+-rw-r--r--  2.0 unx    13817 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_EstimateSquaredCountOR.class
+-rw-r--r--  2.0 unx     2293 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_ToSplinkRule$.class
+-rw-r--r--  2.0 unx     3826 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_GenerateCombinations$.class
+-rw-r--r--  2.0 unx    20236 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_CombinatorialCountAgg.class
+-rw-r--r--  2.0 unx     8978 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_Combinations.class
+-rw-r--r--  2.0 unx    13472 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_MergeCountMapAgg.class
+-rw-r--r--  2.0 unx     8027 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/base/EntropyCountNestedList.class
+-rw-r--r--  2.0 unx     3939 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/base/EntropyCountNestedList$.class
+-rw-r--r--  2.0 unx     4776 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/base/EntropyCountAccumulatorMap$.class
+-rw-r--r--  2.0 unx     1772 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/base/Utils.class
+-rw-r--r--  2.0 unx     5850 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/base/CountAccumulatorMap$.class
+-rw-r--r--  2.0 unx     5448 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/base/Utils$.class
+-rw-r--r--  2.0 unx     6750 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/base/EntropyCountAccumulatorMap.class
+-rw-r--r--  2.0 unx     9856 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/base/CountAccumulatorMap.class
+-rw-r--r--  2.0 unx     3742 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_EntropyAggExpression$.class
+-rw-r--r--  2.0 unx    17902 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_GeneratePartialCombinations.class
+-rw-r--r--  2.0 unx    10435 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/functions$.class
+-rw-r--r--  2.0 unx    10008 b- defN 23-Jul-19 14:27 META-INF/maven/com.databricks.industry.solutions/arc/pom.xml
+-rw-r--r--  2.0 unx       71 b- defN 23-Jul-19 14:28 META-INF/maven/com.databricks.industry.solutions/arc/pom.properties
+2594 files, 14143959 bytes uncompressed, 4913045 bytes compressed:  65.3%
```

#### META-INF/maven/com.databricks.industry.solutions/arc/pom.xml

##### META-INF/maven/com.databricks.industry.solutions/arc/pom.xml

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <groupId>com.databricks.industry.solutions</groupId>
   <artifactId>arc</artifactId>
-  <version>0.0.1</version>
+  <version>0.1.2</version>
   <properties>
     <minimum.coverage>80</minimum.coverage>
     <skipTests>true</skipTests>
     <maven.compiler.source>1.11</maven.compiler.source>
     <maven.compiler.target>1.11</maven.compiler.target>
     <encoding>UTF-8</encoding>
     <spec2.version>4.2.0</spec2.version>
```

#### META-INF/maven/com.databricks.industry.solutions/arc/pom.properties

```diff
@@ -1,5 +1,3 @@
-#Generated by Maven
-#Tue Apr 18 20:09:49 BST 2023
 artifactId=arc
 groupId=com.databricks.industry.solutions
-version=0.0.1
+version=0.1.2
```

### Comparing `databricks-arc-0.1.1/arc/lib/arc-0.0.1.jar` & `databricks-arc-0.1.2/arc/lib/arc-0.1.2.jar`

 * *Files 14% similar despite different names*

#### zipinfo {}

```diff
@@ -1,53 +1,53 @@
-Zip file size: 104860 bytes, number of entries: 51
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 META-INF/
--rw-r--r--  2.0 unx      134 b- defN 23-Apr-18 20:09 META-INF/MANIFEST.MF
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 org/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 org/apache/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 org/apache/spark/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 org/apache/spark/sql/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 org/apache/spark/sql/adapters/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 com/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 com/databricks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 com/databricks/industry/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 com/databricks/industry/solutions/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 com/databricks/industry/solutions/arc/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/base/
--rw-r--r--  2.0 unx      800 b- defN 23-Apr-18 20:09 org/apache/spark/sql/adapters/Column.class
--rw-r--r--  2.0 unx      811 b- defN 23-Apr-18 20:09 org/apache/spark/sql/adapters/Column$.class
--rw-r--r--  2.0 unx     2609 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/ARC.class
--rw-r--r--  2.0 unx     3448 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/ARC$$typecreator5$1.class
--rw-r--r--  2.0 unx     4911 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/functions.class
--rw-r--r--  2.0 unx     3445 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/ARC$$typecreator1$1.class
--rw-r--r--  2.0 unx    11679 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/ARC$.class
--rw-r--r--  2.0 unx     3204 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_MergeCountMapAgg$.class
--rw-r--r--  2.0 unx    23909 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_EntropyAggExpression.class
--rw-r--r--  2.0 unx     3206 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_EstimateSquaredCountOR$.class
--rw-r--r--  2.0 unx     3158 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_GeneratePartialCombinations$.class
--rw-r--r--  2.0 unx    10831 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_ToSplinkRule.class
--rw-r--r--  2.0 unx     6401 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_Combinations$.class
--rw-r--r--  2.0 unx    14299 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_GenerateCombinations.class
--rw-r--r--  2.0 unx     3906 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_CombinatorialCountAgg$.class
--rw-r--r--  2.0 unx    13817 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_EstimateSquaredCountOR.class
--rw-r--r--  2.0 unx     2293 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_ToSplinkRule$.class
--rw-r--r--  2.0 unx     3826 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_GenerateCombinations$.class
--rw-r--r--  2.0 unx    20236 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_CombinatorialCountAgg.class
--rw-r--r--  2.0 unx     8978 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_Combinations.class
--rw-r--r--  2.0 unx    13472 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_MergeCountMapAgg.class
--rw-r--r--  2.0 unx     8027 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/base/EntropyCountNestedList.class
--rw-r--r--  2.0 unx     3939 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/base/EntropyCountNestedList$.class
--rw-r--r--  2.0 unx     4776 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/base/EntropyCountAccumulatorMap$.class
--rw-r--r--  2.0 unx     1772 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/base/Utils.class
--rw-r--r--  2.0 unx     5850 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/base/CountAccumulatorMap$.class
--rw-r--r--  2.0 unx     5448 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/base/Utils$.class
--rw-r--r--  2.0 unx     6750 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/base/EntropyCountAccumulatorMap.class
--rw-r--r--  2.0 unx     9856 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/base/CountAccumulatorMap.class
--rw-r--r--  2.0 unx     3742 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_EntropyAggExpression$.class
--rw-r--r--  2.0 unx    17902 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/expressions/ARC_GeneratePartialCombinations.class
--rw-r--r--  2.0 unx    10435 b- defN 23-Apr-18 20:09 com/databricks/industry/solutions/arc/functions$.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Apr-18 20:09 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Apr-18 20:09 META-INF/maven/com.databricks.industry.solutions/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Apr-18 20:09 META-INF/maven/com.databricks.industry.solutions/arc/
--rw-r--r--  2.0 unx    10008 b- defN 23-Mar-18 11:47 META-INF/maven/com.databricks.industry.solutions/arc/pom.xml
--rw-r--r--  2.0 unx      121 b- defN 23-Apr-18 20:09 META-INF/maven/com.databricks.industry.solutions/arc/pom.properties
-51 files, 247999 bytes uncompressed, 95176 bytes compressed:  61.6%
+Zip file size: 104782 bytes, number of entries: 51
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 META-INF/
+-rw-r--r--  2.0 unx       81 b- defN 23-Jul-19 14:28 META-INF/MANIFEST.MF
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 org/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 org/apache/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 org/apache/spark/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 org/apache/spark/sql/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 org/apache/spark/sql/adapters/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 com/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 com/databricks/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 com/databricks/industry/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 com/databricks/industry/solutions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 com/databricks/industry/solutions/arc/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/base/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 META-INF/maven/com.databricks.industry.solutions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-19 14:28 META-INF/maven/com.databricks.industry.solutions/arc/
+-rw-r--r--  2.0 unx      800 b- defN 23-Jul-19 14:28 org/apache/spark/sql/adapters/Column.class
+-rw-r--r--  2.0 unx      811 b- defN 23-Jul-19 14:28 org/apache/spark/sql/adapters/Column$.class
+-rw-r--r--  2.0 unx     2609 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/ARC.class
+-rw-r--r--  2.0 unx     3448 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/ARC$$typecreator5$1.class
+-rw-r--r--  2.0 unx     4911 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/functions.class
+-rw-r--r--  2.0 unx     3445 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/ARC$$typecreator1$1.class
+-rw-r--r--  2.0 unx    11679 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/ARC$.class
+-rw-r--r--  2.0 unx     3204 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_MergeCountMapAgg$.class
+-rw-r--r--  2.0 unx    23909 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_EntropyAggExpression.class
+-rw-r--r--  2.0 unx     3206 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_EstimateSquaredCountOR$.class
+-rw-r--r--  2.0 unx     3158 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_GeneratePartialCombinations$.class
+-rw-r--r--  2.0 unx    10831 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_ToSplinkRule.class
+-rw-r--r--  2.0 unx     6401 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_Combinations$.class
+-rw-r--r--  2.0 unx    14299 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_GenerateCombinations.class
+-rw-r--r--  2.0 unx     3906 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_CombinatorialCountAgg$.class
+-rw-r--r--  2.0 unx    13817 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_EstimateSquaredCountOR.class
+-rw-r--r--  2.0 unx     2293 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_ToSplinkRule$.class
+-rw-r--r--  2.0 unx     3826 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_GenerateCombinations$.class
+-rw-r--r--  2.0 unx    20236 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_CombinatorialCountAgg.class
+-rw-r--r--  2.0 unx     8978 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_Combinations.class
+-rw-r--r--  2.0 unx    13472 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_MergeCountMapAgg.class
+-rw-r--r--  2.0 unx     8027 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/base/EntropyCountNestedList.class
+-rw-r--r--  2.0 unx     3939 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/base/EntropyCountNestedList$.class
+-rw-r--r--  2.0 unx     4776 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/base/EntropyCountAccumulatorMap$.class
+-rw-r--r--  2.0 unx     1772 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/base/Utils.class
+-rw-r--r--  2.0 unx     5850 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/base/CountAccumulatorMap$.class
+-rw-r--r--  2.0 unx     5448 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/base/Utils$.class
+-rw-r--r--  2.0 unx     6750 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/base/EntropyCountAccumulatorMap.class
+-rw-r--r--  2.0 unx     9856 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/base/CountAccumulatorMap.class
+-rw-r--r--  2.0 unx     3742 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_EntropyAggExpression$.class
+-rw-r--r--  2.0 unx    17902 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/expressions/ARC_GeneratePartialCombinations.class
+-rw-r--r--  2.0 unx    10435 b- defN 23-Jul-19 14:28 com/databricks/industry/solutions/arc/functions$.class
+-rw-r--r--  2.0 unx    10008 b- defN 23-Jul-19 14:27 META-INF/maven/com.databricks.industry.solutions/arc/pom.xml
+-rw-r--r--  2.0 unx       71 b- defN 23-Jul-19 14:28 META-INF/maven/com.databricks.industry.solutions/arc/pom.properties
+51 files, 247896 bytes uncompressed, 95098 bytes compressed:  61.6%
```

#### zipnote «TEMP»/diffoscope__g3f1lhj_/tmpyxnsz4cf_.zip

```diff
@@ -36,14 +36,23 @@
 
 Filename: com/databricks/industry/solutions/arc/expressions/
 Comment: 
 
 Filename: com/databricks/industry/solutions/arc/expressions/base/
 Comment: 
 
+Filename: META-INF/maven/
+Comment: 
+
+Filename: META-INF/maven/com.databricks.industry.solutions/
+Comment: 
+
+Filename: META-INF/maven/com.databricks.industry.solutions/arc/
+Comment: 
+
 Filename: org/apache/spark/sql/adapters/Column.class
 Comment: 
 
 Filename: org/apache/spark/sql/adapters/Column$.class
 Comment: 
 
 Filename: com/databricks/industry/solutions/arc/ARC.class
@@ -132,23 +141,14 @@
 
 Filename: com/databricks/industry/solutions/arc/expressions/ARC_GeneratePartialCombinations.class
 Comment: 
 
 Filename: com/databricks/industry/solutions/arc/functions$.class
 Comment: 
 
-Filename: META-INF/maven/
-Comment: 
-
-Filename: META-INF/maven/com.databricks.industry.solutions/
-Comment: 
-
-Filename: META-INF/maven/com.databricks.industry.solutions/arc/
-Comment: 
-
 Filename: META-INF/maven/com.databricks.industry.solutions/arc/pom.xml
 Comment: 
 
 Filename: META-INF/maven/com.databricks.industry.solutions/arc/pom.properties
 Comment: 
 
 Zip file comment:
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,4 @@
 Manifest-Version: 1.0
-Archiver-Version: Plexus Archiver
-Created-By: Apache Maven 3.8.6
-Built-By: milos.colic
-Build-Jdk: 18.0.2
+Created-By: Maven JAR Plugin 3.3.0
+Build-Jdk-Spec: 20
```

#### META-INF/maven/com.databricks.industry.solutions/arc/pom.xml

##### META-INF/maven/com.databricks.industry.solutions/arc/pom.xml

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <groupId>com.databricks.industry.solutions</groupId>
   <artifactId>arc</artifactId>
-  <version>0.0.1</version>
+  <version>0.1.2</version>
   <properties>
     <minimum.coverage>80</minimum.coverage>
     <skipTests>true</skipTests>
     <maven.compiler.source>1.11</maven.compiler.source>
     <maven.compiler.target>1.11</maven.compiler.target>
     <encoding>UTF-8</encoding>
     <spec2.version>4.2.0</spec2.version>
```

#### META-INF/maven/com.databricks.industry.solutions/arc/pom.properties

```diff
@@ -1,5 +1,3 @@
-#Generated by Maven
-#Tue Apr 18 20:09:49 BST 2023
 artifactId=arc
 groupId=com.databricks.industry.solutions
-version=0.0.1
+version=0.1.2
```

### Comparing `databricks-arc-0.1.1/arc/sql/functions/functions.py` & `databricks-arc-0.1.2/arc/sql/functions/functions.py`

 * *Files identical despite different names*

### Comparing `databricks-arc-0.1.1/arc/sql/functions/library_handler.py` & `databricks-arc-0.1.2/arc/sql/functions/library_handler.py`

 * *Files identical despite different names*

### Comparing `databricks-arc-0.1.1/databricks_arc.egg-info/PKG-INFO` & `databricks-arc-0.1.2/databricks_arc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-arc
-Version: 0.1.1
+Version: 0.1.2
 Summary: ARC: data linking solution for Databricks with Splink
 Home-page: https://github.com/databricks-industry-solutions/splink-public-sector-hackathon
 Author: Databricks
 License: Databricks License
 Classifier: License :: Other/Proprietary License
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Programming Language :: Python
```

### Comparing `databricks-arc-0.1.1/databricks_arc.egg-info/SOURCES.txt` & `databricks-arc-0.1.2/databricks_arc.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,16 @@
 setup.cfg
 setup.py
 arc/__init__.py
 arc/autolinker/__init__.py
 arc/autolinker/autolinker.py
 arc/autolinker/splink_mlflow.py
 arc/lib/__init__.py
-arc/lib/arc-0.0.1-jar-with-dependencies.jar
-arc/lib/arc-0.0.1.jar
-arc/lib/arc-0.1.1-jar-with-dependencies.jar
-arc/lib/arc-0.1.1.jar
+arc/lib/arc-0.1.2-jar-with-dependencies.jar
+arc/lib/arc-0.1.2.jar
 arc/sql/__init__.py
 arc/sql/enable_arc.py
 arc/sql/functions/__init__.py
 arc/sql/functions/functions.py
 arc/sql/functions/library_handler.py
 databricks_arc.egg-info/PKG-INFO
 databricks_arc.egg-info/SOURCES.txt
```

### Comparing `databricks-arc-0.1.1/setup.cfg` & `databricks-arc-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `databricks-arc-0.1.1/test/test_arc_sql.py` & `databricks-arc-0.1.2/test/test_arc_sql.py`

 * *Files identical despite different names*

### Comparing `databricks-arc-0.1.1/test/utils/arc_test.py` & `databricks-arc-0.1.2/test/utils/arc_test.py`

 * *Files identical despite different names*

### Comparing `databricks-arc-0.1.1/test/utils/spark_test_case.py` & `databricks-arc-0.1.2/test/utils/spark_test_case.py`

 * *Files identical despite different names*

