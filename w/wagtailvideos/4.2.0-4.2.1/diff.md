# Comparing `tmp/wagtailvideos-4.2.0.tar.gz` & `tmp/wagtailvideos-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailvideos-4.2.0.tar", last modified: Sat Feb 25 23:37:34 2023, max compression
+gzip compressed data, was "wagtailvideos-4.2.1.tar", last modified: Wed Jul 19 00:21:19 2023, max compression
```

## Comparing `wagtailvideos-4.2.0.tar` & `wagtailvideos-4.2.1.tar`

### file list

```diff
@@ -1,101 +1,103 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 23:37:34.276001 wagtailvideos-4.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1481 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5529 2023-02-25 23:37:34.276001 wagtailvideos-4.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4746 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-02-25 23:37:34.277001 wagtailvideos-4.2.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1285 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 23:37:34.250002 wagtailvideos-4.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 23:37:34.252001 wagtailvideos-4.2.0/tests/app/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/tests/app/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 23:37:34.253001 wagtailvideos-4.2.0/tests/app/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    32030 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/tests/app/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/tests/app/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1591 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/tests/app/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2169 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/tests/app/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/tests/app/test_block.py
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/tests/app/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     6455 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/tests/storage.py
--rw-rw-rw-   0 root         (0) root         (0)    24716 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/tests/test_admin_views.py
--rw-rw-rw-   0 root         (0) root         (0)     1352 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/tests/test_custom_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1628 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/tests/test_template_tag.py
--rw-rw-rw-   0 root         (0) root         (0)      358 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 23:37:34.258001 wagtailvideos-4.2.0/wagtailvideos/
--rw-rw-rw-   0 root         (0) root         (0)      846 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      858 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/blocks.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/edit_handlers.py
--rw-rw-rw-   0 root         (0) root         (0)     2106 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/ffmpeg.py
--rw-rw-rw-   0 root         (0) root         (0)     2113 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/fields.py
--rw-rw-rw-   0 root         (0) root         (0)     3206 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/forms.py
--rw-rw-rw-   0 root         (0) root         (0)      637 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/jinja2tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 23:37:34.266001 wagtailvideos-4.2.0/wagtailvideos/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1966 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/migrations/0002_auto_20160321_1610.py
--rw-rw-rw-   0 root         (0) root         (0)     1273 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/migrations/0003_auto_20160705_1646.py
--rw-rw-rw-   0 root         (0) root         (0)      599 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/migrations/0004_auto_20160706_1153.py
--rw-rw-rw-   0 root         (0) root         (0)      499 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/migrations/0005_videotranscode_error_message.py
--rw-rw-rw-   0 root         (0) root         (0)      585 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/migrations/0006_auto_20160707_1413.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/migrations/0007_video_duration.py
--rw-rw-rw-   0 root         (0) root         (0)      465 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/migrations/0008_auto_20160728_1523.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/migrations/0009_videotranscode_quality.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/migrations/0010_video_ordering.py
--rw-rw-rw-   0 root         (0) root         (0)    28229 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/migrations/0011_video_tracks.py
--rw-rw-rw-   0 root         (0) root         (0)    26753 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/migrations/0012_remove_unique_constraint.py
--rw-rw-rw-   0 root         (0) root         (0)     3473 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/migrations/0013_add_choose_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13354 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/models.py
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     2642 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 23:37:34.242002 wagtailvideos-4.2.0/wagtailvideos/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 23:37:34.242002 wagtailvideos-4.2.0/wagtailvideos/static/wagtailvideos/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 23:37:34.267001 wagtailvideos-4.2.0/wagtailvideos/static/wagtailvideos/css/
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/static/wagtailvideos/css/edit-video.css
--rw-rw-rw-   0 root         (0) root         (0)      364 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/static/wagtailvideos/css/summary-override.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 23:37:34.268001 wagtailvideos-4.2.0/wagtailvideos/static/wagtailvideos/js/
--rw-rw-rw-   0 root         (0) root         (0)     5536 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/static/wagtailvideos/js/add-multiple.js
--rw-rw-rw-   0 root         (0) root         (0)      316 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/static/wagtailvideos/js/video-chooser-telepath.js
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/static/wagtailvideos/js/video-chooser.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 23:37:34.243002 wagtailvideos-4.2.0/wagtailvideos/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 23:37:34.245002 wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 23:37:34.269001 wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/chooser/
--rw-rw-rw-   0 root         (0) root         (0)      926 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/chooser/chooser.html
--rw-rw-rw-   0 root         (0) root         (0)     1988 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/chooser/results.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 23:37:34.269001 wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/homepage/
--rw-rw-rw-   0 root         (0) root         (0)      480 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/homepage/videos_summary.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 23:37:34.270001 wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/multiple/
--rw-rw-rw-   0 root         (0) root         (0)     4414 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/multiple/add.html
--rw-rw-rw-   0 root         (0) root         (0)     1042 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/multiple/edit_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 23:37:34.244002 wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/permissions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 23:37:34.270001 wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/permissions/includes/
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/permissions/includes/video_permissions_formset.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 23:37:34.273001 wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/videos/
--rw-rw-rw-   0 root         (0) root         (0)      246 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/videos/_file_field.html
--rw-rw-rw-   0 root         (0) root         (0)      232 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/videos/_file_field_as_li.html
--rw-rw-rw-   0 root         (0) root         (0)     1222 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/videos/add.html
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/videos/confirm_delete.html
--rw-rw-rw-   0 root         (0) root         (0)     6496 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/videos/edit.html
--rw-rw-rw-   0 root         (0) root         (0)     1393 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/videos/index.html
--rw-rw-rw-   0 root         (0) root         (0)     2019 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/videos/results.html
--rw-rw-rw-   0 root         (0) root         (0)     1903 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/videos/usage.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 23:37:34.274001 wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/widgets/
--rw-rw-rw-   0 root         (0) root         (0)      442 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/widgets/video_chooser.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 23:37:34.274001 wagtailvideos-4.2.0/wagtailvideos/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/templatetags/wagtailvideos_tags.py
--rw-rw-rw-   0 root         (0) root         (0)      712 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 23:37:34.276001 wagtailvideos-4.2.0/wagtailvideos/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5285 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/views/chooser.py
--rw-rw-rw-   0 root         (0) root         (0)     4921 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/views/multiple.py
--rw-rw-rw-   0 root         (0) root         (0)     7923 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/views/videos.py
--rw-rw-rw-   0 root         (0) root         (0)     4344 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/wagtail_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     2085 2023-02-25 23:37:24.000000 wagtailvideos-4.2.0/wagtailvideos/widgets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-25 23:37:34.261001 wagtailvideos-4.2.0/wagtailvideos.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5529 2023-02-25 23:37:34.000000 wagtailvideos-4.2.0/wagtailvideos.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3077 2023-02-25 23:37:34.000000 wagtailvideos-4.2.0/wagtailvideos.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-25 23:37:34.000000 wagtailvideos-4.2.0/wagtailvideos.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-25 23:37:34.000000 wagtailvideos-4.2.0/wagtailvideos.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       91 2023-02-25 23:37:34.000000 wagtailvideos-4.2.0/wagtailvideos.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-02-25 23:37:34.000000 wagtailvideos-4.2.0/wagtailvideos.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.592485 wagtailvideos-4.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1481 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5529 2023-07-19 00:21:19.592485 wagtailvideos-4.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4746 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-07-19 00:21:19.592485 wagtailvideos-4.2.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1285 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.579485 wagtailvideos-4.2.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.580485 wagtailvideos-4.2.1/tests/app/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/app/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.580485 wagtailvideos-4.2.1/tests/app/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    32030 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/app/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      509 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/app/migrations/0002_alter_testpage_video_streamfield.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/app/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1668 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/app/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2218 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/app/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/app/test_block.py
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/app/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     6455 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/storage.py
+-rw-rw-rw-   0 root         (0) root         (0)    24716 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/test_admin_views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1352 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/test_custom_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1628 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/test_template_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)      358 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.583485 wagtailvideos-4.2.1/wagtailvideos/
+-rw-rw-rw-   0 root         (0) root         (0)      846 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      858 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/blocks.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/edit_handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2106 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/ffmpeg.py
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     3206 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)      637 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/jinja2tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.587485 wagtailvideos-4.2.1/wagtailvideos/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1966 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0002_auto_20160321_1610.py
+-rw-rw-rw-   0 root         (0) root         (0)     1273 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0003_auto_20160705_1646.py
+-rw-rw-rw-   0 root         (0) root         (0)      599 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0004_auto_20160706_1153.py
+-rw-rw-rw-   0 root         (0) root         (0)      499 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0005_videotranscode_error_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      585 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0006_auto_20160707_1413.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0007_video_duration.py
+-rw-rw-rw-   0 root         (0) root         (0)      465 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0008_auto_20160728_1523.py
+-rw-rw-rw-   0 root         (0) root         (0)      626 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0009_videotranscode_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0010_video_ordering.py
+-rw-rw-rw-   0 root         (0) root         (0)    28229 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0011_video_tracks.py
+-rw-rw-rw-   0 root         (0) root         (0)    26753 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0012_remove_unique_constraint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3473 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0013_add_choose_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)    44986 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/0014_alter_videotrack_file_alter_videotrack_kind_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13468 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2642 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.575485 wagtailvideos-4.2.1/wagtailvideos/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.575485 wagtailvideos-4.2.1/wagtailvideos/static/wagtailvideos/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.587485 wagtailvideos-4.2.1/wagtailvideos/static/wagtailvideos/css/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/static/wagtailvideos/css/edit-video.css
+-rw-rw-rw-   0 root         (0) root         (0)      364 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/static/wagtailvideos/css/summary-override.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.588485 wagtailvideos-4.2.1/wagtailvideos/static/wagtailvideos/js/
+-rw-rw-rw-   0 root         (0) root         (0)     5536 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/static/wagtailvideos/js/add-multiple.js
+-rw-rw-rw-   0 root         (0) root         (0)      316 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/static/wagtailvideos/js/video-chooser-telepath.js
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/static/wagtailvideos/js/video-chooser.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.575485 wagtailvideos-4.2.1/wagtailvideos/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.576485 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.588485 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/chooser/
+-rw-rw-rw-   0 root         (0) root         (0)      926 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/chooser/chooser.html
+-rw-rw-rw-   0 root         (0) root         (0)     1988 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/chooser/results.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.588485 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/homepage/
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/homepage/videos_summary.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.589485 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/multiple/
+-rw-rw-rw-   0 root         (0) root         (0)     4414 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/multiple/add.html
+-rw-rw-rw-   0 root         (0) root         (0)     1042 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/multiple/edit_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.576485 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/permissions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.589485 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/permissions/includes/
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/permissions/includes/video_permissions_formset.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.590485 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/_file_field.html
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/_file_field_as_li.html
+-rw-rw-rw-   0 root         (0) root         (0)     1222 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/add.html
+-rw-rw-rw-   0 root         (0) root         (0)      820 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/confirm_delete.html
+-rw-rw-rw-   0 root         (0) root         (0)     6496 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/edit.html
+-rw-rw-rw-   0 root         (0) root         (0)     1393 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/index.html
+-rw-rw-rw-   0 root         (0) root         (0)     2019 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/results.html
+-rw-rw-rw-   0 root         (0) root         (0)     1903 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/usage.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.590485 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)      442 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/widgets/video_chooser.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.591485 wagtailvideos-4.2.1/wagtailvideos/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/templatetags/wagtailvideos_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      712 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.591485 wagtailvideos-4.2.1/wagtailvideos/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5285 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/views/chooser.py
+-rw-rw-rw-   0 root         (0) root         (0)     4921 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/views/multiple.py
+-rw-rw-rw-   0 root         (0) root         (0)     7923 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/views/videos.py
+-rw-rw-rw-   0 root         (0) root         (0)     4347 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/wagtail_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2085 2023-07-19 00:21:11.000000 wagtailvideos-4.2.1/wagtailvideos/widgets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 00:21:19.584485 wagtailvideos-4.2.1/wagtailvideos.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5529 2023-07-19 00:21:19.000000 wagtailvideos-4.2.1/wagtailvideos.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3225 2023-07-19 00:21:19.000000 wagtailvideos-4.2.1/wagtailvideos.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:21:19.000000 wagtailvideos-4.2.1/wagtailvideos.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 00:21:19.000000 wagtailvideos-4.2.1/wagtailvideos.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-19 00:21:19.000000 wagtailvideos-4.2.1/wagtailvideos.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-19 00:21:19.000000 wagtailvideos-4.2.1/wagtailvideos.egg-info/top_level.txt
```

### Comparing `wagtailvideos-4.2.0/LICENSE` & `wagtailvideos-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/PKG-INFO` & `wagtailvideos-4.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailvideos
-Version: 4.2.0
+Version: 4.2.1
 Summary: A wagtail module for uploading and displaying videos in various codecs.
 Home-page: https://github.com/neon-jungle/wagtailvideos
 Author: Neon Jungle
 Author-email: developers@neonjungle.studio
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `wagtailvideos-4.2.0/README.rst` & `wagtailvideos-4.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/setup.py` & `wagtailvideos-4.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open("README.rst", "r") as f:
     readme = f.read()
 
 from setuptools import find_packages, setup  # noqa: E4
 
 setup(
     name="wagtailvideos",
-    version="4.2.0",
+    version="4.2.1",
     description="A wagtail module for uploading and displaying videos in various codecs.",
     long_description=readme,
     author="Neon Jungle",
     author_email="developers@neonjungle.studio",
     url="https://github.com/neon-jungle/wagtailvideos",
     install_requires=[
         "wagtail>=4.2",
```

