# Comparing `tmp/bk_resource-0.4.0rc2.tar.gz` & `tmp/bk_resource-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bk_resource-0.4.0rc2.tar", last modified: Fri Apr 21 03:32:04 2023, max compression
+gzip compressed data, was "dist/bk_resource-0.4.1.tar", last modified: Wed Jul 19 07:06:38 2023, max compression
```

## Comparing `bk_resource-0.4.0rc2.tar` & `bk_resource-0.4.1.tar`

### file list

```diff
@@ -1,73 +1,75 @@
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/
--rw-r--r--   0 orenzhang   (501) staff       (20)      221 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/PKG-INFO
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/locale/
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/locale/zh_CN/
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 orenzhang   (501) staff       (20)     3022 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 orenzhang   (501) staff       (20)     4398 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/locale/zh_CN/LC_MESSAGES/django.po
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/locale/en/
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/locale/en/LC_MESSAGES/
--rw-r--r--   0 orenzhang   (501) staff       (20)     2943 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 orenzhang   (501) staff       (20)     4322 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 orenzhang   (501) staff       (20)     4064 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/tasks.py
--rw-r--r--   0 orenzhang   (501) staff       (20)    11571 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/viewsets.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     7083 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/tools.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     2690 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/serializers.py
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/management/
--rw-r--r--   0 orenzhang   (501) staff       (20)     4859 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/management/finder.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     4974 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/management/stub_file_generator.py
--rw-r--r--   0 orenzhang   (501) staff       (20)      891 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/management/__init__.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     1110 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/management/exceptions.py
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/management/commands/
--rw-r--r--   0 orenzhang   (501) staff       (20)     1243 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/management/commands/start_resource.py
--rw-r--r--   0 orenzhang   (501) staff       (20)      891 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/management/commands/__init__.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     1110 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/management/commands/generate_resource_stub_file.py
--rw-r--r--   0 orenzhang   (501) staff       (20)    10304 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/management/root.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     2058 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/__init__.py
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/utils/
--rw-r--r--   0 orenzhang   (501) staff       (20)     1176 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/utils/inspectors.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     3337 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/utils/local.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     1593 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/utils/request.py
--rw-r--r--   0 orenzhang   (501) staff       (20)    10609 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/utils/cache.py
--rw-r--r--   0 orenzhang   (501) staff       (20)      891 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/utils/__init__.py
--rw-r--r--   0 orenzhang   (501) staff       (20)      950 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/utils/logger.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     2080 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/utils/generators.py
--rw-r--r--   0 orenzhang   (501) staff       (20)    10967 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/utils/time_tools.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     3313 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/utils/text.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     3317 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/utils/request_log.py
--rw-r--r--   0 orenzhang   (501) staff       (20)    13170 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/utils/common_utils.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     5017 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/utils/thread_backend.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     1132 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/apps.py
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/contrib/
--rw-r--r--   0 orenzhang   (501) staff       (20)     5589 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/contrib/bk_api.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     2969 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/contrib/cache.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     1121 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/contrib/__init__.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     5941 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/contrib/model.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     8620 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/contrib/api.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     3724 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/settings.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     3883 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/exceptions.py
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/conf/
--rw-r--r--   0 orenzhang   (501) staff       (20)      891 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/conf/__init__.py
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/conf/app_template/
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/conf/app_template/migrations/
--rw-r--r--   0 orenzhang   (501) staff       (20)       24 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/conf/app_template/migrations/__init__.py-tpl
--rw-r--r--   0 orenzhang   (501) staff       (20)       24 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/conf/app_template/__init__.py-tpl
--rw-r--r--   0 orenzhang   (501) staff       (20)      152 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/conf/app_template/resources.py-tpl
--rw-r--r--   0 orenzhang   (501) staff       (20)      173 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/conf/app_template/views.py-tpl
--rw-r--r--   0 orenzhang   (501) staff       (20)      189 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/conf/app_template/urls.py-tpl
--rw-r--r--   0 orenzhang   (501) staff       (20)       60 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/conf/app_template/admin.py-tpl
--rw-r--r--   0 orenzhang   (501) staff       (20)      196 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/conf/app_template/apps.py-tpl
--rw-r--r--   0 orenzhang   (501) staff       (20)       64 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/conf/app_template/serializers.py-tpl
--rw-r--r--   0 orenzhang   (501) staff       (20)       54 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/conf/app_template/models.py-tpl
--rw-r--r--   0 orenzhang   (501) staff       (20)     2369 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/routers.py
--rw-r--r--   0 orenzhang   (501) staff       (20)    13832 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/base.py
--rw-r--r--   0 orenzhang   (501) staff       (20)      141 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/MANIFEST.in
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource.egg-info/
--rw-r--r--   0 orenzhang   (501) staff       (20)      221 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource.egg-info/PKG-INFO
--rw-r--r--   0 orenzhang   (501) staff       (20)     1900 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource.egg-info/SOURCES.txt
--rw-r--r--   0 orenzhang   (501) staff       (20)      164 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource.egg-info/requires.txt
--rw-r--r--   0 orenzhang   (501) staff       (20)       12 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource.egg-info/top_level.txt
--rw-r--r--   0 orenzhang   (501) staff       (20)        1 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource.egg-info/dependency_links.txt
--rw-r--r--   0 orenzhang   (501) staff       (20)     1633 2023-04-21 03:31:53.000000 bk_resource-0.4.0rc2/setup.py
--rw-r--r--   0 orenzhang   (501) staff       (20)       38 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 07:06:38.000000 bk_resource-0.4.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 07:06:38.000000 bk_resource-0.4.1/bk_resource/
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/apps.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 07:06:38.000000 bk_resource-0.4.1/bk_resource/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 07:06:38.000000 bk_resource-0.4.1/bk_resource/locale/zh_CN/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 07:06:38.000000 bk_resource-0.4.1/bk_resource/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     4398 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/locale/zh_CN/LC_MESSAGES/django.po
+-rw-r--r--   0 root         (0) root         (0)     3022 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/locale/zh_CN/LC_MESSAGES/django.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 07:06:38.000000 bk_resource-0.4.1/bk_resource/locale/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 07:06:38.000000 bk_resource-0.4.1/bk_resource/locale/en/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     4322 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 root         (0) root         (0)     2943 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/locale/en/LC_MESSAGES/django.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 07:06:38.000000 bk_resource-0.4.1/bk_resource/conf/
+-rw-r--r--   0 root         (0) root         (0)      891 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/conf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 07:06:38.000000 bk_resource-0.4.1/bk_resource/conf/app_template/
+-rw-r--r--   0 root         (0) root         (0)      196 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/conf/app_template/apps.py-tpl
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/conf/app_template/__init__.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      152 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/conf/app_template/resources.py-tpl
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/conf/app_template/admin.py-tpl
+-rw-r--r--   0 root         (0) root         (0)       54 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/conf/app_template/models.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      189 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/conf/app_template/urls.py-tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 07:06:38.000000 bk_resource-0.4.1/bk_resource/conf/app_template/migrations/
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/conf/app_template/migrations/__init__.py-tpl
+-rw-r--r--   0 root         (0) root         (0)       64 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/conf/app_template/serializers.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      173 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/conf/app_template/views.py-tpl
+-rw-r--r--   0 root         (0) root         (0)     3883 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     3724 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 07:06:38.000000 bk_resource-0.4.1/bk_resource/management/
+-rw-r--r--   0 root         (0) root         (0)      891 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/management/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/management/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    10304 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/management/root.py
+-rw-r--r--   0 root         (0) root         (0)     4859 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/management/finder.py
+-rw-r--r--   0 root         (0) root         (0)     4974 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/management/stub_file_generator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 07:06:38.000000 bk_resource-0.4.1/bk_resource/management/commands/
+-rw-r--r--   0 root         (0) root         (0)      891 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/management/commands/start_resource.py
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/management/commands/generate_resource_stub_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 07:06:38.000000 bk_resource-0.4.1/bk_resource/contrib/
+-rw-r--r--   0 root         (0) root         (0)     2969 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/contrib/cache.py
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/contrib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5941 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/contrib/model.py
+-rw-r--r--   0 root         (0) root         (0)     5589 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/contrib/bk_api.py
+-rw-r--r--   0 root         (0) root         (0)     8620 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/contrib/api.py
+-rw-r--r--   0 root         (0) root         (0)     7083 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 07:06:38.000000 bk_resource-0.4.1/bk_resource/utils/
+-rw-r--r--   0 root         (0) root         (0)    10609 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/utils/cache.py
+-rw-r--r--   0 root         (0) root         (0)     3313 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/utils/text.py
+-rw-r--r--   0 root         (0) root         (0)      891 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1593 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/utils/request.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     5104 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/utils/factory.py
+-rw-r--r--   0 root         (0) root         (0)     3317 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/utils/request_log.py
+-rw-r--r--   0 root         (0) root         (0)    13170 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/utils/common_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5017 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/utils/thread_backend.py
+-rw-r--r--   0 root         (0) root         (0)    10967 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/utils/time_tools.py
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/utils/inspectors.py
+-rw-r--r--   0 root         (0) root         (0)     3337 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/utils/local.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/utils/generators.py
+-rw-r--r--   0 root         (0) root         (0)     2690 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/serializers.py
+-rw-r--r--   0 root         (0) root         (0)    11699 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/viewsets.py
+-rw-r--r--   0 root         (0) root         (0)     2369 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/routers.py
+-rw-r--r--   0 root         (0) root         (0)    13832 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/base.py
+-rw-r--r--   0 root         (0) root         (0)     4064 2023-07-19 07:06:17.000000 bk_resource-0.4.1/bk_resource/tasks.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-07-19 07:06:17.000000 bk_resource-0.4.1/LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 07:06:38.000000 bk_resource-0.4.1/bk_resource.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      164 2023-07-19 07:06:38.000000 bk_resource-0.4.1/bk_resource.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-07-19 07:06:38.000000 bk_resource-0.4.1/bk_resource.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-19 07:06:38.000000 bk_resource-0.4.1/bk_resource.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      233 2023-07-19 07:06:38.000000 bk_resource-0.4.1/bk_resource.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 07:06:38.000000 bk_resource-0.4.1/bk_resource.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      233 2023-07-19 07:06:38.000000 bk_resource-0.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-07-19 07:06:17.000000 bk_resource-0.4.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-19 07:06:38.000000 bk_resource-0.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      141 2023-07-19 07:06:17.000000 bk_resource-0.4.1/MANIFEST.in
```

### Comparing `bk_resource-0.4.0rc2/bk_resource/locale/zh_CN/LC_MESSAGES/django.mo` & `bk_resource-0.4.1/bk_resource/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/locale/zh_CN/LC_MESSAGES/django.po` & `bk_resource-0.4.1/bk_resource/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/locale/en/LC_MESSAGES/django.mo` & `bk_resource-0.4.1/bk_resource/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/locale/en/LC_MESSAGES/django.po` & `bk_resource-0.4.1/bk_resource/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/tasks.py` & `bk_resource-0.4.1/bk_resource/tasks.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/viewsets.py` & `bk_resource-0.4.1/bk_resource/viewsets.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,14 +267,18 @@
                     raise Exception(gettext("[%s] 访问的资源不存在") % resource_route.resource_class.__name__)
 
             if resource_route.content_encoding:
                 response.content_encoding = resource_route.content_encoding
 
             end_time = arrow.now().datetime
 
