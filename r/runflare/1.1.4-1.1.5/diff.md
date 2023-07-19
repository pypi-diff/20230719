# Comparing `tmp/runflare-1.1.4.tar.gz` & `tmp/runflare-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runflare-1.1.4.tar", last modified: Tue Aug 23 05:51:37 2022, max compression
+gzip compressed data, was "runflare-1.1.5.tar", last modified: Wed Jul 19 09:37:31 2023, max compression
```

## Comparing `runflare-1.1.4.tar` & `runflare-1.1.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2022-08-23 05:51:37.700756 runflare-1.1.4/
--rw-rw-rw-   0        0        0       33 2021-10-28 05:27:29.000000 runflare-1.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      403 2022-08-23 05:51:37.699757 runflare-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       86 2021-10-28 05:27:29.000000 runflare-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2022-08-23 05:51:37.396656 runflare-1.1.4/runflare/
--rw-rw-rw-   0        0        0     4478 2022-01-08 11:54:34.000000 runflare-1.1.4/runflare/.runflare_ignore
--rw-rw-rw-   0        0        0       90 2022-08-23 05:42:02.000000 runflare-1.1.4/runflare/__init__.py
--rw-rw-rw-   0        0        0      689 2021-10-28 05:27:28.000000 runflare-1.1.4/runflare/exceptions.py
--rw-rw-rw-   0        0        0     7684 2021-10-28 05:27:28.000000 runflare-1.1.4/runflare/gitignore_parser.py
-drwxrwxrwx   0        0        0        0 2022-08-23 05:51:37.474678 runflare-1.1.4/runflare/inquirer/
--rw-rw-rw-   0        0        0      706 2021-11-08 09:06:06.000000 runflare-1.1.4/runflare/inquirer/__init__.py
--rw-rw-rw-   0        0        0      545 2021-11-08 05:55:14.000000 runflare-1.1.4/runflare/inquirer/errors.py
--rw-rw-rw-   0        0        0      367 2021-11-08 05:55:14.000000 runflare-1.1.4/runflare/inquirer/events.py
--rw-rw-rw-   0        0        0      850 2021-11-08 10:01:42.000000 runflare-1.1.4/runflare/inquirer/prompt.py
--rw-rw-rw-   0        0        0     8457 2021-11-08 09:01:14.000000 runflare-1.1.4/runflare/inquirer/questions.py
-drwxrwxrwx   0        0        0        0 2022-08-23 05:51:37.481670 runflare-1.1.4/runflare/inquirer/render/
--rw-rw-rw-   0        0        0      407 2021-11-08 09:10:32.000000 runflare-1.1.4/runflare/inquirer/render/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-23 05:51:37.550979 runflare-1.1.4/runflare/inquirer/render/console/
--rw-rw-rw-   0        0        0     6380 2021-11-08 09:07:20.000000 runflare-1.1.4/runflare/inquirer/render/console/__init__.py
--rw-rw-rw-   0        0        0     3722 2021-11-08 09:07:46.000000 runflare-1.1.4/runflare/inquirer/render/console/_checkbox.py
--rw-rw-rw-   0        0        0      829 2021-11-08 09:11:12.000000 runflare-1.1.4/runflare/inquirer/render/console/_confirm.py
--rw-rw-rw-   0        0        0     1241 2021-11-08 09:08:06.000000 runflare-1.1.4/runflare/inquirer/render/console/_editor.py
--rw-rw-rw-   0        0        0     3130 2021-11-08 09:08:30.000000 runflare-1.1.4/runflare/inquirer/render/console/_list.py
--rw-rw-rw-   0        0        0      448 2021-11-08 09:08:52.000000 runflare-1.1.4/runflare/inquirer/render/console/_password.py
--rw-rw-rw-   0        0        0      104 2021-11-08 09:08:52.000000 runflare-1.1.4/runflare/inquirer/render/console/_path.py
--rw-rw-rw-   0        0        0     1668 2021-11-08 12:32:06.000000 runflare-1.1.4/runflare/inquirer/render/console/_text.py
--rw-rw-rw-   0        0        0     1157 2021-11-08 05:55:14.000000 runflare-1.1.4/runflare/inquirer/render/console/base.py
--rw-rw-rw-   0        0        0     1419 2021-11-08 09:01:14.000000 runflare-1.1.4/runflare/inquirer/shortcuts.py
--rw-rw-rw-   0        0        0     4112 2021-11-08 09:01:14.000000 runflare-1.1.4/runflare/inquirer/themes.py
--rw-rw-rw-   0        0        0     7332 2022-03-13 07:47:10.000000 runflare-1.1.4/runflare/runflare.py
-drwxrwxrwx   0        0        0        0 2022-08-23 05:51:37.581954 runflare-1.1.4/runflare/runflare_client/
--rw-rw-rw-   0        0        0        0 2021-10-28 05:27:28.000000 runflare-1.1.4/runflare/runflare_client/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-23 05:51:37.596614 runflare-1.1.4/runflare/runflare_client/account/
--rw-rw-rw-   0        0        0      112 2021-11-08 08:33:08.000000 runflare-1.1.4/runflare/runflare_client/account/__init__.py
--rw-rw-rw-   0        0        0     1571 2022-03-13 07:10:28.000000 runflare-1.1.4/runflare/runflare_client/account/auth.py
-drwxrwxrwx   0        0        0        0 2022-08-23 05:51:37.618595 runflare-1.1.4/runflare/runflare_client/analyze/
--rw-rw-rw-   0        0        0      144 2021-10-28 05:27:28.000000 runflare-1.1.4/runflare/runflare_client/analyze/__init__.py
--rw-rw-rw-   0        0        0      840 2021-10-28 05:27:28.000000 runflare-1.1.4/runflare/runflare_client/analyze/events.py
--rw-rw-rw-   0        0        0      842 2021-10-28 05:27:28.000000 runflare-1.1.4/runflare/runflare_client/analyze/log.py
--rw-rw-rw-   0        0        0    55666 2022-03-12 11:33:32.000000 runflare-1.1.4/runflare/runflare_client/custom_pathlib.py
-drwxrwxrwx   0        0        0        0 2022-08-23 05:51:37.643867 runflare-1.1.4/runflare/runflare_client/data_manager/
--rw-rw-rw-   0        0        0        0 2021-10-28 05:27:28.000000 runflare-1.1.4/runflare/runflare_client/data_manager/__init__.py
--rw-rw-rw-   0        0        0     2363 2021-11-07 07:28:00.000000 runflare-1.1.4/runflare/runflare_client/data_manager/adapter.py
--rw-rw-rw-   0        0        0       39 2021-10-28 05:27:28.000000 runflare-1.1.4/runflare/runflare_client/data_manager/base_manager.py
--rw-rw-rw-   0        0        0    13777 2022-03-12 11:34:14.000000 runflare-1.1.4/runflare/runflare_client/data_manager/sqlite_manager.py
-drwxrwxrwx   0        0        0        0 2022-08-23 05:51:37.675842 runflare-1.1.4/runflare/runflare_client/deploy/
--rw-rw-rw-   0        0        0      121 2021-11-07 09:12:24.000000 runflare-1.1.4/runflare/runflare_client/deploy/__init__.py
--rw-rw-rw-   0        0        0     9631 2022-03-15 11:33:38.000000 runflare-1.1.4/runflare/runflare_client/deploy/cache.py
--rw-rw-rw-   0        0        0     7589 2022-08-20 09:43:42.000000 runflare-1.1.4/runflare/runflare_client/deploy/deployment.py
--rw-rw-rw-   0        0        0     4314 2022-08-23 05:43:00.000000 runflare-1.1.4/runflare/runflare_client/deploy/upload.py
--rw-rw-rw-   0        0        0     3401 2022-03-13 07:27:04.000000 runflare-1.1.4/runflare/runflare_client/requester.py
-drwxrwxrwx   0        0        0        0 2022-08-23 05:51:37.698759 runflare-1.1.4/runflare/runflare_client/service/
--rw-rw-rw-   0        0        0      231 2021-10-28 05:27:28.000000 runflare-1.1.4/runflare/runflare_client/service/__init__.py
--rw-rw-rw-   0        0        0     1722 2021-10-28 05:27:28.000000 runflare-1.1.4/runflare/runflare_client/service/manage.py
--rw-rw-rw-   0        0        0      700 2022-03-13 07:27:56.000000 runflare-1.1.4/runflare/runflare_client/service/projects.py
--rw-rw-rw-   0        0        0     4539 2022-07-25 05:24:52.000000 runflare-1.1.4/runflare/runflare_client/web_socket.py
--rw-rw-rw-   0        0        0     1068 2022-08-23 05:41:17.000000 runflare-1.1.4/runflare/settings.py
--rw-rw-rw-   0        0        0     5710 2022-08-20 06:16:48.000000 runflare-1.1.4/runflare/utils.py
--rw-rw-rw-   0        0        0     3432 2022-02-22 06:49:20.000000 runflare-1.1.4/runflare/version_check.py
-drwxrwxrwx   0        0        0        0 2022-08-23 05:51:37.419535 runflare-1.1.4/runflare.egg-info/
--rw-rw-rw-   0        0        0      403 2022-08-23 05:51:36.000000 runflare-1.1.4/runflare.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1929 2022-08-23 05:51:36.000000 runflare-1.1.4/runflare.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-23 05:51:36.000000 runflare-1.1.4/runflare.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2022-08-23 05:51:36.000000 runflare-1.1.4/runflare.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      402 2022-08-23 05:51:36.000000 runflare-1.1.4/runflare.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-08-23 05:51:36.000000 runflare-1.1.4/runflare.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-23 05:51:37.700756 runflare-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1504 2021-12-12 13:05:30.000000 runflare-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:37:31.721013 runflare-1.1.5/
+-rw-rw-rw-   0        0        0       33 2021-10-28 05:27:29.000000 runflare-1.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      403 2023-07-19 09:37:31.720014 runflare-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2021-10-28 05:27:29.000000 runflare-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 09:37:31.346947 runflare-1.1.5/runflare/
+-rw-rw-rw-   0        0        0     4478 2022-01-08 11:54:34.000000 runflare-1.1.5/runflare/.runflare_ignore
+-rw-rw-rw-   0        0        0       90 2023-07-19 09:36:14.000000 runflare-1.1.5/runflare/__init__.py
+-rw-rw-rw-   0        0        0      689 2021-10-28 05:27:28.000000 runflare-1.1.5/runflare/exceptions.py
+-rw-rw-rw-   0        0        0     7684 2021-10-28 05:27:28.000000 runflare-1.1.5/runflare/gitignore_parser.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:37:31.440568 runflare-1.1.5/runflare/inquirer/
+-rw-rw-rw-   0        0        0      706 2021-11-08 09:06:06.000000 runflare-1.1.5/runflare/inquirer/__init__.py
+-rw-rw-rw-   0        0        0      545 2021-11-08 05:55:14.000000 runflare-1.1.5/runflare/inquirer/errors.py
+-rw-rw-rw-   0        0        0      367 2021-11-08 05:55:14.000000 runflare-1.1.5/runflare/inquirer/events.py
+-rw-rw-rw-   0        0        0      850 2021-11-08 10:01:42.000000 runflare-1.1.5/runflare/inquirer/prompt.py
+-rw-rw-rw-   0        0        0     8457 2021-11-08 09:01:14.000000 runflare-1.1.5/runflare/inquirer/questions.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:37:31.448561 runflare-1.1.5/runflare/inquirer/render/
+-rw-rw-rw-   0        0        0      407 2021-11-08 09:10:32.000000 runflare-1.1.5/runflare/inquirer/render/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:37:31.533766 runflare-1.1.5/runflare/inquirer/render/console/
+-rw-rw-rw-   0        0        0     6380 2021-11-08 09:07:20.000000 runflare-1.1.5/runflare/inquirer/render/console/__init__.py
+-rw-rw-rw-   0        0        0     3722 2021-11-08 09:07:46.000000 runflare-1.1.5/runflare/inquirer/render/console/_checkbox.py
+-rw-rw-rw-   0        0        0      829 2021-11-08 09:11:12.000000 runflare-1.1.5/runflare/inquirer/render/console/_confirm.py
+-rw-rw-rw-   0        0        0     1241 2021-11-08 09:08:06.000000 runflare-1.1.5/runflare/inquirer/render/console/_editor.py
+-rw-rw-rw-   0        0        0     3130 2021-11-08 09:08:30.000000 runflare-1.1.5/runflare/inquirer/render/console/_list.py
+-rw-rw-rw-   0        0        0      448 2021-11-08 09:08:52.000000 runflare-1.1.5/runflare/inquirer/render/console/_password.py
+-rw-rw-rw-   0        0        0      104 2021-11-08 09:08:52.000000 runflare-1.1.5/runflare/inquirer/render/console/_path.py
+-rw-rw-rw-   0        0        0     1668 2021-11-08 12:32:06.000000 runflare-1.1.5/runflare/inquirer/render/console/_text.py
+-rw-rw-rw-   0        0        0     1157 2021-11-08 05:55:14.000000 runflare-1.1.5/runflare/inquirer/render/console/base.py
+-rw-rw-rw-   0        0        0     1419 2021-11-08 09:01:14.000000 runflare-1.1.5/runflare/inquirer/shortcuts.py
+-rw-rw-rw-   0        0        0     4112 2021-11-08 09:01:14.000000 runflare-1.1.5/runflare/inquirer/themes.py
+-rw-rw-rw-   0        0        0     7829 2023-07-19 09:36:14.000000 runflare-1.1.5/runflare/runflare.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:37:31.571893 runflare-1.1.5/runflare/runflare_client/
+-rw-rw-rw-   0        0        0        0 2021-10-28 05:27:28.000000 runflare-1.1.5/runflare/runflare_client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:37:31.589880 runflare-1.1.5/runflare/runflare_client/account/
+-rw-rw-rw-   0        0        0      112 2021-11-08 08:33:08.000000 runflare-1.1.5/runflare/runflare_client/account/__init__.py
+-rw-rw-rw-   0        0        0     1567 2023-07-19 09:36:14.000000 runflare-1.1.5/runflare/runflare_client/account/auth.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:37:31.615855 runflare-1.1.5/runflare/runflare_client/analyze/
+-rw-rw-rw-   0        0        0      144 2021-10-28 05:27:28.000000 runflare-1.1.5/runflare/runflare_client/analyze/__init__.py
+-rw-rw-rw-   0        0        0      840 2021-10-28 05:27:28.000000 runflare-1.1.5/runflare/runflare_client/analyze/events.py
+-rw-rw-rw-   0        0        0      842 2021-10-28 05:27:28.000000 runflare-1.1.5/runflare/runflare_client/analyze/log.py
+-rw-rw-rw-   0        0        0    55666 2022-03-12 11:33:32.000000 runflare-1.1.5/runflare/runflare_client/custom_pathlib.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:37:31.647829 runflare-1.1.5/runflare/runflare_client/data_manager/
+-rw-rw-rw-   0        0        0        0 2021-10-28 05:27:28.000000 runflare-1.1.5/runflare/runflare_client/data_manager/__init__.py
+-rw-rw-rw-   0        0        0     2363 2021-11-07 07:28:00.000000 runflare-1.1.5/runflare/runflare_client/data_manager/adapter.py
+-rw-rw-rw-   0        0        0       39 2021-10-28 05:27:28.000000 runflare-1.1.5/runflare/runflare_client/data_manager/base_manager.py
+-rw-rw-rw-   0        0        0    13778 2023-07-19 09:36:14.000000 runflare-1.1.5/runflare/runflare_client/data_manager/sqlite_manager.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:37:31.691516 runflare-1.1.5/runflare/runflare_client/deploy/
+-rw-rw-rw-   0        0        0      121 2021-11-07 09:12:24.000000 runflare-1.1.5/runflare/runflare_client/deploy/__init__.py
+-rw-rw-rw-   0        0        0     9992 2023-07-19 09:36:14.000000 runflare-1.1.5/runflare/runflare_client/deploy/cache.py
+-rw-rw-rw-   0        0        0     8440 2023-07-19 09:36:14.000000 runflare-1.1.5/runflare/runflare_client/deploy/deployment.py
+-rw-rw-rw-   0        0        0     4314 2022-08-23 05:43:00.000000 runflare-1.1.5/runflare/runflare_client/deploy/upload.py
+-rw-rw-rw-   0        0        0     3401 2022-03-13 07:27:04.000000 runflare-1.1.5/runflare/runflare_client/requester.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:37:31.719015 runflare-1.1.5/runflare/runflare_client/service/
+-rw-rw-rw-   0        0        0      193 2023-07-19 09:36:14.000000 runflare-1.1.5/runflare/runflare_client/service/__init__.py
+-rw-rw-rw-   0        0        0     1722 2021-10-28 05:27:28.000000 runflare-1.1.5/runflare/runflare_client/service/manage.py
+-rw-rw-rw-   0        0        0      479 2023-07-19 09:36:14.000000 runflare-1.1.5/runflare/runflare_client/service/projects.py
+-rw-rw-rw-   0        0        0     4539 2023-07-19 09:36:14.000000 runflare-1.1.5/runflare/runflare_client/web_socket.py
+-rw-rw-rw-   0        0        0     1022 2023-07-19 09:36:14.000000 runflare-1.1.5/runflare/settings.py
+-rw-rw-rw-   0        0        0     5950 2023-07-19 09:36:14.000000 runflare-1.1.5/runflare/utils.py
+-rw-rw-rw-   0        0        0     3563 2023-07-19 09:36:14.000000 runflare-1.1.5/runflare/version_check.py
+drwxrwxrwx   0        0        0        0 2023-07-19 09:37:31.372925 runflare-1.1.5/runflare.egg-info/
+-rw-rw-rw-   0        0        0      403 2023-07-19 09:37:30.000000 runflare-1.1.5/runflare.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1929 2023-07-19 09:37:30.000000 runflare-1.1.5/runflare.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 09:37:30.000000 runflare-1.1.5/runflare.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-07-19 09:37:30.000000 runflare-1.1.5/runflare.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      401 2023-07-19 09:37:30.000000 runflare-1.1.5/runflare.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-19 09:37:30.000000 runflare-1.1.5/runflare.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 09:37:31.721013 runflare-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1503 2023-07-19 09:36:14.000000 runflare-1.1.5/setup.py
```

### Comparing `runflare-1.1.4/runflare/.runflare_ignore` & `runflare-1.1.5/runflare/.runflare_ignore`

 * *Files identical despite different names*

### Comparing `runflare-1.1.4/runflare/exceptions.py` & `runflare-1.1.5/runflare/exceptions.py`

 * *Files identical despite different names*

### Comparing `runflare-1.1.4/runflare/gitignore_parser.py` & `runflare-1.1.5/runflare/gitignore_parser.py`

 * *Files identical despite different names*

### Comparing `runflare-1.1.4/runflare/inquirer/__init__.py` & `runflare-1.1.5/runflare/inquirer/__init__.py`

 * *Files identical despite different names*

### Comparing `runflare-1.1.4/runflare/inquirer/errors.py` & `runflare-1.1.5/runflare/inquirer/errors.py`

 * *Files identical despite different names*

### Comparing `runflare-1.1.4/runflare/inquirer/prompt.py` & `runflare-1.1.5/runflare/inquirer/prompt.py`

 * *Files identical despite different names*

### Comparing `runflare-1.1.4/runflare/inquirer/questions.py` & `runflare-1.1.5/runflare/inquirer/questions.py`

 * *Files identical despite different names*

### Comparing `runflare-1.1.4/runflare/inquirer/render/console/__init__.py` & `runflare-1.1.5/runflare/inquirer/render/console/__init__.py`

 * *Files identical despite different names*

### Comparing `runflare-1.1.4/runflare/inquirer/render/console/_checkbox.py` & `runflare-1.1.5/runflare/inquirer/render/console/_checkbox.py`

 * *Files identical despite different names*

### Comparing `runflare-1.1.4/runflare/inquirer/render/console/_confirm.py` & `runflare-1.1.5/runflare/inquirer/render/console/_confirm.py`

 * *Files identical despite different names*

### Comparing `runflare-1.1.4/runflare/inquirer/render/console/_editor.py` & `runflare-1.1.5/runflare/inquirer/render/console/_editor.py`

 * *Files identical despite different names*

### Comparing `runflare-1.1.4/runflare/inquirer/render/console/_list.py` & `runflare-1.1.5/runflare/inquirer/render/console/_list.py`

 * *Files identical despite different names*

### Comparing `runflare-1.1.4/runflare/inquirer/render/console/_text.py` & `runflare-1.1.5/runflare/inquirer/render/console/_text.py`

 * *Files identical despite different names*

### Comparing `runflare-1.1.4/runflare/inquirer/render/console/base.py` & `runflare-1.1.5/runflare/inquirer/render/console/base.py`

 * *Files identical despite different names*

### Comparing `runflare-1.1.4/runflare/inquirer/shortcuts.py` & `runflare-1.1.5/runflare/inquirer/shortcuts.py`

 * *Files identical despite different names*

### Comparing `runflare-1.1.4/runflare/inquirer/themes.py` & `runflare-1.1.5/runflare/inquirer/themes.py`

 * *Files identical despite different names*

### Comparing `runflare-1.1.4/runflare/runflare.py` & `runflare-1.1.5/runflare/runflare.py`

 * *Files 10% similar despite different names*

```diff
@@ -75,15 +75,15 @@
    runflare stop -y\tUse previous item id to Stop project
 {bold_start}Reset Deploy Root:{bold_stop}
    runflare reset \tSelect And Delete root
    runflare reset --all\tDelete all available deploy root
 For More Help Enter
     runflare COMMAND help    
     
