# Comparing `tmp/pymodaq_plugins_mock-4.1.1.tar.gz` & `tmp/pymodaq_plugins_mock-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_plugins_mock-4.1.1.tar", last modified: Fri Jul  7 12:30:04 2023, max compression
+gzip compressed data, was "pymodaq_plugins_mock-4.1.2.tar", last modified: Wed Jul 19 15:29:41 2023, max compression
```

## Comparing `pymodaq_plugins_mock-4.1.1.tar` & `pymodaq_plugins_mock-4.1.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:30:04.226015 pymodaq_plugins_mock-4.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-07 12:30:04.226015 pymodaq_plugins_mock-4.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:30:04.226015 pymodaq_plugins_mock-4.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:30:04.222015 pymodaq_plugins_mock-4.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:30:04.222015 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:30:04.222015 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_move_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_move_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_Mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockCamera.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockTau.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockTauMulti.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_TCPServer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:30:04.222015 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:30:04.226015 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_MockAdaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TCPServer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:30:04.226015 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    11708 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock_spectro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_TCPServer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:30:04.226015 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_MockCamera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_TCPServer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:30:04.226015 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/daq_NDviewer_Mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:30:04.226015 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/hardware/
--rw-r--r--   0 runner    (1001) docker     (123)    26323 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/hardware/CNRS_degrade.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/hardware/camera_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/hardware/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:30:04.226015 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/models/PIDModelBeamSteering.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:29:54.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:30:04.222015 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-07 12:30:04.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-07 12:30:04.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:30:04.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-07 12:30:04.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-07 12:30:04.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-07 12:30:04.000000 pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:29:41.961621 pymodaq_plugins_mock-4.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-19 15:29:41.961621 pymodaq_plugins_mock-4.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 15:29:41.961621 pymodaq_plugins_mock-4.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:29:41.953621 pymodaq_plugins_mock-4.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:29:41.957621 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:29:41.957621 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_move_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_move_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_Mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockCamera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockTau.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockTauMulti.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_TCPServer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:29:41.957621 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:29:41.957621 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_MockAdaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TCPServer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:29:41.961621 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11708 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock_spectro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_TCPServer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:29:41.961621 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_MockCamera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_TCPServer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:29:41.961621 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/daq_NDviewer_Mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:29:41.961621 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)    26323 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/hardware/CNRS_degrade.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/hardware/camera_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/hardware/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:29:41.961621 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/models/PIDModelBeamSteering.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:29:30.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:29:41.957621 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-19 15:29:41.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-19 15:29:41.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 15:29:41.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-19 15:29:41.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-19 15:29:41.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 15:29:41.000000 pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock.egg-info/top_level.txt
```

### Comparing `pymodaq_plugins_mock-4.1.1/LICENSE` & `pymodaq_plugins_mock-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.1.1/PKG-INFO` & `pymodaq_plugins_mock-4.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq_plugins_mock
-Version: 4.1.1
+Version: 4.1.2
 Summary: Set of base PyMoDAQ plugins including Mock ones for development
 Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_mock
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: CECILL B
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_plugins_mock-4.1.1/README.rst` & `pymodaq_plugins_mock-4.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.1.1/setup.py` & `pymodaq_plugins_mock-4.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,11 +38,12 @@
 
 setup(
     version=version,
     packages=find_packages(where='./src'),
     package_dir={'': 'src'},
     include_package_data=True,
     entry_points={'pymodaq.plugins': f'{SHORT_PLUGIN_NAME} = {PLUGIN_NAME}',
-                  'pymodaq.pid_models': f"{SHORT_PLUGIN_NAME} = {PLUGIN_NAME}"},
+                  'pymodaq.pid_models': f"{SHORT_PLUGIN_NAME} = {PLUGIN_NAME}",
+                  'pymodaq.extensions': f"{SHORT_PLUGIN_NAME} = {PLUGIN_NAME}"},
     install_requires=['toml', ]+config['plugin-install']['packages-required'],
     **setupOpts
 )
