# Comparing `tmp/caldav-1.2.1.tar.gz` & `tmp/caldav-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caldav-1.2.1.tar", last modified: Thu May 11 21:25:32 2023, max compression
+gzip compressed data, was "caldav-1.3.2.tar", last modified: Wed Jul 19 13:08:55 2023, max compression
```

## Comparing `caldav-1.2.1.tar` & `caldav-1.3.2.tar`

### file list

```diff
@@ -1,95 +1,110 @@
-drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-05-11 21:25:32.703773 caldav-1.2.1/
--rw-r--r--   0 tobias    (7385) tobias    (7385)    11358 2019-09-10 16:18:00.000000 caldav-1.2.1/COPYING.APACHE
--rw-r--r--   0 tobias    (7385) tobias    (7385)    35147 2019-09-10 16:18:00.000000 caldav-1.2.1/COPYING.GPL
--rw-r--r--   0 tobias    (7385) tobias    (7385)       87 2021-10-10 17:58:14.000000 caldav-1.2.1/MANIFEST.in
--rw-r--r--   0 tobias    (7385) tobias    (7385)     1354 2023-05-11 21:25:32.703773 caldav-1.2.1/PKG-INFO
--rw-r--r--   0 tobias    (7385) tobias    (7385)      635 2021-10-10 17:58:14.000000 caldav-1.2.1/README.md
-drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-05-11 21:25:32.690440 caldav-1.2.1/caldav/
--rw-r--r--   0 tobias    (7385) tobias    (7385)      543 2023-05-11 21:24:22.000000 caldav-1.2.1/caldav/__init__.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)    24907 2023-05-11 21:24:22.000000 caldav-1.2.1/caldav/davclient.py
-drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-05-11 21:25:32.693773 caldav-1.2.1/caldav/elements/
--rw-r--r--   0 tobias    (7385) tobias    (7385)       48 2022-11-21 19:16:34.000000 caldav-1.2.1/caldav/elements/__init__.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     1945 2023-05-11 21:20:36.000000 caldav-1.2.1/caldav/elements/base.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     4935 2022-11-21 19:16:34.000000 caldav-1.2.1/caldav/elements/cdav.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     1609 2022-11-21 19:16:34.000000 caldav-1.2.1/caldav/elements/dav.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)      319 2022-11-21 19:16:34.000000 caldav-1.2.1/caldav/elements/ical.py
-drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-05-11 21:25:32.693773 caldav-1.2.1/caldav/lib/
--rw-r--r--   0 tobias    (7385) tobias    (7385)        0 2019-09-10 16:18:00.000000 caldav-1.2.1/caldav/lib/__init__.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)      231 2023-05-11 21:20:36.000000 caldav-1.2.1/caldav/lib/debug.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     2540 2023-05-11 21:20:36.000000 caldav-1.2.1/caldav/lib/error.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)      668 2022-11-21 19:16:34.000000 caldav-1.2.1/caldav/lib/namespace.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)      798 2023-05-11 21:20:36.000000 caldav-1.2.1/caldav/lib/python_utilities.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     6480 2023-05-11 21:20:36.000000 caldav-1.2.1/caldav/lib/url.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     7325 2023-05-11 21:24:22.000000 caldav-1.2.1/caldav/lib/vcal.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)   106210 2023-05-11 21:24:22.000000 caldav-1.2.1/caldav/objects.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)      402 2023-05-11 21:20:36.000000 caldav-1.2.1/caldav/requests.py
-drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-05-11 21:25:32.693773 caldav-1.2.1/caldav.egg-info/
--rw-r--r--   0 tobias    (7385) tobias    (7385)     1354 2023-05-11 21:25:32.000000 caldav-1.2.1/caldav.egg-info/PKG-INFO
--rw-r--r--   0 tobias    (7385) tobias    (7385)     3063 2023-05-11 21:25:32.000000 caldav-1.2.1/caldav.egg-info/SOURCES.txt
--rw-r--r--   0 tobias    (7385) tobias    (7385)        1 2023-05-11 21:25:32.000000 caldav-1.2.1/caldav.egg-info/dependency_links.txt
--rw-r--r--   0 tobias    (7385) tobias    (7385)        1 2022-11-22 09:14:37.000000 caldav-1.2.1/caldav.egg-info/not-zip-safe
--rw-r--r--   0 tobias    (7385) tobias    (7385)      155 2023-05-11 21:25:32.000000 caldav-1.2.1/caldav.egg-info/requires.txt
--rw-r--r--   0 tobias    (7385) tobias    (7385)        7 2023-05-11 21:25:32.000000 caldav-1.2.1/caldav.egg-info/top_level.txt
--rw-r--r--   0 tobias    (7385) tobias    (7385)      480 2023-05-11 21:25:32.703773 caldav-1.2.1/setup.cfg
--rwxr-xr-x   0 tobias    (7385) tobias    (7385)     2994 2023-05-11 21:20:36.000000 caldav-1.2.1/setup.py
-drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-05-11 21:25:32.697106 caldav-1.2.1/tests/
--rw-r--r--   0 tobias    (7385) tobias    (7385)    98473 2023-05-03 21:25:23.000000 caldav-1.2.1/tests/#test_caldav.py#
--rwxr-xr-x   0 tobias    (7385) tobias    (7385)      888 2022-11-03 16:22:35.000000 caldav-1.2.1/tests/#tmp_226.py#
--rw-r--r--   0 tobias    (7385) tobias    (7385)        0 2019-09-10 16:18:00.000000 caldav-1.2.1/tests/__init__.py
-drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-05-11 21:25:32.703773 caldav-1.2.1/tests/__pycache__/
--rw-r--r--   0 tobias    (7385) tobias    (7385)      130 2022-01-05 17:28:37.000000 caldav-1.2.1/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)      128 2021-10-10 21:24:31.000000 caldav-1.2.1/tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     7969 2023-02-25 18:55:46.000000 caldav-1.2.1/tests/__pycache__/compatibility_issues.cpython-310.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     4188 2021-11-10 00:21:31.000000 caldav-1.2.1/tests/__pycache__/compatibility_issues.cpython-39.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     2401 2023-02-14 21:14:51.000000 caldav-1.2.1/tests/__pycache__/conf.cpython-310.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     1788 2021-10-10 21:24:45.000000 caldav-1.2.1/tests/__pycache__/conf.cpython-39.pyc
--rw-------   0 tobias    (7385) tobias    (7385)     2949 2023-03-06 14:30:08.000000 caldav-1.2.1/tests/__pycache__/conf_private.cpython-310.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)      709 2021-11-30 09:55:30.000000 caldav-1.2.1/tests/__pycache__/conf_private.cpython-39.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    10615 2023-02-27 20:25:36.000000 caldav-1.2.1/tests/__pycache__/proxy.cpython-310.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    10615 2021-10-10 21:24:45.000000 caldav-1.2.1/tests/__pycache__/proxy.cpython-39.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    99664 2022-11-01 22:32:56.000000 caldav-1.2.1/tests/__pycache__/test_caldav.cpython-310-pytest-7.1.3.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)   108125 2023-01-15 22:21:23.000000 caldav-1.2.1/tests/__pycache__/test_caldav.cpython-310-pytest-7.2.0.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)   115157 2023-03-06 14:51:44.000000 caldav-1.2.1/tests/__pycache__/test_caldav.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)   115163 2023-03-13 07:21:44.000000 caldav-1.2.1/tests/__pycache__/test_caldav.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    55936 2023-03-06 14:15:55.000000 caldav-1.2.1/tests/__pycache__/test_caldav.cpython-310.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    41792 2021-12-02 18:17:39.000000 caldav-1.2.1/tests/__pycache__/test_caldav.cpython-39.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    61467 2022-11-01 22:32:56.000000 caldav-1.2.1/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.1.3.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    62010 2023-01-15 22:21:23.000000 caldav-1.2.1/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.0.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    63615 2023-02-27 20:25:36.000000 caldav-1.2.1/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    63618 2023-03-13 07:21:45.000000 caldav-1.2.1/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    33628 2023-03-06 14:13:09.000000 caldav-1.2.1/tests/__pycache__/test_caldav_unit.cpython-310.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    26186 2021-10-10 21:24:31.000000 caldav-1.2.1/tests/__pycache__/test_caldav_unit.cpython-39.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     4379 2022-10-04 22:09:32.000000 caldav-1.2.1/tests/__pycache__/test_cdav.cpython-310-pytest-7.1.3.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     4379 2022-11-21 19:20:28.000000 caldav-1.2.1/tests/__pycache__/test_cdav.cpython-310-pytest-7.2.0.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     4379 2023-01-16 00:55:21.000000 caldav-1.2.1/tests/__pycache__/test_cdav.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     4379 2023-03-13 07:21:45.000000 caldav-1.2.1/tests/__pycache__/test_cdav.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     2057 2023-03-06 14:13:09.000000 caldav-1.2.1/tests/__pycache__/test_cdav.cpython-310.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     2029 2021-10-10 21:24:31.000000 caldav-1.2.1/tests/__pycache__/test_cdav.cpython-39.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)      793 2022-10-04 22:09:32.000000 caldav-1.2.1/tests/__pycache__/test_utils.cpython-310-pytest-7.1.3.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)      793 2022-11-21 19:20:28.000000 caldav-1.2.1/tests/__pycache__/test_utils.cpython-310-pytest-7.2.0.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)      793 2023-01-16 00:55:21.000000 caldav-1.2.1/tests/__pycache__/test_utils.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)      793 2023-03-13 07:21:45.000000 caldav-1.2.1/tests/__pycache__/test_utils.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)      684 2023-03-06 14:13:09.000000 caldav-1.2.1/tests/__pycache__/test_utils.cpython-310.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     3372 2022-10-04 22:09:32.000000 caldav-1.2.1/tests/__pycache__/test_vcal.cpython-310-pytest-7.1.3.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     7304 2023-01-15 22:21:23.000000 caldav-1.2.1/tests/__pycache__/test_vcal.cpython-310-pytest-7.2.0.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     7304 2023-02-11 09:38:03.000000 caldav-1.2.1/tests/__pycache__/test_vcal.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     8024 2023-03-13 07:21:45.000000 caldav-1.2.1/tests/__pycache__/test_vcal.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     5975 2023-03-06 14:13:09.000000 caldav-1.2.1/tests/__pycache__/test_vcal.cpython-310.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     2650 2021-11-30 08:41:46.000000 caldav-1.2.1/tests/__pycache__/test_vcal.cpython-39.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     1290 2022-11-21 19:16:34.000000 caldav-1.2.1/tests/_test_absolute.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)    14105 2023-05-11 21:20:36.000000 caldav-1.2.1/tests/compatibility_issues.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     4909 2023-05-11 21:20:36.000000 caldav-1.2.1/tests/conf.py
--rw-------   0 tobias    (7385) tobias    (7385)     8448 2023-03-06 14:30:03.000000 caldav-1.2.1/tests/conf_private.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     3119 2022-05-09 07:22:01.000000 caldav-1.2.1/tests/conf_private.py.EXAMPLE
--rw-------   0 tobias    (7385) tobias    (7385)     8446 2023-02-16 09:36:29.000000 caldav-1.2.1/tests/conf_private.py~
--rw-r--r--   0 tobias    (7385) tobias    (7385)    11408 2023-05-11 21:20:36.000000 caldav-1.2.1/tests/proxy.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)    97997 2023-05-11 21:24:22.000000 caldav-1.2.1/tests/test_caldav.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)    97373 2023-02-16 21:52:31.000000 caldav-1.2.1/tests/test_caldav.py.orig
--rw-r--r--   0 tobias    (7385) tobias    (7385)      543 2023-02-14 23:21:07.000000 caldav-1.2.1/tests/test_caldav.py.rej
--rw-r--r--   0 tobias    (7385) tobias    (7385)    42187 2023-05-11 21:20:36.000000 caldav-1.2.1/tests/test_caldav_unit.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     1965 2022-11-21 19:16:34.000000 caldav-1.2.1/tests/test_cdav.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)      517 2022-11-21 19:16:34.000000 caldav-1.2.1/tests/test_utils.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)      487 2022-01-07 16:03:24.000000 caldav-1.2.1/tests/test_utils.py~
--rw-r--r--   0 tobias    (7385) tobias    (7385)     7568 2023-05-11 21:20:36.000000 caldav-1.2.1/tests/test_vcal.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)       54 2021-11-26 23:08:18.000000 caldav-1.2.1/tests/test_vcal.py~
--rw-r--r--   0 tobias    (7385) tobias    (7385)      906 2022-11-02 08:07:32.000000 caldav-1.2.1/tests/tmp_226~
+drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-19 13:08:55.442054 caldav-1.3.2/
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    11358 2019-09-10 16:18:00.000000 caldav-1.3.2/COPYING.APACHE
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    35147 2019-09-10 16:18:00.000000 caldav-1.3.2/COPYING.GPL
+-rw-r--r--   0 tobias    (7385) tobias    (7385)       87 2023-05-22 07:00:24.000000 caldav-1.3.2/MANIFEST.in
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     1354 2023-07-19 13:08:55.442054 caldav-1.3.2/PKG-INFO
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      635 2023-05-22 07:00:24.000000 caldav-1.3.2/README.md
+drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-19 13:08:55.428721 caldav-1.3.2/caldav/
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      543 2023-07-19 13:07:21.000000 caldav-1.3.2/caldav/__init__.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    25502 2023-07-18 22:32:35.000000 caldav-1.3.2/caldav/davclient.py
+drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-19 13:08:55.432054 caldav-1.3.2/caldav/elements/
+-rw-r--r--   0 tobias    (7385) tobias    (7385)       48 2023-05-22 07:00:24.000000 caldav-1.3.2/caldav/elements/__init__.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     1945 2023-07-18 22:32:35.000000 caldav-1.3.2/caldav/elements/base.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     4935 2023-05-22 07:00:24.000000 caldav-1.3.2/caldav/elements/cdav.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     1609 2023-05-22 07:00:24.000000 caldav-1.3.2/caldav/elements/dav.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      319 2023-05-22 07:00:24.000000 caldav-1.3.2/caldav/elements/ical.py
+drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-19 13:08:55.432054 caldav-1.3.2/caldav/lib/
+-rw-r--r--   0 tobias    (7385) tobias    (7385)        0 2019-09-10 16:18:00.000000 caldav-1.3.2/caldav/lib/__init__.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      231 2023-07-18 22:45:26.000000 caldav-1.3.2/caldav/lib/debug.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     2540 2023-07-18 22:01:33.000000 caldav-1.3.2/caldav/lib/error.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      668 2023-05-22 07:00:24.000000 caldav-1.3.2/caldav/lib/namespace.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      798 2023-07-18 22:32:35.000000 caldav-1.3.2/caldav/lib/python_utilities.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     6480 2023-07-18 22:32:35.000000 caldav-1.3.2/caldav/lib/url.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     7450 2023-07-18 22:32:35.000000 caldav-1.3.2/caldav/lib/vcal.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)   109108 2023-07-19 13:05:08.000000 caldav-1.3.2/caldav/objects.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      402 2023-05-22 07:00:24.000000 caldav-1.3.2/caldav/requests.py
+drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-19 13:08:55.432054 caldav-1.3.2/caldav.egg-info/
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     1354 2023-07-19 13:08:55.000000 caldav-1.3.2/caldav.egg-info/PKG-INFO
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     3878 2023-07-19 13:08:55.000000 caldav-1.3.2/caldav.egg-info/SOURCES.txt
+-rw-r--r--   0 tobias    (7385) tobias    (7385)        1 2023-07-19 13:08:55.000000 caldav-1.3.2/caldav.egg-info/dependency_links.txt
+-rw-r--r--   0 tobias    (7385) tobias    (7385)        1 2022-11-22 09:14:37.000000 caldav-1.3.2/caldav.egg-info/not-zip-safe
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      130 2023-07-19 13:08:55.000000 caldav-1.3.2/caldav.egg-info/requires.txt
+-rw-r--r--   0 tobias    (7385) tobias    (7385)        7 2023-07-19 13:08:55.000000 caldav-1.3.2/caldav.egg-info/top_level.txt
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      506 2023-07-19 13:08:55.445388 caldav-1.3.2/setup.cfg
+-rwxr-xr-x   0 tobias    (7385) tobias    (7385)     2877 2023-07-18 22:32:35.000000 caldav-1.3.2/setup.py
+drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-19 13:08:55.435388 caldav-1.3.2/tests/
+-rw-------   0 tobias    (7385) tobias    (7385)     8630 2023-05-25 19:43:46.000000 caldav-1.3.2/tests/#conf_private.py#
+-rwxr-xr-x   0 tobias    (7385) tobias    (7385)      888 2022-11-03 16:22:35.000000 caldav-1.3.2/tests/#tmp_226.py#
+-rw-r--r--   0 tobias    (7385) tobias    (7385)        0 2019-09-10 16:18:00.000000 caldav-1.3.2/tests/__init__.py
+drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-19 13:08:55.442054 caldav-1.3.2/tests/__pycache__/
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      130 2022-01-05 17:28:37.000000 caldav-1.3.2/tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      146 2023-05-22 06:28:45.000000 caldav-1.3.2/tests/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      128 2021-10-10 21:24:31.000000 caldav-1.3.2/tests/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     7969 2023-02-25 18:55:46.000000 caldav-1.3.2/tests/__pycache__/compatibility_issues.cpython-310.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     8694 2023-07-19 10:22:04.000000 caldav-1.3.2/tests/__pycache__/compatibility_issues.cpython-311.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     4188 2021-11-10 00:21:31.000000 caldav-1.3.2/tests/__pycache__/compatibility_issues.cpython-39.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     2401 2023-02-14 21:14:51.000000 caldav-1.3.2/tests/__pycache__/conf.cpython-310.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     3722 2023-05-24 11:30:31.000000 caldav-1.3.2/tests/__pycache__/conf.cpython-311.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     1788 2021-10-10 21:24:45.000000 caldav-1.3.2/tests/__pycache__/conf.cpython-39.pyc
+-rw-------   0 tobias    (7385) tobias    (7385)     2949 2023-03-06 14:30:08.000000 caldav-1.3.2/tests/__pycache__/conf_private.cpython-310.pyc
+-rw-------   0 tobias    (7385) tobias    (7385)     3638 2023-07-18 16:05:33.000000 caldav-1.3.2/tests/__pycache__/conf_private.cpython-311.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      709 2021-11-30 09:55:30.000000 caldav-1.3.2/tests/__pycache__/conf_private.cpython-39.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    10615 2023-02-27 20:25:36.000000 caldav-1.3.2/tests/__pycache__/proxy.cpython-310.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    19912 2023-07-19 10:22:04.000000 caldav-1.3.2/tests/__pycache__/proxy.cpython-311.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    10615 2021-10-10 21:24:45.000000 caldav-1.3.2/tests/__pycache__/proxy.cpython-39.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    99664 2022-11-01 22:32:56.000000 caldav-1.3.2/tests/__pycache__/test_caldav.cpython-310-pytest-7.1.3.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)   108125 2023-01-15 22:21:23.000000 caldav-1.3.2/tests/__pycache__/test_caldav.cpython-310-pytest-7.2.0.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)   115157 2023-03-06 14:51:44.000000 caldav-1.3.2/tests/__pycache__/test_caldav.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)   115163 2023-03-13 07:21:44.000000 caldav-1.3.2/tests/__pycache__/test_caldav.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    55936 2023-03-06 14:15:55.000000 caldav-1.3.2/tests/__pycache__/test_caldav.cpython-310.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)   346344 2023-05-24 11:30:31.000000 caldav-1.3.2/tests/__pycache__/test_caldav.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)   353122 2023-07-19 10:22:03.000000 caldav-1.3.2/tests/__pycache__/test_caldav.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    41792 2021-12-02 18:17:39.000000 caldav-1.3.2/tests/__pycache__/test_caldav.cpython-39.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    61467 2022-11-01 22:32:56.000000 caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.1.3.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    62010 2023-01-15 22:21:23.000000 caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.0.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    63615 2023-02-27 20:25:36.000000 caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    63618 2023-03-13 07:21:45.000000 caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    33628 2023-03-06 14:13:09.000000 caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-310.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)   160045 2023-05-24 11:30:31.000000 caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)   160045 2023-07-19 10:22:04.000000 caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    26186 2021-10-10 21:24:31.000000 caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-39.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     4379 2022-10-04 22:09:32.000000 caldav-1.3.2/tests/__pycache__/test_cdav.cpython-310-pytest-7.1.3.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     4379 2022-11-21 19:20:28.000000 caldav-1.3.2/tests/__pycache__/test_cdav.cpython-310-pytest-7.2.0.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     4379 2023-01-16 00:55:21.000000 caldav-1.3.2/tests/__pycache__/test_cdav.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     4379 2023-03-13 07:21:45.000000 caldav-1.3.2/tests/__pycache__/test_cdav.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     2057 2023-03-06 14:13:09.000000 caldav-1.3.2/tests/__pycache__/test_cdav.cpython-310.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    10956 2023-05-24 11:30:31.000000 caldav-1.3.2/tests/__pycache__/test_cdav.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    10956 2023-07-10 18:48:32.000000 caldav-1.3.2/tests/__pycache__/test_cdav.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     2029 2021-10-10 21:24:31.000000 caldav-1.3.2/tests/__pycache__/test_cdav.cpython-39.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      793 2022-10-04 22:09:32.000000 caldav-1.3.2/tests/__pycache__/test_utils.cpython-310-pytest-7.1.3.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      793 2022-11-21 19:20:28.000000 caldav-1.3.2/tests/__pycache__/test_utils.cpython-310-pytest-7.2.0.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      793 2023-01-16 00:55:21.000000 caldav-1.3.2/tests/__pycache__/test_utils.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      793 2023-03-13 07:21:45.000000 caldav-1.3.2/tests/__pycache__/test_utils.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      684 2023-03-06 14:13:09.000000 caldav-1.3.2/tests/__pycache__/test_utils.cpython-310.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     1527 2023-05-24 11:30:31.000000 caldav-1.3.2/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     1527 2023-07-10 18:48:32.000000 caldav-1.3.2/tests/__pycache__/test_utils.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     3372 2022-10-04 22:09:32.000000 caldav-1.3.2/tests/__pycache__/test_vcal.cpython-310-pytest-7.1.3.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     7304 2023-01-15 22:21:23.000000 caldav-1.3.2/tests/__pycache__/test_vcal.cpython-310-pytest-7.2.0.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     7304 2023-02-11 09:38:03.000000 caldav-1.3.2/tests/__pycache__/test_vcal.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     8024 2023-03-13 07:21:45.000000 caldav-1.3.2/tests/__pycache__/test_vcal.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     5975 2023-03-06 14:13:09.000000 caldav-1.3.2/tests/__pycache__/test_vcal.cpython-310.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    15151 2023-05-24 11:30:31.000000 caldav-1.3.2/tests/__pycache__/test_vcal.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    15151 2023-07-19 10:22:04.000000 caldav-1.3.2/tests/__pycache__/test_vcal.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     2650 2021-11-30 08:41:46.000000 caldav-1.3.2/tests/__pycache__/test_vcal.cpython-39.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     1290 2023-05-22 07:00:24.000000 caldav-1.3.2/tests/_test_absolute.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    14105 2023-07-18 22:32:35.000000 caldav-1.3.2/tests/compatibility_issues.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     4909 2023-05-22 07:00:24.000000 caldav-1.3.2/tests/conf.py
+-rw-------   0 tobias    (7385) tobias    (7385)     8630 2023-07-18 16:05:31.000000 caldav-1.3.2/tests/conf_private.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     3119 2023-05-22 07:00:24.000000 caldav-1.3.2/tests/conf_private.py.EXAMPLE
+-rw-------   0 tobias    (7385) tobias    (7385)     8629 2023-05-24 23:13:12.000000 caldav-1.3.2/tests/conf_private.py~
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    11408 2023-07-18 22:32:35.000000 caldav-1.3.2/tests/proxy.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    98646 2023-07-18 22:32:35.000000 caldav-1.3.2/tests/test_caldav.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    97373 2023-02-16 21:52:31.000000 caldav-1.3.2/tests/test_caldav.py.orig
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      543 2023-02-14 23:21:07.000000 caldav-1.3.2/tests/test_caldav.py.rej
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    45062 2023-07-18 22:32:35.000000 caldav-1.3.2/tests/test_caldav_unit.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     1965 2023-05-22 07:00:24.000000 caldav-1.3.2/tests/test_cdav.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      517 2023-05-22 07:00:24.000000 caldav-1.3.2/tests/test_utils.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      487 2022-01-07 16:03:24.000000 caldav-1.3.2/tests/test_utils.py~
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     7959 2023-07-18 22:32:35.000000 caldav-1.3.2/tests/test_vcal.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)       54 2021-11-26 23:08:18.000000 caldav-1.3.2/tests/test_vcal.py~
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      906 2022-11-02 08:07:32.000000 caldav-1.3.2/tests/tmp_226~
```

### Comparing `caldav-1.2.1/COPYING.APACHE` & `caldav-1.3.2/COPYING.APACHE`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/COPYING.GPL` & `caldav-1.3.2/COPYING.GPL`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/PKG-INFO` & `caldav-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caldav
-Version: 1.2.1
+Version: 1.3.2
 Summary: CalDAV (RFC4791) client library
 Home-page: https://github.com/python-caldav/caldav
 Author: Cyril Robert
 Author-email: cyril@hippie.io
 License: GPL
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `caldav-1.2.1/README.md` & `caldav-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/caldav/__init__.py` & `caldav-1.3.2/caldav/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 import logging
 
 import vobject.icalendar
 
-__version__ = "1.2.1"
+__version__ = "1.3.2"
 
 from .davclient import DAVClient
 from .objects import *
 
 ## Notes:
 ##
 ## * The vobject.icalendar has (or had?) to be explicitly imported due to some bug in the tBaxter fork of vobject.
```

