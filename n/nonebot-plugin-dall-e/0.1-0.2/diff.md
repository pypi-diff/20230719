# Comparing `tmp/nonebot_plugin_dall-e-0.1.tar.gz` & `tmp/nonebot_plugin_dall-e-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_dall-e-0.1.tar", last modified: Tue Jul 18 15:43:57 2023, max compression
+gzip compressed data, was "nonebot_plugin_dall-e-0.2.tar", last modified: Wed Jul 19 01:30:58 2023, max compression
```

## Comparing `nonebot_plugin_dall-e-0.1.tar` & `nonebot_plugin_dall-e-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 15:43:57.428733 nonebot_plugin_dall-e-0.1/
--rw-rw-rw-   0        0        0    11558 2023-07-18 15:29:46.000000 nonebot_plugin_dall-e-0.1/LICENSE
--rw-rw-rw-   0        0        0      367 2023-07-18 15:43:57.428733 nonebot_plugin_dall-e-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2487 2023-07-18 15:09:46.000000 nonebot_plugin_dall-e-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 15:43:57.422328 nonebot_plugin_dall-e-0.1/nonebot_plugin_dall-e/
--rw-rw-rw-   0        0        0     5609 2023-07-18 14:47:40.000000 nonebot_plugin_dall-e-0.1/nonebot_plugin_dall-e/__init__.py
--rw-rw-rw-   0        0        0     3733 2023-07-18 14:47:40.000000 nonebot_plugin_dall-e-0.1/nonebot_plugin_dall-e/openai.py
--rw-rw-rw-   0        0        0     2733 2023-07-18 14:58:37.000000 nonebot_plugin_dall-e-0.1/nonebot_plugin_dall-e/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-18 15:43:57.427712 nonebot_plugin_dall-e-0.1/nonebot_plugin_dall_e.egg-info/
--rw-rw-rw-   0        0        0      367 2023-07-18 15:43:57.000000 nonebot_plugin_dall-e-0.1/nonebot_plugin_dall_e.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2023-07-18 15:43:57.000000 nonebot_plugin_dall-e-0.1/nonebot_plugin_dall_e.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 15:43:57.000000 nonebot_plugin_dall-e-0.1/nonebot_plugin_dall_e.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-07-18 15:43:57.000000 nonebot_plugin_dall-e-0.1/nonebot_plugin_dall_e.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-18 15:43:57.000000 nonebot_plugin_dall-e-0.1/nonebot_plugin_dall_e.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 15:43:57.428733 nonebot_plugin_dall-e-0.1/setup.cfg
--rw-rw-rw-   0        0        0      733 2023-07-18 15:42:39.000000 nonebot_plugin_dall-e-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 01:30:58.095930 nonebot_plugin_dall-e-0.2/
+-rw-rw-rw-   0        0        0    11558 2023-07-18 15:29:46.000000 nonebot_plugin_dall-e-0.2/LICENSE
+-rw-rw-rw-   0        0        0      367 2023-07-19 01:30:58.095930 nonebot_plugin_dall-e-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2487 2023-07-18 15:09:46.000000 nonebot_plugin_dall-e-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 01:30:58.083205 nonebot_plugin_dall-e-0.2/nonebot_plugin_dall-e/
+-rw-rw-rw-   0        0        0     5609 2023-07-18 14:47:40.000000 nonebot_plugin_dall-e-0.2/nonebot_plugin_dall-e/__init__.py
+-rw-rw-rw-   0        0        0     3733 2023-07-18 14:47:40.000000 nonebot_plugin_dall-e-0.2/nonebot_plugin_dall-e/openai.py
+-rw-rw-rw-   0        0        0     2733 2023-07-18 14:58:37.000000 nonebot_plugin_dall-e-0.2/nonebot_plugin_dall-e/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-19 01:30:58.095930 nonebot_plugin_dall-e-0.2/nonebot_plugin_dall_e.egg-info/
+-rw-rw-rw-   0        0        0      367 2023-07-19 01:30:58.000000 nonebot_plugin_dall-e-0.2/nonebot_plugin_dall_e.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2023-07-19 01:30:58.000000 nonebot_plugin_dall-e-0.2/nonebot_plugin_dall_e.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 01:30:58.000000 nonebot_plugin_dall-e-0.2/nonebot_plugin_dall_e.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-19 01:30:58.000000 nonebot_plugin_dall-e-0.2/nonebot_plugin_dall_e.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-19 01:30:58.000000 nonebot_plugin_dall-e-0.2/nonebot_plugin_dall_e.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 01:30:58.095930 nonebot_plugin_dall-e-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      759 2023-07-19 01:29:41.000000 nonebot_plugin_dall-e-0.2/setup.py
```

### Comparing `nonebot_plugin_dall-e-0.1/LICENSE` & `nonebot_plugin_dall-e-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dall-e-0.1/README.md` & `nonebot_plugin_dall-e-0.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dall-e-0.1/nonebot_plugin_dall-e/__init__.py` & `nonebot_plugin_dall-e-0.2/nonebot_plugin_dall-e/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dall-e-0.1/nonebot_plugin_dall-e/openai.py` & `nonebot_plugin_dall-e-0.2/nonebot_plugin_dall-e/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dall-e-0.1/nonebot_plugin_dall-e/tools.py` & `nonebot_plugin_dall-e-0.2/nonebot_plugin_dall-e/tools.py`

 * *Files identical despite different names*

