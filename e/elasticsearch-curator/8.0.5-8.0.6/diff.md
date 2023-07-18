# Comparing `tmp/elasticsearch_curator-8.0.5.tar.gz` & `tmp/elasticsearch_curator-8.0.6.tar.gz`

## Comparing `elasticsearch_curator-8.0.5.tar` & `elasticsearch_curator-8.0.6.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/_version.py
--rw-r--r--   0        0        0     9608 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/classdef.py
--rw-r--r--   0        0        0    15861 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/config_utils.py
--rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/curator_cli.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/exceptions.py
--rw-r--r--   0        0        0    57820 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/indexlist.py
--rw-r--r--   0        0        0     5448 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/logtools.py
--rw-r--r--   0        0        0    23556 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/repomgrcli.py
--rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/singletons.py
--rw-r--r--   0        0        0    22898 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/snapshotlist.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/__init__.py
--rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/alias.py
--rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/allocation.py
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/close.py
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/cluster_routing.py
--rw-r--r--   0        0        0     8770 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/cold2frozen.py
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/create_index.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/delete_indices.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/forcemerge.py
--rw-r--r--   0        0        0     5603 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/index_settings.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/open.py
--rw-r--r--   0        0        0    17631 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/reindex.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/replicas.py
--rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/rollover.py
--rw-r--r--   0        0        0    24570 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/shrink.py
--rw-r--r--   0        0        0    21632 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/actions/snapshot.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/__init__.py
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/alias.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/allocation.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/close.py
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/delete.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/forcemerge.py
--rw-r--r--   0        0        0     9687 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/object_class.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/open_indices.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/replicas.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/restore.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/rollover.py
--rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/show.py
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/shrink.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/snapshot.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/cli_singletons/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/defaults/__init__.py
--rw-r--r--   0        0        0    11383 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/defaults/filter_elements.py
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/defaults/filtertypes.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/defaults/logging_defaults.py
--rw-r--r--   0        0        0    18383 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/defaults/option_defaults.py
--rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/defaults/settings.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/helpers/__init__.py
--rw-r--r--   0        0        0    23308 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/helpers/date_ops.py
--rw-r--r--   0        0        0    13903 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/helpers/getters.py
--rw-r--r--   0        0        0    15381 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/helpers/testers.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/helpers/utils.py
--rw-r--r--   0        0        0    12701 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/helpers/waiters.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/validators/__init__.py
--rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/validators/actions.py
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/validators/filter_functions.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/validators/logconfig.py
--rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/validators/options.py
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/curator/validators/schemacheck.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/.gitignore
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/LICENSE
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/NOTICE
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/README.rst
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/pyproject.toml
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.5/PKG-INFO
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/_version.py
+-rw-r--r--   0        0        0     9608 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/classdef.py
+-rw-r--r--   0        0        0    15861 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/cli.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/config_utils.py
+-rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/curator_cli.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/exceptions.py
+-rw-r--r--   0        0        0    60192 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/indexlist.py
+-rw-r--r--   0        0        0     5448 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/logtools.py
+-rw-r--r--   0        0        0    23556 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/repomgrcli.py
+-rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/singletons.py
+-rw-r--r--   0        0        0    22898 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/snapshotlist.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/actions/__init__.py
+-rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/actions/alias.py
+-rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/actions/allocation.py
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/actions/close.py
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/actions/cluster_routing.py
+-rw-r--r--   0        0        0     8770 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/actions/cold2frozen.py
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/actions/create_index.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/actions/delete_indices.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/actions/forcemerge.py
+-rw-r--r--   0        0        0     5603 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/actions/index_settings.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/actions/open.py
+-rw-r--r--   0        0        0    17631 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/actions/reindex.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/actions/replicas.py
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/actions/rollover.py
+-rw-r--r--   0        0        0    24570 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/actions/shrink.py
+-rw-r--r--   0        0        0    21632 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/actions/snapshot.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/cli_singletons/__init__.py
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/cli_singletons/alias.py
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/cli_singletons/allocation.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/cli_singletons/close.py
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/cli_singletons/delete.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/cli_singletons/forcemerge.py
+-rw-r--r--   0        0        0     9687 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/cli_singletons/object_class.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/cli_singletons/open_indices.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/cli_singletons/replicas.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/cli_singletons/restore.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/cli_singletons/rollover.py
+-rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/cli_singletons/show.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/cli_singletons/shrink.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/cli_singletons/snapshot.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/cli_singletons/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/defaults/__init__.py
+-rw-r--r--   0        0        0    11383 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/defaults/filter_elements.py
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/defaults/filtertypes.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/defaults/logging_defaults.py
+-rw-r--r--   0        0        0    18383 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/defaults/option_defaults.py
+-rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/defaults/settings.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/helpers/__init__.py
+-rw-r--r--   0        0        0    23308 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/helpers/date_ops.py
+-rw-r--r--   0        0        0    13903 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/helpers/getters.py
+-rw-r--r--   0        0        0    15381 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/helpers/testers.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/helpers/utils.py
+-rw-r--r--   0        0        0    12701 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/helpers/waiters.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/validators/__init__.py
+-rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/validators/actions.py
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/validators/filter_functions.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/validators/logconfig.py
+-rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/validators/options.py
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/curator/validators/schemacheck.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/.gitignore
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/LICENSE
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/NOTICE
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/README.rst
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.6/PKG-INFO
```

### Comparing `elasticsearch_curator-8.0.5/curator/classdef.py` & `elasticsearch_curator-8.0.6/curator/classdef.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/cli.py` & `elasticsearch_curator-8.0.6/curator/cli.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/config_utils.py` & `elasticsearch_curator-8.0.6/curator/config_utils.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/exceptions.py` & `elasticsearch_curator-8.0.6/curator/exceptions.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/indexlist.py` & `elasticsearch_curator-8.0.6/curator/indexlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
         """
         self.loggit.debug('Getting all indices')
         self.all_indices = get_indices(self.client)
         self.indices = self.all_indices[:]
         if self.indices:
             for index in self.indices:
                 self.__build_index_info(index)
+            self.loggit.debug('FRESH UNPOPULATED: self.index_info = %s', self.index_info)
             self.get_metadata()
             self.get_index_stats()
 
     def __build_index_info(self, index):
         """
         Ensure that ``index`` is a key in ``index_info``. If not, create a sub-dictionary structure
         under that key.
