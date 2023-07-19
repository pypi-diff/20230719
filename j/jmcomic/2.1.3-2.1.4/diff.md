# Comparing `tmp/jmcomic-2.1.3.tar.gz` & `tmp/jmcomic-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jmcomic-2.1.3.tar", last modified: Fri Jul 14 16:20:58 2023, max compression
+gzip compressed data, was "jmcomic-2.1.4.tar", last modified: Wed Jul 19 12:54:24 2023, max compression
```

## Comparing `jmcomic-2.1.3.tar` & `jmcomic-2.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:20:58.902709 jmcomic-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-14 16:20:47.000000 jmcomic-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-14 16:20:58.902709 jmcomic-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-14 16:20:47.000000 jmcomic-2.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:20:58.902709 jmcomic-2.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-14 16:20:47.000000 jmcomic-2.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:20:58.894709 jmcomic-2.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:20:58.898709 jmcomic-2.1.3/src/jmcomic/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-14 16:20:47.000000 jmcomic-2.1.3/src/jmcomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-14 16:20:47.000000 jmcomic-2.1.3/src/jmcomic/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-07-14 16:20:47.000000 jmcomic-2.1.3/src/jmcomic/jm_client_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-07-14 16:20:47.000000 jmcomic-2.1.3/src/jmcomic/jm_client_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-14 16:20:47.000000 jmcomic-2.1.3/src/jmcomic/jm_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-07-14 16:20:47.000000 jmcomic-2.1.3/src/jmcomic/jm_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-07-14 16:20:47.000000 jmcomic-2.1.3/src/jmcomic/jm_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-07-14 16:20:47.000000 jmcomic-2.1.3/src/jmcomic/jm_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:20:58.902709 jmcomic-2.1.3/src/jmcomic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-14 16:20:58.000000 jmcomic-2.1.3/src/jmcomic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-14 16:20:58.000000 jmcomic-2.1.3/src/jmcomic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:20:58.000000 jmcomic-2.1.3/src/jmcomic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-14 16:20:58.000000 jmcomic-2.1.3/src/jmcomic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 16:20:58.000000 jmcomic-2.1.3/src/jmcomic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:54:24.424531 jmcomic-2.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-19 12:54:14.000000 jmcomic-2.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-19 12:54:24.424531 jmcomic-2.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-19 12:54:14.000000 jmcomic-2.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 12:54:24.424531 jmcomic-2.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-19 12:54:14.000000 jmcomic-2.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:54:24.420531 jmcomic-2.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:54:24.420531 jmcomic-2.1.4/src/jmcomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-19 12:54:14.000000 jmcomic-2.1.4/src/jmcomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-19 12:54:14.000000 jmcomic-2.1.4/src/jmcomic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-07-19 12:54:14.000000 jmcomic-2.1.4/src/jmcomic/jm_client_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-07-19 12:54:14.000000 jmcomic-2.1.4/src/jmcomic/jm_client_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-19 12:54:14.000000 jmcomic-2.1.4/src/jmcomic/jm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-07-19 12:54:14.000000 jmcomic-2.1.4/src/jmcomic/jm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-07-19 12:54:14.000000 jmcomic-2.1.4/src/jmcomic/jm_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-07-19 12:54:14.000000 jmcomic-2.1.4/src/jmcomic/jm_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:54:24.424531 jmcomic-2.1.4/src/jmcomic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-19 12:54:24.000000 jmcomic-2.1.4/src/jmcomic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-19 12:54:24.000000 jmcomic-2.1.4/src/jmcomic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:54:24.000000 jmcomic-2.1.4/src/jmcomic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-19 12:54:24.000000 jmcomic-2.1.4/src/jmcomic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-19 12:54:24.000000 jmcomic-2.1.4/src/jmcomic.egg-info/top_level.txt
```

### Comparing `jmcomic-2.1.3/LICENSE` & `jmcomic-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.3/PKG-INFO` & `jmcomic-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.1.3
+Version: 2.1.4
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `jmcomic-2.1.3/README.md` & `jmcomic-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.3/setup.py` & `jmcomic-2.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.3/src/jmcomic/api.py` & `jmcomic-2.1.4/src/jmcomic/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -112,28 +112,25 @@
             decode_image=decode_image,
         )
 
         jm_debug(debug_topic,
                  f'图片下载完成: {debug_tag}, [{image.img_url}] → [{img_save_path}]'
                  )
 
-    length = len(photo_detail)
-    # 根据图片数，决定下载策略
-    if length <= option.download_threading_batch_count:
-        # 如果图片数小的话，直接使用多线程下载，一张图一个线程。
+    batch = option.download_threading_batch_count
+    if batch <= 0:
         multi_thread_launcher(
             iter_objs=enumerate(photo_detail),
             apply_each_obj_func=download_image,
         )
     else:
-        # 如果图片数多的话，还是分批下载。
-        multi_task_launcher_batch(
+        thread_pool_executor(
             iter_objs=enumerate(photo_detail),
             apply_each_obj_func=download_image,
-            batch_size=option.download_threading_batch_count
+            max_workers=batch,
         )
 
 
 def build_client(option: Optional[JmOption]) -> Tuple[JmOption, JmcomicClient]:
     """
     处理option的判空，并且创建jm_client
     """
```

### Comparing `jmcomic-2.1.3/src/jmcomic/jm_client_impl.py` & `jmcomic-2.1.4/src/jmcomic/jm_client_impl.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.3/src/jmcomic/jm_client_interface.py` & `jmcomic-2.1.4/src/jmcomic/jm_client_interface.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.3/src/jmcomic/jm_config.py` & `jmcomic-2.1.4/src/jmcomic/jm_config.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.3/src/jmcomic/jm_entity.py` & `jmcomic-2.1.4/src/jmcomic/jm_entity.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.3/src/jmcomic/jm_option.py` & `jmcomic-2.1.4/src/jmcomic/jm_option.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.3/src/jmcomic/jm_toolkit.py` & `jmcomic-2.1.4/src/jmcomic/jm_toolkit.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.3/src/jmcomic.egg-info/PKG-INFO` & `jmcomic-2.1.4/src/jmcomic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.1.3
+Version: 2.1.4
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

