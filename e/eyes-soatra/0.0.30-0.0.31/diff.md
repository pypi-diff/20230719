# Comparing `tmp/eyes_soatra-0.0.30.tar.gz` & `tmp/eyes_soatra-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyes_soatra-0.0.30.tar", last modified: Fri Jul  7 03:15:14 2023, max compression
+gzip compressed data, was "eyes_soatra-0.0.31.tar", last modified: Wed Jul 19 01:31:52 2023, max compression
```

## Comparing `eyes_soatra-0.0.30.tar` & `eyes_soatra-0.0.31.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.505958 eyes_soatra-0.0.30/
--rw-r--r--   0 soatra     (501) staff       (20)       13 2023-05-02 07:13:47.000000 eyes_soatra-0.0.30/LICENSE
--rw-r--r--   0 soatra     (501) staff       (20)      835 2023-07-07 03:15:14.505799 eyes_soatra-0.0.30/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)      330 2023-06-02 06:41:30.000000 eyes_soatra-0.0.30/README.md
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.492421 eyes_soatra-0.0.30/eyes_soatra/
--rw-r--r--   0 soatra     (501) staff       (20)       28 2023-05-02 07:14:02.000000 eyes_soatra-0.0.30/eyes_soatra/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.494502 eyes_soatra-0.0.30/eyes_soatra/constant/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:45:06.000000 eyes_soatra-0.0.30/eyes_soatra/constant/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.494876 eyes_soatra-0.0.30/eyes_soatra/constant/area/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-06-14 00:49:26.000000 eyes_soatra-0.0.30/eyes_soatra/constant/area/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)    19032 2023-06-14 01:12:10.000000 eyes_soatra-0.0.30/eyes_soatra/constant/area/id.py
--rw-r--r--   0 soatra     (501) staff       (20)      233 2023-06-14 03:16:23.000000 eyes_soatra-0.0.30/eyes_soatra/constant/classes.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.495378 eyes_soatra-0.0.30/eyes_soatra/constant/depends/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:17.000000 eyes_soatra-0.0.30/eyes_soatra/constant/depends/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.496192 eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:54:07.000000 eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      224 2023-05-25 08:54:38.000000 eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/end.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.497130 eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/formats/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-28 09:25:41.000000 eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/formats/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)     6706 2023-05-28 08:16:55.000000 eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/formats/end.py
--rw-r--r--   0 soatra     (501) staff       (20)     9568 2023-05-28 08:16:48.000000 eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/formats/period.py
--rw-r--r--   0 soatra     (501) staff       (20)     1127 2023-05-28 08:16:41.000000 eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/formats/start.py
--rw-r--r--   0 soatra     (501) staff       (20)      354 2023-05-29 02:27:50.000000 eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/period.py
--rw-r--r--   0 soatra     (501) staff       (20)      187 2023-05-25 08:54:29.000000 eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/start.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.497768 eyes_soatra-0.0.30/eyes_soatra/constant/depends/view/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:56:44.000000 eyes_soatra-0.0.30/eyes_soatra/constant/depends/view/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.30/eyes_soatra/constant/depends/view/no_data.py
--rw-r--r--   0 soatra     (501) staff       (20)     7338 2023-05-25 08:53:28.000000 eyes_soatra-0.0.30/eyes_soatra/constant/depends/view/not_found.py
--rw-r--r--   0 soatra     (501) staff       (20)       69 2023-05-28 08:21:44.000000 eyes_soatra-0.0.30/eyes_soatra/constant/labels.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.498168 eyes_soatra-0.0.30/eyes_soatra/constant/libs/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:47:14.000000 eyes_soatra-0.0.30/eyes_soatra/constant/libs/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      387 2023-06-09 08:18:33.000000 eyes_soatra-0.0.30/eyes_soatra/constant/libs/requests.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.498539 eyes_soatra-0.0.30/eyes_soatra/constant/user/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:27.000000 eyes_soatra-0.0.30/eyes_soatra/constant/user/__init__.py
--rw-rw-r--   0 soatra     (501) staff       (20)  1339531 2023-05-11 09:13:03.000000 eyes_soatra-0.0.30/eyes_soatra/constant/user/user_agents.py
--rw-r--r--   0 soatra     (501) staff       (20)      844 2023-06-07 03:44:07.000000 eyes_soatra-0.0.30/eyes_soatra/constant/vars.py
--rw-r--r--   0 soatra     (501) staff       (20)      174 2023-06-14 04:10:56.000000 eyes_soatra-0.0.30/eyes_soatra/eyes.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.501652 eyes_soatra-0.0.30/eyes_soatra/funcs/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:41:01.000000 eyes_soatra-0.0.30/eyes_soatra/funcs/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.502010 eyes_soatra-0.0.30/eyes_soatra/funcs/listener/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-06-14 00:49:35.000000 eyes_soatra-0.0.30/eyes_soatra/funcs/listener/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)     9251 2023-06-14 07:16:46.000000 eyes_soatra-0.0.30/eyes_soatra/funcs/listener/watch_changes.py
--rw-r--r--   0 soatra     (501) staff       (20)    20149 2023-06-09 08:49:06.000000 eyes_soatra-0.0.30/eyes_soatra/funcs/time_app.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.504278 eyes_soatra-0.0.30/eyes_soatra/funcs/utils/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 02:07:05.000000 eyes_soatra-0.0.30/eyes_soatra/funcs/utils/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)      602 2023-06-14 06:18:06.000000 eyes_soatra-0.0.30/eyes_soatra/funcs/utils/console.py
--rw-r--r--   0 soatra     (501) staff       (20)      168 2023-05-23 02:06:56.000000 eyes_soatra-0.0.30/eyes_soatra/funcs/utils/dict.py
--rw-r--r--   0 soatra     (501) staff       (20)      372 2023-05-27 04:33:50.000000 eyes_soatra-0.0.30/eyes_soatra/funcs/utils/list.py
--rw-r--r--   0 soatra     (501) staff       (20)       82 2023-06-14 03:20:51.000000 eyes_soatra-0.0.30/eyes_soatra/funcs/utils/number.py
--rw-r--r--   0 soatra     (501) staff       (20)     2624 2023-06-14 04:22:54.000000 eyes_soatra-0.0.30/eyes_soatra/funcs/utils/string.py
--rw-r--r--   0 soatra     (501) staff       (20)       99 2023-06-14 06:54:22.000000 eyes_soatra-0.0.30/eyes_soatra/funcs/utils/time.py
--rw-r--r--   0 soatra     (501) staff       (20)    14223 2023-07-07 03:11:17.000000 eyes_soatra-0.0.30/eyes_soatra/funcs/view_page.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.493447 eyes_soatra-0.0.30/eyes_soatra.egg-info/
--rw-r--r--   0 soatra     (501) staff       (20)      835 2023-07-07 03:15:14.000000 eyes_soatra-0.0.30/eyes_soatra.egg-info/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)     1644 2023-07-07 03:15:14.000000 eyes_soatra-0.0.30/eyes_soatra.egg-info/SOURCES.txt
--rw-r--r--   0 soatra     (501) staff       (20)        1 2023-07-07 03:15:14.000000 eyes_soatra-0.0.30/eyes_soatra.egg-info/dependency_links.txt
--rw-r--r--   0 soatra     (501) staff       (20)       34 2023-07-07 03:15:14.000000 eyes_soatra-0.0.30/eyes_soatra.egg-info/requires.txt
--rw-r--r--   0 soatra     (501) staff       (20)       12 2023-07-07 03:15:14.000000 eyes_soatra-0.0.30/eyes_soatra.egg-info/top_level.txt
--rw-r--r--   0 soatra     (501) staff       (20)       38 2023-07-07 03:15:14.506008 eyes_soatra-0.0.30/setup.cfg
--rw-r--r--   0 soatra     (501) staff       (20)     1122 2023-07-07 03:14:34.000000 eyes_soatra-0.0.30/setup.py
--rw-r--r--   0 soatra     (501) staff       (20)     1123 2023-06-02 02:26:19.000000 eyes_soatra-0.0.30/start.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-07 03:15:14.505450 eyes_soatra-0.0.30/test/
--rw-r--r--   0 soatra     (501) staff       (20)     2942 2023-05-29 04:49:56.000000 eyes_soatra-0.0.30/test/test.py
--rw-r--r--   0 soatra     (501) staff       (20)     2989 2023-05-25 06:31:32.000000 eyes_soatra-0.0.30/test/test1.py
--rw-r--r--   0 soatra     (501) staff       (20)      794 2023-07-07 03:11:42.000000 eyes_soatra-0.0.30/test/test2.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 01:31:52.122905 eyes_soatra-0.0.31/
+-rw-r--r--   0 soatra     (501) staff       (20)       13 2023-05-02 07:13:47.000000 eyes_soatra-0.0.31/LICENSE
+-rw-r--r--   0 soatra     (501) staff       (20)      835 2023-07-19 01:31:52.122765 eyes_soatra-0.0.31/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)      330 2023-06-02 06:41:30.000000 eyes_soatra-0.0.31/README.md
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 01:31:52.109962 eyes_soatra-0.0.31/eyes_soatra/
+-rw-r--r--   0 soatra     (501) staff       (20)       28 2023-05-02 07:14:02.000000 eyes_soatra-0.0.31/eyes_soatra/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 01:31:52.111843 eyes_soatra-0.0.31/eyes_soatra/constant/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:45:06.000000 eyes_soatra-0.0.31/eyes_soatra/constant/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 01:31:52.112225 eyes_soatra-0.0.31/eyes_soatra/constant/area/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-06-14 00:49:26.000000 eyes_soatra-0.0.31/eyes_soatra/constant/area/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)    19032 2023-06-14 01:12:10.000000 eyes_soatra-0.0.31/eyes_soatra/constant/area/id.py
+-rw-r--r--   0 soatra     (501) staff       (20)      233 2023-06-14 03:16:23.000000 eyes_soatra-0.0.31/eyes_soatra/constant/classes.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 01:31:52.112727 eyes_soatra-0.0.31/eyes_soatra/constant/depends/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:17.000000 eyes_soatra-0.0.31/eyes_soatra/constant/depends/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 01:31:52.113928 eyes_soatra-0.0.31/eyes_soatra/constant/depends/app_date/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:54:07.000000 eyes_soatra-0.0.31/eyes_soatra/constant/depends/app_date/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      224 2023-05-25 08:54:38.000000 eyes_soatra-0.0.31/eyes_soatra/constant/depends/app_date/end.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 01:31:52.114852 eyes_soatra-0.0.31/eyes_soatra/constant/depends/app_date/formats/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-28 09:25:41.000000 eyes_soatra-0.0.31/eyes_soatra/constant/depends/app_date/formats/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)     6706 2023-05-28 08:16:55.000000 eyes_soatra-0.0.31/eyes_soatra/constant/depends/app_date/formats/end.py
+-rw-r--r--   0 soatra     (501) staff       (20)     9568 2023-05-28 08:16:48.000000 eyes_soatra-0.0.31/eyes_soatra/constant/depends/app_date/formats/period.py
+-rw-r--r--   0 soatra     (501) staff       (20)     1127 2023-05-28 08:16:41.000000 eyes_soatra-0.0.31/eyes_soatra/constant/depends/app_date/formats/start.py
+-rw-r--r--   0 soatra     (501) staff       (20)      354 2023-05-29 02:27:50.000000 eyes_soatra-0.0.31/eyes_soatra/constant/depends/app_date/period.py
+-rw-r--r--   0 soatra     (501) staff       (20)      187 2023-05-25 08:54:29.000000 eyes_soatra-0.0.31/eyes_soatra/constant/depends/app_date/start.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 01:31:52.115521 eyes_soatra-0.0.31/eyes_soatra/constant/depends/view/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:56:44.000000 eyes_soatra-0.0.31/eyes_soatra/constant/depends/view/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.31/eyes_soatra/constant/depends/view/no_data.py
+-rw-r--r--   0 soatra     (501) staff       (20)     7338 2023-05-25 08:53:28.000000 eyes_soatra-0.0.31/eyes_soatra/constant/depends/view/not_found.py
+-rw-r--r--   0 soatra     (501) staff       (20)       69 2023-05-28 08:21:44.000000 eyes_soatra-0.0.31/eyes_soatra/constant/labels.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 01:31:52.115938 eyes_soatra-0.0.31/eyes_soatra/constant/libs/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:47:14.000000 eyes_soatra-0.0.31/eyes_soatra/constant/libs/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      387 2023-06-09 08:18:33.000000 eyes_soatra-0.0.31/eyes_soatra/constant/libs/requests.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 01:31:52.116462 eyes_soatra-0.0.31/eyes_soatra/constant/user/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:27.000000 eyes_soatra-0.0.31/eyes_soatra/constant/user/__init__.py
+-rw-rw-r--   0 soatra     (501) staff       (20)  1339531 2023-05-11 09:13:03.000000 eyes_soatra-0.0.31/eyes_soatra/constant/user/user_agents.py
+-rw-r--r--   0 soatra     (501) staff       (20)      844 2023-06-07 03:44:07.000000 eyes_soatra-0.0.31/eyes_soatra/constant/vars.py
+-rw-r--r--   0 soatra     (501) staff       (20)      174 2023-06-14 04:10:56.000000 eyes_soatra-0.0.31/eyes_soatra/eyes.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 01:31:52.119367 eyes_soatra-0.0.31/eyes_soatra/funcs/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:41:01.000000 eyes_soatra-0.0.31/eyes_soatra/funcs/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 01:31:52.119770 eyes_soatra-0.0.31/eyes_soatra/funcs/listener/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-06-14 00:49:35.000000 eyes_soatra-0.0.31/eyes_soatra/funcs/listener/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)     9251 2023-06-14 07:16:46.000000 eyes_soatra-0.0.31/eyes_soatra/funcs/listener/watch_changes.py
+-rw-r--r--   0 soatra     (501) staff       (20)    20149 2023-06-09 08:49:06.000000 eyes_soatra-0.0.31/eyes_soatra/funcs/time_app.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 01:31:52.121508 eyes_soatra-0.0.31/eyes_soatra/funcs/utils/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 02:07:05.000000 eyes_soatra-0.0.31/eyes_soatra/funcs/utils/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      602 2023-06-14 06:18:06.000000 eyes_soatra-0.0.31/eyes_soatra/funcs/utils/console.py
+-rw-r--r--   0 soatra     (501) staff       (20)      168 2023-05-23 02:06:56.000000 eyes_soatra-0.0.31/eyes_soatra/funcs/utils/dict.py
+-rw-r--r--   0 soatra     (501) staff       (20)      372 2023-05-27 04:33:50.000000 eyes_soatra-0.0.31/eyes_soatra/funcs/utils/list.py
+-rw-r--r--   0 soatra     (501) staff       (20)       82 2023-06-14 03:20:51.000000 eyes_soatra-0.0.31/eyes_soatra/funcs/utils/number.py
+-rw-r--r--   0 soatra     (501) staff       (20)     2624 2023-06-14 04:22:54.000000 eyes_soatra-0.0.31/eyes_soatra/funcs/utils/string.py
+-rw-r--r--   0 soatra     (501) staff       (20)       99 2023-06-14 06:54:22.000000 eyes_soatra-0.0.31/eyes_soatra/funcs/utils/time.py
+-rw-r--r--   0 soatra     (501) staff       (20)    14391 2023-07-10 01:38:32.000000 eyes_soatra-0.0.31/eyes_soatra/funcs/view_page.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 01:31:52.110998 eyes_soatra-0.0.31/eyes_soatra.egg-info/
+-rw-r--r--   0 soatra     (501) staff       (20)      835 2023-07-19 01:31:52.000000 eyes_soatra-0.0.31/eyes_soatra.egg-info/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)     1644 2023-07-19 01:31:52.000000 eyes_soatra-0.0.31/eyes_soatra.egg-info/SOURCES.txt
+-rw-r--r--   0 soatra     (501) staff       (20)        1 2023-07-19 01:31:52.000000 eyes_soatra-0.0.31/eyes_soatra.egg-info/dependency_links.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       34 2023-07-19 01:31:52.000000 eyes_soatra-0.0.31/eyes_soatra.egg-info/requires.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       12 2023-07-19 01:31:52.000000 eyes_soatra-0.0.31/eyes_soatra.egg-info/top_level.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       38 2023-07-19 01:31:52.122950 eyes_soatra-0.0.31/setup.cfg
+-rw-r--r--   0 soatra     (501) staff       (20)     1122 2023-07-19 01:31:31.000000 eyes_soatra-0.0.31/setup.py
+-rw-r--r--   0 soatra     (501) staff       (20)     1123 2023-06-02 02:26:19.000000 eyes_soatra-0.0.31/start.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-07-19 01:31:52.122392 eyes_soatra-0.0.31/test/
+-rw-r--r--   0 soatra     (501) staff       (20)     2942 2023-05-29 04:49:56.000000 eyes_soatra-0.0.31/test/test.py
+-rw-r--r--   0 soatra     (501) staff       (20)     2989 2023-05-25 06:31:32.000000 eyes_soatra-0.0.31/test/test1.py
+-rw-r--r--   0 soatra     (501) staff       (20)      232 2023-07-19 01:28:18.000000 eyes_soatra-0.0.31/test/test2.py
```

### Comparing `eyes_soatra-0.0.30/PKG-INFO` & `eyes_soatra-0.0.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyes_soatra
-Version: 0.0.30
+Version: 0.0.31
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: python,crawler,scanner,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eyes_soatra-0.0.30/eyes_soatra/constant/area/id.py` & `eyes_soatra-0.0.31/eyes_soatra/constant/area/id.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/formats/end.py` & `eyes_soatra-0.0.31/eyes_soatra/constant/depends/app_date/formats/end.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/formats/period.py` & `eyes_soatra-0.0.31/eyes_soatra/constant/depends/app_date/formats/period.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.30/eyes_soatra/constant/depends/app_date/formats/start.py` & `eyes_soatra-0.0.31/eyes_soatra/constant/depends/app_date/formats/start.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.30/eyes_soatra/constant/depends/view/not_found.py` & `eyes_soatra-0.0.31/eyes_soatra/constant/depends/view/not_found.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.30/eyes_soatra/constant/user/user_agents.py` & `eyes_soatra-0.0.31/eyes_soatra/constant/user/user_agents.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.30/eyes_soatra/constant/vars.py` & `eyes_soatra-0.0.31/eyes_soatra/constant/vars.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.30/eyes_soatra/funcs/listener/watch_changes.py` & `eyes_soatra-0.0.31/eyes_soatra/funcs/listener/watch_changes.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.30/eyes_soatra/funcs/time_app.py` & `eyes_soatra-0.0.31/eyes_soatra/funcs/time_app.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.30/eyes_soatra/funcs/utils/console.py` & `eyes_soatra-0.0.31/eyes_soatra/funcs/utils/console.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.30/eyes_soatra/funcs/utils/string.py` & `eyes_soatra-0.0.31/eyes_soatra/funcs/utils/string.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.30/eyes_soatra/funcs/view_page.py` & `eyes_soatra-0.0.31/eyes_soatra/funcs/view_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,16 +316,24 @@
                     **expired_obj,
                     'error': f'Server error responses: {status_code}',
                     'redirected': redirected,
                     'url': current_url,
                     'status': status_code,
                     'tried': tried,
                 }
