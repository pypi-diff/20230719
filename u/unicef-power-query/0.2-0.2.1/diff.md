# Comparing `tmp/unicef-power-query-0.2.tar.gz` & `tmp/unicef-power-query-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicef-power-query-0.2.tar", last modified: Tue Jul 18 09:19:09 2023, max compression
+gzip compressed data, was "unicef-power-query-0.2.1.tar", last modified: Tue Jul 18 14:51:56 2023, max compression
```

## Comparing `unicef-power-query-0.2.tar` & `unicef-power-query-0.2.1.tar`

### file list

```diff
@@ -1,172 +1,191 @@
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.585050 unicef-power-query-0.2/
--rw-r--r--   0 jojo       (501) staff       (20)      142 2023-07-18 09:06:00.000000 unicef-power-query-0.2/CHANGES
--rw-r--r--   0 jojo       (501) staff       (20)      546 2023-05-05 13:28:14.000000 unicef-power-query-0.2/LICENSE
--rwxr-xr-x   0 jojo       (501) staff       (20)      197 2023-05-05 13:23:06.000000 unicef-power-query-0.2/MANIFEST.in
--rw-r--r--   0 jojo       (501) staff       (20)      527 2023-07-18 09:19:09.585274 unicef-power-query-0.2/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)     2190 2023-07-04 08:17:12.000000 unicef-power-query-0.2/README.rst
--rw-r--r--   0 jojo       (501) staff       (20)       82 2023-07-18 09:19:09.586698 unicef-power-query-0.2/setup.cfg
--rwxr-xr-x   0 jojo       (501) staff       (20)     1852 2023-07-04 08:17:12.000000 unicef-power-query-0.2/setup.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.305578 unicef-power-query-0.2/src/
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.330578 unicef-power-query-0.2/src/power_query/
--rw-r--r--   0 jojo       (501) staff       (20)       58 2023-07-18 09:06:00.000000 unicef-power-query-0.2/src/power_query/__init__.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.348126 unicef-power-query-0.2/src/power_query/__pycache__/
--rw-r--r--   0 jojo       (501) staff       (20)      223 2023-07-13 10:19:44.000000 unicef-power-query-0.2/src/power_query/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)    15713 2023-07-13 10:19:49.000000 unicef-power-query-0.2/src/power_query/__pycache__/admin.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      411 2023-07-13 10:19:44.000000 unicef-power-query-0.2/src/power_query/__pycache__/apps.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     3741 2023-07-13 10:19:49.000000 unicef-power-query-0.2/src/power_query/__pycache__/celery_tasks.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     1105 2023-07-13 12:04:32.000000 unicef-power-query-0.2/src/power_query/__pycache__/defaults.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      816 2023-07-13 10:19:47.000000 unicef-power-query-0.2/src/power_query/__pycache__/exceptions.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     6621 2023-07-18 08:50:32.000000 unicef-power-query-0.2/src/power_query/__pycache__/fixtures.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     1494 2023-07-13 10:19:49.000000 unicef-power-query-0.2/src/power_query/__pycache__/forms.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      947 2023-07-13 10:19:47.000000 unicef-power-query-0.2/src/power_query/__pycache__/json.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     1130 2023-07-13 10:19:49.000000 unicef-power-query-0.2/src/power_query/__pycache__/mixin.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)    16511 2023-07-13 10:19:47.000000 unicef-power-query-0.2/src/power_query/__pycache__/models.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      508 2023-07-13 10:20:35.000000 unicef-power-query-0.2/src/power_query/__pycache__/urls.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     5157 2023-07-13 10:19:47.000000 unicef-power-query-0.2/src/power_query/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      840 2023-07-13 10:19:47.000000 unicef-power-query-0.2/src/power_query/__pycache__/validators.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     2800 2023-07-13 10:20:35.000000 unicef-power-query-0.2/src/power_query/__pycache__/views.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     3645 2023-07-13 10:19:49.000000 unicef-power-query-0.2/src/power_query/__pycache__/widget.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)    16001 2023-07-13 09:21:20.000000 unicef-power-query-0.2/src/power_query/admin.py
--rw-r--r--   0 jojo       (501) staff       (20)      119 2023-07-13 07:16:39.000000 unicef-power-query-0.2/src/power_query/apps.py
--rw-r--r--   0 jojo       (501) staff       (20)     3009 2023-07-13 07:25:13.000000 unicef-power-query-0.2/src/power_query/celery_tasks.py
--rw-r--r--   0 jojo       (501) staff       (20)     1051 2023-07-13 07:22:15.000000 unicef-power-query-0.2/src/power_query/defaults.py
--rw-r--r--   0 jojo       (501) staff       (20)      404 2023-07-13 07:14:46.000000 unicef-power-query-0.2/src/power_query/exceptions.py
--rw-r--r--   0 jojo       (501) staff       (20)     4351 2023-07-18 09:06:00.000000 unicef-power-query-0.2/src/power_query/fixtures.py
--rw-r--r--   0 jojo       (501) staff       (20)     1438 2023-07-13 07:24:44.000000 unicef-power-query-0.2/src/power_query/forms.py
--rw-r--r--   0 jojo       (501) staff       (20)      572 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/json.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.348854 unicef-power-query-0.2/src/power_query/management/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/management/__init__.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.349710 unicef-power-query-0.2/src/power_query/management/__pycache__/
--rw-r--r--   0 jojo       (501) staff       (20)      170 2023-07-17 14:18:07.000000 unicef-power-query-0.2/src/power_query/management/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.351107 unicef-power-query-0.2/src/power_query/management/commands/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/management/commands/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)     3595 2023-07-13 07:17:04.000000 unicef-power-query-0.2/src/power_query/management/commands/pq.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.352866 unicef-power-query-0.2/src/power_query/migrations/
--rw-r--r--   0 jojo       (501) staff       (20)    15211 2023-07-18 09:06:00.000000 unicef-power-query-0.2/src/power_query/migrations/0001_migration_squashed_0014_migration.py
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/migrations/__init__.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.354160 unicef-power-query-0.2/src/power_query/migrations/__pycache__/
--rw-r--r--   0 jojo       (501) staff       (20)     5436 2023-07-17 14:18:08.000000 unicef-power-query-0.2/src/power_query/migrations/__pycache__/0001_migration_squashed_0014_migration.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      170 2023-07-17 14:18:08.000000 unicef-power-query-0.2/src/power_query/migrations/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      753 2023-07-13 07:18:11.000000 unicef-power-query-0.2/src/power_query/mixin.py
--rw-r--r--   0 jojo       (501) staff       (20)    17115 2023-07-13 07:27:46.000000 unicef-power-query-0.2/src/power_query/models.py
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/notify.py
--rw-r--r--   0 jojo       (501) staff       (20)       91 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/signals.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.361728 unicef-power-query-0.2/src/power_query/static/
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.301923 unicef-power-query-0.2/src/power_query/static/admin/
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.373095 unicef-power-query-0.2/src/power_query/static/admin/power_query/
--rw-r--r--   0 jojo       (501) staff       (20)     3628 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/code.css
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.408072 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/
--rw-r--r--   0 jojo       (501) staff       (20)     1969 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/abcdef.css
--rw-r--r--   0 jojo       (501) staff       (20)     2507 2023-05-08 13:33:06.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/active-line.js
--rw-r--r--   0 jojo       (501) staff       (20)     8706 2023-05-08 13:33:06.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/codemirror.css
--rw-r--r--   0 jojo       (501) staff       (20)   400161 2023-05-08 13:33:06.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/codemirror.js
--rw-r--r--   0 jojo       (501) staff       (20)    11792 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/django.js
--rw-r--r--   0 jojo       (501) staff       (20)     4983 2023-05-08 13:33:06.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/foldcode.js
--rw-r--r--   0 jojo       (501) staff       (20)      435 2023-05-08 13:33:06.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/foldgutter.css
--rw-r--r--   0 jojo       (501) staff       (20)     5368 2023-05-08 13:33:06.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/foldgutter.js
--rw-r--r--   0 jojo       (501) staff       (20)      118 2023-05-08 13:33:06.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/fullscreen.css
--rw-r--r--   0 jojo       (501) staff       (20)     1495 2023-05-08 13:33:06.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/fullscreen.js
--rw-r--r--   0 jojo       (501) staff       (20)     1674 2023-05-08 13:33:06.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/indent-fold.js
--rw-r--r--   0 jojo       (501) staff       (20)     6816 2023-05-08 13:33:06.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/matchbrackets.js
--rw-r--r--   0 jojo       (501) staff       (20)     1856 2023-05-08 13:33:06.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/midnight.css
--rw-r--r--   0 jojo       (501) staff       (20)     3241 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/overlay.js
--rw-r--r--   0 jojo       (501) staff       (20)    14924 2023-05-08 13:33:06.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/python.js
--rw-r--r--   0 jojo       (501) staff       (20)    13351 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/xml.js
--rw-r--r--   0 jojo       (501) staff       (20)     3733 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/yaml.js
--rw-r--r--   0 jojo       (501) staff       (20)     5122 2023-07-04 08:17:12.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/colorful.css
--rw-r--r--   0 jojo       (501) staff       (20)      760 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/diff.css
--rw-r--r--   0 jojo       (501) staff       (20)    16556 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/editor.png
--rw-r--r--   0 jojo       (501) staff       (20)      292 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/power_query.css
--rw-r--r--   0 jojo       (501) staff       (20)      204 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/power_query.css.map
--rw-r--r--   0 jojo       (501) staff       (20)      355 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/power_query.scss
--rw-r--r--   0 jojo       (501) staff       (20)     6742 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/redo.png
--rw-r--r--   0 jojo       (501) staff       (20)     6554 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/undo.png
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.304344 unicef-power-query-0.2/src/power_query/templates/
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.302728 unicef-power-query-0.2/src/power_query/templates/admin/
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.304049 unicef-power-query-0.2/src/power_query/templates/admin/power_query/
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.414609 unicef-power-query-0.2/src/power_query/templates/admin/power_query/dataset/
--rw-r--r--   0 jojo       (501) staff       (20)      109 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/dataset/change_form.html
--rw-r--r--   0 jojo       (501) staff       (20)      366 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/dataset/export.html
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.417010 unicef-power-query-0.2/src/power_query/templates/admin/power_query/formatter/
--rw-r--r--   0 jojo       (501) staff       (20)     2750 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/formatter/change_form.html
--rw-r--r--   0 jojo       (501) staff       (20)      360 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/formatter/change_list.html
--rw-r--r--   0 jojo       (501) staff       (20)      489 2023-07-13 07:30:38.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/formatter/test.html
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.420961 unicef-power-query-0.2/src/power_query/templates/admin/power_query/query/
--rw-r--r--   0 jojo       (501) staff       (20)      407 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/query/change_form.html
--rw-r--r--   0 jojo       (501) staff       (20)      366 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/query/export.html
--rw-r--r--   0 jojo       (501) staff       (20)      822 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/query/monitor.html
--rw-r--r--   0 jojo       (501) staff       (20)     2003 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/query/preview.html
--rw-r--r--   0 jojo       (501) staff       (20)      490 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/query/run_result.html
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.423621 unicef-power-query-0.2/src/power_query/templates/admin/power_query/queryargs/
--rw-r--r--   0 jojo       (501) staff       (20)     1559 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/queryargs/change_form.html
--rw-r--r--   0 jojo       (501) staff       (20)      479 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/queryargs/preview.html
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.424819 unicef-power-query-0.2/src/power_query/templates/admin/power_query/report/
--rw-r--r--   0 jojo       (501) staff       (20)      360 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/report/change_list.html
--rw-r--r--   0 jojo       (501) staff       (20)      743 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/report/monitor.html
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.427212 unicef-power-query-0.2/src/power_query/templates/power_query/
--rw-r--r--   0 jojo       (501) staff       (20)      532 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/power_query/base.html
--rw-r--r--   0 jojo       (501) staff       (20)      762 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/power_query/detail.html
--rw-r--r--   0 jojo       (501) staff       (20)      339 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/power_query/list.html
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.433090 unicef-power-query-0.2/src/power_query/templates/power_query/widgets/
--rw-r--r--   0 jojo       (501) staff       (20)     1235 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/power_query/widgets/codewidget.html
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.440788 unicef-power-query-0.2/src/power_query/templatetags/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templatetags/__init__.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.467201 unicef-power-query-0.2/src/power_query/templatetags/__pycache__/
--rw-r--r--   0 jojo       (501) staff       (20)      172 2023-07-13 10:20:43.000000 unicef-power-query-0.2/src/power_query/templatetags/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     1295 2023-07-13 10:20:43.000000 unicef-power-query-0.2/src/power_query/templatetags/__pycache__/power_query.cpython-39.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      814 2023-07-13 07:18:11.000000 unicef-power-query-0.2/src/power_query/templatetags/power_query.py
--rw-r--r--   0 jojo       (501) staff       (20)      368 2023-07-13 07:19:25.000000 unicef-power-query-0.2/src/power_query/urls.py
--rw-r--r--   0 jojo       (501) staff       (20)     5041 2023-07-13 07:19:03.000000 unicef-power-query-0.2/src/power_query/utils.py
--rw-r--r--   0 jojo       (501) staff       (20)      453 2023-07-13 07:17:09.000000 unicef-power-query-0.2/src/power_query/validators.py
--rw-r--r--   0 jojo       (501) staff       (20)     3360 2023-07-13 09:21:39.000000 unicef-power-query-0.2/src/power_query/views.py
--rw-r--r--   0 jojo       (501) staff       (20)     3111 2023-07-13 07:15:15.000000 unicef-power-query-0.2/src/power_query/widget.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.521110 unicef-power-query-0.2/src/unicef_power_query.egg-info/
--rw-r--r--   0 jojo       (501) staff       (20)      527 2023-07-18 09:19:09.000000 unicef-power-query-0.2/src/unicef_power_query.egg-info/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)     6379 2023-07-18 09:19:09.000000 unicef-power-query-0.2/src/unicef_power_query.egg-info/SOURCES.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-07-18 09:19:09.000000 unicef-power-query-0.2/src/unicef_power_query.egg-info/dependency_links.txt
--rw-r--r--   0 jojo       (501) staff       (20)      319 2023-07-18 09:19:09.000000 unicef-power-query-0.2/src/unicef_power_query.egg-info/requires.txt
--rw-r--r--   0 jojo       (501) staff       (20)       12 2023-07-18 09:19:09.000000 unicef-power-query-0.2/src/unicef_power_query.egg-info/top_level.txt
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.535034 unicef-power-query-0.2/tests/
--rw-r--r--   0 jojo       (501) staff       (20)      214 2023-05-16 13:30:33.000000 unicef-power-query-0.2/tests/.coveragerc
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.2/tests/__init__.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.548127 unicef-power-query-0.2/tests/__pycache__/
--rw-r--r--   0 jojo       (501) staff       (20)    36910 2023-06-12 09:22:39.000000 unicef-power-query-0.2/tests/__pycache__/test_admin.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     3607 2023-06-12 07:29:10.000000 unicef-power-query-0.2/tests/__pycache__/test_auth.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     7475 2023-06-12 07:29:10.000000 unicef-power-query-0.2/tests/__pycache__/test_celery.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     1408 2023-06-12 07:29:10.000000 unicef-power-query-0.2/tests/__pycache__/test_params.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     4525 2023-06-12 07:29:10.000000 unicef-power-query-0.2/tests/__pycache__/test_queries.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     1502 2023-06-12 07:29:10.000000 unicef-power-query-0.2/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 jojo       (501) staff       (20)    11905 2023-05-16 12:47:07.000000 unicef-power-query-0.2/tests/__pycache__/test_views.cpython-311-pytest-7.3.1.pyc
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.560290 unicef-power-query-0.2/tests/demoproject/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-06-02 15:31:56.000000 unicef-power-query-0.2/tests/demoproject/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)   278528 2023-05-31 15:10:33.000000 unicef-power-query-0.2/tests/demoproject/db.sqlite3
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.575539 unicef-power-query-0.2/tests/demoproject/demo/
--rw-r--r--   0 jojo       (501) staff       (20)       65 2023-07-04 08:17:12.000000 unicef-power-query-0.2/tests/demoproject/demo/__init__.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.580677 unicef-power-query-0.2/tests/demoproject/demo/__pycache__/
--rw-r--r--   0 jojo       (501) staff       (20)      267 2023-06-12 07:26:20.000000 unicef-power-query-0.2/tests/demoproject/demo/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      691 2023-06-12 07:26:20.000000 unicef-power-query-0.2/tests/demoproject/demo/__pycache__/celery.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      738 2023-05-16 12:44:40.000000 unicef-power-query-0.2/tests/demoproject/demo/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     2690 2023-06-12 07:26:20.000000 unicef-power-query-0.2/tests/demoproject/demo/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      525 2023-05-31 11:57:14.000000 unicef-power-query-0.2/tests/demoproject/demo/__pycache__/urls.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      699 2023-05-16 13:01:06.000000 unicef-power-query-0.2/tests/demoproject/demo/__pycache__/wsgi.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      245 2023-07-04 08:17:12.000000 unicef-power-query-0.2/tests/demoproject/demo/celery.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.582694 unicef-power-query-0.2/tests/demoproject/demo/migrations/
--rw-r--r--   0 jojo       (501) staff       (20)     5140 2023-05-05 13:23:06.000000 unicef-power-query-0.2/tests/demoproject/demo/migrations/0001_initial.py
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-power-query-0.2/tests/demoproject/demo/migrations/__init__.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.584208 unicef-power-query-0.2/tests/demoproject/demo/migrations/__pycache__/
--rw-r--r--   0 jojo       (501) staff       (20)     3923 2023-05-16 13:01:06.000000 unicef-power-query-0.2/tests/demoproject/demo/migrations/__pycache__/0001_initial.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      195 2023-05-16 13:01:06.000000 unicef-power-query-0.2/tests/demoproject/demo/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      142 2023-05-16 12:43:15.000000 unicef-power-query-0.2/tests/demoproject/demo/models.py
--rw-r--r--   0 jojo       (501) staff       (20)     2590 2023-07-04 08:17:12.000000 unicef-power-query-0.2/tests/demoproject/demo/settings.py
--rw-r--r--   0 jojo       (501) staff       (20)      194 2023-05-16 14:04:29.000000 unicef-power-query-0.2/tests/demoproject/demo/urls.py
--rw-r--r--   0 jojo       (501) staff       (20)      385 2023-05-05 13:23:06.000000 unicef-power-query-0.2/tests/demoproject/demo/wsgi.py
--rw-r--r--   0 jojo       (501) staff       (20)      475 2023-05-05 13:23:06.000000 unicef-power-query-0.2/tests/demoproject/factories.py
--rwxr-xr-x   0 jojo       (501) staff       (20)      246 2023-07-04 08:17:12.000000 unicef-power-query-0.2/tests/demoproject/manage.py
--rw-r--r--   0 jojo       (501) staff       (20)    10380 2023-07-18 09:06:00.000000 unicef-power-query-0.2/tests/test_admin.py
--rw-r--r--   0 jojo       (501) staff       (20)     1719 2023-07-18 09:06:00.000000 unicef-power-query-0.2/tests/test_auth.py
--rw-r--r--   0 jojo       (501) staff       (20)     2097 2023-07-18 09:06:00.000000 unicef-power-query-0.2/tests/test_celery.py
--rw-r--r--   0 jojo       (501) staff       (20)      441 2023-07-18 09:06:00.000000 unicef-power-query-0.2/tests/test_params.py
--rw-r--r--   0 jojo       (501) staff       (20)     1989 2023-07-18 09:06:00.000000 unicef-power-query-0.2/tests/test_queries.py
--rw-r--r--   0 jojo       (501) staff       (20)      829 2023-07-13 09:09:33.000000 unicef-power-query-0.2/tests/test_utils.py
--rw-r--r--   0 jojo       (501) staff       (20)     1772 2023-07-18 09:06:00.000000 unicef-power-query-0.2/tests/test_views.py
--rw-r--r--   0 jojo       (501) staff       (20)     1022 2023-07-04 08:17:12.000000 unicef-power-query-0.2/tox.ini
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:56.036458 unicef-power-query-0.2.1/
+-rw-r--r--   0 jojo       (501) staff       (20)      214 2023-07-18 14:51:26.000000 unicef-power-query-0.2.1/CHANGES
+-rw-r--r--   0 jojo       (501) staff       (20)      546 2023-05-05 13:28:14.000000 unicef-power-query-0.2.1/LICENSE
+-rwxr-xr-x   0 jojo       (501) staff       (20)      197 2023-05-05 13:23:06.000000 unicef-power-query-0.2.1/MANIFEST.in
+-rw-r--r--   0 jojo       (501) staff       (20)      529 2023-07-18 14:51:56.036781 unicef-power-query-0.2.1/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)     2190 2023-07-04 08:17:12.000000 unicef-power-query-0.2.1/README.rst
+-rw-r--r--   0 jojo       (501) staff       (20)       82 2023-07-18 14:51:56.043114 unicef-power-query-0.2.1/setup.cfg
+-rwxr-xr-x   0 jojo       (501) staff       (20)     1852 2023-07-04 08:17:12.000000 unicef-power-query-0.2.1/setup.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.617365 unicef-power-query-0.2.1/src/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.680663 unicef-power-query-0.2.1/src/power_query/
+-rw-r--r--   0 jojo       (501) staff       (20)       60 2023-07-18 14:51:26.000000 unicef-power-query-0.2.1/src/power_query/__init__.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.717682 unicef-power-query-0.2.1/src/power_query/__pycache__/
+-rw-r--r--   0 jojo       (501) staff       (20)      248 2023-07-18 14:47:17.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      223 2023-07-18 09:30:04.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)    27954 2023-07-18 14:47:18.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)    15713 2023-07-13 10:19:49.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/admin.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      522 2023-07-18 14:47:17.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      411 2023-07-13 10:19:44.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/apps.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     6185 2023-07-18 14:47:18.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/celery_tasks.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     3741 2023-07-13 10:19:49.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/celery_tasks.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     1105 2023-07-13 12:04:32.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/defaults.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     1161 2023-07-18 14:47:17.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      816 2023-07-13 10:19:47.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/exceptions.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     6621 2023-07-18 09:30:08.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/fixtures.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     2347 2023-07-18 14:47:18.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/forms.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     1494 2023-07-13 10:19:49.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/forms.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     1519 2023-07-18 14:47:17.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/json.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      947 2023-07-13 10:19:47.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/json.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     1130 2023-07-13 10:19:49.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/mixin.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)    29741 2023-07-18 14:47:17.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)    16511 2023-07-13 10:19:47.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      713 2023-07-18 14:47:18.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/urls.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      508 2023-07-13 10:20:35.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/urls.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     9981 2023-07-18 14:47:17.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     5157 2023-07-13 10:19:47.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     1213 2023-07-18 14:47:17.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/validators.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      840 2023-07-13 10:19:47.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/validators.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     5028 2023-07-18 14:47:18.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/views.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     2800 2023-07-13 10:20:35.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/views.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     5600 2023-07-18 14:47:18.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/widget.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     3645 2023-07-13 10:19:49.000000 unicef-power-query-0.2.1/src/power_query/__pycache__/widget.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)    16001 2023-07-13 09:21:20.000000 unicef-power-query-0.2.1/src/power_query/admin.py
+-rw-r--r--   0 jojo       (501) staff       (20)      119 2023-07-13 07:16:39.000000 unicef-power-query-0.2.1/src/power_query/apps.py
+-rw-r--r--   0 jojo       (501) staff       (20)     3009 2023-07-13 07:25:13.000000 unicef-power-query-0.2.1/src/power_query/celery_tasks.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1051 2023-07-13 07:22:15.000000 unicef-power-query-0.2.1/src/power_query/defaults.py
+-rw-r--r--   0 jojo       (501) staff       (20)      404 2023-07-13 07:14:46.000000 unicef-power-query-0.2.1/src/power_query/exceptions.py
+-rw-r--r--   0 jojo       (501) staff       (20)     4351 2023-07-18 09:06:00.000000 unicef-power-query-0.2.1/src/power_query/fixtures.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1438 2023-07-13 07:24:44.000000 unicef-power-query-0.2.1/src/power_query/forms.py
+-rw-r--r--   0 jojo       (501) staff       (20)      572 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/json.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.718784 unicef-power-query-0.2.1/src/power_query/management/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/management/__init__.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.719159 unicef-power-query-0.2.1/src/power_query/management/__pycache__/
+-rw-r--r--   0 jojo       (501) staff       (20)      170 2023-07-17 14:18:07.000000 unicef-power-query-0.2.1/src/power_query/management/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.720427 unicef-power-query-0.2.1/src/power_query/management/commands/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/management/commands/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)     3595 2023-07-13 07:17:04.000000 unicef-power-query-0.2.1/src/power_query/management/commands/pq.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.722999 unicef-power-query-0.2.1/src/power_query/migrations/
+-rw-r--r--   0 jojo       (501) staff       (20)    15211 2023-07-18 09:06:00.000000 unicef-power-query-0.2.1/src/power_query/migrations/0001_migration_squashed_0014_migration.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1003 2023-07-18 14:51:26.000000 unicef-power-query-0.2.1/src/power_query/migrations/0015_alter_dataset_description_and_more.py
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/migrations/__init__.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.730604 unicef-power-query-0.2.1/src/power_query/migrations/__pycache__/
+-rw-r--r--   0 jojo       (501) staff       (20)    10802 2023-07-18 14:47:18.000000 unicef-power-query-0.2.1/src/power_query/migrations/__pycache__/0001_migration_squashed_0014_migration.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     5436 2023-07-18 09:30:10.000000 unicef-power-query-0.2.1/src/power_query/migrations/__pycache__/0001_migration_squashed_0014_migration.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      923 2023-07-18 14:48:37.000000 unicef-power-query-0.2.1/src/power_query/migrations/__pycache__/0015_alter_dataset_description_and_more.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      188 2023-07-18 14:47:18.000000 unicef-power-query-0.2.1/src/power_query/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      170 2023-07-17 14:18:08.000000 unicef-power-query-0.2.1/src/power_query/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      753 2023-07-13 07:18:11.000000 unicef-power-query-0.2.1/src/power_query/mixin.py
+-rw-r--r--   0 jojo       (501) staff       (20)    17115 2023-07-13 07:27:46.000000 unicef-power-query-0.2.1/src/power_query/models.py
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/notify.py
+-rw-r--r--   0 jojo       (501) staff       (20)       91 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/signals.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.735870 unicef-power-query-0.2.1/src/power_query/static/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.609371 unicef-power-query-0.2.1/src/power_query/static/admin/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.740199 unicef-power-query-0.2.1/src/power_query/static/admin/power_query/
+-rw-r--r--   0 jojo       (501) staff       (20)     3628 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/static/admin/power_query/code.css
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.764378 unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/
+-rw-r--r--   0 jojo       (501) staff       (20)     1969 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/abcdef.css
+-rw-r--r--   0 jojo       (501) staff       (20)     2507 2023-05-08 13:33:06.000000 unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/active-line.js
+-rw-r--r--   0 jojo       (501) staff       (20)     8706 2023-05-08 13:33:06.000000 unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/codemirror.css
+-rw-r--r--   0 jojo       (501) staff       (20)   400161 2023-05-08 13:33:06.000000 unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/codemirror.js
+-rw-r--r--   0 jojo       (501) staff       (20)    11792 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/django.js
+-rw-r--r--   0 jojo       (501) staff       (20)     4983 2023-05-08 13:33:06.000000 unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/foldcode.js
+-rw-r--r--   0 jojo       (501) staff       (20)      435 2023-05-08 13:33:06.000000 unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/foldgutter.css
+-rw-r--r--   0 jojo       (501) staff       (20)     5368 2023-05-08 13:33:06.000000 unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/foldgutter.js
+-rw-r--r--   0 jojo       (501) staff       (20)      118 2023-05-08 13:33:06.000000 unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/fullscreen.css
+-rw-r--r--   0 jojo       (501) staff       (20)     1495 2023-05-08 13:33:06.000000 unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/fullscreen.js
+-rw-r--r--   0 jojo       (501) staff       (20)     1674 2023-05-08 13:33:06.000000 unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/indent-fold.js
+-rw-r--r--   0 jojo       (501) staff       (20)     6816 2023-05-08 13:33:06.000000 unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/matchbrackets.js
+-rw-r--r--   0 jojo       (501) staff       (20)     1856 2023-05-08 13:33:06.000000 unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/midnight.css
+-rw-r--r--   0 jojo       (501) staff       (20)     3241 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/overlay.js
+-rw-r--r--   0 jojo       (501) staff       (20)    14924 2023-05-08 13:33:06.000000 unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/python.js
+-rw-r--r--   0 jojo       (501) staff       (20)    13351 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/xml.js
+-rw-r--r--   0 jojo       (501) staff       (20)     3733 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/yaml.js
+-rw-r--r--   0 jojo       (501) staff       (20)     5122 2023-07-04 08:17:12.000000 unicef-power-query-0.2.1/src/power_query/static/admin/power_query/colorful.css
+-rw-r--r--   0 jojo       (501) staff       (20)      760 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/static/admin/power_query/diff.css
+-rw-r--r--   0 jojo       (501) staff       (20)    16556 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/static/admin/power_query/editor.png
+-rw-r--r--   0 jojo       (501) staff       (20)      292 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/static/power_query.css
+-rw-r--r--   0 jojo       (501) staff       (20)      204 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/static/power_query.css.map
+-rw-r--r--   0 jojo       (501) staff       (20)      355 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/static/power_query.scss
+-rw-r--r--   0 jojo       (501) staff       (20)     6742 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/static/redo.png
+-rw-r--r--   0 jojo       (501) staff       (20)     6554 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/static/undo.png
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.615231 unicef-power-query-0.2.1/src/power_query/templates/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.610784 unicef-power-query-0.2.1/src/power_query/templates/admin/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.614931 unicef-power-query-0.2.1/src/power_query/templates/admin/power_query/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.766096 unicef-power-query-0.2.1/src/power_query/templates/admin/power_query/dataset/
+-rw-r--r--   0 jojo       (501) staff       (20)      109 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/templates/admin/power_query/dataset/change_form.html
+-rw-r--r--   0 jojo       (501) staff       (20)      366 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/templates/admin/power_query/dataset/export.html
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.768974 unicef-power-query-0.2.1/src/power_query/templates/admin/power_query/formatter/
+-rw-r--r--   0 jojo       (501) staff       (20)     2750 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/templates/admin/power_query/formatter/change_form.html
+-rw-r--r--   0 jojo       (501) staff       (20)      360 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/templates/admin/power_query/formatter/change_list.html
+-rw-r--r--   0 jojo       (501) staff       (20)      489 2023-07-13 07:30:38.000000 unicef-power-query-0.2.1/src/power_query/templates/admin/power_query/formatter/test.html
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.778825 unicef-power-query-0.2.1/src/power_query/templates/admin/power_query/query/
+-rw-r--r--   0 jojo       (501) staff       (20)      407 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/templates/admin/power_query/query/change_form.html
+-rw-r--r--   0 jojo       (501) staff       (20)      366 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/templates/admin/power_query/query/export.html
+-rw-r--r--   0 jojo       (501) staff       (20)      822 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/templates/admin/power_query/query/monitor.html
+-rw-r--r--   0 jojo       (501) staff       (20)     2003 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/templates/admin/power_query/query/preview.html
+-rw-r--r--   0 jojo       (501) staff       (20)      490 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/templates/admin/power_query/query/run_result.html
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.780004 unicef-power-query-0.2.1/src/power_query/templates/admin/power_query/queryargs/
+-rw-r--r--   0 jojo       (501) staff       (20)     1559 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/templates/admin/power_query/queryargs/change_form.html
+-rw-r--r--   0 jojo       (501) staff       (20)      479 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/templates/admin/power_query/queryargs/preview.html
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.786785 unicef-power-query-0.2.1/src/power_query/templates/admin/power_query/report/
+-rw-r--r--   0 jojo       (501) staff       (20)      360 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/templates/admin/power_query/report/change_list.html
+-rw-r--r--   0 jojo       (501) staff       (20)      743 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/templates/admin/power_query/report/monitor.html
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.791687 unicef-power-query-0.2.1/src/power_query/templates/power_query/
+-rw-r--r--   0 jojo       (501) staff       (20)      532 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/templates/power_query/base.html
+-rw-r--r--   0 jojo       (501) staff       (20)      762 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/templates/power_query/detail.html
+-rw-r--r--   0 jojo       (501) staff       (20)      339 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/templates/power_query/list.html
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.792627 unicef-power-query-0.2.1/src/power_query/templates/power_query/widgets/
+-rw-r--r--   0 jojo       (501) staff       (20)     1235 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/templates/power_query/widgets/codewidget.html
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.794274 unicef-power-query-0.2.1/src/power_query/templatetags/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/src/power_query/templatetags/__init__.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.808795 unicef-power-query-0.2.1/src/power_query/templatetags/__pycache__/
+-rw-r--r--   0 jojo       (501) staff       (20)      190 2023-07-18 14:47:18.000000 unicef-power-query-0.2.1/src/power_query/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      172 2023-07-13 10:20:43.000000 unicef-power-query-0.2.1/src/power_query/templatetags/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     2150 2023-07-18 14:47:18.000000 unicef-power-query-0.2.1/src/power_query/templatetags/__pycache__/power_query.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     1295 2023-07-13 10:20:43.000000 unicef-power-query-0.2.1/src/power_query/templatetags/__pycache__/power_query.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      814 2023-07-13 07:18:11.000000 unicef-power-query-0.2.1/src/power_query/templatetags/power_query.py
+-rw-r--r--   0 jojo       (501) staff       (20)      368 2023-07-13 07:19:25.000000 unicef-power-query-0.2.1/src/power_query/urls.py
+-rw-r--r--   0 jojo       (501) staff       (20)     5041 2023-07-13 07:19:03.000000 unicef-power-query-0.2.1/src/power_query/utils.py
+-rw-r--r--   0 jojo       (501) staff       (20)      453 2023-07-13 07:17:09.000000 unicef-power-query-0.2.1/src/power_query/validators.py
+-rw-r--r--   0 jojo       (501) staff       (20)     3360 2023-07-13 09:21:39.000000 unicef-power-query-0.2.1/src/power_query/views.py
+-rw-r--r--   0 jojo       (501) staff       (20)     3111 2023-07-13 07:15:15.000000 unicef-power-query-0.2.1/src/power_query/widget.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.847737 unicef-power-query-0.2.1/src/unicef_power_query.egg-info/
+-rw-r--r--   0 jojo       (501) staff       (20)      529 2023-07-18 14:51:55.000000 unicef-power-query-0.2.1/src/unicef_power_query.egg-info/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)     7505 2023-07-18 14:51:55.000000 unicef-power-query-0.2.1/src/unicef_power_query.egg-info/SOURCES.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-07-18 14:51:55.000000 unicef-power-query-0.2.1/src/unicef_power_query.egg-info/dependency_links.txt
+-rw-r--r--   0 jojo       (501) staff       (20)      319 2023-07-18 14:51:55.000000 unicef-power-query-0.2.1/src/unicef_power_query.egg-info/requires.txt
+-rw-r--r--   0 jojo       (501) staff       (20)       12 2023-07-18 14:51:55.000000 unicef-power-query-0.2.1/src/unicef_power_query.egg-info/top_level.txt
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.873765 unicef-power-query-0.2.1/tests/
+-rw-r--r--   0 jojo       (501) staff       (20)      214 2023-05-16 13:30:33.000000 unicef-power-query-0.2.1/tests/.coveragerc
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.2.1/tests/__init__.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.883138 unicef-power-query-0.2.1/tests/__pycache__/
+-rw-r--r--   0 jojo       (501) staff       (20)    36910 2023-06-12 09:22:39.000000 unicef-power-query-0.2.1/tests/__pycache__/test_admin.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     3607 2023-06-12 07:29:10.000000 unicef-power-query-0.2.1/tests/__pycache__/test_auth.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     7475 2023-06-12 07:29:10.000000 unicef-power-query-0.2.1/tests/__pycache__/test_celery.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     1408 2023-06-12 07:29:10.000000 unicef-power-query-0.2.1/tests/__pycache__/test_params.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     4525 2023-06-12 07:29:10.000000 unicef-power-query-0.2.1/tests/__pycache__/test_queries.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     1502 2023-06-12 07:29:10.000000 unicef-power-query-0.2.1/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)    11905 2023-05-16 12:47:07.000000 unicef-power-query-0.2.1/tests/__pycache__/test_views.cpython-311-pytest-7.3.1.pyc
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.899242 unicef-power-query-0.2.1/tests/demoproject/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-06-02 15:31:56.000000 unicef-power-query-0.2.1/tests/demoproject/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)   278528 2023-05-31 15:10:33.000000 unicef-power-query-0.2.1/tests/demoproject/db.sqlite3
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:55.998886 unicef-power-query-0.2.1/tests/demoproject/demo/
+-rw-r--r--   0 jojo       (501) staff       (20)       65 2023-07-04 08:17:12.000000 unicef-power-query-0.2.1/tests/demoproject/demo/__init__.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:56.029611 unicef-power-query-0.2.1/tests/demoproject/demo/__pycache__/
+-rw-r--r--   0 jojo       (501) staff       (20)      267 2023-07-18 14:47:16.000000 unicef-power-query-0.2.1/tests/demoproject/demo/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      691 2023-07-18 14:47:16.000000 unicef-power-query-0.2.1/tests/demoproject/demo/__pycache__/celery.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      738 2023-05-16 12:44:40.000000 unicef-power-query-0.2.1/tests/demoproject/demo/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     2690 2023-07-18 14:47:16.000000 unicef-power-query-0.2.1/tests/demoproject/demo/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      525 2023-05-31 11:57:14.000000 unicef-power-query-0.2.1/tests/demoproject/demo/__pycache__/urls.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      699 2023-05-16 13:01:06.000000 unicef-power-query-0.2.1/tests/demoproject/demo/__pycache__/wsgi.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      245 2023-07-04 08:17:12.000000 unicef-power-query-0.2.1/tests/demoproject/demo/celery.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:56.033094 unicef-power-query-0.2.1/tests/demoproject/demo/migrations/
+-rw-r--r--   0 jojo       (501) staff       (20)     5140 2023-05-05 13:23:06.000000 unicef-power-query-0.2.1/tests/demoproject/demo/migrations/0001_initial.py
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-power-query-0.2.1/tests/demoproject/demo/migrations/__init__.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 14:51:56.035064 unicef-power-query-0.2.1/tests/demoproject/demo/migrations/__pycache__/
+-rw-r--r--   0 jojo       (501) staff       (20)     3923 2023-05-16 13:01:06.000000 unicef-power-query-0.2.1/tests/demoproject/demo/migrations/__pycache__/0001_initial.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      195 2023-05-16 13:01:06.000000 unicef-power-query-0.2.1/tests/demoproject/demo/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      142 2023-05-16 12:43:15.000000 unicef-power-query-0.2.1/tests/demoproject/demo/models.py
+-rw-r--r--   0 jojo       (501) staff       (20)     2590 2023-07-04 08:17:12.000000 unicef-power-query-0.2.1/tests/demoproject/demo/settings.py
+-rw-r--r--   0 jojo       (501) staff       (20)      194 2023-05-16 14:04:29.000000 unicef-power-query-0.2.1/tests/demoproject/demo/urls.py
+-rw-r--r--   0 jojo       (501) staff       (20)      385 2023-05-05 13:23:06.000000 unicef-power-query-0.2.1/tests/demoproject/demo/wsgi.py
+-rw-r--r--   0 jojo       (501) staff       (20)      475 2023-05-05 13:23:06.000000 unicef-power-query-0.2.1/tests/demoproject/factories.py
+-rwxr-xr-x   0 jojo       (501) staff       (20)      246 2023-07-04 08:17:12.000000 unicef-power-query-0.2.1/tests/demoproject/manage.py
+-rw-r--r--   0 jojo       (501) staff       (20)    10380 2023-07-18 09:06:00.000000 unicef-power-query-0.2.1/tests/test_admin.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1719 2023-07-18 09:06:00.000000 unicef-power-query-0.2.1/tests/test_auth.py
+-rw-r--r--   0 jojo       (501) staff       (20)     2097 2023-07-18 09:06:00.000000 unicef-power-query-0.2.1/tests/test_celery.py
+-rw-r--r--   0 jojo       (501) staff       (20)      441 2023-07-18 09:06:00.000000 unicef-power-query-0.2.1/tests/test_params.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1989 2023-07-18 09:06:00.000000 unicef-power-query-0.2.1/tests/test_queries.py
+-rw-r--r--   0 jojo       (501) staff       (20)      829 2023-07-13 09:09:33.000000 unicef-power-query-0.2.1/tests/test_utils.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1772 2023-07-18 09:06:00.000000 unicef-power-query-0.2.1/tests/test_views.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1022 2023-07-04 08:17:12.000000 unicef-power-query-0.2.1/tox.ini
```

### Comparing `unicef-power-query-0.2/LICENSE` & `unicef-power-query-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/PKG-INFO` & `unicef-power-query-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicef-power-query
-Version: 0.2
+Version: 0.2.1
 Summary: Provides Basic UNICEF User model and integration with Azure
 Home-page: https://github.com/unicef/unicef-security
 Author: UNICEF
 License: Apache 2 License
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `unicef-power-query-0.2/README.rst` & `unicef-power-query-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/setup.py` & `unicef-power-query-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/__pycache__/admin.cpython-39.pyc` & `unicef-power-query-0.2.1/src/power_query/__pycache__/admin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/__pycache__/celery_tasks.cpython-39.pyc` & `unicef-power-query-0.2.1/src/power_query/__pycache__/celery_tasks.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/__pycache__/defaults.cpython-39.pyc` & `unicef-power-query-0.2.1/src/power_query/__pycache__/defaults.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/__pycache__/exceptions.cpython-39.pyc` & `unicef-power-query-0.2.1/src/power_query/__pycache__/exceptions.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/__pycache__/fixtures.cpython-39.pyc` & `unicef-power-query-0.2.1/src/power_query/__pycache__/fixtures.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jul 13 09:15:57 2023 UTC, .py size: 4351 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 cdc0 af64 ff10 0000  a..........d....
+00000000: 610d 0d0a 0000 0000 f855 b664 ff10 0000  a........U.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 2c01 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6400 6405 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6400 6401 6c0d 5a0d 6400  m.Z...d.d.l.Z.d.
```

