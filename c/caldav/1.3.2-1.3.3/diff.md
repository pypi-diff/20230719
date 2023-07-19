# Comparing `tmp/caldav-1.3.2.tar.gz` & `tmp/caldav-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caldav-1.3.2.tar", last modified: Wed Jul 19 13:08:55 2023, max compression
+gzip compressed data, was "caldav-1.3.3.tar", last modified: Wed Jul 19 13:39:09 2023, max compression
```

## Comparing `caldav-1.3.2.tar` & `caldav-1.3.3.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-19 13:08:55.442054 caldav-1.3.2/
--rw-r--r--   0 tobias    (7385) tobias    (7385)    11358 2019-09-10 16:18:00.000000 caldav-1.3.2/COPYING.APACHE
--rw-r--r--   0 tobias    (7385) tobias    (7385)    35147 2019-09-10 16:18:00.000000 caldav-1.3.2/COPYING.GPL
--rw-r--r--   0 tobias    (7385) tobias    (7385)       87 2023-05-22 07:00:24.000000 caldav-1.3.2/MANIFEST.in
--rw-r--r--   0 tobias    (7385) tobias    (7385)     1354 2023-07-19 13:08:55.442054 caldav-1.3.2/PKG-INFO
--rw-r--r--   0 tobias    (7385) tobias    (7385)      635 2023-05-22 07:00:24.000000 caldav-1.3.2/README.md
-drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-19 13:08:55.428721 caldav-1.3.2/caldav/
--rw-r--r--   0 tobias    (7385) tobias    (7385)      543 2023-07-19 13:07:21.000000 caldav-1.3.2/caldav/__init__.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)    25502 2023-07-18 22:32:35.000000 caldav-1.3.2/caldav/davclient.py
-drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-19 13:08:55.432054 caldav-1.3.2/caldav/elements/
--rw-r--r--   0 tobias    (7385) tobias    (7385)       48 2023-05-22 07:00:24.000000 caldav-1.3.2/caldav/elements/__init__.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     1945 2023-07-18 22:32:35.000000 caldav-1.3.2/caldav/elements/base.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     4935 2023-05-22 07:00:24.000000 caldav-1.3.2/caldav/elements/cdav.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     1609 2023-05-22 07:00:24.000000 caldav-1.3.2/caldav/elements/dav.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)      319 2023-05-22 07:00:24.000000 caldav-1.3.2/caldav/elements/ical.py
-drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-19 13:08:55.432054 caldav-1.3.2/caldav/lib/
--rw-r--r--   0 tobias    (7385) tobias    (7385)        0 2019-09-10 16:18:00.000000 caldav-1.3.2/caldav/lib/__init__.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)      231 2023-07-18 22:45:26.000000 caldav-1.3.2/caldav/lib/debug.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     2540 2023-07-18 22:01:33.000000 caldav-1.3.2/caldav/lib/error.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)      668 2023-05-22 07:00:24.000000 caldav-1.3.2/caldav/lib/namespace.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)      798 2023-07-18 22:32:35.000000 caldav-1.3.2/caldav/lib/python_utilities.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     6480 2023-07-18 22:32:35.000000 caldav-1.3.2/caldav/lib/url.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     7450 2023-07-18 22:32:35.000000 caldav-1.3.2/caldav/lib/vcal.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)   109108 2023-07-19 13:05:08.000000 caldav-1.3.2/caldav/objects.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)      402 2023-05-22 07:00:24.000000 caldav-1.3.2/caldav/requests.py
-drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-19 13:08:55.432054 caldav-1.3.2/caldav.egg-info/
--rw-r--r--   0 tobias    (7385) tobias    (7385)     1354 2023-07-19 13:08:55.000000 caldav-1.3.2/caldav.egg-info/PKG-INFO
--rw-r--r--   0 tobias    (7385) tobias    (7385)     3878 2023-07-19 13:08:55.000000 caldav-1.3.2/caldav.egg-info/SOURCES.txt
--rw-r--r--   0 tobias    (7385) tobias    (7385)        1 2023-07-19 13:08:55.000000 caldav-1.3.2/caldav.egg-info/dependency_links.txt
--rw-r--r--   0 tobias    (7385) tobias    (7385)        1 2022-11-22 09:14:37.000000 caldav-1.3.2/caldav.egg-info/not-zip-safe
--rw-r--r--   0 tobias    (7385) tobias    (7385)      130 2023-07-19 13:08:55.000000 caldav-1.3.2/caldav.egg-info/requires.txt
--rw-r--r--   0 tobias    (7385) tobias    (7385)        7 2023-07-19 13:08:55.000000 caldav-1.3.2/caldav.egg-info/top_level.txt
--rw-r--r--   0 tobias    (7385) tobias    (7385)      506 2023-07-19 13:08:55.445388 caldav-1.3.2/setup.cfg
--rwxr-xr-x   0 tobias    (7385) tobias    (7385)     2877 2023-07-18 22:32:35.000000 caldav-1.3.2/setup.py
-drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-19 13:08:55.435388 caldav-1.3.2/tests/
--rw-------   0 tobias    (7385) tobias    (7385)     8630 2023-05-25 19:43:46.000000 caldav-1.3.2/tests/#conf_private.py#
--rwxr-xr-x   0 tobias    (7385) tobias    (7385)      888 2022-11-03 16:22:35.000000 caldav-1.3.2/tests/#tmp_226.py#
--rw-r--r--   0 tobias    (7385) tobias    (7385)        0 2019-09-10 16:18:00.000000 caldav-1.3.2/tests/__init__.py
-drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-19 13:08:55.442054 caldav-1.3.2/tests/__pycache__/
--rw-r--r--   0 tobias    (7385) tobias    (7385)      130 2022-01-05 17:28:37.000000 caldav-1.3.2/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)      146 2023-05-22 06:28:45.000000 caldav-1.3.2/tests/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)      128 2021-10-10 21:24:31.000000 caldav-1.3.2/tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     7969 2023-02-25 18:55:46.000000 caldav-1.3.2/tests/__pycache__/compatibility_issues.cpython-310.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     8694 2023-07-19 10:22:04.000000 caldav-1.3.2/tests/__pycache__/compatibility_issues.cpython-311.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     4188 2021-11-10 00:21:31.000000 caldav-1.3.2/tests/__pycache__/compatibility_issues.cpython-39.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     2401 2023-02-14 21:14:51.000000 caldav-1.3.2/tests/__pycache__/conf.cpython-310.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     3722 2023-05-24 11:30:31.000000 caldav-1.3.2/tests/__pycache__/conf.cpython-311.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     1788 2021-10-10 21:24:45.000000 caldav-1.3.2/tests/__pycache__/conf.cpython-39.pyc
--rw-------   0 tobias    (7385) tobias    (7385)     2949 2023-03-06 14:30:08.000000 caldav-1.3.2/tests/__pycache__/conf_private.cpython-310.pyc
--rw-------   0 tobias    (7385) tobias    (7385)     3638 2023-07-18 16:05:33.000000 caldav-1.3.2/tests/__pycache__/conf_private.cpython-311.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)      709 2021-11-30 09:55:30.000000 caldav-1.3.2/tests/__pycache__/conf_private.cpython-39.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    10615 2023-02-27 20:25:36.000000 caldav-1.3.2/tests/__pycache__/proxy.cpython-310.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    19912 2023-07-19 10:22:04.000000 caldav-1.3.2/tests/__pycache__/proxy.cpython-311.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    10615 2021-10-10 21:24:45.000000 caldav-1.3.2/tests/__pycache__/proxy.cpython-39.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    99664 2022-11-01 22:32:56.000000 caldav-1.3.2/tests/__pycache__/test_caldav.cpython-310-pytest-7.1.3.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)   108125 2023-01-15 22:21:23.000000 caldav-1.3.2/tests/__pycache__/test_caldav.cpython-310-pytest-7.2.0.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)   115157 2023-03-06 14:51:44.000000 caldav-1.3.2/tests/__pycache__/test_caldav.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)   115163 2023-03-13 07:21:44.000000 caldav-1.3.2/tests/__pycache__/test_caldav.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    55936 2023-03-06 14:15:55.000000 caldav-1.3.2/tests/__pycache__/test_caldav.cpython-310.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)   346344 2023-05-24 11:30:31.000000 caldav-1.3.2/tests/__pycache__/test_caldav.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)   353122 2023-07-19 10:22:03.000000 caldav-1.3.2/tests/__pycache__/test_caldav.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    41792 2021-12-02 18:17:39.000000 caldav-1.3.2/tests/__pycache__/test_caldav.cpython-39.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    61467 2022-11-01 22:32:56.000000 caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.1.3.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    62010 2023-01-15 22:21:23.000000 caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.0.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    63615 2023-02-27 20:25:36.000000 caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    63618 2023-03-13 07:21:45.000000 caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    33628 2023-03-06 14:13:09.000000 caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-310.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)   160045 2023-05-24 11:30:31.000000 caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)   160045 2023-07-19 10:22:04.000000 caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    26186 2021-10-10 21:24:31.000000 caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-39.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     4379 2022-10-04 22:09:32.000000 caldav-1.3.2/tests/__pycache__/test_cdav.cpython-310-pytest-7.1.3.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     4379 2022-11-21 19:20:28.000000 caldav-1.3.2/tests/__pycache__/test_cdav.cpython-310-pytest-7.2.0.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     4379 2023-01-16 00:55:21.000000 caldav-1.3.2/tests/__pycache__/test_cdav.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     4379 2023-03-13 07:21:45.000000 caldav-1.3.2/tests/__pycache__/test_cdav.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     2057 2023-03-06 14:13:09.000000 caldav-1.3.2/tests/__pycache__/test_cdav.cpython-310.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    10956 2023-05-24 11:30:31.000000 caldav-1.3.2/tests/__pycache__/test_cdav.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    10956 2023-07-10 18:48:32.000000 caldav-1.3.2/tests/__pycache__/test_cdav.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     2029 2021-10-10 21:24:31.000000 caldav-1.3.2/tests/__pycache__/test_cdav.cpython-39.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)      793 2022-10-04 22:09:32.000000 caldav-1.3.2/tests/__pycache__/test_utils.cpython-310-pytest-7.1.3.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)      793 2022-11-21 19:20:28.000000 caldav-1.3.2/tests/__pycache__/test_utils.cpython-310-pytest-7.2.0.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)      793 2023-01-16 00:55:21.000000 caldav-1.3.2/tests/__pycache__/test_utils.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)      793 2023-03-13 07:21:45.000000 caldav-1.3.2/tests/__pycache__/test_utils.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)      684 2023-03-06 14:13:09.000000 caldav-1.3.2/tests/__pycache__/test_utils.cpython-310.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     1527 2023-05-24 11:30:31.000000 caldav-1.3.2/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     1527 2023-07-10 18:48:32.000000 caldav-1.3.2/tests/__pycache__/test_utils.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     3372 2022-10-04 22:09:32.000000 caldav-1.3.2/tests/__pycache__/test_vcal.cpython-310-pytest-7.1.3.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     7304 2023-01-15 22:21:23.000000 caldav-1.3.2/tests/__pycache__/test_vcal.cpython-310-pytest-7.2.0.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     7304 2023-02-11 09:38:03.000000 caldav-1.3.2/tests/__pycache__/test_vcal.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     8024 2023-03-13 07:21:45.000000 caldav-1.3.2/tests/__pycache__/test_vcal.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     5975 2023-03-06 14:13:09.000000 caldav-1.3.2/tests/__pycache__/test_vcal.cpython-310.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    15151 2023-05-24 11:30:31.000000 caldav-1.3.2/tests/__pycache__/test_vcal.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)    15151 2023-07-19 10:22:04.000000 caldav-1.3.2/tests/__pycache__/test_vcal.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     2650 2021-11-30 08:41:46.000000 caldav-1.3.2/tests/__pycache__/test_vcal.cpython-39.pyc
--rw-r--r--   0 tobias    (7385) tobias    (7385)     1290 2023-05-22 07:00:24.000000 caldav-1.3.2/tests/_test_absolute.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)    14105 2023-07-18 22:32:35.000000 caldav-1.3.2/tests/compatibility_issues.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     4909 2023-05-22 07:00:24.000000 caldav-1.3.2/tests/conf.py
--rw-------   0 tobias    (7385) tobias    (7385)     8630 2023-07-18 16:05:31.000000 caldav-1.3.2/tests/conf_private.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     3119 2023-05-22 07:00:24.000000 caldav-1.3.2/tests/conf_private.py.EXAMPLE
--rw-------   0 tobias    (7385) tobias    (7385)     8629 2023-05-24 23:13:12.000000 caldav-1.3.2/tests/conf_private.py~
--rw-r--r--   0 tobias    (7385) tobias    (7385)    11408 2023-07-18 22:32:35.000000 caldav-1.3.2/tests/proxy.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)    98646 2023-07-18 22:32:35.000000 caldav-1.3.2/tests/test_caldav.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)    97373 2023-02-16 21:52:31.000000 caldav-1.3.2/tests/test_caldav.py.orig
--rw-r--r--   0 tobias    (7385) tobias    (7385)      543 2023-02-14 23:21:07.000000 caldav-1.3.2/tests/test_caldav.py.rej
--rw-r--r--   0 tobias    (7385) tobias    (7385)    45062 2023-07-18 22:32:35.000000 caldav-1.3.2/tests/test_caldav_unit.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     1965 2023-05-22 07:00:24.000000 caldav-1.3.2/tests/test_cdav.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)      517 2023-05-22 07:00:24.000000 caldav-1.3.2/tests/test_utils.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)      487 2022-01-07 16:03:24.000000 caldav-1.3.2/tests/test_utils.py~
--rw-r--r--   0 tobias    (7385) tobias    (7385)     7959 2023-07-18 22:32:35.000000 caldav-1.3.2/tests/test_vcal.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)       54 2021-11-26 23:08:18.000000 caldav-1.3.2/tests/test_vcal.py~
--rw-r--r--   0 tobias    (7385) tobias    (7385)      906 2022-11-02 08:07:32.000000 caldav-1.3.2/tests/tmp_226~
+drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-19 13:39:09.335202 caldav-1.3.3/
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    11358 2019-09-10 16:18:00.000000 caldav-1.3.3/COPYING.APACHE
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    35147 2019-09-10 16:18:00.000000 caldav-1.3.3/COPYING.GPL
+-rw-r--r--   0 tobias    (7385) tobias    (7385)       87 2023-05-22 07:00:24.000000 caldav-1.3.3/MANIFEST.in
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     1354 2023-07-19 13:39:09.335202 caldav-1.3.3/PKG-INFO
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      635 2023-05-22 07:00:24.000000 caldav-1.3.3/README.md
+drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-19 13:39:09.325202 caldav-1.3.3/caldav/
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      543 2023-07-19 13:37:36.000000 caldav-1.3.3/caldav/__init__.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    25502 2023-07-18 22:32:35.000000 caldav-1.3.3/caldav/davclient.py
+drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-19 13:39:09.325202 caldav-1.3.3/caldav/elements/
+-rw-r--r--   0 tobias    (7385) tobias    (7385)       48 2023-05-22 07:00:24.000000 caldav-1.3.3/caldav/elements/__init__.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     1945 2023-07-18 22:32:35.000000 caldav-1.3.3/caldav/elements/base.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     4935 2023-05-22 07:00:24.000000 caldav-1.3.3/caldav/elements/cdav.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     1609 2023-05-22 07:00:24.000000 caldav-1.3.3/caldav/elements/dav.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      319 2023-05-22 07:00:24.000000 caldav-1.3.3/caldav/elements/ical.py
+drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-19 13:39:09.325202 caldav-1.3.3/caldav/lib/
+-rw-r--r--   0 tobias    (7385) tobias    (7385)        0 2019-09-10 16:18:00.000000 caldav-1.3.3/caldav/lib/__init__.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      231 2023-07-18 22:45:26.000000 caldav-1.3.3/caldav/lib/debug.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     2540 2023-07-18 22:01:33.000000 caldav-1.3.3/caldav/lib/error.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      668 2023-05-22 07:00:24.000000 caldav-1.3.3/caldav/lib/namespace.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      798 2023-07-18 22:32:35.000000 caldav-1.3.3/caldav/lib/python_utilities.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     6480 2023-07-18 22:32:35.000000 caldav-1.3.3/caldav/lib/url.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     7450 2023-07-18 22:32:35.000000 caldav-1.3.3/caldav/lib/vcal.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)   109108 2023-07-19 13:05:08.000000 caldav-1.3.3/caldav/objects.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      402 2023-05-22 07:00:24.000000 caldav-1.3.3/caldav/requests.py
+drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-19 13:39:09.325202 caldav-1.3.3/caldav.egg-info/
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     1354 2023-07-19 13:39:09.000000 caldav-1.3.3/caldav.egg-info/PKG-INFO
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     3878 2023-07-19 13:39:09.000000 caldav-1.3.3/caldav.egg-info/SOURCES.txt
+-rw-r--r--   0 tobias    (7385) tobias    (7385)        1 2023-07-19 13:39:09.000000 caldav-1.3.3/caldav.egg-info/dependency_links.txt
+-rw-r--r--   0 tobias    (7385) tobias    (7385)        1 2022-11-22 09:14:37.000000 caldav-1.3.3/caldav.egg-info/not-zip-safe
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      130 2023-07-19 13:39:09.000000 caldav-1.3.3/caldav.egg-info/requires.txt
+-rw-r--r--   0 tobias    (7385) tobias    (7385)        7 2023-07-19 13:39:09.000000 caldav-1.3.3/caldav.egg-info/top_level.txt
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      506 2023-07-19 13:39:09.338535 caldav-1.3.3/setup.cfg
+-rwxr-xr-x   0 tobias    (7385) tobias    (7385)     2877 2023-07-18 22:32:35.000000 caldav-1.3.3/setup.py
+drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-19 13:39:09.328535 caldav-1.3.3/tests/
+-rw-------   0 tobias    (7385) tobias    (7385)     8630 2023-05-25 19:43:46.000000 caldav-1.3.3/tests/#conf_private.py#
+-rwxr-xr-x   0 tobias    (7385) tobias    (7385)      888 2022-11-03 16:22:35.000000 caldav-1.3.3/tests/#tmp_226.py#
+-rw-r--r--   0 tobias    (7385) tobias    (7385)        0 2019-09-10 16:18:00.000000 caldav-1.3.3/tests/__init__.py
+drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-19 13:39:09.335202 caldav-1.3.3/tests/__pycache__/
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      130 2022-01-05 17:28:37.000000 caldav-1.3.3/tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      146 2023-05-22 06:28:45.000000 caldav-1.3.3/tests/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      128 2021-10-10 21:24:31.000000 caldav-1.3.3/tests/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     7969 2023-02-25 18:55:46.000000 caldav-1.3.3/tests/__pycache__/compatibility_issues.cpython-310.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     8694 2023-07-19 10:22:04.000000 caldav-1.3.3/tests/__pycache__/compatibility_issues.cpython-311.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     4188 2021-11-10 00:21:31.000000 caldav-1.3.3/tests/__pycache__/compatibility_issues.cpython-39.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     2401 2023-02-14 21:14:51.000000 caldav-1.3.3/tests/__pycache__/conf.cpython-310.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     3722 2023-05-24 11:30:31.000000 caldav-1.3.3/tests/__pycache__/conf.cpython-311.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     1788 2021-10-10 21:24:45.000000 caldav-1.3.3/tests/__pycache__/conf.cpython-39.pyc
+-rw-------   0 tobias    (7385) tobias    (7385)     2949 2023-03-06 14:30:08.000000 caldav-1.3.3/tests/__pycache__/conf_private.cpython-310.pyc
+-rw-------   0 tobias    (7385) tobias    (7385)     3638 2023-07-18 16:05:33.000000 caldav-1.3.3/tests/__pycache__/conf_private.cpython-311.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      709 2021-11-30 09:55:30.000000 caldav-1.3.3/tests/__pycache__/conf_private.cpython-39.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    10615 2023-02-27 20:25:36.000000 caldav-1.3.3/tests/__pycache__/proxy.cpython-310.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    19912 2023-07-19 10:22:04.000000 caldav-1.3.3/tests/__pycache__/proxy.cpython-311.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    10615 2021-10-10 21:24:45.000000 caldav-1.3.3/tests/__pycache__/proxy.cpython-39.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    99664 2022-11-01 22:32:56.000000 caldav-1.3.3/tests/__pycache__/test_caldav.cpython-310-pytest-7.1.3.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)   108125 2023-01-15 22:21:23.000000 caldav-1.3.3/tests/__pycache__/test_caldav.cpython-310-pytest-7.2.0.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)   115157 2023-03-06 14:51:44.000000 caldav-1.3.3/tests/__pycache__/test_caldav.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)   115163 2023-03-13 07:21:44.000000 caldav-1.3.3/tests/__pycache__/test_caldav.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    55936 2023-03-06 14:15:55.000000 caldav-1.3.3/tests/__pycache__/test_caldav.cpython-310.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)   346344 2023-05-24 11:30:31.000000 caldav-1.3.3/tests/__pycache__/test_caldav.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)   353122 2023-07-19 10:22:03.000000 caldav-1.3.3/tests/__pycache__/test_caldav.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    41792 2021-12-02 18:17:39.000000 caldav-1.3.3/tests/__pycache__/test_caldav.cpython-39.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    61467 2022-11-01 22:32:56.000000 caldav-1.3.3/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.1.3.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    62010 2023-01-15 22:21:23.000000 caldav-1.3.3/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.0.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    63615 2023-02-27 20:25:36.000000 caldav-1.3.3/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    63618 2023-03-13 07:21:45.000000 caldav-1.3.3/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    33628 2023-03-06 14:13:09.000000 caldav-1.3.3/tests/__pycache__/test_caldav_unit.cpython-310.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)   160045 2023-05-24 11:30:31.000000 caldav-1.3.3/tests/__pycache__/test_caldav_unit.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)   160045 2023-07-19 10:22:04.000000 caldav-1.3.3/tests/__pycache__/test_caldav_unit.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    26186 2021-10-10 21:24:31.000000 caldav-1.3.3/tests/__pycache__/test_caldav_unit.cpython-39.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     4379 2022-10-04 22:09:32.000000 caldav-1.3.3/tests/__pycache__/test_cdav.cpython-310-pytest-7.1.3.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     4379 2022-11-21 19:20:28.000000 caldav-1.3.3/tests/__pycache__/test_cdav.cpython-310-pytest-7.2.0.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     4379 2023-01-16 00:55:21.000000 caldav-1.3.3/tests/__pycache__/test_cdav.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     4379 2023-03-13 07:21:45.000000 caldav-1.3.3/tests/__pycache__/test_cdav.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     2057 2023-03-06 14:13:09.000000 caldav-1.3.3/tests/__pycache__/test_cdav.cpython-310.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    10956 2023-05-24 11:30:31.000000 caldav-1.3.3/tests/__pycache__/test_cdav.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    10956 2023-07-10 18:48:32.000000 caldav-1.3.3/tests/__pycache__/test_cdav.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     2029 2021-10-10 21:24:31.000000 caldav-1.3.3/tests/__pycache__/test_cdav.cpython-39.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      793 2022-10-04 22:09:32.000000 caldav-1.3.3/tests/__pycache__/test_utils.cpython-310-pytest-7.1.3.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      793 2022-11-21 19:20:28.000000 caldav-1.3.3/tests/__pycache__/test_utils.cpython-310-pytest-7.2.0.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      793 2023-01-16 00:55:21.000000 caldav-1.3.3/tests/__pycache__/test_utils.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      793 2023-03-13 07:21:45.000000 caldav-1.3.3/tests/__pycache__/test_utils.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      684 2023-03-06 14:13:09.000000 caldav-1.3.3/tests/__pycache__/test_utils.cpython-310.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     1527 2023-05-24 11:30:31.000000 caldav-1.3.3/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     1527 2023-07-10 18:48:32.000000 caldav-1.3.3/tests/__pycache__/test_utils.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     3372 2022-10-04 22:09:32.000000 caldav-1.3.3/tests/__pycache__/test_vcal.cpython-310-pytest-7.1.3.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     7304 2023-01-15 22:21:23.000000 caldav-1.3.3/tests/__pycache__/test_vcal.cpython-310-pytest-7.2.0.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     7304 2023-02-11 09:38:03.000000 caldav-1.3.3/tests/__pycache__/test_vcal.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     8024 2023-03-13 07:21:45.000000 caldav-1.3.3/tests/__pycache__/test_vcal.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     5975 2023-03-06 14:13:09.000000 caldav-1.3.3/tests/__pycache__/test_vcal.cpython-310.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    15151 2023-05-24 11:30:31.000000 caldav-1.3.3/tests/__pycache__/test_vcal.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    15151 2023-07-19 10:22:04.000000 caldav-1.3.3/tests/__pycache__/test_vcal.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     2650 2021-11-30 08:41:46.000000 caldav-1.3.3/tests/__pycache__/test_vcal.cpython-39.pyc
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     1290 2023-05-22 07:00:24.000000 caldav-1.3.3/tests/_test_absolute.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    14105 2023-07-18 22:32:35.000000 caldav-1.3.3/tests/compatibility_issues.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     4909 2023-05-22 07:00:24.000000 caldav-1.3.3/tests/conf.py
+-rw-------   0 tobias    (7385) tobias    (7385)     8630 2023-07-18 16:05:31.000000 caldav-1.3.3/tests/conf_private.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     3119 2023-05-22 07:00:24.000000 caldav-1.3.3/tests/conf_private.py.EXAMPLE
+-rw-------   0 tobias    (7385) tobias    (7385)     8629 2023-05-24 23:13:12.000000 caldav-1.3.3/tests/conf_private.py~
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    11408 2023-07-18 22:32:35.000000 caldav-1.3.3/tests/proxy.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    98646 2023-07-18 22:32:35.000000 caldav-1.3.3/tests/test_caldav.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    97373 2023-02-16 21:52:31.000000 caldav-1.3.3/tests/test_caldav.py.orig
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      543 2023-02-14 23:21:07.000000 caldav-1.3.3/tests/test_caldav.py.rej
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    45062 2023-07-18 22:32:35.000000 caldav-1.3.3/tests/test_caldav_unit.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     1965 2023-05-22 07:00:24.000000 caldav-1.3.3/tests/test_cdav.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      517 2023-05-22 07:00:24.000000 caldav-1.3.3/tests/test_utils.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      487 2022-01-07 16:03:24.000000 caldav-1.3.3/tests/test_utils.py~
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     7959 2023-07-18 22:32:35.000000 caldav-1.3.3/tests/test_vcal.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)       54 2021-11-26 23:08:18.000000 caldav-1.3.3/tests/test_vcal.py~
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      906 2022-11-02 08:07:32.000000 caldav-1.3.3/tests/tmp_226~
```

### Comparing `caldav-1.3.2/COPYING.APACHE` & `caldav-1.3.3/COPYING.APACHE`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/COPYING.GPL` & `caldav-1.3.3/COPYING.GPL`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/PKG-INFO` & `caldav-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caldav
-Version: 1.3.2
+Version: 1.3.3
 Summary: CalDAV (RFC4791) client library
 Home-page: https://github.com/python-caldav/caldav
 Author: Cyril Robert
 Author-email: cyril@hippie.io
 License: GPL
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `caldav-1.3.2/README.md` & `caldav-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/caldav/__init__.py` & `caldav-1.3.3/caldav/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 import logging
 
 import vobject.icalendar
 
-__version__ = "1.3.2"
+__version__ = "1.3.3"
 
 from .davclient import DAVClient
 from .objects import *
 
 ## Notes:
 ##
 ## * The vobject.icalendar has (or had?) to be explicitly imported due to some bug in the tBaxter fork of vobject.
```

