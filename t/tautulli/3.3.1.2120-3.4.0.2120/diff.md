# Comparing `tmp/tautulli-3.3.1.2120.tar.gz` & `tmp/tautulli-3.4.0.2120.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tautulli-3.3.1.2120.tar", last modified: Wed Jul  5 19:06:35 2023, max compression
+gzip compressed data, was "tautulli-3.4.0.2120.tar", last modified: Wed Jul 19 04:05:40 2023, max compression
```

## Comparing `tautulli-3.3.1.2120.tar` & `tautulli-3.4.0.2120.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:06:35.721929 tautulli-3.3.1.2120/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-07-05 19:06:35.721929 tautulli-3.3.1.2120/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-05 19:06:35.721929 tautulli-3.3.1.2120/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-05 19:06:09.000000 tautulli-3.3.1.2120/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:06:35.705928 tautulli-3.3.1.2120/tautulli/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/API_VERSIONS.json
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/PYTHON_VERSIONS.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:06:35.705928 tautulli-3.3.1.2120/tautulli/api/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    96521 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/api/json_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    67022 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/api/object_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:06:35.709929 tautulli-3.3.1.2120/tautulli/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/internal/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/internal/static.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:06:35.721929 tautulli-3.3.1.2120/tautulli/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13663 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/children_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/collections_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/date_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/export_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/exports_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/geo_ip_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/get_plays_or_stream_types_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/home_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/item_user_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/item_watch_time_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/libraries_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/library.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/library_media_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/library_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/library_user_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/library_watch_time_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/new_rating_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/newsletter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/newsletter_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/newsletter_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/newsletter_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/notification_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/notifier_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/notifier_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/notifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/old_rating_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/playlists_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/plex_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/pms_update.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/recently_added.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/registered_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     9114 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/search_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/server_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/server_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/server_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/server_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/server_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/servers_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    25625 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/stream_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/synced_items.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/tautulli_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/update_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/user_ips.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/user_logins.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/user_player_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/user_watch_time_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/usernames.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/users_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/models/whois_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:06:35.721929 tautulli-3.3.1.2120/tautulli/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/tools/api_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-05 19:06:08.000000 tautulli-3.3.1.2120/tautulli/tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:06:35.705928 tautulli-3.3.1.2120/tautulli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-07-05 19:06:35.000000 tautulli-3.3.1.2120/tautulli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-05 19:06:35.000000 tautulli-3.3.1.2120/tautulli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:06:35.000000 tautulli-3.3.1.2120/tautulli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-05 19:06:35.000000 tautulli-3.3.1.2120/tautulli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 19:06:35.000000 tautulli-3.3.1.2120/tautulli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:05:40.212597 tautulli-3.4.0.2120/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-07-19 04:05:40.212597 tautulli-3.4.0.2120/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-19 04:05:40.212597 tautulli-3.4.0.2120/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-19 04:05:17.000000 tautulli-3.4.0.2120/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:05:40.204597 tautulli-3.4.0.2120/tautulli/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/API_VERSIONS.json
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/PYTHON_VERSIONS.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:05:40.204597 tautulli-3.4.0.2120/tautulli/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97154 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/api/json_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67520 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/api/object_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:05:40.204597 tautulli-3.4.0.2120/tautulli/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/internal/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/internal/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:05:40.212597 tautulli-3.4.0.2120/tautulli/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13663 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/children_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/collections_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/date_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/export_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/exports_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/geo_ip_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/get_plays_or_stream_types_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/home_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/item_user_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/item_watch_time_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/libraries_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/library_media_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/library_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/library_user_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/library_watch_time_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/new_rating_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/newsletter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/newsletter_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/newsletter_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/newsletter_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/notification_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/notifier_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/notifier_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/notifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/old_rating_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/playlists_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/plex_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/pms_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/recently_added.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/registered_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9114 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/search_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/server_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/server_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/server_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/server_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/server_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/servers_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25625 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/stream_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/synced_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/tautulli_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/update_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/user_ips.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/user_logins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/user_player_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/user_watch_time_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/usernames.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/users_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/models/whois_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:05:40.212597 tautulli-3.4.0.2120/tautulli/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/tools/api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-19 04:05:16.000000 tautulli-3.4.0.2120/tautulli/tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:05:40.204597 tautulli-3.4.0.2120/tautulli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-07-19 04:05:40.000000 tautulli-3.4.0.2120/tautulli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-19 04:05:40.000000 tautulli-3.4.0.2120/tautulli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 04:05:40.000000 tautulli-3.4.0.2120/tautulli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-19 04:05:40.000000 tautulli-3.4.0.2120/tautulli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 04:05:40.000000 tautulli-3.4.0.2120/tautulli.egg-info/top_level.txt
```

### Comparing `tautulli-3.3.1.2120/LICENSE` & `tautulli-3.4.0.2120/LICENSE`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/PKG-INFO` & `tautulli-3.4.0.2120/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tautulli
-Version: 3.3.1.2120
+Version: 3.4.0.2120
 Summary: A complete Python client for Tautulli's API
 Home-page: https://github.com/nwithan8/pytulli
 Author: Nate Harris
 Author-email: n8gr8gbln@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/nwithan8/pytulli/archive/refs/tags/3.3.1.2120.tar.gz
+Download-URL: https://github.com/nwithan8/pytulli/archive/refs/tags/3.4.0.2120.tar.gz
 Description: # A Python client for Tautulli's API
         [![PyPi](https://img.shields.io/pypi/dm/tautulli?label=Downloads&logo=pypi)](https://pypi.org/project/tautulli)
         [![License](https://img.shields.io/pypi/l/tautulli?color=orange&style=flat-square)](https://github.com/nwithan8/pytulli/blob/master/LICENSE)
         
         [![Open Issues](https://img.shields.io/github/issues-raw/nwithan8/pytulli?color=gold&style=flat-square)](https://github.com/nwithan8/pytulli/issues?q=is%3Aopen+is%3Aissue)
         [![Closed Issues](https://img.shields.io/github/issues-closed-raw/nwithan8/pytulli?color=black&style=flat-square)](https://github.com/nwithan8/pytulli/issues?q=is%3Aissue+is%3Aclosed)
         [![Latest Release](https://img.shields.io/github/v/release/nwithan8/pytulli?color=red&label=latest%20release&logo=github&style=flat-square)](https://github.com/nwithan8/pytulli/releases)
```

