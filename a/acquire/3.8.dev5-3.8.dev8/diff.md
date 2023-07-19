# Comparing `tmp/acquire-3.8.dev5.tar.gz` & `tmp/acquire-3.8.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acquire-3.8.dev5.tar", last modified: Tue Jul 18 12:05:03 2023, max compression
+gzip compressed data, was "acquire-3.8.dev8.tar", last modified: Wed Jul 19 14:27:54 2023, max compression
```

## Comparing `acquire-3.8.dev5.tar` & `acquire-3.8.dev8.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:05:03.582886 acquire-3.8.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-18 12:04:49.000000 acquire-3.8.dev5/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-18 12:04:49.000000 acquire-3.8.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-18 12:04:49.000000 acquire-3.8.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-18 12:05:03.582886 acquire-3.8.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-18 12:04:49.000000 acquire-3.8.dev5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:05:03.566886 acquire-3.8.dev5/acquire/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79082 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/acquire.py
--rw-r--r--   0 runner    (1001) docker     (123)    20937 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:05:03.566886 acquire-3.8.dev5/acquire/dynamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/dynamic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:05:03.570886 acquire-3.8.dev5/acquire/dynamic/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/dynamic/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/dynamic/windows/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/dynamic/windows/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/dynamic/windows/handles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/dynamic/windows/named_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/dynamic/windows/ntdll.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/dynamic/windows/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/esxi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:05:03.574886 acquire-3.8.dev5/acquire/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/outputs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/outputs/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/outputs/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:05:03.574886 acquire-3.8.dev5/acquire/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15901 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/tools/decrypter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:05:03.574886 acquire-3.8.dev5/acquire/uploaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/uploaders/minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/uploaders/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/uploaders/plugin_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-07-18 12:04:49.000000 acquire-3.8.dev5/acquire/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-18 12:05:03.000000 acquire-3.8.dev5/acquire/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:05:03.566886 acquire-3.8.dev5/acquire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-18 12:05:03.000000 acquire-3.8.dev5/acquire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-18 12:05:03.000000 acquire-3.8.dev5/acquire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 12:05:03.000000 acquire-3.8.dev5/acquire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-18 12:05:03.000000 acquire-3.8.dev5/acquire.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-18 12:05:03.000000 acquire-3.8.dev5/acquire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 12:05:03.000000 acquire-3.8.dev5/acquire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-18 12:04:53.000000 acquire-3.8.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 12:05:03.582886 acquire-3.8.dev5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:05:03.578886 acquire-3.8.dev5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:04:49.000000 acquire-3.8.dev5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-18 12:04:49.000000 acquire-3.8.dev5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:05:03.582886 acquire-3.8.dev5/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-18 12:04:49.000000 acquire-3.8.dev5/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-18 12:04:49.000000 acquire-3.8.dev5/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-18 12:04:49.000000 acquire-3.8.dev5/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-18 12:04:49.000000 acquire-3.8.dev5/tests/test_acquire_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-18 12:04:49.000000 acquire-3.8.dev5/tests/test_acquire_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-07-18 12:04:49.000000 acquire-3.8.dev5/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-18 12:04:49.000000 acquire-3.8.dev5/tests/test_decryptor_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-18 12:04:49.000000 acquire-3.8.dev5/tests/test_esxi_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-18 12:04:49.000000 acquire-3.8.dev5/tests/test_file_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-18 12:04:49.000000 acquire-3.8.dev5/tests/test_minio_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-18 12:04:49.000000 acquire-3.8.dev5/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-07-18 12:04:49.000000 acquire-3.8.dev5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-18 12:04:49.000000 acquire-3.8.dev5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:54.183662 acquire-3.8.dev8/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-19 14:27:23.000000 acquire-3.8.dev8/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-19 14:27:23.000000 acquire-3.8.dev8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-19 14:27:23.000000 acquire-3.8.dev8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-19 14:27:54.183662 acquire-3.8.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-19 14:27:23.000000 acquire-3.8.dev8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:54.163662 acquire-3.8.dev8/acquire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79835 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/acquire.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21648 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:54.167662 acquire-3.8.dev8/acquire/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/dynamic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:54.167662 acquire-3.8.dev8/acquire/dynamic/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/dynamic/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/dynamic/windows/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/dynamic/windows/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/dynamic/windows/handles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/dynamic/windows/named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/dynamic/windows/ntdll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/dynamic/windows/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/esxi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:54.171662 acquire-3.8.dev8/acquire/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/outputs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/outputs/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/outputs/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:54.171662 acquire-3.8.dev8/acquire/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15901 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/tools/decrypter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:54.175662 acquire-3.8.dev8/acquire/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/uploaders/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/uploaders/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/uploaders/plugin_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-19 14:27:53.000000 acquire-3.8.dev8/acquire/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:54.163662 acquire-3.8.dev8/acquire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-19 14:27:54.000000 acquire-3.8.dev8/acquire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-19 14:27:54.000000 acquire-3.8.dev8/acquire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 14:27:54.000000 acquire-3.8.dev8/acquire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-19 14:27:54.000000 acquire-3.8.dev8/acquire.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-19 14:27:54.000000 acquire-3.8.dev8/acquire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-19 14:27:54.000000 acquire-3.8.dev8/acquire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-19 14:27:40.000000 acquire-3.8.dev8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 14:27:54.183662 acquire-3.8.dev8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:54.183662 acquire-3.8.dev8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:54.183662 acquire-3.8.dev8/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/test_acquire_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/test_acquire_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/test_decryptor_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/test_esxi_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/test_file_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/test_minio_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/test_misc_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tox.ini
```

### Comparing `acquire-3.8.dev5/LICENSE` & `acquire-3.8.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/PKG-INFO` & `acquire-3.8.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.8.dev5
+Version: 3.8.dev8
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `acquire-3.8.dev5/README.md` & `acquire-3.8.dev8/README.md`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/acquire/acquire.py` & `acquire-3.8.dev8/acquire/acquire.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import subprocess
 import sys
 import time
 import urllib.parse
 import urllib.request
 from collections import defaultdict
 from pathlib import Path
