# Comparing `tmp/first-breaks-picking-0.2.0.tar.gz` & `tmp/first-breaks-picking-0.3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "first-breaks-picking-0.2.0.tar", last modified: Tue Jun 20 18:34:08 2023, max compression
+gzip compressed data, was "first-breaks-picking-0.3.0b0.tar", last modified: Wed Jul 19 05:44:41 2023, max compression
```

## Comparing `first-breaks-picking-0.2.0.tar` & `first-breaks-picking-0.3.0b0.tar`

### file list

```diff
@@ -1,56 +1,66 @@
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/
--rw-r--r--   0 daloro    (1000) daloro    (1000)    11357 2023-05-10 12:43:20.000000 first-breaks-picking-0.2.0/LICENSE
--rw-rw-r--   0 daloro    (1000) daloro    (1000)    23658 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/PKG-INFO
--rw-r--r--   0 daloro    (1000) daloro    (1000)    22444 2023-06-20 18:03:09.000000 first-breaks-picking-0.2.0/README.md
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/first_breaks/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.2.0/first_breaks/__init__.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/first_breaks/_pytorch/
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/first_breaks/_pytorch/models/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-06-14 14:08:31.000000 first-breaks-picking-0.2.0/first_breaks/_pytorch/models/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     5730 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/first_breaks/_pytorch/models/unet3plus.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)      352 2023-06-12 06:38:44.000000 first-breaks-picking-0.2.0/first_breaks/cli.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     1171 2023-06-14 14:08:31.000000 first-breaks-picking-0.2.0/first_breaks/const.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/first_breaks/desktop/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.2.0/first_breaks/desktop/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)    17108 2023-06-20 18:20:30.000000 first-breaks-picking-0.2.0/first_breaks/desktop/graph.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)    17672 2023-06-20 18:24:58.000000 first-breaks-picking-0.2.0/first_breaks/desktop/main_gui.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     6739 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/first_breaks/desktop/picking_widget.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     2700 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/first_breaks/desktop/threads.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     2394 2023-06-20 18:22:43.000000 first-breaks-picking-0.2.0/first_breaks/desktop/utils.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/first_breaks/picking/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-30 07:39:18.000000 first-breaks-picking-0.2.0/first_breaks/picking/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)      955 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/first_breaks/picking/ipicker.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     4952 2023-06-20 13:01:25.000000 first-breaks-picking-0.2.0/first_breaks/picking/picker_onnx.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     8990 2023-06-20 18:09:50.000000 first-breaks-picking-0.2.0/first_breaks/picking/task.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)      437 2023-06-12 06:38:44.000000 first-breaks-picking-0.2.0/first_breaks/picking/utils.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/first_breaks/sgy/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.2.0/first_breaks/sgy/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     7843 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/first_breaks/sgy/headers.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)    14416 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/first_breaks/sgy/reader.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/first_breaks/utils/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.2.0/first_breaks/utils/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)      635 2023-05-10 12:43:20.000000 first-breaks-picking-0.2.0/first_breaks/utils/debug.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     4191 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/first_breaks/utils/utils.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     3815 2023-05-26 13:27:32.000000 first-breaks-picking-0.2.0/first_breaks/utils/visualizations.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/first_breaks_picking.egg-info/
--rw-rw-r--   0 daloro    (1000) daloro    (1000)    23658 2023-06-20 18:34:08.000000 first-breaks-picking-0.2.0/first_breaks_picking.egg-info/PKG-INFO
--rw-rw-r--   0 daloro    (1000) daloro    (1000)     1290 2023-06-20 18:34:08.000000 first-breaks-picking-0.2.0/first_breaks_picking.egg-info/SOURCES.txt
--rw-rw-r--   0 daloro    (1000) daloro    (1000)        1 2023-06-20 18:34:08.000000 first-breaks-picking-0.2.0/first_breaks_picking.egg-info/dependency_links.txt
--rw-rw-r--   0 daloro    (1000) daloro    (1000)       71 2023-06-20 18:34:08.000000 first-breaks-picking-0.2.0/first_breaks_picking.egg-info/entry_points.txt
--rw-rw-r--   0 daloro    (1000) daloro    (1000)      168 2023-06-20 18:34:08.000000 first-breaks-picking-0.2.0/first_breaks_picking.egg-info/requires.txt
--rw-rw-r--   0 daloro    (1000) daloro    (1000)       19 2023-06-20 18:34:08.000000 first-breaks-picking-0.2.0/first_breaks_picking.egg-info/top_level.txt
--rw-r--r--   0 daloro    (1000) daloro    (1000)      337 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/setup.cfg
--rw-r--r--   0 daloro    (1000) daloro    (1000)     2229 2023-06-20 18:30:32.000000 first-breaks-picking-0.2.0/setup.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/tests/
--rw-r--r--   0 daloro    (1000) daloro    (1000)      330 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/tests/test_demo_sgy.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/tests/test_desktop/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/tests/test_desktop/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/tests/test_desktop/test_graph.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     1559 2023-06-20 14:17:10.000000 first-breaks-picking-0.2.0/tests/test_markdown_examples.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/tests/test_picking/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/tests/test_picking/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     1288 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/tests/test_picking/test_picker.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     3329 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/tests/test_picking/test_task.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/tests/test_sgy/
--rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/tests/test_sgy/__init__.py
--rw-r--r--   0 daloro    (1000) daloro    (1000)     1867 2023-06-20 14:27:17.000000 first-breaks-picking-0.2.0/tests/test_sgy/test_reader.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)    11357 2023-05-10 12:43:20.000000 first-breaks-picking-0.3.0b0/LICENSE
+-rw-rw-r--   0 daloro    (1000) daloro    (1000)    24007 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/PKG-INFO
+-rw-r--r--   0 daloro    (1000) daloro    (1000)    22791 2023-07-19 05:43:43.000000 first-breaks-picking-0.3.0b0/README.md
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.3.0b0/first_breaks/__init__.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks/_pytorch/
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks/_pytorch/models/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/first_breaks/_pytorch/models/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     5730 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/first_breaks/_pytorch/models/unet3plus.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)      352 2023-06-12 06:38:44.000000 first-breaks-picking-0.3.0b0/first_breaks/cli.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     1171 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/first_breaks/const.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks/data_models/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-07-17 07:07:08.000000 first-breaks-picking-0.3.0b0/first_breaks/data_models/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     1701 2023-07-18 13:44:34.000000 first-breaks-picking-0.3.0b0/first_breaks/data_models/dependent.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     2090 2023-07-18 17:00:55.000000 first-breaks-picking-0.3.0b0/first_breaks/data_models/independent.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)      441 2023-07-18 13:44:34.000000 first-breaks-picking-0.3.0b0/first_breaks/data_models/initialised_defaults.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks/desktop/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     5525 2023-07-18 16:48:46.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/byte_encode_unit_widget.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     1903 2023-07-18 16:49:22.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/combobox_with_mapping.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)    18931 2023-07-18 13:48:53.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/graph.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)    20070 2023-07-19 05:38:40.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/main_gui.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     6739 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/picking_widget.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     2661 2023-07-18 16:49:29.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/radioset_widget.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     3571 2023-07-18 16:49:46.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/slider_with_values.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     2700 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/threads.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     4238 2023-07-18 16:49:38.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/utils.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     7474 2023-07-18 16:47:54.000000 first-breaks-picking-0.3.0b0/first_breaks/desktop/visualization_settings_widget.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks/picking/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-30 07:39:18.000000 first-breaks-picking-0.3.0b0/first_breaks/picking/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)      955 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/first_breaks/picking/ipicker.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     4952 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/first_breaks/picking/picker_onnx.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     9351 2023-07-18 16:46:26.000000 first-breaks-picking-0.3.0b0/first_breaks/picking/task.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     2197 2023-07-18 17:00:56.000000 first-breaks-picking-0.3.0b0/first_breaks/picking/utils.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks/sgy/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.3.0b0/first_breaks/sgy/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     8608 2023-07-18 16:49:53.000000 first-breaks-picking-0.3.0b0/first_breaks/sgy/headers.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)    16232 2023-07-18 16:46:38.000000 first-breaks-picking-0.3.0b0/first_breaks/sgy/reader.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks/utils/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.3.0b0/first_breaks/utils/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)      635 2023-05-10 12:43:20.000000 first-breaks-picking-0.3.0b0/first_breaks/utils/debug.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     5833 2023-07-18 16:46:46.000000 first-breaks-picking-0.3.0b0/first_breaks/utils/utils.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     3815 2023-05-26 13:27:32.000000 first-breaks-picking-0.3.0b0/first_breaks/utils/visualizations.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/
+-rw-rw-r--   0 daloro    (1000) daloro    (1000)    24007 2023-07-19 05:44:41.000000 first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/PKG-INFO
+-rw-rw-r--   0 daloro    (1000) daloro    (1000)     1683 2023-07-19 05:44:41.000000 first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/SOURCES.txt
+-rw-rw-r--   0 daloro    (1000) daloro    (1000)        1 2023-07-19 05:44:41.000000 first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/dependency_links.txt
+-rw-rw-r--   0 daloro    (1000) daloro    (1000)       71 2023-07-19 05:44:41.000000 first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/entry_points.txt
+-rw-rw-r--   0 daloro    (1000) daloro    (1000)      184 2023-07-19 05:44:41.000000 first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/requires.txt
+-rw-rw-r--   0 daloro    (1000) daloro    (1000)       19 2023-07-19 05:44:41.000000 first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/top_level.txt
+-rw-r--r--   0 daloro    (1000) daloro    (1000)      337 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/setup.cfg
+-rw-rw-r--   0 daloro    (1000) daloro    (1000)     2238 2023-07-18 16:41:29.000000 first-breaks-picking-0.3.0b0/setup.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/tests/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)      330 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/tests/test_demo_sgy.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/tests/test_desktop/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/tests/test_desktop/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/tests/test_desktop/test_graph.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/tests/test_picking/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/tests/test_picking/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     1288 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/tests/test_picking/test_picker.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     3329 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/tests/test_picking/test_task.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     1467 2023-07-18 16:41:44.000000 first-breaks-picking-0.3.0b0/tests/test_readme_examples.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-07-19 05:44:41.852779 first-breaks-picking-0.3.0b0/tests/test_sgy/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-07-10 12:37:21.000000 first-breaks-picking-0.3.0b0/tests/test_sgy/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     1859 2023-07-18 12:38:11.000000 first-breaks-picking-0.3.0b0/tests/test_sgy/test_reader.py
```

### Comparing `first-breaks-picking-0.2.0/LICENSE` & `first-breaks-picking-0.3.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.2.0/PKG-INFO` & `first-breaks-picking-0.3.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: first-breaks-picking
-Version: 0.2.0
+Version: 0.3.0b0
 Summary: Tool for picking first breaks in seismic gather
 Home-page: https://github.com/DaloroAT/first_breaks_picking
 Author: Aleksei Tarasov
 Author-email: aleksei.v.tarasov@gmail.com
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/DaloroAT/first_breaks_picking
 Keywords: seismic,first-breaks,computer-vision,deep-learning,segmentation,data-science