@@ -191,20 +192,46 @@
                 data_sliced = data[num*slice_number:(num+1)*slice_number]
             query_result.update(exec_func(data_sliced))
         return query_result
 
     def _get_cluster_state(self, data):
         return self.client.cluster.state(index=to_csv(data), metric='metadata')['metadata']['indices']
 
+    def mitigate_alias(self, index):
+        """
+        Mitigate when an alias is detected instead of an index name
+
+        :param index: The index name that is showing up *instead* of what was expected
+
+        :type index: str
+
+        :returns: No return value:
+        :rtype: None
+        """
+        self.loggit.debug('Correcting an instance where an alias name points to index "%s"', index)
+        data = self.client.indices.get(index=index)
+        aliases = list(data[index]['aliases'])
+        if aliases:
+            for alias in aliases:
+                if alias in self.indices:
+                    self.loggit.warning('Removing alias "%s" from IndexList.indices', alias)
+                    self.indices.remove(alias)
+                if alias in list(self.index_info):
+                    self.loggit.warning('Removing alias "%s" from IndexList.index_info', alias)
+                    del self.index_info[alias]
+        self.loggit.debug('Adding "%s" to IndexList.indices', index)
+        self.indices.append(index)
+        self.loggit.debug('Adding preliminary metadata for "%s" to IndexList.index_info', index)
+        self.__build_index_info(index)
+
     def get_metadata(self):
         """
         Populate ``index_info`` with index ``size_in_bytes`` and doc count information for each
         index.
         """
