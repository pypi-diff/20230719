# Comparing `tmp/yams-0.49.3.tar.gz` & `tmp/yams-0.50.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yams-0.49.3.tar", last modified: Fri Mar 10 15:37:01 2023, max compression
+gzip compressed data, was "yams-0.50.0.tar", last modified: Wed Jul 19 08:48:09 2023, max compression
```

## Comparing `yams-0.49.3.tar` & `yams-0.50.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:37:01.909863 yams-0.49.3/
--rw-rw-rw-   0 root         (0) root         (0)    17987 2023-03-10 15:36:49.000000 yams-0.49.3/COPYING
--rw-rw-rw-   0 root         (0) root         (0)    26527 2023-03-10 15:36:49.000000 yams-0.49.3/COPYING.LESSER
--rw-rw-rw-   0 root         (0) root         (0)    13724 2023-03-10 15:36:49.000000 yams-0.49.3/ChangeLog
--rw-rw-rw-   0 root         (0) root         (0)      469 2023-03-10 15:36:49.000000 yams-0.49.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1397 2023-03-10 15:37:01.909863 yams-0.49.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      969 2023-03-10 15:36:49.000000 yams-0.49.3/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1681 2023-03-10 15:36:49.000000 yams-0.49.3/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:37:01.889862 yams-0.49.3/bin/
--rwxrwxrwx   0 root         (0) root         (0)     3838 2023-03-10 15:36:49.000000 yams-0.49.3/bin/owl2yams
--rwxrwxrwx   0 root         (0) root         (0)       94 2023-03-10 15:36:49.000000 yams-0.49.3/bin/yams-check
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-03-10 15:36:49.000000 yams-0.49.3/bin/yams-check.bat
--rwxrwxrwx   0 root         (0) root         (0)       94 2023-03-10 15:36:49.000000 yams-0.49.3/bin/yams-view
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-03-10 15:36:49.000000 yams-0.49.3/bin/yams-view.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:37:01.893862 yams-0.49.3/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-03-10 15:36:49.000000 yams-0.49.3/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     1923 2023-03-10 15:36:49.000000 yams-0.49.3/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-03-10 15:36:49.000000 yams-0.49.3/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-03-10 15:36:49.000000 yams-0.49.3/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)     1415 2023-03-10 15:36:49.000000 yams-0.49.3/docs/yams.rst
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-03-10 15:36:49.000000 yams-0.49.3/mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-03-10 15:36:49.000000 yams-0.49.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-10 15:37:01.909863 yams-0.49.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2095 2023-03-10 15:36:49.000000 yams-0.49.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:37:01.897863 yams-0.49.3/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:37:01.897863 yams-0.49.3/test/data/
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-03-10 15:36:49.000000 yams-0.49.3/test/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:37:01.897863 yams-0.49.3/test/data/dbmodel/
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-03-10 15:36:49.000000 yams-0.49.3/test/data/dbmodel/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1274 2023-03-10 15:36:49.000000 yams-0.49.3/test/data/dbmodel/blog.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:37:01.901862 yams-0.49.3/test/data/schema/
--rw-rw-rw-   0 root         (0) root         (0)     2470 2023-03-10 15:36:49.000000 yams-0.49.3/test/data/schema/Company.py
--rw-rw-rw-   0 root         (0) root         (0)     1135 2023-03-10 15:36:49.000000 yams-0.49.3/test/data/schema/Dates.py
--rw-rw-rw-   0 root         (0) root         (0)     3252 2023-03-10 15:36:49.000000 yams-0.49.3/test/data/schema/State.py
--rw-rw-rw-   0 root         (0) root         (0)      978 2023-03-10 15:36:49.000000 yams-0.49.3/test/data/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3610 2023-03-10 15:36:49.000000 yams-0.49.3/test/data/schema/schema.py
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-03-10 15:36:49.000000 yams-0.49.3/test/data/schema/toignore
--rw-rw-rw-   0 root         (0) root         (0)     1625 2023-03-10 15:36:49.000000 yams-0.49.3/test/data/schema1.txt
--rw-rw-rw-   0 root         (0) root         (0)     1489 2023-03-10 15:36:49.000000 yams-0.49.3/test/data/schema2.txt
--rw-rw-rw-   0 root         (0) root         (0)      925 2023-03-10 15:36:49.000000 yams-0.49.3/test/data/schema_post_build_callback.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:37:01.901862 yams-0.49.3/test/data2/
--rw-rw-rw-   0 root         (0) root         (0)      821 2023-03-10 15:36:49.000000 yams-0.49.3/test/data2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-03-10 15:36:49.000000 yams-0.49.3/test/data2/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    12011 2023-03-10 15:36:49.000000 yams-0.49.3/test/unittest_constraints.py
--rw-rw-rw-   0 root         (0) root         (0)     6356 2023-03-10 15:36:49.000000 yams-0.49.3/test/unittest_diff.py
--rw-rw-rw-   0 root         (0) root         (0)    36196 2023-03-10 15:36:49.000000 yams-0.49.3/test/unittest_reader.py
--rw-rw-rw-   0 root         (0) root         (0)    29241 2023-03-10 15:36:49.000000 yams-0.49.3/test/unittest_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     2742 2023-03-10 15:36:49.000000 yams-0.49.3/test/unittest_schema2dot.py
--rw-rw-rw-   0 root         (0) root         (0)     2313 2023-03-10 15:36:49.000000 yams-0.49.3/test/unittest_serialize.py
--rw-rw-rw-   0 root         (0) root         (0)     9952 2023-03-10 15:36:49.000000 yams-0.49.3/test/unittest_specialization.py
--rw-rw-rw-   0 root         (0) root         (0)     2497 2023-03-10 15:36:49.000000 yams-0.49.3/test/unittest_xy.py
--rw-rw-rw-   0 root         (0) root         (0)     2559 2023-03-10 15:36:49.000000 yams-0.49.3/tox.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:37:01.905863 yams-0.49.3/yams/
--rw-rw-rw-   0 root         (0) root         (0)     7151 2023-03-10 15:36:49.000000 yams-0.49.3/yams/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5183 2023-03-10 15:36:49.000000 yams-0.49.3/yams/_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    39853 2023-03-10 15:36:49.000000 yams-0.49.3/yams/buildobjs.py
--rw-rw-rw-   0 root         (0) root         (0)    28708 2023-03-10 15:36:49.000000 yams-0.49.3/yams/constraints.py
--rw-rw-rw-   0 root         (0) root         (0)    12410 2023-03-10 15:36:49.000000 yams-0.49.3/yams/diff.py
--rw-rw-rw-   0 root         (0) root         (0)     6181 2023-03-10 15:36:49.000000 yams-0.49.3/yams/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-10 15:36:49.000000 yams-0.49.3/yams/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    16243 2023-03-10 15:36:49.000000 yams-0.49.3/yams/reader.py
--rw-rw-rw-   0 root         (0) root         (0)    71400 2023-03-10 15:36:49.000000 yams-0.49.3/yams/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    12618 2023-03-10 15:36:49.000000 yams-0.49.3/yams/schema2dot.py
--rw-rw-rw-   0 root         (0) root         (0)     1681 2023-03-10 15:36:49.000000 yams-0.49.3/yams/serialize.py
--rw-rw-rw-   0 root         (0) root         (0)     4512 2023-03-10 15:36:49.000000 yams-0.49.3/yams/tools.py
--rw-rw-rw-   0 root         (0) root         (0)     2272 2023-03-10 15:36:49.000000 yams-0.49.3/yams/types.py
--rw-rw-rw-   0 root         (0) root         (0)     5851 2023-03-10 15:36:49.000000 yams-0.49.3/yams/xy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 15:37:01.909863 yams-0.49.3/yams.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1397 2023-03-10 15:37:01.000000 yams-0.49.3/yams.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1218 2023-03-10 15:37:01.000000 yams-0.49.3/yams.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-10 15:37:01.000000 yams-0.49.3/yams.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-03-10 15:37:01.000000 yams-0.49.3/yams.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-03-10 15:37:01.000000 yams-0.49.3/yams.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    21077 2023-03-10 15:36:49.000000 yams-0.49.3/yams.png
--rw-rw-rw-   0 root         (0) root         (0)     5326 2023-03-10 15:36:49.000000 yams-0.49.3/yams.svg
+drwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)        0 2023-07-19 08:48:09.471916 yams-0.50.0/
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    17987 2023-07-17 22:32:31.000000 yams-0.50.0/COPYING
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    26527 2023-07-17 22:32:31.000000 yams-0.50.0/COPYING.LESSER
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    13724 2023-07-17 22:32:31.000000 yams-0.50.0/ChangeLog
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      469 2023-07-17 22:32:31.000000 yams-0.50.0/MANIFEST.in
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     1397 2023-07-19 08:48:09.471916 yams-0.50.0/PKG-INFO
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      969 2023-07-17 22:32:31.000000 yams-0.50.0/README.rst
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     1679 2023-07-19 08:36:22.000000 yams-0.50.0/__pkginfo__.py
+drwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)        0 2023-07-19 08:48:09.459916 yams-0.50.0/bin/
+-rwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)     3838 2023-07-17 22:32:31.000000 yams-0.50.0/bin/owl2yams
+-rwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)       94 2023-07-17 22:32:31.000000 yams-0.50.0/bin/yams-check
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      360 2023-07-17 22:32:31.000000 yams-0.50.0/bin/yams-check.bat
+-rwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)       94 2023-07-17 22:32:31.000000 yams-0.50.0/bin/yams-view
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      360 2023-07-17 22:32:31.000000 yams-0.50.0/bin/yams-view.bat
+drwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)        0 2023-07-19 08:48:09.459916 yams-0.50.0/docs/
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      634 2023-07-17 22:32:31.000000 yams-0.50.0/docs/Makefile
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     1923 2023-07-17 22:32:31.000000 yams-0.50.0/docs/conf.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      460 2023-07-17 22:32:31.000000 yams-0.50.0/docs/index.rst
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      760 2023-07-17 22:32:31.000000 yams-0.50.0/docs/make.bat
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     1415 2023-07-17 22:32:31.000000 yams-0.50.0/docs/yams.rst
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)       74 2023-07-17 22:32:31.000000 yams-0.50.0/mypy.ini
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      244 2023-07-17 22:32:31.000000 yams-0.50.0/pyproject.toml
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)       38 2023-07-19 08:48:09.475916 yams-0.50.0/setup.cfg
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     2095 2023-07-17 22:32:31.000000 yams-0.50.0/setup.py
+drwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)        0 2023-07-19 08:48:09.463916 yams-0.50.0/test/
+drwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)        0 2023-07-19 08:48:09.463916 yams-0.50.0/test/data/
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      824 2023-07-17 22:32:31.000000 yams-0.50.0/test/data/__init__.py
+drwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)        0 2023-07-19 08:48:09.463916 yams-0.50.0/test/data/dbmodel/
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      815 2023-07-17 22:32:31.000000 yams-0.50.0/test/data/dbmodel/__init__.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     1274 2023-07-17 22:32:31.000000 yams-0.50.0/test/data/dbmodel/blog.py
+drwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)        0 2023-07-19 08:48:09.463916 yams-0.50.0/test/data/schema/
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     2470 2023-07-17 22:32:31.000000 yams-0.50.0/test/data/schema/Company.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     1135 2023-07-17 22:32:31.000000 yams-0.50.0/test/data/schema/Dates.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     3252 2023-07-17 22:32:31.000000 yams-0.50.0/test/data/schema/State.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      978 2023-07-17 22:32:31.000000 yams-0.50.0/test/data/schema/__init__.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     3610 2023-07-17 22:32:31.000000 yams-0.50.0/test/data/schema/schema.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)        7 2023-07-17 22:32:31.000000 yams-0.50.0/test/data/schema/toignore
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     1625 2023-07-17 22:32:31.000000 yams-0.50.0/test/data/schema1.txt
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     1489 2023-07-17 22:32:31.000000 yams-0.50.0/test/data/schema2.txt
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      925 2023-07-17 22:32:31.000000 yams-0.50.0/test/data/schema_post_build_callback.py
+drwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)        0 2023-07-19 08:48:09.467916 yams-0.50.0/test/data2/
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)      821 2023-07-17 22:32:31.000000 yams-0.50.0/test/data2/__init__.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     1067 2023-07-17 22:32:31.000000 yams-0.50.0/test/data2/schema.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    13040 2023-07-17 22:32:31.000000 yams-0.50.0/test/unittest_constraints.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     6356 2023-07-17 22:32:31.000000 yams-0.50.0/test/unittest_diff.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    36195 2023-07-17 22:32:31.000000 yams-0.50.0/test/unittest_reader.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    29219 2023-07-17 22:32:31.000000 yams-0.50.0/test/unittest_schema.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     2742 2023-07-17 22:32:31.000000 yams-0.50.0/test/unittest_schema2dot.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     2313 2023-07-17 22:32:31.000000 yams-0.50.0/test/unittest_serialize.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     9932 2023-07-19 08:36:00.000000 yams-0.50.0/test/unittest_specialization.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     2497 2023-07-17 22:32:31.000000 yams-0.50.0/test/unittest_xy.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     2559 2023-07-17 22:32:31.000000 yams-0.50.0/tox.ini
+drwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)        0 2023-07-19 08:48:09.467916 yams-0.50.0/yams/
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     7211 2023-07-19 08:36:00.000000 yams-0.50.0/yams/__init__.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     5163 2023-07-19 08:36:00.000000 yams-0.50.0/yams/_exceptions.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    39988 2023-07-19 08:41:42.000000 yams-0.50.0/yams/buildobjs.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    29393 2023-07-19 08:36:00.000000 yams-0.50.0/yams/constraints.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    12344 2023-07-19 08:36:00.000000 yams-0.50.0/yams/diff.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     6181 2023-07-17 22:32:31.000000 yams-0.50.0/yams/interfaces.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)        0 2023-07-17 22:32:31.000000 yams-0.50.0/yams/py.typed
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    16241 2023-07-19 08:36:00.000000 yams-0.50.0/yams/reader.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    71338 2023-07-19 08:36:00.000000 yams-0.50.0/yams/schema.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    12618 2023-07-17 22:32:31.000000 yams-0.50.0/yams/schema2dot.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     1665 2023-07-19 08:36:00.000000 yams-0.50.0/yams/serialize.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     4506 2023-07-19 08:36:00.000000 yams-0.50.0/yams/tools.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     2272 2023-07-17 22:32:31.000000 yams-0.50.0/yams/types.py
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     5851 2023-07-19 08:36:00.000000 yams-0.50.0/yams/xy.py
+drwxrwxr-x   0 psycojoker  (1000) psycojoker  (1000)        0 2023-07-19 08:48:09.471916 yams-0.50.0/yams.egg-info/
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     1397 2023-07-19 08:48:09.000000 yams-0.50.0/yams.egg-info/PKG-INFO
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     1218 2023-07-19 08:48:09.000000 yams-0.50.0/yams.egg-info/SOURCES.txt
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)        1 2023-07-19 08:48:09.000000 yams-0.50.0/yams.egg-info/dependency_links.txt
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)       49 2023-07-19 08:48:09.000000 yams-0.50.0/yams.egg-info/requires.txt
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)        5 2023-07-19 08:48:09.000000 yams-0.50.0/yams.egg-info/top_level.txt
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)    21077 2023-07-17 22:32:31.000000 yams-0.50.0/yams.png
+-rw-rw-r--   0 psycojoker  (1000) psycojoker  (1000)     5326 2023-07-17 22:32:31.000000 yams-0.50.0/yams.svg
```

### Comparing `yams-0.49.3/COPYING` & `yams-0.50.0/COPYING`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/COPYING.LESSER` & `yams-0.50.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/ChangeLog` & `yams-0.50.0/ChangeLog`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/PKG-INFO` & `yams-0.50.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yams
-Version: 0.49.3
+Version: 0.50.0
 Summary: entity / relation schema
 Home-page: https://forge.extranet.logilab.fr/open-source/yams
 Author: Logilab
 Author-email: devel@logilab.fr
 License: LGPL
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yams-0.49.3/README.rst` & `yams-0.50.0/README.rst`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/__pkginfo__.py` & `yams-0.50.0/__pkginfo__.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 # pylint: disable-msg=W0622
 
 # package name
 modname = "yams"
 
 # release version
-numversion = (0, 49, 3)
+numversion = (0, 50, 0)
 version = ".".join(str(num) for num in numversion)
 
 # license and copyright
 license = "LGPL"
 
 # short and long description
 description = "entity / relation schema"
 
 # author name and email
 author = "Logilab"
 author_email = "devel@logilab.fr"
 
 # home page
-web = "https://forge.extranet.logilab.fr/open-source/%s" % modname
+web = f"https://forge.extranet.logilab.fr/open-source/{modname}"
 
 # mailing list
 mailinglist = "mailto://python-projects@lists.logilab.org"
 
 # executable
 scripts = ["bin/yams-check", "bin/yams-view"]
```