-
-            text = __re.sub('(<\?.*\?>)', '', response.text + response.content.decode())
+            
+            content = ''
+            
+            try:
+                content = response.content.decode()
+            except:
+                pass
+            
+            
+            text = __re.sub('(<\?.*\?>)', '', response.text + content)
             html = __html.fromstring(text)
             __etree.strip_elements(html, *__remove_tags)
             
             if allow_redirects:
                 meta_refresh = html.xpath("//meta[translate(@http-equiv,'REFSH','refsh')='refresh']/@content")
                 
                 if len(meta_refresh):
```

### Comparing `eyes_soatra-0.0.30/eyes_soatra.egg-info/PKG-INFO` & `eyes_soatra-0.0.31/eyes_soatra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyes-soatra
-Version: 0.0.30
+Version: 0.0.31
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: python,crawler,scanner,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eyes_soatra-0.0.30/eyes_soatra.egg-info/SOURCES.txt` & `eyes_soatra-0.0.31/eyes_soatra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.30/setup.py` & `eyes_soatra-0.0.31/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 NAME = 'eyes_soatra'
-VERSION = '0.0.30'
+VERSION = '0.0.31'
 DESCRIPTION = 'Eyes'
 
 AUTHOR_NAME = 'Soatra'
 AUTHOR_EMAIL = 'johnsoatra@gmail.com'
 
 # Setting up
 setup(
```

### Comparing `eyes_soatra-0.0.30/start.py` & `eyes_soatra-0.0.31/start.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.30/test/test.py` & `eyes_soatra-0.0.31/test/test.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.30/test/test1.py` & `eyes_soatra-0.0.31/test/test1.py`

 * *Files identical despite different names*