```

### Comparing `pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_Mock.py` & `pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_Mock.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockCamera.py` & `pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockCamera.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockTau.py` & `pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockTau.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockTauMulti.py` & `pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockTauMulti.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Mock.py` & `pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Mock.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from qtpy import QtWidgets
+from qtpy import QtWidgets, QtCore
 
 from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
 from pymodaq.utils.data import DataFromPlugins, DataToExport
 import numpy as np
 from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base, comon_parameters, main
 
 from pymodaq.utils.math_utils import gauss1D
@@ -80,26 +80,31 @@
 
         Returns
         -------
         info: str
         initialized: bool
             False if initialization failed otherwise True
         """
+        self.emit_status(ThreadCommand('show_splash', 'Starting initialization'))
+        QtCore.QThread.msleep(500)
         self.ini_detector_init(old_controller=controller,
                                new_controller='Mock controller')
 
+        self.emit_status(ThreadCommand('show_splash', 'generating Mock Data'))
+        QtCore.QThread.msleep(500)
         self.set_Mock_data()
         self.emit_status(ThreadCommand('update_main_settings', [['wait_time'],
                                                                 self.settings.child('wait_time').value(), 'value']))
-
+        self.emit_status(ThreadCommand('show_splash', 'Displaying initial data'))
+        QtCore.QThread.msleep(500)
         # initialize viewers with the future type of data
         self.dte_signal_temp.emit(DataToExport('Mock0D', data=[DataFromPlugins(name='Mock1', data=[np.array([0])],
                                                                                dim='Data0D',
                                                                                labels=['Mock1', 'label2'])]))
-
+        self.emit_status(ThreadCommand('close_splash'))
         initialized = True
         info = 'RAS'
         return info, initialized
 
     def close(self):
         """
             not implemented.
@@ -141,22 +146,23 @@
         else:
             self.dte_signal.emit(DataToExport('Mock0D',
                                               data=[DataFromPlugins(name='Mock0D', data=data_tot,
                                                                     dim='Data0D', labels=['dat0', 'data1'])]))
         self.ind_data += 1
         if self.settings['lcd']:
             if not self.lcd_init:
-                self.emit_status(ThreadCommand('init_lcd', [dict(labels=['dat0', 'data1'], Nvals=2, digits=6)]))
+                self.emit_status(ThreadCommand('init_lcd', dict(labels=['dat0', 'data1'], Nvals=2, digits=6)))
                 QtWidgets.QApplication.processEvents()
                 self.lcd_init = True
 
-            self.emit_status(ThreadCommand('lcd', [data_tot]))
+            self.emit_status(ThreadCommand('lcd', data_tot))
 
     def stop(self):
         """
             not implemented.
         """
 
         return ""
 
+
 if __name__ == '__main__':
-    main(__file__)
+    main(__file__)
```

### Comparing `pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_MockAdaptive.py` & `pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_MockAdaptive.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TCPServer.py` & `pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TCPServer.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock.py` & `pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock_spectro.py` & `pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock_spectro.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_TCPServer.py` & `pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_TCPServer.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Mock.py` & `pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Mock.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_MockCamera.py` & `pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_MockCamera.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_TCPServer.py` & `pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_TCPServer.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/daq_NDviewer_Mock.py` & `pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/daq_NDviewer_Mock.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/hardware/CNRS_degrade.png` & `pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/hardware/CNRS_degrade.png`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/hardware/camera_wrapper.py` & `pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/hardware/camera_wrapper.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/hardware/wrapper.py` & `pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/hardware/wrapper.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock/models/PIDModelBeamSteering.py` & `pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock/models/PIDModelBeamSteering.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock.egg-info/PKG-INFO` & `pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq-plugins-mock
-Version: 4.1.1
+Version: 4.1.2
 Summary: Set of base PyMoDAQ plugins including Mock ones for development
 Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_mock
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: CECILL B
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_plugins_mock-4.1.1/src/pymodaq_plugins_mock.egg-info/SOURCES.txt` & `pymodaq_plugins_mock-4.1.2/src/pymodaq_plugins_mock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

