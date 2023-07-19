# Comparing `tmp/dj_beatcloud-2.6.0b2.tar.gz` & `tmp/dj_beatcloud-2.6.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_beatcloud-2.6.0b2.tar", last modified: Wed Jul 19 05:20:29 2023, max compression
+gzip compressed data, was "dj_beatcloud-2.6.0b3.tar", last modified: Wed Jul 19 06:07:40 2023, max compression
```

## Comparing `dj_beatcloud-2.6.0b2.tar` & `dj_beatcloud-2.6.0b3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 05:20:29.476716 dj_beatcloud-2.6.0b2/
--rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.6.0b2/LICENSE
--rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-26 19:42:57.000000 dj_beatcloud-2.6.0b2/MANIFEST.in
--rw-r--r--   0 alrichards   (502) staff       (20)     2556 2023-07-19 05:20:29.476814 dj_beatcloud-2.6.0b2/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1319 2023-05-26 21:16:19.000000 dj_beatcloud-2.6.0b2/README.md
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 05:20:29.460146 dj_beatcloud-2.6.0b2/dj_beatcloud.egg-info/
--rw-r--r--   0 alrichards   (502) staff       (20)     2556 2023-07-19 05:20:29.000000 dj_beatcloud-2.6.0b2/dj_beatcloud.egg-info/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1248 2023-07-19 05:20:29.000000 dj_beatcloud-2.6.0b2/dj_beatcloud.egg-info/SOURCES.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-07-19 05:20:29.000000 dj_beatcloud-2.6.0b2/dj_beatcloud.egg-info/dependency_links.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-07-19 05:20:29.000000 dj_beatcloud-2.6.0b2/dj_beatcloud.egg-info/entry_points.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-07-19 05:20:29.000000 dj_beatcloud-2.6.0b2/dj_beatcloud.egg-info/requires.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-07-19 05:20:29.000000 dj_beatcloud-2.6.0b2/dj_beatcloud.egg-info/top_level.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 05:20:29.461753 dj_beatcloud-2.6.0b2/djtools/
--rw-r--r--   0 alrichards   (502) staff       (20)     2543 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1776 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/__main__.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 05:20:29.466400 dj_beatcloud-2.6.0b2/djtools/collections/
--rw-r--r--   0 alrichards   (502) staff       (20)     1434 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/collections/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)    12878 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/collections/collections.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2810 2023-07-19 05:18:06.000000 dj_beatcloud-2.6.0b2/djtools/collections/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2515 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/collections/copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)    27150 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/collections/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     7584 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/collections/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)    15833 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/collections/playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2405 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/collections/shuffle_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)    13832 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/collections/tracks.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 05:20:29.469762 dj_beatcloud-2.6.0b2/djtools/configs/
--rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b2/djtools/configs/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1179 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/configs/collection_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)     1765 2023-07-19 05:18:06.000000 dj_beatcloud-2.6.0b2/djtools/configs/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1301 2023-07-19 05:18:23.000000 dj_beatcloud-2.6.0b2/djtools/configs/config.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)    15665 2023-07-19 05:18:06.000000 dj_beatcloud-2.6.0b2/djtools/configs/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b2/djtools/configs/logging.conf
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b2/djtools/configs/spotify_playlists.yaml
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 05:20:29.470030 dj_beatcloud-2.6.0b2/djtools/logs/
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b2/djtools/logs/empty.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 05:20:29.471415 dj_beatcloud-2.6.0b2/djtools/spotify/
--rw-r--r--   0 alrichards   (502) staff       (20)      735 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/spotify/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3258 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/spotify/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    16599 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/spotify/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6053 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/spotify/playlist_builder.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 05:20:29.473956 dj_beatcloud-2.6.0b2/djtools/sync/
--rw-r--r--   0 alrichards   (502) staff       (20)      825 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b2/djtools/sync/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3535 2023-07-19 05:18:06.000000 dj_beatcloud-2.6.0b2/djtools/sync/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     7647 2023-07-19 05:18:06.000000 dj_beatcloud-2.6.0b2/djtools/sync/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5170 2023-07-19 05:18:06.000000 dj_beatcloud-2.6.0b2/djtools/sync/sync_operations.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 05:20:29.476369 dj_beatcloud-2.6.0b2/djtools/utils/
--rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-07-15 20:42:42.000000 dj_beatcloud-2.6.0b2/djtools/utils/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3660 2023-07-15 20:42:42.000000 dj_beatcloud-2.6.0b2/djtools/utils/check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1409 2023-07-19 05:18:06.000000 dj_beatcloud-2.6.0b2/djtools/utils/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    10160 2023-07-19 05:18:06.000000 dj_beatcloud-2.6.0b2/djtools/utils/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b2/djtools/utils/url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)       92 2023-07-19 05:19:41.000000 dj_beatcloud-2.6.0b2/djtools/version.py
--rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 dj_beatcloud-2.6.0b2/pyproject.toml
--rw-r--r--   0 alrichards   (502) staff       (20)       99 2023-07-19 05:20:29.477169 dj_beatcloud-2.6.0b2/setup.cfg
--rw-r--r--   0 alrichards   (502) staff       (20)     2346 2023-07-19 05:18:06.000000 dj_beatcloud-2.6.0b2/setup.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 06:07:40.018348 dj_beatcloud-2.6.0b3/
+-rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.6.0b3/LICENSE
+-rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-26 19:42:57.000000 dj_beatcloud-2.6.0b3/MANIFEST.in
+-rw-r--r--   0 alrichards   (502) staff       (20)     2556 2023-07-19 06:07:40.018475 dj_beatcloud-2.6.0b3/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1319 2023-05-26 21:16:19.000000 dj_beatcloud-2.6.0b3/README.md
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 06:07:39.982681 dj_beatcloud-2.6.0b3/dj_beatcloud.egg-info/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2556 2023-07-19 06:07:39.000000 dj_beatcloud-2.6.0b3/dj_beatcloud.egg-info/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1248 2023-07-19 06:07:39.000000 dj_beatcloud-2.6.0b3/dj_beatcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-07-19 06:07:39.000000 dj_beatcloud-2.6.0b3/dj_beatcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-07-19 06:07:39.000000 dj_beatcloud-2.6.0b3/dj_beatcloud.egg-info/entry_points.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-07-19 06:07:39.000000 dj_beatcloud-2.6.0b3/dj_beatcloud.egg-info/requires.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-07-19 06:07:39.000000 dj_beatcloud-2.6.0b3/dj_beatcloud.egg-info/top_level.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 06:07:39.985787 dj_beatcloud-2.6.0b3/djtools/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2543 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b3/djtools/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1776 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b3/djtools/__main__.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 06:07:39.996074 dj_beatcloud-2.6.0b3/djtools/collections/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1434 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b3/djtools/collections/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    12878 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b3/djtools/collections/collections.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2810 2023-07-19 05:18:06.000000 dj_beatcloud-2.6.0b3/djtools/collections/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2515 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b3/djtools/collections/copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    27150 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b3/djtools/collections/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7584 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b3/djtools/collections/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    15833 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b3/djtools/collections/playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2405 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b3/djtools/collections/shuffle_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    13839 2023-07-19 06:04:36.000000 dj_beatcloud-2.6.0b3/djtools/collections/tracks.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 06:07:40.001636 dj_beatcloud-2.6.0b3/djtools/configs/
+-rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b3/djtools/configs/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1179 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b3/djtools/configs/collection_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)     1765 2023-07-19 05:18:06.000000 dj_beatcloud-2.6.0b3/djtools/configs/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1301 2023-07-19 06:05:49.000000 dj_beatcloud-2.6.0b3/djtools/configs/config.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)    15665 2023-07-19 05:18:06.000000 dj_beatcloud-2.6.0b3/djtools/configs/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b3/djtools/configs/logging.conf
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b3/djtools/configs/spotify_playlists.yaml
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 06:07:40.002330 dj_beatcloud-2.6.0b3/djtools/logs/
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b3/djtools/logs/empty.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 06:07:40.006090 dj_beatcloud-2.6.0b3/djtools/spotify/
+-rw-r--r--   0 alrichards   (502) staff       (20)      735 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b3/djtools/spotify/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3258 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b3/djtools/spotify/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    16599 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b3/djtools/spotify/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6053 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b3/djtools/spotify/playlist_builder.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 06:07:40.012053 dj_beatcloud-2.6.0b3/djtools/sync/
+-rw-r--r--   0 alrichards   (502) staff       (20)      825 2023-07-15 20:42:45.000000 dj_beatcloud-2.6.0b3/djtools/sync/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3532 2023-07-19 06:05:27.000000 dj_beatcloud-2.6.0b3/djtools/sync/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7683 2023-07-19 06:04:36.000000 dj_beatcloud-2.6.0b3/djtools/sync/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5170 2023-07-19 05:18:06.000000 dj_beatcloud-2.6.0b3/djtools/sync/sync_operations.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-07-19 06:07:40.017835 dj_beatcloud-2.6.0b3/djtools/utils/
+-rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-07-15 20:42:42.000000 dj_beatcloud-2.6.0b3/djtools/utils/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3660 2023-07-15 20:42:42.000000 dj_beatcloud-2.6.0b3/djtools/utils/check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1409 2023-07-19 05:18:06.000000 dj_beatcloud-2.6.0b3/djtools/utils/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    10160 2023-07-19 05:18:06.000000 dj_beatcloud-2.6.0b3/djtools/utils/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 dj_beatcloud-2.6.0b3/djtools/utils/url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)       92 2023-07-19 06:05:37.000000 dj_beatcloud-2.6.0b3/djtools/version.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 dj_beatcloud-2.6.0b3/pyproject.toml
+-rw-r--r--   0 alrichards   (502) staff       (20)       99 2023-07-19 06:07:40.018869 dj_beatcloud-2.6.0b3/setup.cfg
+-rw-r--r--   0 alrichards   (502) staff       (20)     2346 2023-07-19 05:18:06.000000 dj_beatcloud-2.6.0b3/setup.py
```

### Comparing `dj_beatcloud-2.6.0b2/LICENSE` & `dj_beatcloud-2.6.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/PKG-INFO` & `dj_beatcloud-2.6.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj_beatcloud
-Version: 2.6.0b2
+Version: 2.6.0b3
 Summary: DJ Tools is a library for managing a collection of music.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 Keywords: DJ Rekordbox spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dj_beatcloud Version: 2.6.0b2 Summary: DJ Tools is