### Comparing `caldav-1.2.1/caldav/davclient.py` & `caldav-1.3.2/caldav/davclient.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,21 +32,25 @@
     """
 
     raw = ""
     reason = ""
     tree = None
     headers = {}
     status = 0
+    davclient = None
+    huge_tree = False
 
-    def __init__(self, response):
+    def __init__(self, response, davclient=None):
         self.headers = response.headers
         log.debug("response headers: " + str(self.headers))
         log.debug("response status: " + str(self.status))
 
         self._raw = response.content
+        if davclient:
+            self.huge_tree = davclient.huge_tree
 
         ## TODO: this if/else/elif could possibly be refactored, or we should
         ## consider to do streaming into the xmltree library as originally
         ## intended.  It only makes sense for really huge payloads though.
         if self.headers.get("Content-Type", "").startswith(
             "text/xml"
         ) or self.headers.get("Content-Type", "").startswith("application/xml"):
@@ -61,20 +65,23 @@
             else:
                 ## With response.raw we could be streaming the content, but it does not work because
                 ## the stream often is compressed.  We could add uncompression on the fly, but not
                 ## considered worth the effort as for now.
                 # self.tree = etree.parse(response.raw, parser=etree.XMLParser(remove_blank_text=True))
                 try:
                     self.tree = etree.XML(
-                        self._raw, parser=etree.XMLParser(remove_blank_text=True)
+                        self._raw,
+                        parser=etree.XMLParser(
+                            remove_blank_text=True, huge_tree=self.huge_tree
+                        ),
                     )
                 except:
                     logging.critical(
                         "Expected some valid XML from the server, but got this: \n"
-                        + self._raw,
+                        + str(self._raw),
                         exc_info=True,
                     )
                     raise
                 if log.level <= logging.DEBUG:
                     log.debug(etree.tostring(self.tree, pretty_print=True))
         elif self.headers.get("Content-Type", "").startswith(
             "text/calendar"
@@ -88,15 +95,18 @@
             ## give text/html as the default when no content is
             ## delivered or on errors (ref
             ## https://github.com/python-caldav/caldav/issues/142).
             ## TODO: maybe just remove all of the code above in this if/else and let all
             ## data be parsed through this code.
             try:
                 self.tree = etree.XML(
-                    self._raw, parser=etree.XMLParser(remove_blank_text=True)
+                    self._raw,
+                    parser=etree.XMLParser(
+                        remove_blank_text=True, huge_tree=self.huge_tree
+                    ),
                 )
             except:
                 pass
 
         ## this if will always be true as for now, see other comments on streaming.
         if hasattr(self, "_raw"):
             log.debug(self._raw)
@@ -306,46 +316,50 @@
 
     Unless you have special needs, you should probably care most about
     the constructor (__init__), the principal method and the calendar method.
     """
 
     proxy = None
     url = None
