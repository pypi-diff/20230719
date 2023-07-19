# Comparing `tmp/parallel_corpus_mnbvc-1.0.7.tar.gz` & `tmp/parallel_corpus_mnbvc-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parallel_corpus_mnbvc-1.0.7.tar", last modified: Wed Jul 19 09:41:23 2023, max compression
+gzip compressed data, was "parallel_corpus_mnbvc-1.0.8.tar", last modified: Wed Jul 19 10:11:00 2023, max compression
```

## Comparing `parallel_corpus_mnbvc-1.0.7.tar` & `parallel_corpus_mnbvc-1.0.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-19 09:41:23.421008 parallel_corpus_mnbvc-1.0.7/
--rw-rw-r--   0 ran       (1000) ran       (1000)    11357 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-1.0.7/LICENSE
--rw-rw-r--   0 ran       (1000) ran       (1000)       80 2023-07-18 18:04:18.000000 parallel_corpus_mnbvc-1.0.7/MANIFEST.in
--rw-rw-r--   0 ran       (1000) ran       (1000)      282 2023-07-19 09:41:23.421008 parallel_corpus_mnbvc-1.0.7/PKG-INFO
--rw-rw-r--   0 ran       (1000) ran       (1000)     1113 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-1.0.7/README.md
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-19 09:41:23.417008 parallel_corpus_mnbvc-1.0.7/alignment/
--rw-rw-r--   0 ran       (1000) ran       (1000)      281 2023-07-19 09:35:02.000000 parallel_corpus_mnbvc-1.0.7/alignment/__init__.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     6084 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.7/alignment/batch_detector.py
--rw-rw-r--   0 ran       (1000) ran       (1000)    20475 2023-07-19 09:33:49.000000 parallel_corpus_mnbvc-1.0.7/alignment/batch_sequential_detector.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     1970 2023-07-19 09:34:01.000000 parallel_corpus_mnbvc-1.0.7/alignment/batch_sequential_for_one_file.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     6775 2023-07-19 09:34:34.000000 parallel_corpus_mnbvc-1.0.7/alignment/evaluate_segmentation.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     8954 2023-07-19 09:34:44.000000 parallel_corpus_mnbvc-1.0.7/alignment/rule_based_detector.py
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-19 09:41:23.417008 parallel_corpus_mnbvc-1.0.7/alignment/script/
--rw-rw-r--   0 ran       (1000) ran       (1000)       49 2023-07-19 09:00:04.000000 parallel_corpus_mnbvc-1.0.7/alignment/script/__init__.py
--rw-rw-r--   0 ran       (1000) ran       (1000)    22157 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-1.0.7/alignment/script/gpt_helper.py
--rw-rw-r--   0 ran       (1000) ran       (1000)    13345 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.7/alignment/script/preprocess.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     6029 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-1.0.7/alignment/text_segmenter.py
--rw-rw-r--   0 ran       (1000) ran       (1000)    12285 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.7/alignment/utils.py
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-19 09:41:23.417008 parallel_corpus_mnbvc-1.0.7/download_data/
--rw-rw-r--   0 ran       (1000) ran       (1000)       79 2023-07-19 09:02:09.000000 parallel_corpus_mnbvc-1.0.7/download_data/__init__.py
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-19 09:41:23.417008 parallel_corpus_mnbvc-1.0.7/download_data/about_sitemap/
--rw-rw-r--   0 ran       (1000) ran       (1000)      125 2023-07-19 09:01:36.000000 parallel_corpus_mnbvc-1.0.7/download_data/about_sitemap/__init__.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     3437 2023-06-16 09:39:48.000000 parallel_corpus_mnbvc-1.0.7/download_data/about_sitemap/download_after_2000_year_pdf_to_loacl.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     3305 2023-06-16 09:39:48.000000 parallel_corpus_mnbvc-1.0.7/download_data/about_sitemap/download_all_pdf_url.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     4045 2023-06-16 09:39:48.000000 parallel_corpus_mnbvc-1.0.7/download_data/about_sitemap/get_pdf_link_information.py
--rw-rw-r--   0 ran       (1000) ran       (1000)    10603 2023-07-19 09:00:50.000000 parallel_corpus_mnbvc-1.0.7/download_data/download_un_corpus.py
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-19 09:41:23.417008 parallel_corpus_mnbvc-1.0.7/parallel_corpus_mnbvc.egg-info/
--rw-rw-r--   0 ran       (1000) ran       (1000)      282 2023-07-19 09:41:23.000000 parallel_corpus_mnbvc-1.0.7/parallel_corpus_mnbvc.egg-info/PKG-INFO
--rw-rw-r--   0 ran       (1000) ran       (1000)      921 2023-07-19 09:41:23.000000 parallel_corpus_mnbvc-1.0.7/parallel_corpus_mnbvc.egg-info/SOURCES.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)        1 2023-07-19 09:41:23.000000 parallel_corpus_mnbvc-1.0.7/parallel_corpus_mnbvc.egg-info/dependency_links.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       89 2023-07-19 09:41:23.000000 parallel_corpus_mnbvc-1.0.7/parallel_corpus_mnbvc.egg-info/requires.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       46 2023-07-19 09:41:23.000000 parallel_corpus_mnbvc-1.0.7/parallel_corpus_mnbvc.egg-info/top_level.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       37 2023-07-19 09:07:23.000000 parallel_corpus_mnbvc-1.0.7/parallel_corpus_mnbvc.py
--rw-rw-r--   0 ran       (1000) ran       (1000)       90 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.7/requirements.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       38 2023-07-19 09:41:23.421008 parallel_corpus_mnbvc-1.0.7/setup.cfg
--rw-rw-r--   0 ran       (1000) ran       (1000)      614 2023-07-19 09:39:41.000000 parallel_corpus_mnbvc-1.0.7/setup.py
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-19 10:11:00.143246 parallel_corpus_mnbvc-1.0.8/
+-rw-rw-r--   0 ran       (1000) ran       (1000)    11357 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-1.0.8/LICENSE
+-rw-rw-r--   0 ran       (1000) ran       (1000)       80 2023-07-18 18:04:18.000000 parallel_corpus_mnbvc-1.0.8/MANIFEST.in
+-rw-rw-r--   0 ran       (1000) ran       (1000)      288 2023-07-19 10:11:00.143246 parallel_corpus_mnbvc-1.0.8/PKG-INFO
+-rw-rw-r--   0 ran       (1000) ran       (1000)     1175 2023-07-19 10:00:18.000000 parallel_corpus_mnbvc-1.0.8/README.md
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-19 10:11:00.139245 parallel_corpus_mnbvc-1.0.8/alignment/
+-rw-rw-r--   0 ran       (1000) ran       (1000)      281 2023-07-19 09:35:02.000000 parallel_corpus_mnbvc-1.0.8/alignment/__init__.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     6084 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.8/alignment/batch_detector.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)    20475 2023-07-19 09:33:49.000000 parallel_corpus_mnbvc-1.0.8/alignment/batch_sequential_detector.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     1970 2023-07-19 09:34:01.000000 parallel_corpus_mnbvc-1.0.8/alignment/batch_sequential_for_one_file.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     6775 2023-07-19 09:34:34.000000 parallel_corpus_mnbvc-1.0.8/alignment/evaluate_segmentation.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     8954 2023-07-19 09:34:44.000000 parallel_corpus_mnbvc-1.0.8/alignment/rule_based_detector.py
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-19 10:11:00.143246 parallel_corpus_mnbvc-1.0.8/alignment/script/
+-rw-rw-r--   0 ran       (1000) ran       (1000)       49 2023-07-19 09:00:04.000000 parallel_corpus_mnbvc-1.0.8/alignment/script/__init__.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)    22157 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-1.0.8/alignment/script/gpt_helper.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)    13345 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.8/alignment/script/preprocess.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     6029 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-1.0.8/alignment/text_segmenter.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)    12285 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.8/alignment/utils.py
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-19 10:11:00.143246 parallel_corpus_mnbvc-1.0.8/download_data/
+-rw-rw-r--   0 ran       (1000) ran       (1000)       79 2023-07-19 09:02:09.000000 parallel_corpus_mnbvc-1.0.8/download_data/__init__.py
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-19 10:11:00.143246 parallel_corpus_mnbvc-1.0.8/download_data/about_sitemap/
+-rw-rw-r--   0 ran       (1000) ran       (1000)      125 2023-07-19 09:01:36.000000 parallel_corpus_mnbvc-1.0.8/download_data/about_sitemap/__init__.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     3437 2023-06-16 09:39:48.000000 parallel_corpus_mnbvc-1.0.8/download_data/about_sitemap/download_after_2000_year_pdf_to_loacl.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     3305 2023-06-16 09:39:48.000000 parallel_corpus_mnbvc-1.0.8/download_data/about_sitemap/download_all_pdf_url.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     4045 2023-06-16 09:39:48.000000 parallel_corpus_mnbvc-1.0.8/download_data/about_sitemap/get_pdf_link_information.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)    10603 2023-07-19 09:00:50.000000 parallel_corpus_mnbvc-1.0.8/download_data/download_un_corpus.py
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-19 10:11:00.143246 parallel_corpus_mnbvc-1.0.8/parallel_corpus_mnbvc.egg-info/
+-rw-rw-r--   0 ran       (1000) ran       (1000)      288 2023-07-19 10:11:00.000000 parallel_corpus_mnbvc-1.0.8/parallel_corpus_mnbvc.egg-info/PKG-INFO
+-rw-rw-r--   0 ran       (1000) ran       (1000)      921 2023-07-19 10:11:00.000000 parallel_corpus_mnbvc-1.0.8/parallel_corpus_mnbvc.egg-info/SOURCES.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)        1 2023-07-19 10:11:00.000000 parallel_corpus_mnbvc-1.0.8/parallel_corpus_mnbvc.egg-info/dependency_links.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       89 2023-07-19 10:11:00.000000 parallel_corpus_mnbvc-1.0.8/parallel_corpus_mnbvc.egg-info/requires.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       46 2023-07-19 10:11:00.000000 parallel_corpus_mnbvc-1.0.8/parallel_corpus_mnbvc.egg-info/top_level.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       37 2023-07-19 09:07:23.000000 parallel_corpus_mnbvc-1.0.8/parallel_corpus_mnbvc.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)       90 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.8/requirements.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       38 2023-07-19 10:11:00.143246 parallel_corpus_mnbvc-1.0.8/setup.cfg
+-rw-rw-r--   0 ran       (1000) ran       (1000)      625 2023-07-19 10:10:22.000000 parallel_corpus_mnbvc-1.0.8/setup.py
```

### Comparing `parallel_corpus_mnbvc-1.0.7/LICENSE` & `parallel_corpus_mnbvc-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.7/README.md` & `parallel_corpus_mnbvc-1.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 parallel corpus dataset from the mnbvc project
 
 # Install the requirements
 ```
 pip install -r requirements.txt
 ```
 