### Comparing `wagtailvideos-4.2.0/tests/app/migrations/0001_initial.py` & `wagtailvideos-4.2.1/tests/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/tests/app/models.py` & `wagtailvideos-4.2.1/tests/app/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,45 +11,54 @@
     AbstractVideoTranscode)
 
 
 class CustomVideoModel(AbstractVideo):
     attribution = models.TextField(blank=True)
 
     admin_form_fields = (
-        'title',
-        'attribution',
-        'file',
-        'collection',
-        'thumbnail',
-        'tags',
+        "title",
+        "attribution",
+        "file",
+        "collection",
+        "thumbnail",
+        "tags",
     )
 
 
 class CustomVideoTranscode(AbstractVideoTranscode):
-    video = models.ForeignKey(CustomVideoModel, related_name='transcodes', on_delete=models.CASCADE)
+    video = models.ForeignKey(
+        CustomVideoModel, related_name="transcodes", on_delete=models.CASCADE
+    )
 
     class Meta:
-        unique_together = (
-            ('video', 'media_format')
-        )
+        unique_together = ("video", "media_format")
 
 
 class CustomTrackListing(AbstractTrackListing):
-    video = models.OneToOneField(CustomVideoModel, related_name='track_listing', on_delete=models.CASCADE)
+    video = models.OneToOneField(
+        CustomVideoModel, related_name="track_listing", on_delete=models.CASCADE
+    )
 
 
 class CustomVideoTrack(AbstractVideoTrack):