+    huge_tree = False
 
     def __init__(
         self,
         url,
         proxy=None,
         username=None,
         password=None,
         auth=None,
         timeout=None,
         ssl_verify_cert=True,
         ssl_cert=None,
         headers={},
+        huge_tree=False,
     ):
         """
         Sets up a HTTPConnection object towards the server in the url.
         Parameters:
          * url: A fully qualified url: `scheme://user:pass@hostname:port`
          * proxy: A string defining a proxy server: `hostname:port`
          * username and password should be passed as arguments or in the URL
          * auth, timeout and ssl_verify_cert are passed to requests.request.
-         ** ssl_verify_cert can be the path of a CA-bundle or False.
+         * ssl_verify_cert can be the path of a CA-bundle or False.
+         * huge_tree: boolean, enable XMLParser huge_tree to handle big events, beware
+           of security issues, see : https://lxml.de/api/lxml.etree.XMLParser-class.html
 
         The requests library will honor a .netrc-file, if such a file exists
         username and password may be omitted.  Known bug: .netrc is honored
         even if a username/password is given, ref https://github.com/python-caldav/caldav/issues/206
         """
 
         self.session = requests.Session()
 
         log.debug("url: " + str(url))
         self.url = URL.objectify(url)
-
+        self.huge_tree = huge_tree
         # Prepare proxy info
         if proxy is not None:
             self.proxy = proxy
             # requests library expects the proxy url to have a scheme
             if re.match("^.*://", proxy) is None:
                 self.proxy = self.url.scheme + "://" + proxy
 