-from typing import Optional, Union
+from typing import Iterator, Optional, Union
 
 from dissect.target import Target, exceptions
 from dissect.target.filesystems import dir, ntfs
 from dissect.target.helpers import fsutil
 from dissect.target.loaders.remote import RemoteStreamConnection
 from dissect.target.loaders.targetd import TargetdLoader
 from dissect.target.plugins.apps.webservers import iis
@@ -91,15 +91,15 @@
 log = logging.getLogger("acquire")
 log.propagate = 0
 log_file_handler = None
 logging.lastResort = None
 logging.raiseExceptions = False
 
 
-def misc_windows_user_homes(target):
+def misc_windows_user_homes(target: Target) -> Iterator[fsutil.TargetPath]:
     misc_dirs = {
         ("windows/serviceprofiles/localservice", False),
         ("windows/serviceprofiles/networkservice", False),
         ("windows/system32/config/systemprofile", False),
         ("users", True),
         ("documents and settings", True),
     }
@@ -118,20 +118,45 @@
                 for entry in misc_path.iterdir():
                     if entry.is_dir():
                         yield entry
             else:
                 yield misc_path
 
 
-def from_user_home(target, path):
+def misc_unix_user_homes(target: Target) -> Iterator[fsutil.TargetPath]:
+    user_dirs = ["root", "home/*"]
+
+    home_dirs = (target.fs.path("/").glob(path) for path in user_dirs)
+    for home_dir in itertools.chain.from_iterable(home_dirs):
+        yield home_dir
+
+
+def misc_osx_user_homes(target: Target) -> Iterator[fsutil.TargetPath]:
+    for homedir in itertools.chain(target.fs.path("/Users/").glob("*"), misc_unix_user_homes(target)):
+        yield homedir
+
+
+MISC_MAPPING = {
+    "osx": misc_osx_user_homes,
+    "windows": misc_windows_user_homes,
+}
+
+
+def from_user_home(target: Target, path: str):
+    # Until getting the users from osx is implemented in dissect.target
+    if target.os == "osx":
+        for misc_dir in misc_osx_user_homes(target):
+            yield str(misc_dir.joinpath(path))
+        return
     for user_details in target.user_details.all_with_home():
         yield str(user_details.home_path.joinpath(path))