-    listing = ParentalKey(CustomTrackListing, related_name='tracks', on_delete=models.CASCADE)
+    listing = ParentalKey(
+        CustomTrackListing, related_name="tracks", on_delete=models.CASCADE
+    )
 
 
 class TestPage(Page):
     video_field = models.ForeignKey(
-        CustomVideoModel, related_name='+', null=True, blank=True, on_delete=models.SET_NULL)
+        CustomVideoModel,
+        related_name="+",
+        null=True,
+        blank=True,
+        on_delete=models.SET_NULL,
+    )
 
-    video_streamfield = StreamField([
-        ('video', VideoChooserBlock())
-    ], blank=True)
+    video_streamfield = StreamField(
+        [("video", VideoChooserBlock())], blank=True, use_json_field=True
+    )
 
     content_panels = Page.content_panels + [
-        VideoChooserPanel('video_field'),
-        FieldPanel('video_streamfield'),
+        VideoChooserPanel("video_field"),
+        FieldPanel("video_streamfield"),
     ]
```

### Comparing `wagtailvideos-4.2.0/tests/app/test_block.py` & `wagtailvideos-4.2.1/tests/app/test_block.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/tests/app/urls.py` & `wagtailvideos-4.2.1/tests/app/urls.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/tests/storage.py` & `wagtailvideos-4.2.1/tests/storage.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/tests/test_admin_views.py` & `wagtailvideos-4.2.1/tests/test_admin_views.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/tests/test_custom_model.py` & `wagtailvideos-4.2.1/tests/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/tests/test_template_tag.py` & `wagtailvideos-4.2.1/tests/test_template_tag.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/__init__.py` & `wagtailvideos-4.2.1/wagtailvideos/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/apps.py` & `wagtailvideos-4.2.1/wagtailvideos/apps.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/blocks.py` & `wagtailvideos-4.2.1/wagtailvideos/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/ffmpeg.py` & `wagtailvideos-4.2.1/wagtailvideos/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/fields.py` & `wagtailvideos-4.2.1/wagtailvideos/fields.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/forms.py` & `wagtailvideos-4.2.1/wagtailvideos/forms.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/jinja2tags.py` & `wagtailvideos-4.2.1/wagtailvideos/jinja2tags.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/migrations/0001_initial.py` & `wagtailvideos-4.2.1/wagtailvideos/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/migrations/0002_auto_20160321_1610.py` & `wagtailvideos-4.2.1/wagtailvideos/migrations/0002_auto_20160321_1610.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/migrations/0003_auto_20160705_1646.py` & `wagtailvideos-4.2.1/wagtailvideos/migrations/0003_auto_20160705_1646.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/migrations/0004_auto_20160706_1153.py` & `wagtailvideos-4.2.1/wagtailvideos/migrations/0004_auto_20160706_1153.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/migrations/0006_auto_20160707_1413.py` & `wagtailvideos-4.2.1/wagtailvideos/migrations/0006_auto_20160707_1413.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/migrations/0009_videotranscode_quality.py` & `wagtailvideos-4.2.1/wagtailvideos/migrations/0009_videotranscode_quality.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/migrations/0011_video_tracks.py` & `wagtailvideos-4.2.1/wagtailvideos/migrations/0011_video_tracks.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/migrations/0012_remove_unique_constraint.py` & `wagtailvideos-4.2.1/wagtailvideos/migrations/0012_remove_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/migrations/0013_add_choose_permissions.py` & `wagtailvideos-4.2.1/wagtailvideos/migrations/0013_add_choose_permissions.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/models.py` & `wagtailvideos-4.2.1/wagtailvideos/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -349,33 +349,35 @@
         Video, on_delete=models.CASCADE,
         related_name='track_listing')
 
 
 class AbstractVideoTrack(Orderable):
     # TODO move to TextChoices once django < 3 is dropped
     track_kinds = [
-        ('subtitles', 'Subtitles'),
-        ('captions', 'Captions'),
-        ('descriptions', 'Descriptions'),
-        ('chapters', 'Chapters'),
-        ('metadata', 'Metadata'),
+        ('subtitles', _('Subtitles')),
+        ('captions', _('Captions')),
+        ('descriptions', _('Descriptions')),
+        ('chapters', _('Chapters')),
+        ('metadata', _('Metadata')),
     ]
 
     file = models.FileField(
-        verbose_name=_('file'),
+        verbose_name=_('File'),
         upload_to=get_upload_to
     )
