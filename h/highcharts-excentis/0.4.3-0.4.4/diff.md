# Comparing `tmp/highcharts-excentis-0.4.3.tar.gz` & `tmp/highcharts-excentis-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/tom/programming/python-highcharts/dist/.tmp-mb2_xhyy/highcharts-excentis-0.4.3.tar", last modified: Mon Mar 27 10:08:55 2023, max compression
+gzip compressed data, was "/home/tom/programming/python-highcharts/dist/.tmp-uucge9h2/highcharts-excentis-0.4.4.tar", last modified: Wed Jul 19 09:57:48 2023, max compression
```

## Comparing `highcharts-excentis-0.4.3.tar` & `highcharts-excentis-0.4.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-27 10:08:55.000000 highcharts-excentis-0.4.3/
--rw-r--r--   0 tom       (1000) tom       (1000)     1068 2023-03-24 10:38:38.000000 highcharts-excentis-0.4.3/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)       74 2023-03-24 10:38:38.000000 highcharts-excentis-0.4.3/MANIFEST.in
--rw-r--r--   0 tom       (1000) tom       (1000)    20707 2023-03-27 10:08:55.000000 highcharts-excentis-0.4.3/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)    18640 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-27 10:08:55.000000 highcharts-excentis-0.4.3/highcharts_excentis/
--rw-r--r--   0 tom       (1000) tom       (1000)      221 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-27 10:08:55.000000 highcharts-excentis-0.4.3/highcharts_excentis/highcharts/
--rw-r--r--   0 tom       (1000) tom       (1000)       33 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highcharts/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)    22987 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highcharts/common.py
--rw-r--r--   0 tom       (1000) tom       (1000)    23655 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highcharts/highchart_types.py
--rw-r--r--   0 tom       (1000) tom       (1000)    17725 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highcharts/highcharts.py
--rw-r--r--   0 tom       (1000) tom       (1000)    22310 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highcharts/options.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-27 10:08:55.000000 highcharts-excentis-0.4.3/highcharts_excentis/highcharts/templates/
--rw-r--r--   0 tom       (1000) tom       (1000)      412 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highcharts/templates/base.html
--rw-r--r--   0 tom       (1000) tom       (1000)     2683 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highcharts/templates/content.html
--rw-r--r--   0 tom       (1000) tom       (1000)      294 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highcharts/templates/page.html
--rw-r--r--   0 tom       (1000) tom       (1000)      253 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highcharts/templates/test.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-27 10:08:55.000000 highcharts-excentis-0.4.3/highcharts_excentis/highmaps/
--rw-r--r--   0 tom       (1000) tom       (1000)       29 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highmaps/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)    22323 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highmaps/common.py
--rw-r--r--   0 tom       (1000) tom       (1000)     9143 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highmaps/highmap_helper.py
--rw-r--r--   0 tom       (1000) tom       (1000)    12119 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highmaps/highmap_types.py
--rw-r--r--   0 tom       (1000) tom       (1000)    18990 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highmaps/highmaps.py
--rw-r--r--   0 tom       (1000) tom       (1000)    18202 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highmaps/options.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-27 10:08:55.000000 highcharts-excentis-0.4.3/highcharts_excentis/highmaps/templates/
--rw-r--r--   0 tom       (1000) tom       (1000)      410 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highmaps/templates/base.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1391 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highmaps/templates/content.html
--rw-r--r--   0 tom       (1000) tom       (1000)      294 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highmaps/templates/page.html
--rw-r--r--   0 tom       (1000) tom       (1000)      253 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highmaps/templates/test.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-27 10:08:55.000000 highcharts-excentis-0.4.3/highcharts_excentis/highstock/
--rw-r--r--   0 tom       (1000) tom       (1000)       32 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highstock/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)    22923 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highstock/common.py
--rw-r--r--   0 tom       (1000) tom       (1000)    16492 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highstock/highstock.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5347 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highstock/highstock_helper.py
--rw-r--r--   0 tom       (1000) tom       (1000)    19610 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highstock/highstock_types.py
--rw-r--r--   0 tom       (1000) tom       (1000)    20254 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highstock/options.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-27 10:08:55.000000 highcharts-excentis-0.4.3/highcharts_excentis/highstock/templates/
--rw-r--r--   0 tom       (1000) tom       (1000)      412 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highstock/templates/base.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1432 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highstock/templates/content.html
--rw-r--r--   0 tom       (1000) tom       (1000)      320 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highstock/templates/page.html
--rw-r--r--   0 tom       (1000) tom       (1000)      253 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/highstock/templates/test.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1226 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/ipynb.py
--rw-r--r--   0 tom       (1000) tom       (1000)       90 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/highcharts_excentis/version.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-27 10:08:55.000000 highcharts-excentis-0.4.3/highcharts_excentis.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)    20707 2023-03-27 10:08:55.000000 highcharts-excentis-0.4.3/highcharts_excentis.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     1771 2023-03-27 10:08:55.000000 highcharts-excentis-0.4.3/highcharts_excentis.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-03-27 10:08:55.000000 highcharts-excentis-0.4.3/highcharts_excentis.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       14 2023-03-27 10:08:55.000000 highcharts-excentis-0.4.3/highcharts_excentis.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       20 2023-03-27 10:08:55.000000 highcharts-excentis-0.4.3/highcharts_excentis.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)     1661 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.3/pyproject.toml
--rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-03-27 10:08:55.000000 highcharts-excentis-0.4.3/setup.cfg
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-27 10:08:55.000000 highcharts-excentis-0.4.3/tests/
--rw-r--r--   0 tom       (1000) tom       (1000)     2972 2023-03-24 10:38:38.000000 highcharts-excentis-0.4.3/tests/test_highcharts.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1434 2023-03-24 10:38:38.000000 highcharts-excentis-0.4.3/tests/test_highmaps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1596 2023-03-24 10:38:38.000000 highcharts-excentis-0.4.3/tests/test_highstock.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-19 09:57:48.000000 highcharts-excentis-0.4.4/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1068 2023-03-24 10:38:38.000000 highcharts-excentis-0.4.4/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)       74 2023-03-24 10:38:38.000000 highcharts-excentis-0.4.4/MANIFEST.in
+-rw-r--r--   0 tom       (1000) tom       (1000)    20707 2023-07-19 09:57:48.000000 highcharts-excentis-0.4.4/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)    18640 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-19 09:57:48.000000 highcharts-excentis-0.4.4/highcharts_excentis/
+-rw-r--r--   0 tom       (1000) tom       (1000)      254 2023-07-19 09:21:12.000000 highcharts-excentis-0.4.4/highcharts_excentis/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-19 09:57:48.000000 highcharts-excentis-0.4.4/highcharts_excentis/highcharts/
+-rw-r--r--   0 tom       (1000) tom       (1000)       69 2023-07-19 09:12:00.000000 highcharts-excentis-0.4.4/highcharts_excentis/highcharts/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    22987 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/highcharts/common.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    23655 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/highcharts/highchart_types.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    17894 2023-07-19 09:04:25.000000 highcharts-excentis-0.4.4/highcharts_excentis/highcharts/highcharts.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    22310 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/highcharts/options.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-19 09:57:48.000000 highcharts-excentis-0.4.4/highcharts_excentis/highcharts/templates/
+-rw-r--r--   0 tom       (1000) tom       (1000)      412 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/highcharts/templates/base.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     2683 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/highcharts/templates/content.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      294 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/highcharts/templates/page.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      253 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/highcharts/templates/test.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-19 09:57:48.000000 highcharts-excentis-0.4.4/highcharts_excentis/highmaps/
+-rw-r--r--   0 tom       (1000) tom       (1000)       63 2023-07-19 09:12:11.000000 highcharts-excentis-0.4.4/highcharts_excentis/highmaps/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    22323 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/highmaps/common.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     9143 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/highmaps/highmap_helper.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    12119 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/highmaps/highmap_types.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    18990 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/highmaps/highmaps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    18202 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/highmaps/options.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-19 09:57:48.000000 highcharts-excentis-0.4.4/highcharts_excentis/highmaps/templates/
+-rw-r--r--   0 tom       (1000) tom       (1000)      410 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/highmaps/templates/base.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1391 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/highmaps/templates/content.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      294 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/highmaps/templates/page.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      253 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/highmaps/templates/test.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-19 09:57:48.000000 highcharts-excentis-0.4.4/highcharts_excentis/highstock/
+-rw-r--r--   0 tom       (1000) tom       (1000)       68 2023-07-19 09:12:23.000000 highcharts-excentis-0.4.4/highcharts_excentis/highstock/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    22923 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/highstock/common.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    16492 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/highstock/highstock.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5347 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/highstock/highstock_helper.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    19610 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/highstock/highstock_types.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    20254 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/highstock/options.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-19 09:57:48.000000 highcharts-excentis-0.4.4/highcharts_excentis/highstock/templates/
+-rw-r--r--   0 tom       (1000) tom       (1000)      412 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/highstock/templates/base.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1432 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/highstock/templates/content.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      320 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/highstock/templates/page.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      253 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/highstock/templates/test.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1226 2023-03-27 10:05:04.000000 highcharts-excentis-0.4.4/highcharts_excentis/ipynb.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       90 2023-07-19 09:35:36.000000 highcharts-excentis-0.4.4/highcharts_excentis/version.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-19 09:57:48.000000 highcharts-excentis-0.4.4/highcharts_excentis.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)    20707 2023-07-19 09:57:48.000000 highcharts-excentis-0.4.4/highcharts_excentis.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     1771 2023-07-19 09:57:48.000000 highcharts-excentis-0.4.4/highcharts_excentis.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-07-19 09:57:48.000000 highcharts-excentis-0.4.4/highcharts_excentis.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       14 2023-07-19 09:57:48.000000 highcharts-excentis-0.4.4/highcharts_excentis.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       20 2023-07-19 09:57:48.000000 highcharts-excentis-0.4.4/highcharts_excentis.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)     1661 2023-07-19 09:26:55.000000 highcharts-excentis-0.4.4/pyproject.toml
+-rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-07-19 09:57:48.000000 highcharts-excentis-0.4.4/setup.cfg
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-19 09:57:48.000000 highcharts-excentis-0.4.4/tests/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2972 2023-03-24 10:38:38.000000 highcharts-excentis-0.4.4/tests/test_highcharts.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1434 2023-03-24 10:38:38.000000 highcharts-excentis-0.4.4/tests/test_highmaps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1596 2023-03-24 10:38:38.000000 highcharts-excentis-0.4.4/tests/test_highstock.py
```

### Comparing `highcharts-excentis-0.4.3/LICENSE` & `highcharts-excentis-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `highcharts-excentis-0.4.3/PKG-INFO` & `highcharts-excentis-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: highcharts-excentis
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python Highcharts wrapper
 Author-email: Kyper Developers <developers@kyperdata.com>
 Maintainer-email: Excentis Development Team <support@excentis.com>, Tom Ghyselinck <tom.ghyselinck@excentis.com>
 License: Copyright (c) 2015 Kyper Data Technologies
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `highcharts-excentis-0.4.3/README.md` & `highcharts-excentis-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `highcharts-excentis-0.4.3/highcharts_excentis/highcharts/common.py` & `highcharts-excentis-0.4.4/highcharts_excentis/highcharts/common.py`

 * *Files identical despite different names*