+Metadata-Version: 2.1 Name: dj_beatcloud Version: 2.6.0b3 Summary: DJ Tools is
 a library for managing a collection of music. Home-page: https://github.com/a-
 rich/DJ-tools Author: Alex Richards Author-email: alex.richards006@gmail.com
 Keywords: DJ Rekordbox spotify reddit aws s3 Classifier: Development Status ::
 4 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: End Users/Desktop Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English Classifier: Operating System :: MacOS
```

### Comparing `dj_beatcloud-2.6.0b2/README.md` & `dj_beatcloud-2.6.0b3/README.md`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/dj_beatcloud.egg-info/PKG-INFO` & `dj_beatcloud-2.6.0b3/dj_beatcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-beatcloud
-Version: 2.6.0b2
+Version: 2.6.0b3
 Summary: DJ Tools is a library for managing a collection of music.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 Keywords: DJ Rekordbox spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dj-beatcloud Version: 2.6.0b2 Summary: DJ Tools is
+Metadata-Version: 2.1 Name: dj-beatcloud Version: 2.6.0b3 Summary: DJ Tools is
 a library for managing a collection of music. Home-page: https://github.com/a-
 rich/DJ-tools Author: Alex Richards Author-email: alex.richards006@gmail.com
 Keywords: DJ Rekordbox spotify reddit aws s3 Classifier: Development Status ::
 4 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: End Users/Desktop Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English Classifier: Operating System :: MacOS
```