-    if target.os == "windows":
-        for misc_dir in misc_windows_user_homes(target):
-            yield str(misc_dir.joinpath(path))
+
+    misc_user_homes = MISC_MAPPING.get(target.os, misc_unix_user_homes)
+    for user_dir in misc_user_homes(target):
+        yield str(user_dir.joinpath(path))
 
 
 def iter_ntfs_filesystems(target):
     mount_lookup = defaultdict(list)
     for mount, fs in target.fs.mounts.items():
         mount_lookup[fs].append(mount)
 
@@ -226,30 +251,26 @@
 
 class Module:
     DESC = None
     SPEC = []
     EXEC_ORDER = ExecutionOrder.DEFAULT
 
     @classmethod
-    def run(cls, target, cli_args, collector):
+    def run(cls, target: Target, cli_args: argparse.Namespace, collector: Collector):
         desc = cls.DESC or cls.__name__.lower()
         log.info("*** Acquiring %s", desc)
 
-        collector.bind(cls)
-
-        try:
+        with collector.bind_module(cls):
             collector.collect(cls.SPEC)
 
             spec_ext = cls.get_spec_additions(target)
             if spec_ext:
                 collector.collect(list(spec_ext))
 
             cls._run(target, collector)
-        finally:
-            collector.unbind()
 
     @classmethod
     def get_spec_additions(cls, target):
         pass
 
     @classmethod
     def _run(cls, target, collector):
@@ -1078,41 +1099,41 @@
             from_user_home,
         ),
         (
             "glob",
             "Local Settings/Application Data/Google/Chrom*/User Data/*/Last Tabs",
             from_user_home,
         ),
-        ("glob", "/Users/*/Library/Application Support/Google/Chrome/*/Bookmarks"),
-        ("glob", "/Users/*/Library/Application Support/Google/Chrome/*/Favicons"),
-        ("glob", "/Users/*/Library/Application Support/Google/Chrome/*/History"),
-        ("glob", "/Users/*/Library/Application Support/Google/Chrome/*/Login Data"),
-        ("glob", "/Users/*/Library/Application Support/Google/Chrome/*/Login Data For Account"),
-        ("glob", "/Users/*/Library/Application Support/Google/Chrome/*/Shortcuts"),
-        ("glob", "/Users/*/Library/Application Support/Google/Chrome/*/Top Sites"),
-        ("glob", "/Users/*/Library/Application Support/Google/Chrome/*/Web Data"),
-        ("glob", "/Users/*/Library/Application Support/Chromium/*/Bookmarks"),
-        ("glob", "/Users/*/Library/Application Support/Chromium/*/Favicons"),
-        ("glob", "/Users/*/Library/Application Support/Chromium/*/History"),
-        ("glob", "/Users/*/Library/Application Support/Chromium/*/Login Data"),
-        ("glob", "/Users/*/Library/Application Support/Chromium/*/Login Data For Account"),
-        ("glob", "/Users/*/Library/Application Support/Chromium/*/Shortcuts"),
-        ("glob", "/Users/*/Library/Application Support/Chromium/*/Top Sites"),
-        ("glob", "/Users/*/Library/Application Support/Chromium/*/Web Data"),
+        ("glob", "Library/Application Support/Google/Chrome/*/Bookmarks", from_user_home),
+        ("glob", "Library/Application Support/Google/Chrome/*/Favicons", from_user_home),
+        ("glob", "Library/Application Support/Google/Chrome/*/History", from_user_home),
+        ("glob", "Library/Application Support/Google/Chrome/*/Login Data", from_user_home),
+        ("glob", "Library/Application Support/Google/Chrome/*/Login Data For Account", from_user_home),
+        ("glob", "Library/Application Support/Google/Chrome/*/Shortcuts", from_user_home),
+        ("glob", "Library/Application Support/Google/Chrome/*/Top Sites", from_user_home),
+        ("glob", "Library/Application Support/Google/Chrome/*/Web Data", from_user_home),
+        ("glob", "Library/Application Support/Chromium/*/Bookmarks", from_user_home),
+        ("glob", "Library/Application Support/Chromium/*/Favicons", from_user_home),
+        ("glob", "Library/Application Support/Chromium/*/History", from_user_home),
+        ("glob", "Library/Application Support/Chromium/*/Login Data", from_user_home),
+        ("glob", "Library/Application Support/Chromium/*/Login Data For Account", from_user_home),
+        ("glob", "Library/Application Support/Chromium/*/Shortcuts", from_user_home),
+        ("glob", "Library/Application Support/Chromium/*/Top Sites", from_user_home),
+        ("glob", "Library/Application Support/Chromium/*/Web Data", from_user_home),
         # Chrome - Legacy