### Comparing `unicef-power-query-0.2/src/power_query/__pycache__/forms.cpython-39.pyc` & `unicef-power-query-0.2.1/src/power_query/__pycache__/forms.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/__pycache__/json.cpython-39.pyc` & `unicef-power-query-0.2.1/src/power_query/__pycache__/json.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/__pycache__/mixin.cpython-39.pyc` & `unicef-power-query-0.2.1/src/power_query/__pycache__/mixin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/__pycache__/models.cpython-39.pyc` & `unicef-power-query-0.2.1/src/power_query/__pycache__/models.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/__pycache__/utils.cpython-39.pyc` & `unicef-power-query-0.2.1/src/power_query/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/__pycache__/validators.cpython-39.pyc` & `unicef-power-query-0.2.1/src/power_query/__pycache__/validators.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/__pycache__/views.cpython-39.pyc` & `unicef-power-query-0.2.1/src/power_query/__pycache__/views.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/__pycache__/widget.cpython-39.pyc` & `unicef-power-query-0.2.1/src/power_query/__pycache__/widget.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/admin.py` & `unicef-power-query-0.2.1/src/power_query/admin.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/celery_tasks.py` & `unicef-power-query-0.2.1/src/power_query/celery_tasks.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/defaults.py` & `unicef-power-query-0.2.1/src/power_query/defaults.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/fixtures.py` & `unicef-power-query-0.2.1/src/power_query/fixtures.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/forms.py` & `unicef-power-query-0.2.1/src/power_query/forms.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/json.py` & `unicef-power-query-0.2.1/src/power_query/json.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/management/commands/pq.py` & `unicef-power-query-0.2.1/src/power_query/management/commands/pq.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/migrations/0001_migration_squashed_0014_migration.py` & `unicef-power-query-0.2.1/src/power_query/migrations/0001_migration_squashed_0014_migration.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/migrations/__pycache__/0001_migration_squashed_0014_migration.cpython-39.pyc` & `unicef-power-query-0.2.1/src/power_query/migrations/__pycache__/0001_migration_squashed_0014_migration.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jul 13 07:18:09 2023 UTC, .py size: 15211 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 31a5 af64 6b3b 0000  a.......1..dk;..
+00000000: 610d 0d0a 0000 0000 f855 b664 6b3b 0000  a........U.dk;..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 0100 6400 6401 6c08  m.Z.m.Z...d.d.l.
 00000060: 5a09 6400 6401 6c0a 5a09 6400 6401 6c0b  Z.d.d.l.Z.d.d.l.
 00000070: 5a09 6400 6404 6c0c 6d0d 5a0d 0100 6405  Z.d.d.l.m.Z...d.