### Comparing `dj_beatcloud-2.6.0b2/dj_beatcloud.egg-info/SOURCES.txt` & `dj_beatcloud-2.6.0b3/dj_beatcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/djtools/__init__.py` & `dj_beatcloud-2.6.0b3/djtools/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/djtools/__main__.py` & `dj_beatcloud-2.6.0b3/djtools/__main__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/djtools/collections/__init__.py` & `dj_beatcloud-2.6.0b3/djtools/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/djtools/collections/collections.py` & `dj_beatcloud-2.6.0b3/djtools/collections/collections.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/djtools/collections/config.py` & `dj_beatcloud-2.6.0b3/djtools/collections/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/djtools/collections/copy_playlists.py` & `dj_beatcloud-2.6.0b3/djtools/collections/copy_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/djtools/collections/helpers.py` & `dj_beatcloud-2.6.0b3/djtools/collections/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/djtools/collections/playlist_builder.py` & `dj_beatcloud-2.6.0b3/djtools/collections/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/djtools/collections/playlists.py` & `dj_beatcloud-2.6.0b3/djtools/collections/playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/djtools/collections/shuffle_playlists.py` & `dj_beatcloud-2.6.0b3/djtools/collections/shuffle_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/djtools/collections/tracks.py` & `dj_beatcloud-2.6.0b3/djtools/collections/tracks.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,15 +361,15 @@
             if key == "Genre":
                 value = " / ".join(value)
 
             # Re-insert the location prefix and quote the path.
             if key == "Location":
                 value = (
                     f"{self.__location_prefix}"
-                    f'{quote(str(value), safe="/,()!+=#;$")}'
+                    f'{quote(value.as_posix(), safe="/,()!+=#;$:")}'
                 )
                 value = re.sub(
                     r'%[0-9A-Z]{2}', lambda x: x.group(0).lower(), value 
                 )
 
             # Reverse the rating value to the range recognized by Rekordbox.
             if key == "Rating":
