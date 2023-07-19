# Comparing `tmp/xfact-0.4.65.tar.gz` & `tmp/xfact-0.4.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xfact-0.4.65.tar", last modified: Wed Jul 19 08:49:02 2023, max compression
+gzip compressed data, was "xfact-0.4.66.tar", last modified: Wed Jul 19 08:48:50 2023, max compression
```

## Comparing `xfact-0.4.65.tar` & `xfact-0.4.66.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:49:02.532488 xfact-0.4.65/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-19 08:46:26.000000 xfact-0.4.65/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-19 08:49:02.532488 xfact-0.4.65/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-19 08:46:26.000000 xfact-0.4.65/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-19 08:46:26.000000 xfact-0.4.65/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 08:49:02.532488 xfact-0.4.65/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-19 08:46:26.000000 xfact-0.4.65/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:49:02.528488 xfact-0.4.65/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:49:02.532488 xfact-0.4.65/src/xfact/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-19 08:46:26.000000 xfact-0.4.65/src/xfact/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:49:02.532488 xfact-0.4.65/src/xfact/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 08:46:26.000000 xfact-0.4.65/src/xfact/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-07-19 08:46:26.000000 xfact-0.4.65/src/xfact/config/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:49:02.532488 xfact-0.4.65/src/xfact/logs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 08:46:26.000000 xfact-0.4.65/src/xfact/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-19 08:46:26.000000 xfact-0.4.65/src/xfact/logs/comet_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-19 08:46:26.000000 xfact-0.4.65/src/xfact/logs/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:49:02.532488 xfact-0.4.65/src/xfact/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-19 08:46:26.000000 xfact-0.4.65/src/xfact/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-19 08:46:26.000000 xfact-0.4.65/src/xfact/nlp/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11644 2023-07-19 08:46:26.000000 xfact-0.4.65/src/xfact/nlp/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:49:02.532488 xfact-0.4.65/src/xfact/nlp/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 08:46:26.000000 xfact-0.4.65/src/xfact/nlp/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-19 08:46:26.000000 xfact-0.4.65/src/xfact/nlp/datasets/fever_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-19 08:46:26.000000 xfact-0.4.65/src/xfact/nlp/datasets/snli_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-19 08:46:26.000000 xfact-0.4.65/src/xfact/nlp/datasets/squad_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    15095 2023-07-19 08:46:26.000000 xfact-0.4.65/src/xfact/nlp/deardr_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:49:02.532488 xfact-0.4.65/src/xfact/nlp/inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 08:46:26.000000 xfact-0.4.65/src/xfact/nlp/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-19 08:46:26.000000 xfact-0.4.65/src/xfact/nlp/inference/prefix_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-19 08:46:26.000000 xfact-0.4.65/src/xfact/nlp/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-19 08:46:26.000000 xfact-0.4.65/src/xfact/nlp/post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-19 08:46:26.000000 xfact-0.4.65/src/xfact/nlp/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-19 08:46:26.000000 xfact-0.4.65/src/xfact/nlp/scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:49:02.532488 xfact-0.4.65/src/xfact/registry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 08:46:26.000000 xfact-0.4.65/src/xfact/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-19 08:46:26.000000 xfact-0.4.65/src/xfact/registry/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-19 08:46:26.000000 xfact-0.4.65/src/xfact/registry/registrable.py
--rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-07-19 08:46:26.000000 xfact-0.4.65/src/xfact/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:49:02.532488 xfact-0.4.65/src/xfact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-19 08:49:02.000000 xfact-0.4.65/src/xfact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-19 08:49:02.000000 xfact-0.4.65/src/xfact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 08:49:02.000000 xfact-0.4.65/src/xfact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-19 08:49:02.000000 xfact-0.4.65/src/xfact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 08:49:02.000000 xfact-0.4.65/src/xfact.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:48:50.111353 xfact-0.4.66/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-19 08:46:41.000000 xfact-0.4.66/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-19 08:48:50.111353 xfact-0.4.66/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-19 08:46:41.000000 xfact-0.4.66/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-19 08:46:41.000000 xfact-0.4.66/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 08:48:50.111353 xfact-0.4.66/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-19 08:46:42.000000 xfact-0.4.66/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:48:50.107353 xfact-0.4.66/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:48:50.107353 xfact-0.4.66/src/xfact/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-19 08:46:41.000000 xfact-0.4.66/src/xfact/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:48:50.111353 xfact-0.4.66/src/xfact/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 08:46:41.000000 xfact-0.4.66/src/xfact/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-07-19 08:46:41.000000 xfact-0.4.66/src/xfact/config/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:48:50.111353 xfact-0.4.66/src/xfact/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 08:46:41.000000 xfact-0.4.66/src/xfact/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-19 08:46:41.000000 xfact-0.4.66/src/xfact/logs/comet_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-19 08:46:41.000000 xfact-0.4.66/src/xfact/logs/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:48:50.111353 xfact-0.4.66/src/xfact/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-19 08:46:41.000000 xfact-0.4.66/src/xfact/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-19 08:46:41.000000 xfact-0.4.66/src/xfact/nlp/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11644 2023-07-19 08:46:41.000000 xfact-0.4.66/src/xfact/nlp/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:48:50.111353 xfact-0.4.66/src/xfact/nlp/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 08:46:41.000000 xfact-0.4.66/src/xfact/nlp/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-19 08:46:41.000000 xfact-0.4.66/src/xfact/nlp/datasets/fever_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-19 08:46:41.000000 xfact-0.4.66/src/xfact/nlp/datasets/snli_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-19 08:46:41.000000 xfact-0.4.66/src/xfact/nlp/datasets/squad_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15095 2023-07-19 08:46:41.000000 xfact-0.4.66/src/xfact/nlp/deardr_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:48:50.111353 xfact-0.4.66/src/xfact/nlp/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 08:46:41.000000 xfact-0.4.66/src/xfact/nlp/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-19 08:46:41.000000 xfact-0.4.66/src/xfact/nlp/inference/prefix_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-19 08:46:41.000000 xfact-0.4.66/src/xfact/nlp/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-19 08:46:41.000000 xfact-0.4.66/src/xfact/nlp/post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-19 08:46:41.000000 xfact-0.4.66/src/xfact/nlp/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-19 08:46:41.000000 xfact-0.4.66/src/xfact/nlp/scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:48:50.111353 xfact-0.4.66/src/xfact/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 08:46:41.000000 xfact-0.4.66/src/xfact/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-19 08:46:41.000000 xfact-0.4.66/src/xfact/registry/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-19 08:46:41.000000 xfact-0.4.66/src/xfact/registry/registrable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-07-19 08:46:41.000000 xfact-0.4.66/src/xfact/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:48:50.111353 xfact-0.4.66/src/xfact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-19 08:48:49.000000 xfact-0.4.66/src/xfact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-19 08:48:50.000000 xfact-0.4.66/src/xfact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 08:48:49.000000 xfact-0.4.66/src/xfact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-19 08:48:49.000000 xfact-0.4.66/src/xfact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 08:48:49.000000 xfact-0.4.66/src/xfact.egg-info/top_level.txt
```

### Comparing `xfact-0.4.65/README.md` & `xfact-0.4.66/README.md`

 * *Files identical despite different names*

### Comparing `xfact-0.4.65/setup.py` & `xfact-0.4.66/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 install = [req for req in reqs if not req.startswith("git+git://")]
 depends = [req.replace("git+git://", "git+http://") for req in reqs if req.startswith("git+git://")]
 
 
 setup(
     name='xfact',
-    version='0.4.65',
+    version='0.4.66',
     author='James Thorne',
     author_email='james@jamesthorne.com',
     description='xfact',
     long_description="readme",
     python_requires='>=3.8',
     packages=["xfact",
               "xfact.nlp",
```

### Comparing `xfact-0.4.65/src/xfact/config/args.py` & `xfact-0.4.66/src/xfact/config/args.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.65/src/xfact/logs/comet_callback.py` & `xfact-0.4.66/src/xfact/logs/comet_callback.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.65/src/xfact/logs/logs.py` & `xfact-0.4.66/src/xfact/logs/logs.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.65/src/xfact/nlp/data_utils.py` & `xfact-0.4.66/src/xfact/nlp/data_utils.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.65/src/xfact/nlp/dataset.py` & `xfact-0.4.66/src/xfact/nlp/dataset.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.65/src/xfact/nlp/datasets/fever_dataset.py` & `xfact-0.4.66/src/xfact/nlp/datasets/fever_dataset.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.65/src/xfact/nlp/datasets/snli_dataset.py` & `xfact-0.4.66/src/xfact/nlp/datasets/snli_dataset.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.65/src/xfact/nlp/datasets/squad_dataset.py` & `xfact-0.4.66/src/xfact/nlp/datasets/squad_dataset.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.65/src/xfact/nlp/deardr_trainer.py` & `xfact-0.4.66/src/xfact/nlp/deardr_trainer.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.65/src/xfact/nlp/inference/prefix_decoder.py` & `xfact-0.4.66/src/xfact/nlp/inference/prefix_decoder.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.65/src/xfact/nlp/model.py` & `xfact-0.4.66/src/xfact/nlp/model.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.65/src/xfact/nlp/post_processing.py` & `xfact-0.4.66/src/xfact/nlp/post_processing.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.65/src/xfact/nlp/reader.py` & `xfact-0.4.66/src/xfact/nlp/reader.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.65/src/xfact/nlp/scoring.py` & `xfact-0.4.66/src/xfact/nlp/scoring.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.65/src/xfact/registry/module.py` & `xfact-0.4.66/src/xfact/registry/module.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.65/src/xfact/registry/registrable.py` & `xfact-0.4.66/src/xfact/registry/registrable.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.65/src/xfact/train.py` & `xfact-0.4.66/src/xfact/train.py`

 * *Files identical despite different names*

### Comparing `xfact-0.4.65/src/xfact.egg-info/SOURCES.txt` & `xfact-0.4.66/src/xfact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