@@ -17,15 +17,15 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8,<3.9
 Description-Content-Type: text/markdown
 Provides-Extra: gpu
 License-File: LICENSE
 
 # First breaks picking
 This project is devoted to pick waves that are the first to be detected on a seismogram (first breaks, first arrivals).
 Traditionally, this procedure is performed manually. When processing field data, the number of picks reaches hundreds of
@@ -372,19 +372,22 @@
 
 # you can see results of picking
 print(task.picks_in_samples)
 print(task.picks_in_ms)
 print(task.confidence)
 
 # you can export picks to file as plain text
-task.export_result('result.txt', as_plain=True)
+task.export_result_as_txt('result.txt')
 # or save as json file
-task.export_result('result.json', as_json=True)
+task.export_result_as_json('result.json')
 # or make a copy of source SGY and put picks to 236 byte
-task.export_result('result.segy', as_sgy=True)
+task.export_result_as_sgy('result.segy',
+                          byte_position=236,
+                          encoding='i',
+                          picks_unit='mcs')
 ```
 [code-block-end]:pick-fb
 
 ### Visualizations
 
 You can save the seismogram and picks as an image. We use Qt backend for visualizations. Here we describe some usage
 scenarios.
@@ -400,15 +403,15 @@
 from first_breaks.desktop.graph import export_image
 
 sgy_filename = 'data.sgy'
 image_filename = 'image.png'
 
 sgy = SGY(sgy_filename)
 export_image(sgy, image_filename,
-             normalize=False,
+             normalize=None,
              traces_window=(5, 10),
              time_window=(0, 200),
              height=300,
              width_per_trace=30)
 ```
 [code-block-end]:plot-sgy
 
@@ -475,15 +478,15 @@
             traces_per_gather=24,
             maximum_time=200)
 picker = PickerONNX()
 task = picker.process_task(task)
 
 export_image(task, image_filename,
              show_processing_region=False,
-             fill_black_left=False,
+             fill_black='right',
              width=1000)
 ```
 [code-block-end]:plot-sgy-real-picks
 
 ### *Limit processing region
 
 Unfortunately, processing of a part of a file is not currently supported natively. We will add this functionality soon!
@@ -565,24 +568,30 @@
 
 ### Processing grid
 
 Click on 4 button to toggle the display of the processing grid on or off. Horizontal line
 shows `Maximum time` and vertical lines are drawn at intervals equal to `Traces per gather`. The neural network
 processes blocks independently, as separate images.
 
+### Visual settings
+
+Click on 5 button to open window for visual settings. You can select gain, clip, normalization method,
+and trace values. In addition, you can also load a pick from a file, specifying how to read it.
+
 ### Save results
 
-Click on 5 button to save picks into file. Depending on file extension, results will be saved as `json`,
+Click on 6 button to save picks into file. Depending on file extension, results will be saved as `json`,
 as plain `txt`, or as `segy` file.
 
 For extensions `txt` and `json`, picking parameters and model confidence for each peak are additionally saved.
 
 When choosing an extension `segy`, the copy of original SGY file is saved with the values of the first breaks in the
-trace headers. They are stored in the last 4 bytes (236 byte if counting from 0) to be decoded as an unsigned integer.
-Values are in microseconds.
+trace headers. After selecting a file, you will be prompted to choose in which byte to save (counting starts from 1),
+in which units of measurement and how to encode.
+
 # Picking process
 
 Neural network process file as series of **images**. There is why **the traces should not be random**,
 since we are using information about adjacent traces.
 
 To obtain the first breaks we do the following steps:
 1) Read all traces in the file.
```

### Comparing `first-breaks-picking-0.2.0/README.md` & `first-breaks-picking-0.3.0b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -344,19 +344,22 @@
 
 # you can see results of picking
 print(task.picks_in_samples)
 print(task.picks_in_ms)
 print(task.confidence)
 
 # you can export picks to file as plain text
-task.export_result('result.txt', as_plain=True)
+task.export_result_as_txt('result.txt')
 # or save as json file
-task.export_result('result.json', as_json=True)
+task.export_result_as_json('result.json')
 # or make a copy of source SGY and put picks to 236 byte
-task.export_result('result.segy', as_sgy=True)
+task.export_result_as_sgy('result.segy',
+                          byte_position=236,
+                          encoding='i',
+                          picks_unit='mcs')
 ```
 [code-block-end]:pick-fb
 
 ### Visualizations
 
 You can save the seismogram and picks as an image. We use Qt backend for visualizations. Here we describe some usage
 scenarios.
@@ -372,15 +375,15 @@
 from first_breaks.desktop.graph import export_image
 
 sgy_filename = 'data.sgy'
 image_filename = 'image.png'
 
 sgy = SGY(sgy_filename)
 export_image(sgy, image_filename,
-             normalize=False,
+             normalize=None,
              traces_window=(5, 10),
              time_window=(0, 200),
              height=300,
              width_per_trace=30)
 ```
 [code-block-end]:plot-sgy
 
@@ -447,15 +450,15 @@
             traces_per_gather=24,
             maximum_time=200)
 picker = PickerONNX()
 task = picker.process_task(task)
 
 export_image(task, image_filename,
              show_processing_region=False,
-             fill_black_left=False,
+             fill_black='right',
              width=1000)
 ```
 [code-block-end]:plot-sgy-real-picks
 
 ### *Limit processing region
 
 Unfortunately, processing of a part of a file is not currently supported natively. We will add this functionality soon!
@@ -537,24 +540,30 @@
 
 ### Processing grid
 
 Click on 4 button to toggle the display of the processing grid on or off. Horizontal line
 shows `Maximum time` and vertical lines are drawn at intervals equal to `Traces per gather`. The neural network
 processes blocks independently, as separate images.
 
+### Visual settings
+
+Click on 5 button to open window for visual settings. You can select gain, clip, normalization method,
+and trace values. In addition, you can also load a pick from a file, specifying how to read it.
+
 ### Save results
 
-Click on 5 button to save picks into file. Depending on file extension, results will be saved as `json`,
+Click on 6 button to save picks into file. Depending on file extension, results will be saved as `json`,
 as plain `txt`, or as `segy` file.
 
 For extensions `txt` and `json`, picking parameters and model confidence for each peak are additionally saved.
 
 When choosing an extension `segy`, the copy of original SGY file is saved with the values of the first breaks in the
-trace headers. They are stored in the last 4 bytes (236 byte if counting from 0) to be decoded as an unsigned integer.
-Values are in microseconds.
+trace headers. After selecting a file, you will be prompted to choose in which byte to save (counting starts from 1),
+in which units of measurement and how to encode.
+
 # Picking process
 
 Neural network process file as series of **images**. There is why **the traces should not be random**,
 since we are using information about adjacent traces.
 
 To obtain the first breaks we do the following steps:
 1) Read all traces in the file.
```

### Comparing `first-breaks-picking-0.2.0/first_breaks/_pytorch/models/unet3plus.py` & `first-breaks-picking-0.3.0b0/first_breaks/_pytorch/models/unet3plus.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.2.0/first_breaks/const.py` & `first-breaks-picking-0.3.0b0/first_breaks/const.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.2.0/first_breaks/desktop/graph.py` & `first-breaks-picking-0.3.0b0/first_breaks/desktop/graph.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,33 @@
+import ast
 import os
 import warnings
 from pathlib import Path
 from typing import Any, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pyqtgraph as pg
 from PyQt5.QtCore import Qt, QTimer, pyqtSlot
 from PyQt5.QtGui import QColor, QFont, QPainterPath, QPen
 from PyQt5.QtWidgets import QApplication
+from pyqtgraph import AxisItem
 from pyqtgraph.exporters import ImageExporter
 from pyqtgraph.GraphicsScene.mouseEvents import MouseClickEvent
 
 from first_breaks.const import HIGH_DPI
+from first_breaks.data_models.independent import TColor, TNormalize
+from first_breaks.data_models.initialised_defaults import DEFAULTS
 from first_breaks.picking.task import Task
 from first_breaks.picking.utils import preprocess_gather
 from first_breaks.sgy.reader import SGY
 
 if HIGH_DPI:
     QApplication.setAttribute(Qt.AA_EnableHighDpiScaling, True)
     QApplication.setAttribute(Qt.AA_UseHighDpiPixmaps, True)
 
-TColor = Union[Tuple[int, int, int, int], Tuple[int, int, int]]
-
-
-class GraphDefaults:
-    normalize: bool = True
-    gain: float = 1.0
-    clip: float = 0.9
-    fill_black_left: bool = True
-    picks_color: TColor = (255, 0, 0)
-    region_contour_color: TColor = (100, 100, 100)
-    region_contour_width: float = 0.2
-    region_poly_color: TColor = (100, 100, 100, 50)
-
 
 class GraphWidget(pg.PlotWidget):
     def __init__(self, use_open_gl: bool = True, *args: Any, **kwargs: Any):
         super().__init__(useOpenGL=use_open_gl, *args, **kwargs)
         self.getPlotItem().disableAutoRange()
         self.setAntialiasing(False)
         self.getPlotItem().setClipToView(True)
@@ -44,63 +35,70 @@
 
         self.getPlotItem().invertY(True)
         self.getPlotItem().showAxis("top", True)
         self.getPlotItem().showAxis("bottom", False)
         self.x_ax = self.getPlotItem().getAxis("top")
         self.y_ax = self.getPlotItem().getAxis("left")
         text_size = 12
-        labelstyle = {"font-size": f"{text_size}pt"}
+        self.label_style = {"font-size": f"{text_size}pt"}
         font = QFont()
         font.setPointSize(text_size)
-        self.x_ax.setLabel("trace", **labelstyle)
-        self.y_ax.setLabel("t, ms", **labelstyle)
+        self.x_ax.setLabel(None, **self.label_style)
+        self.y_ax.setLabel("t, ms", **self.label_style)
         self.x_ax.setTickFont(font)
         self.y_ax.setTickFont(font)
         self.plotItem.ctrlMenu = None
 
+        self.x_ax.tickStrings = self.replace_tick_labels
+
         self.sgy: Optional[SGY] = None