@@ -587,15 +601,15 @@
                 proxies=proxies,
                 auth=self.auth,
                 timeout=self.timeout,
                 verify=self.ssl_verify_cert,
                 cert=self.ssl_cert,
             )
             log.debug("server responded with %i %s" % (r.status_code, r.reason))
-            response = DAVResponse(r)
+            response = DAVResponse(r, self)
         except:
             ## this is a workaround needed due to some weird server
             ## that would just abort the connection rather than send a
             ## 401 when an unauthenticated request with a body was
             ## sent to the server - ref https://github.com/python-caldav/caldav/issues/158
             if self.auth or not self.password:
                 raise
```

### Comparing `caldav-1.2.1/caldav/elements/base.py` & `caldav-1.3.2/caldav/elements/base.py`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/caldav/elements/cdav.py` & `caldav-1.3.2/caldav/elements/cdav.py`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/caldav/elements/dav.py` & `caldav-1.3.2/caldav/elements/dav.py`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/caldav/lib/error.py` & `caldav-1.3.2/caldav/lib/error.py`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/caldav/lib/namespace.py` & `caldav-1.3.2/caldav/lib/namespace.py`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/caldav/lib/python_utilities.py` & `caldav-1.3.2/caldav/lib/python_utilities.py`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/caldav/lib/url.py` & `caldav-1.3.2/caldav/lib/url.py`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/caldav/lib/vcal.py` & `caldav-1.3.2/caldav/lib/vcal.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,15 +101,18 @@
         fixup_error_loggings += 1
         remove_bit = lambda n: n & (n - 1)
         if not remove_bit(fixup_error_loggings):
             log = logging.error
         else:
             log = logging.debug
         log(
-            "Ical data was modified to avoid compatibility issues.  (error count: %i - this error is ratelimited)"
+            """Ical data was modified to avoid compatibility issues
+(Your calendar server breaks the icalendar standard)
+This is probably harmless, particularly if not editing events or tasks
+(error count: %i - this error is ratelimited)"""
             % fixup_error_loggings,
             exc_info=True,
         )
         try:
             import difflib
 
             log(
@@ -169,15 +172,15 @@
             if isinstance(props[prop], datetime.datetime) and not props[prop].tzinfo:
                 ## We need to have a timezone!  Assume UTC.
                 props[prop] = props[prop].astimezone(datetime.timezone.utc)
             if prop in ("child", "parent"):
                 for value in props[prop]:
                     component.add(
                         "related-to",
-                        props[prop],
+                        str(value),
                         parameters={"reltype": prop.upper()},
                         encode=True,
                     )
             else:
                 component.add(prop, props[prop])
     ret = to_normal_str(my_instance.to_ical())
     if ical_fragment and ical_fragment.strip():
```

### Comparing `caldav-1.2.1/caldav/objects.py` & `caldav-1.3.2/caldav/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 (This file has become huge and will be split up prior to the next
 release.  I think it makes sense moving the CalendarObjectResource
 class hierarchy into a separate file)
 """
 import re
 import uuid
+from collections import defaultdict
 from datetime import date
 from datetime import datetime
 from datetime import timedelta
 from datetime import timezone
 
 import icalendar
 import vobject
@@ -67,15 +68,15 @@
         self,
         client=None,
         url=None,
         parent=None,
         name=None,
         id=None,
         props=None,
-        **extra
+        **extra,
     ):
         """
         Default constructor.
 
         Parameters:
          * client: A DAVClient instance
          * url: The url for this object.  May be a full URL or a relative URL.
@@ -195,14 +196,23 @@
             url = self.url
         ret = getattr(self.client, query_method)(url, body, depth)
         if ret.status == 404:
             raise error.NotFoundError(errmsg(ret))
         if (
             expected_return_value is not None and ret.status != expected_return_value
         ) or ret.status >= 400:
+            ## COMPATIBILITY HACK - see https://github.com/python-caldav/caldav/issues/309
+            body = to_wire(body)
+            if ret.status == 500 and not b"getetag" in body:
+                body = body.replace(
+                    b"<C:calendar-data/>", b"<D:getetag/><C:calendar-data/>"
+                )
+                return self._query(
+                    body, depth, query_method, url, expected_return_value
+                )
             raise error.exception_by_method[query_method](errmsg(ret))
         return ret
 
     def get_property(self, prop, use_cached=False, **passthrough):
         ## TODO: use_cached should probably be true
         if use_cached:
             if prop.tag in self.props:
@@ -273,14 +283,19 @@
             ## Workaround for a known iCloud bug.
             ## The properties key is expected to be the same as the path.
             ## path is on the format /123456/principal/ but properties key is /principal/
             ## tests apparently passed post bc589093a34f0ed0ef489ad5e9cba048750c9837 and 3ee4e42e2fa8f78b71e5ffd1ef322e4007df7a60, even without this workaround
             ## TODO: should probably be investigated more.
             ## (observed also by others, ref https://github.com/python-caldav/caldav/issues/168)
             rc = properties["/principal/"]
