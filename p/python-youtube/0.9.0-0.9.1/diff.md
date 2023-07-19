# Comparing `tmp/python_youtube-0.9.0.tar.gz` & `tmp/python_youtube-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_youtube-0.9.0.tar", max compression
+gzip compressed data, was "python_youtube-0.9.1.tar", max compression
```

## Comparing `python_youtube-0.9.0.tar` & `python_youtube-0.9.1.tar`

### file list

```diff
@@ -1,122 +1,121 @@
--rw-r--r--   0        0        0     1065 2022-12-26 02:41:16.449888 python_youtube-0.9.0/LICENSE
--rw-r--r--   0        0        0    25805 2022-12-26 02:41:16.449888 python_youtube-0.9.0/README.rst
--rw-r--r--   0        0        0     1340 2022-12-26 02:41:16.453888 python_youtube-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      167 2022-12-26 02:41:16.453888 python_youtube-0.9.0/pyyoutube/__init__.py
--rw-r--r--   0        0        0      705 2022-12-26 02:41:16.453888 python_youtube-0.9.0/pyyoutube/__version__.py
--rw-r--r--   0        0        0   101095 2022-12-26 02:41:16.453888 python_youtube-0.9.0/pyyoutube/api.py
--rw-r--r--   0        0        0    15757 2022-12-26 02:41:16.453888 python_youtube-0.9.0/pyyoutube/client.py
--rw-r--r--   0        0        0     2381 2022-12-26 02:41:16.453888 python_youtube-0.9.0/pyyoutube/error.py
--rw-r--r--   0        0        0     7027 2022-12-26 02:41:16.453888 python_youtube-0.9.0/pyyoutube/media.py
--rw-r--r--   0        0        0      667 2022-12-26 02:41:16.453888 python_youtube-0.9.0/pyyoutube/models/__init__.py
--rw-r--r--   0        0        0     6266 2022-12-26 02:41:16.453888 python_youtube-0.9.0/pyyoutube/models/activity.py
--rw-r--r--   0        0        0     1212 2022-12-26 02:41:16.453888 python_youtube-0.9.0/pyyoutube/models/auth.py
--rw-r--r--   0        0        0      690 2022-12-26 02:41:16.453888 python_youtube-0.9.0/pyyoutube/models/base.py
--rw-r--r--   0        0        0     1770 2022-12-26 02:41:16.453888 python_youtube-0.9.0/pyyoutube/models/caption.py
--rw-r--r--   0        0        0     1299 2022-12-26 02:41:16.453888 python_youtube-0.9.0/pyyoutube/models/category.py
--rw-r--r--   0        0        0     6690 2022-12-26 02:41:16.453888 python_youtube-0.9.0/pyyoutube/models/channel.py
--rw-r--r--   0        0        0      596 2022-12-26 02:41:16.453888 python_youtube-0.9.0/pyyoutube/models/channel_banner.py
--rw-r--r--   0        0        0     1784 2022-12-26 02:41:16.453888 python_youtube-0.9.0/pyyoutube/models/channel_section.py
--rw-r--r--   0        0        0     2247 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/models/comment.py
--rw-r--r--   0        0        0     1737 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/models/comment_thread.py
--rw-r--r--   0        0        0     5085 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/models/common.py
--rw-r--r--   0        0        0     1944 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/models/i18n.py
--rw-r--r--   0        0        0     2958 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/models/member.py
--rw-r--r--   0        0        0     1305 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/models/memberships_level.py
--rw-r--r--   0        0        0      813 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/models/mixins.py
--rw-r--r--   0        0        0     2250 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/models/playlist.py
--rw-r--r--   0        0        0     2751 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/models/playlist_item.py
--rw-r--r--   0        0        0     2010 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/models/search_result.py
--rw-r--r--   0        0        0     2568 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/models/subscription.py
--rw-r--r--   0        0        0    12219 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/models/video.py
--rw-r--r--   0        0        0     1533 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/models/video_abuse_report_reason.py
--rw-r--r--   0        0        0     1063 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/models/watermark.py
--rw-r--r--   0        0        0     1089 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/resources/__init__.py
--rw-r--r--   0        0        0     3723 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/resources/activities.py
--rw-r--r--   0        0        0      444 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/resources/base_resource.py
--rw-r--r--   0        0        0     9791 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/resources/captions.py
--rw-r--r--   0        0        0     2034 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/resources/channel_banners.py
--rw-r--r--   0        0        0    11405 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/resources/channel_sections.py
--rw-r--r--   0        0        0     7718 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/resources/channels.py
--rw-r--r--   0        0        0     7024 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/resources/comment_threads.py
--rw-r--r--   0        0        0     9155 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/resources/comments.py
--rw-r--r--   0        0        0     1889 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/resources/i18n_languages.py
--rw-r--r--   0        0        0     1821 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/resources/i18n_regions.py
--rw-r--r--   0        0        0     3160 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/resources/members.py
--rw-r--r--   0        0        0     1648 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/resources/membership_levels.py
--rw-r--r--   0        0        0    10667 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/resources/playlist_items.py
--rw-r--r--   0        0        0    12569 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/resources/playlists.py
--rw-r--r--   0        0        0    13674 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/resources/search.py
--rw-r--r--   0        0        0     9109 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/resources/subscriptions.py
--rw-r--r--   0        0        0      975 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/resources/thumbnails.py
--rw-r--r--   0        0        0     1951 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/resources/video_abuse_report_reasons.py
--rw-r--r--   0        0        0     2933 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/resources/video_categories.py
--rw-r--r--   0        0        0    19004 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/resources/videos.py
--rw-r--r--   0        0        0     3937 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/resources/watermarks.py
--rw-r--r--   0        0        0        0 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/utils/__init__.py
--rw-r--r--   0        0        0     4527 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/utils/constants.py
--rw-r--r--   0        0        0     3146 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/utils/params_checker.py
--rw-r--r--   0        0        0      864 2022-12-26 02:41:16.457888 python_youtube-0.9.0/pyyoutube/youtube_utils.py
--rw-r--r--   0        0        0        0 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/apis/__init__.py
--rw-r--r--   0        0        0     3499 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/apis/test_activities.py
--rw-r--r--   0        0        0     2928 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/apis/test_auth.py
--rw-r--r--   0        0        0     1830 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/apis/test_captions.py
--rw-r--r--   0        0        0     2256 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/apis/test_categories.py
--rw-r--r--   0        0        0     2655 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/apis/test_channel_sections.py
--rw-r--r--   0        0        0     3461 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/apis/test_channels.py
--rw-r--r--   0        0        0     6628 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/apis/test_comment_threads.py
--rw-r--r--   0        0        0     4579 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/apis/test_comments.py
--rw-r--r--   0        0        0     1625 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/apis/test_i18ns.py
--rw-r--r--   0        0        0     1907 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/apis/test_members.py
--rw-r--r--   0        0        0     5894 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/apis/test_playlist_items.py
--rw-r--r--   0        0        0     4336 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/apis/test_playlists.py
--rw-r--r--   0        0        0     7183 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/apis/test_search.py
--rw-r--r--   0        0        0     8062 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/apis/test_subscriptions.py
--rw-r--r--   0        0        0     1131 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/apis/test_video_abuse_reason.py
--rw-r--r--   0        0        0     7709 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/apis/test_videos.py
--rw-r--r--   0        0        0        0 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/clients/__init__.py
--rw-r--r--   0        0        0      355 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/clients/base.py
--rw-r--r--   0        0        0     1071 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/clients/test_activities.py
--rw-r--r--   0        0        0     3378 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/clients/test_captions.py
--rw-r--r--   0        0        0      390 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/clients/test_channel_banners.py
--rw-r--r--   0        0        0     3977 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/clients/test_channel_sections.py
--rw-r--r--   0        0        0     2878 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/clients/test_channels.py
--rw-r--r--   0        0        0     2819 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/clients/test_client.py
--rw-r--r--   0        0        0     2414 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/clients/test_comment_threads.py
--rw-r--r--   0        0        0     5118 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/clients/test_comments.py
--rw-r--r--   0        0        0     1018 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/clients/test_i18n.py
--rw-r--r--   0        0        0     4063 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/clients/test_media.py
--rw-r--r--   0        0        0      575 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/clients/test_members.py
--rw-r--r--   0        0        0      548 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/clients/test_membership_levels.py
--rw-r--r--   0        0        0     3626 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/clients/test_playlist_items.py
--rw-r--r--   0        0        0     3222 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/clients/test_playlists.py
--rw-r--r--   0        0        0     2049 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/clients/test_search.py
--rw-r--r--   0        0        0     3617 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/clients/test_subscriptions.py
--rw-r--r--   0        0        0      488 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/clients/test_thumbnails.py
--rw-r--r--   0        0        0      571 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/clients/test_video_abuse_report_reasons.py
--rw-r--r--   0        0        0     1196 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/clients/test_video_categories.py
--rw-r--r--   0        0        0     5075 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/clients/test_videos.py
--rw-r--r--   0        0        0     1544 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/clients/test_watermarks.py
--rw-r--r--   0        0        0      577 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/models/__init__.py
--rw-r--r--   0        0        0      942 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/models/test_abuse_reason.py
--rw-r--r--   0        0        0     1685 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/models/test_activities.py
--rw-r--r--   0        0        0      881 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/models/test_auth_models.py
--rw-r--r--   0        0        0     1326 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/models/test_captions.py
--rw-r--r--   0        0        0     1204 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/models/test_category.py
--rw-r--r--   0        0        0     3346 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/models/test_channel.py
--rw-r--r--   0        0        0     1006 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/models/test_channel_sections.py
--rw-r--r--   0        0        0     3521 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/models/test_comments.py
--rw-r--r--   0        0        0     1447 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/models/test_i18n_models.py
--rw-r--r--   0        0        0     1069 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/models/test_members.py
--rw-r--r--   0        0        0     2200 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/models/test_playlist.py
--rw-r--r--   0        0        0     2883 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/models/test_playlist_item.py
--rw-r--r--   0        0        0     1831 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/models/test_search_result.py
--rw-r--r--   0        0        0     2388 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/models/test_subscriptions.py
--rw-r--r--   0        0        0     3723 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/models/test_videos.py
--rw-r--r--   0        0        0     1498 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/test_error_handling.py
--rw-r--r--   0        0        0      415 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/test_youtube_utils.py
--rw-r--r--   0        0        0        0 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     1581 2022-12-26 02:41:16.465888 python_youtube-0.9.0/tests/utils/test_params_checker.py
--rw-r--r--   0        0        0    27938 1970-01-01 00:00:00.000000 python_youtube-0.9.0/setup.py
--rw-r--r--   0        0        0    27387 1970-01-01 00:00:00.000000 python_youtube-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-19 10:20:57.912924 python_youtube-0.9.1/LICENSE
+-rw-r--r--   0        0        0     6342 2023-07-19 10:20:57.912924 python_youtube-0.9.1/README.rst
+-rw-r--r--   0        0        0     1351 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      167 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/__init__.py
+-rw-r--r--   0        0        0      705 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/__version__.py
+-rw-r--r--   0        0        0   101095 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/api.py
+-rw-r--r--   0        0        0    15757 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/client.py
+-rw-r--r--   0        0        0     2381 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/error.py
+-rw-r--r--   0        0        0     7027 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/media.py
+-rw-r--r--   0        0        0      667 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/models/__init__.py
+-rw-r--r--   0        0        0     6266 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/models/activity.py
+-rw-r--r--   0        0        0     1212 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/models/auth.py
+-rw-r--r--   0        0        0      690 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/models/base.py
+-rw-r--r--   0        0        0     1770 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/models/caption.py
+-rw-r--r--   0        0        0     1299 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/models/category.py
+-rw-r--r--   0        0        0     6690 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/models/channel.py
+-rw-r--r--   0        0        0      596 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/models/channel_banner.py
+-rw-r--r--   0        0        0     1784 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/models/channel_section.py
+-rw-r--r--   0        0        0     2247 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/models/comment.py
+-rw-r--r--   0        0        0     1737 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/models/comment_thread.py
+-rw-r--r--   0        0        0     5085 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/models/common.py
+-rw-r--r--   0        0        0     1944 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/models/i18n.py
+-rw-r--r--   0        0        0     2958 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/models/member.py
+-rw-r--r--   0        0        0     1305 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/models/memberships_level.py
+-rw-r--r--   0        0        0      813 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/models/mixins.py
+-rw-r--r--   0        0        0     2250 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/models/playlist.py
+-rw-r--r--   0        0        0     2751 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/models/playlist_item.py
+-rw-r--r--   0        0        0     2010 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/models/search_result.py
+-rw-r--r--   0        0        0     2568 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/models/subscription.py
+-rw-r--r--   0        0        0    12219 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/models/video.py
+-rw-r--r--   0        0        0     1533 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/models/video_abuse_report_reason.py
+-rw-r--r--   0        0        0     1063 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/models/watermark.py
+-rw-r--r--   0        0        0     1089 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/resources/__init__.py
+-rw-r--r--   0        0        0     3723 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/resources/activities.py
+-rw-r--r--   0        0        0      444 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/resources/base_resource.py
+-rw-r--r--   0        0        0     9791 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/resources/captions.py
+-rw-r--r--   0        0        0     2034 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/resources/channel_banners.py
+-rw-r--r--   0        0        0    11405 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/resources/channel_sections.py
+-rw-r--r--   0        0        0     7718 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/resources/channels.py
+-rw-r--r--   0        0        0     7024 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/resources/comment_threads.py
+-rw-r--r--   0        0        0     9155 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/resources/comments.py
+-rw-r--r--   0        0        0     1889 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/resources/i18n_languages.py
+-rw-r--r--   0        0        0     1821 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/resources/i18n_regions.py
+-rw-r--r--   0        0        0     3160 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/resources/members.py
+-rw-r--r--   0        0        0     1648 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/resources/membership_levels.py
+-rw-r--r--   0        0        0    10667 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/resources/playlist_items.py
+-rw-r--r--   0        0        0    12569 2023-07-19 10:20:57.920924 python_youtube-0.9.1/pyyoutube/resources/playlists.py
+-rw-r--r--   0        0        0    13674 2023-07-19 10:20:57.924924 python_youtube-0.9.1/pyyoutube/resources/search.py
+-rw-r--r--   0        0        0     9109 2023-07-19 10:20:57.924924 python_youtube-0.9.1/pyyoutube/resources/subscriptions.py
+-rw-r--r--   0        0        0      975 2023-07-19 10:20:57.924924 python_youtube-0.9.1/pyyoutube/resources/thumbnails.py
+-rw-r--r--   0        0        0     1951 2023-07-19 10:20:57.924924 python_youtube-0.9.1/pyyoutube/resources/video_abuse_report_reasons.py
+-rw-r--r--   0        0        0     2933 2023-07-19 10:20:57.924924 python_youtube-0.9.1/pyyoutube/resources/video_categories.py
+-rw-r--r--   0        0        0    19004 2023-07-19 10:20:57.924924 python_youtube-0.9.1/pyyoutube/resources/videos.py
+-rw-r--r--   0        0        0     3937 2023-07-19 10:20:57.924924 python_youtube-0.9.1/pyyoutube/resources/watermarks.py
+-rw-r--r--   0        0        0        0 2023-07-19 10:20:57.924924 python_youtube-0.9.1/pyyoutube/utils/__init__.py
+-rw-r--r--   0        0        0     4527 2023-07-19 10:20:57.924924 python_youtube-0.9.1/pyyoutube/utils/constants.py
+-rw-r--r--   0        0        0     3146 2023-07-19 10:20:57.924924 python_youtube-0.9.1/pyyoutube/utils/params_checker.py
+-rw-r--r--   0        0        0      864 2023-07-19 10:20:57.924924 python_youtube-0.9.1/pyyoutube/youtube_utils.py
+-rw-r--r--   0        0        0        0 2023-07-19 10:20:57.932924 python_youtube-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 10:20:57.932924 python_youtube-0.9.1/tests/apis/__init__.py
+-rw-r--r--   0        0        0     3499 2023-07-19 10:20:57.932924 python_youtube-0.9.1/tests/apis/test_activities.py
+-rw-r--r--   0        0        0     2928 2023-07-19 10:20:57.932924 python_youtube-0.9.1/tests/apis/test_auth.py
+-rw-r--r--   0        0        0     1830 2023-07-19 10:20:57.932924 python_youtube-0.9.1/tests/apis/test_captions.py
+-rw-r--r--   0        0        0     2256 2023-07-19 10:20:57.932924 python_youtube-0.9.1/tests/apis/test_categories.py
+-rw-r--r--   0        0        0     2655 2023-07-19 10:20:57.932924 python_youtube-0.9.1/tests/apis/test_channel_sections.py
+-rw-r--r--   0        0        0     3461 2023-07-19 10:20:57.932924 python_youtube-0.9.1/tests/apis/test_channels.py
+-rw-r--r--   0        0        0     6628 2023-07-19 10:20:57.932924 python_youtube-0.9.1/tests/apis/test_comment_threads.py
+-rw-r--r--   0        0        0     4579 2023-07-19 10:20:57.932924 python_youtube-0.9.1/tests/apis/test_comments.py
+-rw-r--r--   0        0        0     1625 2023-07-19 10:20:57.932924 python_youtube-0.9.1/tests/apis/test_i18ns.py
+-rw-r--r--   0        0        0     1907 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/apis/test_members.py
+-rw-r--r--   0        0        0     5894 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/apis/test_playlist_items.py
+-rw-r--r--   0        0        0     4336 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/apis/test_playlists.py
+-rw-r--r--   0        0        0     7183 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/apis/test_search.py
+-rw-r--r--   0        0        0     8062 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/apis/test_subscriptions.py
+-rw-r--r--   0        0        0     1131 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/apis/test_video_abuse_reason.py
+-rw-r--r--   0        0        0     7709 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/apis/test_videos.py
+-rw-r--r--   0        0        0        0 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/clients/__init__.py
+-rw-r--r--   0        0        0      355 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/clients/base.py
+-rw-r--r--   0        0        0     1071 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/clients/test_activities.py
+-rw-r--r--   0        0        0     3378 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/clients/test_captions.py
+-rw-r--r--   0        0        0      390 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/clients/test_channel_banners.py
+-rw-r--r--   0        0        0     3977 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/clients/test_channel_sections.py
+-rw-r--r--   0        0        0     2878 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/clients/test_channels.py
+-rw-r--r--   0        0        0     2819 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/clients/test_client.py
+-rw-r--r--   0        0        0     2414 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/clients/test_comment_threads.py
+-rw-r--r--   0        0        0     5118 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/clients/test_comments.py
+-rw-r--r--   0        0        0     1018 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/clients/test_i18n.py
+-rw-r--r--   0        0        0     4063 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/clients/test_media.py
+-rw-r--r--   0        0        0      575 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/clients/test_members.py
+-rw-r--r--   0        0        0      548 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/clients/test_membership_levels.py
+-rw-r--r--   0        0        0     3626 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/clients/test_playlist_items.py
+-rw-r--r--   0        0        0     3222 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/clients/test_playlists.py
+-rw-r--r--   0        0        0     2049 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/clients/test_search.py
+-rw-r--r--   0        0        0     3617 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/clients/test_subscriptions.py
+-rw-r--r--   0        0        0      488 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/clients/test_thumbnails.py
+-rw-r--r--   0        0        0      571 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/clients/test_video_abuse_report_reasons.py
+-rw-r--r--   0        0        0     1196 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/clients/test_video_categories.py
+-rw-r--r--   0        0        0     5075 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/clients/test_videos.py
+-rw-r--r--   0        0        0     1544 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/clients/test_watermarks.py
+-rw-r--r--   0        0        0      577 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/models/__init__.py
+-rw-r--r--   0        0        0      942 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/models/test_abuse_reason.py
+-rw-r--r--   0        0        0     1685 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/models/test_activities.py
+-rw-r--r--   0        0        0      881 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/models/test_auth_models.py
+-rw-r--r--   0        0        0     1326 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/models/test_captions.py
+-rw-r--r--   0        0        0     1204 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/models/test_category.py
+-rw-r--r--   0        0        0     3344 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/models/test_channel.py
+-rw-r--r--   0        0        0     1006 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/models/test_channel_sections.py
+-rw-r--r--   0        0        0     3521 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/models/test_comments.py
+-rw-r--r--   0        0        0     1447 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/models/test_i18n_models.py
+-rw-r--r--   0        0        0     1069 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/models/test_members.py
+-rw-r--r--   0        0        0     2200 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/models/test_playlist.py
+-rw-r--r--   0        0        0     2883 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/models/test_playlist_item.py
+-rw-r--r--   0        0        0     1831 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/models/test_search_result.py
+-rw-r--r--   0        0        0     2388 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/models/test_subscriptions.py
+-rw-r--r--   0        0        0     3721 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/models/test_videos.py
+-rw-r--r--   0        0        0     1498 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/test_error_handling.py
+-rw-r--r--   0        0        0      415 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/test_youtube_utils.py
+-rw-r--r--   0        0        0        0 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1581 2023-07-19 10:20:57.936924 python_youtube-0.9.1/tests/utils/test_params_checker.py
+-rw-r--r--   0        0        0     7724 1970-01-01 00:00:00.000000 python_youtube-0.9.1/PKG-INFO
```

### Comparing `python_youtube-0.9.0/LICENSE` & `python_youtube-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyproject.toml` & `python_youtube-0.9.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-youtube"
-version = "0.9.0"
+version = "0.9.1"
 description = "A Python wrapper around for YouTube Data API."
 authors = ["ikaroskun <merle.liukun@gmail.com>"]
 license = "MIT"
 keywords = ["youtube-api", "youtube-v3-api", "youtube-data-api", "youtube-sdk"]
 readme = "README.rst"
 homepage = "https://github.com/sns-sdks/python-youtube"
 repository = "https://github.com/sns-sdks/python-youtube"