```

### Comparing `unicef-power-query-0.2/src/power_query/mixin.py` & `unicef-power-query-0.2.1/src/power_query/mixin.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/models.py` & `unicef-power-query-0.2.1/src/power_query/models.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/static/admin/power_query/code.css` & `unicef-power-query-0.2.1/src/power_query/static/admin/power_query/code.css`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/abcdef.css` & `unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/abcdef.css`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/active-line.js` & `unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/active-line.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/codemirror.css` & `unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/codemirror.css`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/codemirror.js` & `unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/codemirror.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/django.js` & `unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/django.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/foldcode.js` & `unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/foldcode.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/foldgutter.js` & `unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/foldgutter.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/fullscreen.js` & `unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/fullscreen.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/indent-fold.js` & `unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/indent-fold.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/matchbrackets.js` & `unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/matchbrackets.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/midnight.css` & `unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/midnight.css`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/overlay.js` & `unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/overlay.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/python.js` & `unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/python.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/xml.js` & `unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/xml.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/yaml.js` & `unicef-power-query-0.2.1/src/power_query/static/admin/power_query/codemirror/yaml.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/static/admin/power_query/colorful.css` & `unicef-power-query-0.2.1/src/power_query/static/admin/power_query/colorful.css`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/static/admin/power_query/diff.css` & `unicef-power-query-0.2.1/src/power_query/static/admin/power_query/diff.css`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/static/admin/power_query/editor.png` & `unicef-power-query-0.2.1/src/power_query/static/admin/power_query/editor.png`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/static/redo.png` & `unicef-power-query-0.2.1/src/power_query/static/redo.png`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/static/undo.png` & `unicef-power-query-0.2.1/src/power_query/static/undo.png`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/templates/admin/power_query/formatter/change_form.html` & `unicef-power-query-0.2.1/src/power_query/templates/admin/power_query/formatter/change_form.html`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/templates/admin/power_query/query/monitor.html` & `unicef-power-query-0.2.1/src/power_query/templates/admin/power_query/query/monitor.html`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/templates/admin/power_query/query/preview.html` & `unicef-power-query-0.2.1/src/power_query/templates/admin/power_query/query/preview.html`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/templates/admin/power_query/queryargs/change_form.html` & `unicef-power-query-0.2.1/src/power_query/templates/admin/power_query/queryargs/change_form.html`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/templates/admin/power_query/report/monitor.html` & `unicef-power-query-0.2.1/src/power_query/templates/admin/power_query/report/monitor.html`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/templates/power_query/base.html` & `unicef-power-query-0.2.1/src/power_query/templates/power_query/base.html`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/templates/power_query/detail.html` & `unicef-power-query-0.2.1/src/power_query/templates/power_query/detail.html`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/templates/power_query/widgets/codewidget.html` & `unicef-power-query-0.2.1/src/power_query/templates/power_query/widgets/codewidget.html`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/templatetags/__pycache__/power_query.cpython-39.pyc` & `unicef-power-query-0.2.1/src/power_query/templatetags/__pycache__/power_query.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/templatetags/power_query.py` & `unicef-power-query-0.2.1/src/power_query/templatetags/power_query.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/utils.py` & `unicef-power-query-0.2.1/src/power_query/utils.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/views.py` & `unicef-power-query-0.2.1/src/power_query/views.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/power_query/widget.py` & `unicef-power-query-0.2.1/src/power_query/widget.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/src/unicef_power_query.egg-info/PKG-INFO` & `unicef-power-query-0.2.1/src/unicef_power_query.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicef-power-query
-Version: 0.2
+Version: 0.2.1
 Summary: Provides Basic UNICEF User model and integration with Azure
 Home-page: https://github.com/unicef/unicef-security
 Author: UNICEF
 License: Apache 2 License
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `unicef-power-query-0.2/src/unicef_power_query.egg-info/SOURCES.txt` & `unicef-power-query-0.2.1/src/unicef_power_query.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -19,37 +19,54 @@
 src/power_query/notify.py
 src/power_query/signals.py
 src/power_query/urls.py
 src/power_query/utils.py
 src/power_query/validators.py
 src/power_query/views.py
 src/power_query/widget.py