+# Install the repository
+
+[参考](./setup.md#install-title)
+
 
 ### 输出的jsonl格式说明
 
 对于每一个文件，他的json结构层次如下：
 
 ```python
 {
```

### Comparing `parallel_corpus_mnbvc-1.0.7/alignment/batch_detector.py` & `parallel_corpus_mnbvc-1.0.8/alignment/batch_detector.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.7/alignment/batch_sequential_detector.py` & `parallel_corpus_mnbvc-1.0.8/alignment/batch_sequential_detector.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.7/alignment/batch_sequential_for_one_file.py` & `parallel_corpus_mnbvc-1.0.8/alignment/batch_sequential_for_one_file.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.7/alignment/evaluate_segmentation.py` & `parallel_corpus_mnbvc-1.0.8/alignment/evaluate_segmentation.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.7/alignment/rule_based_detector.py` & `parallel_corpus_mnbvc-1.0.8/alignment/rule_based_detector.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.7/alignment/script/gpt_helper.py` & `parallel_corpus_mnbvc-1.0.8/alignment/script/gpt_helper.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.7/alignment/script/preprocess.py` & `parallel_corpus_mnbvc-1.0.8/alignment/script/preprocess.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.7/alignment/text_segmenter.py` & `parallel_corpus_mnbvc-1.0.8/alignment/text_segmenter.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.7/alignment/utils.py` & `parallel_corpus_mnbvc-1.0.8/alignment/utils.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.7/download_data/about_sitemap/download_after_2000_year_pdf_to_loacl.py` & `parallel_corpus_mnbvc-1.0.8/download_data/about_sitemap/download_after_2000_year_pdf_to_loacl.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.7/download_data/about_sitemap/download_all_pdf_url.py` & `parallel_corpus_mnbvc-1.0.8/download_data/about_sitemap/download_all_pdf_url.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.7/download_data/about_sitemap/get_pdf_link_information.py` & `parallel_corpus_mnbvc-1.0.8/download_data/about_sitemap/get_pdf_link_information.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.7/download_data/download_un_corpus.py` & `parallel_corpus_mnbvc-1.0.8/download_data/download_un_corpus.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.7/parallel_corpus_mnbvc.egg-info/SOURCES.txt` & `parallel_corpus_mnbvc-1.0.8/parallel_corpus_mnbvc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