-    kind = models.CharField(max_length=50, choices=track_kinds, default=track_kinds[0][0])
+    kind = models.CharField(max_length=50, choices=track_kinds, default=track_kinds[0][0], verbose_name=_('Kind'))
     label = models.CharField(
         max_length=255, blank=True,
-        help_text='A user-readable title of the text track.')
+        help_text=_('A user-readable title of the text track.'),
+        verbose_name=_('Label'))
     language = models.CharField(
         max_length=50,
         choices=[(v, k) for k, v in bcp47.languages.items()],
-        default='en', blank=True, help_text='Required if type is "Subtitle"')
+        default='en', blank=True, help_text=_('Required if type is "Subtitle"'),
+        verbose_name=_('Language'))
 
     def track_tag(self):
         attrs = {
             'kind': self.kind,
             'src': self.url,
         }
         if self.label:
```

### Comparing `wagtailvideos-4.2.0/wagtailvideos/signals.py` & `wagtailvideos-4.2.1/wagtailvideos/signals.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/static/wagtailvideos/js/add-multiple.js` & `wagtailvideos-4.2.1/wagtailvideos/static/wagtailvideos/js/add-multiple.js`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/chooser/chooser.html` & `wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/chooser/chooser.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/chooser/results.html` & `wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/chooser/results.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/multiple/add.html` & `wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/multiple/add.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/multiple/edit_form.html` & `wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/multiple/edit_form.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/videos/add.html` & `wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/add.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/videos/confirm_delete.html` & `wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/videos/edit.html` & `wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/edit.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/videos/index.html` & `wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/index.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/videos/results.html` & `wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/results.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/templates/wagtailvideos/videos/usage.html` & `wagtailvideos-4.2.1/wagtailvideos/templates/wagtailvideos/videos/usage.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/templatetags/wagtailvideos_tags.py` & `wagtailvideos-4.2.1/wagtailvideos/templatetags/wagtailvideos_tags.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/urls.py` & `wagtailvideos-4.2.1/wagtailvideos/urls.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/views/chooser.py` & `wagtailvideos-4.2.1/wagtailvideos/views/chooser.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/views/multiple.py` & `wagtailvideos-4.2.1/wagtailvideos/views/multiple.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/views/videos.py` & `wagtailvideos-4.2.1/wagtailvideos/views/videos.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos/wagtail_hooks.py` & `wagtailvideos-4.2.1/wagtailvideos/wagtail_hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 Video = get_video_model()
 
 
 class TracksAdmin(ModelAdmin):
     model = Video.get_track_listing_model()
     menu_icon = 'openquote'
-    menu_label = 'Text tracks'
+    menu_label = _('Text tracks')
 
     list_display = ('__str__', 'track_count')
 
     def track_count(self, track_listing):
         return track_listing.tracks.count()
     track_count.short_description = 'No. tracks'
```

