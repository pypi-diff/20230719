# Comparing `tmp/genai_test_lib-1.0.2.tar.gz` & `tmp/genai_test_lib-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genai_test_lib-1.0.2.tar", last modified: Wed Jul 19 14:02:45 2023, max compression
+gzip compressed data, was "genai_test_lib-1.0.3.tar", last modified: Wed Jul 19 14:33:49 2023, max compression
```

## Comparing `genai_test_lib-1.0.2.tar` & `genai_test_lib-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-19 14:02:45.416931 genai_test_lib-1.0.2/
--rw-r--r--   0 atul       (501) staff       (20)     1065 2023-07-11 03:33:05.000000 genai_test_lib-1.0.2/LICENSE
--rw-r--r--   0 atul       (501) staff       (20)       80 2023-07-19 14:02:45.416743 genai_test_lib-1.0.2/PKG-INFO
-drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-19 14:02:45.414569 genai_test_lib-1.0.2/genai_test_lib/
--rw-r--r--   0 atul       (501) staff       (20)        0 2023-07-18 12:20:19.000000 genai_test_lib-1.0.2/genai_test_lib/__init__.py
-drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-19 14:02:45.415782 genai_test_lib-1.0.2/genai_test_lib/generate_qna/
--rw-r--r--   0 atul       (501) staff       (20)        0 2023-07-18 13:31:53.000000 genai_test_lib-1.0.2/genai_test_lib/generate_qna/__init__.py
--rw-r--r--   0 atul       (501) staff       (20)     5768 2023-07-19 14:01:49.000000 genai_test_lib-1.0.2/genai_test_lib/generate_qna/retrive_qna.py
-drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-19 14:02:45.416438 genai_test_lib-1.0.2/genai_test_lib/text_comparision/
--rw-r--r--   0 atul       (501) staff       (20)        0 2023-07-18 12:20:19.000000 genai_test_lib-1.0.2/genai_test_lib/text_comparision/__init__.py
--rw-r--r--   0 atul       (501) staff       (20)      594 2023-07-18 08:00:17.000000 genai_test_lib-1.0.2/genai_test_lib/text_comparision/output_parser.py
--rw-r--r--   0 atul       (501) staff       (20)     2189 2023-07-19 07:39:47.000000 genai_test_lib-1.0.2/genai_test_lib/text_comparision/text_compare.py
-drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-19 14:02:45.415503 genai_test_lib-1.0.2/genai_test_lib.egg-info/
--rw-r--r--   0 atul       (501) staff       (20)       80 2023-07-19 14:02:45.000000 genai_test_lib-1.0.2/genai_test_lib.egg-info/PKG-INFO
--rw-r--r--   0 atul       (501) staff       (20)      493 2023-07-19 14:02:45.000000 genai_test_lib-1.0.2/genai_test_lib.egg-info/SOURCES.txt
--rw-r--r--   0 atul       (501) staff       (20)        1 2023-07-19 14:02:45.000000 genai_test_lib-1.0.2/genai_test_lib.egg-info/dependency_links.txt
--rw-r--r--   0 atul       (501) staff       (20)        1 2023-07-19 14:02:45.000000 genai_test_lib-1.0.2/genai_test_lib.egg-info/not-zip-safe
--rw-r--r--   0 atul       (501) staff       (20)       17 2023-07-19 14:02:45.000000 genai_test_lib-1.0.2/genai_test_lib.egg-info/requires.txt
--rw-r--r--   0 atul       (501) staff       (20)       15 2023-07-19 14:02:45.000000 genai_test_lib-1.0.2/genai_test_lib.egg-info/top_level.txt
--rw-r--r--   0 atul       (501) staff       (20)       38 2023-07-19 14:02:45.416978 genai_test_lib-1.0.2/setup.cfg
--rw-r--r--   0 atul       (501) staff       (20)      238 2023-07-19 14:02:32.000000 genai_test_lib-1.0.2/setup.py
+drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-19 14:33:49.015549 genai_test_lib-1.0.3/
+-rw-r--r--   0 atul       (501) staff       (20)     1065 2023-07-11 03:33:05.000000 genai_test_lib-1.0.3/LICENSE
+-rw-r--r--   0 atul       (501) staff       (20)       80 2023-07-19 14:33:49.015351 genai_test_lib-1.0.3/PKG-INFO
+drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-19 14:33:49.012436 genai_test_lib-1.0.3/genai_test_lib/
+-rw-r--r--   0 atul       (501) staff       (20)        0 2023-07-18 12:20:19.000000 genai_test_lib-1.0.3/genai_test_lib/__init__.py
+drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-19 14:33:49.013851 genai_test_lib-1.0.3/genai_test_lib/generate_qna/
+-rw-r--r--   0 atul       (501) staff       (20)        0 2023-07-18 13:31:53.000000 genai_test_lib-1.0.3/genai_test_lib/generate_qna/__init__.py
+-rw-r--r--   0 atul       (501) staff       (20)     5811 2023-07-19 14:32:33.000000 genai_test_lib-1.0.3/genai_test_lib/generate_qna/retrive_qna.py
+drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-19 14:33:49.014998 genai_test_lib-1.0.3/genai_test_lib/text_comparision/
+-rw-r--r--   0 atul       (501) staff       (20)        0 2023-07-18 12:20:19.000000 genai_test_lib-1.0.3/genai_test_lib/text_comparision/__init__.py
+-rw-r--r--   0 atul       (501) staff       (20)      594 2023-07-18 08:00:17.000000 genai_test_lib-1.0.3/genai_test_lib/text_comparision/output_parser.py
+-rw-r--r--   0 atul       (501) staff       (20)     2189 2023-07-19 07:39:47.000000 genai_test_lib-1.0.3/genai_test_lib/text_comparision/text_compare.py
+drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-19 14:33:49.013548 genai_test_lib-1.0.3/genai_test_lib.egg-info/
+-rw-r--r--   0 atul       (501) staff       (20)       80 2023-07-19 14:33:48.000000 genai_test_lib-1.0.3/genai_test_lib.egg-info/PKG-INFO
+-rw-r--r--   0 atul       (501) staff       (20)      493 2023-07-19 14:33:49.000000 genai_test_lib-1.0.3/genai_test_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 atul       (501) staff       (20)        1 2023-07-19 14:33:48.000000 genai_test_lib-1.0.3/genai_test_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 atul       (501) staff       (20)        1 2023-07-19 14:33:48.000000 genai_test_lib-1.0.3/genai_test_lib.egg-info/not-zip-safe
+-rw-r--r--   0 atul       (501) staff       (20)       17 2023-07-19 14:33:48.000000 genai_test_lib-1.0.3/genai_test_lib.egg-info/requires.txt
+-rw-r--r--   0 atul       (501) staff       (20)       15 2023-07-19 14:33:48.000000 genai_test_lib-1.0.3/genai_test_lib.egg-info/top_level.txt
+-rw-r--r--   0 atul       (501) staff       (20)       38 2023-07-19 14:33:49.015603 genai_test_lib-1.0.3/setup.cfg
+-rw-r--r--   0 atul       (501) staff       (20)      238 2023-07-19 14:33:45.000000 genai_test_lib-1.0.3/setup.py
```

### Comparing `genai_test_lib-1.0.2/LICENSE` & `genai_test_lib-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `genai_test_lib-1.0.2/genai_test_lib/generate_qna/retrive_qna.py` & `genai_test_lib-1.0.3/genai_test_lib/generate_qna/retrive_qna.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,17 +58,17 @@
             retriever=docsearch.as_retriever(),
             return_source_documents=True,
         )
         return qa({"query": query})
 
     def create_spark_session(self, params={}):
         spark_conf = SparkConf()
-        spark_conf.setAppName("gx-test")
+        spark_conf.setAppName("gpt-test")
         spark_conf.set("spark.master", 'k8s://https://kubernetes.default.svc.cluster.local:443')
-        spark_conf.set("spark.kubernetes.namespace", "spark-operator")
+        spark_conf.set("spark.kubernetes.namespace", params.get("spark.kubernetes.namespace", "spark-operator"))
         spark_conf.set("spark.driver.bindAddress", "0.0.0.0")
         spark_conf.set("spark.driver.host", str(socket.gethostbyname(socket.gethostname())))
         spark_conf.set("spark.driver.port", "50243")
         spark_conf.set("spark.executor.memory", params.get("spark.executor.memory", "2g"))
         spark_conf.set("spark.driver.memory", params.get("spark.driver.memory", "1g"))
         spark_conf.set("spark.executor.instances", params.get("spark.executor.instances", "3"))
         spark_conf.set("spark.executor.cores", params.get("spark.executor.cores", "3"))
```

### Comparing `genai_test_lib-1.0.2/genai_test_lib/text_comparision/output_parser.py` & `genai_test_lib-1.0.3/genai_test_lib/text_comparision/output_parser.py`

 * *Files identical despite different names*

### Comparing `genai_test_lib-1.0.2/genai_test_lib/text_comparision/text_compare.py` & `genai_test_lib-1.0.3/genai_test_lib/text_comparision/text_compare.py`

 * *Files identical despite different names*