+        elif "//" in path and path.replace("//", "/") in properties:
+            ## ref https://github.com/python-caldav/caldav/issues/302
+            ## though, it would be nice to find the root cause,
+            ## self.url should not contain double slashes in the first place
+            rc = properties[path.replace("//", "/")]
         elif len(properties) == 1:
             ## Ref https://github.com/python-caldav/caldav/issues/191 ...
             ## let's be pragmatic and just accept whatever the server is
             ## throwing at us.  But we'll log an error anyway.
             log.error(
                 "Possibly the server has a path handling problem, possibly the URL configured is wrong.\n"
                 "Path expected: %s, path found: %s %s.\n"
@@ -373,15 +388,22 @@
         Returns:
          * [Calendar(), ...]
         """
         cals = []
 
         data = self.children(cdav.Calendar.tag)
         for c_url, c_type, c_name in data:
-            cals.append(Calendar(self.client, c_url, parent=self, name=c_name))
+            try:
+                cal_id = c_url.split("/")[-2]
+            except:
+                log.error(f"Calendar {c_name} has unexpected url {c_url}")
+                cal_id = None
+            cals.append(
+                Calendar(self.client, id=cal_id, url=c_url, parent=self, name=c_name)
+            )
 
         return cals
 
     def make_calendar(
         self, name=None, cal_id=None, supported_calendar_component_set=None
     ):
         """
@@ -965,15 +987,16 @@
         self,
         xml=None,
         comp_class=None,
         todo=None,
         include_completed=False,
         sort_keys=(),
         split_expanded=True,
-        **kwargs
+        props=None,
+        **kwargs,
     ):
         """Creates an XML query, does a REPORT request towards the
         server and returns objects found, eventually sorting them
         before delivery.
 
         This method contains some special logics to ensure that it can
         consistently return a list of pending tasks on any server
@@ -1006,29 +1029,29 @@
         ## special compatibility-case when searching for pending todos
         if todo and not include_completed:
             matches1 = self.search(
                 todo=True,
                 comp_class=comp_class,
                 ignore_completed1=True,
                 include_completed=True,
-                **kwargs
+                **kwargs,
             )
             matches2 = self.search(
                 todo=True,
                 comp_class=comp_class,
                 ignore_completed2=True,
                 include_completed=True,
-                **kwargs
+                **kwargs,
             )
             matches3 = self.search(
                 todo=True,
                 comp_class=comp_class,
                 ignore_completed3=True,
                 include_completed=True,
-                **kwargs
+                **kwargs,
             )
             objects = []
             match_set = set()
             for item in matches1 + matches2 + matches3:
                 if not item.url in match_set:
                     match_set.add(item.url)
                     ## and still, Zimbra seems to deliver too many TODOs in the
@@ -1040,35 +1063,44 @@
                         and not "\nSTATUS:CANCELLED" in item.data
                     ):
                         objects.append(item)
         else:
 
             if not xml:
                 (xml, comp_class) = self.build_search_xml_query(
-                    comp_class=comp_class, todo=todo, **kwargs
+                    comp_class=comp_class, todo=todo, props=props, **kwargs
                 )
             elif kwargs:
                 raise error.ConsistencyError(
                     "Inconsistent usage parameters: xml together with other search options"
                 )
-            (response, objects) = self._request_report_build_resultlist(xml, comp_class)
+            (response, objects) = self._request_report_build_resultlist(
+                xml, comp_class, props=props
+            )
 
         if kwargs.get("expand", False):
             ## expand can only be used together with start and end.
             ## Error checking is done in build_search_xml_query.  If
             ## search is fed with an XML query together with expand,
             ## then it's considered a "search option", and an error is
             ## raised above.
             start = kwargs["start"]
             end = kwargs["end"]
 
             for o in objects:
-                ## This should not be needed
+                ## This would not be needed if the servers would follow the standard ...
                 o.load(only_if_unloaded=True)
+
+            ## Google sometimes returns empty objects
+            objects = [o for o in objects if o.icalendar_component]
+
+            for o in objects:
                 component = o.icalendar_component
+                if component is None:
+                    continue
                 recurrance_properties = ["exdate", "exrule", "rdate", "rrule"]
                 if any(key in component for key in recurrance_properties):
                     o.expand_rrule(start, end)
             if split_expanded:
                 objects_ = objects
                 objects = []
                 for o in objects_:
@@ -1129,15 +1161,16 @@
         ignore_completed2=None,
         ignore_completed3=None,
         event=None,
         filters=None,
         expand=None,
         start=None,
         end=None,
-        **kwargs
+        props=None,
+        **kwargs,
     ):
         """This method will produce a caldav search query as an etree object.
 
         It is primarily to be used from the search method.  See the
         documentation for the search method for more information.
         """
         # those xml elements are weird.  (a+b)+c != a+(b+c).  First makes b and c as list members of a, second makes c an element in b which is an element of a.
@@ -1148,16 +1181,19 @@
 
         # build the request
         data = cdav.CalendarData()
         if expand:
             if not start or not end:
                 raise error.ReportError("can't expand without a date range")
             data += cdav.Expand(start, end)
-        prop = dav.Prop() + data
-
+        if props is None:
+            props_ = [data]
+        else:
+            props_ = [data] + props
+        prop = dav.Prop() + props_
         vcalendar = cdav.CompFilter("VCALENDAR")
 
         comp_filter = None
 
         if not filters:
             filters = []
 
@@ -1802,14 +1838,57 @@
 
         self.icalendar_component.add(
             "related-to", uid, parameters={"RELTYPE": reltype}, encode=True
         )
 
         self.save()
 
+    ## TODO: this method is undertested in the caldav library.
+    ## However, as this consolidated and eliminated quite some duplicated code in the
+    ## plann project, it is extensively tested in plann.
+    def get_relatives(
+        self, reltypes=None, relfilter=None, fetch_objects=True, ignore_missing=True
+    ):
+        """
+        By default, loads all objects pointed to by the RELATED-TO
+        property and loads the related objects.
+
+        It's possible to filter, either by passing a set or a list of
+        acceptable relation types in reltypes, or by passing a lambda
+        function in relfilter.
+
+        TODO: Make it possible to  also check up reverse relationships
+
+        TODO: this is partially overlapped by plann.lib._relships_by_type
+        in the plann tool.  Should consolidate the code.
+        """
+        ret = defaultdict(set)
+        relations = self.icalendar_component.get("RELATED-TO", [])
+        if not isinstance(relations, list):
+            relations = [relations]
+        for rel in relations:
+            if relfilter and not relfilter(rel):
+                continue
+            reltype = rel.params.get("RELTYPE", "PARENT")
+            if reltypes and not reltype in reltypes:
+                continue
+            ret[reltype].add(str(rel))
+
+        if fetch_objects:
+            for reltype in ret:
+                uids = ret[reltype]
+                ret[reltype] = []
+                for obj in uids:
+                    try:
+                        ret[reltype].append(self.parent.object_by_uid(obj))
+                    except error.NotFoundError:
+                        if not ignore_missing:
+                            raise
+        return ret
+
     def _get_icalendar_component(self, assert_one=False):
         """Returns the icalendar subcomponent - which should be an
         Event, Journal, Todo or FreeBusy from the icalendar class
 
         See also https://github.com/python-caldav/caldav/issues/232
         """
         self.load(only_if_unloaded=True)
@@ -1844,14 +1923,34 @@
 
     icalendar_component = property(
         _get_icalendar_component,
         _set_icalendar_component,
         doc="icalendar component - should not be used with recurrence sets",
     )
 
+    def get_due(self):
+        """
+        A VTODO may have due or duration set.  Return or calculate due.
+
+        WARNING: this method is likely to be deprecated and moved to
+        the icalendar library.  If you decide to use it, please put
+        caldav<2.0 in the requirements.
+        """
+        i = self.icalendar_component
+        if "DUE" in i:
+            return i["DUE"].dt
+        elif "DTEND" in i:
+            return i["DTEND"].dt
+        elif "DURATION" in i and "DTSTART" in i:
+            return i["DTSTART"].dt + i["DURATION"].dt
+        else:
+            return None
+
+    get_dtend = get_due
+
     def add_attendee(self, attendee, no_default_parameters=False, **parameters):
         """
         For the current (event/todo/journal), add an attendee.
 
         The attendee can be any of the following:
         * A principal
         * An email address prepended with "mailto:"
@@ -2617,21 +2716,21 @@
            datetime.now().
          * handle_rrule - if set to True, the library will try to be smart if
            the task is recurring.  The default is False, for backward
            compatibility.  I may consider making this one mandatory.
          * rrule_mode -   The RFC leaves a lot of room for intepretation on how
            to handle recurring tasks, and what works on one server may break at
            another.  The following modes are accepted:
-            * this_and_future - see doc for _complete_recurring_thisandfuture for details
-            * safe - see doc for _complete_recurring_safe for details
+           * this_and_future - see doc for _complete_recurring_thisandfuture for details
+           * safe - see doc for _complete_recurring_safe for details
         """
         if not completion_timestamp:
             completion_timestamp = datetime.utcnow().astimezone(timezone.utc)
 
-        if hasattr(self.instance.vtodo, "rrule") and handle_rrule:
+        if "RRULE" in self.icalendar_component and handle_rrule:
             return getattr(self, "_complete_recurring_%s" % rrule_mode)(
                 completion_timestamp
             )
         self._complete_ical(completion_timestamp=completion_timestamp)
         self.save()
 
     def _complete_ical(self, i=None, completion_timestamp=None):
@@ -2697,30 +2796,14 @@
         elif "DTSTART" in i:
             i.add("DUE", i["DTSTART"].dt + duration)
         else:
             if "DURATION" in i:
                 i.pop("DURATION")
             i.add("DURATION", duration)
 
-    def get_due(self):
-        """
-        A VTODO may have due or duration set.  Return or calculate due.
-
-        WARNING: this method is likely to be deprecated and moved to
-        the icalendar library.  If you decide to use it, please put
-        caldav<2.0 in the requirements.
-        """
-        i = self.icalendar_component
-        if "DUE" in i:
-            return i["DUE"].dt
-        elif "DURATION" in i and "DTSTART" in i:
-            return i["DTSTART"].dt + i["DURATION"].dt
-        else:
-            return None
-
     def set_due(self, due, move_dtstart=False, check_dependent=False):
         """The RFC specifies that a VTODO cannot have both due and
         duration, so when setting due, the duration field must be
         evicted
 
         check_dependent=True will raise some error if there exists a
         parent calendar component (through RELATED-TO), and the parents