-        """.format(bold_stop=Style.RESET_ALL,bold_start=Style.BRIGHT,VERSION=VERSION)
+        """.format(bold_stop=Style.RESET_ALL, bold_start=Style.BRIGHT, VERSION=VERSION)
 
     def help(self):
         """for more help"""
         return self._help()
 
     @staticmethod
     def login(email=None,password=None):
@@ -200,21 +200,28 @@
 
     def __str__(self):
         return self._help()
 
 
 def run():
     clear()
-    checker = Version.has_new_version()
+    checker = Version.check_version()
     if checker:
+        if checker == 3:
+            print("""                     ╭──────────────────────────────────────╮
+                     │    Old Version, Please Update CLI    │
+                     │ Run `pip install --upgrade runflare` │
+                     ╰──────────────────────────────────────╯""")
+            exit()
+
         try:
             fire.Fire(RunFlare)
         except KeyError:
             raise SystemExit
-        if checker == 2:
+        if checker in [2,3]:
             print()
             print("""                     ╭──────────────────────────────────────╮
                      │           Update available           │
                      │ Run `pip install --upgrade runflare` │
                      ╰──────────────────────────────────────╯""")
     else:
         print(Fore.RED + " ## Please Check Your Internet Connection ##")
```

### Comparing `runflare-1.1.4/runflare/runflare_client/account/auth.py` & `runflare-1.1.5/runflare/runflare_client/account/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from runflare.settings import LOGIN_URL
 from runflare.runflare_client.data_manager.adapter import Adapter
 
 from colorama import Fore, Style
 
 
 def save_token(email=None,password=None):
