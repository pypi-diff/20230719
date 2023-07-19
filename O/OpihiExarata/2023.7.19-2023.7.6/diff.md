# Comparing `tmp/OpihiExarata-2023.7.19.tar.gz` & `tmp/OpihiExarata-2023.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpihiExarata-2023.7.19.tar", last modified: Wed Jul 19 05:03:05 2023, max compression
+gzip compressed data, was "OpihiExarata-2023.7.6.tar", last modified: Thu Jul  6 05:36:47 2023, max compression
```

## Comparing `OpihiExarata-2023.7.19.tar` & `OpihiExarata-2023.7.6.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:03:05.651361 OpihiExarata-2023.7.19/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-19 05:03:05.651361 OpihiExarata-2023.7.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 05:03:05.651361 OpihiExarata-2023.7.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:03:05.635361 OpihiExarata-2023.7.19/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:03:05.639361 OpihiExarata-2023.7.19/src/OpihiExarata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-19 05:03:05.000000 OpihiExarata-2023.7.19/src/OpihiExarata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-19 05:03:05.000000 OpihiExarata-2023.7.19/src/OpihiExarata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 05:03:05.000000 OpihiExarata-2023.7.19/src/OpihiExarata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-19 05:03:05.000000 OpihiExarata-2023.7.19/src/OpihiExarata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-19 05:03:05.000000 OpihiExarata-2023.7.19/src/OpihiExarata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-19 05:03:05.000000 OpihiExarata-2023.7.19/src/OpihiExarata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:03:05.639361 OpihiExarata-2023.7.19/src/opihiexarata/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:03:05.639361 OpihiExarata-2023.7.19/src/opihiexarata/astrometry/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/astrometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22668 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/astrometry/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)    29924 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/astrometry/webclient.py
--rw-r--r--   0 runner    (1001) docker     (123)    16247 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/configuration.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:03:05.639361 OpihiExarata-2023.7.19/src/opihiexarata/ephemeris/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/ephemeris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23092 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/ephemeris/jplhorizons.py
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/ephemeris/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:03:05.643361 OpihiExarata-2023.7.19/src/opihiexarata/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39220 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/gui/automatic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/gui/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)   129487 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/gui/manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/gui/name.py
--rw-r--r--   0 runner    (1001) docker     (123)    41611 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/gui/old_automatic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:03:05.647361 OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/automatic.ui
--rw-r--r--   0 runner    (1001) docker     (123)   264160 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/busy_image_pyukumuku.png
--rw-r--r--   0 runner    (1001) docker     (123)   276135 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/busy_image_pyukumuku_1of4.png
--rw-r--r--   0 runner    (1001) docker     (123)   277313 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/busy_image_pyukumuku_2of4.png
--rw-r--r--   0 runner    (1001) docker     (123)   278520 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/busy_image_pyukumuku_3of4.png
--rw-r--r--   0 runner    (1001) docker     (123)   282276 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/busy_image_pyukumuku_4of4.png
--rw-r--r--   0 runner    (1001) docker     (123)    81555 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/manual.ui
--rw-r--r--   0 runner    (1001) docker     (123)    61288 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/old_manual.ui
--rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/qtui_automatic.py
--rw-r--r--   0 runner    (1001) docker     (123)   125614 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/qtui_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/qtui_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10677 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/selector.ui
--rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/window_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    50589 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/gui/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:03:05.647361 OpihiExarata-2023.7.19/src/opihiexarata/library/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/library/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    16385 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/library/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/library/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/library/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/library/fits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/library/hint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/library/http.py
--rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/library/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/library/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/library/mpcrecord.py
--rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/library/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/library/phototable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/library/tcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/library/temporary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:03:05.647361 OpihiExarata-2023.7.19/src/opihiexarata/opihi/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/opihi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46295 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/opihi/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    22047 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/opihi/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    54721 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/opihi/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:03:05.651361 OpihiExarata-2023.7.19/src/opihiexarata/orbit/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/orbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/orbit/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    27658 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/orbit/orbfit.py
--rw-r--r--   0 runner    (1001) docker     (123)    18894 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/orbit/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:03:05.651361 OpihiExarata-2023.7.19/src/opihiexarata/photometry/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/photometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12147 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/photometry/panstarrs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34587 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/photometry/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:03:05.651361 OpihiExarata-2023.7.19/src/opihiexarata/propagate/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/propagate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/propagate/polynomial.py
--rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/propagate/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/src/opihiexarata/secrets.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:03:05.651361 OpihiExarata-2023.7.19/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-19 05:02:47.000000 OpihiExarata-2023.7.19/tests/test_global.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.333629 OpihiExarata-2023.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-06 05:36:29.000000 OpihiExarata-2023.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-06 05:36:47.333629 OpihiExarata-2023.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-06 05:36:29.000000 OpihiExarata-2023.7.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 05:36:47.333629 OpihiExarata-2023.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.305630 OpihiExarata-2023.7.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.313629 OpihiExarata-2023.7.6/src/OpihiExarata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-06 05:36:47.000000 OpihiExarata-2023.7.6/src/OpihiExarata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-06 05:36:47.000000 OpihiExarata-2023.7.6/src/OpihiExarata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 05:36:47.000000 OpihiExarata-2023.7.6/src/OpihiExarata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 05:36:47.000000 OpihiExarata-2023.7.6/src/OpihiExarata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-06 05:36:47.000000 OpihiExarata-2023.7.6/src/OpihiExarata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 05:36:47.000000 OpihiExarata-2023.7.6/src/OpihiExarata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.313629 OpihiExarata-2023.7.6/src/opihiexarata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.313629 OpihiExarata-2023.7.6/src/opihiexarata/astrometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/astrometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22668 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/astrometry/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29924 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/astrometry/webclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16247 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/configuration.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.317630 OpihiExarata-2023.7.6/src/opihiexarata/ephemeris/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/ephemeris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23092 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/ephemeris/jplhorizons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/ephemeris/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.317630 OpihiExarata-2023.7.6/src/opihiexarata/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39220 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/automatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)   129487 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41611 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/old_automatic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.325630 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/automatic.ui
+-rw-r--r--   0 runner    (1001) docker     (123)   264160 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/busy_image_pyukumuku.png
+-rw-r--r--   0 runner    (1001) docker     (123)   276135 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/busy_image_pyukumuku_1of4.png
+-rw-r--r--   0 runner    (1001) docker     (123)   277313 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/busy_image_pyukumuku_2of4.png
+-rw-r--r--   0 runner    (1001) docker     (123)   278520 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/busy_image_pyukumuku_3of4.png
+-rw-r--r--   0 runner    (1001) docker     (123)   282276 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/busy_image_pyukumuku_4of4.png
+-rw-r--r--   0 runner    (1001) docker     (123)    81555 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/manual.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    61288 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/old_manual.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/qtui_automatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125614 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/qtui_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/qtui_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10677 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/selector.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/window_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50589 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.329630 OpihiExarata-2023.7.6/src/opihiexarata/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16385 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/hint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/mpcrecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/phototable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/tcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/temporary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.329630 OpihiExarata-2023.7.6/src/opihiexarata/opihi/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/opihi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46007 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/opihi/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22047 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/opihi/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54721 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/opihi/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.333629 OpihiExarata-2023.7.6/src/opihiexarata/orbit/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/orbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/orbit/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27658 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/orbit/orbfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18894 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/orbit/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.333629 OpihiExarata-2023.7.6/src/opihiexarata/photometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/photometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12147 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/photometry/panstarrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34086 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/photometry/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.333629 OpihiExarata-2023.7.6/src/opihiexarata/propagate/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/propagate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/propagate/polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/propagate/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/secrets.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.333629 OpihiExarata-2023.7.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/tests/test_global.py
```

### Comparing `OpihiExarata-2023.7.19/LICENSE` & `OpihiExarata-2023.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/PKG-INFO` & `OpihiExarata-2023.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpihiExarata
-Version: 2023.7.19
+Version: 2023.7.6
 Summary: Analysis software for the IRTF Opihi telescope.
 Home-page: https://github.com/psmd-iberutaru/OpihiExarata
 Author: Sparrow
 Author-email: psmd.iberutaru@gmail.com
 Project-URL: Bug Tracker, https://github.com/psmd-iberutaru/OpihiExarata/issues
 Project-URL: Documentation, https://github.com/psmd-iberutaru/OpihiExarata
 Project-URL: Source Code, https://github.com/psmd-iberutaru/OpihiExarata
