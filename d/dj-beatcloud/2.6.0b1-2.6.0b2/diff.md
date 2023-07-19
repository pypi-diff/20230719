# Comparing `tmp/dj_beatcloud-2.6.0b1.tar.gz` & `tmp/dj_beatcloud-2.6.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_beatcloud-2.6.0b1.tar", last modified: Mon Jul 17 23:19:11 2023, max compression
+gzip compressed data, was "dj_beatcloud-2.6.0b2.tar", last modified: Wed Jul 19 05:20:29 2023, max compression
```

## Comparing `dj_beatcloud-2.6.0b1.tar` & `dj_beatcloud-2.6.0b2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-17 23:19:11.668217 dj_beatcloud-2.6.0b1/
--rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.6.0b1/LICENSE
--rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-26 19:42:57.000000 dj_beatcloud-2.6.0b1/MANIFEST.in
--rw-r--r--   0 alrichards   (502) staff       (20)     2575 2023-07-17 23:19:11.668380 dj_beatcloud-2.6.0b1/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1319 2023-05-26 21:16:19.000000 dj_beatcloud-2.6.0b1/README.md
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-17 23:19:11.513790 dj_beatcloud-2.6.0b1/dj_beatcloud.egg-info/
--rw-r--r--   0 alrichards   (502) staff       (20)     2575 2023-07-17 23:19:11.000000 dj_beatcloud-2.6.0b1/dj_beatcloud.egg-info/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1248 2023-07-17 23:19:11.000000 dj_beatcloud-2.6.0b1/dj_beatcloud.egg-info/SOURCES.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-07-17 23:19:11.000000 dj_beatcloud-2.6.0b1/dj_beatcloud.egg-info/dependency_links.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-07-17 23:19:11.000000 dj_beatcloud-2.6.0b1/dj_beatcloud.egg-info/entry_points.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-07-17 23:19:11.000000 dj_beatcloud-2.6.0b1/dj_beatcloud.egg-info/requires.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-07-17 23:19:11.000000 dj_beatcloud-2.6.0b1/dj_beatcloud.egg-info/top_level.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-17 23:19:11.525350 dj_beatcloud-2.6.0b1/djtools/
--rw-r--r--   0 alrichards   (502) staff       (20)     2543 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1776 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/__main__.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-17 23:19:11.617071 dj_beatcloud-2.6.0b1/djtools/collections/
--rw-r--r--   0 alrichards   (502) staff       (20)     1434 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/collections/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)    12878 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/collections/collections.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2810 2023-07-17 22:44:15.000000 dj_beatcloud-2.6.0b1/djtools/collections/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2515 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/collections/copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)    27150 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/collections/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     7584 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/collections/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)    15833 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/collections/playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2405 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/collections/shuffle_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)    13832 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/collections/tracks.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-17 23:19:11.649746 dj_beatcloud-2.6.0b1/djtools/configs/
--rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b1/djtools/configs/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1179 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/configs/collection_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)     1765 2023-07-17 22:43:41.000000 dj_beatcloud-2.6.0b1/djtools/configs/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1301 2023-07-17 23:15:45.000000 dj_beatcloud-2.6.0b1/djtools/configs/config.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)    15653 2023-07-17 23:14:09.000000 dj_beatcloud-2.6.0b1/djtools/configs/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b1/djtools/configs/logging.conf
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b1/djtools/configs/spotify_playlists.yaml
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-17 23:19:11.650762 dj_beatcloud-2.6.0b1/djtools/logs/
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b1/djtools/logs/empty.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-17 23:19:11.657011 dj_beatcloud-2.6.0b1/djtools/spotify/
--rw-r--r--   0 alrichards   (502) staff       (20)      735 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/spotify/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3258 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/spotify/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    16599 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/spotify/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6053 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/spotify/playlist_builder.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-17 23:19:11.661345 dj_beatcloud-2.6.0b1/djtools/sync/
--rw-r--r--   0 alrichards   (502) staff       (20)      825 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/sync/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3535 2023-07-17 22:33:04.000000 dj_beatcloud-2.6.0b1/djtools/sync/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     7959 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/djtools/sync/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4888 2023-07-17 21:15:05.000000 dj_beatcloud-2.6.0b1/djtools/sync/sync_operations.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-17 23:19:11.667129 dj_beatcloud-2.6.0b1/djtools/utils/
--rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-07-15 20:42:42.000000 dj_beatcloud-2.6.0b1/djtools/utils/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3660 2023-07-15 20:42:42.000000 dj_beatcloud-2.6.0b1/djtools/utils/check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1409 2023-07-17 22:43:18.000000 dj_beatcloud-2.6.0b1/djtools/utils/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    10158 2023-07-15 20:42:42.000000 dj_beatcloud-2.6.0b1/djtools/utils/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b1/djtools/utils/url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)       92 2023-07-17 23:16:00.000000 dj_beatcloud-2.6.0b1/djtools/version.py
--rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 dj_beatcloud-2.6.0b1/pyproject.toml
--rw-r--r--   0 alrichards   (502) staff       (20)       99 2023-07-17 23:19:11.668902 dj_beatcloud-2.6.0b1/setup.cfg
--rw-r--r--   0 alrichards   (502) staff       (20)     2371 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b1/setup.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 05:20:29.476716 dj_beatcloud-2.6.0b2/
+-rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.6.0b2/LICENSE
+-rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-26 19:42:57.000000 dj_beatcloud-2.6.0b2/MANIFEST.in
+-rw-r--r--   0 alrichards   (502) staff       (20)     2556 2023-07-19 05:20:29.476814 dj_beatcloud-2.6.0b2/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1319 2023-05-26 21:16:19.000000 dj_beatcloud-2.6.0b2/README.md
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 05:20:29.460146 dj_beatcloud-2.6.0b2/dj_beatcloud.egg-info/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2556 2023-07-19 05:20:29.000000 dj_beatcloud-2.6.0b2/dj_beatcloud.egg-info/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1248 2023-07-19 05:20:29.000000 dj_beatcloud-2.6.0b2/dj_beatcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-07-19 05:20:29.000000 dj_beatcloud-2.6.0b2/dj_beatcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-07-19 05:20:29.000000 dj_beatcloud-2.6.0b2/dj_beatcloud.egg-info/entry_points.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-07-19 05:20:29.000000 dj_beatcloud-2.6.0b2/dj_beatcloud.egg-info/requires.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-07-19 05:20:29.000000 dj_beatcloud-2.6.0b2/dj_beatcloud.egg-info/top_level.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 05:20:29.461753 dj_beatcloud-2.6.0b2/djtools/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2543 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1776 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/__main__.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 05:20:29.466400 dj_beatcloud-2.6.0b2/djtools/collections/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1434 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/collections/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    12878 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/collections/collections.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2810 2023-07-19 05:18:06.000000 dj_beatcloud-2.6.0b2/djtools/collections/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2515 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/collections/copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    27150 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/collections/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7584 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/collections/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    15833 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/collections/playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2405 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/collections/shuffle_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    13832 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/collections/tracks.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 05:20:29.469762 dj_beatcloud-2.6.0b2/djtools/configs/
+-rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b2/djtools/configs/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1179 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/configs/collection_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)     1765 2023-07-19 05:18:06.000000 dj_beatcloud-2.6.0b2/djtools/configs/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1301 2023-07-19 05:18:23.000000 dj_beatcloud-2.6.0b2/djtools/configs/config.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)    15665 2023-07-19 05:18:06.000000 dj_beatcloud-2.6.0b2/djtools/configs/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b2/djtools/configs/logging.conf
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b2/djtools/configs/spotify_playlists.yaml
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 05:20:29.470030 dj_beatcloud-2.6.0b2/djtools/logs/
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b2/djtools/logs/empty.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 05:20:29.471415 dj_beatcloud-2.6.0b2/djtools/spotify/
+-rw-r--r--   0 alrichards   (502) staff       (20)      735 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/spotify/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3258 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/spotify/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    16599 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/spotify/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6053 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/spotify/playlist_builder.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 05:20:29.473956 dj_beatcloud-2.6.0b2/djtools/sync/
+-rw-r--r--   0 alrichards   (502) staff       (20)      825 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/sync/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3535 2023-07-19 05:18:06.000000 dj_beatcloud-2.6.0b2/djtools/sync/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7647 2023-07-19 05:18:06.000000 dj_beatcloud-2.6.0b2/djtools/sync/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5170 2023-07-19 05:18:06.000000 dj_beatcloud-2.6.0b2/djtools/sync/sync_operations.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 05:20:29.476369 dj_beatcloud-2.6.0b2/djtools/utils/
+-rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-07-15 20:42:42.000000 dj_beatcloud-2.6.0b2/djtools/utils/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3660 2023-07-15 20:42:42.000000 dj_beatcloud-2.6.0b2/djtools/utils/check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1409 2023-07-19 05:18:06.000000 dj_beatcloud-2.6.0b2/djtools/utils/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    10160 2023-07-19 05:18:06.000000 dj_beatcloud-2.6.0b2/djtools/utils/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b2/djtools/utils/url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)       92 2023-07-19 05:19:41.000000 dj_beatcloud-2.6.0b2/djtools/version.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 dj_beatcloud-2.6.0b2/pyproject.toml
+-rw-r--r--   0 alrichards   (502) staff       (20)       99 2023-07-19 05:20:29.477169 dj_beatcloud-2.6.0b2/setup.cfg
+-rw-r--r--   0 alrichards   (502) staff       (20)     2346 2023-07-19 05:18:06.000000 dj_beatcloud-2.6.0b2/setup.py
```

### Comparing `dj_beatcloud-2.6.0b1/LICENSE` & `dj_beatcloud-2.6.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/PKG-INFO` & `dj_beatcloud-2.6.0b2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: dj_beatcloud
-Version: 2.6.0b1
+Version: 2.6.0b2
 Summary: DJ Tools is a library for managing a collection of music.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