+            # 不记录日志的直接返回
+            if not resource.support_data_collect:
+                return response
+
             # 记录请求日志
             resource_name = "{}.{}".format(resource.__class__.__module__, resource.__class__.__name__)
             log_handler = bk_resource_settings.REQUEST_LOG_HANDLER
             log_handler(resource_name, start_time, end_time, request_data, data).record()
 
             return response
```

### Comparing `bk_resource-0.4.0rc2/bk_resource/tools.py` & `bk_resource-0.4.1/bk_resource/tools.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/serializers.py` & `bk_resource-0.4.1/bk_resource/serializers.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/management/finder.py` & `bk_resource-0.4.1/bk_resource/management/finder.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/management/stub_file_generator.py` & `bk_resource-0.4.1/bk_resource/management/stub_file_generator.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/management/__init__.py` & `bk_resource-0.4.1/bk_resource/management/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/management/exceptions.py` & `bk_resource-0.4.1/bk_resource/management/exceptions.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/management/commands/start_resource.py` & `bk_resource-0.4.1/bk_resource/management/commands/start_resource.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/management/commands/__init__.py` & `bk_resource-0.4.1/bk_resource/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/management/commands/generate_resource_stub_file.py` & `bk_resource-0.4.1/bk_resource/management/commands/generate_resource_stub_file.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/management/root.py` & `bk_resource-0.4.1/bk_resource/management/root.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/__init__.py` & `bk_resource-0.4.1/bk_resource/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/utils/inspectors.py` & `bk_resource-0.4.1/bk_resource/utils/inspectors.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/utils/local.py` & `bk_resource-0.4.1/bk_resource/utils/local.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/utils/request.py` & `bk_resource-0.4.1/bk_resource/utils/request.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/utils/cache.py` & `bk_resource-0.4.1/bk_resource/utils/cache.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/utils/__init__.py` & `bk_resource-0.4.1/bk_resource/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/utils/logger.py` & `bk_resource-0.4.1/bk_resource/utils/logger.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/utils/generators.py` & `bk_resource-0.4.1/bk_resource/utils/generators.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/utils/time_tools.py` & `bk_resource-0.4.1/bk_resource/utils/time_tools.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/utils/text.py` & `bk_resource-0.4.1/bk_resource/utils/text.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/utils/request_log.py` & `bk_resource-0.4.1/bk_resource/utils/request_log.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/utils/common_utils.py` & `bk_resource-0.4.1/bk_resource/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/utils/thread_backend.py` & `bk_resource-0.4.1/bk_resource/utils/thread_backend.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/apps.py` & `bk_resource-0.4.1/bk_resource/apps.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/contrib/bk_api.py` & `bk_resource-0.4.1/bk_resource/contrib/bk_api.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/contrib/cache.py` & `bk_resource-0.4.1/bk_resource/contrib/cache.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/contrib/__init__.py` & `bk_resource-0.4.1/bk_resource/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/contrib/model.py` & `bk_resource-0.4.1/bk_resource/contrib/model.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/contrib/api.py` & `bk_resource-0.4.1/bk_resource/contrib/api.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/settings.py` & `bk_resource-0.4.1/bk_resource/settings.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/exceptions.py` & `bk_resource-0.4.1/bk_resource/exceptions.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/conf/__init__.py` & `bk_resource-0.4.1/bk_resource/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/routers.py` & `bk_resource-0.4.1/bk_resource/routers.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource/base.py` & `bk_resource-0.4.1/bk_resource/base.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc2/bk_resource.egg-info/SOURCES.txt` & `bk_resource-0.4.1/bk_resource.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 MANIFEST.in
 setup.py
 bk_resource/__init__.py
 bk_resource/apps.py
 bk_resource/base.py
 bk_resource/exceptions.py
 bk_resource/routers.py