-        ("glob", "/Users/*/Library/Application Support/Google/Chrome/*/Current Session"),
-        ("glob", "/Users/*/Library/Application Support/Google/Chrome/*/Current Tabs"),
-        ("glob", "/Users/*/Library/Application Support/Google/Chrome/*/Archived History"),
-        ("glob", "/Users/*/Library/Application Support/Google/Chrome/*/Last Session"),
-        ("glob", "/Users/*/Library/Application Support/Google/Chrome/*/Last Tabs"),
-        ("glob", "/Users/*/Library/Application Support/Chromium/*/Current Session"),
-        ("glob", "/Users/*/Library/Application Support/Chromium/*/Current Tabs"),
-        ("glob", "/Users/*/Library/Application Support/Chromium/*/Archived History"),
-        ("glob", "/Users/*/Library/Application Support/Chromium/*/Last Session"),
-        ("glob", "/Users/*/Library/Application Support/Chromium/*/Last Tabs"),
+        ("glob", "Library/Application Support/Google/Chrome/*/Current Session", from_user_home),
+        ("glob", "Library/Application Support/Google/Chrome/*/Current Tabs", from_user_home),
+        ("glob", "Library/Application Support/Google/Chrome/*/Archived History", from_user_home),
+        ("glob", "Library/Application Support/Google/Chrome/*/Last Session", from_user_home),
+        ("glob", "Library/Application Support/Google/Chrome/*/Last Tabs", from_user_home),
+        ("glob", "Library/Application Support/Chromium/*/Current Session", from_user_home),
+        ("glob", "Library/Application Support/Chromium/*/Current Tabs", from_user_home),
+        ("glob", "Library/Application Support/Chromium/*/Archived History", from_user_home),
+        ("glob", "Library/Application Support/Chromium/*/Last Session", from_user_home),
+        ("glob", "Library/Application Support/Chromium/*/Last Tabs", from_user_home),
         # Chrome - RHEL/Ubuntu - DNF
         ("glob", ".config/google-chrome/*/Bookmarks", from_user_home),
         ("glob", ".config/google-chrome/*/Favicons", from_user_home),
         ("glob", ".config/google-chrome/*/History", from_user_home),
         ("glob", ".config/google-chrome/*/Login Data", from_user_home),
         ("glob", ".config/google-chrome/*/Login Data For Account", from_user_home),
         ("glob", ".config/google-chrome/*/Shortcuts", from_user_home),
@@ -1205,23 +1226,23 @@
             from_user_home,
         ),
         (
             "glob",
             "Local Settings/Application Data/Microsoft/Edge/User Data/*/Web Data",
             from_user_home,
         ),