-
     clear()
     if not email and not password:
         credentials = [
             inquirer.Text("email", message="Please enter your email > "),
             inquirer.Password("password", message="Please enter your password > "),
         ]
 
@@ -28,15 +27,14 @@
         token = response.json().get("token",None)
         Adapter.save_token(token=token, email=email)
         return Fore.GREEN + " Successfully Logged In"
     else:
         print(Fore.RED + " Wrong Credentials")
         exit()
 
-
 def del_token():
     clear()
 
     questions =[
         inquirer.Confirm("exit", message="Do you want to exit?"),
     ]
```

### Comparing `runflare-1.1.4/runflare/runflare_client/analyze/events.py` & `runflare-1.1.5/runflare/runflare_client/analyze/events.py`

 * *Files identical despite different names*

### Comparing `runflare-1.1.4/runflare/runflare_client/analyze/log.py` & `runflare-1.1.5/runflare/runflare_client/analyze/log.py`

 * *Files identical despite different names*

### Comparing `runflare-1.1.4/runflare/runflare_client/custom_pathlib.py` & `runflare-1.1.5/runflare/runflare_client/custom_pathlib.py`

 * *Files identical despite different names*

### Comparing `runflare-1.1.4/runflare/runflare_client/data_manager/adapter.py` & `runflare-1.1.5/runflare/runflare_client/data_manager/adapter.py`

 * *Files identical despite different names*

### Comparing `runflare-1.1.4/runflare/runflare_client/data_manager/sqlite_manager.py` & `runflare-1.1.5/runflare/runflare_client/data_manager/sqlite_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         cursor.execute(query)
 
 
     def save_token(self,token,email):
         self.conn = self.create_connection(self.main_db_path,self.db_name)
         self.cursor = self.conn.cursor()
         self.create_table(self.conn,"Token", token="VARCHAR(255)", email="VARCHAR(255)")