-License: GNU GPLv3
 Keywords: DJ Rekordbox spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,34 +1,33 @@
-Metadata-Version: 2.1 Name: dj_beatcloud Version: 2.6.0b1 Summary: DJ Tools is
+Metadata-Version: 2.1 Name: dj_beatcloud Version: 2.6.0b2 Summary: DJ Tools is
 a library for managing a collection of music. Home-page: https://github.com/a-
 rich/DJ-tools Author: Alex Richards Author-email: alex.richards006@gmail.com
-License: GNU GPLv3 Keywords: DJ Rekordbox spotify reddit aws s3 Classifier:
-Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop Classifier: Intended
-Audience :: Other Audience Classifier: License :: OSI Approved :: GNU General
-Public License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
-Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
-:: Windows Classifier: Operating System :: POSIX :: Linux Classifier:
-Programming Language :: Python :: 3.6 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Topic :: Multimedia :: Sound/Audio Classifier: Topic :: Other/Nonlisted Topic
-Requires-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra:
-levenshtein License-File: LICENSE # DJ Tools [![image](https://img.shields.io/
-pypi/v/dj-beatcloud.svg)](https://pypi.org/project/dj-beatcloud/) Please see
-the [docs](https://a-rich.github.io/DJ-Tools/) for tutorials, how-to guides,
-conceptual guides, and references! # Release Plan * 2.5.1 - [ ] [Stability
-issues with requests to the search endpoint of the Spotify API](https://
-github.com/a-rich/DJ-Tools/issues/58) - [ ] [Make Spotify API calls
-asynchronous](https://github.com/a-rich/DJ-Tools/issues/38) - [ ] [Print ASCII
-histogram of tag statistics for Combiner playlists](https://github.com/a-rich/
-DJ-Tools/issues/87) - [x] [Deprecate registered_users.yaml](https://github.com/
-a-rich/DJ-Tools/issues/99) - [x] [Parameterize whether Beatcloud tracks should
-be read as
+Keywords: DJ Rekordbox spotify reddit aws s3 Classifier: Development Status ::
+4 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: End Users/Desktop Classifier: Intended Audience :: Other Audience
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English Classifier: Operating System :: MacOS
+:: MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
+Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
+:: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Multimedia ::
+Sound/Audio Classifier: Topic :: Other/Nonlisted Topic Requires-Python: >=3.6
+Description-Content-Type: text/markdown Provides-Extra: levenshtein License-
+File: LICENSE # DJ Tools [![image](https://img.shields.io/pypi/v/dj-
+beatcloud.svg)](https://pypi.org/project/dj-beatcloud/) Please see the [docs]
+(https://a-rich.github.io/DJ-Tools/) for tutorials, how-to guides, conceptual
+guides, and references! # Release Plan * 2.5.1 - [ ] [Stability issues with
+requests to the search endpoint of the Spotify API](https://github.com/a-rich/
+DJ-Tools/issues/58) - [ ] [Make Spotify API calls asynchronous](https://
+github.com/a-rich/DJ-Tools/issues/38) - [ ] [Print ASCII histogram of tag
+statistics for Combiner playlists](https://github.com/a-rich/DJ-Tools/issues/
+87) - [x] [Deprecate registered_users.yaml](https://github.com/a-rich/DJ-Tools/
+issues/99) - [x] [Parameterize whether Beatcloud tracks should be read as
  or vice versa](https://github.com/a-rich/DJ-Tools/issues/95) * 2.6.0 - [ ]
 [Create serializers package for converting database files from other DJ
 software (e.g. Serato, Traktor, Denon, etc.) so that operations in the
 rekordbox package can be used on them](https://github.com/a-rich/DJ-Tools/
 issues/68) - [ ] [Improve Reddit submission title parsing in order to improve
 precision and recall of Spotify API search results](https://github.com/a-rich/
 DJ-Tools/issues/59) # Contribution Please see the [CONTRIBUTING]
```

### Comparing `dj_beatcloud-2.6.0b1/README.md` & `dj_beatcloud-2.6.0b2/README.md`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/dj_beatcloud.egg-info/PKG-INFO` & `dj_beatcloud-2.6.0b2/dj_beatcloud.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: dj-beatcloud
-Version: 2.6.0b1
+Version: 2.6.0b2
 Summary: DJ Tools is a library for managing a collection of music.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
-License: GNU GPLv3
 Keywords: DJ Rekordbox spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,34 +1,33 @@
-Metadata-Version: 2.1 Name: dj-beatcloud Version: 2.6.0b1 Summary: DJ Tools is
+Metadata-Version: 2.1 Name: dj-beatcloud Version: 2.6.0b2 Summary: DJ Tools is
 a library for managing a collection of music. Home-page: https://github.com/a-
 rich/DJ-tools Author: Alex Richards Author-email: alex.richards006@gmail.com
-License: GNU GPLv3 Keywords: DJ Rekordbox spotify reddit aws s3 Classifier:
-Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop Classifier: Intended
-Audience :: Other Audience Classifier: License :: OSI Approved :: GNU General
-Public License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
-Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
-:: Windows Classifier: Operating System :: POSIX :: Linux Classifier:
-Programming Language :: Python :: 3.6 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Topic :: Multimedia :: Sound/Audio Classifier: Topic :: Other/Nonlisted Topic
-Requires-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra:
-levenshtein License-File: LICENSE # DJ Tools [![image](https://img.shields.io/
-pypi/v/dj-beatcloud.svg)](https://pypi.org/project/dj-beatcloud/) Please see
-the [docs](https://a-rich.github.io/DJ-Tools/) for tutorials, how-to guides,
-conceptual guides, and references! # Release Plan * 2.5.1 - [ ] [Stability
-issues with requests to the search endpoint of the Spotify API](https://
-github.com/a-rich/DJ-Tools/issues/58) - [ ] [Make Spotify API calls
-asynchronous](https://github.com/a-rich/DJ-Tools/issues/38) - [ ] [Print ASCII
-histogram of tag statistics for Combiner playlists](https://github.com/a-rich/
-DJ-Tools/issues/87) - [x] [Deprecate registered_users.yaml](https://github.com/
-a-rich/DJ-Tools/issues/99) - [x] [Parameterize whether Beatcloud tracks should
-be read as
+Keywords: DJ Rekordbox spotify reddit aws s3 Classifier: Development Status ::
+4 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: End Users/Desktop Classifier: Intended Audience :: Other Audience
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English Classifier: Operating System :: MacOS
+:: MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
+Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
+:: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Multimedia ::
+Sound/Audio Classifier: Topic :: Other/Nonlisted Topic Requires-Python: >=3.6
+Description-Content-Type: text/markdown Provides-Extra: levenshtein License-
+File: LICENSE # DJ Tools [![image](https://img.shields.io/pypi/v/dj-
+beatcloud.svg)](https://pypi.org/project/dj-beatcloud/) Please see the [docs]
+(https://a-rich.github.io/DJ-Tools/) for tutorials, how-to guides, conceptual
+guides, and references! # Release Plan * 2.5.1 - [ ] [Stability issues with
+requests to the search endpoint of the Spotify API](https://github.com/a-rich/
+DJ-Tools/issues/58) - [ ] [Make Spotify API calls asynchronous](https://
+github.com/a-rich/DJ-Tools/issues/38) - [ ] [Print ASCII histogram of tag
+statistics for Combiner playlists](https://github.com/a-rich/DJ-Tools/issues/
+87) - [x] [Deprecate registered_users.yaml](https://github.com/a-rich/DJ-Tools/
+issues/99) - [x] [Parameterize whether Beatcloud tracks should be read as
  or vice versa](https://github.com/a-rich/DJ-Tools/issues/95) * 2.6.0 - [ ]
 [Create serializers package for converting database files from other DJ
 software (e.g. Serato, Traktor, Denon, etc.) so that operations in the
 rekordbox package can be used on them](https://github.com/a-rich/DJ-Tools/
 issues/68) - [ ] [Improve Reddit submission title parsing in order to improve
 precision and recall of Spotify API search results](https://github.com/a-rich/
 DJ-Tools/issues/59) # Contribution Please see the [CONTRIBUTING]
```

### Comparing `dj_beatcloud-2.6.0b1/dj_beatcloud.egg-info/SOURCES.txt` & `dj_beatcloud-2.6.0b2/dj_beatcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/djtools/__init__.py` & `dj_beatcloud-2.6.0b2/djtools/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/djtools/__main__.py` & `dj_beatcloud-2.6.0b2/djtools/__main__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/djtools/collections/__init__.py` & `dj_beatcloud-2.6.0b2/djtools/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/djtools/collections/collections.py` & `dj_beatcloud-2.6.0b2/djtools/collections/collections.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/djtools/collections/config.py` & `dj_beatcloud-2.6.0b2/djtools/collections/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/djtools/collections/copy_playlists.py` & `dj_beatcloud-2.6.0b2/djtools/collections/copy_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/djtools/collections/helpers.py` & `dj_beatcloud-2.6.0b2/djtools/collections/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/djtools/collections/playlist_builder.py` & `dj_beatcloud-2.6.0b2/djtools/collections/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/djtools/collections/playlists.py` & `dj_beatcloud-2.6.0b2/djtools/collections/playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/djtools/collections/shuffle_playlists.py` & `dj_beatcloud-2.6.0b2/djtools/collections/shuffle_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/djtools/collections/tracks.py` & `dj_beatcloud-2.6.0b2/djtools/collections/tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/djtools/configs/collection_playlists.yaml` & `dj_beatcloud-2.6.0b2/djtools/configs/collection_playlists.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/djtools/configs/config.py` & `dj_beatcloud-2.6.0b2/djtools/configs/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/djtools/configs/config.yaml` & `dj_beatcloud-2.6.0b2/djtools/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/djtools/configs/helpers.py` & `dj_beatcloud-2.6.0b2/djtools/configs/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     )
     subparsers = parser.add_subparsers(title="subcommands")
 
     ###########################################################################
     # Sub-command for the collections package.
     ###########################################################################
     collections_parser = subparsers.add_parser("collections")
-    parser.add_argument(
+    collections_parser.add_argument(
         "--collection-path",
         type=convert_to_paths,
         help='Path to a collection database',
     )
     collections_parser.add_argument(
         "--collection-playlists",
         action="store_true",
```

### Comparing `dj_beatcloud-2.6.0b1/djtools/spotify/__init__.py` & `dj_beatcloud-2.6.0b2/djtools/spotify/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/djtools/spotify/config.py` & `dj_beatcloud-2.6.0b2/djtools/spotify/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/djtools/spotify/helpers.py` & `dj_beatcloud-2.6.0b2/djtools/spotify/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/djtools/spotify/playlist_builder.py` & `dj_beatcloud-2.6.0b2/djtools/spotify/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/djtools/sync/__init__.py` & `dj_beatcloud-2.6.0b2/djtools/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/djtools/sync/config.py` & `dj_beatcloud-2.6.0b2/djtools/sync/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/djtools/sync/helpers.py` & `dj_beatcloud-2.6.0b2/djtools/sync/helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -113,61 +113,52 @@
 
     Raises:
         CalledProcessError: raised if "aws s3 sync" command fails.
 
     Returns:
         Formatted list of uploaded tracks; tracks are grouped by directory.
     """
+    line = ""
+    termination_chars = {"\n", "\r"}
     tracks = []
     try:
-        with Popen(_cmd, stdout=PIPE, universal_newlines=True) as proc:
+        with Popen(_cmd, stdout=PIPE) as proc:
             while True:
-                line = proc.stdout.readline()
-                if line == "" and proc.poll() is not None:
+                char = proc.stdout.read(1).decode()
+                if char == "" and proc.poll() is not None:
                     break
-                if "upload: " in line:
-                    print(line.strip(), flush=True)
-                    tracks.append(
-                        line.strip().split(
-                            " to s3://dj.beatcloud.com/dj/music/"
-                        )[-1]
-                    )
-                else:
-                    print(
-                        f"{line.strip()}                                  "
-                        "                        ",
-                        end="\r", flush=True
-                    )
-
+                if char not in termination_chars:
+                    line += char
+                    continue
+                print(line, end=char)
+                if char != "\r" and "upload: " in line:
+                    line = line.split("s3://dj.beatcloud.com/dj/music/")[-1]
+                    tracks.append(Path(line))
+                line = ""
             proc.stdout.close()
             return_code = proc.wait()
         if return_code:
             raise CalledProcessError(return_code, " ".join(_cmd))
     except Exception as exc:
         msg = f"Failure while syncing: {exc}"
         logger.critical(msg)
         raise Exception(msg) from exc
 
     new_music = ""
-    if tracks:
-        logger.info(
-            f'Successfully {"down" if "s3://" in _cmd[3] else "up"}loaded the '
-            "following tracks:"
-        )
     for group_id, group in groupby(
-        sorted(tracks, key=lambda x: "/".join(x.split("/")[:-1])),
-        key=lambda x: "/".join(x.split("/")[:-1]),
+        sorted(tracks, key=lambda x: x.parent), key=lambda x: x.parent
     ):
         group = sorted(group)
         new_music += f"{group_id}: {len(group)}\n"
         for track in group:
-            track = track.split("/")[-1]
-            new_music += f"\t{track}\n"
+            new_music += f"\t{track.name}\n"
     if new_music:
-        logger.info(new_music)
+        logger.info(
+            f"Successfully uploaded {len(tracks)} tracks:\n{new_music}"
+        )
 
     return new_music
 
 
 def upload_log(config: BaseConfig, log_file: Path):
     """This function uploads "log_file" to the "USER" logs folder in S3. It
         then deletes all files created more than one day ago.
@@ -180,17 +171,17 @@
         logger.warning(
             "Logs cannot be backed up without specifying the config option "
             "AWS_PROFILE"
         )
         return
 
     dst = f"s3://dj.beatcloud.com/dj/logs/{config.USER}/{log_file.name}"
-    cmd = f"aws s3 cp {log_file.as_posix()} {dst}"
-    logger.info(cmd)
-    with Popen(cmd, shell=True) as proc:
+    cmd = ["aws", "s3", "cp", log_file.as_posix(), dst]
+    logger.info(" ".join(cmd))
+    with Popen(cmd) as proc:
         proc.wait()
 
     now = datetime.now()
     one_day = timedelta(days=1)
     for _file in log_file.parent.rglob("*"):
         if _file.name == "empty.txt":
             continue
```

### Comparing `dj_beatcloud-2.6.0b1/djtools/sync/sync_operations.py` & `dj_beatcloud-2.6.0b2/djtools/sync/sync_operations.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,20 +40,20 @@
         )
         config.DOWNLOAD_INCLUDE_DIRS = [
             (Path(user) / path.split(f"{Path(user)}/")[-1])
             for path in beatcloud_matches
         ]
         config.DOWNLOAD_EXCLUDE_DIRS = []
 
+    logger.info("Downloading track collection...")
     dest = Path(config.USB_PATH) / "DJ Music"
     glob_path = (Path("**") / "*.*").as_posix()
     old = {str(p) for p in dest.rglob(glob_path)}
-    logger.info(f"Found {len(old)} files")
+    logger.info(f"Found {len(old)} files at {config.USB_PATH}")
 
-    logger.info("Downloading track collection...")
     dest.mkdir(parents=True, exist_ok=True)
     cmd = [
         "aws", "s3", "sync", "s3://dj.beatcloud.com/dj/music/", dest.as_posix()
     ]
     run_sync(parse_sync_command(cmd, config))
 
     new = {str(p) for p in dest.rglob(glob_path)}
@@ -71,30 +71,34 @@
     
     After downloading "IMPORT_USER"'s collection, the location of all the
     tracks are modified so that they point to USER's "USB_PATH".
 
     Args:
         config: Configuration object.
     """
-    logger.info(f"Downloading {config.IMPORT_USER}'s collection...")
+    logger.info(
+        f"Downloading {config.IMPORT_USER}'s {config.PLATFORM} collection..."
+    )
     collection_dir = config.COLLECTION_PATH.parent
-    collection_dir.mkdir(parents=True, exist_ok=True)
-    _file = (
+    src = (
+        f"s3://dj.beatcloud.com/dj/collections/{config.IMPORT_USER}/"
+        f"{config.PLATFORM}_collection"
+    )
+    dst = (
         Path(collection_dir) /
         f'{config.IMPORT_USER}_{config.COLLECTION_PATH.name}'
     )
-    cmd = (
-        "aws s3 cp s3://dj.beatcloud.com/dj/collections/"
-        f'{config.IMPORT_USER}/collection {_file}'
-    )
-    logger.info(cmd)
-    with Popen(cmd, shell=True) as proc:
+    cmd = ["aws", "s3", "cp", src, dst.as_posix()]
+    if config.COLLECTION_PATH.is_dir():
+        cmd.append("--recursive")
+    logger.info(" ".join(cmd))
+    with Popen(cmd) as proc:
         proc.wait()
     if config.USER != config.IMPORT_USER:
-        rewrite_track_paths(config, _file)
+        rewrite_track_paths(config, dst)
 
 
 def upload_music(config: BaseConfig):
     """This function syncs tracks from "USB_PATH" to the Beatcloud.
 
     "AWS_USE_DATE_MODIFIED" can be used in order to re-upload tracks that
     already exist in the Beatcloud but have been modified since the last time
@@ -129,13 +133,21 @@
 
 def upload_collection(config: BaseConfig):
     """This function uploads "COLLECTION_PATH" to the cloud.
 
     Args:
         config: Configuration object.
     """
-    logger.info(f"Uploading {config.USER}'s collection...")
-    dst = f"s3://dj.beatcloud.com/dj/collections/{config.USER}/collection"
-    cmd = f"aws s3 cp {config.COLLECTION_PATH} {dst}"
-    logger.info(cmd)
-    with Popen(cmd, shell=True) as proc:
+    logger.info(
+        f"Uploading {config.USER}'s {config.PLATFORM} collection..."
+    )
+    dst = (
+      f"s3://dj.beatcloud.com/dj/collections/{config.USER}/"
+      f"{config.PLATFORM}_collection"
+    )
+    cmd = ["aws", "s3", "cp", config.COLLECTION_PATH.as_posix(), dst]
+    if config.COLLECTION_PATH.is_dir():
+        cmd.append("--recursive")
+    logger.info(" ".join(cmd))
+    with Popen(cmd) as proc:
+
         proc.wait()
```

### Comparing `dj_beatcloud-2.6.0b1/djtools/utils/__init__.py` & `dj_beatcloud-2.6.0b2/djtools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/djtools/utils/check_tracks.py` & `dj_beatcloud-2.6.0b2/djtools/utils/check_tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/djtools/utils/config.py` & `dj_beatcloud-2.6.0b2/djtools/utils/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/djtools/utils/helpers.py` & `dj_beatcloud-2.6.0b2/djtools/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,16 +167,16 @@
 def get_beatcloud_tracks() -> List[str]:
     """Lists all the music files in S3 and parses out the track titles and
         artist names.
     
     Returns:
         Beatcloud track titles and artist names.
     """
-    cmd = "aws s3 ls --recursive s3://dj.beatcloud.com/dj/music/"
-    output = check_output(cmd, shell=True).decode("utf-8").split("\n")
+    cmd = ["aws", "s3", "ls", "--recursive", "s3://dj.beatcloud.com/dj/music/"]
+    output = check_output(cmd).decode("utf-8").split("\n")
     tracks = [Path(track) for track in output if track]
     logger.info(f"Got {len(tracks)} tracks from the beatcloud")
 
     return tracks
 
 
 def get_local_tracks(config: BaseConfig) -> Dict[str, List[str]]:
```

### Comparing `dj_beatcloud-2.6.0b1/djtools/utils/url_download.py` & `dj_beatcloud-2.6.0b2/djtools/utils/url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b1/setup.py` & `dj_beatcloud-2.6.0b2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     version=VERSION,
     description='DJ Tools is a library for managing a collection of music.',
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url='https://github.com/a-rich/DJ-tools',
     author='Alex Richards',
     author_email='alex.richards006@gmail.com',
-    license='GNU GPLv3',
     packages=[
         "djtools",
         "djtools.configs",
         "djtools.collections",
         "djtools.spotify",
         "djtools.sync",
         "djtools.utils",
```

