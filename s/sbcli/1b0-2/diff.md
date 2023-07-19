# Comparing `tmp/sbcli-1b0.tar.gz` & `tmp/sbcli-2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\HP\PycharmProjects\ultra_repo\ultra\api\dist\.tmp-exg_4h85\sbcli-1b0.tar", last modified: Wed Jul 19 14:32:40 2023, max compression
+gzip compressed data, was "C:\Users\HP\PycharmProjects\ultra_repo\ultra\api\dist\.tmp-1ff45xo3\sbcli-2.tar", last modified: Wed Jul 19 14:35:07 2023, max compression
```

## Comparing `sbcli-1b0.tar` & `sbcli-2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 14:32:40.152911 sbcli-1b0/
--rw-rw-rw-   0        0        0    43376 2023-07-19 14:32:40.151912 sbcli-1b0/PKG-INFO
--rw-rw-rw-   0        0        0    43124 2023-07-13 15:17:09.000000 sbcli-1b0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 14:32:40.077114 sbcli-1b0/management/
--rw-rw-rw-   0        0        0        0 2021-10-27 21:58:56.000000 sbcli-1b0/management/__init__.py
--rw-rw-rw-   0        0        0    51657 2023-07-19 14:29:48.000000 sbcli-1b0/management/cli.py
--rw-rw-rw-   0        0        0     6893 2023-07-11 13:47:18.000000 sbcli-1b0/management/cluster_ops.py
--rw-rw-rw-   0        0        0     5264 2023-03-06 15:46:56.000000 sbcli-1b0/management/compute_node_ops.py
--rw-rw-rw-   0        0        0      755 2023-07-06 18:09:38.000000 sbcli-1b0/management/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-19 14:32:40.087085 sbcli-1b0/management/controllers/
--rw-rw-rw-   0        0        0        0 2023-03-06 16:32:43.000000 sbcli-1b0/management/controllers/__init__.py
--rw-rw-rw-   0        0        0      955 2023-06-27 12:09:06.000000 sbcli-1b0/management/controllers/cluster_lifecycle.py
--rw-rw-rw-   0        0        0     8787 2023-06-27 12:04:07.000000 sbcli-1b0/management/controllers/device_lifecycle.py
--rw-rw-rw-   0        0        0    16507 2023-07-13 17:10:28.000000 sbcli-1b0/management/controllers/lvol_controller.py
--rw-rw-rw-   0        0        0    13889 2023-06-27 12:01:46.000000 sbcli-1b0/management/controllers/node_lifecycle.py
--rw-rw-rw-   0        0        0     9473 2023-06-29 12:54:01.000000 sbcli-1b0/management/controllers/pool_controller.py
--rw-rw-rw-   0        0        0     5773 2023-07-13 17:28:28.000000 sbcli-1b0/management/kv_store.py
--rw-rw-rw-   0        0        0     3578 2023-05-22 22:51:19.000000 sbcli-1b0/management/mgmt_node_ops.py
-drwxrwxrwx   0        0        0        0 2023-07-19 14:32:40.106035 sbcli-1b0/management/models/
--rw-rw-rw-   0        0        0        0 2021-10-28 14:11:47.000000 sbcli-1b0/management/models/__init__.py
--rw-rw-rw-   0        0        0     4681 2023-07-13 17:24:37.000000 sbcli-1b0/management/models/base_model.py
--rw-rw-rw-   0        0        0     1815 2023-07-11 12:10:41.000000 sbcli-1b0/management/models/cluster.py
--rw-rw-rw-   0        0        0      943 2023-02-08 22:16:26.000000 sbcli-1b0/management/models/compute_node.py
--rw-rw-rw-   0        0        0     3019 2023-07-13 18:37:17.000000 sbcli-1b0/management/models/device_stat.py
--rw-rw-rw-   0        0        0     1251 2023-05-09 17:37:12.000000 sbcli-1b0/management/models/global_settings.py
--rw-rw-rw-   0        0        0      830 2023-07-03 20:33:53.000000 sbcli-1b0/management/models/iface.py
--rw-rw-rw-   0        0        0      620 2023-05-22 22:52:24.000000 sbcli-1b0/management/models/mgmt_node.py
--rw-rw-rw-   0        0        0     1451 2023-06-28 16:43:11.000000 sbcli-1b0/management/models/nvme_device.py
--rw-rw-rw-   0        0        0     1690 2023-06-29 12:54:01.000000 sbcli-1b0/management/models/pool.py
--rw-rw-rw-   0        0        0     3364 2023-06-28 16:58:39.000000 sbcli-1b0/management/models/storage_node.py
--rw-rw-rw-   0        0        0      966 2023-02-16 22:27:55.000000 sbcli-1b0/management/pci_utils.py
--rw-rw-rw-   0        0        0    11574 2023-06-28 16:43:12.000000 sbcli-1b0/management/rpc_client.py
-drwxrwxrwx   0        0        0        0 2023-07-19 14:32:40.124984 sbcli-1b0/management/services/
--rw-rw-rw-   0        0        0     5008 2023-07-12 16:29:01.000000 sbcli-1b0/management/services/__init__.py
--rw-rw-rw-   0        0        0     1865 2021-12-22 20:16:04.000000 sbcli-1b0/management/services/device_monitor.py
--rw-rw-rw-   0        0        0     3515 2023-07-13 19:22:01.000000 sbcli-1b0/management/services/device_stat_collector.py
--rw-rw-rw-   0        0        0     3185 2023-07-13 19:22:01.000000 sbcli-1b0/management/services/lvol_stat_collector.py
--rw-rw-rw-   0        0        0     3012 2023-06-27 11:52:17.000000 sbcli-1b0/management/services/mgmt_node_monitor.py
--rw-rw-rw-   0        0        0     2153 2022-01-11 22:20:04.000000 sbcli-1b0/management/services/node_monitor.py
--rw-rw-rw-   0        0        0     2445 2023-07-03 20:33:53.000000 sbcli-1b0/management/services/port_stat_collector.py
--rw-rw-rw-   0        0        0     3999 2022-01-14 19:44:44.000000 sbcli-1b0/management/services/stat_collector.py
--rw-rw-rw-   0        0        0      288 2023-02-16 23:53:54.000000 sbcli-1b0/management/shell_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-19 14:32:40.126982 sbcli-1b0/management/spdk_installer/
--rw-rw-rw-   0        0        0      747 2023-03-02 14:29:22.000000 sbcli-1b0/management/spdk_installer/__init__.py
--rw-rw-rw-   0        0        0    53543 2023-07-13 19:39:33.000000 sbcli-1b0/management/storage_node_ops.py
--rw-rw-rw-   0        0        0     1784 2023-07-03 20:29:53.000000 sbcli-1b0/management/utils.py
--rw-rw-rw-   0        0        0       86 2023-07-19 14:06:48.000000 sbcli-1b0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-19 14:32:40.149921 sbcli-1b0/sbcli.egg-info/
--rw-rw-rw-   0        0        0    43376 2023-07-19 14:32:40.000000 sbcli-1b0/sbcli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1427 2023-07-19 14:32:40.000000 sbcli-1b0/sbcli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 14:32:40.000000 sbcli-1b0/sbcli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-07-19 14:32:40.000000 sbcli-1b0/sbcli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-07-19 14:32:40.000000 sbcli-1b0/sbcli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-19 14:32:40.152911 sbcli-1b0/setup.cfg
--rw-rw-rw-   0        0        0      728 2023-07-19 14:32:22.000000 sbcli-1b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 14:35:07.288292 sbcli-2/
+-rw-rw-rw-   0        0        0    43374 2023-07-19 14:35:07.287295 sbcli-2/PKG-INFO
+-rw-rw-rw-   0        0        0    43124 2023-07-13 15:17:09.000000 sbcli-2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 14:35:07.217480 sbcli-2/management/
+-rw-rw-rw-   0        0        0        0 2021-10-27 21:58:56.000000 sbcli-2/management/__init__.py
+-rw-rw-rw-   0        0        0    51657 2023-07-19 14:29:48.000000 sbcli-2/management/cli.py
+-rw-rw-rw-   0        0        0     6893 2023-07-11 13:47:18.000000 sbcli-2/management/cluster_ops.py
+-rw-rw-rw-   0        0        0     5264 2023-03-06 15:46:56.000000 sbcli-2/management/compute_node_ops.py
+-rw-rw-rw-   0        0        0      755 2023-07-06 18:09:38.000000 sbcli-2/management/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-19 14:35:07.228452 sbcli-2/management/controllers/
+-rw-rw-rw-   0        0        0        0 2023-03-06 16:32:43.000000 sbcli-2/management/controllers/__init__.py
+-rw-rw-rw-   0        0        0      955 2023-06-27 12:09:06.000000 sbcli-2/management/controllers/cluster_lifecycle.py
+-rw-rw-rw-   0        0        0     8787 2023-06-27 12:04:07.000000 sbcli-2/management/controllers/device_lifecycle.py
+-rw-rw-rw-   0        0        0    16507 2023-07-13 17:10:28.000000 sbcli-2/management/controllers/lvol_controller.py
+-rw-rw-rw-   0        0        0    13889 2023-06-27 12:01:46.000000 sbcli-2/management/controllers/node_lifecycle.py
+-rw-rw-rw-   0        0        0     9473 2023-06-29 12:54:01.000000 sbcli-2/management/controllers/pool_controller.py
+-rw-rw-rw-   0        0        0     5773 2023-07-13 17:28:28.000000 sbcli-2/management/kv_store.py
+-rw-rw-rw-   0        0        0     3578 2023-05-22 22:51:19.000000 sbcli-2/management/mgmt_node_ops.py
+drwxrwxrwx   0        0        0        0 2023-07-19 14:35:07.247401 sbcli-2/management/models/
+-rw-rw-rw-   0        0        0        0 2021-10-28 14:11:47.000000 sbcli-2/management/models/__init__.py
+-rw-rw-rw-   0        0        0     4681 2023-07-13 17:24:37.000000 sbcli-2/management/models/base_model.py
+-rw-rw-rw-   0        0        0     1815 2023-07-11 12:10:41.000000 sbcli-2/management/models/cluster.py
+-rw-rw-rw-   0        0        0      943 2023-02-08 22:16:26.000000 sbcli-2/management/models/compute_node.py
+-rw-rw-rw-   0        0        0     3019 2023-07-13 18:37:17.000000 sbcli-2/management/models/device_stat.py
+-rw-rw-rw-   0        0        0     1251 2023-05-09 17:37:12.000000 sbcli-2/management/models/global_settings.py
+-rw-rw-rw-   0        0        0      830 2023-07-03 20:33:53.000000 sbcli-2/management/models/iface.py
+-rw-rw-rw-   0        0        0      620 2023-05-22 22:52:24.000000 sbcli-2/management/models/mgmt_node.py
+-rw-rw-rw-   0        0        0     1451 2023-06-28 16:43:11.000000 sbcli-2/management/models/nvme_device.py
+-rw-rw-rw-   0        0        0     1690 2023-06-29 12:54:01.000000 sbcli-2/management/models/pool.py
+-rw-rw-rw-   0        0        0     3364 2023-06-28 16:58:39.000000 sbcli-2/management/models/storage_node.py
+-rw-rw-rw-   0        0        0      966 2023-02-16 22:27:55.000000 sbcli-2/management/pci_utils.py
+-rw-rw-rw-   0        0        0    11574 2023-06-28 16:43:12.000000 sbcli-2/management/rpc_client.py
+drwxrwxrwx   0        0        0        0 2023-07-19 14:35:07.262362 sbcli-2/management/services/
+-rw-rw-rw-   0        0        0     5008 2023-07-12 16:29:01.000000 sbcli-2/management/services/__init__.py
+-rw-rw-rw-   0        0        0     1865 2021-12-22 20:16:04.000000 sbcli-2/management/services/device_monitor.py
+-rw-rw-rw-   0        0        0     3515 2023-07-13 19:22:01.000000 sbcli-2/management/services/device_stat_collector.py
+-rw-rw-rw-   0        0        0     3185 2023-07-13 19:22:01.000000 sbcli-2/management/services/lvol_stat_collector.py
+-rw-rw-rw-   0        0        0     3012 2023-06-27 11:52:17.000000 sbcli-2/management/services/mgmt_node_monitor.py
+-rw-rw-rw-   0        0        0     2153 2022-01-11 22:20:04.000000 sbcli-2/management/services/node_monitor.py
+-rw-rw-rw-   0        0        0     2445 2023-07-03 20:33:53.000000 sbcli-2/management/services/port_stat_collector.py
+-rw-rw-rw-   0        0        0     3999 2022-01-14 19:44:44.000000 sbcli-2/management/services/stat_collector.py
+-rw-rw-rw-   0        0        0      288 2023-02-16 23:53:54.000000 sbcli-2/management/shell_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-19 14:35:07.264357 sbcli-2/management/spdk_installer/
+-rw-rw-rw-   0        0        0      747 2023-03-02 14:29:22.000000 sbcli-2/management/spdk_installer/__init__.py
+-rw-rw-rw-   0        0        0    53543 2023-07-13 19:39:33.000000 sbcli-2/management/storage_node_ops.py
+-rw-rw-rw-   0        0        0     1784 2023-07-03 20:29:53.000000 sbcli-2/management/utils.py
+-rw-rw-rw-   0        0        0       86 2023-07-19 14:06:48.000000 sbcli-2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-19 14:35:07.286298 sbcli-2/sbcli.egg-info/
+-rw-rw-rw-   0        0        0    43374 2023-07-19 14:35:07.000000 sbcli-2/sbcli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1427 2023-07-19 14:35:07.000000 sbcli-2/sbcli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 14:35:07.000000 sbcli-2/sbcli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-19 14:35:07.000000 sbcli-2/sbcli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2023-07-19 14:35:07.000000 sbcli-2/sbcli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 14:35:07.289290 sbcli-2/setup.cfg
+-rw-rw-rw-   0        0        0      723 2023-07-19 14:34:49.000000 sbcli-2/setup.py
```

### Comparing `sbcli-1b0/PKG-INFO` & `sbcli-2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli
-Version: 1b0
+Version: 2
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://github.com/simplyblock-io/ultra
 Author: Hamdy Khader
 Author-email: hamdy.khader@gmail.com
 Description-Content-Type: text/markdown