@@ -2733,33 +2816,23 @@
         WARNING: the check_dependent-logic may be rewritten to support
         RFC9253 in 1.x already
         """
         if hasattr(due, "tzinfo") and not due.tzinfo:
             due = due.astimezone(timezone.utc)
         i = self.icalendar_component
         if check_dependent:
-            rels = i.get("RELATED-TO")
-            if rels is None:
-                rels = []
-            if not isinstance(rels, list):
-                rels = [rels]
-            for rel in rels:
-                if rel.params.get("RELTYPE") == "PARENT":
-                    parent = self.parent.object_by_uid(rel)
-                    pend = parent.icalendar_component.get("DTEND")
-                    if pend:
-                        pend = pend.dt
-                    else:
-                        pend = parent.get_due()
-                    if pend and pend.astimezone(timezone.utc) < due:
-                        if check_dependent == "return":
-                            return parent
-                        raise error.ConsistencyError(
-                            "parent object has due/end %s, cannot procrastinate child object without first procrastinating parent object"
-                        )
+            parents = self.get_relatives({"PARENT"})
+            for parent in parents["PARENT"]:
+                pend = parent.get_dtend()
+                if pend and pend.astimezone(timezone.utc) < due:
+                    if check_dependent == "return":
+                        return parent
+                    raise error.ConsistencyError(
+                        "parent object has due/end %s, cannot procrastinate child object without first procrastinating parent object"
+                    )
         duration = self.get_duration()
         i.pop("DURATION", None)
         i.pop("DUE", None)
 
         if move_dtstart and duration and "DTSTART" in i:
             i.pop("DTSTART")
             i.add("DTSTART", due - duration)
```

### Comparing `caldav-1.2.1/caldav.egg-info/PKG-INFO` & `caldav-1.3.2/caldav.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caldav
-Version: 1.2.1
+Version: 1.3.2
 Summary: CalDAV (RFC4791) client library
 Home-page: https://github.com/python-caldav/caldav
 Author: Cyril Robert
 Author-email: cyril@hippie.io
 License: GPL
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `caldav-1.2.1/caldav.egg-info/SOURCES.txt` & `caldav-1.3.2/caldav.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 caldav/lib/__init__.py
 caldav/lib/debug.py
 caldav/lib/error.py
 caldav/lib/namespace.py
 caldav/lib/python_utilities.py
 caldav/lib/url.py
 caldav/lib/vcal.py
-tests/#test_caldav.py#
+tests/#conf_private.py#
 tests/#tmp_226.py#
 tests/__init__.py
 tests/_test_absolute.py
 tests/compatibility_issues.py
 tests/conf.py
 tests/conf_private.py
 tests/conf_private.py.EXAMPLE
@@ -43,45 +43,60 @@
 tests/test_cdav.py
 tests/test_utils.py
 tests/test_utils.py~
 tests/test_vcal.py
 tests/test_vcal.py~
 tests/tmp_226~
 tests/__pycache__/__init__.cpython-310.pyc
+tests/__pycache__/__init__.cpython-311.pyc
 tests/__pycache__/__init__.cpython-39.pyc
 tests/__pycache__/compatibility_issues.cpython-310.pyc
+tests/__pycache__/compatibility_issues.cpython-311.pyc
 tests/__pycache__/compatibility_issues.cpython-39.pyc
 tests/__pycache__/conf.cpython-310.pyc
+tests/__pycache__/conf.cpython-311.pyc
 tests/__pycache__/conf.cpython-39.pyc
 tests/__pycache__/conf_private.cpython-310.pyc
+tests/__pycache__/conf_private.cpython-311.pyc
 tests/__pycache__/conf_private.cpython-39.pyc
 tests/__pycache__/proxy.cpython-310.pyc
+tests/__pycache__/proxy.cpython-311.pyc
 tests/__pycache__/proxy.cpython-39.pyc
 tests/__pycache__/test_caldav.cpython-310-pytest-7.1.3.pyc
 tests/__pycache__/test_caldav.cpython-310-pytest-7.2.0.pyc
 tests/__pycache__/test_caldav.cpython-310-pytest-7.2.1.pyc
 tests/__pycache__/test_caldav.cpython-310-pytest-7.2.2.pyc
 tests/__pycache__/test_caldav.cpython-310.pyc
+tests/__pycache__/test_caldav.cpython-311-pytest-7.3.1.pyc
+tests/__pycache__/test_caldav.cpython-311-pytest-7.4.0.pyc
 tests/__pycache__/test_caldav.cpython-39.pyc
 tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.1.3.pyc
 tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.0.pyc
 tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.1.pyc
 tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.2.pyc
 tests/__pycache__/test_caldav_unit.cpython-310.pyc
+tests/__pycache__/test_caldav_unit.cpython-311-pytest-7.3.1.pyc
+tests/__pycache__/test_caldav_unit.cpython-311-pytest-7.4.0.pyc
 tests/__pycache__/test_caldav_unit.cpython-39.pyc
 tests/__pycache__/test_cdav.cpython-310-pytest-7.1.3.pyc
 tests/__pycache__/test_cdav.cpython-310-pytest-7.2.0.pyc
 tests/__pycache__/test_cdav.cpython-310-pytest-7.2.1.pyc
 tests/__pycache__/test_cdav.cpython-310-pytest-7.2.2.pyc
 tests/__pycache__/test_cdav.cpython-310.pyc
+tests/__pycache__/test_cdav.cpython-311-pytest-7.3.1.pyc
+tests/__pycache__/test_cdav.cpython-311-pytest-7.4.0.pyc
 tests/__pycache__/test_cdav.cpython-39.pyc
 tests/__pycache__/test_utils.cpython-310-pytest-7.1.3.pyc
 tests/__pycache__/test_utils.cpython-310-pytest-7.2.0.pyc
 tests/__pycache__/test_utils.cpython-310-pytest-7.2.1.pyc
 tests/__pycache__/test_utils.cpython-310-pytest-7.2.2.pyc
 tests/__pycache__/test_utils.cpython-310.pyc
+tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc
+tests/__pycache__/test_utils.cpython-311-pytest-7.4.0.pyc
 tests/__pycache__/test_vcal.cpython-310-pytest-7.1.3.pyc
 tests/__pycache__/test_vcal.cpython-310-pytest-7.2.0.pyc
 tests/__pycache__/test_vcal.cpython-310-pytest-7.2.1.pyc
 tests/__pycache__/test_vcal.cpython-310-pytest-7.2.2.pyc
 tests/__pycache__/test_vcal.cpython-310.pyc
+tests/__pycache__/test_vcal.cpython-311-pytest-7.3.1.pyc
+tests/__pycache__/test_vcal.cpython-311-pytest-7.4.0.pyc
 tests/__pycache__/test_vcal.cpython-39.pyc
```

### Comparing `caldav-1.2.1/setup.py` & `caldav-1.3.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,20 +41,17 @@
         extra_test_packages = []
     except:
         extra_test_packages = ["mock"]
 
     test_packages = [
         "pytest",
         "pytest-coverage",
-        "icalendar",
         "coverage",
-        "tzlocal",
-        "pytz",
         "xandikos",
-        "radicale",
+        "sphinx",
     ]
 
     setup(
         name="caldav",
         version=version,
         py_modules=[
             "caldav",
@@ -83,12 +80,11 @@
             "vobject",
             "lxml",
             "requests",
             "icalendar",
             "recurring-ical-events>=2.0.0",
         ]
         + extra_packages,
-        tests_require=test_packages + extra_test_packages,
         extras_require={
             "test": test_packages,
         },
     )
```

### Comparing `caldav-1.2.1/tests/#test_caldav.py#` & `caldav-1.3.2/tests/test_caldav.py`

 * *Files 0% similar despite different names*

```diff
@@ -1482,20 +1482,24 @@
             assert len(rt) == 1
             rt = rt[0]
         assert rt == parent.id
         assert rt.params["RELTYPE"] == "PARENT"
 
         foo = parent_.get_relatives(reltypes={"PARENT"})
         assert len(foo) == 1
-        assert [foo[0].icalendar_component["UID"] == grandparent.id]
+        assert len(foo["PARENT"]) == 1
+        assert [foo["PARENT"][0].icalendar_component["UID"] == grandparent.id]
         foo = parent_.get_relatives(reltypes={"CHILD"})
         assert len(foo) == 1
-        assert [foo[0].icalendar_component["UID"] == child.id]
+        assert len(foo["CHILD"]) == 1
+        assert [foo["CHILD"][0].icalendar_component["UID"] == child.id]
         foo = parent_.get_relatives(reltypes={"CHILD", "PARENT"})
         assert len(foo) == 2
+        assert len(foo["CHILD"]) == 1
+        assert len(foo["PARENT"]) == 1
         foo = parent_.get_relatives(relfilter=lambda x: x.params.get("GAP"))
 
     def testSetDue(self):
         self.skip_on_compatibility_flag("read_only")
 
         c = self._fixCalendar(supported_calendar_component_set=["VTODO"])
```

### Comparing `caldav-1.2.1/tests/#tmp_226.py#` & `caldav-1.3.2/tests/#tmp_226.py#`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/compatibility_issues.cpython-310.pyc` & `caldav-1.3.2/tests/__pycache__/compatibility_issues.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/compatibility_issues.cpython-39.pyc` & `caldav-1.3.2/tests/__pycache__/compatibility_issues.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/conf.cpython-310.pyc` & `caldav-1.3.2/tests/__pycache__/conf.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/conf.cpython-39.pyc` & `caldav-1.3.2/tests/__pycache__/conf.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/conf_private.cpython-310.pyc` & `caldav-1.3.2/tests/__pycache__/conf_private.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/conf_private.cpython-39.pyc` & `caldav-1.3.2/tests/__pycache__/conf_private.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/proxy.cpython-310.pyc` & `caldav-1.3.2/tests/__pycache__/proxy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/proxy.cpython-39.pyc` & `caldav-1.3.2/tests/__pycache__/proxy.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_caldav.cpython-310-pytest-7.1.3.pyc` & `caldav-1.3.2/tests/__pycache__/test_caldav.cpython-310-pytest-7.1.3.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_caldav.cpython-310-pytest-7.2.0.pyc` & `caldav-1.3.2/tests/__pycache__/test_caldav.cpython-310-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_caldav.cpython-310-pytest-7.2.1.pyc` & `caldav-1.3.2/tests/__pycache__/test_caldav.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_caldav.cpython-310-pytest-7.2.2.pyc` & `caldav-1.3.2/tests/__pycache__/test_caldav.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_caldav.cpython-310.pyc` & `caldav-1.3.2/tests/__pycache__/test_caldav.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_caldav.cpython-39.pyc` & `caldav-1.3.2/tests/__pycache__/test_caldav.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.1.3.pyc` & `caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.1.3.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.0.pyc` & `caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.1.pyc` & `caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.2.pyc` & `caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_caldav_unit.cpython-310.pyc` & `caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_caldav_unit.cpython-39.pyc` & `caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_cdav.cpython-310-pytest-7.1.3.pyc` & `caldav-1.3.2/tests/__pycache__/test_cdav.cpython-310-pytest-7.1.3.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_cdav.cpython-310-pytest-7.2.0.pyc` & `caldav-1.3.2/tests/__pycache__/test_cdav.cpython-310-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_cdav.cpython-310-pytest-7.2.1.pyc` & `caldav-1.3.2/tests/__pycache__/test_cdav.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_cdav.cpython-310-pytest-7.2.2.pyc` & `caldav-1.3.2/tests/__pycache__/test_cdav.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_cdav.cpython-310.pyc` & `caldav-1.3.2/tests/__pycache__/test_cdav.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_cdav.cpython-39.pyc` & `caldav-1.3.2/tests/__pycache__/test_cdav.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_utils.cpython-310-pytest-7.1.3.pyc` & `caldav-1.3.2/tests/__pycache__/test_utils.cpython-310-pytest-7.1.3.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_utils.cpython-310-pytest-7.2.0.pyc` & `caldav-1.3.2/tests/__pycache__/test_utils.cpython-310-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_utils.cpython-310-pytest-7.2.1.pyc` & `caldav-1.3.2/tests/__pycache__/test_utils.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_utils.cpython-310-pytest-7.2.2.pyc` & `caldav-1.3.2/tests/__pycache__/test_utils.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_utils.cpython-310.pyc` & `caldav-1.3.2/tests/__pycache__/test_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_vcal.cpython-310-pytest-7.1.3.pyc` & `caldav-1.3.2/tests/__pycache__/test_vcal.cpython-310-pytest-7.1.3.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_vcal.cpython-310-pytest-7.2.0.pyc` & `caldav-1.3.2/tests/__pycache__/test_vcal.cpython-310-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_vcal.cpython-310-pytest-7.2.1.pyc` & `caldav-1.3.2/tests/__pycache__/test_vcal.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_vcal.cpython-310-pytest-7.2.2.pyc` & `caldav-1.3.2/tests/__pycache__/test_vcal.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_vcal.cpython-310.pyc` & `caldav-1.3.2/tests/__pycache__/test_vcal.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/__pycache__/test_vcal.cpython-39.pyc` & `caldav-1.3.2/tests/__pycache__/test_vcal.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/_test_absolute.py` & `caldav-1.3.2/tests/_test_absolute.py`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/compatibility_issues.py` & `caldav-1.3.2/tests/compatibility_issues.py`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/conf.py` & `caldav-1.3.2/tests/conf.py`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/conf_private.py` & `caldav-1.3.2/tests/#conf_private.py#`

 * *Files 3% similar despite different names*

```diff
@@ -124,24 +124,29 @@
         'incompatibilities': ["time_based_sync_tokens", "search_needs_comptype", "fastmail_buggy_noexpand_date_search", "text_search_not_working", "isnotdefined_not_working", 'no_journal', 'no_freebusy_rfc4791'] ## and in addition ... the requests are efficiently rate limited, as it spawns lots of postgresql connections all until a limit
     },
     { # 15 - posteo
         'url': 'https://posteo.de:8443/',
         'username': 'pycaltest',
         'password': 'stopped-prototype-frostingA1',
         'incompatibilities': ['no_scheduling', 'no_mkcalendar', 'no_journal', 'no_recurring_todo', 'no_sync_token'] ## no freebusy?
+    },
+    { # 16 - gmx
+        'url': 'https://caldav.gmx.net/begenda/dav/users/pycaldavtest@gmx.net/',
+        'username': 'pycaldavtest@gmx.net',
+        'password': 'CalDavTest'
     }
 ]
 
 if False:
     test_xandikos = True
     test_radicale = True
-elif False:
+elif True:
     for x in caldav_servers:
         x['enable'] = False
-    caldav_servers[12]['enable']=True
+    caldav_servers[16]['enable']=True
 
     test_xandikos = False
     test_radicale = False
 else:
     caldav_servers = []
     test_xandikos = True
     test_radicale = True
@@ -158,15 +163,15 @@
 ## 2) I installed virtualbox on my laptop
 ## 3) "virtualbox ~/Downloads/ZEG-5.0.0.ova" (TODO: probably it's possible to launch it "headless"?)
 ## 4) I clicked on some buttons to get the file "imported" and started
 ## 5) I went to "tools" -> "preferences" -> "network" and created a NatNetwork
 ## 6) I think I went to ZEG -> Settings -> Network and chose "Host-only Adapter"
 ## 7) SOGo was then available at http://192.168.56.101/ from my laptop
 ## 8) I added the lines below to my conf_private.py
-#caldav_servers.append({
+#cal-dav_servers.append({
 #    'url': 'http://192.168.56.101/SOGo/dav/',
 #    'username': 'sogo1'.
 #    'password': 'sogo'
 #})
 #for i in (1, 2, 3):
 #    sogo = caldav_servers[-1].copy()
 #    sogo['username'] = 'sogo%i' % i
```

### Comparing `caldav-1.2.1/tests/conf_private.py.EXAMPLE` & `caldav-1.3.2/tests/conf_private.py.EXAMPLE`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/conf_private.py~` & `caldav-1.3.2/tests/conf_private.py~`

 * *Files 4% similar despite different names*

```diff
@@ -124,24 +124,29 @@
         'incompatibilities': ["time_based_sync_tokens", "search_needs_comptype", "fastmail_buggy_noexpand_date_search", "text_search_not_working", "isnotdefined_not_working", 'no_journal', 'no_freebusy_rfc4791'] ## and in addition ... the requests are efficiently rate limited, as it spawns lots of postgresql connections all until a limit
     },
     { # 15 - posteo
         'url': 'https://posteo.de:8443/',
         'username': 'pycaltest',
         'password': 'stopped-prototype-frostingA1',
         'incompatibilities': ['no_scheduling', 'no_mkcalendar', 'no_journal', 'no_recurring_todo', 'no_sync_token'] ## no freebusy?
+    },
+    { # 16 - gmx
+        'url': 'https://caldav.gmx.net/begenda/dav/users/pycaldavtest@gmx.net/',
+        'username': 'pycaldavtest@gmx.net',
+        'password': 'CalDavTest'
     }
 ]
 
 if False:
     test_xandikos = True
     test_radicale = True
 elif True:
     for x in caldav_servers:
         x['enable'] = False
-    caldav_servers[1]['enable']=True
+    caldav_servers[16]['enable']=True
 
     test_xandikos = False
     test_radicale = False
 else:
     caldav_servers = []
     test_xandikos = True
     test_radicale = True
```

### Comparing `caldav-1.2.1/tests/proxy.py` & `caldav-1.3.2/tests/proxy.py`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/test_caldav.py` & `caldav-1.3.2/tests/test_caldav.py.orig`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 Tests here communicate with third party servers and/or
 internal ad-hoc instances of Xandikos and Radicale, dependent on the
 configuration in conf_private.py.
 Tests that do not require communication with a working caldav server
 belong in test_caldav_unit.py
 """
