# Comparing `tmp/huetui-1.0.tar.gz` & `tmp/huetui-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huetui-1.0.tar", last modified: Sat Feb 13 21:09:18 2021, max compression
+gzip compressed data, was "huetui-2.0.tar", last modified: Wed Jul 19 09:04:01 2023, max compression
```

## Comparing `huetui-1.0.tar` & `huetui-2.0.tar`

### file list

```diff
@@ -1,19 +1,30 @@
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2021-02-13 21:09:18.641383 huetui-1.0/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      178 2021-02-13 11:25:47.000000 huetui-1.0/.gitignore
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2021-02-13 21:09:18.641383 huetui-1.0/.resources/
--rw-r--r--   0 lukas     (1000) lukas     (1000)   169782 2021-02-13 18:10:10.000000 huetui-1.0/.resources/huetui.gif
--rw-r--r--   0 lukas     (1000) lukas     (1000)   205987 2021-02-13 11:04:55.000000 huetui-1.0/.resources/screen.jpg
--rw-r--r--   0 lukas     (1000) lukas     (1000)    42755 2021-02-13 11:02:36.000000 huetui-1.0/.resources/setup1.png
--rw-r--r--   0 lukas     (1000) lukas     (1000)    49675 2021-02-13 11:02:47.000000 huetui-1.0/.resources/setup2.png
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1067 2021-01-21 10:29:50.000000 huetui-1.0/LICENSE
--rw-r--r--   0 lukas     (1000) lukas     (1000)     5200 2021-02-13 21:09:18.641383 huetui-1.0/PKG-INFO
--rw-r--r--   0 lukas     (1000) lukas     (1000)     4154 2021-02-13 18:10:17.000000 huetui-1.0/README.md
--rwxr-xr-x   0 lukas     (1000) lukas     (1000)    24999 2021-02-13 21:09:12.000000 huetui-1.0/huetui
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2021-02-13 21:09:18.641383 huetui-1.0/huetui.egg-info/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     5200 2021-02-13 21:09:18.000000 huetui-1.0/huetui.egg-info/PKG-INFO
--rw-r--r--   0 lukas     (1000) lukas     (1000)      281 2021-02-13 21:09:18.000000 huetui-1.0/huetui.egg-info/SOURCES.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)        1 2021-02-13 21:09:18.000000 huetui-1.0/huetui.egg-info/dependency_links.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)       54 2021-02-13 21:09:18.000000 huetui-1.0/huetui.egg-info/requires.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)        1 2021-02-13 21:09:18.000000 huetui-1.0/huetui.egg-info/top_level.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)       38 2021-02-13 21:09:18.641383 huetui-1.0/setup.cfg
--rw-r--r--   0 lukas     (1000) lukas     (1000)      710 2021-02-13 20:22:28.000000 huetui-1.0/setup.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-07-19 09:04:01.107851 huetui-2.0/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1067 2020-05-06 12:45:10.000000 huetui-2.0/LICENSE
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3546 2023-07-19 09:04:01.107851 huetui-2.0/PKG-INFO
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3149 2023-07-19 08:56:33.000000 huetui-2.0/README.md
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-07-19 09:04:01.107851 huetui-2.0/bin/
+-rwxr-xr-x   0 lukas     (1000) lukas     (1000)      273 2023-07-19 08:56:33.000000 huetui-2.0/bin/huetui
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-07-19 09:04:01.107851 huetui-2.0/huetui/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-07-19 09:00:53.000000 huetui-2.0/huetui/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-07-19 09:04:01.107851 huetui-2.0/huetui/backend/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-07-19 09:00:53.000000 huetui-2.0/huetui/backend/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     7257 2023-07-19 09:00:53.000000 huetui-2.0/huetui/backend/bridge.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2170 2023-07-19 09:00:53.000000 huetui-2.0/huetui/backend/group.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     8441 2023-07-19 09:00:53.000000 huetui-2.0/huetui/backend/light.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1166 2023-07-19 09:00:53.000000 huetui-2.0/huetui/backend/scene.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     5394 2023-07-19 09:00:53.000000 huetui-2.0/huetui/backend/utils.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-07-19 09:04:01.107851 huetui-2.0/huetui/frontend/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-07-19 09:00:53.000000 huetui-2.0/huetui/frontend/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     4687 2023-07-19 09:00:53.000000 huetui-2.0/huetui/frontend/groups_menu.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     4504 2023-07-19 09:00:53.000000 huetui-2.0/huetui/frontend/lights_menu.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     9812 2023-07-19 09:00:53.000000 huetui-2.0/huetui/frontend/main_window.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      443 2023-07-19 09:00:53.000000 huetui-2.0/huetui/frontend/root.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2080 2023-07-19 09:00:53.000000 huetui-2.0/huetui/frontend/scenes_menu.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-07-19 09:04:01.107851 huetui-2.0/huetui.egg-info/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3546 2023-07-19 09:04:01.000000 huetui-2.0/huetui.egg-info/PKG-INFO
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      529 2023-07-19 09:04:01.000000 huetui-2.0/huetui.egg-info/SOURCES.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        1 2023-07-19 09:04:01.000000 huetui-2.0/huetui.egg-info/dependency_links.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       39 2023-07-19 09:04:01.000000 huetui-2.0/huetui.egg-info/requires.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        7 2023-07-19 09:04:01.000000 huetui-2.0/huetui.egg-info/top_level.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       38 2023-07-19 09:04:01.107851 huetui-2.0/setup.cfg
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      765 2023-07-19 08:56:33.000000 huetui-2.0/setup.py
```

### Comparing `huetui-1.0/LICENSE` & `huetui-2.0/LICENSE`

 * *Files identical despite different names*