### Comparing `wagtailvideos-4.2.0/wagtailvideos/widgets.py` & `wagtailvideos-4.2.1/wagtailvideos/widgets.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-4.2.0/wagtailvideos.egg-info/PKG-INFO` & `wagtailvideos-4.2.1/wagtailvideos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailvideos
-Version: 4.2.0
+Version: 4.2.1
 Summary: A wagtail module for uploading and displaying videos in various codecs.
 Home-page: https://github.com/neon-jungle/wagtailvideos
 Author: Neon Jungle
 Author-email: developers@neonjungle.studio
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `wagtailvideos-4.2.0/wagtailvideos.egg-info/SOURCES.txt` & `wagtailvideos-4.2.1/wagtailvideos.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 tests/utils.py
 tests/app/__init__.py
 tests/app/models.py
 tests/app/settings.py
 tests/app/test_block.py
 tests/app/urls.py
 tests/app/migrations/0001_initial.py
+tests/app/migrations/0002_alter_testpage_video_streamfield.py
 tests/app/migrations/__init__.py
 wagtailvideos/__init__.py
 wagtailvideos/apps.py
 wagtailvideos/blocks.py
 wagtailvideos/edit_handlers.py
 wagtailvideos/ffmpeg.py
 wagtailvideos/fields.py
@@ -45,14 +46,15 @@
 wagtailvideos/migrations/0007_video_duration.py
 wagtailvideos/migrations/0008_auto_20160728_1523.py
 wagtailvideos/migrations/0009_videotranscode_quality.py
 wagtailvideos/migrations/0010_video_ordering.py
 wagtailvideos/migrations/0011_video_tracks.py
 wagtailvideos/migrations/0012_remove_unique_constraint.py
 wagtailvideos/migrations/0013_add_choose_permissions.py
+wagtailvideos/migrations/0014_alter_videotrack_file_alter_videotrack_kind_and_more.py
 wagtailvideos/migrations/__init__.py
 wagtailvideos/static/wagtailvideos/css/edit-video.css
 wagtailvideos/static/wagtailvideos/css/summary-override.css
 wagtailvideos/static/wagtailvideos/js/add-multiple.js
 wagtailvideos/static/wagtailvideos/js/video-chooser-telepath.js
 wagtailvideos/static/wagtailvideos/js/video-chooser.js
 wagtailvideos/templates/wagtailvideos/chooser/chooser.html
```