-        self.picks_in_ms: Optional[np.ndarray] = None
-        self.picks_as_item: Optional[pg.PlotCurveItem] = None
+        self.nn_picks_in_ms: Optional[np.ndarray] = None
+        self.nn_picks_as_item: Optional[pg.PlotCurveItem] = None
+        self.extra_picks_as_item_list: Optional[List[pg.PlotCurveItem]] = []
         self.processing_region_as_items: List[pg.QtWidgets.QGraphicsPathItem] = []
         self.traces_as_items: List[pg.QtWidgets.QGraphicsPathItem] = []
         self.is_picks_modified_manually = False
+        self.x_ax_header: Optional[str] = None
 
         self.mouse_click_signal = pg.SignalProxy(self.sceneObj.sigMouseClicked, rateLimit=60, slot=self.mouse_clicked)
 
     def mouse_clicked(self, ev: Tuple[MouseClickEvent]) -> None:
         ev = ev[0]
-        if self.picks_as_item is not None and ev.button() == 1:
+        if self.nn_picks_as_item is not None and ev.button() == 1:
             mouse_point = self.getPlotItem().vb.mapSceneToView(ev.scenePos())
             x, y = mouse_point.x(), mouse_point.y()
-            ids, picks = self.picks_as_item.getData()
+            ids, picks = self.nn_picks_as_item.getData()
             closest = np.argmin(np.abs(ids - x))
             y = np.clip(y, 0, self.sgy.max_time_ms)
             picks[closest] = y
-            self.picks_as_item.setData(ids, picks)
-            self.picks_in_ms = picks
+            self.nn_picks_as_item.setData(ids, picks)
+            self.nn_picks_in_ms = picks
             self.is_picks_modified_manually = True
 
     def full_clean(self) -> None:
-        self.remove_picks()
+        self.remove_nn_picks()
         self.remove_traces()
         self.remove_processing_region()
-        self.picks_as_item = None
-        self.picks_in_ms = None
+        self.nn_picks_as_item = None
+        self.nn_picks_in_ms = None
         self.is_picks_modified_manually = False
         self.clear()
 
     def plotseis(
         self,
         sgy: SGY,
-        clip: float = GraphDefaults.clip,
-        gain: float = GraphDefaults.gain,
-        normalize: bool = GraphDefaults.normalize,
-        fill_black_left: bool = GraphDefaults.fill_black_left,
+        clip: float = DEFAULTS.clip,
+        gain: float = DEFAULTS.gain,
+        normalize: TNormalize = DEFAULTS.normalize,
+        x_axis: Optional[str] = DEFAULTS.x_axis,
+        fill_black: Optional[str] = DEFAULTS.fill_black,
         refresh_view: bool = True,
     ) -> None:
+        self.x_ax_header = x_axis
+
         self.sgy = sgy
 
         traces = self.sgy.read()
         traces = preprocess_gather(traces, gain=gain, clip=clip, normalize=normalize, copy=True)
 
         self.clear()
 
@@ -110,17 +108,39 @@
         self.getViewBox().setLimits(xMin=0, xMax=num_traces + 1, yMin=0, yMax=t[-1])
 
         if refresh_view:
             self.getPlotItem().setYRange(0, t[-1])
             self.getPlotItem().setXRange(0, num_traces + 1)
 
         for idx in range(num_traces):
-            self._plot_trace_fast(traces[:, idx], t, idx + 1, fill_black_left)
+            self._plot_trace_fast(traces[:, idx], t, idx + 1, fill_black)
+
+        self.x_ax.showLabel()
 
-    def _plot_trace_fast(self, trace: np.ndarray, t: np.ndarray, shift: int, fill_black_left: bool) -> None:
+    def replace_tick_labels(self, *args: Any, **kwargs: Any) -> List[str]:
+        self.x_ax.setLabel(self.x_ax_header, **self.label_style)
+        previous_labels = AxisItem.tickStrings(self.x_ax, *args, **kwargs)
+
+        if self.x_ax_header is not None:
+            labels_from_headers = []
+            for v in previous_labels:
+                v = ast.literal_eval(v)
+                if v % 1 == 0:
+                    v = int(v) - 1
+                    if 0 <= v < self.sgy.num_traces:
+                        labels_from_headers.append(str(self.sgy.traces_headers[self.x_ax_header].iloc[v]))
+                    else:
+                        labels_from_headers.append("")
+                else:
+                    labels_from_headers.append("")
+            return labels_from_headers
+        else:
+            return previous_labels
+
+    def _plot_trace_fast(self, trace: np.ndarray, t: np.ndarray, shift: int, fill_black: Optional[str]) -> None:
         connect = np.ones(len(t), dtype=np.int32)
         connect[-1] = 0
 
         trace[0] = 0
         trace[-1] = 0
 
         shifted_trace = trace + shift
@@ -129,37 +149,45 @@
         item = pg.QtWidgets.QGraphicsPathItem(path)
         pen = QPen(Qt.black, 1, Qt.SolidLine, Qt.FlatCap, Qt.MiterJoin)
         # pen.setWidthF(0.01)
         pen.setWidth(0.1)
         item.setPen(pen)
         item.setBrush(Qt.white)
         self.addItem(item)
+        self.traces_as_items.append(item)
 
-        rect = QPainterPath()
+        if fill_black is None:
+            return
+        else:
+            sign = -1 if fill_black == "left" else 1
 
-        sign = -1 if fill_black_left else 1
-        rect.addRect(shift, t[0], sign * 1.1 * max(np.abs(trace)), t[-1])
+            rect = QPainterPath()
+            rect.addRect(shift, t[0], sign * 1.1 * max(np.abs(shifted_trace)), t[-1])
 
-        patch = path.intersected(rect)
-        item = pg.QtWidgets.QGraphicsPathItem(patch)
+            patch = path.intersected(rect)
+            item = pg.QtWidgets.QGraphicsPathItem(patch)
 
-        pen = QPen(QColor(255, 255, 255, 0), 1, Qt.SolidLine, Qt.FlatCap, Qt.MiterJoin)
-        # pen.setWidthF(0.01)
-        pen.setWidth(0.1)
-        item.setPen(pen)
-        item.setBrush(Qt.black)
-        self.addItem(item)
-        self.traces_as_items.append(item)
+            pen = QPen(QColor(255, 255, 255, 0), 1, Qt.SolidLine, Qt.FlatCap, Qt.MiterJoin)
+            # pen.setWidthF(0.01)
+            pen.setWidth(0.1)
+            item.setPen(pen)
+            item.setBrush(Qt.black)
+            self.addItem(item)
+            self.traces_as_items.append(item)
 
-    def remove_picks(self) -> None:
+    def remove_nn_picks(self) -> None:
         self.is_picks_modified_manually = False
-        if self.picks_as_item:
-            self.removeItem(self.picks_as_item)
-            self.picks_as_item = None
-            self.picks_in_ms = None
+        if self.nn_picks_as_item:
+            self.removeItem(self.nn_picks_as_item)
+            self.nn_picks_as_item = None
+            self.nn_picks_in_ms = None
+
+    def remove_extra_picks(self) -> None:
+        for item in self.extra_picks_as_item_list:
+            self.removeItem(item)
 
     def remove_processing_region(self) -> None:
         if self.processing_region_as_items:
             for item in self.processing_region_as_items:
                 self.removeItem(item)
 
     def remove_traces(self) -> None:
@@ -167,26 +195,26 @@
             for item in self.traces_as_items:
                 self.removeItem(item)
 
     def plot_processing_region(
         self,
         traces_per_gather: int,
         maximum_time: float,
-        contour_color: TColor = GraphDefaults.region_contour_color,
-        poly_color: TColor = GraphDefaults.region_poly_color,
-        contour_width: float = GraphDefaults.region_contour_width,
+        region_contour_color: TColor = DEFAULTS.region_contour_color,
+        region_poly_color: TColor = DEFAULTS.region_poly_color,
+        region_contour_width: float = DEFAULTS.region_contour_width,
     ) -> None:
         self.remove_processing_region()
 
         num_sample, num_traces = self.sgy.shape
         sgy_end_time = (num_sample + 2) * self.sgy.dt_ms
         region_start_time = maximum_time if maximum_time > 0 else sgy_end_time
 
-        contour_pen = QPen(QColor(*contour_color), contour_width, Qt.DashLine, Qt.FlatCap, Qt.MiterJoin)
-        poly_brush = QColor(*poly_color)
+        contour_pen = QPen(QColor(*region_contour_color), region_contour_width, Qt.DashLine, Qt.FlatCap, Qt.MiterJoin)
+        poly_brush = QColor(*region_poly_color)
 
         # Vertical lines
         line_t = np.array([0, region_start_time])
         for idx in np.arange(traces_per_gather + 0.5, num_traces - 1, traces_per_gather):
             line_x = np.array([idx, idx])
             line_path = pg.arrayToQPath(line_x, line_t, np.ones(2, dtype=np.int32))
             line_item = pg.QtWidgets.QGraphicsPathItem(line_path)
@@ -200,28 +228,41 @@
         poly_path = pg.arrayToQPath(poly_x, poly_t, np.ones(4, dtype=np.int32))
         poly_item = pg.QtWidgets.QGraphicsPathItem(poly_path)
         poly_item.setPen(contour_pen)
         poly_item.setBrush(poly_brush)
         self.processing_region_as_items.append(poly_item)
         self.addItem(poly_item)
 
-    def plot_picks(self, picks_ms: Sequence[float], color: TColor = GraphDefaults.picks_color) -> None:
-        self.remove_picks()
+    def get_picks_as_item(
+        self,
+        picks_ms: Sequence[float],
+        color: TColor = DEFAULTS.picks_color,
+    ) -> pg.PlotCurveItem:
+        ids = np.arange(self.sgy.num_traces) + 1
+        line = pg.PlotCurveItem()
+        line.setData(ids, np.array(picks_ms))
+        pen = pg.mkPen(color=color, width=3)
+        line.setPen(pen)
+
+        return line
+
+    def plot_nn_picks(self, picks_ms: Sequence[float], color: TColor = DEFAULTS.picks_color) -> None:
+        self.remove_nn_picks()
         self.is_picks_modified_manually = False
 
-        picks_ms = np.array(picks_ms)
-        ids = np.arange(self.sgy.num_traces) + 1
+        self.nn_picks_in_ms = np.array(picks_ms)
+        self.nn_picks_as_item = self.get_picks_as_item(self.nn_picks_in_ms, color)
 
-        self.picks_in_ms = picks_ms
-        self.picks_as_item = pg.PlotCurveItem()
-        self.picks_as_item.setData(ids, picks_ms)
+        self.addItem(self.nn_picks_as_item)
 