+src/power_query/__pycache__/__init__.cpython-311.pyc
 src/power_query/__pycache__/__init__.cpython-39.pyc
+src/power_query/__pycache__/admin.cpython-311.pyc
 src/power_query/__pycache__/admin.cpython-39.pyc
+src/power_query/__pycache__/apps.cpython-311.pyc
 src/power_query/__pycache__/apps.cpython-39.pyc
+src/power_query/__pycache__/celery_tasks.cpython-311.pyc
 src/power_query/__pycache__/celery_tasks.cpython-39.pyc
 src/power_query/__pycache__/defaults.cpython-39.pyc
+src/power_query/__pycache__/exceptions.cpython-311.pyc
 src/power_query/__pycache__/exceptions.cpython-39.pyc
 src/power_query/__pycache__/fixtures.cpython-39.pyc
+src/power_query/__pycache__/forms.cpython-311.pyc
 src/power_query/__pycache__/forms.cpython-39.pyc
+src/power_query/__pycache__/json.cpython-311.pyc
 src/power_query/__pycache__/json.cpython-39.pyc
 src/power_query/__pycache__/mixin.cpython-39.pyc
+src/power_query/__pycache__/models.cpython-311.pyc
 src/power_query/__pycache__/models.cpython-39.pyc
+src/power_query/__pycache__/urls.cpython-311.pyc
 src/power_query/__pycache__/urls.cpython-39.pyc