```

### Comparing `sbcli-1b0/README.md` & `sbcli-2/README.md`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/cli.py` & `sbcli-2/management/cli.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/cluster_ops.py` & `sbcli-2/management/cluster_ops.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/compute_node_ops.py` & `sbcli-2/management/compute_node_ops.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/constants.py` & `sbcli-2/management/constants.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/controllers/cluster_lifecycle.py` & `sbcli-2/management/controllers/cluster_lifecycle.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/controllers/device_lifecycle.py` & `sbcli-2/management/controllers/device_lifecycle.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/controllers/lvol_controller.py` & `sbcli-2/management/controllers/lvol_controller.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/controllers/node_lifecycle.py` & `sbcli-2/management/controllers/node_lifecycle.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/controllers/pool_controller.py` & `sbcli-2/management/controllers/pool_controller.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/kv_store.py` & `sbcli-2/management/kv_store.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/mgmt_node_ops.py` & `sbcli-2/management/mgmt_node_ops.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/models/base_model.py` & `sbcli-2/management/models/base_model.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/models/cluster.py` & `sbcli-2/management/models/cluster.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/models/compute_node.py` & `sbcli-2/management/models/compute_node.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/models/device_stat.py` & `sbcli-2/management/models/device_stat.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/models/global_settings.py` & `sbcli-2/management/models/global_settings.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/models/iface.py` & `sbcli-2/management/models/iface.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/models/mgmt_node.py` & `sbcli-2/management/models/mgmt_node.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/models/nvme_device.py` & `sbcli-2/management/models/nvme_device.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/models/pool.py` & `sbcli-2/management/models/pool.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/models/storage_node.py` & `sbcli-2/management/models/storage_node.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/pci_utils.py` & `sbcli-2/management/pci_utils.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/rpc_client.py` & `sbcli-2/management/rpc_client.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/services/__init__.py` & `sbcli-2/management/services/__init__.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/services/device_monitor.py` & `sbcli-2/management/services/device_monitor.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/services/device_stat_collector.py` & `sbcli-2/management/services/device_stat_collector.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/services/lvol_stat_collector.py` & `sbcli-2/management/services/lvol_stat_collector.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/services/mgmt_node_monitor.py` & `sbcli-2/management/services/mgmt_node_monitor.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/services/node_monitor.py` & `sbcli-2/management/services/node_monitor.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/services/port_stat_collector.py` & `sbcli-2/management/services/port_stat_collector.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/services/stat_collector.py` & `sbcli-2/management/services/stat_collector.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/spdk_installer/__init__.py` & `sbcli-2/management/spdk_installer/__init__.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/storage_node_ops.py` & `sbcli-2/management/storage_node_ops.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/management/utils.py` & `sbcli-2/management/utils.py`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/sbcli.egg-info/PKG-INFO` & `sbcli-2/sbcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli
-Version: 1b0
+Version: 2
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://github.com/simplyblock-io/ultra
 Author: Hamdy Khader
 Author-email: hamdy.khader@gmail.com
 Description-Content-Type: text/markdown
```

### Comparing `sbcli-1b0/sbcli.egg-info/SOURCES.txt` & `sbcli-2/sbcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sbcli-1b0/setup.py` & `sbcli-2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='sbcli',
-    version='1-beta',
+    version='2',
     packages=find_packages(),
     url='https://github.com/simplyblock-io/ultra',
     author='Hamdy Khader',
     author_email='hamdy.khader@gmail.com',
     description='CLI for managing SimplyBlock cluster',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