@@ -41,14 +42,15 @@
 bk_resource/management/stub_file_generator.py
 bk_resource/management/commands/__init__.py
 bk_resource/management/commands/generate_resource_stub_file.py
 bk_resource/management/commands/start_resource.py
 bk_resource/utils/__init__.py
 bk_resource/utils/cache.py
 bk_resource/utils/common_utils.py
+bk_resource/utils/factory.py
 bk_resource/utils/generators.py
 bk_resource/utils/inspectors.py
 bk_resource/utils/local.py
 bk_resource/utils/logger.py
 bk_resource/utils/request.py
 bk_resource/utils/request_log.py
 bk_resource/utils/text.py
```

### Comparing `bk_resource-0.4.0rc2/setup.py` & `bk_resource-0.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,30 +16,30 @@
 to the current version of the project delivered to anyone in the future.
 """
 
 from setuptools import setup
 
 setup(
     name="bk_resource",
-    version="0.4.0-rc.2",
+    version="0.4.1",
     author="blueking",
     url="https://bk.tencent.com",
     author_email="blueking@tencent.com",
     description="Bk Resource",
     packages=[
         "bk_resource",
         "bk_resource.conf",
         "bk_resource.contrib",
         "bk_resource.management",
         "bk_resource.management.commands",
         "bk_resource.utils",
     ],
     install_requires=[
-        "blueapps>=4.6.0rc2",
-        "django>=3.2,<4",
+        "blueapps==4.7.0rc1",
+        "django>=3.2.18",
         "djangorestframework>=3.12.0",
         "drf-yasg>=1.20.0",
         "pyinstrument>=3.4.2",
         "arrow>=1.2.0",
         "django-rest-framework-condition>=0.1.1",
         "celery>=4,<5",
     ],
```