-        ("glob", "/Users/*/Library/Application Support/Microsoft Edge/*/Bookmarks"),
-        ("glob", "/Users/*/Library/Application Support/Microsoft Edge/*/Extension Cookies"),
-        ("glob", "/Users/*/Library/Application Support/Microsoft Edge/*/Favicons"),
-        ("glob", "/Users/*/Library/Application Support/Microsoft Edge/*/History"),
-        ("glob", "/Users/*/Library/Application Support/Microsoft Edge/*/Login Data"),
-        ("glob", "/Users/*/Library/Application Support/Microsoft Edge/*/Media History"),
-        ("glob", "/Users/*/Library/Application Support/Microsoft Edge/*/Shortcuts"),
-        ("glob", "/Users/*/Library/Application Support/Microsoft Edge/*/Top Sites"),
-        ("glob", "/Users/*/Library/Application Support/Microsoft Edge/*/Web Data"),
+        ("glob", "Library/Application Support/Microsoft Edge/*/Bookmarks", from_user_home),
+        ("glob", "Library/Application Support/Microsoft Edge/*/Extension Cookies", from_user_home),
+        ("glob", "Library/Application Support/Microsoft Edge/*/Favicons", from_user_home),
+        ("glob", "Library/Application Support/Microsoft Edge/*/History", from_user_home),
+        ("glob", "Library/Application Support/Microsoft Edge/*/Login Data", from_user_home),
+        ("glob", "Library/Application Support/Microsoft Edge/*/Media History", from_user_home),
+        ("glob", "Library/Application Support/Microsoft Edge/*/Shortcuts", from_user_home),
+        ("glob", "Library/Application Support/Microsoft Edge/*/Top Sites", from_user_home),
+        ("glob", "Library/Application Support/Microsoft Edge/*/Web Data", from_user_home),
         # Edge - RHEL/Ubuntu - DNF/apt
         ("glob", ".config/microsoft-edge/*/Bookmarks", from_user_home),
         ("glob", ".config/microsoft-edge/*/Favicons", from_user_home),
         ("glob", ".config/microsoft-edge/*/History", from_user_home),
         ("glob", ".config/microsoft-edge/*/Login Data", from_user_home),
         ("glob", ".config/microsoft-edge/*/Login Data For Account", from_user_home),
         ("glob", ".config/microsoft-edge/*/Shortcuts", from_user_home),
@@ -1245,20 +1266,20 @@
         # Firefox - RHEL/Ubuntu - Flatpak
         ("glob", ".var/app/org.mozilla.firefox/.mozilla/firefox/*/*.sqlite", from_user_home),
         # Firefox - RHEL/Ubuntu - DNF/apt
         ("glob", ".mozilla/firefox/*/*.sqlite", from_user_home),
         # Firefox - RHEL/Ubuntu - snap
         ("glob", "snap/firefox/common/.mozilla/firefox/*/*.sqlite", from_user_home),
         # Safari - macOS
-        ("glob", "/Users/*/Library/Safari/Bookmarks.plist"),
-        ("glob", "/Users/*/Library/Safari/Downloads.plist"),
-        ("glob", "/Users/*/Library/Safari/Extensions/Extensions.plist"),
-        ("glob", "/Users/*/Library/Safari/History.*"),
-        ("glob", "/Users/*/Library/Safari/LastSession.plist"),
-        ("glob", "/Users/*/Library/Caches/com.apple.Safari/Cache.db"),
+        ("file", "Library/Safari/Bookmarks.plist", from_user_home),
+        ("file", "Library/Safari/Downloads.plist", from_user_home),
+        ("file", "Library/Safari/Extensions/Extensions.plist", from_user_home),
+        ("glob", "Library/Safari/History.*", from_user_home),
+        ("file", "Library/Safari/LastSession.plist", from_user_home),
+        ("file", "Library/Caches/com.apple.Safari/Cache.db", from_user_home),
     ]
 
 
 @register_module("--remoteaccess")
 class RemoteAccess(Module):
     DESC = "common remote access tools' log files"
     SPEC = [
@@ -1333,63 +1354,55 @@
         ("glob", "/boot/config*"),
         ("glob", "/boot/efi*"),
         ("glob", "/boot/grub*"),
         ("glob", "/boot/init*"),
     ]
 
 