### Comparing `highcharts-excentis-0.4.3/highcharts_excentis/highcharts/highchart_types.py` & `highcharts-excentis-0.4.4/highcharts_excentis/highcharts/highchart_types.py`

 * *Files identical despite different names*

### Comparing `highcharts-excentis-0.4.3/highcharts_excentis/highcharts/highcharts.py` & `highcharts-excentis-0.4.4/highcharts_excentis/highcharts/highcharts.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                 'https://code.highcharts.com/6/highcharts-more.js',
                 'https://code.highcharts.com/6/modules/heatmap.js',
                 'https://code.highcharts.com/6/modules/exporting.js'
             ]
 
         # set CSS src
         self.CSSsource = [
-                'https://www.highcharts.com/highslide/highslide.css',
+                'https://code.highcharts.com/6/css/highcharts.css',
 
             ]
 
         self.offline = kwargs.get("offline", False)
 
         # set data
         self.data = []
@@ -344,20 +344,25 @@
 
 
         if self.offline:
             opener = urllib.request.build_opener()
             opener.addheaders = [('User-Agent', 'Mozilla/5.0')]
 
             self.header_css = [
-                '<style>%s</style>' % opener.open(h).read() for h in self.CSSsource
+                '<style>' +
+                opener.open(source).read().decode('utf-8').replace('\n', '') +
+                '</style>' for source in self.CSSsource
             ]
 
             self.header_js = [
-                '<script type="text/javascript">%s</script>' % opener.open(h).read() for h in self.JSsource
+                '<script type="text/javascript">' +
+                opener.open(source).read().decode('utf-8').replace('\n', '') +
+                '</script>' for source in self.JSsource
             ]
