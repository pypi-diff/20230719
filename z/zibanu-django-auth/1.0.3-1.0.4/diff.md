# Comparing `tmp/zibanu-django-auth-1.0.3.tar.gz` & `tmp/zibanu-django-auth-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zibanu-django-auth-1.0.3.tar", last modified: Wed Jul  5 14:49:04 2023, max compression
+gzip compressed data, was "zibanu-django-auth-1.0.4.tar", last modified: Wed Jul 19 01:06:15 2023, max compression
```

## Comparing `zibanu-django-auth-1.0.3.tar` & `zibanu-django-auth-1.0.4.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 14:49:04.709203 zibanu-django-auth-1.0.3/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu-django-auth-1.0.3/LICENSE
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      109 2023-06-19 16:17:43.000000 zibanu-django-auth-1.0.3/MANIFEST.in
--rw-r--r--   0 macercha  (1000) macercha  (1000)    41404 2023-07-05 14:49:04.708203 zibanu-django-auth-1.0.3/PKG-INFO
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      179 2023-06-19 19:19:54.000000 zibanu-django-auth-1.0.3/README.md
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      956 2023-07-05 14:48:09.000000 zibanu-django-auth-1.0.3/pyproject.toml
--rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-07-05 14:49:04.709203 zibanu-django-auth-1.0.3/setup.cfg
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 14:49:04.683204 zibanu-django-auth-1.0.3/zibanu/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 14:49:04.683204 zibanu-django-auth-1.0.3/zibanu/django/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 14:49:04.701204 zibanu-django-auth-1.0.3/zibanu/django/auth/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      311 2023-04-08 12:20:31.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 14:49:04.701204 zibanu-django-auth-1.0.3/zibanu/django/auth/api/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      311 2023-04-08 12:25:30.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/api/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 14:49:04.702204 zibanu-django-auth-1.0.3/zibanu/django/auth/api/serializers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      787 2023-06-19 16:01:54.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/api/serializers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      533 2023-06-19 15:57:29.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/api/serializers/group.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      549 2023-06-19 16:00:06.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/api/serializers/permission.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      749 2023-04-27 12:00:18.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/api/serializers/profile.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3051 2023-04-27 12:17:39.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/api/serializers/token.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3944 2023-06-07 19:44:45.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/api/serializers/user.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 14:49:04.703204 zibanu-django-auth-1.0.3/zibanu/django/auth/api/services/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      553 2023-06-19 19:50:50.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/api/services/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1104 2023-06-19 16:01:54.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/api/services/group.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      954 2023-06-19 16:05:31.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/api/services/permission.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2012 2023-06-19 20:05:14.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/api/services/profile.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    13346 2023-06-20 15:59:00.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/api/services/user.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1245 2023-05-17 01:05:01.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 14:49:04.704203 zibanu-django-auth-1.0.3/zibanu/django/auth/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      313 2023-04-10 19:32:01.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 14:49:04.705203 zibanu-django-auth-1.0.3/zibanu/django/auth/lib/choices/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      313 2023-04-10 19:48:01.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/lib/choices/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 14:49:04.705203 zibanu-django-auth-1.0.3/zibanu/django/auth/lib/managers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      314 2023-05-25 18:23:00.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/lib/managers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1396 2023-05-17 00:58:35.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/lib/signal_events.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      412 2023-05-13 17:53:49.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/lib/signals.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      916 2023-06-19 17:31:05.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/lib/utils.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 14:49:04.699204 zibanu-django-auth-1.0.3/zibanu/django/auth/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 14:49:04.699204 zibanu-django-auth-1.0.3/zibanu/django/auth/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 14:49:04.705203 zibanu-django-auth-1.0.3/zibanu/django/auth/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2172 2023-06-19 20:43:36.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3203 2023-06-19 20:43:24.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 14:49:04.706204 zibanu-django-auth-1.0.3/zibanu/django/auth/migrations/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    24474 2023-04-11 22:39:55.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/migrations/0001_initial.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    23351 2023-07-05 13:34:24.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/migrations/0002_alter_userprofile_timezone.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      313 2023-04-10 19:31:28.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/migrations/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1914 2023-07-05 13:34:15.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/models.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 14:49:04.707203 zibanu-django-auth-1.0.3/zibanu/django/auth/templates/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      487 2023-05-23 16:11:28.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/templates/change_password.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      324 2023-05-22 17:32:26.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/templates/change_password.txt
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      123 2023-05-13 16:44:16.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/templates/request-code.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2023-05-13 16:41:48.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/templates/request-code.txt
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      559 2023-05-22 17:30:07.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/templates/request_password.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      346 2023-05-13 16:55:01.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/templates/request_password.txt
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1701 2023-06-19 20:28:16.000000 zibanu-django-auth-1.0.3/zibanu/django/auth/urls.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-05 14:49:04.708203 zibanu-django-auth-1.0.3/zibanu_django_auth.egg-info/
--rw-r--r--   0 macercha  (1000) macercha  (1000)    41404 2023-07-05 14:49:04.000000 zibanu-django-auth-1.0.3/zibanu_django_auth.egg-info/PKG-INFO
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1665 2023-07-05 14:49:04.000000 zibanu-django-auth-1.0.3/zibanu_django_auth.egg-info/SOURCES.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-07-05 14:49:04.000000 zibanu-django-auth-1.0.3/zibanu_django_auth.egg-info/dependency_links.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)      105 2023-07-05 14:49:04.000000 zibanu-django-auth-1.0.3/zibanu_django_auth.egg-info/requires.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2023-07-05 14:49:04.000000 zibanu-django-auth-1.0.3/zibanu_django_auth.egg-info/top_level.txt
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-19 01:06:15.582108 zibanu-django-auth-1.0.4/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu-django-auth-1.0.4/LICENSE
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      109 2023-06-19 16:17:43.000000 zibanu-django-auth-1.0.4/MANIFEST.in
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    41404 2023-07-19 01:06:15.582108 zibanu-django-auth-1.0.4/PKG-INFO
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      179 2023-06-19 19:19:54.000000 zibanu-django-auth-1.0.4/README.md
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      956 2023-07-19 01:05:22.000000 zibanu-django-auth-1.0.4/pyproject.toml
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-07-19 01:06:15.582108 zibanu-django-auth-1.0.4/setup.cfg
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-19 01:06:15.569109 zibanu-django-auth-1.0.4/zibanu/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-19 01:06:15.569109 zibanu-django-auth-1.0.4/zibanu/django/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-19 01:06:15.575109 zibanu-django-auth-1.0.4/zibanu/django/auth/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      311 2023-04-08 12:20:31.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-19 01:06:15.575109 zibanu-django-auth-1.0.4/zibanu/django/auth/api/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      311 2023-04-08 12:25:30.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/api/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-19 01:06:15.576109 zibanu-django-auth-1.0.4/zibanu/django/auth/api/serializers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      787 2023-06-19 16:01:54.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/api/serializers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      533 2023-06-19 15:57:29.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/api/serializers/group.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      549 2023-06-19 16:00:06.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/api/serializers/permission.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      767 2023-07-19 00:58:14.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/api/serializers/profile.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3051 2023-04-27 12:17:39.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/api/serializers/token.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3944 2023-06-07 19:44:45.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/api/serializers/user.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-19 01:06:15.577108 zibanu-django-auth-1.0.4/zibanu/django/auth/api/services/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      553 2023-06-19 19:50:50.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/api/services/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1104 2023-06-19 16:01:54.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/api/services/group.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      954 2023-06-19 16:05:31.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/api/services/permission.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2012 2023-06-19 20:05:14.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/api/services/profile.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    13346 2023-06-20 15:59:00.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/api/services/user.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1245 2023-05-17 01:05:01.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-19 01:06:15.578109 zibanu-django-auth-1.0.4/zibanu/django/auth/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      313 2023-04-10 19:32:01.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-19 01:06:15.578109 zibanu-django-auth-1.0.4/zibanu/django/auth/lib/choices/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      313 2023-04-10 19:48:01.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/lib/choices/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-19 01:06:15.578109 zibanu-django-auth-1.0.4/zibanu/django/auth/lib/managers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      314 2023-05-25 18:23:00.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/lib/managers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1396 2023-05-17 00:58:35.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/lib/signal_events.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      412 2023-05-13 17:53:49.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/lib/signals.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      916 2023-06-19 17:31:05.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/lib/utils.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-19 01:06:15.573109 zibanu-django-auth-1.0.4/zibanu/django/auth/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-19 01:06:15.573109 zibanu-django-auth-1.0.4/zibanu/django/auth/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-19 01:06:15.578109 zibanu-django-auth-1.0.4/zibanu/django/auth/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2258 2023-07-19 01:02:40.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3286 2023-07-19 01:02:29.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-19 01:06:15.579109 zibanu-django-auth-1.0.4/zibanu/django/auth/migrations/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    24474 2023-04-11 22:39:55.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/migrations/0001_initial.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    23351 2023-07-05 13:34:24.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/migrations/0002_alter_userprofile_timezone.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      443 2023-07-19 00:48:43.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/migrations/0003_userprofile_multiple_login.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      313 2023-04-10 19:31:28.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/migrations/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2676 2023-07-19 00:45:47.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/models.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-19 01:06:15.581108 zibanu-django-auth-1.0.4/zibanu/django/auth/templates/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      487 2023-05-23 16:11:28.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/templates/change_password.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      324 2023-05-22 17:32:26.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/templates/change_password.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      123 2023-05-13 16:44:16.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/templates/request-code.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2023-05-13 16:41:48.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/templates/request-code.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      559 2023-05-22 17:30:07.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/templates/request_password.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      346 2023-05-13 16:55:01.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/templates/request_password.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1701 2023-06-19 20:28:16.000000 zibanu-django-auth-1.0.4/zibanu/django/auth/urls.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-07-19 01:06:15.582108 zibanu-django-auth-1.0.4/zibanu_django_auth.egg-info/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    41404 2023-07-19 01:06:15.000000 zibanu-django-auth-1.0.4/zibanu_django_auth.egg-info/PKG-INFO
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1730 2023-07-19 01:06:15.000000 zibanu-django-auth-1.0.4/zibanu_django_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-07-19 01:06:15.000000 zibanu-django-auth-1.0.4/zibanu_django_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      105 2023-07-19 01:06:15.000000 zibanu-django-auth-1.0.4/zibanu_django_auth.egg-info/requires.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2023-07-19 01:06:15.000000 zibanu-django-auth-1.0.4/zibanu_django_auth.egg-info/top_level.txt
```

### Comparing `zibanu-django-auth-1.0.3/LICENSE` & `zibanu-django-auth-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.3/PKG-INFO` & `zibanu-django-auth-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibanu-django-auth
-Version: 1.0.3
+Version: 1.0.4
 Summary: Zibanu authentication library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `zibanu-django-auth-1.0.3/pyproject.toml` & `zibanu-django-auth-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel",
 ]
 build-backend="setuptools.build_meta"
 
 [project]
 name = "zibanu-django-auth"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
     {name="Mario Cerón", email="mario.ceron@cqinversiones.co"}
 ]
 description = "Zibanu authentication library for django projects"
 readme = "README.md"
 license = {file="LICENSE"}
 requires-python = ">=3.9"
```