+def private_key_filter(path: fsutil.TargetPath) -> bool:
+    with path.open("rt") as file:
+        return "PRIVATE KEY" in file.readline()
+
+
 @register_module("--home")
 class Home(Module):
     SPEC = [
-        # TODO: Use from_user_home if supported for osx
-        ("glob", "/root/.*[akz]sh*"),
-        ("dir", "/root/.config"),
-        ("glob", "/home/*/.*[akz]sh*"),
-        ("glob", "/home/*/.config"),
-        ("glob", "/home/*/*/.*[akz]sh*"),
-        ("glob", "/home/*/*/.config"),
+        ("glob", ".*[akz]sh*", from_user_home),
+        ("dir", ".config", from_user_home),
+        ("glob", "*/.*[akz]sh*", from_user_home),
+        ("glob", "*/.config", from_user_home),
         # OS-X home (aka /Users)
-        ("glob", "/Users/*/.*[akz]sh*"),
-        ("glob", "/Users/*/.config"),
-        ("glob", "/Users/*/.bash_sessions/*"),
-        ("glob", "/Users/*/Library/LaunchAgents/*"),
-        ("glob", "/Users/*/Library/Logs/*"),
-        ("glob", "/Users/*/Preferences/*"),
-        ("glob", "/Users/*/Library/Preferences/*"),
+        ("glob", ".bash_sessions/*", from_user_home),
+        ("glob", "Library/LaunchAgents/*", from_user_home),
+        ("glob", "Library/Logs/*", from_user_home),
+        ("glob", "Preferences/*", from_user_home),
+        ("glob", "Library/Preferences/*", from_user_home),
     ]
 
 
 @register_module("--ssh")
+@module_arg("--private-keys", action="store_true", help="Add any private keys", default=False)
 class SSH(Module):
-    @classmethod
-    def _run(cls, target: Target, collector):
-        user_pattern = ".ssh/*"
-
-        # Gather user paths
-        # TODO: Use from_user_home if supported for osx
-        if target._os.os == "osx":
-            iterator = [f"/Users/*/{user_pattern}"]
-        else:
-            iterator = list(from_user_home(target, user_pattern))
+    SPEC = [
+        ("glob", ".ssh/*", from_user_home),
+        ("glob", "/etc/ssh/*"),
+        ("glob", "sysvol/ProgramData/ssh/*"),
+    ]
 
+    @classmethod
+    def run(cls, target: Target, cli_args: argparse.Namespace, collector: Collector):
         # Acquire SSH configuration in sshd directories
-        iterator += ["/etc/ssh/*", "sysvol/ProgramData/ssh/*"]
 
-        globbed_path = (path for pattern in iterator for path in target.fs.glob(pattern))
-        for path in globbed_path:
-            if target.fs.path(path).is_dir():
-                collector.collect_dir(path)
-                continue
+        filter = None if cli_args.private_keys else private_key_filter
 
-            with target.fs.path(path).open("rt") as file:
-                if "PRIVATE KEY" in file.readline():
-                    # Detected a private key, skipping.
-                    continue
+        if filter:
+            log.info("Executing SSH without --private-keys, skipping private keys.")
 