### Comparing `tautulli-3.3.1.2120/README.md` & `tautulli-3.4.0.2120/README.md`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/setup.py` & `tautulli-3.4.0.2120/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os
 from typing import List
 
 import setuptools
 
-__version__ = '3.3.1.2120'
+__version__ = '3.4.0.2120'
 
 __title__ = "tautulli"
 __author__ = 'Nate Harris'
 __author_email__ = 'n8gr8gbln@gmail.com'
 __github_username__ = "nwithan8"
 __github_repo__ = "pytulli"
 __copyright__ = "Copyright © 2023 - Nate Harris"
```

### Comparing `tautulli-3.3.1.2120/tautulli/api/json_api.py` & `tautulli-3.4.0.2120/tautulli/api/json_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,37 +100,39 @@
             except:
                 # TODO: Do we want to just log an error and return an empty dict, or raise an exception?
                 self._logger.error(f"Could not parse JSON from response: {response.text}")
                 return static.empty_dict
         return static.empty_dict
 
     @raw_json
-    def _get_x_by(self, endpoint: str, time_range: int = None, y_axis: str = None, user_id: str = None,
+    def _get_x_by(self, endpoint: str, time_range: int = None, y_axis: str = None, user_ids: List[str] = None,
                   grouping: bool = False) -> dict:
         """
         Abstract method for the get_plays_by_X and get_streams_by_X functions
 
         :param endpoint: Tautulli endpoint
         :type endpoint: str
         :param time_range: Number of days of data to return
         :type time_range: int, optional
         :param y_axis: Stat type ('plays' or 'duration')
         :type y_axis: str, optional
-        :param user_id: User ID to filter data
-        :type user_id: str, optional
+        :param user_ids: List of user IDs to filter data
+        :type user_ids: List[str], optional
         :param grouping: Whether to group the results (default: False)
         :type grouping: bool, optional
         :returns: Dict of data
         :rtype: dict
         """
         grouping = bool_to_int(boolean=grouping)
         if _is_invalid_choice(value=y_axis, variable_name='y_axis',
                               choices=static.stats_type):
             return False, None
-        params = build_optional_params(time_range=time_range, y_axis=y_axis, user_id=user_id, grouping=grouping)
+        if user_ids:
+            user_ids = comma_delimit(user_ids)
+        params = build_optional_params(time_range=time_range, y_axis=y_axis, user_id=user_ids, grouping=grouping)
         return endpoint, params
 
     @property
     def shortcuts(self) -> APIShortcuts:
         """
         Shortcuts for common API actions
 
@@ -1359,184 +1361,184 @@
             return False, None
         params = {}
         name, value = _which_used(section_id=section_id, user_id=user_id)
         if name:
             params[name] = value
         return 'get_playlists_table', params
 
-    def get_plays_by_date(self, time_range: int = None, y_axis: str = None, user_id: str = None,
+    def get_plays_by_date(self, time_range: int = None, y_axis: str = None, user_ids: List[str] = None,
                           grouping: bool = False) -> dict:
         """
         Get graph data by date
 
         :param time_range: Number of days of data to return
         :type time_range: int, optional
         :param y_axis: Stat type ('plays' or 'duration')
         :type y_axis: str, optional
-        :param user_id: User ID to filter data
-        :type user_id: str, optional
+        :param user_ids: List of user IDs to filter data
+        :type user_ids: List[str], optional
         :param grouping: Whether to group the results (default: False)
         :type grouping: bool, optional
         :returns: Dict of data
         :rtype: dict
         """
-        return self._get_x_by(endpoint='get_plays_by_date', time_range=time_range, y_axis=y_axis, user_id=user_id,
+        return self._get_x_by(endpoint='get_plays_by_date', time_range=time_range, y_axis=y_axis, user_ids=user_ids,
                               grouping=grouping)
 
-    def get_plays_by_day_of_week(self, time_range: int = None, y_axis: str = None, user_id: str = None,
+    def get_plays_by_day_of_week(self, time_range: int = None, y_axis: str = None, user_ids: List[str] = None,
                                  grouping: bool = False) -> dict:
         """
         Get graph data by day of the week
 
         :param time_range: Number of days of data to return
         :type time_range: int, optional
         :param y_axis: Stat type ('plays' or 'duration')
         :type y_axis: str, optional
-        :param user_id: User ID to filter data
-        :type user_id: str, optional
+        :param user_ids: List of user IDs to filter data
+        :type user_ids: List[str], optional
         :param grouping: Whether to group the results (default: False)
         :type grouping: bool, optional
         :returns: Dict of data
         :rtype: dict
         """
-        return self._get_x_by(endpoint='get_plays_by_dayofweek', time_range=time_range, y_axis=y_axis, user_id=user_id,
+        return self._get_x_by(endpoint='get_plays_by_dayofweek', time_range=time_range, y_axis=y_axis, user_ids=user_ids,
                               grouping=grouping)
 
-    def get_plays_by_hour_of_day(self, time_range: int = None, y_axis: str = None, user_id: str = None,
+    def get_plays_by_hour_of_day(self, time_range: int = None, y_axis: str = None, user_ids: List[str] = None,
                                  grouping: bool = False) -> dict:
         """
         Get graph data by hour of the day
 
         :param time_range: Number of days of data to return
         :type time_range: int, optional
         :param y_axis: Stat type ('plays' or 'duration')
         :type y_axis: str, optional
-        :param user_id: User ID to filter data
-        :type user_id: str, optional
+        :param user_ids: List of user IDs to filter data
+        :type user_ids: List[str], optional
         :param grouping: Whether to group the results (default: False)
         :type grouping: bool, optional
         :returns: Dict of data
         :rtype: dict
         """
         # noinspection SpellCheckingInspection
-        return self._get_x_by(endpoint='get_plays_by_hourofday', time_range=time_range, y_axis=y_axis, user_id=user_id,
+        return self._get_x_by(endpoint='get_plays_by_hourofday', time_range=time_range, y_axis=y_axis, user_ids=user_ids,
                               grouping=grouping)
 
-    def get_plays_by_source_resolution(self, time_range: int = None, y_axis: str = None, user_id: str = None,
+    def get_plays_by_source_resolution(self, time_range: int = None, y_axis: str = None, user_ids: List[str] = None,
                                        grouping: bool = False) -> dict:
         """
         Get graph data by source resolution
 
         :param time_range: Number of days of data to return
         :type time_range: int, optional
         :param y_axis: Stat type ('plays' or 'duration')
         :type y_axis: str, optional
-        :param user_id: User ID to filter data
-        :type user_id: str, optional
+        :param user_ids: List of user IDs to filter data
+        :type user_ids: List[str], optional
         :param grouping: Whether to group the results (default: False)
         :type grouping: bool, optional
         :returns: Dict of data
         :rtype: dict
         """
         return self._get_x_by(endpoint='get_plays_by_source_resolution', time_range=time_range, y_axis=y_axis,
-                              user_id=user_id, grouping=grouping)
+                              user_ids=user_ids, grouping=grouping)
 
-    def get_plays_by_stream_resolution(self, time_range: int = None, y_axis: str = None, user_id: str = None,
+    def get_plays_by_stream_resolution(self, time_range: int = None, y_axis: str = None, user_ids: List[str] = None,
                                        grouping: bool = False) -> dict:
         """
         Get graph data by stream resolution
 
         :param time_range: Number of days of data to return
         :type time_range: int, optional
         :param y_axis: Stat type ('plays' or 'duration')
         :type y_axis: str, optional
-        :param user_id: User ID to filter data
-        :type user_id: str, optional
+        :param user_ids: List of user IDs to filter data
+        :type user_ids: List[str], optional
         :param grouping: Whether to group the results (default: False)
         :type grouping: bool, optional
         :returns: Dict of data
         :rtype: dict
         """
         return self._get_x_by(endpoint='get_plays_by_stream_resolution', time_range=time_range, y_axis=y_axis,
-                              user_id=user_id, grouping=grouping)
+                              user_ids=user_ids, grouping=grouping)
 
-    def get_plays_by_stream_type(self, time_range: int = None, y_axis: str = None, user_id: str = None,
+    def get_plays_by_stream_type(self, time_range: int = None, y_axis: str = None, user_ids: List[str] = None,
                                  grouping: bool = False) -> dict:
         """
         Get graph data by stream type
 
         :param time_range: Number of days of data to return
         :type time_range: int, optional
         :param y_axis: Stat type ('plays' or 'duration')
         :type y_axis: str, optional
-        :param user_id: User ID to filter data
-        :type user_id: str, optional
+        :param user_ids: List of user IDs to filter data
+        :type user_ids: List[str], optional
         :param grouping: Whether to group the results (default: False)
         :type grouping: bool, optional
         :returns: Dict of data
         :rtype: dict
         """
         return self._get_x_by(endpoint='get_plays_by_stream_type', time_range=time_range, y_axis=y_axis,
-                              user_id=user_id, grouping=grouping)
+                              user_ids=user_ids, grouping=grouping)
 
-    def get_plays_by_top_10_platforms(self, time_range: int = None, y_axis: str = None, user_id: str = None,
+    def get_plays_by_top_10_platforms(self, time_range: int = None, y_axis: str = None, user_ids: List[str] = None,
                                       grouping: bool = False) -> dict:
         """
         Get graph data by top 10 platforms
 
         :param time_range: Number of days of data to return
         :type time_range: int, optional
         :param y_axis: Stat type ('plays' or 'duration')
         :type y_axis: str, optional
-        :param user_id: User ID to filter data
-        :type user_id: str, optional
+        :param user_ids: List of user IDs to filter data
+        :type user_ids: List[str], optional
         :param grouping: Whether to group the results (default: False)
         :type grouping: bool, optional
         :returns: Dict of data
         :rtype: dict
         """
         return self._get_x_by(endpoint='get_plays_by_top_10_platforms', time_range=time_range, y_axis=y_axis,
-                              user_id=user_id, grouping=grouping)
+                              user_ids=user_ids, grouping=grouping)
 
-    def get_plays_by_top_10_users(self, time_range: int = None, y_axis: str = None, user_id: str = None,
+    def get_plays_by_top_10_users(self, time_range: int = None, y_axis: str = None, user_ids: List[str] = None,
                                   grouping: bool = False) -> dict:
         """
         Get graph data by top 10 users
 
         :param time_range: Number of days of data to return
         :type time_range: int, optional
         :param y_axis: Stat type ('plays' or 'duration')
         :type y_axis: str, optional
-        :param user_id: User ID to filter data
-        :type user_id: str, optional
+        :param user_ids: List of user IDs to filter data
+        :type user_ids: List[str], optional
         :param grouping: Whether to group the results (default: False)
         :type grouping: bool, optional
         :returns: Dict of data
         :rtype: dict
         """
         return self._get_x_by(endpoint='get_plays_by_top_10_users', time_range=time_range, y_axis=y_axis,
-                              user_id=user_id, grouping=grouping)
+                              user_ids=user_ids, grouping=grouping)
 
-    def get_plays_per_month(self, time_range: int = None, y_axis: str = None, user_id: str = None,
+    def get_plays_per_month(self, time_range: int = None, y_axis: str = None, user_ids: List[str] = None,
                             grouping: bool = False) -> dict:
         """
         Get graph data by month
 
         :param time_range: Number of days of data to return
         :type time_range: int, optional
         :param y_axis: Stat type ('plays' or 'duration')
         :type y_axis: str, optional
-        :param user_id: User ID to filter data
-        :type user_id: str, optional
+        :param user_ids: List of user IDs to filter data
+        :type user_ids: List[str], optional
         :param grouping: Whether to group the results (default: False)
         :type grouping: bool, optional
         :returns: Dict of data
         :rtype: dict
         """
-        return self._get_x_by(endpoint='get_plays_per_month', time_range=time_range, y_axis=y_axis, user_id=user_id,
+        return self._get_x_by(endpoint='get_plays_per_month', time_range=time_range, y_axis=y_axis, user_ids=user_ids,
                               grouping=grouping)
 
     @raw_json
     def get_plex_log(self, window: int = None, logfile: str = None) -> dict:
         """
         Get the Plex Media Server logs
 
@@ -1710,51 +1712,51 @@
             return False, None
         params = {}
         name, value = _which_used(row_id=row_id, session_key=session_key)
         if name:
             params[name] = value
         return 'get_stream_data', params
 
-    def get_stream_type_by_top_10_platforms(self, time_range: int = None, y_axis: str = None, user_id: str = None,
+    def get_stream_type_by_top_10_platforms(self, time_range: int = None, y_axis: str = None, user_ids: List[str] = None,
                                             grouping: bool = False) -> dict:
         """
         Get graph data by stream type by the top 10 platforms
 
         :param time_range: Number of days of data to return
         :type time_range: int, optional
         :param y_axis: Stat type ('plays' or 'duration')
         :type y_axis: str, optional
-        :param user_id: User ID to filter data
-        :type user_id: str, optional
+        :param user_ids: List of user IDs to filter data
+        :type user_ids: List[str], optional
         :param grouping: Whether to group the results (default: False)
         :type grouping: bool, optional
         :returns: Dict of data
         :rtype: dict
         """
         return self._get_x_by(endpoint='get_stream_type_by_top_10_platforms', time_range=time_range, y_axis=y_axis,
-                              user_id=user_id, grouping=grouping)
+                              user_ids=user_ids, grouping=grouping)
 
-    def get_stream_type_by_top_10_users(self, time_range: int = None, y_axis: str = None, user_id: str = None,
+    def get_stream_type_by_top_10_users(self, time_range: int = None, y_axis: str = None, user_ids: List[str] = None,
                                         grouping: bool = False) -> dict:
         """
         Get graph data by stream type by the top 10 users
 
         :param time_range: Number of days of data to return
         :type time_range: int, optional
         :param y_axis: Stat type ('plays' or 'duration')
         :type y_axis: str, optional
-        :param user_id: User ID to filter data
-        :type user_id: str, optional
+        :param user_ids: List of user IDs to filter data
+        :type user_ids: List[str], optional
         :param grouping: Whether to group the results (default: False)
         :type grouping: bool, optional
         :returns: Dict of data
         :rtype: dict
         """
         return self._get_x_by(endpoint='get_stream_type_by_top_10_users', time_range=time_range, y_axis=y_axis,
-                              user_id=user_id, grouping=grouping)
+                              user_ids=user_ids, grouping=grouping)
 
     @raw_json
     def get_synced_items(self, machine_id: str = None, user_id: str = None) -> dict:
         """
         Get a list of synced items on the Plex Media Server
 
         :param machine_id: Plex Media Server identifier
@@ -2177,14 +2179,24 @@
         params = build_optional_params(platform=platform, version=version, friendly_name=friendly_name,
                                        onesignal_id=onesignal_id, min_version=min_version)
         params['device_id'] = device_id
         params['device_name'] = device_name
         return 'register_device', params
 
     @set_and_forget
+    def regroup_history(self) -> bool:
+        """
+        Regroup play history in the database
+
+        :returns: `True` if successful, `False` if unsuccessful
+        :rtype: bool
+        """
+        return 'regroup_history', None
+
+    @set_and_forget
     def restart(self) -> bool:
         """
         Restart Tautulli
 
         :returns: `True` if successful, `False` if unsuccessful
         :rtype: bool
         """
```

### Comparing `tautulli-3.3.1.2120/tautulli/api/object_api.py` & `tautulli-3.4.0.2120/tautulli/api/object_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -996,177 +996,177 @@
         :type user_id: str, optional
         :returns: PlaylistsTable object
 
         """
         return 'PlaylistsTable'
 
     @make_object
-    def get_plays_by_date(self, time_range: int = None, y_axis: str = None, user_id: str = None,
+    def get_plays_by_date(self, time_range: int = None, y_axis: str = None, user_ids: List[str] = None,
                           grouping: bool = False) -> PlaysOrStreamTypesBy:
         """
         Get graph data by date
 
         :param time_range: Number of days of data to return
         :type time_range: int, optional
         :param y_axis: Stat type ('plays' or 'duration')
         :type y_axis: str, optional
-        :param user_id: User ID to filter data
-        :type user_id: str, optional
+        :param user_ids: List of user IDs to filter data
+        :type user_ids: List[str], optional
         :param grouping: Whether to group the results (default: False)
         :type grouping: bool, optional
         :returns: PlaysOrStreamTypesBy object
         :rtype: PlaysOrStreamTypesBy
         """
         return 'PlaysOrStreamTypesBy'
 
     @make_object
-    def get_plays_by_day_of_week(self, time_range: int = None, y_axis: str = None, user_id: str = None,
+    def get_plays_by_day_of_week(self, time_range: int = None, y_axis: str = None, user_ids: List[str] = None,
                                  grouping: bool = False) -> PlaysOrStreamTypesBy:
         """
         Get graph data by day of the week
 
         :param time_range: Number of days of data to return
         :type time_range: int, optional
         :param y_axis: Stat type ('plays' or 'duration')
         :type y_axis: str, optional
-        :param user_id: User ID to filter data
-        :type user_id: str, optional
+        :param user_ids: List of user IDs to filter data
+        :type user_ids: List[str], optional
         :param grouping: Whether to group the results (default: False)
         :type grouping: bool, optional
         :returns: PlaysOrStreamTypesBy object
         :rtype: PlaysOrStreamTypesBy
         """
         return 'PlaysOrStreamTypesBy'
 
     @make_object
-    def get_plays_by_hour_of_day(self, time_range: int = None, y_axis: str = None, user_id: str = None,
+    def get_plays_by_hour_of_day(self, time_range: int = None, y_axis: str = None, user_ids: List[str] = None,
                                  grouping: bool = False) -> PlaysOrStreamTypesBy:
         """
         Get graph data by hour of the day
 
         :param time_range: Number of days of data to return
         :type time_range: int, optional
         :param y_axis: Stat type ('plays' or 'duration')
         :type y_axis: str, optional
-        :param user_id: User ID to filter data
-        :type user_id: str, optional
+        :param user_ids: List of user IDs to filter data
+        :type user_ids: List[str], optional
         :param grouping: Whether to group the results (default: False)
         :type grouping: bool, optional
         :returns: PlaysOrStreamTypesBy object
         :rtype: PlaysOrStreamTypesBy
         """
         return 'PlaysOrStreamTypesBy'
 
     @make_object
-    def get_plays_by_source_resolution(self, time_range: int = None, y_axis: str = None, user_id: str = None,
+    def get_plays_by_source_resolution(self, time_range: int = None, y_axis: str = None, user_ids: List[str] = None,
                                        grouping: bool = False) -> PlaysOrStreamTypesBy:
         """
         Get graph data by source resolution
 
         :param time_range: Number of days of data to return
         :type time_range: int, optional
         :param y_axis: Stat type ('plays' or 'duration')
         :type y_axis: str, optional
-        :param user_id: User ID to filter data
-        :type user_id: str, optional
+        :param user_ids: List of user IDs to filter data
+        :type user_ids: List[str], optional
         :param grouping: Whether to group the results (default: False)
         :type grouping: bool, optional
         :returns: PlaysOrStreamTypesBy object
         :rtype: PlaysOrStreamTypesBy
         """
         return 'PlaysOrStreamTypesBy'
 
     @make_object
-    def get_plays_by_stream_resolution(self, time_range: int = None, y_axis: str = None, user_id: str = None,
+    def get_plays_by_stream_resolution(self, time_range: int = None, y_axis: str = None, user_ids: List[str] = None,
                                        grouping: bool = False) -> PlaysOrStreamTypesBy:
         """
         Get graph data by stream resolution
 
         :param time_range: Number of days of data to return
         :type time_range: int, optional
         :param y_axis: Stat type ('plays' or 'duration')
         :type y_axis: str, optional
-        :param user_id: User ID to filter data
-        :type user_id: str, optional
+        :param user_ids: List of user IDs to filter data
+        :type user_ids: List[str], optional
         :param grouping: Whether to group the results (default: False)
         :type grouping: bool, optional
         :returns: PlaysOrStreamTypesBy object
         :rtype: PlaysOrStreamTypesBy
         """
         return 'PlaysOrStreamTypesBy'
 
     @make_object
-    def get_plays_by_stream_type(self, time_range: int = None, y_axis: str = None, user_id: str = None,
+    def get_plays_by_stream_type(self, time_range: int = None, y_axis: str = None, user_ids: List[str] = None,
                                  grouping: bool = False) -> PlaysOrStreamTypesBy:
         """
         Get graph data by stream type
 
         :param time_range: Number of days of data to return
         :type time_range: int, optional
         :param y_axis: Stat type ('plays' or 'duration')
         :type y_axis: str, optional
-        :param user_id: User ID to filter data
-        :type user_id: str, optional
+        :param user_ids: List of user IDs to filter data
+        :type user_ids: List[str], optional
         :param grouping: Whether to group the results (default: False)
         :type grouping: bool, optional
         :returns: PlaysOrStreamTypesBy object
         :rtype: PlaysOrStreamTypesBy
         """
         return 'PlaysOrStreamTypesBy'
 
     @make_object
-    def get_plays_by_top_10_platforms(self, time_range: int = None, y_axis: str = None, user_id: str = None,
+    def get_plays_by_top_10_platforms(self, time_range: int = None, y_axis: str = None, user_ids: List[str] = None,
                                       grouping: bool = False) -> PlaysOrStreamTypesBy:
         """
         Get graph data by top 10 platforms
 
         :param time_range: Number of days of data to return
         :type time_range: int, optional
         :param y_axis: Stat type ('plays' or 'duration')
         :type y_axis: str, optional
-        :param user_id: User ID to filter data
-        :type user_id: str, optional
+        :param user_ids: List of user IDs to filter data
+        :type user_ids: List[str], optional
         :param grouping: Whether to group the results (default: False)
         :type grouping: bool, optional
         :returns: PlaysOrStreamTypesBy object
         :rtype: PlaysOrStreamTypesBy
         """
         return 'PlaysOrStreamTypesBy'
 
     @make_object
-    def get_plays_by_top_10_users(self, time_range: int = None, y_axis: str = None, user_id: str = None,
+    def get_plays_by_top_10_users(self, time_range: int = None, y_axis: str = None, user_ids: List[str] = None,
                                   grouping: bool = False) -> PlaysOrStreamTypesBy:
         """
         Get graph data by top 10 users
 
         :param time_range: Number of days of data to return
         :type time_range: int, optional
         :param y_axis: Stat type ('plays' or 'duration')
         :type y_axis: str, optional
-        :param user_id: User ID to filter data
-        :type user_id: str, optional
+        :param user_ids: List of user IDs to filter data
+        :type user_ids: List[str], optional
         :param grouping: Whether to group the results (default: False)
         :type grouping: bool, optional
         :returns: PlaysOrStreamTypesBy object
         :rtype: PlaysOrStreamTypesBy
         """
         return 'PlaysOrStreamTypesBy'
 
     @make_object
-    def get_plays_per_month(self, time_range: int = None, y_axis: str = None, user_id: str = None,
+    def get_plays_per_month(self, time_range: int = None, y_axis: str = None, user_ids: List[str] = None,
                             grouping: bool = False) -> PlaysOrStreamTypesBy:
         """
         Get graph data by month
 
         :param time_range: Number of days of data to return
         :type time_range: int, optional
         :param y_axis: Stat type ('plays' or 'duration')
         :type y_axis: str, optional
-        :param user_id: User ID to filter data
-        :type user_id: str, optional
+        :param user_ids: List of user IDs to filter data
+        :type user_ids: List[str], optional
         :param grouping: Whether to group the results (default: False)
         :type grouping: bool, optional
         :returns: PlaysOrStreamTypesBy object
         :rtype: PlaysOrStreamTypesBy
         """
         return 'PlaysOrStreamTypesBy'
 
@@ -1316,44 +1316,44 @@
         :type session_key: int, optional
         :returns: StreamData object
 
         """
         return 'StreamData'
 
     @make_object
-    def get_stream_type_by_top_10_platforms(self, time_range: int = None, y_axis: str = None, user_id: str = None,
+    def get_stream_type_by_top_10_platforms(self, time_range: int = None, y_axis: str = None, user_ids: List[str] = None,
                                             grouping: bool = False) -> PlaysOrStreamTypesBy:
         """
         Get graph data by stream type by the top 10 platforms
 
         :param time_range: Number of days of data to return
         :type time_range: int, optional
         :param y_axis: Stat type ('plays' or 'duration')
         :type y_axis: str, optional
-        :param user_id: User ID to filter data
-        :type user_id: str, optional
+        :param user_ids: List of user IDs to filter data
+        :type user_ids: List[str], optional
         :param grouping: Whether to group the results (default: False)
         :type grouping: bool, optional
         :returns: PlaysOrStreamTypesBy object
         :rtype: PlaysOrStreamTypesBy
         """
         return 'PlaysOrStreamTypesBy'
 
     @make_object
-    def get_stream_type_by_top_10_users(self, time_range: int = None, y_axis: str = None, user_id: str = None,
+    def get_stream_type_by_top_10_users(self, time_range: int = None, y_axis: str = None, user_ids: List[str] = None,
                                         grouping: bool = False) -> PlaysOrStreamTypesBy:
         """
         Get graph data by stream type by the top 10 users
 
         :param time_range: Number of days of data to return
         :type time_range: int, optional
         :param y_axis: Stat type ('plays' or 'duration')
         :type y_axis: str, optional
-        :param user_id: User ID to filter data
-        :type user_id: str, optional
+        :param user_ids: List of user IDs to filter data
+        :type user_ids: List[str], optional
         :param grouping: Whether to group the results (default: False)
         :type grouping: bool, optional
         :returns: PlaysOrStreamTypesBy object
         :rtype: PlaysOrStreamTypesBy
         """
         return 'PlaysOrStreamTypesBy'
 
@@ -1703,14 +1703,24 @@
         :type min_version: str, optional
         :returns: RegisteredDevice object
 
         """
         return 'RegisteredDevice'
 
     @raw_api_bool
+    def regroup_history(self) -> bool:
+        """
+        Regroup play history in the database
+
+        :returns: `True` if successful, `False` if unsuccessful
+        :rtype: bool
+        """
+        return False
+
+    @raw_api_bool
     def restart(self) -> bool:
         """
         Restart Tautulli
 
         :returns: `True` if successful, `False` if unsuccessful
         :rtype: bool
         """
```

### Comparing `tautulli-3.3.1.2120/tautulli/internal/static.py` & `tautulli-3.4.0.2120/tautulli/internal/static.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/internal/utils.py` & `tautulli-3.4.0.2120/tautulli/internal/utils.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/__init__.py` & `tautulli-3.4.0.2120/tautulli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/activity.py` & `tautulli-3.4.0.2120/tautulli/models/activity.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/children_metadata.py` & `tautulli-3.4.0.2120/tautulli/models/children_metadata.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/collections_table.py` & `tautulli-3.4.0.2120/tautulli/models/collections_table.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/docs.py` & `tautulli-3.4.0.2120/tautulli/models/docs.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/export_fields.py` & `tautulli-3.4.0.2120/tautulli/models/export_fields.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/exports_table.py` & `tautulli-3.4.0.2120/tautulli/models/exports_table.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/geo_ip_lookup.py` & `tautulli-3.4.0.2120/tautulli/models/geo_ip_lookup.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/get_plays_or_stream_types_by.py` & `tautulli-3.4.0.2120/tautulli/models/get_plays_or_stream_types_by.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/history.py` & `tautulli-3.4.0.2120/tautulli/models/history.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/home_stats.py` & `tautulli-3.4.0.2120/tautulli/models/home_stats.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/item_user_stats.py` & `tautulli-3.4.0.2120/tautulli/models/item_user_stats.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/libraries.py` & `tautulli-3.4.0.2120/tautulli/models/libraries.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/libraries_table.py` & `tautulli-3.4.0.2120/tautulli/models/libraries_table.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/library.py` & `tautulli-3.4.0.2120/tautulli/models/library.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/library_media_info.py` & `tautulli-3.4.0.2120/tautulli/models/library_media_info.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/library_user_stats.py` & `tautulli-3.4.0.2120/tautulli/models/library_user_stats.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/metadata.py` & `tautulli-3.4.0.2120/tautulli/models/metadata.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/newsletter.py` & `tautulli-3.4.0.2120/tautulli/models/newsletter.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/newsletter_config.py` & `tautulli-3.4.0.2120/tautulli/models/newsletter_config.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/newsletter_log.py` & `tautulli-3.4.0.2120/tautulli/models/newsletter_log.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/notification_log.py` & `tautulli-3.4.0.2120/tautulli/models/notification_log.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/notifier_config.py` & `tautulli-3.4.0.2120/tautulli/models/notifier_config.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/notifiers.py` & `tautulli-3.4.0.2120/tautulli/models/notifiers.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/parser.py` & `tautulli-3.4.0.2120/tautulli/models/parser.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/playlists_table.py` & `tautulli-3.4.0.2120/tautulli/models/playlists_table.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/pms_update.py` & `tautulli-3.4.0.2120/tautulli/models/pms_update.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/registered_device.py` & `tautulli-3.4.0.2120/tautulli/models/registered_device.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/search_results.py` & `tautulli-3.4.0.2120/tautulli/models/search_results.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/server_info.py` & `tautulli-3.4.0.2120/tautulli/models/server_info.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/server_list.py` & `tautulli-3.4.0.2120/tautulli/models/server_list.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/servers_info.py` & `tautulli-3.4.0.2120/tautulli/models/servers_info.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/settings.py` & `tautulli-3.4.0.2120/tautulli/models/settings.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/stream_data.py` & `tautulli-3.4.0.2120/tautulli/models/stream_data.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/synced_items.py` & `tautulli-3.4.0.2120/tautulli/models/synced_items.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/tautulli_info.py` & `tautulli-3.4.0.2120/tautulli/models/tautulli_info.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/user.py` & `tautulli-3.4.0.2120/tautulli/models/user.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/user_ips.py` & `tautulli-3.4.0.2120/tautulli/models/user_ips.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/user_logins.py` & `tautulli-3.4.0.2120/tautulli/models/user_logins.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/user_player_stats.py` & `tautulli-3.4.0.2120/tautulli/models/user_player_stats.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/users.py` & `tautulli-3.4.0.2120/tautulli/models/users.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/users_table.py` & `tautulli-3.4.0.2120/tautulli/models/users_table.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/models/whois_lookup.py` & `tautulli-3.4.0.2120/tautulli/models/whois_lookup.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/tools/api_helper.py` & `tautulli-3.4.0.2120/tautulli/tools/api_helper.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli/tools/utils.py` & `tautulli-3.4.0.2120/tautulli/tools/utils.py`

 * *Files identical despite different names*

### Comparing `tautulli-3.3.1.2120/tautulli.egg-info/PKG-INFO` & `tautulli-3.4.0.2120/tautulli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tautulli
-Version: 3.3.1.2120
+Version: 3.4.0.2120
 Summary: A complete Python client for Tautulli's API
 Home-page: https://github.com/nwithan8/pytulli
 Author: Nate Harris
 Author-email: n8gr8gbln@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/nwithan8/pytulli/archive/refs/tags/3.3.1.2120.tar.gz
+Download-URL: https://github.com/nwithan8/pytulli/archive/refs/tags/3.4.0.2120.tar.gz
 Description: # A Python client for Tautulli's API
         [![PyPi](https://img.shields.io/pypi/dm/tautulli?label=Downloads&logo=pypi)](https://pypi.org/project/tautulli)
         [![License](https://img.shields.io/pypi/l/tautulli?color=orange&style=flat-square)](https://github.com/nwithan8/pytulli/blob/master/LICENSE)
         
         [![Open Issues](https://img.shields.io/github/issues-raw/nwithan8/pytulli?color=gold&style=flat-square)](https://github.com/nwithan8/pytulli/issues?q=is%3Aopen+is%3Aissue)
         [![Closed Issues](https://img.shields.io/github/issues-closed-raw/nwithan8/pytulli?color=black&style=flat-square)](https://github.com/nwithan8/pytulli/issues?q=is%3Aissue+is%3Aclosed)
         [![Latest Release](https://img.shields.io/github/v/release/nwithan8/pytulli?color=red&label=latest%20release&logo=github&style=flat-square)](https://github.com/nwithan8/pytulli/releases)
```

### Comparing `tautulli-3.3.1.2120/tautulli.egg-info/SOURCES.txt` & `tautulli-3.4.0.2120/tautulli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