### Comparing `zibanu-django-auth-1.0.3/zibanu/django/auth/api/serializers/__init__.py` & `zibanu-django-auth-1.0.4/zibanu/django/auth/api/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.3/zibanu/django/auth/api/serializers/group.py` & `zibanu-django-auth-1.0.4/zibanu/django/auth/api/serializers/group.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.3/zibanu/django/auth/api/serializers/permission.py` & `zibanu-django-auth-1.0.4/zibanu/django/auth/api/serializers/permission.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.3/zibanu/django/auth/api/serializers/profile.py` & `zibanu-django-auth-1.0.4/zibanu/django/auth/api/serializers/profile.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,8 +18,8 @@
     """
 
     class Meta:
         """
         Profile Serializer Meta Class
         """
         model = UserProfile
-        fields = ("timezone", "theme", "lang", "avatar", "messages_timeout", "keep_logged_in", "app_profile")
+        fields = ("timezone", "theme", "lang", "avatar", "messages_timeout", "keep_logged_in", "app_profile", "multiple_login")
```

### Comparing `zibanu-django-auth-1.0.3/zibanu/django/auth/api/serializers/token.py` & `zibanu-django-auth-1.0.4/zibanu/django/auth/api/serializers/token.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.3/zibanu/django/auth/api/serializers/user.py` & `zibanu-django-auth-1.0.4/zibanu/django/auth/api/serializers/user.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.3/zibanu/django/auth/api/services/__init__.py` & `zibanu-django-auth-1.0.4/zibanu/django/auth/api/services/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.3/zibanu/django/auth/api/services/group.py` & `zibanu-django-auth-1.0.4/zibanu/django/auth/api/services/group.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.3/zibanu/django/auth/api/services/permission.py` & `zibanu-django-auth-1.0.4/zibanu/django/auth/api/services/permission.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.3/zibanu/django/auth/api/services/profile.py` & `zibanu-django-auth-1.0.4/zibanu/django/auth/api/services/profile.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.3/zibanu/django/auth/api/services/user.py` & `zibanu-django-auth-1.0.4/zibanu/django/auth/api/services/user.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.3/zibanu/django/auth/apps.py` & `zibanu-django-auth-1.0.4/zibanu/django/auth/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.3/zibanu/django/auth/lib/signal_events.py` & `zibanu-django-auth-1.0.4/zibanu/django/auth/lib/signal_events.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.3/zibanu/django/auth/lib/utils.py` & `zibanu-django-auth-1.0.4/zibanu/django/auth/lib/utils.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.3/zibanu/django/auth/locale/es/LC_MESSAGES/django.mo` & `zibanu-django-auth-1.0.4/zibanu/django/auth/locale/es/LC_MESSAGES/django.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,14 +7,17 @@
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
+msgid "Allow multiple login"
+msgstr "Permite acceso múltiple"
+
 msgid "Avatar"
 msgstr "Avatar"
 
 msgid "Cannot delete yourself."
 msgstr "No se puede eliminar a si mismo."
 
 msgid "Custom Application Profile"
```

### Comparing `zibanu-django-auth-1.0.3/zibanu/django/auth/locale/es/LC_MESSAGES/django.po` & `zibanu-django-auth-1.0.4/zibanu/django/auth/locale/es/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-19 15:39-0500\n"
+"POT-Creation-Date: 2023-07-18 20:02-0500\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -22,43 +22,43 @@
 msgid "The password is required."
 msgstr "La clave es obligatoria."
 
 #: api/serializers/user.py:81
 msgid "Email is already registered in our database."
 msgstr "El correo ya se encuentra registrado con nosotros."
 
-#: api/services/user.py:165
+#: api/services/user.py:166
 msgid "User does not exists."
 msgstr "El usuario no existe."
 
-#: api/services/user.py:190
+#: api/services/user.py:191
 msgid "Cannot delete yourself."
 msgstr "No se puede eliminar a si mismo."
 
-#: api/services/user.py:197
+#: api/services/user.py:198
 msgid "User has protected child records. Cannot delete."
 msgstr "El usuario tiene registros dependientes. No se puede eliminar."
 
-#: api/services/user.py:226
+#: api/services/user.py:227
 msgid "Password change"
 msgstr "Cambio de clave"
 
-#: api/services/user.py:229
+#: api/services/user.py:230
 msgid "Old password does not match."
 msgstr "La clave antigua no coincide."
 
-#: api/services/user.py:231
+#: api/services/user.py:232
 msgid "Old/New password are required."
 msgstr "Se requiere la clave antigua y la nueva."
 
-#: api/services/user.py:261
+#: api/services/user.py:262
 msgid "Request password."
 msgstr "Solicitar clave."
 
-#: api/services/user.py:264
+#: api/services/user.py:265
 msgid "Email is not registered."
 msgstr "El correo no está registrado con nosotros."
 
 #: apps.py:20
 msgid "Zibanu Auth for Django"
 msgstr "Autenticación Zibanu Django"
 
@@ -83,14 +83,18 @@
 msgstr "Tiempo de espera de mensajes"
 
 #: models.py:27
 msgid "Keep Logged In"
 msgstr "Mantener sesión abierta"
 
 #: models.py:28
+msgid "Allow multiple login"
+msgstr "Permite acceso múltiple"
+
+#: models.py:29
 msgid "Custom Application Profile"
 msgstr "Perfil de aplicación"
 
 #: templates/change_password.html:8 templates/change_password.txt:2
 #: templates/request_password.html:8 templates/request_password.txt:2
 msgid "Hello"
 msgstr "Hola"
@@ -101,13 +105,14 @@
 
 #: templates/change_password.html:13 templates/change_password.txt:7
 #: templates/request_password.html:15 templates/request_password.txt:9
 #, python-format
 msgid ""
 "This email was generated automatically at %(email_datetime)s with id "
 "%(email_id)s. Please do not answer it."
-msgstr "Este correo ha sido generado automaticamente a las %(email_datetime)s con el id "
-"%(email_id)s. Por favor no lo responda."
+msgstr ""
+"Este correo ha sido generado automaticamente a las %(email_datetime)s con el "
+"id %(email_id)s. Por favor no lo responda."
 
 #: templates/request_password.html:9 templates/request_password.txt:4
 msgid "The system has generated a new password for you:"
 msgstr "El sistema ha generado un nuevo password para usted:"
```

### Comparing `zibanu-django-auth-1.0.3/zibanu/django/auth/migrations/0001_initial.py` & `zibanu-django-auth-1.0.4/zibanu/django/auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.3/zibanu/django/auth/migrations/0002_alter_userprofile_timezone.py` & `zibanu-django-auth-1.0.4/zibanu/django/auth/migrations/0002_alter_userprofile_timezone.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.3/zibanu/django/auth/models.py` & `zibanu-django-auth-1.0.4/zibanu/django/auth/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,23 +21,38 @@
     timezone = models.CharField(max_length=50, null=False, blank=False, default="UTC",
                                 choices=ALL_TIMEZONES_CHOICES, verbose_name=_("Time Zone"))
     theme = models.CharField(max_length=50, null=True, blank=False, verbose_name=_("User Theme"))
     lang = models.CharField(max_length=3, null=False, blank=False, default="en", verbose_name=_("Language"))
     avatar = models.BinaryField(null=True, blank=False, verbose_name=_("Avatar"))
     messages_timeout = models.IntegerField(default=10, null=False, blank=False, verbose_name=_("Message's Timeout"))
     keep_logged_in = models.BooleanField(default=False, null=False, blank=False, verbose_name=_("Keep Logged In"))
+    multiple_login = models.BooleanField(default=False, null=False, blank=False, verbose_name=_("Allow multiple login"))
     app_profile = models.JSONField(null=True, blank=False, verbose_name=_("Custom Application Profile"))
 
     def set(self, fields: dict):
         """
         Change field values from a field dict list
         :param fields: dictionary with key, value for field
         :return: None
         """
         for key, value in fields.items():
             if hasattr(self, key):
                 setattr(self, key, value)
             self.save(force_update=True)
 
+    def save(self, force_insert=False, force_update=False, using=None, update_fields=None):
+        """
+        Override save method to force set multiple_login to False if is_staff is False
+        :param force_insert: Flag to force insert at save
+        :param force_update: Flat to force update at save
+        :param using: Using db name at settings
+        :param update_fields: Fields to be updated
+        :return: None
+        """
+        if not self.user.is_staff:
+            self.multiple_login = False
+        return super().save(force_insert=force_insert, force_update=force_update, using=using, update_fields=update_fields)
+
+
 
     class Meta:
         db_table = "zb_auth_user_profile"
```

### Comparing `zibanu-django-auth-1.0.3/zibanu/django/auth/templates/request_password.html` & `zibanu-django-auth-1.0.4/zibanu/django/auth/templates/request_password.html`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.3/zibanu/django/auth/urls.py` & `zibanu-django-auth-1.0.4/zibanu/django/auth/urls.py`

 * *Files identical despite different names*

### Comparing `zibanu-django-auth-1.0.3/zibanu_django_auth.egg-info/PKG-INFO` & `zibanu-django-auth-1.0.4/zibanu_django_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibanu-django-auth
-Version: 1.0.3
+Version: 1.0.4
 Summary: Zibanu authentication library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `zibanu-django-auth-1.0.3/zibanu_django_auth.egg-info/SOURCES.txt` & `zibanu-django-auth-1.0.4/zibanu_django_auth.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 zibanu/django/auth/lib/utils.py
 zibanu/django/auth/lib/choices/__init__.py
 zibanu/django/auth/lib/managers/__init__.py
 zibanu/django/auth/locale/es/LC_MESSAGES/django.mo
 zibanu/django/auth/locale/es/LC_MESSAGES/django.po
 zibanu/django/auth/migrations/0001_initial.py
 zibanu/django/auth/migrations/0002_alter_userprofile_timezone.py
+zibanu/django/auth/migrations/0003_userprofile_multiple_login.py
 zibanu/django/auth/migrations/__init__.py
 zibanu/django/auth/templates/change_password.html
 zibanu/django/auth/templates/change_password.txt
 zibanu/django/auth/templates/request-code.html
 zibanu/django/auth/templates/request-code.txt
 zibanu/django/auth/templates/request_password.html
 zibanu/django/auth/templates/request_password.txt
```