-            collector.collect_file(path, outpath=path)
+        with collector.file_filter(filter):
+            super().run(target, cli_args, collector)
 
 
 @register_module("--var")
 class Var(Module):
     SPEC = [
         # In OS-X /var is a symlink to /private/var. To prevent collecting
         # duplicates, we only use the /var directory here.
@@ -1560,28 +1573,25 @@
 
     @classmethod
     def run(cls, target, cli_args, collector):
         log.info("*** Acquiring file hashes")
 
         specs = cls.get_specs(cli_args)
 
-        collector.bind(cls)
-        try:
+        with collector.bind_module(cls):
             start = time.time()
 
             path_hashes = collect_hashes(target, specs, path_filters=cls.DEFAULT_FILE_FILTERS)
             rows_count, csv_compressed_bytes = serialize_into_csv(path_hashes, compress=True)
 
             collector.write_bytes(
                 f"{collector.base}/{collector.METADATA_BASE}/file-hashes.csv.gz",
                 csv_compressed_bytes,
             )
             log.info("Hashing is done, %s files processed in %.2f secs", rows_count, (time.time() - start))
-        finally:
-            collector.unbind()
 
     @classmethod
     def get_specs(cls, cli_args):
         path_selectors = []
 
         if cli_args.ext_to_hash:
             extensions = cli_args.ext_to_hash
@@ -1628,26 +1638,23 @@
         from acquire.dynamic.windows.collect import collect_open_handles
         from acquire.dynamic.windows.handles import serialize_handles_into_csv
 
         log.info("*** Acquiring open handles")
 
         handle_types = cli_args.handle_types
 
-        collector.bind(cls)
-        try:
+        with collector.bind_module(cls):
             handles = collect_open_handles(handle_types)
             csv_compressed_handles = serialize_handles_into_csv(handles)
 
             collector.write_bytes(
                 f"{collector.base}/{collector.METADATA_BASE}/open_handles.csv.gz",
                 csv_compressed_handles,
             )
             log.info("Collecting open handles is done.")
-        finally:
-            collector.unbind()
 
 
 def print_disks_overview(target):
     log.info("// Disks")
     try:
         for disk in target.disks:
             log.info("%s", disk)
```

### Comparing `acquire-3.8.dev5/acquire/collector.py` & `acquire-3.8.dev8/acquire/collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,28 @@
 
 import dataclasses
 import errno
 import logging
 import subprocess
 import textwrap
 from collections import defaultdict
+from contextlib import contextmanager
 from dataclasses import dataclass
 from itertools import groupby
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Iterable, Optional, Sequence, Type, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Iterable,
+    Optional,
+    Sequence,
+    Type,
+    Union,
+)
 
 from dissect.target import Target
 from dissect.target.exceptions import (
     FileNotFoundError,
     NotADirectoryError,
     NotASymlinkError,
     SymlinkRecursionError,
@@ -180,23 +190,41 @@
         self.target = target
         self.output = output
         self.base = base
         self.skip_list = skip_list or set()
 
         self.report = CollectionReport()
         self.bound_module_name = None
+        self.filter = lambda _: False
 
         self.output.init(self.target)
 
     def __enter__(self) -> Collector:
         return self
 
     def __exit__(self, *args, **kwargs) -> None:
         self.close()
 
+    @contextmanager
+    def bind_module(self, module: Type) -> Collector:
+        try:
+            self.bind(module)
+            yield self
+        finally:
+            self.unbind()
+
+    @contextmanager
+    def file_filter(self, filter: Optional[Callable[[fsutil.TargetPath], bool]]) -> Collector:
+        try:
+            if filter:
+                self.filter = filter
+            yield self
+        finally:
+            self.filter = lambda _: False
+
     def bind(self, module: Type) -> None:
         self.bound_module_name = module.__name__
 
     def unbind(self) -> None:
         self.bound_module_name = None
 
     def close(self) -> None:
@@ -259,14 +287,18 @@
         module_name = self.bound_module_name or module_name
         if not module_name:
             raise ValueError("Module name must be provided or Collector needs to be bound to a module")
 
         if not isinstance(path, fsutil.TargetPath):
             path = self.target.fs.path(path)
 
+        if self.filter(path) is True:
+            log.info("- Collecting file %s: Skipped (filtered out)", path)
+            return
+
         if self.report.was_path_seen(path):
             log.info("- Collecting file %s: Skipped (DEDUP)", path)
             return
 
         outpath = self._create_output_path(outpath or path, base)
         entry = path.get()
```

### Comparing `acquire-3.8.dev5/acquire/crypt.py` & `acquire-3.8.dev8/acquire/crypt.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/acquire/dynamic/windows/collect.py` & `acquire-3.8.dev8/acquire/dynamic/windows/collect.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/acquire/dynamic/windows/handles.py` & `acquire-3.8.dev8/acquire/dynamic/windows/handles.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/acquire/dynamic/windows/named_objects.py` & `acquire-3.8.dev8/acquire/dynamic/windows/named_objects.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/acquire/dynamic/windows/ntdll.py` & `acquire-3.8.dev8/acquire/dynamic/windows/ntdll.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/acquire/dynamic/windows/types.py` & `acquire-3.8.dev8/acquire/dynamic/windows/types.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/acquire/esxi.py` & `acquire-3.8.dev8/acquire/esxi.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/acquire/hashes.py` & `acquire-3.8.dev8/acquire/hashes.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/acquire/log.py` & `acquire-3.8.dev8/acquire/log.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/acquire/outputs/base.py` & `acquire-3.8.dev8/acquire/outputs/base.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/acquire/outputs/dir.py` & `acquire-3.8.dev8/acquire/outputs/dir.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/acquire/outputs/tar.py` & `acquire-3.8.dev8/acquire/outputs/tar.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/acquire/tools/decrypter.py` & `acquire-3.8.dev8/acquire/tools/decrypter.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/acquire/uploaders/minio.py` & `acquire-3.8.dev8/acquire/uploaders/minio.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/acquire/uploaders/plugin.py` & `acquire-3.8.dev8/acquire/uploaders/plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/acquire/uploaders/plugin_registry.py` & `acquire-3.8.dev8/acquire/uploaders/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/acquire/utils.py` & `acquire-3.8.dev8/acquire/utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/acquire.egg-info/PKG-INFO` & `acquire-3.8.dev8/acquire.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.8.dev5
+Version: 3.8.dev8
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `acquire-3.8.dev5/acquire.egg-info/SOURCES.txt` & `acquire-3.8.dev8/acquire.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -42,12 +42,13 @@
 tests/test_acquire_command.py
 tests/test_acquire_modules.py
 tests/test_collector.py
 tests/test_decryptor_funcs.py
 tests/test_esxi_memory.py
 tests/test_file_sorting.py
 tests/test_minio_uploader.py
+tests/test_misc_users.py
 tests/test_plugin.py
 tests/test_utils.py
 tests/docs/Makefile
 tests/docs/conf.py
 tests/docs/index.rst
```

### Comparing `acquire-3.8.dev5/pyproject.toml` & `acquire-3.8.dev8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/tests/conftest.py` & `acquire-3.8.dev8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/tests/docs/Makefile` & `acquire-3.8.dev8/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/tests/docs/conf.py` & `acquire-3.8.dev8/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/tests/test_acquire_command.py` & `acquire-3.8.dev8/tests/test_acquire_command.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/tests/test_acquire_modules.py` & `acquire-3.8.dev8/tests/test_acquire_modules.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/tests/test_collector.py` & `acquire-3.8.dev8/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/tests/test_decryptor_funcs.py` & `acquire-3.8.dev8/tests/test_decryptor_funcs.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/tests/test_esxi_memory.py` & `acquire-3.8.dev8/tests/test_esxi_memory.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/tests/test_file_sorting.py` & `acquire-3.8.dev8/tests/test_file_sorting.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/tests/test_minio_uploader.py` & `acquire-3.8.dev8/tests/test_minio_uploader.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/tests/test_plugin.py` & `acquire-3.8.dev8/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/tests/test_utils.py` & `acquire-3.8.dev8/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev5/tox.ini` & `acquire-3.8.dev8/tox.ini`

 * *Files identical despite different names*