### Comparing `yams-0.49.3/bin/owl2yams` & `yams-0.50.0/bin/owl2yams`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/docs/Makefile` & `yams-0.50.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/docs/conf.py` & `yams-0.50.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/docs/make.bat` & `yams-0.50.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/docs/yams.rst` & `yams-0.50.0/docs/yams.rst`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/setup.py` & `yams-0.50.0/setup.py`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/test/data/__init__.py` & `yams-0.50.0/test/data/__init__.py`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/test/data/dbmodel/__init__.py` & `yams-0.50.0/test/data/dbmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/test/data/dbmodel/blog.py` & `yams-0.50.0/test/data/dbmodel/blog.py`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/test/data/schema/Company.py` & `yams-0.50.0/test/data/schema/Company.py`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/test/data/schema/Dates.py` & `yams-0.50.0/test/data/schema/Dates.py`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/test/data/schema/State.py` & `yams-0.50.0/test/data/schema/State.py`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/test/data/schema/__init__.py` & `yams-0.50.0/test/data/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/test/data/schema/schema.py` & `yams-0.50.0/test/data/schema/schema.py`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/test/data/schema1.txt` & `yams-0.50.0/test/data/schema1.txt`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/test/data/schema2.txt` & `yams-0.50.0/test/data/schema2.txt`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/test/data/schema_post_build_callback.py` & `yams-0.50.0/test/data/schema_post_build_callback.py`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/test/data2/__init__.py` & `yams-0.50.0/test/data2/__init__.py`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/test/data2/schema.py` & `yams-0.50.0/test/data2/schema.py`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/test/unittest_constraints.py` & `yams-0.50.0/test/unittest_constraints.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     RegexpConstraint,
     SizeConstraint,
     StaticVocabularyConstraint,
     TODAY,
     UniqueConstraint,
     _check_no_error_during_convert,
 )