```

### Comparing `dj_beatcloud-2.6.0b2/djtools/configs/collection_playlists.yaml` & `dj_beatcloud-2.6.0b3/djtools/configs/collection_playlists.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/djtools/configs/config.py` & `dj_beatcloud-2.6.0b3/djtools/configs/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/djtools/configs/config.yaml` & `dj_beatcloud-2.6.0b3/djtools/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/djtools/configs/helpers.py` & `dj_beatcloud-2.6.0b3/djtools/configs/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/djtools/spotify/__init__.py` & `dj_beatcloud-2.6.0b3/djtools/spotify/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/djtools/spotify/config.py` & `dj_beatcloud-2.6.0b3/djtools/spotify/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/djtools/spotify/helpers.py` & `dj_beatcloud-2.6.0b3/djtools/spotify/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/djtools/spotify/playlist_builder.py` & `dj_beatcloud-2.6.0b3/djtools/spotify/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/djtools/sync/__init__.py` & `dj_beatcloud-2.6.0b3/djtools/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/djtools/sync/config.py` & `dj_beatcloud-2.6.0b3/djtools/sync/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,16 @@
                 self.UPLOAD_MUSIC,
             ]
         ):
             if not self.AWS_PROFILE:
                 msg = "Config must include AWS_PROFILE for sync operations"
                 logger.critical(msg)
                 raise RuntimeError(msg)
-            os.environ["AWS_PROFILE"] = self.AWS_PROFILE
+
+        os.environ["AWS_PROFILE"] = self.AWS_PROFILE
 
         if (
             any([self.DOWNLOAD_MUSIC, self.UPLOAD_MUSIC]) and
             (not self.USB_PATH or not self.USB_PATH.exists())
         ):
             msg = (
                 "Config must include USB_PATH for both DOWNLOAD_MUSIC and "
```

### Comparing `dj_beatcloud-2.6.0b2/djtools/sync/helpers.py` & `dj_beatcloud-2.6.0b3/djtools/sync/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         other_user_collection: Path to another user's collection.
     """
     music_path = Path("DJ Music")
     collection = PLATFORM_REGISTRY[config.PLATFORM]["collection"](
         path=other_user_collection
     )
     for track in collection.get_tracks().values():
-        loc = str(track.get_location())
+        loc = track.get_location().as_posix()
         common_path = (
             music_path / loc.split(str(music_path) + '/', maxsplit=-1)[-1]
         )
         track.set_location(config.USB_PATH / common_path)
     collection.serialize(new_path=other_user_collection)
 
 
@@ -141,15 +141,16 @@
     except Exception as exc:
         msg = f"Failure while syncing: {exc}"
         logger.critical(msg)
         raise Exception(msg) from exc
 
     new_music = ""
     for group_id, group in groupby(
-        sorted(tracks, key=lambda x: x.parent), key=lambda x: x.parent
+        sorted(tracks, key=lambda x: x.parent.as_posix()),
+        key=lambda x: x.parent.as_posix()
     ):
         group = sorted(group)
         new_music += f"{group_id}: {len(group)}\n"
         for track in group:
             new_music += f"\t{track.name}\n"
     if new_music:
         logger.info(
```

### Comparing `dj_beatcloud-2.6.0b2/djtools/sync/sync_operations.py` & `dj_beatcloud-2.6.0b3/djtools/sync/sync_operations.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/djtools/utils/__init__.py` & `dj_beatcloud-2.6.0b3/djtools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/djtools/utils/check_tracks.py` & `dj_beatcloud-2.6.0b3/djtools/utils/check_tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/djtools/utils/config.py` & `dj_beatcloud-2.6.0b3/djtools/utils/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/djtools/utils/helpers.py` & `dj_beatcloud-2.6.0b3/djtools/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/djtools/utils/url_download.py` & `dj_beatcloud-2.6.0b3/djtools/utils/url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.6.0b2/setup.py` & `dj_beatcloud-2.6.0b3/setup.py`

 * *Files identical despite different names*