@@ -35,9 +35,9 @@
 
 [tool.poetry.dev-dependencies]
 responses = "^0.12.0"
 pytest = "^6.0.2"
 pytest-cov = "^2.10.1"
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `python_youtube-0.9.0/pyyoutube/__version__.py` & `python_youtube-0.9.1/pyyoutube/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 # d8888b. db    db d888888b db   db  .d88b.  d8b   db db    db  .d88b.  db    db d888888b db    db d8888b. d88888b
 # 88  `8D `8b  d8' `~~88~~' 88   88 .8P  Y8. 888o  88 `8b  d8' .8P  Y8. 88    88 `~~88~~' 88    88 88  `8D 88'
 # 88oodD'  `8bd8'     88    88ooo88 88    88 88V8o 88  `8bd8'  88    88 88    88    88    88    88 88oooY' 88ooooo
 # 88~~~      88       88    88~~~88 88    88 88 V8o88    88    88    88 88    88    88    88    88 88~~~b. 88~~~~~
 # 88         88       88    88   88 `8b  d8' 88  V888    88    `8b  d8' 88b  d88    88    88b  d88 88   8D 88.
 # 88         YP       YP    YP   YP  `Y88P'  VP   V8P    YP     `Y88P'  ~Y8888P'    YP    ~Y8888P' Y8888P' Y88888P
 