+src/power_query/__pycache__/utils.cpython-311.pyc
 src/power_query/__pycache__/utils.cpython-39.pyc
+src/power_query/__pycache__/validators.cpython-311.pyc
 src/power_query/__pycache__/validators.cpython-39.pyc
+src/power_query/__pycache__/views.cpython-311.pyc
 src/power_query/__pycache__/views.cpython-39.pyc
+src/power_query/__pycache__/widget.cpython-311.pyc
 src/power_query/__pycache__/widget.cpython-39.pyc
 src/power_query/management/__init__.py
 src/power_query/management/__pycache__/__init__.cpython-39.pyc
 src/power_query/management/commands/__init__.py
 src/power_query/management/commands/pq.py
 src/power_query/migrations/0001_migration_squashed_0014_migration.py
+src/power_query/migrations/0015_alter_dataset_description_and_more.py
 src/power_query/migrations/__init__.py
+src/power_query/migrations/__pycache__/0001_migration_squashed_0014_migration.cpython-311.pyc
 src/power_query/migrations/__pycache__/0001_migration_squashed_0014_migration.cpython-39.pyc
+src/power_query/migrations/__pycache__/0015_alter_dataset_description_and_more.cpython-39.pyc
+src/power_query/migrations/__pycache__/__init__.cpython-311.pyc
 src/power_query/migrations/__pycache__/__init__.cpython-39.pyc
 src/power_query/static/power_query.css
 src/power_query/static/power_query.css.map
 src/power_query/static/power_query.scss
 src/power_query/static/redo.png
 src/power_query/static/undo.png
 src/power_query/static/admin/power_query/code.css