-import codecs
 import logging
 import random
 import sys
 import tempfile
 import threading
 import time
 import uuid
@@ -38,14 +37,15 @@
 from caldav.objects import CalendarSet
 from caldav.objects import DAVObject
 from caldav.objects import Event
 from caldav.objects import FreeBusy
 from caldav.objects import Principal
 from caldav.objects import Todo
 from requests.packages import urllib3
+from six import PY3
 
 from . import compatibility_issues
 from .conf import caldav_servers
 from .conf import client
 from .conf import proxy
 from .conf import proxy_noport
 from .conf import radicale_host
@@ -66,15 +66,18 @@
 
 if test_radicale:
     import radicale.config
     import radicale
     import radicale.server
     import socket
 
-from urllib.parse import urlparse
+if PY3:
+    from urllib.parse import urlparse
+else:
+    from urlparse import urlparse
 
 log = logging.getLogger("caldav")
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 ev1 = """BEGIN:VCALENDAR
 VERSION:2.0
@@ -508,15 +511,24 @@
         if False and self.check_compatibility_flag("no-current-user-principal"):
             self.principal = Principal(
                 client=self.caldav, url=self.server_params["principal_url"]
             )
         else:
             self.principal = self.caldav.principal()
 
-        self._cleanup("pre")
+        if (
+            not self.check_compatibility_flag("read_only")
+            and self.cleanup_regime == "thorough"
+        ):
+            logging.debug(
+                "## going to tear down old test calendars, "
+                "in case teardown_method wasn't properly executed "
+                "last time tests were run"
+            )
+            self._cleanup("pre")
 
         if self.check_compatibility_flag("object_by_uid_is_broken"):
             import caldav.objects
 
             caldav.objects.NotImplementedError = SkipTest
 
         logging.debug("##############################")
@@ -529,14 +541,16 @@
         logging.debug("############################")
         self._cleanup("post")
         logging.debug("############## test teardown_method done")
 
     def _cleanup(self, mode=None):
         if self.cleanup_regime in ("pre", "post") and self.cleanup_regime != mode:
             return
+        for cal in self.calendars_used:
+            cal.delete()
         if self.check_compatibility_flag("read_only"):
             return  ## no cleanup needed
         if (
             self.check_compatibility_flag("no_mkcalendar")
             or self.cleanup_regime == "thorough"
         ):
             for uid in uids_used:
@@ -546,22 +560,15 @@
                 except error.NotFoundError:
                     pass
                 except:
                     logging.error(
                         "Something went kaboom while deleting event", exc_info=True
                     )
             return
-        for cal in self.calendars_used:
-            cal.delete()
-        if self.check_compatibility_flag("unique_calendar_ids") and mode == "pre":
-            a = self._teardownCalendar(name="Yep")
-        if mode == "post":
-            for calid in (self.testcal_id, self.testcal_id2):
-                self._teardownCalendar(cal_id=calid)
-        if self.cleanup_regime == "thorough":
+        if self.cleanup_regime in ("normal", "thorough"):
             for name in ("Yep", "Yapp", "Yølp", self.testcal_id, self.testcal_id2):
                 self._teardownCalendar(name=name)
                 self._teardownCalendar(cal_id=name)
 
     def _teardownCalendar(self, name=None, cal_id=None):
         try:
             cal = self.principal.calendar(name=name, cal_id=cal_id)
@@ -814,16 +821,14 @@
         assert events2[0].url == events[0].url
 
         if not self.check_compatibility_flag(
             "no_mkcalendar"
         ) and not self.check_compatibility_flag("no_displayname"):
             # We should be able to access the calender through the name
             c2 = self.principal.calendar(name="Yep")
-            ## may break if we have multiple calendars with the same name
-            assert c2.url == c.url
             events2 = c2.events()
             assert len(events2) == 1
             assert events2[0].url == events[0].url
 
         # add another event, it should be doable without having premade ICS
         ev2 = c.save_event(
             dtstart=datetime(2015, 10, 10, 8, 7, 6),
@@ -1416,30 +1421,14 @@
         some_todos = c.search(todo=True)
         assert len(some_todos) == 3
 
         ## unless we specifically ask for completed tasks
         all_todos = c.search(todo=True, include_completed=True)
         assert len(all_todos) == 6
 
-    def testWrongPassword(self):
-        if (
-            not "password" in self.server_params
-            or not self.server_params["password"]
-            or self.server_params["password"] == "any-password-seems-to-work"
-        ):
-            pytest.skip(
-                "Testing with wrong password skipped as calendar server does not require a password"
-            )
-        server_params = self.server_params.copy()
-        server_params["password"] = (
-            codecs.encode(server_params["password"], "rot13") + "!"
-        )
-        with pytest.raises(error.AuthorizationError):
-            client(**server_params).principal()
-
     def testCreateChildParent(self):
         self.skip_on_compatibility_flag("read_only")
         self.skip_on_compatibility_flag("no_relships")
         c = self._fixCalendar(supported_calendar_component_set=["VEVENT"])
         parent = c.save_event(
             dtstart=datetime(2022, 12, 26, 19, 15),
             dtend=datetime(2022, 12, 26, 20, 00),
@@ -1483,15 +1472,15 @@
             rt = rt[0]
         assert rt == parent.id
         assert rt.params["RELTYPE"] == "PARENT"
 
     def testSetDue(self):
         self.skip_on_compatibility_flag("read_only")
 
-        c = self._fixCalendar(supported_calendar_component_set=["VTODO"])
+        c = self._fixCalendar(supported_calendar_component_set=["VEVENT"])
 
         utc = timezone.utc
 
         some_todo = c.save_todo(
             dtstart=datetime(2022, 12, 26, 19, 15, tzinfo=utc),
             due=datetime(2022, 12, 26, 20, 00, tzinfo=utc),
             summary="Some task",
@@ -2447,15 +2436,15 @@
         self.configuration.update(
             {"storage": {"filesystem_folder": self.serverdir.name}}
         )
         self.server = radicale.server
         self.server_params = {
             "url": "http://%s:%i/" % (radicale_host, radicale_port),
             "username": "user1",
-            "password": "any-password-seems-to-work",
+            "password": "password1",
         }
         self.server_params["backwards_compatibility_url"] = (
             self.server_params["url"] + "user1"
         )
         self.server_params["incompatibilities"] = compatibility_issues.radicale
         self.shutdown_socket, self.shutdown_socket_out = socket.socketpair()
         self.radicale_thread = threading.Thread(
```

### Comparing `caldav-1.2.1/tests/test_caldav.py.rej` & `caldav-1.3.2/tests/test_caldav.py.rej`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/test_caldav_unit.py` & `caldav-1.3.2/tests/test_caldav_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,24 +143,24 @@
 CLASS:CONFIDENTIAL
 CATEGORIES:FAMILY,FINANCE
 PRIORITY:1
 END:VTODO
 END:VCALENDAR"""
 
 