-__version__ = "0.9.0"
+__version__ = "0.9.1"
```

### Comparing `python_youtube-0.9.0/pyyoutube/api.py` & `python_youtube-0.9.1/pyyoutube/api.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/client.py` & `python_youtube-0.9.1/pyyoutube/client.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/error.py` & `python_youtube-0.9.1/pyyoutube/error.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/media.py` & `python_youtube-0.9.1/pyyoutube/media.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/models/__init__.py` & `python_youtube-0.9.1/pyyoutube/models/__init__.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/models/activity.py` & `python_youtube-0.9.1/pyyoutube/models/activity.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/models/auth.py` & `python_youtube-0.9.1/pyyoutube/models/auth.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/models/base.py` & `python_youtube-0.9.1/pyyoutube/models/base.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/models/caption.py` & `python_youtube-0.9.1/pyyoutube/models/caption.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/models/category.py` & `python_youtube-0.9.1/pyyoutube/models/category.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/models/channel.py` & `python_youtube-0.9.1/pyyoutube/models/channel.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/models/channel_banner.py` & `python_youtube-0.9.1/pyyoutube/models/channel_banner.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/models/channel_section.py` & `python_youtube-0.9.1/pyyoutube/models/channel_section.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/models/comment.py` & `python_youtube-0.9.1/pyyoutube/models/comment.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/models/comment_thread.py` & `python_youtube-0.9.1/pyyoutube/models/comment_thread.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/models/common.py` & `python_youtube-0.9.1/pyyoutube/models/common.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/models/i18n.py` & `python_youtube-0.9.1/pyyoutube/models/i18n.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/models/member.py` & `python_youtube-0.9.1/pyyoutube/models/member.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/models/memberships_level.py` & `python_youtube-0.9.1/pyyoutube/models/memberships_level.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/models/mixins.py` & `python_youtube-0.9.1/pyyoutube/models/mixins.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/models/playlist.py` & `python_youtube-0.9.1/pyyoutube/models/playlist.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/models/playlist_item.py` & `python_youtube-0.9.1/pyyoutube/models/playlist_item.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/models/search_result.py` & `python_youtube-0.9.1/pyyoutube/models/search_result.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/models/subscription.py` & `python_youtube-0.9.1/pyyoutube/models/subscription.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/models/video.py` & `python_youtube-0.9.1/pyyoutube/models/video.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/models/video_abuse_report_reason.py` & `python_youtube-0.9.1/pyyoutube/models/video_abuse_report_reason.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/models/watermark.py` & `python_youtube-0.9.1/pyyoutube/models/watermark.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/resources/__init__.py` & `python_youtube-0.9.1/pyyoutube/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/resources/activities.py` & `python_youtube-0.9.1/pyyoutube/resources/activities.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/resources/captions.py` & `python_youtube-0.9.1/pyyoutube/resources/captions.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/resources/channel_banners.py` & `python_youtube-0.9.1/pyyoutube/resources/channel_banners.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/resources/channel_sections.py` & `python_youtube-0.9.1/pyyoutube/resources/channel_sections.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/resources/channels.py` & `python_youtube-0.9.1/pyyoutube/resources/channels.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/resources/comment_threads.py` & `python_youtube-0.9.1/pyyoutube/resources/comment_threads.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/resources/comments.py` & `python_youtube-0.9.1/pyyoutube/resources/comments.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/resources/i18n_languages.py` & `python_youtube-0.9.1/pyyoutube/resources/i18n_languages.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/resources/i18n_regions.py` & `python_youtube-0.9.1/pyyoutube/resources/i18n_regions.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/resources/members.py` & `python_youtube-0.9.1/pyyoutube/resources/members.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/resources/membership_levels.py` & `python_youtube-0.9.1/pyyoutube/resources/membership_levels.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/resources/playlist_items.py` & `python_youtube-0.9.1/pyyoutube/resources/playlist_items.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/resources/playlists.py` & `python_youtube-0.9.1/pyyoutube/resources/playlists.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/resources/search.py` & `python_youtube-0.9.1/pyyoutube/resources/search.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/resources/subscriptions.py` & `python_youtube-0.9.1/pyyoutube/resources/subscriptions.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/resources/thumbnails.py` & `python_youtube-0.9.1/pyyoutube/resources/thumbnails.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/resources/video_abuse_report_reasons.py` & `python_youtube-0.9.1/pyyoutube/resources/video_abuse_report_reasons.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/resources/video_categories.py` & `python_youtube-0.9.1/pyyoutube/resources/video_categories.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/resources/videos.py` & `python_youtube-0.9.1/pyyoutube/resources/videos.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/resources/watermarks.py` & `python_youtube-0.9.1/pyyoutube/resources/watermarks.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/utils/constants.py` & `python_youtube-0.9.1/pyyoutube/utils/constants.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/utils/params_checker.py` & `python_youtube-0.9.1/pyyoutube/utils/params_checker.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/pyyoutube/youtube_utils.py` & `python_youtube-0.9.1/pyyoutube/youtube_utils.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/apis/test_activities.py` & `python_youtube-0.9.1/tests/apis/test_activities.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/apis/test_auth.py` & `python_youtube-0.9.1/tests/apis/test_auth.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/apis/test_captions.py` & `python_youtube-0.9.1/tests/apis/test_captions.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/apis/test_categories.py` & `python_youtube-0.9.1/tests/apis/test_categories.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/apis/test_channel_sections.py` & `python_youtube-0.9.1/tests/apis/test_channel_sections.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/apis/test_channels.py` & `python_youtube-0.9.1/tests/apis/test_channels.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/apis/test_comment_threads.py` & `python_youtube-0.9.1/tests/apis/test_comment_threads.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/apis/test_comments.py` & `python_youtube-0.9.1/tests/apis/test_comments.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/apis/test_i18ns.py` & `python_youtube-0.9.1/tests/apis/test_i18ns.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/apis/test_members.py` & `python_youtube-0.9.1/tests/apis/test_members.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/apis/test_playlist_items.py` & `python_youtube-0.9.1/tests/apis/test_playlist_items.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/apis/test_playlists.py` & `python_youtube-0.9.1/tests/apis/test_playlists.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/apis/test_search.py` & `python_youtube-0.9.1/tests/apis/test_search.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/apis/test_subscriptions.py` & `python_youtube-0.9.1/tests/apis/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/apis/test_video_abuse_reason.py` & `python_youtube-0.9.1/tests/apis/test_video_abuse_reason.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/apis/test_videos.py` & `python_youtube-0.9.1/tests/apis/test_videos.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/clients/test_activities.py` & `python_youtube-0.9.1/tests/clients/test_activities.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/clients/test_captions.py` & `python_youtube-0.9.1/tests/clients/test_captions.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/clients/test_channel_sections.py` & `python_youtube-0.9.1/tests/clients/test_channel_sections.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/clients/test_channels.py` & `python_youtube-0.9.1/tests/clients/test_channels.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/clients/test_client.py` & `python_youtube-0.9.1/tests/clients/test_client.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/clients/test_comment_threads.py` & `python_youtube-0.9.1/tests/clients/test_comment_threads.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/clients/test_comments.py` & `python_youtube-0.9.1/tests/clients/test_comments.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/clients/test_i18n.py` & `python_youtube-0.9.1/tests/clients/test_i18n.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/clients/test_media.py` & `python_youtube-0.9.1/tests/clients/test_media.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/clients/test_members.py` & `python_youtube-0.9.1/tests/clients/test_members.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/clients/test_membership_levels.py` & `python_youtube-0.9.1/tests/clients/test_membership_levels.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/clients/test_playlist_items.py` & `python_youtube-0.9.1/tests/clients/test_playlist_items.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/clients/test_playlists.py` & `python_youtube-0.9.1/tests/clients/test_playlists.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/clients/test_search.py` & `python_youtube-0.9.1/tests/clients/test_search.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/clients/test_subscriptions.py` & `python_youtube-0.9.1/tests/clients/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/clients/test_video_abuse_report_reasons.py` & `python_youtube-0.9.1/tests/clients/test_video_abuse_report_reasons.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/clients/test_video_categories.py` & `python_youtube-0.9.1/tests/clients/test_video_categories.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/clients/test_videos.py` & `python_youtube-0.9.1/tests/clients/test_videos.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/clients/test_watermarks.py` & `python_youtube-0.9.1/tests/clients/test_watermarks.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/conftest.py` & `python_youtube-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/models/test_abuse_reason.py` & `python_youtube-0.9.1/tests/models/test_abuse_reason.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/models/test_activities.py` & `python_youtube-0.9.1/tests/models/test_activities.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/models/test_auth_models.py` & `python_youtube-0.9.1/tests/models/test_auth_models.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/models/test_captions.py` & `python_youtube-0.9.1/tests/models/test_captions.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/models/test_category.py` & `python_youtube-0.9.1/tests/models/test_category.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/models/test_channel.py` & `python_youtube-0.9.1/tests/models/test_channel.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
         published_at = m.string_to_datetime(m.publishedAt)
         self.assertEqual(published_at.isoformat(), "2007-08-23T00:34:43+00:00")
 
     def testChannelStatistics(self) -> None:
         m = models.ChannelStatistics.from_dict(self.STATISTICS_INFO)
 