-        self.loggit.debug('Getting index metadata')
         self.empty_list_check()
         for lst in chunk_index_list(self.indices):
             working_list = {}
             # The API called by _get_cluster_state doesn't suffer from the same problems that
             # _get_indices_stats does. This won't result in an error if an index is suddenly
             # missing.
             try:
@@ -212,16 +239,33 @@
             except TransportError as err:
                 if '413' in err.errors:
                     msg = 'Huge Payload 413 Err - Trying to get information via multiple requests'
                     self.loggit.debug(msg)
                     working_list = {}
                     working_list.update(self._bulk_queries(lst, self._get_cluster_state))
             if working_list:
+                self.loggit.debug('working_list.keys() = %s', working_list.keys())
                 for index in list(working_list.keys()):
-                    sii = self.index_info[index]
+                    self.loggit.debug('index = %s', index)
+                    try:
+                        sii = self.index_info[index]
+                    except KeyError:
+                        # What I believe has happened with this race condition is that during
+                        # __build_index_info initially, an index has a name, but is in process
+                        # of being remounted as a searchable snapshot index, and suddenly the
+                        # original index name is an alias, and the _get_cluster_state call returns
+                        # the new, actual index name instead of the alias it had. This is how a
+                        # KeyError can actually happen in this case. The relevant logs showing
+                        # this behavior are in issue #1682
+                        self.loggit.warning(
+                            'Index %s was not present at IndexList initialization, and may be '
+                            'behind an alias', index
+                        )
+                        self.mitigate_alias(index)
+                        sii = self.index_info[index]
                     wli = working_list[index]
                     sii['age']['creation_date'] = (
                         fix_epoch(wli['settings']['index']['creation_date'])
                     )
                     sii['number_of_replicas'] = wli['settings']['index']['number_of_replicas']
                     sii['number_of_shards'] = wli['settings']['index']['number_of_shards']
                     sii['state'] = wli['state']