+from yams._exceptions import BadSchemaDefinition
 from datetime import datetime, date, timedelta, timezone
 from dateutil.tz import tzoffset
 
 
 class CheckAndConverttTC(unittest.TestCase):
     def test_check_no_error_during_convert(self):
         self.assertTrue(_check_no_error_during_convert("4", int))
@@ -169,15 +170,15 @@
 
     def test_regexp_deserialization(self):
         cstr = RegexpConstraint.deserialize("[a-z]+,[A-Z]+,40")
         self.assertEqual(cstr.regexp, "[a-z]+,[A-Z]+")
         self.assertEqual(cstr.flags, 40)
 
     def test_interval_with_attribute(self):
-        cstr = IntervalBoundConstraint(NOW(), Attribute("hop"))
+        cstr = IntervalBoundConstraint(NOW(type="Datetime"), Attribute("hop"))
         cstr2 = IntervalBoundConstraint.deserialize(cstr.serialize())
         self.assertEqual(cstr2.minvalue.offset, None)
         self.assertEqual(cstr2.maxvalue.attr, "hop")
         self.assertTrue(
             cstr2.check(
                 mock_object(hop=datetime.now() + timedelta(hours=1)),
                 "hip",
@@ -208,14 +209,33 @@
         self.assertEqual(cstr2.maxvalue.offset, timedelta(3))
         self.assertTrue(cstr2.check(None, "hip", date.today() + timedelta(2)))
         # fail, value < minvalue
         self.assertFalse(cstr2.check(None, "hip", date.today()))
         # fail, value > maxvalue
         self.assertFalse(cstr2.check(None, "hip", date.today() + timedelta(4)))
 
+    def test_boundary_constraint_consistency(self):
+        cstr = BoundaryConstraint("<=", NOW(type="TZDatetime"))
+        subjschema = mock_object()
+        valid_objschema = mock_object(type="TZDatetime", final=True)
+        rdef = mock_object()
+
+        # Consistent
+        cstr.check_consistency(subjschema, valid_objschema, rdef)
+
+        # BoundaryConstraint doesn't apply to non final attribute schema
+        non_final_objschema = mock_object(type="TZDatetime", final=False)
+        with self.assertRaisesRegex(BadSchemaDefinition, "non final entity type"):
+            cstr.check_consistency(subjschema, non_final_objschema, rdef)
+
+        # BoundaryConstraint with NOW/TODAY as boundary must match type of the attribute schema
+        inconsistent_objschema = mock_object(type="Datetime", final=True)
+        with self.assertRaisesRegex(BadSchemaDefinition, "got Datetime"):
+            cstr.check_consistency(subjschema, inconsistent_objschema, rdef)
+
     def test_bound_constant(self):
         cstr = BoundaryConstraint("<=", 0)
         cstr2 = BoundaryConstraint.deserialize(cstr.serialize())
         self.assertFalse(cstr2.check(None, "hip", 25))
         self.assertTrue(cstr2.check(None, "hip", -1))
 
     def test_bound_with_attribute(self):
```

### Comparing `yams-0.49.3/test/unittest_diff.py` & `yams-0.50.0/test/unittest_diff.py`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/test/unittest_reader.py` & `yams-0.50.0/test/unittest_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -553,15 +553,15 @@
         d2 = datetest.default("d2")
         t1 = datetest.default("t1")
         t2 = datetest.default("t2")
         # datetimes
         self.assertIsInstance(dt1, datetime)
         # there's no easy way to test NOW (except monkey patching now() itself)
         delta = dt1 - _now
-        self.assertTrue(abs(delta.seconds) < 5)
+        self.assertLess(abs(delta.seconds), 5)
         self.assertEqual(date(dt2.year, dt2.month, dt2.day), _today)
         self.assertIsInstance(dt2, datetime)
         # dates
         self.assertEqual(d1, _today)
         self.assertIsInstance(d1, date)
         self.assertEqual(d2, date(2007, 12, 11))
         self.assertIsInstance(d2, date)
```

### Comparing `yams-0.49.3/test/unittest_schema.py` & `yams-0.50.0/test/unittest_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,23 +225,23 @@
 
 
 class EntitySchemaTC(BaseSchemaTC):
     def test_base(self):
         self.assertTrue(repr(eperson))
 
     def test_cmp(self):
-        self.assertTrue(eperson == "Person")
-        self.assertFalse(eperson != "Person")
-        self.assertTrue("Person" == eperson)
-        self.assertTrue(eperson != "Note")
-        self.assertTrue("Note" != eperson)
-        self.assertFalse(enote == eperson)
-        self.assertFalse(eperson == enote)
-        self.assertTrue(enote != eperson)
-        self.assertTrue(eperson != enote)
+        self.assertEqual(eperson, "Person")
+        self.assertEqual(eperson, "Person")
+        self.assertEqual("Person", eperson)
+        self.assertNotEqual(eperson, "Note")
+        self.assertNotEqual("Note", eperson)
+        self.assertNotEqual(enote, eperson)
+        self.assertNotEqual(eperson, enote)
+        self.assertNotEqual(enote, eperson)
+        self.assertNotEqual(eperson, enote)
         entities = [eperson, enote, eaffaire, esociete]
         entities.sort()
         self.assertListEqual(entities, [eaffaire, enote, eperson, esociete])
         self.assertListEqual(entities, ["Affaire", "Note", "Person", "Societe"])
 
     def test_hash(self):
         d = {}
@@ -266,15 +266,15 @@
         self.assertEqual(rgx_cstr2.regexp, rgx_cstr.regexp)
         self.assertEqual(rgx_cstr2.flags, rgx_cstr.flags)
         self.assertEqual(rgx_cstr2._rgx, rgx_cstr._rgx)
 
     def test_deepcopy(self):
         global schema
         schema = deepcopy(schema)
-        self.assertFalse(eperson is schema["Person"])
+        self.assertIsNot(eperson, schema["Person"])
         self.assertEqual(eperson, schema["Person"])
         self.assertEqual("Person", schema["Person"])
         self.assertCountEqual(
             list(eperson.subject_relations.values()), schema["Person"].subject_relations()
         )
         self.assertCountEqual(
             list(eperson.object_relations.values()), schema["Person"].object_relations()
@@ -384,36 +384,34 @@
         eperson._unique_together = [("prenom", "nom")]
         eperson.check_unique_together()
 
     def test_check_unique_together2(self):
         eperson._unique_together = [("prenom", "noms")]
         with self.assertRaises(BadSchemaDefinition) as cm:
             eperson.check_unique_together()
-        self.assertTrue("no such attribute or relation noms" in cm.exception.args[0])
+        self.assertIn("no such attribute or relation noms", cm.exception.args[0])
 
     def test_check_unique_together3(self):
         eperson._unique_together = [("nom", "travaille")]
         with self.assertRaises(BadSchemaDefinition) as cm:
             eperson.check_unique_together()
-        self.assertTrue(
-            "travaille is not an attribute or an inlined relation" in cm.exception.args[0]
-        )
+        self.assertIn("travaille is not an attribute or an inlined relation", cm.exception.args[0])
 
 
 class RelationSchemaTC(BaseSchemaTC):
     def test_cmp(self):
-        self.assertTrue(rconcerne == "concerne")
-        self.assertFalse(rconcerne != "concerne")
-        self.assertTrue("concerne" == rconcerne)
-        self.assertTrue(rconcerne != "nom")
-        self.assertTrue("nom" != rconcerne)
-        self.assertFalse(rnom == rconcerne)
-        self.assertFalse(rconcerne == rnom)
-        self.assertTrue(rnom != rconcerne)
-        self.assertTrue(rconcerne != rnom)
+        self.assertEqual(rconcerne, "concerne")
+        self.assertEqual(rconcerne, "concerne")
+        self.assertEqual("concerne", rconcerne)
+        self.assertNotEqual(rconcerne, "nom")
+        self.assertNotEqual("nom", rconcerne)
+        self.assertNotEqual(rnom, rconcerne)
+        self.assertNotEqual(rconcerne, rnom)
+        self.assertNotEqual(rnom, rconcerne)
+        self.assertNotEqual(rconcerne, rnom)
 
     def test_hash(self):
         d = {}
         d[rconcerne] = "p"
         d[rnom] = "n"
         self.assertEqual(d[copy(rconcerne)], "p")
         self.assertEqual(d[copy(rnom)], "n")
@@ -644,15 +642,15 @@
         import pickle
 
         picklefile = mktemp()
         picklestream = open(picklefile, "wb")
         pickle.dump(schema, picklestream)
         picklestream.close()
         pschema = pickle.load(open(picklefile, "rb"))
-        self.assertFalse(eperson is pschema["Person"])
+        self.assertIsNot(eperson, pschema["Person"])
         self.assertEqual(eperson, pschema["Person"])
         self.assertEqual("Person", pschema["Person"])
         self.assertEqual(eperson.ordered_relations(), pschema["Person"].ordered_relations())
         self.assertEqual(
             list(eperson.object_relations.values()), pschema["Person"].object_relations()
         )
```

### Comparing `yams-0.49.3/test/unittest_schema2dot.py` & `yams-0.50.0/test/unittest_schema2dot.py`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/test/unittest_serialize.py` & `yams-0.50.0/test/unittest_serialize.py`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/test/unittest_specialization.py` & `yams-0.50.0/test/unittest_specialization.py`

 * *Files 6% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         for subjobj in krschema.relation_definitions:
             subject, object = subjobj
             done.add(subjobj)
             self.assertIn(subjobj, expected)
             self.assertEqual(
                 krschema.relation_definition(subject, object).infered, expected[subjobj]
             )
-        self.assertEqual(len(set(expected) - done), 0, "missing %s" % (set(expected) - done))
+        self.assertEqual(len(set(expected) - done), 0, f"missing {set(expected) - done}")
         expected = {
             ("Person", "Company"): False,
             ("Person", "Division"): True,
             ("Person", "SubDivision"): True,
             ("Person", "SubCompany"): True,
             ("Student", "Company"): False,
             ("Student", "Division"): True,
@@ -159,15 +159,15 @@
         for subjobj in wrschema.relation_definitions:
             subject, object = subjobj
             done.add(subjobj)
             self.assertIn(subjobj, expected)
             self.assertEqual(
                 wrschema.relation_definition(subject, object).infered, expected[subjobj]
             )
-        self.assertEqual(len(set(expected) - done), 0, "missing %s" % (set(expected) - done))
+        self.assertEqual(len(set(expected) - done), 0, f"missing {set(expected) - done}")
 
         self.assertIn("custom_attr", self.schema["Student"].subject_relations)
         self.assertEqual(
             self.schema["custom_attr"].relation_definitions[("Student", "String")].permissions,
             {"read": ("managers",), "add": ("managers",), "update": ("managers",)},
         )
 
@@ -185,28 +185,28 @@
         for subjobj in krschema.relation_definitions:
             subject, object = subjobj
             done.add(subjobj)
             self.assertIn(subjobj, expected)
             self.assertEqual(
                 krschema.relation_definition(subject, object).infered, expected[subjobj]
             )
-        self.assertEqual(len(set(expected) - done), 0, "missing %s" % (set(expected) - done))
+        self.assertEqual(len(set(expected) - done), 0, f"missing {set(expected) - done}")
         expected = {
             ("Person", "Company"): False,
             ("Student", "Company"): False,
         }
         done = set()
         for subjobj in wrschema.relation_definitions:
             subject, object = subjobj
             done.add(subjobj)
-            self.assertTrue(subjobj in expected)
+            self.assertIn(subjobj, expected)
             self.assertEqual(
                 wrschema.relation_definition(subject, object).infered, expected[subjobj]
             )
-        self.assertEqual(len(set(expected) - done), 0, "missing %s" % (set(expected) - done))
+        self.assertEqual(len(set(expected) - done), 0, f"missing {set(expected) - done}")
 
     def test_no_more_infered_relations(self):
         relation_definition = self.schema["division_of"].relation_definitions[
             "SubSubDivision", "SubCompany"
         ]
         self.assertEqual("**", relation_definition.cardinality)
         relation_definition = RelationDefinition(
```

### Comparing `yams-0.49.3/test/unittest_xy.py` & `yams-0.50.0/test/unittest_xy.py`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/tox.ini` & `yams-0.50.0/tox.ini`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/yams/__init__.py` & `yams-0.50.0/yams/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with yams. If not, see <https://www.gnu.org/licenses/>.
 """Object model and utilities to define generic Entities/Relations schemas.
 """
 import warnings
-from datetime import datetime, date
+from datetime import datetime, date, timezone
 
 from typing import Set, Type, Dict, Union, Callable, Any, Iterable, TypeVar
 
 import pkg_resources
 
 from logilab.common.date import strptime_time
 from logilab.common import nullobject
@@ -119,15 +119,18 @@
 }
 
 # This provides a way to specify callable objects as default values
 # First level is the final type, second is the keyword to callable map
 _current_date_or_datetime_constructor_type = Callable[[], Union[date, datetime]]
 KEYWORD_MAP: Dict[str, Dict[str, _current_date_or_datetime_constructor_type]] = {
     "Datetime": {"NOW": datetime.now, "TODAY": datetime.today},
-    "TZDatetime": {"NOW": datetime.utcnow, "TODAY": datetime.today},
+    "TZDatetime": {
+        "NOW": lambda: datetime.now(timezone.utc),
+        "TODAY": lambda: datetime.now(timezone.utc),
+    },
     "Date": {"TODAY": date.today},
 }
 
 # bw compat for literal date/time values stored as strings in schemas
 DATE_FACTORY_MAP: Dict[str, Callable[[str], Union[datetime, float]]] = {
     "Datetime": lambda x: ":" in x
     and datetime.strptime(x, "%Y/%m/%d %H:%M")
@@ -195,15 +198,15 @@
     """register a yams base (final) type. You'll have to call
     base_type_class to generate the class.
     """
     from yams.schema import RelationDefinitionSchema
     from yams.constraints import BASE_CHECKERS, yes
 
     # Add the datatype to yams base types
-    assert name not in BASE_TYPES, "%s already in BASE_TYPES %s" % (name, BASE_TYPES)
+    assert name not in BASE_TYPES, f"{name} already in BASE_TYPES {BASE_TYPES}"
 
     BASE_TYPES.add(name)
 
     # Add the new datatype to the authorized types of RelationDefinitionSchema
     if not isinstance(parameters, dict):
         # turn tuple/list into dict with None values
         parameters = dict((p, None) for p in parameters)
@@ -215,12 +218,12 @@
 
 
 def unregister_base_type(name: str) -> None:
     """Unregister a yams base (final) type"""
     from yams.schema import RelationDefinitionSchema
     from yams.constraints import BASE_CHECKERS
 
-    assert name in BASE_TYPES, "%s not in BASE_TYPES %s" % (name, BASE_TYPES)
+    assert name in BASE_TYPES, f"{name} not in BASE_TYPES {BASE_TYPES}"
 
     BASE_TYPES.remove(name)
     RelationDefinitionSchema.BASE_TYPE_PROPERTIES.pop(name)
     BASE_CHECKERS.pop(name)
```

### Comparing `yams-0.49.3/yams/_exceptions.py` & `yams-0.50.0/yams/_exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,19 +114,19 @@
             errors_dict = self.errors
         else:
             errors_dict = dict(self._translated_errors(str))
 
         if len(errors_dict) == 1:
             attr, error = next(iter(errors_dict.items()))
 
-            return "%s (%s): %s" % (self.entity, attr, error)
+            return f"{self.entity} ({attr}): {error}"
 
-        errors = "\n".join("* %s: %s" % (k, v) for k, v in errors_dict.items())
+        errors = "\n".join(f"* {k}: {v}" for k, v in errors_dict.items())
 
-        return "%s:\n%s" % (self.entity, errors)
+        return f"{self.entity}:\n{errors}"
 
     def translate(self, _: Callable[[str], str]) -> None:
         """Translate and interpolate messsages in the errors dictionary, using
         the given translation function.
 
         If no substitution has been given, suppose msg is already translated for
         bw compat, so no translation occurs.
```

### Comparing `yams-0.49.3/yams/buildobjs.py` & `yams-0.50.0/yams/buildobjs.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 _KwargsKeyType = TypeVar("_KwargsKeyType")
 
 
 def _check_kwargs(kwargs: Dict[_KwargsKeyType, Any], attributes: Sequence[_KwargsKeyType]) -> None:
     """Check that all keys of kwargs are actual attributes."""
     for key in kwargs:
         if key not in attributes:
-            raise BadSchemaDefinition("no such property %r in %r" % (key, attributes))
+            raise BadSchemaDefinition(f"no such property {key!r} in {attributes!r}")
 
 
 @deprecation.argument_renamed(old_name="fromobj", new_name="from_object", version="0.48")
 @deprecation.argument_renamed(old_name="toobj", new_name="to_object", version="0.48")
 def _copy_attributes(from_object: Any, to_object: Any, attributes: Iterable[str]) -> None:
     for attribute in attributes:
         value = getattr(from_object, attribute, MARKER)
@@ -222,15 +222,15 @@
         )
 
         if self.__doc__:
             self.description = " ".join(self.__doc__.split())
             cast(str, self.description)
 
     def __repr__(self) -> str:
-        return "<%s %r @%x>" % (self.__class__.__name__, self.name, id(self))
+        return f"<{self.__class__.__name__} {self.name!r} @{id(self):x}>"
 
     @classmethod
     def expand_type_definitions(cls: Type["Definition"], defined: Defined) -> None:
         """Schema building step 1: register definition objects by adding them
         to the `defined` dictionnary.
         """
         raise NotImplementedError()
@@ -310,26 +310,26 @@
             bad_schema_definition.tb_offset = 2  # type: ignore
 
             raise bad_schema_definition
 
         self.__dict__.update(kwargs)
 
     def __repr__(self) -> str:
-        return "%(name)s %(entity_type)s" % self.__dict__
+        return f"{self.__dict__['name']} {self.__dict__['entity_type']}"
 
 
 class SubjectRelation(ObjectRelation):
     uid = MARKER
     indexed = MARKER
     fulltextindexed = MARKER
     internationalizable = MARKER
     default = MARKER
 
     def __repr__(self) -> str:
-        return "%(entity_type)s %(name)s" % self.__dict__
+        return f"{self.__dict__['entity_type']} {self.__dict__['name']}"
 
 
 class AbstractTypedAttribute(SubjectRelation):
     """AbstractTypedAttribute is not directly instantiable
 
     subclasses must provide a <entity_type> attribute to be instantiable
     """
@@ -407,15 +407,15 @@
 
         if self.__class__.__name__ == "String":  # XXX
             max_size = max(len(x) for x in vocabulary)
 
             _add_constraint(kwargs, SizeConstraint(max=max_size))
 
     def __repr__(self) -> str:
-        return "<%(name)s(%(entity_type)s)>" % self.__dict__
+        return f"<{self.__dict__['name']}({self.__dict__['entity_type']})>"
 
 
 @deprecation.argument_renamed(old_name="etype", new_name="entity_type", version="0.48")
 def make_type(entity_type: str) -> Type[AbstractTypedAttribute]:
     """create a python class for a Yams base type.
 
     Notice it is now possible to create a specific type with user-defined
@@ -649,28 +649,28 @@
 
         _check_kwargs(kwargs, ETYPE_PROPERTIES)
 
         self.__dict__.update(kwargs)
         self.specialized_type: Optional[str] = self.__class__.__dict__.get("__specializes__")
 
     def __str__(self) -> str:
-        return "entity type %r" % self.name
+        return f"entity type {self.name!r}"
 
     @property
     def specialized_by(self) -> List[str]:
         return self.__class__.__dict__.get("__specialized_by__", [])
 
     @classmethod
     def expand_type_definitions(cls: Type["EntityType"], defined: Defined) -> None:
         """Schema building step 1: register definition objects by adding
         them to the `defined` dictionnary.
         """
         name: str = getattr(cls, "name", cls.__name__)
 
-        assert cls is not defined.get(name), "duplicate registration: %s" % name
+        assert cls is not defined.get(name), f"duplicate registration: {name}"
         assert (
             name not in defined
         ), "type '%s' was already defined here %s, new definition here %s" % (
             name,
             defined[name].__module__,
             cls,
         )
@@ -751,15 +751,15 @@
                 )
 
                 _copy_attributes(relation, relation_definition, relation_definitions_properties)
 
             elif isinstance(relation, RelationDefinition):
                 relation_definition = relation
             else:
-                raise BadSchemaDefinition("dunno how to handle %s" % relation)
+                raise BadSchemaDefinition(f"dunno how to handle {relation}")
 
             order += 1
             relation_definition._add_relations(defined, schema)
 
     # methods that can be used to extend an existant schema definition ########
 
     @classmethod
@@ -821,15 +821,15 @@
         # dynamically set attribute, full yams magic
         number = 0
         for number, rel in enumerate(cls.__relations__):  # type: ignore
             if rel.name == after_relation_name:
                 break
 
         else:
-            raise BadSchemaDefinition("can't find %s relation on %s" % (after_relation_name, cls))
+            raise BadSchemaDefinition(f"can't find {after_relation_name} relation on {cls}")
 
         # mypy: "Type[EntityType]" has no attribute "__relations__"
         # dynamically set attribute, full yams magic
         _add_relation(cls.__relations__, relation_definition, name, number + 1)  # type: ignore
 
     @classmethod
     def remove_relation(cls: Type["EntityType"], name: str) -> None:
@@ -878,30 +878,30 @@
             warn("[yams 0.37] meta is deprecated", DeprecationWarning, stacklevel=2)
 
         _check_kwargs(kwargs, RTYPE_PROPERTIES + ("description", "__permissions__"))
 
         self.__dict__.update(kwargs)
 
     def __str__(self) -> str:
-        return "relation type %r" % self.name
+        return f"relation type {self.name!r}"
 
     @classmethod
     def expand_type_definitions(cls: Type["RelationType"], defined: Defined) -> None:
         """schema building step 1:
 
         register definition objects by adding them to the `defined` dictionnary
         """
         name: str = getattr(cls, "name", cls.__name__)
 
         if cls.__doc__ and not cls.description:
             cls.description = " ".join(cls.__doc__.split())
 
         if name in defined:
             if defined[name].__class__ is not RelationType:
-                raise BadSchemaDefinition("duplicated relation type for %s" % name)
+                raise BadSchemaDefinition(f"duplicated relation type for {name}")
 
             # relation type created from a relation definition, override it
             all_properties = _RELATION_PROPERTIES() + ("subject", "object")
 
             _copy_attributes(defined[name], cls, all_properties)
 
         defined[name] = cls
@@ -946,15 +946,15 @@
     # subject or object the relation, the cardinality, the constraints
     # and the symmetric property.
     # """
 
     subject: Union[nullobject, str, List[str], None] = MARKER
     object: Union[nullobject, str, List[str], None] = MARKER
     cardinality: Union[nullobject, str, None] = MARKER
-    constraints = MARKER
+    constraints: list[BaseConstraint] = MARKER  # type: ignore
     symmetric = MARKER
     inlined = MARKER
     formula = MARKER
 
     def __init__(
         self,
         subject: Optional[Union[str, Tuple[str]]] = None,
@@ -994,15 +994,18 @@
         _check_kwargs(kwargs, relation_definitions_properties)
         _copy_attributes(attrdict(**kwargs), self, relation_definitions_properties)
 
         if self.constraints:
             self.constraints = list(self.constraints)
 
     def __str__(self) -> str:
-        return "relation definition (%(subject)s %(name)s %(object)s)" % self.__dict__
+        return (
+            f"relation definition ({self.__dict__['subject']} {self.__dict__['name']} "
+            f"{self.__dict__['object']})"
+        )
 
     @classmethod
     def expand_type_definitions(cls: Type["RelationDefinition"], defined: Defined) -> None:
         """schema building step 1:
 
         register definition objects by adding them to the `defined` dictionnary
         """
```

### Comparing `yams-0.49.3/yams/constraints.py` & `yams-0.50.0/yams/constraints.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,28 @@
 import decimal
 import operator
 import json
 import datetime
 from dateutil.parser import parse
 import warnings
 
-from typing import Any, Dict, Match, Tuple, Type, Union, Optional, Callable, Sequence, List, cast
+from typing import (
+    Any,
+    Dict,
+    Literal,
+    Match,
+    Tuple,
+    Type,
+    Union,
+    Optional,
+    Callable,
+    Sequence,
+    List,
+    cast,
+)
 
 from logilab.common.deprecation import class_renamed, send_warning
 from logilab.common.date import todate, todatetime
 
 import yams
 from yams import KEYWORD_MAP, BadSchemaDefinition
 from yams.interfaces import IConstraint, IVocabularyConstraint
@@ -44,23 +57,23 @@
     def default(self, obj: Union[Any, "NOW", "TODAY"]) -> Union[Any, dict]:
         if isinstance(obj, Attribute):
             return {"__attribute__": obj.attr}
 
         if isinstance(obj, NOW):
             # it is not a timedelta
             if obj.offset is None:
-                return {"__now__": True, "offset": obj.offset}
+                return {"__now__": True, "offset": obj.offset, "type": obj.type}
 
             d = {
                 "days": obj.offset.days,
                 "seconds": obj.offset.seconds,
                 "microseconds": obj.offset.microseconds,
             }
 
-            return {"__now__": True, "offset": d}
+            return {"__now__": True, "offset": d, "type": obj.type}
 
         if isinstance(obj, TODAY):
             # it is not a timedelta
             if obj.offset is None:
                 return {"__today__": True, "offset": obj.offset, "type": obj.type}
 
             d = {
@@ -82,15 +95,15 @@
 
     if "__now__" in dct:
         if dct["offset"] is not None:
             offset = datetime.timedelta(**dct["offset"])
         else:
             offset = None
 
-        return NOW(offset)
+        return NOW(offset, type=dct.get("type", "TZDatetime"))
 
     if "__today__" in dct:
         if dct["offset"] is not None:
             offset = datetime.timedelta(**dct["offset"])
         else:
             offset = None
 
@@ -105,24 +118,29 @@
 
 cstr_json_loads: Callable[[str], Dict] = json.JSONDecoder(object_hook=_json_object_hook).decode
 
 
 def _message_value(boundary) -> Any:
     if isinstance(boundary, Attribute):
         return boundary.attr
+    elif isinstance(boundary, (NOW, TODAY)):
+        return str(boundary)
     return boundary
 
 
 class BaseConstraint:
     """base class for constraints"""
 
     __implements__ = IConstraint
 
+    msg: Optional[str]
+    """user defined message returned by failed_message when the constraint check fails"""
+
     def __init__(self, msg: Optional[str] = None) -> None:
-        self.msg: Optional[str] = msg
+        self.msg = msg
 
     def check_consistency(
         self,
         subjschema: yams_types.EntitySchema,
         objschema: yams_types.EntitySchema,
         rdef: yams_types.RelationDefinition,
     ) -> None:
@@ -145,15 +163,15 @@
         if value and value != "None":
             d = cstr_json_loads(value)
         else:
             d = {}
 
         return cls(**d)
 
-    def failed_message(self, key: str, value, entity=None) -> Tuple[Optional[str], Dict[str, Any]]:
+    def failed_message(self, key: str, value, entity=None) -> Tuple[str, Dict[str, Any]]:
         if entity is None:
             warnings.warn(
                 "[yams 0.44] failed message " "should now be given entity has argument.",
                 DeprecationWarning,
                 stacklevel=2,
             )
 
@@ -215,50 +233,48 @@
         self, max: Optional[int] = None, min: Optional[int] = None, msg: Optional[str] = None
     ) -> None:
         super(SizeConstraint, self).__init__(msg)
 
         assert max is not None or min is not None, "No max or min"
 
         if min is not None:
-            assert isinstance(min, int), "min must be an int, not %r" % min
+            assert isinstance(min, int), f"min must be an int, not {min!r}"
 
         if max is not None:
-            assert isinstance(max, int), "max must be an int, not %r" % max
+            assert isinstance(max, int), f"max must be an int, not {max!r}"
 
         self.max: Optional[int] = max
         self.min: Optional[int] = min
 
     def __str__(self) -> str:
         res = "size"
 
         if self.max is not None:
-            res = "%s <= %s" % (res, self.max)
+            res = f"{res} <= {self.max}"
 
         if self.min is not None:
-            res = "%s <= %s" % (self.min, res)
+            res = f"{self.min} <= {res}"
 
         return res
 
     def check_consistency(
         self,
         subjschema: yams_types.EntitySchema,
         objschema: yams_types.EntitySchema,
         rdef: yams_types.RelationDefinition,
     ) -> None:
         if not objschema.final:
             raise BadSchemaDefinition("size constraint doesn't apply to non " "final entity type")
 
         if objschema not in ("String", "Bytes", "Password"):
-            raise BadSchemaDefinition(
-                "size constraint doesn't apply to %s " "entity type" % objschema
-            )
+            raise BadSchemaDefinition(f"size constraint doesn't apply to {objschema} entity type")
 
         if self.max:
             for cstr in rdef.constraints:
-                if cstr.__class__ is StaticVocabularyConstraint:
+                if type(cstr) is StaticVocabularyConstraint:
                     for value in cstr.values:
                         if len(value) > self.max:
                             raise BadSchemaDefinition(
                                 "size constraint set to %s but vocabulary "
                                 "contains string of greater size" % self.max
                             )
 
@@ -331,29 +347,27 @@
         """
         super(RegexpConstraint, self).__init__(msg)
         self.regexp: str = regexp
         self.flags: int = flags
         self._rgx = re.compile(regexp, flags)
 
     def __str__(self) -> str:
-        return "regexp %s" % self.regexp
+        return f"regexp {self.regexp}"
 
     def check_consistency(
         self,
         subjschema: yams_types.EntitySchema,
         objschema: yams_types.EntitySchema,
         rdef: yams_types.RelationDefinition,
     ) -> None:
         if not objschema.final:
             raise BadSchemaDefinition("regexp constraint doesn't apply to non " "final entity type")
 
         if objschema not in ("String", "Password"):
-            raise BadSchemaDefinition(
-                "regexp constraint doesn't apply to %s " "entity type" % objschema
-            )
+            raise BadSchemaDefinition(f"regexp constraint doesn't apply to {objschema} entity type")
 
     def check(self, entity, rtype: yams_types.RelationType, value: str) -> Optional[Match[str]]:
         """return true if the value maches the regular expression"""
         return self._rgx.match(value, self.flags)
 
     def _failed_message(self, entity, key: str, value) -> Tuple[str, Dict[str, Any]]:
         return (
@@ -402,24 +416,30 @@
 
         assert op in OPERATORS, op
 
         self.operator: str = op
         self.boundary: Optional[Union["Attribute", "NOW", "TODAY"]] = boundary
 
     def __str__(self) -> str:
-        return "value %s" % self.serialize()
+        return f"value {self.serialize()}"
 
     def check_consistency(
         self,
         subjschema: yams_types.EntitySchema,
         objschema: yams_types.EntitySchema,
         rdef: yams_types.RelationDefinition,
     ) -> None:
+        if isinstance(self.boundary, (NOW, TODAY)) and self.boundary.type != objschema.type:
+            raise BadSchemaDefinition(
+                f"boundary constraint {str(self.boundary)} applies to {self.boundary.type}"
+                f" attributes, got {objschema.type}"
+            )
+
         if not objschema.final:
-            raise BadSchemaDefinition("bound constraint doesn't apply to non " "final entity type")
+            raise BadSchemaDefinition("boundary constraint doesn't apply to non final entity type")
 
     def check(self, entity, rtype: yams_types.RelationType, value) -> bool:
         """return true if the value satisfies the constraint, else false"""
         boundary = actual_value(self.boundary, entity)
 
         if boundary is None:
             return True
@@ -427,15 +447,15 @@
         return OPERATORS[self.operator](value, boundary)
 
     def _failed_message(self, entity, key: str, value) -> Tuple[str, Dict[str, Any]]:
         return (
             "value %%(KEY-value)s must be %s %%(KEY-boundary)s" % self.operator,
             {
                 key + "-value": value,
-                key + "-boundary": _message_value(actual_value(self.boundary, entity)),
+                key + "-boundary": _message_value(self.boundary),
             },
         )
 
     def serialize(self) -> str:
         """simple text serialization"""
         return cstr_json_dumps({"op": self.operator, "boundary": self.boundary, "msg": self.msg})
 
@@ -486,15 +506,15 @@
 
         super(IntervalBoundConstraint, self).__init__(msg)
 
         self.minvalue: Optional[Union[int, float]] = minvalue
         self.maxvalue: Optional[Union[int, float]] = maxvalue
 
     def __str__(self) -> str:
-        return "value [%s]" % self.serialize()
+        return f"value [{self.serialize()}]"
 
     def check_consistency(
         self,
         subjschema: yams_types.EntitySchema,
         objschema: yams_types.EntitySchema,
         rdef: yams_types.RelationDefinition,
     ) -> None:
@@ -556,24 +576,24 @@
     __implements__ = IVocabularyConstraint
 
     def __init__(self, values: Sequence[str], msg: Optional[str] = None) -> None:
         super(StaticVocabularyConstraint, self).__init__(msg)
         self.values: Tuple[str, ...] = tuple(values)
 
     def __str__(self) -> str:
-        return "value in (%s)" % ", ".join(repr(str(word)) for word in self.vocabulary())
+        return f"value in ({', '.join(repr(str(word)) for word in self.vocabulary())})"
 
     def check(self, entity, rtype: yams_types.RelationType, value: str) -> bool:
         """return true if the value is in the specific vocabulary"""
         return value in self.vocabulary(entity=entity)
 
     def _failed_message(self, entity, key: str, value) -> Tuple[str, Dict[str, Any]]:
         if isinstance(value, str):
-            value = '"%s"' % str(value)
-            choices = ", ".join('"%s"' % val for val in self.values)
+            value = f'"{str(value)}"'
+            choices = ", ".join(f'"{val}"' for val in self.values)
         else:
             choices = ", ".join(str(val) for val in self.values)
 
         return (
             _("invalid value %(KEY-value)s, " "it must be one of %(KEY-choices)s"),
             {key + "-value": value, key + "-choices": choices},
         )
@@ -663,44 +683,54 @@
 
 
 class Attribute:
     def __init__(self, attr) -> None:
         self.attr = attr
 
     def __str__(self) -> str:
-        return "%s(%r)" % (self.__class__.__name__, self.attr)
+        return f"{self.__class__.__name__}({self.attr!r})"
 
     def value(self, entity) -> Any:
         return getattr(entity, self.attr)
 
 
 class NOW:
-    def __init__(self, offset: Optional[datetime.timedelta] = None) -> None:
-        self.offset: Optional[datetime.timedelta] = offset
+    def __init__(
+        self,
+        offset: Optional[datetime.timedelta] = None,
+        type: Literal["Datetime", "TZDatetime"] = "TZDatetime",
+    ) -> None:
+        self.offset = offset
+        # XXX no check that self.type is in KEYWORD_MAP?
+        self.type = type
 
-    def __str__(self) -> str:
-        return "%s(%r)" % (self.__class__.__name__, self.offset)
+    def __str__(self):
+        return f"{type(self).__name__}({self.offset}, {self.type})"
 
-    def value(self, entity) -> datetime.date:
-        now = yams.KEYWORD_MAP["Datetime"]["NOW"]()
+    def value(self, entity) -> datetime.datetime:
+        now = yams.KEYWORD_MAP[self.type]["NOW"]()
 
         if self.offset:
             now += self.offset
 
-        return now
+        return cast(datetime.datetime, now)
 
 
 class TODAY:
-    def __init__(self, offset: Optional[datetime.timedelta] = None, type: str = "Date") -> None:
+    def __init__(
+        self,
+        offset: Optional[datetime.timedelta] = None,
+        type: Literal["Date", "Datetime", "TZDatetime"] = "Date",
+    ) -> None:
         self.offset: Optional[datetime.timedelta] = offset
         # XXX no check that self.type is in KEYWORD_MAP?
         self.type: str = type
 
     def __str__(self):
-        return "%s(%r, %r)" % (self.__class__.__name__, self.offset, self.type)
+        return f"{type(self).__name__}({self.offset}, {self.type})"
 
     def value(self, entity) -> datetime.date:
         now = yams.KEYWORD_MAP[self.type]["TODAY"]()
 
         if self.offset:
             now += self.offset
```

### Comparing `yams-0.49.3/yams/diff.py` & `yams-0.50.0/yams/diff.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,16 +51,16 @@
 def quoted(obj: Union[str, Any]) -> str:
     if isinstance(obj, str):
         # NOT repr, because .....
         # strings here turn out as unicode strings (from the repo side)
         # but are (mostly) really str in the schema.py source
         # and we don't want a bogus diff about '...' vs u'...'
         if "'" in obj:
-            return '"%s"' % obj
-    return "'%s'" % obj
+            return f'"{obj}"'
+    return f"'{obj}'"
 
 
 class attr_scope:
     indentation: int = 2
     spacer: str = ""
     nextline: str = ","
 
@@ -83,17 +83,17 @@
 ) -> str:
     out = []
 
     for prop, val in sorted(props.items()):
         if prop in ignore:
             continue
 
-        out.append("\t" * scope.indentation + "%s%s=%s%s" % (prop, scope.spacer, scope.spacer, val))
+        out.append("\t" * scope.indentation + f"{prop}{scope.spacer}={scope.spacer}{val}")
 
-    return ("%s\n" % scope.nextline).join(out)
+    return (f"{scope.nextline}\n").join(out)
 
 
 def format_expression(expr) -> str:
     mainvars = expr.mainvars - set("SUXO")
 
     return "%s(%s%s)" % (
         expr.__class__.__name__,
@@ -103,15 +103,15 @@
 
 
 def format_tuple(iterator: Iterable) -> str:
     out = []
     for thing in iterator:
         out.append(thing)
 
-    return "(%s)" % ",".join(out)
+    return f"({','.join(out)})"
 
 
 def format_perms(
     perms: Dict[str, Iterable], scope: Union[Type[attr_scope], Type[class_scope]], isdefault: bool
 ) -> str:
     out = []
     for p in ("read", "add", "update", "delete"):
@@ -138,19 +138,19 @@
     )
 
 
 def format_constraint(cstr: IConstraint) -> str:
     cclass = cstr.__class__.__name__
 
     if "RQL" in cclass:
-        out = ["%s(%s" % (cclass, quoted(cstr.expression))]  # type:ignore[attr-defined]
+        out = [f"{cclass}({quoted(cstr.expression)}"]  # type:ignore[attr-defined]
         mainvars = getattr(cstr, "mainvars", None)
 
         if mainvars:
-            out.append(", mainvars=%s" % quoted(",".join(mainvars)))
+            out.append(f", mainvars={quoted(','.join(mainvars))}")
 
         out.append(")")
     elif "Boundary" in cclass:
         return "%s(%s %s)" % (
             cclass,
             quoted(cstr.operator),  # type:ignore[attr-defined]
             str(cstr.boundary),  # type:ignore[attr-defined]
@@ -228,15 +228,15 @@
                         transform = identity
 
                     ret["vocabulary"] = [transform(x) for x in constraint.vocabulary()]
                 else:
                     other.append(constraint)
 
             if other:
-                ret["constraints"] = "[%s]" % ",".join(format_constraint(cstr) for cstr in other)
+                ret["constraints"] = f"[{','.join(format_constraint(cstr) for cstr in other)}]"
 
             continue
 
         if val is None:
             continue
 
         if prop == "default":
@@ -265,17 +265,17 @@
     ignore: Set = set(ignore)  # type: ignore
     multirtypes = []
 
     for entity in sorted(schema.entities()):
         if entity.final:
             continue
 
-        output.append("class %s(EntityType):\n" % entity.type)
+        output.append(f"class {entity.type}(EntityType):\n")
         perms, isdefault = permissionshandler(entity, entity.permissions)
-        output.append("\t__permissions__ = %s\n\n" % format_perms(perms, class_scope, isdefault))
+        output.append(f"\t__permissions__ = {format_perms(perms, class_scope, isdefault)}\n\n")
 
         attributes = [
             (
                 attr[0].type,
                 attr[1].type,
                 properties_from(entity.relation_definition(attr[0].type), permissionshandler),
             )
@@ -327,17 +327,17 @@
             subjetype = subjectschema.type
             objetype = objectschema.type
 
             output.append(
                 "class %s_%s_%s(RelationDefinition):\n"
                 % (rtype, subjetype.lower(), objetype.lower())
             )
-            output.append("\tname = %s\n" % quoted(rtype))
-            output.append("\tsubject = %s\n" % quoted(subjetype))
-            output.append("\tobject = %s\n" % quoted(objetype))
+            output.append(f"\tname = {quoted(rtype)}\n")
+            output.append(f"\tsubject = {quoted(subjetype)}\n")
+            output.append(f"\tobject = {quoted(objetype)}\n")
             output.append(
                 format_props(properties_from(relation, permissionshandler), class_scope, ignore)
             )
             output.append("\n\n")
 
     return "".join(output)
 
@@ -368,18 +368,18 @@
     output1 = os.path.join(tmpdir, "schema1.txt")
     output2 = os.path.join(tmpdir, "schema2.txt")
 
     schema2file(schema1, output1, permissionshandler, ignore)
     schema2file(schema2, output2, permissionshandler, ignore)
 
     if diff_tool:
-        cmd = "%s %s %s" % (diff_tool, output1, output2)
+        cmd = f"{diff_tool} {output1} {output2}"
         subprocess.Popen(cmd, shell=True)
     else:
-        print("description files save in %s and %s" % (output1, output2))
+        print(f"description files save in {output1} and {output2}")
 
     print(output1, output2)
 
     return output1, output2
 
 
 if __name__ == "__main__":
@@ -397,13 +397,13 @@
     )
     (options, args) = parser.parse_args()
     if options.schema1 and options.schema2:
         schema1 = SchemaLoader().load([options.schema1])
         schema2 = SchemaLoader().load([options.schema2])
         output1, output2 = schema_diff(schema1, schema2)
         if options.diff_tool:
-            cmd = "%s %s %s" % (options.diff_tool, output1, output2)
+            cmd = f"{options.diff_tool} {output1} {output2}"
             process = subprocess.Popen(cmd, shell=True)
         else:
-            print("description files save in %s and %s" % (output1, output2))
+            print(f"description files save in {output1} and {output2}")
     else:
         parser.error("An input file name must be specified")
```

### Comparing `yams-0.49.3/yams/interfaces.py` & `yams-0.50.0/yams/interfaces.py`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/yams/reader.py` & `yams-0.50.0/yams/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -371,15 +371,15 @@
                 __import__(package)
 
             with open(file_path) as f:
                 try:
                     code = compile(f.read(), file_path, "exec")
                     exec(code, file_globals)
                 except Exception:
-                    print("exception while reading %s" % file_path, file=sys.stderr)
+                    print(f"exception while reading {file_path}", file=sys.stderr)
                     raise
 
             file_globals["__file__"] = file_path
 
             module = types.ModuleType(str(module_name))
             module.__dict__.update(file_globals)
```

### Comparing `yams-0.49.3/yams/schema.py` & `yams-0.50.0/yams/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
 
 @deprecation.argument_renamed(old_name="rtype", new_name="relation_type", version="0.48")
 def role_name(relation_type, role) -> str:
     """function to use for qualifying attribute / relation in ValidationError
     errors'dictionnary
     """
-    return "%s-%s" % (relation_type, role)
+    return f"{relation_type}-{role}"
 
 
 def rehash(dictionary: Dict) -> dict:
     """this function manually builds a copy of `dictionary` but forces
     hash values to be recomputed. Note that dict(d) or d.copy() don't
     do that.
 
@@ -200,36 +200,36 @@
         return self.permissions[action]
 
     def set_action_permissions(self, action: str, permissions: yams_types.Permission) -> None:
         assert type(permissions) is tuple, "permissions is expected to be a tuple not %s" % type(
             permissions
         )
 
-        assert action in self.ACTIONS, "%s not in %s" % (action, self.ACTIONS)
+        assert action in self.ACTIONS, f"{action} not in {self.ACTIONS}"
 
         self.permissions[action] = permissions
 
     def check_permission_definitions(self) -> None:
         """check permissions are correctly defined"""
 
         # already initialized, check everything is fine
         for action, groups in self.permissions.items():
-            assert action in self.ACTIONS, "unknown action %s for %s" % (action, self)
+            assert action in self.ACTIONS, f"unknown action {action} for {self}"
 
             assert isinstance(
                 groups, tuple
-            ), "permission for action %s of %s isn't a tuple as " "expected" % (action, self)
+            ), f"permission for action {action} of {self} isn't a tuple as expected"
 
         if self.final:
             self.advertise_new_add_permission()
 
         for action in self.ACTIONS:
             assert (
                 action in self.permissions
-            ), "missing expected permissions for action %s for %s" % (action, self)
+            ), f"missing expected permissions for action {action} for {self}"
 
 
 # Schema objects definition ###################################################
 
 
 class TargetInlinedDeprecationWarning(TargetRemovedDeprecationWarning):
     def __init__(self, reason: str, kind: DeprecationWarningKind, name: str):
@@ -321,18 +321,18 @@
         errors = []
 
         for unique_together in self._unique_together:
             for name in unique_together:
                 try:
                     relation_schema = self.relation_definition(name, take_first=True)
                 except KeyError:
-                    errors.append("no such attribute or relation %s" % name)
+                    errors.append(f"no such attribute or relation {name}")
                 else:
                     if not (relation_schema.final or relation_schema.relation_type.inlined):
-                        errors.append("%s is not an attribute or an inlined " "relation" % name)
+                        errors.append(f"{name} is not an attribute or an inlined relation")
 
         if errors:
             message = "invalid __unique_together__ specification for %s: %s" % (
                 self,
                 ", ".join(errors),
             )
             raise BadSchemaDefinition(message)
@@ -604,15 +604,15 @@
         return meta_attributes
 
     @deprecation.argument_renamed(old_name="attr", new_name="attribute", version="0.48")
     def has_metadata(self, attribute, metadata) -> Optional["RelationSchema"]:
         """return metadata's relation schema if this entity has the given
         `metadata` field for the given `attribute` attribute
         """
-        return self.subject_relations.get("%s_%s" % (attribute, metadata))
+        return self.subject_relations.get(f"{attribute}_{metadata}")
 
     @deprecation.argument_renamed(old_name="attr", new_name="attribute", version="0.48")
     def is_metadata(self, attribute) -> Optional[Tuple[str, str]]:
         """return a metadata for an attribute (None if unspecified)"""
         try:
             attribute, metadata = str(attribute).rsplit("_", 1)
         except ValueError:
@@ -895,17 +895,17 @@
 
     def update(self, values: Dict[str, Any]) -> None:
         # XXX check we're copying existent properties
         self.__dict__.update(values)
 
     def __str__(self) -> str:
         if self.object.final:
-            return "attribute %s.%s[%s]" % (self.subject, self.relation_type, self.object)
+            return f"attribute {self.subject}.{self.relation_type}[{self.object}]"
 
-        return "relation %s %s %s" % (self.subject, self.relation_type, self.object)
+        return f"relation {self.subject} {self.relation_type} {self.object}"
 
     def __repr__(self) -> str:
         return "<%s at @%#x>" % (self, id(self))
 
     def as_triple(self) -> Tuple["EntitySchema", "RelationSchema", "EntitySchema"]:
         return (self.subject, self.relation_type, self.object)
```

### Comparing `yams-0.49.3/yams/schema2dot.py` & `yams-0.50.0/yams/schema2dot.py`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/yams/serialize.py` & `yams-0.50.0/yams/serialize.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,27 +27,27 @@
 
     for e in reversed(ordered_nodes(graph)):
         if not e.final:
             if e._specialized_type:
                 base = e._specialized_type
             else:
                 base = "EntityType"
-            w("class %s(%s):\n" % (e.type, base))
+            w(f"class {e.type}({base}):\n")
             attr_defs = list(e.attribute_definitions())
             if attr_defs:
                 for attr, obj in attr_defs:
-                    w("    %s = %s()\n" % (attr.type, obj.type))
+                    w(f"    {attr.type} = {obj.type}()\n")
             else:
                 w("    pass\n")
             w("\n")
 
     for r in schema.relations():
         if not r.final:
             if r.subjects() and r.objects():
-                w("class %s(RelationDefinition):\n" % r.type)
+                w(f"class {r.type}(RelationDefinition):\n")
                 w("    subject = (%s,)\n" % ", ".join("'%s'" % x for x in r.subjects()))
                 w("    object = (%s,)\n" % ", ".join("'%s'" % x for x in r.objects()))
                 w("\n")
             else:
-                logging.warning("relation definition %s missing subject/object" % r.type)
+                logging.warning(f"relation definition {r.type} missing subject/object")
 
     return out.getvalue()
```

### Comparing `yams-0.49.3/yams/tools.py` & `yams-0.50.0/yams/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         filename, lineno, _, _ = extract_tb(traceback)[-1 - tb_offset]
 
         if hasattr(ex, "schema_files"):
             # mypy: "Exception" has no attribute "schema_files"
             # but we've added it above in the exception chain and we test it before
             filename = ", ".join(ex.schema_files)  # type: ignore
 
-        _error(filename, lineno, "%s -> %s" % (ex.__class__.__name__, ex))
+        _error(filename, lineno, f"{ex.__class__.__name__} -> {ex}")
 
         return 2
 
 
 def schema_image() -> int:
     options = [
         (
```

### Comparing `yams-0.49.3/yams/types.py` & `yams-0.50.0/yams/types.py`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/yams/xy.py` & `yams-0.50.0/yams/xy.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                 DeprecationWarning,
                 stacklevel=2,
             )
 
             prefix, xmlns = xmlns, prefix
 
         if not overwrite and prefix in self.prefixes and self.prefixes.get(prefix) != xmlns:
-            raise Exception("prefix %r already defined with different value" % prefix)
+            raise Exception(f"prefix {prefix!r} already defined with different value")
 
         self.prefixes[prefix] = xmlns
 
     def _norm_yams_key(self, yamssnippet: str) -> Tuple[str, str, str]:
         parts = yamssnippet.split(" ")
 
         if len(parts) == 1:
```

### Comparing `yams-0.49.3/yams.egg-info/PKG-INFO` & `yams-0.50.0/yams.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yams
-Version: 0.49.3
+Version: 0.50.0
 Summary: entity / relation schema
 Home-page: https://forge.extranet.logilab.fr/open-source/yams
 Author: Logilab
 Author-email: devel@logilab.fr
 License: LGPL
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yams-0.49.3/yams.egg-info/SOURCES.txt` & `yams-0.50.0/yams.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/yams.png` & `yams-0.50.0/yams.png`

 * *Files identical despite different names*

### Comparing `yams-0.49.3/yams.svg` & `yams-0.50.0/yams.svg`

 * *Files identical despite different names*