-        self.insert_into(self.conn,"Token",token=token, email=email)
+        self.insert_into(self.conn,"Token", token=token, email=email)
         self.close_connection(self.conn)
 
     def del_token(self):
         if os.path.exists(self.main_db_path+self.db_name):
 
             self.conn = self.create_connection(self.main_db_path, self.db_name)
             self.cursor = self.conn.cursor()
```

### Comparing `runflare-1.1.4/runflare/runflare_client/deploy/cache.py` & `runflare-1.1.5/runflare/runflare_client/deploy/cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from runflare import inquirer
 from runflare.runflare_client.data_manager.adapter import Adapter
-from runflare.runflare_client.service.projects import get_projects, get_project_items
+from runflare.runflare_client.service.projects import get_projects
 from runflare.settings import FOLDER_NAME,DOC_URL
 from colorama import init,Fore,Style
-from runflare.utils import clear
+from runflare.utils import clear, check_required_files
 
 
 class Cache_Manager:
 
     def __init__(self,root,type):
         self.root = root
         self.type = type
@@ -71,14 +71,15 @@
         return status,data
 
     def save_cache(self,project,project_id,service,service_id):
         Adapter.save_project_cache(self.local_db_path,project,project_id,service,service_id)
 
 
     def update_item(self,data):
+        print(data)
         status, response = get_project_items(data[1])
         if status:
             items = response.json()
             service = items.get("service", [])
             if self.type != "Deploy":
                 database = items.get("database", [])
 