-        pen = pg.mkPen(color=color, width=3)
-        self.picks_as_item.setPen(pen)
-        self.addItem(self.picks_as_item)
+    def plot_extra_picks(self, picks_ms: Sequence[float], color: TColor = DEFAULTS.picks_color) -> None:
+        picks = self.get_picks_as_item(picks_ms, color)
+
+        self.addItem(picks)
+        self.extra_picks_as_item_list.append(picks)
 
 
 class HighMemoryConsumption(Exception):
     pass
 
 
 class UnsupportedImageSize(Exception):
@@ -278,27 +319,28 @@
 
     def export(
         self,
         sgy: SGY,
         image_filename: Optional[Union[str, Path]],
         *args: Any,
         # content parameters
-        clip: float = GraphDefaults.clip,
-        gain: float = GraphDefaults.gain,
-        normalize: bool = GraphDefaults.normalize,
-        fill_black_left: bool = GraphDefaults.fill_black_left,
+        clip: float = DEFAULTS.clip,
+        gain: float = DEFAULTS.gain,
+        normalize: TNormalize = DEFAULTS.normalize,
+        fill_black: Optional[str] = DEFAULTS.fill_black,
         time_window: Optional[Tuple[float, float]] = None,
         traces_window: Optional[Tuple[float, float]] = None,
         picks_ms: Optional[Sequence[float]] = None,
         task: Optional[Task] = None,
         show_processing_region: bool = True,
-        picks_color: TColor = GraphDefaults.picks_color,
-        contour_color: TColor = GraphDefaults.region_contour_color,
-        poly_color: TColor = GraphDefaults.region_poly_color,
-        contour_width: float = GraphDefaults.region_contour_width,
+        picks_color: TColor = DEFAULTS.picks_color,
+        contour_color: TColor = DEFAULTS.region_contour_color,
+        poly_color: TColor = DEFAULTS.region_poly_color,
+        contour_width: float = DEFAULTS.region_contour_width,
+        x_axis: Optional[str] = DEFAULTS.x_axis,
         # rendering parameters
         height: int = 500,
         width: Optional[int] = None,
         width_per_trace: int = 20,
         headers_total_pixels: int = 50,
         headers_font_pixels: Optional[int] = None,
         time_spacing: Optional[int] = None,
@@ -316,48 +358,48 @@
                 num_traces = sgy.num_traces
                 width = int(width_per_trace * num_traces) + headers_total_pixels
             else:
                 width = int(width_per_trace * (traces_window[1] - traces_window[0])) + headers_total_pixels
 
         self.avoid_memory_bomb(height, width)
 
+        self.x_ax_header = x_axis
+
         self.clear()
-        self.plotseis(
-            sgy, normalize=normalize, clip=clip, gain=gain, fill_black_left=fill_black_left, refresh_view=True
-        )
+        self.plotseis(sgy, normalize=normalize, clip=clip, gain=gain, fill_black=fill_black, refresh_view=True)
 
         if task:
             picks_to_plot = task.picks_in_ms  # type: ignore
         elif picks_ms is not None:
             picks_to_plot = picks_ms  # type: ignore
         else:
             picks_to_plot = None  # type: ignore
 
         if picks_to_plot is not None:
-            self.plot_picks(picks_to_plot, color=picks_color)
+            self.plot_nn_picks(picks_to_plot, color=picks_color)
 
         if task is not None and show_processing_region:
             self.plot_processing_region(
                 maximum_time=task.maximum_time_parsed,
                 traces_per_gather=task.traces_per_gather_parsed,
-                contour_color=contour_color,
-                poly_color=poly_color,
-                contour_width=contour_width,
+                region_contour_color=contour_color,
+                region_poly_color=poly_color,
+                region_contour_width=contour_width,
             )
 
         if time_window:
             self.getPlotItem().setYRange(time_window[0], time_window[1], padding=0)
         if traces_window:
             self.getPlotItem().setXRange(traces_window[0], traces_window[1], padding=0)
 
         headers_font_pixels = headers_font_pixels or int(0.35 * headers_total_pixels)
         labelstyle = {"font-size": f"{headers_font_pixels}px"}
         tickfont = QFont()
         tickfont.setPixelSize(max(int(0.9 * headers_font_pixels), 1))
-        self.x_ax.setLabel("trace", **labelstyle)
+        self.x_ax.setLabel(self.x_ax_header, **labelstyle)
         self.y_ax.setLabel("t, ms", **labelstyle)
         self.x_ax.setTickFont(tickfont)
         self.y_ax.setTickFont(tickfont)
 
         self.x_ax.setHeight(headers_total_pixels)
 
         if time_spacing:
@@ -390,26 +432,27 @@
 
 
 def export_image(
     source: Union[str, Path, bytes, np.ndarray, SGY, Task],
     image_filename: Optional[Union[str, Path]],
     *args: Any,
     dt_mcs: float = 1e3,
-    clip: float = GraphDefaults.clip,
-    gain: float = GraphDefaults.gain,
-    normalize: bool = GraphDefaults.normalize,
-    fill_black_left: bool = GraphDefaults.fill_black_left,
+    clip: float = DEFAULTS.clip,
+    gain: float = DEFAULTS.gain,
+    normalize: TNormalize = DEFAULTS.normalize,
+    fill_black: Optional[str] = DEFAULTS.fill_black,
     time_window: Optional[Tuple[float, float]] = None,
     traces_window: Optional[Tuple[float, float]] = None,
     picks_ms: Optional[Sequence[float]] = None,
     show_processing_region: bool = True,
-    picks_color: TColor = GraphDefaults.picks_color,
-    contour_color: TColor = GraphDefaults.region_contour_color,
-    poly_color: TColor = GraphDefaults.region_poly_color,
-    contour_width: float = GraphDefaults.region_contour_width,
+    picks_color: TColor = DEFAULTS.picks_color,
+    contour_color: TColor = DEFAULTS.region_contour_color,
+    poly_color: TColor = DEFAULTS.region_poly_color,
+    contour_width: float = DEFAULTS.region_contour_width,
+    x_axis: Optional[str] = DEFAULTS.x_axis,
     # rendering parameters
     height: int = 500,
     width: Optional[int] = None,
     width_per_trace: int = 20,
     headers_total_pixels: int = 50,
     headers_font_pixels: Optional[int] = None,
     time_spacing: Optional[int] = None,
@@ -442,24 +485,25 @@
     window.setAntialiasing(True)
     window.export(
         sgy=sgy,
         image_filename=image_filename,
         clip=clip,
         gain=gain,
         normalize=normalize,
-        fill_black_left=fill_black_left,
+        fill_black=fill_black,
         time_window=time_window,
         traces_window=traces_window,
         picks_ms=picks_ms,
         task=task,
         show_processing_region=show_processing_region,
         picks_color=picks_color,
         contour_color=contour_color,
         poly_color=poly_color,
         contour_width=contour_width,
+        x_axis=x_axis,
         height=height,
         width=width,
         width_per_trace=width_per_trace,
         headers_total_pixels=headers_total_pixels,
         headers_font_pixels=headers_font_pixels,
         time_spacing=time_spacing,
         traces_spacing=traces_spacing,
```

### Comparing `first-breaks-picking-0.2.0/first_breaks/desktop/main_gui.py` & `first-breaks-picking-0.3.0b0/first_breaks/desktop/main_gui.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 import sys
 import warnings
 from pathlib import Path
-from typing import Any, Dict, Optional, Type, Union
+from typing import Any, Dict, Optional, Tuple, Type, Union
 
 from PyQt5.QtCore import QSize, Qt, QThreadPool
 from PyQt5.QtWidgets import (
     QAction,
     QApplication,
     QDialog,
     QFileDialog,
     QHBoxLayout,
     QLabel,
     QMainWindow,
     QProgressBar,
     QSizePolicy,
-    QSlider,
     QStyle,
     QToolBar,
     QWidget,
 )
 
 from first_breaks.const import DEMO_SGY_PATH, HIGH_DPI, MODEL_ONNX_HASH, MODEL_ONNX_PATH
+from first_breaks.data_models.dependent import TraceHeaderParams
+from first_breaks.desktop.byte_encode_unit_widget import QDialogByteEncodeUnit
 from first_breaks.desktop.graph import GraphWidget
 from first_breaks.desktop.picking_widget import PickingWindow
 from first_breaks.desktop.threads import CallInThread, PickerQRunnable
 from first_breaks.desktop.utils import MessageBox, set_geometry
+from first_breaks.desktop.visualization_settings_widget import (
+    PicksFromFileSettings,
+    PlotseisSettings,
+    VisualizationSettingsWidget,
+)
 from first_breaks.picking.ipicker import IPicker
 from first_breaks.picking.picker_onnx import PickerONNX
 from first_breaks.picking.task import Task
 from first_breaks.sgy.reader import SGY
 from first_breaks.utils.utils import (
+    UnitsConverter,
     calc_hash,
     download_demo_sgy,
     download_model_onnx,
     multiply_iterable_by,
     remove_unused_kwargs,
 )
 
@@ -61,28 +68,14 @@
     sgy_selected: bool = False
     model_loaded: bool = False
 
     def is_ready(self) -> bool:
         return (self.sgy_selected == self.model_loaded) is True
 
 
-class SliderConverter:
-    multiplier = 10
-
-    @classmethod
-    def slider2value(cls, slider_value: int) -> float:
-        a = slider_value / cls.multiplier
-        return a
-
-    @classmethod
-    def value2slider(cls, value: float) -> int:
-        a = int(cls.multiplier * value)
-        return a
-
-
 class MainWindow(QMainWindow):
     def __init__(self, use_open_gl: bool = True):  # type: ignore
         super(MainWindow, self).__init__()
 
         if getattr(sys, "frozen", False):
             self.main_folder = Path(sys._MEIPASS)  # type: ignore
         else:
@@ -130,27 +123,19 @@
         self.button_processing_show.setCheckable(True)
         if self.need_processing_region:
             self.button_processing_show.toggle()
         self.toolbar.addAction(self.button_processing_show)
 
         self.toolbar.addSeparator()
 
-        default_gain_value = 1.0
-        self.gain_value = default_gain_value
-        self.gain_label = QLabel(str(default_gain_value))
-        self.slider_gain = QSlider(Qt.Horizontal)
-        self.slider_gain.setRange(SliderConverter.value2slider(-5), SliderConverter.value2slider(5))
-        self.slider_gain.setValue(SliderConverter.value2slider(1))
-        self.slider_gain.setSingleStep(SliderConverter.value2slider(0.1))
-        self.slider_gain.wheelEvent = lambda *args: args[-1].ignore()  # block scrolling with wheel
-        self.slider_gain.setMaximumWidth(150)
-        self.slider_gain.valueChanged.connect(self.gain_changed)
-        self.slider_gain.sliderReleased.connect(self.update_plot)
-        self.toolbar.addWidget(self.slider_gain)
-        self.toolbar.addWidget(self.gain_label)
+        icon_visual_settings = self.style().standardIcon(QStyle.SP_BrowserReload)
+        self.button_visual_settings = QAction(icon_visual_settings, "Show visual settings", self)
+        self.button_visual_settings.triggered.connect(self.show_visual_settings_window)
+        self.button_visual_settings.setEnabled(False)
+        self.toolbar.addAction(self.button_visual_settings)
 
         icon_export = self.style().standardIcon(QStyle.SP_DialogSaveButton)
         # icon_export = QIcon(str(self.main_folder / "icons" / "export.png"))
         self.button_export = QAction(icon_export, "Export picks to file", self)
         self.button_export.triggered.connect(self.export)
         self.button_export.setEnabled(False)
         self.toolbar.addAction(self.button_export)
@@ -175,21 +160,37 @@
         self.status.addPermanentWidget(status_widget)
 
         # graph widget
         self.graph = GraphWidget(use_open_gl=use_open_gl, background="w")
         self.graph.hide()
         self.setCentralWidget(self.graph)
 
+        # visual settings widget
+        self.plotseis_settings = PlotseisSettings()
+        first_byte = 1
+        self.picks_from_file_settings = PicksFromFileSettings(byte_position=first_byte)
+        self.visual_settings_widget = VisualizationSettingsWidget(
+            hide_on_close=True,
+            first_byte=first_byte,
+            **{**self.plotseis_settings.model_dump(), **self.picks_from_file_settings.model_dump()},
+        )
+        self.visual_settings_widget.hide()
+        self.visual_settings_widget.export_plotseis_settings_signal.connect(self.update_plotseis_settings)
+        self.visual_settings_widget.export_picks_from_file_settings_signal.connect(self.update_picks_from_file_settings)
+        self.visual_settings_widget.toggle_picks_from_file_signal.connect(self.toggle_picks_from_file)
+        self.is_toggled_picks_from_file = False
+
         # placeholders
         self.sgy: Optional[SGY] = None
         self.fn_sgy: Optional[Union[str, Path]] = None
         self.ready_to_process = ReadyToProcess()
         self.last_task: Optional[Task] = None
         self.settings: Optional[Dict[str, Any]] = None
         self.last_folder: Optional[Union[str, Path]] = None
+        self.picks_from_file_in_ms: Optional[Tuple[Union[int, float], ...]] = None
 
         self.picker_class: Type[IPicker] = PickerONNX
         self.picker: Optional[IPicker] = None
         self.picker_hash = MODEL_ONNX_HASH
         self.picker_extra_kwargs_init = {"show_progressbar": False, "device": "cpu"}
 
         self.picking_window_class = PickingWindow
@@ -211,18 +212,14 @@
     def set_last_folder_based_on_file(self, file: Union[str, Path]) -> None:
         file = Path(file)
         if file.exists():
             self.last_folder = str(file.parent)
         else:
             self.last_folder = None
 
-    def gain_changed(self, gain_from_slider: int) -> None:
-        self.gain_value = SliderConverter.slider2value(gain_from_slider)
-        self.gain_label.setText(str(self.gain_value))
-
     def _thread_init_net(self, weights: Union[str, Path]) -> None:
         task = CallInThread(self.picker_class, model_path=weights, **self.picker_extra_kwargs_init)
         task.signals.result.connect(self.init_net)
         self.threadpool.start(task)
 
     def init_net(self, picker: PickerONNX) -> None:
         self.picker = picker
@@ -295,15 +292,15 @@
 
     def on_progressbar_task(self, value: int) -> None:
         self.status_progress.setValue(value)
 
     def on_result_task(self, result: Task) -> None:
         self.store_task(result)
         if result.success:
-            self.graph.plot_picks(self.last_task.picks_in_ms)
+            self.graph.plot_nn_picks(self.last_task.picks_in_ms)
             self.run_processing_region()
             self.button_export.setEnabled(True)
         else:
             window_error = MessageBox(self, title="InternalError", message=result.error_message)
             window_error.exec_()
 
         self.button_get_filename.setEnabled(True)
@@ -325,22 +322,58 @@
                 self.last_task.traces_per_gather_parsed, self.last_task.maximum_time_parsed
             )
 
     def hide_processing_region(self) -> None:
         if self.last_task and self.last_task.success:
             self.graph.remove_processing_region()
 
-    def show_picks(self) -> None:
+    def show_nn_picks(self) -> None:
         if self.last_task and self.last_task.success:
-            self.graph.plot_picks(self.last_task.picks_in_ms)
+            self.graph.plot_nn_picks(self.last_task.picks_in_ms)
+
+    def read_picks_from_file(self) -> None:
+        picks = self.sgy.read_custom_trace_header(
+            **TraceHeaderParams(**self.picks_from_file_settings.model_dump()).model_dump(),
+        )
+        units_converter = UnitsConverter(sgy_mcs=self.sgy.dt_mcs)
+        if self.picks_from_file_settings.picks_unit == "sample":
+            self.picks_from_file_in_ms = units_converter.index2ms(picks)  # type: ignore
+        elif self.picks_from_file_settings.picks_unit == "mcs":
+            self.picks_from_file_in_ms = units_converter.mcs2ms(picks)  # type: ignore
+        else:
+            self.picks_from_file_in_ms = picks
+
+    def update_picks_from_file_settings(self, new_settings: PicksFromFileSettings) -> None:
+        print(new_settings)
+        self.picks_from_file_settings = new_settings
+
+    def toggle_picks_from_file(self, toggled: bool) -> None:
+        self.is_toggled_picks_from_file = toggled
+        self.show_picks_from_file()
+
+    def show_picks_from_file(self) -> None:
+        if self.is_toggled_picks_from_file:
+            self.read_picks_from_file()
+            self.graph.plot_extra_picks(picks_ms=self.picks_from_file_in_ms, color=(0, 0, 255))
+        else:
+            self.graph.remove_extra_picks()
+
+    def update_plotseis_settings(self, new_settings: PlotseisSettings) -> None:
+        self.plotseis_settings = new_settings
+        self.update_plot(False)
 
     def update_plot(self, refresh_view: bool = False) -> None:
-        self.graph.plotseis(self.sgy, gain=self.gain_value, refresh_view=refresh_view)
+        self.graph.plotseis(self.sgy, refresh_view=refresh_view, **self.plotseis_settings.model_dump())
         self.show_processing_region()
-        self.show_picks()
+        self.show_nn_picks()
+        self.show_picks_from_file()
+
+    def show_visual_settings_window(self) -> None:
+        self.visual_settings_widget.show()
+        self.visual_settings_widget.focusWidget()
 
     def unlock_pickng_if_ready(self) -> None:
         if self.ready_to_process.is_ready():
             self.button_fb.setEnabled(True)
             self.status_message.setText("Click on picking to start processing")
 
     def load_nn(self, filename: Optional[Union[str, Path]] = None) -> None:
@@ -381,19 +414,21 @@
                 filter="SEGY-file (*.segy *.sgy);; Any file (*)",
             )
         if filename:
             try:
                 self.fn_sgy = Path(filename)
                 self.last_task = None
                 self.sgy = SGY(self.fn_sgy)
+                self.picks_from_file_in_ms = None
 
                 self.graph.full_clean()
                 self.update_plot(refresh_view=True)
                 self.graph.show()
                 self.button_export.setEnabled(False)
+                self.button_visual_settings.setEnabled(True)
 
                 self.button_get_filename.setEnabled(True)
                 self.ready_to_process.sgy_selected = True
 
                 if not self.ready_to_process.model_loaded:
                     status_message = "Load model to start picking"
                     self.status_message.setText(status_message)
@@ -414,22 +449,27 @@
             filename = Path(filename).resolve()
             if self.last_task is not None and self.last_task.success:
                 filename.parent.mkdir(parents=True, exist_ok=True)
 
                 picks_in_samples_prev = self.last_task.picks_in_samples
                 if self.graph.is_picks_modified_manually:
                     self.last_task.picks_in_samples = multiply_iterable_by(
-                        self.graph.picks_in_ms, 1 / self.sgy.dt_ms, int
+                        self.graph.nn_picks_in_ms, 1 / self.sgy.dt_ms, int
                     )
                 if filename.suffix.lower() in (".sgy", ".segy"):
-                    self.last_task.export_result(str(filename), as_sgy=True)  # type: ignore
+                    save_params = QDialogByteEncodeUnit(first_byte=1, byte_position=237, encoding="I", picks_unit="mcs")
+                    save_params.setWindowTitle("How to save first breaks")
+                    save_params.show()
+                    save_params.exec_()
+                    export_params = save_params.get_values()
+                    self.last_task.export_result_as_sgy(str(filename), **export_params)  # type: ignore
                 elif filename.suffix.lower() == ".txt":
-                    self.last_task.export_result(str(filename), as_plain=True)
+                    self.last_task.export_result_as_txt(str(filename))
                 elif filename.suffix.lower() == ".json":
-                    self.last_task.export_result(str(filename), as_json=True)
+                    self.last_task.export_result_as_json(str(filename))
                 else:
                     message_er = "The file can only be saved in '.sgy', '.segy', '.txt, or '.json' formats"
                     window_err = MessageBox(self, title="Wrong filename", message=message_er)
                     window_err.exec_()
                 if self.graph.is_picks_modified_manually:
                     self.last_task.picks_in_samples = picks_in_samples_prev
```

### Comparing `first-breaks-picking-0.2.0/first_breaks/desktop/picking_widget.py` & `first-breaks-picking-0.3.0b0/first_breaks/desktop/picking_widget.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.2.0/first_breaks/desktop/threads.py` & `first-breaks-picking-0.3.0b0/first_breaks/desktop/threads.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.2.0/first_breaks/picking/ipicker.py` & `first-breaks-picking-0.3.0b0/first_breaks/picking/ipicker.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.2.0/first_breaks/picking/picker_onnx.py` & `first-breaks-picking-0.3.0b0/first_breaks/picking/picker_onnx.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.2.0/first_breaks/picking/task.py` & `first-breaks-picking-0.3.0b0/first_breaks/picking/task.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import warnings
 from pathlib import Path
-from typing import List, Optional, Sequence, Tuple, Union
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
 
 from first_breaks.sgy.reader import SGY
 from first_breaks.utils.utils import chunk_iterable, multiply_iterable_by
 
@@ -144,72 +144,86 @@
     @property
     def picks_in_mcs(self) -> Optional[List[int]]:
         if self.picks_in_samples is not None:
             return multiply_iterable_by(self.picks_in_samples, self.sgy.dt_mcs, cast_to=int)  # type: ignore
         else:
             return None
 
-    def export_result(
-        self, filename: Union[str, Path], as_plain: bool = False, as_json: bool = False, as_sgy: bool = False
-    ) -> None:
+    def _check_and_convert_picks(self) -> List[float]:  # type: ignore
         if self.picks_in_samples is None:
             raise ValueError("There are no picks. Put them manually or process the task first")
-
-        if sum([as_plain, as_json, as_sgy]) == 0:
-            raise ValueError("One of the options 'as_plain', 'as_json', or 'as_sgy' must be explicitly selected.")
-        elif sum([as_plain, as_json, as_sgy]) > 1:
-            raise ValueError("Only one of the options 'as_plain', 'as_json', or 'as_sgy' can be selected.")
-
         if isinstance(self.picks_in_samples, (tuple, list)):
             picks_in_samples = self.picks_in_samples
         elif isinstance(self.picks_in_samples, np.ndarray):
             picks_in_samples = self.picks_in_samples.tolist()
         else:
             raise TypeError("Only 1D sequence can be saved")
+        return picks_in_samples  # type: ignore
 
-        if as_sgy:
-            self.sgy.export_sgy_with_picks(filename, picks_in_samples)  # type: ignore
+    def _prepare_output_for_nonbinary_export(self) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+        picks_in_samples = self._check_and_convert_picks()
+        picks_in_ms = self.sgy.units_converter.index2ms(picks_in_samples, cast_to=float)
+
+        confidence = self.confidence
+
+        is_source_file = isinstance(self.sgy.source, (str, Path))
+        if is_source_file:
+            source_filename = str(Path(self.sgy.source).name)  # type: ignore
+            source_full_name = str(Path(self.sgy.source).resolve())  # type: ignore
         else:
-            picks_in_ms = multiply_iterable_by(picks_in_samples, multiplier=self.sgy.dt_ms)
-            confidence = self.confidence
+            source_filename = None
+            source_full_name = None
 
-            is_source_file = isinstance(self.sgy.source, (str, Path))
-            if is_source_file:
-                source_filename = str(Path(self.sgy.source).name)  # type: ignore
-                source_full_name = str(Path(self.sgy.source).resolve())  # type: ignore
-            else:
-                source_filename = None
-                source_full_name = None
+        meta = {
+            "is_source_file": is_source_file,
+            "is_source_ndarray": self.sgy.is_source_ndarray,
+            "filename": source_filename,
+            "full_name": source_full_name,
+            "hash": self.sgy.get_hash(),
+            "dt_ms": self.sgy.dt_ms,
+            "is_picked_with_model": bool(self.success),
+            "model_hash": self.model_hash,
+            "traces_per_gather": self.traces_per_gather_parsed,
+            "maximum_time": self.maximum_time_parsed,
+            "traces_to_inverse": self.traces_to_inverse_parsed,
+            "gain": self.gain_parsed,
+            "clip": self.clip_parsed,
+        }
+        data = {
+            "trace": list(range(1, len(picks_in_samples) + 1)),
+            "picks_in_samples": picks_in_samples,
+            "picks_in_ms": picks_in_ms,
+            "confidence": confidence,
+        }
+        return meta, data
 
-            meta = {
-                "is_source_file": is_source_file,
-                "is_source_ndarray": self.sgy.is_source_ndarray,
-                "filename": source_filename,
-                "full_name": source_full_name,
-                "hash": self.sgy.get_hash(),
-                "dt_ms": self.sgy.dt_ms,
-                "is_picked_with_model": bool(self.success),
-                "model_hash": self.model_hash,
-                "traces_per_gather": self.traces_per_gather_parsed,
-                "maximum_time": self.maximum_time_parsed,
-                "traces_to_inverse": self.traces_to_inverse_parsed,
-                "gain": self.gain_parsed,
-                "clip": self.clip_parsed,
-            }
-            data = {
-                "trace": list(range(1, len(picks_in_samples) + 1)),
-                "picks_in_samples": picks_in_samples,
-                "picks_in_ms": picks_in_ms,
-                "confidence": confidence,
-            }
-
-            Path(filename).parent.mkdir(parents=True, exist_ok=True)
-
-            with open(filename, "w") as fout:
-                if as_plain:
-                    content = [f"{k}={v}" for k, v in meta.items()]
-                    data_str = pd.DataFrame(data).to_string(index=False, justify="right")
-                    content.append(data_str)
-                    content = "\n".join(content)
-                    fout.write(content)
-                else:
-                    json.dump({**meta, **data}, fout)
+    def export_result_as_sgy(
+        self,
+        filename: Union[str, Path],
+        byte_position: int = 236,
+        encoding: str = "I",
+        picks_unit: str = "mcs",
+    ) -> None:
+        picks_in_samples = self._check_and_convert_picks()
+        self.sgy.export_sgy_with_picks(
+            output_fname=filename,
+            picks_in_samples=picks_in_samples,
+            encoding=encoding,
+            byte_position=byte_position,
+            picks_unit=picks_unit,
+        )
+
+    def export_result_as_json(self, filename: Union[str, Path]) -> None:
+        meta, data = self._prepare_output_for_nonbinary_export()
+        Path(filename).parent.mkdir(parents=True, exist_ok=True)
+        with open(filename, "w") as fout:
+            json.dump({**meta, **data}, fout)
+
+    def export_result_as_txt(self, filename: Union[str, Path]) -> None:
+        meta, data = self._prepare_output_for_nonbinary_export()
+        Path(filename).parent.mkdir(parents=True, exist_ok=True)
+        with open(filename, "w") as fout:
+            content = [f"{k}={v}" for k, v in meta.items()]
+            data_str = pd.DataFrame(data).to_string(index=False, justify="right")
+            content.append(data_str)
+            content = "\n".join(content)
+            fout.write(content)
```

### Comparing `first-breaks-picking-0.2.0/first_breaks/sgy/headers.py` & `first-breaks-picking-0.3.0b0/first_breaks/sgy/headers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, List, Tuple
+from typing import Dict, List, Tuple
 
 
 class InvalidHeaders(Exception):
     pass
 
 
 THeadersAttr = List[Tuple[int, str, str]]
@@ -61,17 +61,14 @@
                 upd_headers.append(upd_header)
                 offset += self.get_num_bytes(header[2])
             return upd_headers
         elif any(offsets_is_none) and not all(offsets_is_none):
             raise InvalidHeaders("To fill offsets, they must all be either empty or filled (no modification)")
         return self.headers_schema
 
-    def get_template(self, *args: Any, **kwargs: Any) -> Any:
-        raise NotImplementedError
-
 
 class FileHeaders(Headers):
     dt_name = "dt"
     dt_name_orig = "dt_orig"
     ns_name = "ns"
     ns_name_orig = "ns_orig"
     data_sample_format_name = "data_sample_format"
@@ -209,7 +206,39 @@
             (224, "source_measurement_mantissa", "i"),
             (228, "source_measurement_exponent", "H"),
             (230, "source_measurement_unit", "h"),
             (232, "unassigned1", "i"),
             (236, self.fb_pick_default, "I"),
         ]
         self.validate()