-def MockedDAVResponse(text):
+def MockedDAVResponse(text, davclient=None):
     """
     For unit testing - a mocked DAVResponse with some specific content
     """
     resp = mock.MagicMock()
     resp.status_code = 207
     resp.reason = "multistatus"
     resp.headers = {}
     resp.content = text
-    return DAVResponse(resp)
+    return DAVResponse(resp, davclient)
 
 
 def MockedDAVClient(xml_returned):
     """
     For unit testing - a mocked DAVClient returning some specific content every time
     a request is performed
     """
@@ -261,14 +261,26 @@
             "bringebærsyltetøy 北京 пиво".encode("utf-8"),
             {},
         )
         assert response.status == 200
         assert response.tree is None
 
     @mock.patch("caldav.davclient.requests.Session.request")
+    def testRequestCustomHeaders(self, mocked):
+        """
+        ref https://github.com/python-caldav/caldav/issues/285
+        """
+        mocked().status_code = 200
+        mocked().headers = {}
+        cal_url = "http://me:hunter2@calendar.møøh.example:80/"
+        client = DAVClient(url=cal_url, headers={"X-NC-CalDAV-Webcal-Caching": "On"})
+        assert client.headers["Content-Type"] == "text/xml"
+        assert client.headers["X-NC-CalDAV-Webcal-Caching"] == "On"
+
+    @mock.patch("caldav.davclient.requests.Session.request")
     def testEmptyXMLNoContentLength(self, mocked):
         """
         ref https://github.com/python-caldav/caldav/issues/213
         """
         mocked().status_code = 200
         mocked().headers = {"Content-Type": "text/xml"}
         mocked().content = ""
@@ -866,14 +878,95 @@
             },
             "/17149682/calendars/testcalendar-f96b3bf0-09e1-4f3d-b891-3a25c99a2894/20010712T182145Z-123401@example.com.ics": {
                 "{DAV:}getetag": '"kkkgoqqu"',
                 "{urn:ietf:params:xml:ns:caldav}calendar-data": None,
             },
         }
 
+    def testHugeTreeParam(self):
+        """
+        With dealing with a huge XML response, such as event containing attachments, XMLParser will throw an exception
+        huge_tree parameters allows to handle this kind of events.
+        """
+
+        xml = """
+<multistatus xmlns="DAV:">
+  <response>
+    <href>/17149682/calendars/testcalendar-84439d0b-ce46-4416-b978-7b4009122c64/</href>
+    <propstat>
+      <prop>
+                </prop>
+      <status>HTTP/1.1 200 OK</status>
+    </propstat>
+    <propstat>
+      <prop>
+        <calendar-data xmlns="urn:ietf:params:xml:ns:caldav"/>
+      </prop>
+      <status>HTTP/1.1 404 Not Found</status>
+    </propstat>
+  </response>
+  <response>
+    <href>/17149682/calendars/testcalendar-84439d0b-ce46-4416-b978-7b4009122c64/20010712T182145Z-123401%40example.com.ics</href>
+    <propstat>
+      <prop>
+        <calendar-data xmlns="urn:ietf:params:xml:ns:caldav">
+
+BEGIN:VCALENDAR
+PRODID:-//MDaemon Technologies Ltd//MDaemon 21.5.2
+VERSION:2.0
+METHOD:PUBLISH
+BEGIN:VEVENT
+UID:
+ 040000008200E0007000B7101A82E0080000000050BF99B19D31
+SEQUENCE:0
+DTSTAMP:20230213T142930Z
+SUMMARY:This a summary of a very bug event
+DESCRIPTION:Description of this very big event
+LOCATION:Somewhere
+ORGANIZER:MAILTO:noreply@test.com
+PRIORITY:5
+ATTACH;VALUE=BINARY;ENCODING=BASE64;FMTTYPE=image/jpeg;
+ X-FILENAME=image001.jpg;X-ORACLE-FILENAME=image001.jpg:
+"""
+        xml += (
+            "gIyIoLTkwKCo2KyIjM4444449QEBAJjBGS0U+Sjk/QD3/2wBDAQsLCw8NDx0QEB09KSMpPT09\n"
+            * 153490
+        )
+        xml += """
+ /Z
+DTSTART;TZID="Europe/Paris":20230310T140000
+DTEND;TZID="Europe/Paris":20230310T150000
+END:VEVENT
+END:VCALENDAR
+</calendar-data>
+      </prop>
+      <status>HTTP/1.1 200 OK</status>
+    </propstat>
+  </response>
+</multistatus>
+"""
+        davclient = MockedDAVClient(xml)
+        resp = mock.MagicMock()
+        resp.headers = {"Content-Type": "text/xml"}
+        resp.content = xml
+
+        davclient.huge_tree = False
+        try:
+            DAVResponse(resp, davclient=davclient)
+            assert False
+        except Exception as e:
+            assert type(e) == lxml.etree.XMLSyntaxError
+
+        davclient.huge_tree = True
+        try:
+            DAVResponse(resp, davclient=davclient)
+            assert True
+        except:
+            assert False
+
     def testFailedQuery(self):
         """
         ref https://github.com/python-caldav/caldav/issues/54
         """
         cal_url = "http://me:hunter2@calendar.example:80/"
         client = DAVClient(url=cal_url)
         calhome = CalendarSet(client, cal_url + "me/")
```

### Comparing `caldav-1.2.1/tests/test_cdav.py` & `caldav-1.3.2/tests/test_cdav.py`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/test_utils.py` & `caldav-1.3.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `caldav-1.2.1/tests/test_vcal.py` & `caldav-1.3.2/tests/test_vcal.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,30 @@
         assert re.search(b"DTSTART(;VALUE=DATE-TIME)?:20321010T101010Z", some_ical)
 
     def test_vcal_fixups(self):
         """
         There is an obscure function lib.vcal that attempts to fix up
         known ical standard breaches from various calendar servers.
         """
+        non_broken_ical = [
+            """BEGIN:VCALENDAR
+VERSION:2.0
+PRODID:-//python-caldav//caldav//en_DK
+BEGIN:VEVENT
+SUMMARY:Foo bar blah
+ blub
+DTSTART:20230313T084500Z
+DURATION:PT30M
+DTSTAMP:20230312T215907Z
+UID:1c9bba3e-c121-11ed-bf96-982cbcdd642c
+CATEGORIES:oslo
+END:VEVENT
+END:VCALENDAR
+"""
+        ]
         broken_ical = [
             ## This first one contains duplicated DTSTAMP in the event data
             """BEGIN:VCALENDAR
 X-EXPANDED:True
 X-MASTER-DTSTART:20200517T060000Z
 X-MASTER-RRULE:FREQ=YEARLY
 BEGIN:VEVENT
@@ -229,7 +245,10 @@
 
         for ical in broken_ical:
             ## This should raise error
             with pytest.raises(vobject.base.ValidateError):
                 vobject.readOne(ical).serialize()
             ## This should not raise error
             vobject.readOne(vcal.fix(ical)).serialize()
+
+        for ical in non_broken_ical:
+            assert vcal.fix(ical) == ical
```

### Comparing `caldav-1.2.1/tests/tmp_226~` & `caldav-1.3.2/tests/tmp_226~`

 * *Files identical despite different names*