-        self.assertEqual(m.viewCount, "160361638")
+        self.assertEqual(m.viewCount, 160361638)
 
     def testChannelStatus(self) -> None:
         m = models.ChannelStatus.from_dict(self.STATUS_INFO)
 
         self.assertEqual(m.privacyStatus, "public")
 
     def testChannel(self) -> None:
```

### Comparing `python_youtube-0.9.0/tests/models/test_channel_sections.py` & `python_youtube-0.9.1/tests/models/test_channel_sections.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/models/test_comments.py` & `python_youtube-0.9.1/tests/models/test_comments.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/models/test_i18n_models.py` & `python_youtube-0.9.1/tests/models/test_i18n_models.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/models/test_members.py` & `python_youtube-0.9.1/tests/models/test_members.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/models/test_playlist.py` & `python_youtube-0.9.1/tests/models/test_playlist.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/models/test_playlist_item.py` & `python_youtube-0.9.1/tests/models/test_playlist_item.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/models/test_search_result.py` & `python_youtube-0.9.1/tests/models/test_search_result.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/models/test_subscriptions.py` & `python_youtube-0.9.1/tests/models/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/models/test_videos.py` & `python_youtube-0.9.1/tests/models/test_videos.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         self.assertEqual(
             m.localized.title, "What are Actions on Google (Assistant on Air)"
         )
 
     def testVideoStatistics(self) -> None:
         m = models.VideoStatistics.from_dict(self.STATISTICS_INFO)
 
-        self.assertEqual(m.viewCount, "8087")
+        self.assertEqual(m.viewCount, 8087)
 
     def testVideoStatus(self) -> None:
         m = models.VideoStatus.from_dict(self.STATUS_INFO)
 
         self.assertEqual(m.uploadStatus, "processed")
 
         self.assertEqual(
```

### Comparing `python_youtube-0.9.0/tests/test_error_handling.py` & `python_youtube-0.9.1/tests/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `python_youtube-0.9.0/tests/utils/test_params_checker.py` & `python_youtube-0.9.1/tests/utils/test_params_checker.py`

 * *Files identical despite different names*