+        self.scalar_from2apply = {
+            "elevation_scalar": [
+                "REC_ELEV",
+                "SOU_ELEV",
+                "DEPTH",
+                "REC_DATUM",
+                "SOU_DATUM",
+                "SOU_H2OD",
+                "REC_H2OD",
+            ],
+            "source_group_scalar": [
+                "SOU_X",
+                "SOU_Y",
+                "REC_X",
+                "REC_Y",
+            ],
+            "shot_point_scalar": [
+                "shot_point",
+            ],
+            "scalar_trace_header": [
+                "UPHOLE",
+                "REC_UPHOLE",
+                "SOU_STAT",
+                "REC_STAT",
+                "TOT_STAT",
+                "lag_time_a",
+                "lag_time_b",
+                "delay_recording_time",
+                "TLIVE_S",
+                "TFULL_S",
+            ],
+        }
```

### Comparing `first-breaks-picking-0.2.0/first_breaks/sgy/reader.py` & `first-breaks-picking-0.3.0b0/first_breaks/sgy/reader.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,21 +6,15 @@
 from pathlib import Path
 from typing import Any, Dict, Generator, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
 
 from first_breaks.sgy.headers import FileHeaders, TraceHeaders
-from first_breaks.utils.utils import (
-    calc_hash,
-    chunk_iterable,
-    get_io,
-    ms2index,
-    multiply_iterable_by,
-)
+from first_breaks.utils.utils import UnitsConverter, calc_hash, chunk_iterable, get_io
 
 SizeHW = Tuple[int, int]
 
 
 class NotImplementedReader(Exception):
     pass
 