```

### Comparing `elasticsearch_curator-8.0.5/curator/logtools.py` & `elasticsearch_curator-8.0.6/curator/logtools.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/repomgrcli.py` & `elasticsearch_curator-8.0.6/curator/repomgrcli.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/singletons.py` & `elasticsearch_curator-8.0.6/curator/singletons.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/snapshotlist.py` & `elasticsearch_curator-8.0.6/curator/snapshotlist.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/actions/__init__.py` & `elasticsearch_curator-8.0.6/curator/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/actions/alias.py` & `elasticsearch_curator-8.0.6/curator/actions/alias.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/actions/allocation.py` & `elasticsearch_curator-8.0.6/curator/actions/allocation.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/actions/close.py` & `elasticsearch_curator-8.0.6/curator/actions/close.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/actions/cluster_routing.py` & `elasticsearch_curator-8.0.6/curator/actions/cluster_routing.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/actions/cold2frozen.py` & `elasticsearch_curator-8.0.6/curator/actions/cold2frozen.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/actions/create_index.py` & `elasticsearch_curator-8.0.6/curator/actions/create_index.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/actions/delete_indices.py` & `elasticsearch_curator-8.0.6/curator/actions/delete_indices.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/actions/forcemerge.py` & `elasticsearch_curator-8.0.6/curator/actions/forcemerge.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/actions/index_settings.py` & `elasticsearch_curator-8.0.6/curator/actions/index_settings.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/actions/open.py` & `elasticsearch_curator-8.0.6/curator/actions/open.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/actions/reindex.py` & `elasticsearch_curator-8.0.6/curator/actions/reindex.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/actions/replicas.py` & `elasticsearch_curator-8.0.6/curator/actions/replicas.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/actions/rollover.py` & `elasticsearch_curator-8.0.6/curator/actions/rollover.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/actions/shrink.py` & `elasticsearch_curator-8.0.6/curator/actions/shrink.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/actions/snapshot.py` & `elasticsearch_curator-8.0.6/curator/actions/snapshot.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/cli_singletons/__init__.py` & `elasticsearch_curator-8.0.6/curator/cli_singletons/__init__.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/cli_singletons/alias.py` & `elasticsearch_curator-8.0.6/curator/cli_singletons/alias.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/cli_singletons/allocation.py` & `elasticsearch_curator-8.0.6/curator/cli_singletons/allocation.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/cli_singletons/close.py` & `elasticsearch_curator-8.0.6/curator/cli_singletons/close.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/cli_singletons/delete.py` & `elasticsearch_curator-8.0.6/curator/cli_singletons/delete.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/cli_singletons/forcemerge.py` & `elasticsearch_curator-8.0.6/curator/cli_singletons/forcemerge.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/cli_singletons/object_class.py` & `elasticsearch_curator-8.0.6/curator/cli_singletons/object_class.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/cli_singletons/open_indices.py` & `elasticsearch_curator-8.0.6/curator/cli_singletons/open_indices.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/cli_singletons/replicas.py` & `elasticsearch_curator-8.0.6/curator/cli_singletons/replicas.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/cli_singletons/restore.py` & `elasticsearch_curator-8.0.6/curator/cli_singletons/restore.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/cli_singletons/rollover.py` & `elasticsearch_curator-8.0.6/curator/cli_singletons/rollover.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/cli_singletons/show.py` & `elasticsearch_curator-8.0.6/curator/cli_singletons/show.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/cli_singletons/shrink.py` & `elasticsearch_curator-8.0.6/curator/cli_singletons/shrink.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/cli_singletons/snapshot.py` & `elasticsearch_curator-8.0.6/curator/cli_singletons/snapshot.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/cli_singletons/utils.py` & `elasticsearch_curator-8.0.6/curator/cli_singletons/utils.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/defaults/filter_elements.py` & `elasticsearch_curator-8.0.6/curator/defaults/filter_elements.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/defaults/filtertypes.py` & `elasticsearch_curator-8.0.6/curator/defaults/filtertypes.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/defaults/logging_defaults.py` & `elasticsearch_curator-8.0.6/curator/defaults/logging_defaults.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/defaults/option_defaults.py` & `elasticsearch_curator-8.0.6/curator/defaults/option_defaults.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/defaults/settings.py` & `elasticsearch_curator-8.0.6/curator/defaults/settings.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/helpers/date_ops.py` & `elasticsearch_curator-8.0.6/curator/helpers/date_ops.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/helpers/getters.py` & `elasticsearch_curator-8.0.6/curator/helpers/getters.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/helpers/testers.py` & `elasticsearch_curator-8.0.6/curator/helpers/testers.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/helpers/utils.py` & `elasticsearch_curator-8.0.6/curator/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/helpers/waiters.py` & `elasticsearch_curator-8.0.6/curator/helpers/waiters.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/validators/actions.py` & `elasticsearch_curator-8.0.6/curator/validators/actions.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/validators/filter_functions.py` & `elasticsearch_curator-8.0.6/curator/validators/filter_functions.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/validators/options.py` & `elasticsearch_curator-8.0.6/curator/validators/options.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/curator/validators/schemacheck.py` & `elasticsearch_curator-8.0.6/curator/validators/schemacheck.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/LICENSE` & `elasticsearch_curator-8.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/NOTICE` & `elasticsearch_curator-8.0.6/NOTICE`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/README.rst` & `elasticsearch_curator-8.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/pyproject.toml` & `elasticsearch_curator-8.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.5/PKG-INFO` & `elasticsearch_curator-8.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elasticsearch-curator
-Version: 8.0.5
+Version: 8.0.6
 Summary: Tending your Elasticsearch indices and snapshots
 Project-URL: Homepage, https://github.com/elastic/curator
 Project-URL: Bug Tracker, https://github.com/elastic/curator/issues
 Author-email: Elastic <info@elastic.co>
 License: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
```