@@ -136,18 +137,18 @@
         else:
             selected_service = None
             selected_service_id = None
         self.save_cache(data[0], data[1], selected_service, selected_service_id)
         return data[0], data[1], selected_service, selected_service_id
 
     def update_cache(self,email=None,password=None,namespace=None,app=None):
-
+        required_files = []
         status, response = get_projects(email=email,password=password)
         if status:
-            projects = response.json().get("projects",[])
+            projects = response.json()
         else:
             return Fore.RED + response
 
         if not projects:
             return Fore.RED + "Go To Runflare and Create Project First"
 
         choices = []
@@ -169,23 +170,18 @@
             selected_project = answer["project"]
         else:
             selected_project = namespace
 
         for project in projects:
             if project["namespace"] == selected_project:
                 selected_project_id = project["id"]
-                status, response = get_project_items(selected_project_id)
-                if status:
-                    items = response.json()
-                    service = items.get("service", [])
-                    if self.type != "Deploy":
-                        database = items.get("database", [])
-
-                else:
-                    return response
+                items = project.get("items")
+                service = items.get("service", [])
+                if self.type != "Deploy":
+                    database = items.get("database", [])
 
         if self.type != "Watch Events":
 
             if self.type != "Deploy":
                 item_type_prompt = [
                     inquirer.List(
                         "item_type",
@@ -203,22 +199,23 @@
             item_info = dict()
             if selected_item_type == "Service":
                 if service:
                     for item in service:
                         if item.get("status") != "ACTIVE":
                             not_active.append(item["name"])
                         choices.append(item["name"])
-                        item_info[item["name"]] = item["id"]
+                        item_info[item["name"]] = {}
+                        item_info[item["name"]]["id"] = item["id"]
+                        item_info[item["name"]]["required_files"] = item["required_files"]
 
                 else:
                     print(Fore.RED + "Selected Project doesn't have any `Service`")
                     print(Fore.RED + f"For more help please visit {DOC_URL}")
                     exit()
 
-
             elif selected_item_type == "Database":
                 if database:
                     for item in database:
                         if item.get("status") != "ACTIVE":
                             not_active.append(item["name"])
                         choices.append(item["name"])
                         item_info[item["name"]] = item["id"]
@@ -240,18 +237,27 @@
                 selected_service = answer["service"]
 
                 if selected_service in not_active:
                     print(Fore.RED + f"{selected_service} is not active")
                     print(Fore.RED + f"For more help please visit {DOC_URL}")
                     exit()
 
-
             else:
                 selected_service = app
-            selected_service_id = item_info[selected_service]
+            selected_service_id = item_info[selected_service].get("id")
+            required_files = item_info[selected_service].get("required_files")
         else:
             selected_service = None
             selected_service_id = None
-        self.save_cache(selected_project,selected_project_id,selected_service,selected_service_id)
-        return selected_project,selected_project_id,selected_service,selected_service_id
+
+        ok, files = check_required_files(required_files)
+
+        if not ok:
+            print(Fore.RED + f"For Your App You Must Have These Files/Directory!")
+            for f in files:
+                print(Fore.RED + f"  {f}")
+            exit()
+
+        self.save_cache(selected_project, selected_project_id, selected_service, selected_service_id)
+        return selected_project, selected_project_id, selected_service, selected_service_id
```

### Comparing `runflare-1.1.4/runflare/runflare_client/deploy/deployment.py` & `runflare-1.1.5/runflare/runflare_client/deploy/deployment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import json
 import os
 import shutil
 from time import sleep
 from runflare import inquirer
+import requests
 
 from runflare.runflare_client.requester import Requester
 
 from runflare.runflare_client.data_manager.adapter import Adapter
 from pprint import pprint
-from runflare.runflare_client.service.projects import get_projects, get_project_items
+from runflare.runflare_client.service.projects import get_projects
 from colorama import Fore, Style, init
 from runflare.utils import clear, compare, make_tar, list_to_dict, makedirs
 from .cache import Cache_Manager
 from .upload import upload, pre_upload_check, uploader_info
 import platform
 from runflare.runflare_client.service.manage import restart
-from ...settings import FOLDER_NAME, TAR_NAME, CHANGES_NAME, MAX_TRY, USER_HOME_PATH, RESTART_URL, LOG_URL
+from ...settings import FOLDER_NAME, TAR_NAME, CHANGES_NAME, MAX_TRY, USER_HOME_PATH, LOG_URL
 import sys
 from halo import Halo
 
 
 def deploy(y,email=None,password=None,namespace=None,app=None):
     try:
 
@@ -30,34 +31,35 @@
         selected_project, selected_service, selected_service_id = data[1], data[2], data[3]
 
         new, changed, deleted, _ = compare(project_root, send_all_files=False)
         any_change = any((new,changed,deleted))
         try_num = 1
         sp = Halo(text=Style.BRIGHT + f"Checking Upload Conditions", color="magenta")
         sp.start()
-        # while try_num <= MAX_TRY:
-        while try_num <= 1:
-            status, response = uploader_info(selected_service_id,any_change=any_change, spinner=sp)
+        while try_num <= MAX_TRY:
+            status, response = uploader_info(selected_service_id, any_change=any_change, spinner=sp)
             if "401" in response:
                 return "\n" + Fore.RED + response
             if status:
                 break
             try_num += 1
-            # sleep(2)
+            sleep(2)
         if not status:
             return "\n" + Fore.RED + response
         sp.stop()
         sys.stdout.write(f"\r √  Upload Conditions Verified\n")
 
         url = response.json().get("url")
+        url_mirror = response.json().get("url_mirror")
         token = response.json().get("token")
         free_disk = response.json().get("free_disk")
         restart_value = response.json().get("restart")
         log_identifier = response.json().get("log_identifier")
         send_all_files = response.json().get("send_all_files")
+
         if send_all_files:
             sp = Halo(text=Style.BRIGHT + f"Scaning All Directory {project_root}", color="magenta")
         else:
             sp = Halo(text=Style.BRIGHT + f"Scaning Directory {project_root}", color="magenta")
         sp.start()
         new, changed, deleted, scaned_files = compare(project_root,send_all_files=send_all_files)
         sp.stop()
@@ -65,48 +67,61 @@
         sys.stdout.write(f"\r √  Scaned {scaned_files} item(s)    {space}\n")
 
 
         if not new and not deleted and not changed:
             print(Fore.RED + "No New Files\nDirectory already synced with server !")
             exit()
 
+        compressed = False
+        for uploader_url in [url, url_mirror]:
 
-        status, response = pre_upload_check(url, token)
-        if not status:
-            return Fore.RED + response
+            if not uploader_url:
+                continue
 
-        makedirs(project_root + f"/{FOLDER_NAME}/")
-        changes_file_path = project_root + f"/{FOLDER_NAME}/{CHANGES_NAME}"
-        with open(changes_file_path, "w+") as changes:
-            changes.write(json.dumps({
-                "new": list_to_dict(new),
-                "count_of_new": len(new),
-                "modify": list_to_dict(changed),
-                "count_of_modify": len(changed),
-                "delete": list_to_dict(deleted),
-                "count_of_delete": len(deleted),
-                "log_identifier": log_identifier,
-            }, indent=4))
-        number_of_files = len(changed) + len(new)
-        sp = Halo(text=Style.BRIGHT + f"Compressing 0 of {number_of_files} item(s)", color="magenta")
-        sp.start()
-        i = 0
-        for i in make_tar(project_root, changed, new, changes_file_path=changes_file_path):
-            sp.text = (Style.BRIGHT + f"Compressing {str(i)} of {number_of_files} items")
-        sp.stop()
-        space = " " * len(str(number_of_files) + str(i))
-        sys.stdout.write(f"\r √  {number_of_files} item(s) Compressed  {space}\n")
+            status, response = pre_upload_check(uploader_url, token)
+            if not status:
+                return Fore.RED + response
+
+            if not compressed:
+                makedirs(project_root + f"/{FOLDER_NAME}/")
+                changes_file_path = project_root + f"/{FOLDER_NAME}/{CHANGES_NAME}"
+                with open(changes_file_path, "w+") as changes:
+                    changes.write(json.dumps({
+                        "new": list_to_dict(new),
+                        "count_of_new": len(new),
+                        "modify": list_to_dict(changed),
+                        "count_of_modify": len(changed),
+                        "delete": list_to_dict(deleted),
+                        "count_of_delete": len(deleted),
+                        "log_identifier": log_identifier,
+                    }, indent=4))
+                number_of_files = len(changed) + len(new)
+                sp = Halo(text=Style.BRIGHT + f"Compressing 0 of {number_of_files} item(s)", color="magenta")
+                sp.start()
+                i = 0
+                for i in make_tar(project_root, changed, new, changes_file_path=changes_file_path):
+                    sp.text = (Style.BRIGHT + f"Compressing {str(i)} of {number_of_files} items")
+                sp.stop()
+                space = " " * len(str(number_of_files) + str(i))
+                sys.stdout.write(f"\r √  {number_of_files} item(s) Compressed  {space}\n")
+
+                size = os.path.getsize(project_root + f"/{FOLDER_NAME}/{TAR_NAME}") / 1048576
+                if free_disk < size:
+                    print(Fore.RED + Style.BRIGHT + "Not Enough Disk,Please Upgrade Your Plan")
+                    exit()
+                compressed = True
 
-        size = os.path.getsize(project_root + f"/{FOLDER_NAME}/{TAR_NAME}") / 1048576
-        if free_disk < size:
-            print(Fore.RED + Style.BRIGHT + "Not Enough Disk,Please Upgrade Your Plan")
-            exit()
-        color = upload(project_root, url, token)
+            color = upload(project_root, uploader_url, token)
+
+            if color == "green":
+                color = Fore.GREEN
+                break
+            else:
+                color = Fore.RED
 
-        color = Fore.GREEN if color == "green" else Fore.RED
         if status:
             Adapter.save_last_deploy(project_root + f"/{FOLDER_NAME}/")
             os.remove(project_root + f"/{FOLDER_NAME}/{TAR_NAME}")
             os.remove(project_root + f"/{FOLDER_NAME}/{CHANGES_NAME}")
             if color == Fore.GREEN:
                 result = "\n\n {}Files Successfully Uploaded {:.3f} MB".format(color + Style.BRIGHT, size)
                 result += "\n\n  Scaned Files :{} \n   {}New Files :{} \n   Changed Files :{} \n   Deleted Files :{}\n".format(
@@ -120,14 +135,20 @@
                         inquirer.Confirm("log", message="Deployment takes time,Do you want to Watch log?"),
                     ]
 
                     questions = inquirer.prompt(questions)
                     answer = questions["log"]
                     if answer:
                         from runflare.runflare_client.web_socket import Socket
+                        print("Your Files Successfully uploaded To Server.")
+                        sleep(6)
+                        print("New Version will be replaced soon ...")
+                        sleep(6)
+                        print("Trying to watch logs ...")
+                        sleep(6)
                         Socket().run_loop("watch", LOG_URL, data[3])
             return
         else:
             return Fore.RED + response
     except KeyboardInterrupt:
         print(Fore.RED + Style.BRIGHT + f"\n\n X  ERORR - Cancelled By User")
         exit()
@@ -178,7 +199,8 @@
             if os.path.exists(path):
                 shutil.rmtree(path)
         main_root = str(USER_HOME_PATH) + f"/{FOLDER_NAME}/"
         shutil.rmtree(main_root)
         print(Fore.GREEN + "Successfully Cleaned")
     else:
         print(Fore.RED + "Choose Carefully")
+
```

### Comparing `runflare-1.1.4/runflare/runflare_client/deploy/upload.py` & `runflare-1.1.5/runflare/runflare_client/deploy/upload.py`

 * *Files identical despite different names*

### Comparing `runflare-1.1.4/runflare/runflare_client/requester.py` & `runflare-1.1.5/runflare/runflare_client/requester.py`

 * *Files identical despite different names*

### Comparing `runflare-1.1.4/runflare/runflare_client/service/manage.py` & `runflare-1.1.5/runflare/runflare_client/service/manage.py`

 * *Files identical despite different names*

### Comparing `runflare-1.1.4/runflare/runflare_client/web_socket.py` & `runflare-1.1.5/runflare/runflare_client/web_socket.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import time
 class Socket:
 
     async def watch(self,url,id):
         clear()
         print(Style.BRIGHT + "Intialize Secure Session")
         url = WEBSOCKET_URL + "/ws/{}/{}/?token={}".format(url,id, self._get_token())
-        time.sleep(5)
+        time.sleep(6)
         try:
             ssl_context = ssl.SSLContext()
             ssl_context.verify_mode = ssl.CERT_NONE
             ssl_context.check_hostname = False
             async with websockets.connect(url,ssl=ssl_context) as ws:
                 print(Fore.GREEN + Style.BRIGHT + "Connected")
                 while True:
```

### Comparing `runflare-1.1.4/runflare/settings.py` & `runflare-1.1.5/runflare/settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 import platform
 from pathlib import Path
 
-
+#
 BASE_URL = "https://api.runflare.com"
 WEBSOCKET_URL = 'wss://api.runflare.com'
+
 FOLDER_NAME = ".cloud"
 DATASTORE = {
     "BACKEND": "sqlite3",
     "NAME": "db.sqlite3",
 }
 TAR_NAME = "workspace.tar.gz"
 CHANGES_NAME = "changes.json"
-
 LOGIN_URL = '/account/login/'
-PROJECT_LIST_URL = '/project/?filter=ACTIVE'
-ITEM_LIST_URL = '/project/items-show/{}/'
+PROJECT_LIST_URL = '/api/v1/projects/cli/'
 UPLOAD_URL = "/project/deploy/{}/"
 START_URL = "/project/deployment-start/{}/"
 STOP_URL = "/project/deployment-stop/{}/"
 RESTART_URL = "/project/deployment-restart/{}/"
 VERSION_URL = "/version/"
 
 
 NR_LOG_URL = "/project/pod-log/{}/"
 NR_EVENTS_URL = '/project/events/{}/'
 
 
 DOC_URL = 'https://runflare.com/docs/get-started/'
-
 MAX_TRY = 3
 
 LOG_URL = "pod-log"
 EVENTS_URL = "project-events"
 
 
 OS_SYSTEM = platform.system()
```

### Comparing `runflare-1.1.4/runflare/utils.py` & `runflare-1.1.5/runflare/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -161,7 +161,16 @@
         full_path = project_root + "/.gitignore"
         with open(full_path, "r+") as default_ignored:
             lst = list(map(lambda x: x.strip("\n"), default_ignored.readlines()))
             for item in DEFAULT_IGNORE_FILE:
                 if item not in lst:
                     default_ignored.write(f"\n{item}")
     return full_path
+
+def check_required_files(required_files):
+    not_exists = []
+    for f in required_files:
+        if not os.path.exists(f):
+            not_exists.append(f)
+    if not_exists:
+        return False, not_exists
+    return True, []
```

### Comparing `runflare-1.1.4/runflare/version_check.py` & `runflare-1.1.5/runflare/version_check.py`

 * *Files 7% similar despite different names*

```diff
@@ -78,30 +78,32 @@
         except:
             return Version("0")
         if request.status_code == 503:
             clear()
             print(Fore.RED + f"\nRunflare Is Under Maintance, Please Try Again Later")
             exit()
         elif request.status_code != 200:
-            return Version("0")
+            return Version("0"), None
         ok,response = request.ok,request.json()
         if ok:
-            return Version(response.get("version"))
+            return Version(response.get("version")),Version(response.get("minimum_version"))
         else:
             return Version.get_current_version()
 
 
     @staticmethod
     def get_current_version():
         return Version(VERSION)
 
     @staticmethod
     @Halo(text=Style.BRIGHT + "Preparing ...", color="magenta")
-    def has_new_version():
+    def check_version():
         current_version = Version.get_current_version()
-        latest_version = Version.get_latest_version()
+        latest_version, minimum_version = Version.get_latest_version()
         if latest_version == Version("0"):
             return 0
-        if latest_version > current_version:
+        if minimum_version > current_version:
+            return 3
+        elif latest_version > current_version:
             return 2
         else:
-            return 1
+            return 1
```

### Comparing `runflare-1.1.4/runflare.egg-info/SOURCES.txt` & `runflare-1.1.5/runflare.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `runflare-1.1.4/setup.py` & `runflare-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         'idna==3.2',
         'log-symbols==0.0.14',
         'Pygments==2.10.0',
         "blessed==1.19.0",
         'readchar==2.0.1',
         'python-editor==1.0.4',
         'pytz==2021.3',
-        'regex==2021.10.8',
+        'regex==2023.6.3',
         'requests==2.26.0',
         'requests-toolbelt==0.9.1',
         'six==1.16.0',
         'spinners==0.0.24',
         'termcolor==1.1.0',
         'tzdata==2021.2.post0',
         'tzlocal==3.0',
```