@@ -89,15 +106,17 @@
 src/power_query/templates/admin/power_query/report/monitor.html
 src/power_query/templates/power_query/base.html
 src/power_query/templates/power_query/detail.html
 src/power_query/templates/power_query/list.html
 src/power_query/templates/power_query/widgets/codewidget.html
 src/power_query/templatetags/__init__.py
 src/power_query/templatetags/power_query.py
+src/power_query/templatetags/__pycache__/__init__.cpython-311.pyc
 src/power_query/templatetags/__pycache__/__init__.cpython-39.pyc
+src/power_query/templatetags/__pycache__/power_query.cpython-311.pyc
 src/power_query/templatetags/__pycache__/power_query.cpython-39.pyc
 src/unicef_power_query.egg-info/PKG-INFO
 src/unicef_power_query.egg-info/SOURCES.txt
 src/unicef_power_query.egg-info/dependency_links.txt
 src/unicef_power_query.egg-info/requires.txt
 src/unicef_power_query.egg-info/top_level.txt
 tests/.coveragerc
```

### Comparing `unicef-power-query-0.2/tests/__pycache__/test_admin.cpython-311-pytest-7.3.1.pyc` & `unicef-power-query-0.2.1/tests/__pycache__/test_admin.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/tests/__pycache__/test_auth.cpython-311-pytest-7.3.1.pyc` & `unicef-power-query-0.2.1/tests/__pycache__/test_auth.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/tests/__pycache__/test_celery.cpython-311-pytest-7.3.1.pyc` & `unicef-power-query-0.2.1/tests/__pycache__/test_celery.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/tests/__pycache__/test_params.cpython-311-pytest-7.3.1.pyc` & `unicef-power-query-0.2.1/tests/__pycache__/test_params.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/tests/__pycache__/test_queries.cpython-311-pytest-7.3.1.pyc` & `unicef-power-query-0.2.1/tests/__pycache__/test_queries.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc` & `unicef-power-query-0.2.1/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/tests/__pycache__/test_views.cpython-311-pytest-7.3.1.pyc` & `unicef-power-query-0.2.1/tests/__pycache__/test_views.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/tests/demoproject/db.sqlite3` & `unicef-power-query-0.2.1/tests/demoproject/db.sqlite3`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/tests/demoproject/demo/__pycache__/celery.cpython-311.pyc` & `unicef-power-query-0.2.1/tests/demoproject/demo/__pycache__/celery.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x17ab7d64 (Mon Jun  5 09:29:59 2023 UTC)
+moddate:  0x88d5a364 (Tue Jul  4 08:17:12 2023 UTC)
 files sz: 245
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `unicef-power-query-0.2/tests/demoproject/demo/__pycache__/models.cpython-311.pyc` & `unicef-power-query-0.2.1/tests/demoproject/demo/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/tests/demoproject/demo/__pycache__/settings.cpython-311.pyc` & `unicef-power-query-0.2.1/tests/demoproject/demo/__pycache__/settings.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x17ab7d64 (Mon Jun  5 09:29:59 2023 UTC)
+moddate:  0x88d5a364 (Tue Jul  4 08:17:12 2023 UTC)
 files sz: 2590
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `unicef-power-query-0.2/tests/demoproject/demo/__pycache__/urls.cpython-311.pyc` & `unicef-power-query-0.2.1/tests/demoproject/demo/__pycache__/urls.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/tests/demoproject/demo/__pycache__/wsgi.cpython-311.pyc` & `unicef-power-query-0.2.1/tests/demoproject/demo/__pycache__/wsgi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/tests/demoproject/demo/migrations/0001_initial.py` & `unicef-power-query-0.2.1/tests/demoproject/demo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/tests/demoproject/demo/migrations/__pycache__/0001_initial.cpython-311.pyc` & `unicef-power-query-0.2.1/tests/demoproject/demo/migrations/__pycache__/0001_initial.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/tests/demoproject/demo/settings.py` & `unicef-power-query-0.2.1/tests/demoproject/demo/settings.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/tests/test_admin.py` & `unicef-power-query-0.2.1/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/tests/test_auth.py` & `unicef-power-query-0.2.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/tests/test_celery.py` & `unicef-power-query-0.2.1/tests/test_celery.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/tests/test_queries.py` & `unicef-power-query-0.2.1/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/tests/test_utils.py` & `unicef-power-query-0.2.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/tests/test_views.py` & `unicef-power-query-0.2.1/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.2/tox.ini` & `unicef-power-query-0.2.1/tox.ini`

 * *Files identical despite different names*