@@ -76,15 +70,15 @@
         return self.ntr
 
     @property
     def shape(self) -> SizeHW:
         return self.ns, self.ntr
 
     def ms2index(self, ms_value: float) -> int:
-        return ms2index(ms_value, self.dt_ms)
+        return self.units_converter.ms2index(ms_value)  # type: ignore
 
     @property
     def max_time_ms(self) -> float:
         return self.num_samples * self.dt_ms
 
     def __init__(
         self,
@@ -104,23 +98,25 @@
 
         # headers for file
         self.general_headers: Optional[Dict[str, Any]] = None
         self._general_headers_schema: FileHeaders = general_headers_schema
 
         # headers for traces
         self.traces_headers: Optional[pd.DataFrame] = None
+        self._traces_headers_raw: Optional[pd.DataFrame] = None
         self._traces_headers_schema: TraceHeaders = traces_headers_schema
 
         # other
         self._descriptor: Optional[Union[io.BytesIO, io.FileIO]] = None
         self.is_source_ndarray: Optional[bool] = None
         self._endianess: Optional[str] = None
         self._bps: Optional[int] = None
         self._data_fmt: Optional[int] = None
         self._hash_value: Optional[str] = None
+        self.units_converter: Optional[UnitsConverter] = None
 
         self.__init()
 
     def get_hash(self) -> Optional[str]:
         if self.is_source_ndarray:
             return None
         else:
@@ -140,14 +136,15 @@
         elif isinstance(self.source, np.ndarray):
             if self._dt_mcs_input is None:
                 raise SGYInitParamsError("Argument 'dt_mcs' is required if nd.array is used as input")
             self._init_from_numpy()
             self.is_source_ndarray = True
         else:
             raise SGYInitParamsError("Only `str, Path, bytes, np.ndarray` types are available as input")
+        self.units_converter = UnitsConverter(sgy_mcs=self.dt_mcs)
 
     def _init_from_numpy(self) -> None:
         assert self.source.ndim == 1 or self.source.ndim == 2, "Only arrays are available"  # type: ignore
         if self.source.ndim == 1:  # type: ignore
             self._ntr = 1
         elif self.source.ndim == 2:  # type: ignore
             self._ntr = self.source.shape[1]  # type: ignore
@@ -159,14 +156,15 @@
         self._ns = self.source.shape[0]  # type: ignore
 
     def _init_from_external(self) -> None:
         self._descriptor = get_io(self.source, mode="rb")
         self._read_endianess()
         self._read_general_headers()
         self._read_traces_headers()
+        self._scalar_raw_traces_headers()
         self._descriptor.close()
         self._descriptor = None
 
     def _read_endianess(self) -> None:
         num_bytes = self._descriptor.seek(0, 2)
         if num_bytes < 3600 + 240 + 1:  # at least general headers, 1 trace headers block and byte for 1 sample
             raise InvalidSGY("Invalid structure of SGY file. File is small")
@@ -208,24 +206,43 @@
         if num_bytes != (3600 + (240 + self._ns * self._bps) * self._ntr):
             raise InvalidSGY("Invalid number of bytes")
 
     def _read_traces_headers(self) -> None:
         traces_headers = {}
 
         for offset, name, fmt in self._traces_headers_schema.headers_schema:
-            size = self._traces_headers_schema.get_num_bytes(fmt)
-            buffer = []
-            for idx in range(self._ntr):
-                pointer = 3600 + (240 + self._ns * self._bps) * idx + offset
-                self._descriptor.seek(pointer)
-                buffer.append(self._descriptor.read(size))
+            header = self._read_custom_trace_header_with_existed_descriptor(offset, fmt)
+            traces_headers[name] = header
 
-            traces_headers[name] = struct.unpack(f"{self._endianess}{fmt * self._ntr}", b"".join(buffer))
+        self._traces_headers_raw = pd.DataFrame(data=traces_headers)
 
-        self.traces_headers = pd.DataFrame(data=traces_headers)
+    def _scalar_raw_traces_headers(self) -> None:
+        self.traces_headers = self._traces_headers_raw.copy()
+        for scalar_from, apply_to_columns in self._traces_headers_schema.scalar_from2apply.items():
+            scalar = self._traces_headers_raw[scalar_from].copy()
+
+            scalar[scalar == 0] = 1
+            scalar[scalar < 0] = 1 / abs(scalar[scalar < 0])
+            self.traces_headers[apply_to_columns] = self.traces_headers[apply_to_columns].apply(lambda x: scalar * x)
+
+    def _read_custom_trace_header_with_existed_descriptor(self, byte_position: int, encoding: str) -> Tuple[Any, ...]:
+        size = self._traces_headers_schema.get_num_bytes(encoding)
+        buffer = []
+        for idx in range(self._ntr):
+            pointer = 3600 + (240 + self._ns * self._bps) * idx + byte_position
+            self._descriptor.seek(pointer)
+            buffer.append(self._descriptor.read(size))
+        return struct.unpack(f"{self._endianess}{encoding * self._ntr}", b"".join(buffer))
+
+    def read_custom_trace_header(self, byte_position: int, encoding: str) -> Tuple[Any, ...]:
+        self._descriptor = get_io(self.source, mode="rb")
+        result = self._read_custom_trace_header_with_existed_descriptor(byte_position, encoding)
+        self._descriptor.close()
+        self._descriptor = None
+        return result
 
     def replace_traces(self, traces: np.ndarray) -> None:
         if traces.shape == self.shape:
             self._traces = traces
 
     def read(self, min_sample: Optional[int] = None, max_sample: Optional[int] = None) -> np.ndarray:
         ids = list(range(self.num_traces))
@@ -347,38 +364,53 @@
     def _read_traces_float(self, buffer: bytes, shape: SizeHW) -> np.ndarray:
         return np.ndarray(shape, f"{self._endianess}f4", buffer, order="F")
 
     def _read_traces_double(self, buffer: bytes, shape: SizeHW) -> np.ndarray:
         return np.ndarray(shape, f"{self._endianess}f8", buffer, order="F")
 
     def export_sgy_with_picks(
-        self, output_fname: Union[str, Path], picks_in_samples: List[int], byte_to_write: int = 236
+        self,
+        output_fname: Union[str, Path],
+        picks_in_samples: List[float],
+        byte_position: int = 236,
+        encoding: Optional[str] = None,
+        picks_unit: Optional[str] = "mcs",
     ) -> None:
         assert not self.is_source_ndarray, "Only true SGY can be used for importing picks"
-        assert 0 <= byte_to_write <= 236, "Only 0-236 bytes can be ised for writing"
+        assert 0 <= byte_position <= 236, "Only 0-236 bytes can be ised for writing"
         assert len(picks_in_samples) == self.num_traces, "Number of traces and picks differs"
+        assert picks_unit in ["ms", "mcs", "sample"]
 
         Path(output_fname).parent.mkdir(exist_ok=True, parents=True)
 
         if isinstance(self.source, (str, Path)):
-            shutil.copyfile(str(self.source), str(output_fname))
+            if Path(self.source).resolve() != Path(output_fname).resolve():
+                shutil.copyfile(str(self.source), str(output_fname))
         elif isinstance(self.source, bytes):
             with open(output_fname, "wb+") as f_output:
                 f_output.write(self.source)
         else:
             raise TypeError("Invalid type of source data")
 
-        picks_in_mcs = multiply_iterable_by(picks_in_samples, self.dt_mcs, cast_to=int)
-
-        pack_type = [
-            pack_type
-            for _, header, pack_type in self._traces_headers_schema.headers_schema
-            if header == self._traces_headers_schema.fb_pick_default
-        ][0]
+        if encoding is None:
+            encoding = [
+                pack_type
+                for _, header, pack_type in self._traces_headers_schema.headers_schema
+                if header == self._traces_headers_schema.fb_pick_default
+            ][0]
+
+        cast_to = float if encoding in ["f", "d"] else int
+
+        if picks_unit == "ms":
+            picks = self.units_converter.index2ms(picks_in_samples, cast_to=cast_to)
+        elif picks_unit == "mcs":
+            picks = self.units_converter.index2mcs(picks_in_samples, cast_to=cast_to)
+        else:
+            picks = picks_in_samples
 
         self._descriptor = get_io(output_fname, mode="r+b")
-        for idx, pick in enumerate(picks_in_mcs):  # type: ignore
-            pointer = 3600 + (240 + self.num_samples * self._bps) * idx + byte_to_write
-            pick_byte = struct.pack(f"{self._endianess}{pack_type}", int(pick))
+        for idx, pick in enumerate(picks):  # type: ignore
+            pointer = 3600 + (240 + self.num_samples * self._bps) * idx + byte_position
+            pick_byte = struct.pack(f"{self._endianess}{encoding}", pick)
             self._descriptor.seek(pointer)
             self._descriptor.write(pick_byte)
         self._descriptor.close()
```

### Comparing `first-breaks-picking-0.2.0/first_breaks/utils/debug.py` & `first-breaks-picking-0.3.0b0/first_breaks/utils/debug.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.2.0/first_breaks/utils/utils.py` & `first-breaks-picking-0.3.0b0/first_breaks/utils/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import hashlib
 import inspect
 import io
 from itertools import islice
 from pathlib import Path
-from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
+from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
 import numpy as np
 import onnxruntime as ort
 import requests
 
 from first_breaks.const import (
     DEMO_SGY_HASH,
@@ -87,33 +87,68 @@
 
 def download_model_onnx(
     fname: Union[str, Path] = MODEL_ONNX_PATH, url: str = MODEL_ONNX_URL, md5: str = MODEL_ONNX_HASH
 ) -> Union[str, Path]:
     return download_and_validate_file(fname=fname, url=url, md5=md5)
 
 
-def multiply_iterable_by(
-    sample: TTimeType, multiplier: float, cast_to: Optional[Callable[[Any], Any]] = None
-) -> TTimeType:
+def multiply_iterable_by(sample: TTimeType, multiplier: float, cast_to: Optional[Any] = None) -> TTimeType:
     if isinstance(sample, (int, float, str)):
         result = sample * multiplier  # type: ignore
-        return cast_to(result) if cast_to else result
+        return cast_to(result) if cast_to is not None else result
     elif isinstance(sample, (np.number, np.ndarray)):
         result = sample * multiplier
-        return result.astype(cast_to) if cast_to else result
+        return result.astype(cast_to) if cast_to is not None else result
     elif isinstance(sample, list):
         return list(multiply_iterable_by(val, multiplier, cast_to) for val in sample)
     elif isinstance(sample, tuple):
         return tuple(multiply_iterable_by(val, multiplier, cast_to) for val in sample)
     else:
         raise TypeError("Invalid type for samples")
 
 
-def ms2index(ms: float, sgy_ms: float) -> int:
-    return int(ms / sgy_ms)
+class UnitsConverter:
+    def __init__(
+        self,
+        *args: Any,
+        sgy_mcs: Optional[Union[int, float]] = None,
+        sgy_ms: Optional[Union[int, float]] = None,
+    ):
+        if args:
+            raise ValueError("Specify explicitly either `sgy_mcs`or `sgy_ms` as keyword argument")
+        if (sgy_mcs is None and sgy_ms is None) or (sgy_mcs is not None and sgy_ms is not None):
+            raise RuntimeError("One and only one of `sgy_mcs` or `sgy_ms` must be specified")
+        elif sgy_mcs is not None:
+            self.sgy_mcs = sgy_mcs
+            self.sgy_ms = self.mcs2ms(sgy_mcs)  # type: ignore
+        elif sgy_ms is not None:
+            self.sgy_mcs = self.ms2mcs(sgy_ms)  # type: ignore
+            self.sgy_ms = sgy_ms
+        else:
+            raise RuntimeError("Init error")
+
+    @staticmethod
+    def ms2mcs(sample: TTimeType, cast_to: Any = int) -> TTimeType:
+        return multiply_iterable_by(sample, 1000, cast_to)
+
+    @staticmethod
+    def mcs2ms(sample: TTimeType, cast_to: Any = float) -> TTimeType:
+        return multiply_iterable_by(sample, 0.001, cast_to)
+
+    def ms2index(self, sample: TTimeType, cast_to: Any = int) -> TTimeType:
+        return multiply_iterable_by(sample, 1 / self.sgy_ms, cast_to)  # type: ignore
+
+    def mcs2index(self, sample: TTimeType, cast_to: Any = int) -> TTimeType:
+        return multiply_iterable_by(sample, 1 / self.sgy_mcs, cast_to)
+
+    def index2ms(self, sample: TTimeType, cast_to: Any = float) -> TTimeType:
+        return multiply_iterable_by(sample, self.sgy_ms, cast_to)  # type: ignore
+
+    def index2mcs(self, sample: TTimeType, cast_to: Any = int) -> TTimeType:
+        return multiply_iterable_by(sample, self.sgy_mcs, cast_to)
 
 
 def remove_unused_kwargs(kwargs: Dict[str, Any], constructor: Any) -> Dict[str, Any]:
     return {k: v for k, v in kwargs.items() if k in inspect.signature(constructor).parameters}
 
 
 ONNX_DEVICE2PROVIDER = {"cuda": "CUDAExecutionProvider", "cpu": "CPUExecutionProvider"}
```

### Comparing `first-breaks-picking-0.2.0/first_breaks/utils/visualizations.py` & `first-breaks-picking-0.3.0b0/first_breaks/utils/visualizations.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.2.0/first_breaks_picking.egg-info/PKG-INFO` & `first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: first-breaks-picking
-Version: 0.2.0
+Version: 0.3.0b0
 Summary: Tool for picking first breaks in seismic gather
 Home-page: https://github.com/DaloroAT/first_breaks_picking
 Author: Aleksei Tarasov
 Author-email: aleksei.v.tarasov@gmail.com
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/DaloroAT/first_breaks_picking
 Keywords: seismic,first-breaks,computer-vision,deep-learning,segmentation,data-science
@@ -17,15 +17,15 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8,<3.9
 Description-Content-Type: text/markdown
 Provides-Extra: gpu
 License-File: LICENSE
 
 # First breaks picking
 This project is devoted to pick waves that are the first to be detected on a seismogram (first breaks, first arrivals).
 Traditionally, this procedure is performed manually. When processing field data, the number of picks reaches hundreds of
@@ -372,19 +372,22 @@
 
 # you can see results of picking
 print(task.picks_in_samples)
 print(task.picks_in_ms)
 print(task.confidence)
 
 # you can export picks to file as plain text
-task.export_result('result.txt', as_plain=True)
+task.export_result_as_txt('result.txt')
 # or save as json file
-task.export_result('result.json', as_json=True)
+task.export_result_as_json('result.json')
 # or make a copy of source SGY and put picks to 236 byte
-task.export_result('result.segy', as_sgy=True)
+task.export_result_as_sgy('result.segy',
+                          byte_position=236,
+                          encoding='i',
+                          picks_unit='mcs')
 ```
 [code-block-end]:pick-fb
 
 ### Visualizations
 
 You can save the seismogram and picks as an image. We use Qt backend for visualizations. Here we describe some usage
 scenarios.
@@ -400,15 +403,15 @@
 from first_breaks.desktop.graph import export_image
 
 sgy_filename = 'data.sgy'
 image_filename = 'image.png'
 
 sgy = SGY(sgy_filename)
 export_image(sgy, image_filename,
-             normalize=False,
+             normalize=None,
              traces_window=(5, 10),
              time_window=(0, 200),
              height=300,
              width_per_trace=30)
 ```
 [code-block-end]:plot-sgy
 
@@ -475,15 +478,15 @@
             traces_per_gather=24,
             maximum_time=200)
 picker = PickerONNX()
 task = picker.process_task(task)
 
 export_image(task, image_filename,
              show_processing_region=False,
-             fill_black_left=False,
+             fill_black='right',
              width=1000)
 ```
 [code-block-end]:plot-sgy-real-picks
 
 ### *Limit processing region
 
 Unfortunately, processing of a part of a file is not currently supported natively. We will add this functionality soon!
@@ -565,24 +568,30 @@
 
 ### Processing grid
 
 Click on 4 button to toggle the display of the processing grid on or off. Horizontal line
 shows `Maximum time` and vertical lines are drawn at intervals equal to `Traces per gather`. The neural network
 processes blocks independently, as separate images.
 
+### Visual settings
+
+Click on 5 button to open window for visual settings. You can select gain, clip, normalization method,
+and trace values. In addition, you can also load a pick from a file, specifying how to read it.
+
 ### Save results
 
-Click on 5 button to save picks into file. Depending on file extension, results will be saved as `json`,
+Click on 6 button to save picks into file. Depending on file extension, results will be saved as `json`,
 as plain `txt`, or as `segy` file.
 
 For extensions `txt` and `json`, picking parameters and model confidence for each peak are additionally saved.
 
 When choosing an extension `segy`, the copy of original SGY file is saved with the values of the first breaks in the
-trace headers. They are stored in the last 4 bytes (236 byte if counting from 0) to be decoded as an unsigned integer.
-Values are in microseconds.
+trace headers. After selecting a file, you will be prompted to choose in which byte to save (counting starts from 1),
+in which units of measurement and how to encode.
+
 # Picking process
 
 Neural network process file as series of **images**. There is why **the traces should not be random**,
 since we are using information about adjacent traces.
 
 To obtain the first breaks we do the following steps:
 1) Read all traces in the file.
```

### Comparing `first-breaks-picking-0.2.0/first_breaks_picking.egg-info/SOURCES.txt` & `first-breaks-picking-0.3.0b0/first_breaks_picking.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -3,20 +3,29 @@
 setup.cfg
 setup.py
 first_breaks/__init__.py
 first_breaks/cli.py
 first_breaks/const.py
 first_breaks/_pytorch/models/__init__.py
 first_breaks/_pytorch/models/unet3plus.py
+first_breaks/data_models/__init__.py
+first_breaks/data_models/dependent.py
+first_breaks/data_models/independent.py
+first_breaks/data_models/initialised_defaults.py
 first_breaks/desktop/__init__.py
+first_breaks/desktop/byte_encode_unit_widget.py
+first_breaks/desktop/combobox_with_mapping.py
 first_breaks/desktop/graph.py
 first_breaks/desktop/main_gui.py
 first_breaks/desktop/picking_widget.py
+first_breaks/desktop/radioset_widget.py
+first_breaks/desktop/slider_with_values.py
 first_breaks/desktop/threads.py
 first_breaks/desktop/utils.py
+first_breaks/desktop/visualization_settings_widget.py
 first_breaks/picking/__init__.py
 first_breaks/picking/ipicker.py
 first_breaks/picking/picker_onnx.py
 first_breaks/picking/task.py
 first_breaks/picking/utils.py
 first_breaks/sgy/__init__.py
 first_breaks/sgy/headers.py
@@ -28,15 +37,15 @@
 first_breaks_picking.egg-info/PKG-INFO
 first_breaks_picking.egg-info/SOURCES.txt
 first_breaks_picking.egg-info/dependency_links.txt
 first_breaks_picking.egg-info/entry_points.txt
 first_breaks_picking.egg-info/requires.txt
 first_breaks_picking.egg-info/top_level.txt
 tests/test_demo_sgy.py
-tests/test_markdown_examples.py
+tests/test_readme_examples.py
 tests/test_desktop/__init__.py
 tests/test_desktop/test_graph.py
 tests/test_picking/__init__.py
 tests/test_picking/test_picker.py
 tests/test_picking/test_task.py
 tests/test_sgy/__init__.py
 tests/test_sgy/test_reader.py
```

### Comparing `first-breaks-picking-0.2.0/setup.py` & `first-breaks-picking-0.3.0b0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 basic_reqs = load_requirements("requirements/basic.txt")
 cpu_reqs = load_requirements("requirements/cpu.txt")
 gpu_extra_reqs = load_requirements("requirements/gpu.txt")
 
 
 setup(
     # technical things
-    version="0.2.0",
+    version="0.3.0b",
     packages=find_packages(exclude=['data', 'docs', 'legacy', 'first_breaks._pytorch', 'tests', "requirements"]),
-    python_requires=">=3.8,<4.0",
+    python_requires=">=3.8,<3.9",  # todo
     install_requires=basic_reqs + cpu_reqs,
     extras_require={'gpu': gpu_extra_reqs},
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     entry_points={
             "console_scripts": [
                 "first-breaks-picking=first_breaks.cli:cli_commands"
```

### Comparing `first-breaks-picking-0.2.0/tests/test_markdown_examples.py` & `first-breaks-picking-0.3.0b0/tests/test_readme_examples.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import shutil
-import subprocess
 from pathlib import Path
 
 import pytest
 
 from first_breaks.const import PROJECT_ROOT
 
 
@@ -13,36 +12,34 @@
         text = f.readlines()
 
     i = text.index(start_indicator) + 2
     j = text.index(end_indicator) - 1
 
     code_block = "".join(text[i:j])
 
-    # print(code_block)
-
     return code_block
 
 
 @pytest.mark.parametrize(
     "block_name",
     [
-        # "e2e-example",
+        "e2e-example",
         # "downloading-extra",
-        # "init-from-path",
-        # "init-from-bytes",
-        # "init-from-np",
-        # "init-from-np",
-        # "sgy-content",
-        # "create-task",
-        # "create-picker",
-        # "pick-fb",
+        "init-from-path",
+        "init-from-bytes",
+        "init-from-np",
+        "init-from-np",
+        "sgy-content",
+        "create-task",
+        "create-picker",
+        "pick-fb",
         "plot-sgy",
         "plot-np",
         "plot-sgy-custom-picks",
-        # "plot-sgy-real-picks"
+        "plot-sgy-real-picks"
     ],
 )
 def test_code_blocks_in_readme(block_name: str,
                                demo_sgy: Path,
                                logs_dir_for_tests: Path) -> None:
     os.chdir(str(logs_dir_for_tests))
     shutil.copyfile(str(demo_sgy), str(logs_dir_for_tests / 'data.sgy'))
@@ -54,10 +51,10 @@
 
     tmp_fname = "tmp.py"
 
     with open(tmp_fname, "w") as f:
         f.write(code)
 
     try:
-        subprocess.run(f"python {tmp_fname}", check=True, shell=True)
+        os.system(f"python {tmp_fname}")
     finally:
         Path(tmp_fname).unlink()
```

### Comparing `first-breaks-picking-0.2.0/tests/test_picking/test_picker.py` & `first-breaks-picking-0.3.0b0/tests/test_picking/test_picker.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.2.0/tests/test_picking/test_task.py` & `first-breaks-picking-0.3.0b0/tests/test_picking/test_task.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.2.0/tests/test_sgy/test_reader.py` & `first-breaks-picking-0.3.0b0/tests/test_sgy/test_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,15 +46,7 @@
     sgy_with_picks_path = logs_dir_for_tests / 'sgy_with_picks.sgy'
     sgy.export_sgy_with_picks(sgy_with_picks_path, picks_in_samples)
     sgy_with_picks = SGY(sgy_with_picks_path)
 
     picks_in_mcs = multiply_iterable_by(picks_in_samples, sgy.dt_mcs, cast_to=int)
 
     assert np.all(picks_in_mcs == sgy_with_picks.traces_headers[picks_col_name])
-
-
-
-
-
-
-
-
```