```

### Comparing `OpihiExarata-2023.7.19/README.md` & `OpihiExarata-2023.7.6/README.md`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/setup.py` & `OpihiExarata-2023.7.6/setup.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/OpihiExarata.egg-info/PKG-INFO` & `OpihiExarata-2023.7.6/src/OpihiExarata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpihiExarata
-Version: 2023.7.19
+Version: 2023.7.6
 Summary: Analysis software for the IRTF Opihi telescope.
 Home-page: https://github.com/psmd-iberutaru/OpihiExarata
 Author: Sparrow
 Author-email: psmd.iberutaru@gmail.com
 Project-URL: Bug Tracker, https://github.com/psmd-iberutaru/OpihiExarata/issues
 Project-URL: Documentation, https://github.com/psmd-iberutaru/OpihiExarata
 Project-URL: Source Code, https://github.com/psmd-iberutaru/OpihiExarata
```

### Comparing `OpihiExarata-2023.7.19/src/OpihiExarata.egg-info/SOURCES.txt` & `OpihiExarata-2023.7.6/src/OpihiExarata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/__init__.py` & `OpihiExarata-2023.7.6/src/opihiexarata/__init__.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/__main__.py` & `OpihiExarata-2023.7.6/src/opihiexarata/__main__.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/astrometry/solution.py` & `OpihiExarata-2023.7.6/src/opihiexarata/astrometry/solution.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/astrometry/webclient.py` & `OpihiExarata-2023.7.6/src/opihiexarata/astrometry/webclient.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/configuration.yaml` & `OpihiExarata-2023.7.6/src/opihiexarata/configuration.yaml`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/ephemeris/jplhorizons.py` & `OpihiExarata-2023.7.6/src/opihiexarata/ephemeris/jplhorizons.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/ephemeris/solution.py` & `OpihiExarata-2023.7.6/src/opihiexarata/ephemeris/solution.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/gui/__init__.py` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/gui/automatic.py` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/automatic.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/gui/functions.py` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/functions.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/gui/manual.py` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/manual.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/gui/name.py` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/name.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/gui/old_automatic.py` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/old_automatic.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/automatic.ui` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/automatic.ui`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/busy_image_pyukumuku.png` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/busy_image_pyukumuku.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/busy_image_pyukumuku_1of4.png` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/busy_image_pyukumuku_1of4.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/busy_image_pyukumuku_2of4.png` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/busy_image_pyukumuku_2of4.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/busy_image_pyukumuku_3of4.png` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/busy_image_pyukumuku_3of4.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/busy_image_pyukumuku_4of4.png` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/busy_image_pyukumuku_4of4.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/manual.ui` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/manual.ui`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/old_manual.ui` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/old_manual.ui`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/qtui_automatic.py` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/qtui_automatic.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/qtui_manual.py` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/qtui_manual.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/qtui_selector.py` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/qtui_selector.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/selector.ui` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/selector.ui`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/gui/qtui/window_icon.png` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/window_icon.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/gui/selector.py` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/selector.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/library/__init__.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/__init__.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/library/config.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/config.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/library/conversion.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/conversion.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/library/engine.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/engine.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/library/error.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/error.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/library/fits.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/fits.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/library/hint.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/hint.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/library/http.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/http.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/library/image.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/image.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/library/json.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/json.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/library/mpcrecord.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/mpcrecord.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/library/path.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/path.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/library/phototable.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/phototable.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/library/tcs.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/tcs.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/library/temporary.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/temporary.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/opihi/database.py` & `OpihiExarata-2023.7.6/src/opihiexarata/opihi/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -418,32 +418,25 @@
             line.
         """
         # We break up the record into its parts. We do not care about the
         # plus minus symbol.
         (
             datetime_str,
             zero_point_str,
-            plus_minus_str,
+            __,
             zero_point_error_str,
             filter_name_str,
         ) = record.split()
 
         # We use datetime to better format the ISO date time string.
         record_datetime = datetime.datetime.fromisoformat(datetime_str)
 
-        # Converting to numbers. If it cannot be converted to numbers, then 
-        # by definition, it is not really a valid record.
-        try:
-            zero_point = float(zero_point_str)
-        except ValueError:
-            zero_point = float("nan")
-        try:
-            zero_point_error = float(zero_point_error_str)
-        except ValueError:
-            zero_point_error_str = float("nan")
+        # Converting to numbers.
+        zero_point = float(zero_point_str)
+        zero_point_error = float(zero_point_error_str)
 
         # We can compile the dictionary from here. We include the datetime for
         # ease of handling.
         parsed_record_dictionary = {
             "datetime": datetime_str,
             "year": record_datetime.year,
             "month": record_datetime.month,
```

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/opihi/preprocess.py` & `OpihiExarata-2023.7.6/src/opihiexarata/opihi/preprocess.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/opihi/solution.py` & `OpihiExarata-2023.7.6/src/opihiexarata/opihi/solution.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/orbit/custom.py` & `OpihiExarata-2023.7.6/src/opihiexarata/orbit/custom.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/orbit/orbfit.py` & `OpihiExarata-2023.7.6/src/opihiexarata/orbit/orbfit.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/orbit/solution.py` & `OpihiExarata-2023.7.6/src/opihiexarata/orbit/solution.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/photometry/panstarrs.py` & `OpihiExarata-2023.7.6/src/opihiexarata/photometry/panstarrs.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/photometry/solution.py` & `OpihiExarata-2023.7.6/src/opihiexarata/photometry/solution.py`

 * *Files 1% similar despite different names*

```diff
@@ -499,17 +499,17 @@
                 )
             )
         else:
             self.filter_name = str(filter_name)
 
         # Extract the proper photometric values for the filter being used.
         filter_table_header = "{f}_mag".format(f=filter_name)
-        magnitude = inter_star_table[filter_table_header].as_array()
+        magnitude = inter_star_table[filter_table_header]
         # And the count data.
-        counts = inter_star_table["counts"].as_array()
+        counts = inter_star_table["counts"]
         # Instrument magnitudes.
         sqrt5_100 = 2.51188643151
         inst_magnitude = -sqrt5_100 * np.log10(counts / exposure_time)
 
         # We filter the stars so that we avoid using stars and targets
         # which otherwise would skew our results.
         # Stars which are too bright saturate our detector. We limit based on
@@ -540,25 +540,14 @@
         # We use the error on the mean, but instead we use medians and its
         # standard deviation equivalent to be robust to bad data points.
         n_stars = np.sum(np.isfinite(zero_points))
         zero_point_deviation = sp_stats.median_abs_deviation(
             zero_points, nan_policy="omit"
         )
         zero_point_error = zero_point_deviation / np.sqrt(n_stars)
-        # Final consistency check, if the values are not actually finite or 
-        # real values for that matter, the zero point is nothing. We also 
-        # properly handle the different cases of NaN for values and errors.
-        if not np.isfinite(zero_point):
-            zero_point = np.nan
-            zero_point_error = np.nan
-        elif not np.isfinite(zero_point_error):
-            zero_point_error = np.nan
-        else:
-            # All good.
-            pass
         return zero_point, zero_point_error
 
     def calculate_star_photon_counts_coordinate(
         self, ra: float, dec: float, radius: float
     ) -> float:
         """Calculate the total number of photometric counts at an RA DEC. The
         counts are already corrected for the sky counts.
```

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/propagate/polynomial.py` & `OpihiExarata-2023.7.6/src/opihiexarata/propagate/polynomial.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.7.19/src/opihiexarata/propagate/solution.py` & `OpihiExarata-2023.7.6/src/opihiexarata/propagate/solution.py`

 * *Files identical despite different names*