+            
         else:
             self.header_css = [
                 '<link href="%s" rel="stylesheet" />' % h for h in self.CSSsource
             ]
 
             self.header_js = [
                 '<script type="text/javascript" src="%s"></script>' % h for h in self.JSsource
```

### Comparing `highcharts-excentis-0.4.3/highcharts_excentis/highcharts/options.py` & `highcharts-excentis-0.4.4/highcharts_excentis/highcharts/options.py`

 * *Files identical despite different names*

### Comparing `highcharts-excentis-0.4.3/highcharts_excentis/highcharts/templates/content.html` & `highcharts-excentis-0.4.4/highcharts_excentis/highcharts/templates/content.html`

 * *Files identical despite different names*

### Comparing `highcharts-excentis-0.4.3/highcharts_excentis/highmaps/common.py` & `highcharts-excentis-0.4.4/highcharts_excentis/highmaps/common.py`

 * *Files identical despite different names*

### Comparing `highcharts-excentis-0.4.3/highcharts_excentis/highmaps/highmap_helper.py` & `highcharts-excentis-0.4.4/highcharts_excentis/highmaps/highmap_helper.py`

 * *Files identical despite different names*

### Comparing `highcharts-excentis-0.4.3/highcharts_excentis/highmaps/highmap_types.py` & `highcharts-excentis-0.4.4/highcharts_excentis/highmaps/highmap_types.py`

 * *Files identical despite different names*

### Comparing `highcharts-excentis-0.4.3/highcharts_excentis/highmaps/highmaps.py` & `highcharts-excentis-0.4.4/highcharts_excentis/highmaps/highmaps.py`

 * *Files identical despite different names*

### Comparing `highcharts-excentis-0.4.3/highcharts_excentis/highmaps/options.py` & `highcharts-excentis-0.4.4/highcharts_excentis/highmaps/options.py`

 * *Files identical despite different names*

### Comparing `highcharts-excentis-0.4.3/highcharts_excentis/highmaps/templates/content.html` & `highcharts-excentis-0.4.4/highcharts_excentis/highmaps/templates/content.html`

 * *Files identical despite different names*

### Comparing `highcharts-excentis-0.4.3/highcharts_excentis/highstock/common.py` & `highcharts-excentis-0.4.4/highcharts_excentis/highstock/common.py`

 * *Files identical despite different names*

### Comparing `highcharts-excentis-0.4.3/highcharts_excentis/highstock/highstock.py` & `highcharts-excentis-0.4.4/highcharts_excentis/highstock/highstock.py`

 * *Files identical despite different names*

### Comparing `highcharts-excentis-0.4.3/highcharts_excentis/highstock/highstock_helper.py` & `highcharts-excentis-0.4.4/highcharts_excentis/highstock/highstock_helper.py`

 * *Files identical despite different names*

### Comparing `highcharts-excentis-0.4.3/highcharts_excentis/highstock/highstock_types.py` & `highcharts-excentis-0.4.4/highcharts_excentis/highstock/highstock_types.py`

 * *Files identical despite different names*

### Comparing `highcharts-excentis-0.4.3/highcharts_excentis/highstock/options.py` & `highcharts-excentis-0.4.4/highcharts_excentis/highstock/options.py`

 * *Files identical despite different names*

### Comparing `highcharts-excentis-0.4.3/highcharts_excentis/highstock/templates/content.html` & `highcharts-excentis-0.4.4/highcharts_excentis/highstock/templates/content.html`

 * *Files identical despite different names*

### Comparing `highcharts-excentis-0.4.3/highcharts_excentis/ipynb.py` & `highcharts-excentis-0.4.4/highcharts_excentis/ipynb.py`

 * *Files identical despite different names*

### Comparing `highcharts-excentis-0.4.3/highcharts_excentis.egg-info/PKG-INFO` & `highcharts-excentis-0.4.4/highcharts_excentis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: highcharts-excentis
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python Highcharts wrapper
 Author-email: Kyper Developers <developers@kyperdata.com>
 Maintainer-email: Excentis Development Team <support@excentis.com>, Tom Ghyselinck <tom.ghyselinck@excentis.com>
 License: Copyright (c) 2015 Kyper Data Technologies
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `highcharts-excentis-0.4.3/highcharts_excentis.egg-info/SOURCES.txt` & `highcharts-excentis-0.4.4/highcharts_excentis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `highcharts-excentis-0.4.3/pyproject.toml` & `highcharts-excentis-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `highcharts-excentis-0.4.3/tests/test_highcharts.py` & `highcharts-excentis-0.4.4/tests/test_highcharts.py`

 * *Files identical despite different names*

### Comparing `highcharts-excentis-0.4.3/tests/test_highmaps.py` & `highcharts-excentis-0.4.4/tests/test_highmaps.py`

 * *Files identical despite different names*

### Comparing `highcharts-excentis-0.4.3/tests/test_highstock.py` & `highcharts-excentis-0.4.4/tests/test_highstock.py`

 * *Files identical despite different names*