### Comparing `caldav-1.3.2/caldav/davclient.py` & `caldav-1.3.3/caldav/davclient.py`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/caldav/elements/base.py` & `caldav-1.3.3/caldav/elements/base.py`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/caldav/elements/cdav.py` & `caldav-1.3.3/caldav/elements/cdav.py`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/caldav/elements/dav.py` & `caldav-1.3.3/caldav/elements/dav.py`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/caldav/lib/error.py` & `caldav-1.3.3/caldav/lib/error.py`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/caldav/lib/namespace.py` & `caldav-1.3.3/caldav/lib/namespace.py`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/caldav/lib/python_utilities.py` & `caldav-1.3.3/caldav/lib/python_utilities.py`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/caldav/lib/url.py` & `caldav-1.3.3/caldav/lib/url.py`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/caldav/lib/vcal.py` & `caldav-1.3.3/caldav/lib/vcal.py`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/caldav/objects.py` & `caldav-1.3.3/caldav/objects.py`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/caldav.egg-info/PKG-INFO` & `caldav-1.3.3/caldav.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caldav
-Version: 1.3.2
+Version: 1.3.3
 Summary: CalDAV (RFC4791) client library
 Home-page: https://github.com/python-caldav/caldav
 Author: Cyril Robert
 Author-email: cyril@hippie.io
 License: GPL
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `caldav-1.3.2/caldav.egg-info/SOURCES.txt` & `caldav-1.3.3/caldav.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/setup.py` & `caldav-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/#conf_private.py#` & `caldav-1.3.3/tests/#conf_private.py#`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/#tmp_226.py#` & `caldav-1.3.3/tests/#tmp_226.py#`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/compatibility_issues.cpython-310.pyc` & `caldav-1.3.3/tests/__pycache__/compatibility_issues.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/compatibility_issues.cpython-311.pyc` & `caldav-1.3.3/tests/__pycache__/compatibility_issues.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/compatibility_issues.cpython-39.pyc` & `caldav-1.3.3/tests/__pycache__/compatibility_issues.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/conf.cpython-310.pyc` & `caldav-1.3.3/tests/__pycache__/conf.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/conf.cpython-311.pyc` & `caldav-1.3.3/tests/__pycache__/conf.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/conf.cpython-39.pyc` & `caldav-1.3.3/tests/__pycache__/conf.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/conf_private.cpython-310.pyc` & `caldav-1.3.3/tests/__pycache__/conf_private.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/conf_private.cpython-311.pyc` & `caldav-1.3.3/tests/__pycache__/conf_private.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/conf_private.cpython-39.pyc` & `caldav-1.3.3/tests/__pycache__/conf_private.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/proxy.cpython-310.pyc` & `caldav-1.3.3/tests/__pycache__/proxy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/proxy.cpython-311.pyc` & `caldav-1.3.3/tests/__pycache__/proxy.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/proxy.cpython-39.pyc` & `caldav-1.3.3/tests/__pycache__/proxy.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_caldav.cpython-310-pytest-7.1.3.pyc` & `caldav-1.3.3/tests/__pycache__/test_caldav.cpython-310-pytest-7.1.3.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_caldav.cpython-310-pytest-7.2.0.pyc` & `caldav-1.3.3/tests/__pycache__/test_caldav.cpython-310-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_caldav.cpython-310-pytest-7.2.1.pyc` & `caldav-1.3.3/tests/__pycache__/test_caldav.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_caldav.cpython-310-pytest-7.2.2.pyc` & `caldav-1.3.3/tests/__pycache__/test_caldav.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_caldav.cpython-310.pyc` & `caldav-1.3.3/tests/__pycache__/test_caldav.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_caldav.cpython-311-pytest-7.3.1.pyc` & `caldav-1.3.3/tests/__pycache__/test_caldav.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_caldav.cpython-311-pytest-7.4.0.pyc` & `caldav-1.3.3/tests/__pycache__/test_caldav.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_caldav.cpython-39.pyc` & `caldav-1.3.3/tests/__pycache__/test_caldav.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.1.3.pyc` & `caldav-1.3.3/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.1.3.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.0.pyc` & `caldav-1.3.3/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.1.pyc` & `caldav-1.3.3/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.2.pyc` & `caldav-1.3.3/tests/__pycache__/test_caldav_unit.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-310.pyc` & `caldav-1.3.3/tests/__pycache__/test_caldav_unit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-311-pytest-7.3.1.pyc` & `caldav-1.3.3/tests/__pycache__/test_caldav_unit.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-311-pytest-7.4.0.pyc` & `caldav-1.3.3/tests/__pycache__/test_caldav_unit.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_caldav_unit.cpython-39.pyc` & `caldav-1.3.3/tests/__pycache__/test_caldav_unit.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_cdav.cpython-310-pytest-7.1.3.pyc` & `caldav-1.3.3/tests/__pycache__/test_cdav.cpython-310-pytest-7.1.3.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_cdav.cpython-310-pytest-7.2.0.pyc` & `caldav-1.3.3/tests/__pycache__/test_cdav.cpython-310-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_cdav.cpython-310-pytest-7.2.1.pyc` & `caldav-1.3.3/tests/__pycache__/test_cdav.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_cdav.cpython-310-pytest-7.2.2.pyc` & `caldav-1.3.3/tests/__pycache__/test_cdav.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_cdav.cpython-310.pyc` & `caldav-1.3.3/tests/__pycache__/test_cdav.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_cdav.cpython-311-pytest-7.3.1.pyc` & `caldav-1.3.3/tests/__pycache__/test_cdav.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_cdav.cpython-311-pytest-7.4.0.pyc` & `caldav-1.3.3/tests/__pycache__/test_cdav.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_cdav.cpython-39.pyc` & `caldav-1.3.3/tests/__pycache__/test_cdav.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_utils.cpython-310-pytest-7.1.3.pyc` & `caldav-1.3.3/tests/__pycache__/test_utils.cpython-310-pytest-7.1.3.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_utils.cpython-310-pytest-7.2.0.pyc` & `caldav-1.3.3/tests/__pycache__/test_utils.cpython-310-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_utils.cpython-310-pytest-7.2.1.pyc` & `caldav-1.3.3/tests/__pycache__/test_utils.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_utils.cpython-310-pytest-7.2.2.pyc` & `caldav-1.3.3/tests/__pycache__/test_utils.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_utils.cpython-310.pyc` & `caldav-1.3.3/tests/__pycache__/test_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc` & `caldav-1.3.3/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_utils.cpython-311-pytest-7.4.0.pyc` & `caldav-1.3.3/tests/__pycache__/test_utils.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_vcal.cpython-310-pytest-7.1.3.pyc` & `caldav-1.3.3/tests/__pycache__/test_vcal.cpython-310-pytest-7.1.3.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_vcal.cpython-310-pytest-7.2.0.pyc` & `caldav-1.3.3/tests/__pycache__/test_vcal.cpython-310-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_vcal.cpython-310-pytest-7.2.1.pyc` & `caldav-1.3.3/tests/__pycache__/test_vcal.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_vcal.cpython-310-pytest-7.2.2.pyc` & `caldav-1.3.3/tests/__pycache__/test_vcal.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_vcal.cpython-310.pyc` & `caldav-1.3.3/tests/__pycache__/test_vcal.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_vcal.cpython-311-pytest-7.3.1.pyc` & `caldav-1.3.3/tests/__pycache__/test_vcal.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_vcal.cpython-311-pytest-7.4.0.pyc` & `caldav-1.3.3/tests/__pycache__/test_vcal.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/__pycache__/test_vcal.cpython-39.pyc` & `caldav-1.3.3/tests/__pycache__/test_vcal.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/_test_absolute.py` & `caldav-1.3.3/tests/_test_absolute.py`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/compatibility_issues.py` & `caldav-1.3.3/tests/compatibility_issues.py`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/conf.py` & `caldav-1.3.3/tests/conf.py`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/conf_private.py` & `caldav-1.3.3/tests/conf_private.py`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/conf_private.py.EXAMPLE` & `caldav-1.3.3/tests/conf_private.py.EXAMPLE`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/conf_private.py~` & `caldav-1.3.3/tests/conf_private.py~`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/proxy.py` & `caldav-1.3.3/tests/proxy.py`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/test_caldav.py` & `caldav-1.3.3/tests/test_caldav.py`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/test_caldav.py.orig` & `caldav-1.3.3/tests/test_caldav.py.orig`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/test_caldav.py.rej` & `caldav-1.3.3/tests/test_caldav.py.rej`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/test_caldav_unit.py` & `caldav-1.3.3/tests/test_caldav_unit.py`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/test_cdav.py` & `caldav-1.3.3/tests/test_cdav.py`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/test_utils.py` & `caldav-1.3.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/test_vcal.py` & `caldav-1.3.3/tests/test_vcal.py`

 * *Files identical despite different names*

### Comparing `caldav-1.3.2/tests/tmp_226~` & `caldav-1.3.3/tests/tmp_226~`

 * *Files identical despite different names*

