# Comparing `tmp/molgenis-emx2-ontomanager-0.2.8.tar.gz` & `tmp/molgenis-emx2-ontomanager-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgenis-emx2-ontomanager-0.2.8.tar", last modified: Mon Jul 17 12:48:19 2023, max compression
+gzip compressed data, was "molgenis-emx2-ontomanager-0.2.9.tar", last modified: Wed Jul 19 11:35:07 2023, max compression
```

## Comparing `molgenis-emx2-ontomanager-0.2.8.tar` & `molgenis-emx2-ontomanager-0.2.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-17 12:48:19.641599 molgenis-emx2-ontomanager-0.2.8/
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     6544 2023-07-17 12:48:19.641028 molgenis-emx2-ontomanager-0.2.8/PKG-INFO
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     6020 2023-07-14 14:46:13.000000 molgenis-emx2-ontomanager-0.2.8/README.md
-drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-17 12:48:19.605517 molgenis-emx2-ontomanager-0.2.8/demos/
-drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-17 12:48:19.607438 molgenis-emx2-ontomanager-0.2.8/demos/data/
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       82 2023-07-05 10:52:46.000000 molgenis-emx2-ontomanager-0.2.8/demos/data/Countries.csv
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       89 2023-07-03 12:58:30.000000 molgenis-emx2-ontomanager-0.2.8/demos/data/update.csv
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     2279 2023-07-05 14:32:26.000000 molgenis-emx2-ontomanager-0.2.8/demos/demo_csv_upload.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     2150 2023-07-05 10:54:36.000000 molgenis-emx2-ontomanager-0.2.8/demos/demo_ontomanager.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     1860 2023-07-05 08:54:51.000000 molgenis-emx2-ontomanager-0.2.8/demos/demo_search.py
-drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-17 12:48:19.608969 molgenis-emx2-ontomanager-0.2.8/dev/
-drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-17 12:48:19.633486 molgenis-emx2-ontomanager-0.2.8/dev/data/
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       82 2023-07-05 10:52:46.000000 molgenis-emx2-ontomanager-0.2.8/dev/data/Countries.csv
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       89 2023-07-03 12:58:30.000000 molgenis-emx2-ontomanager-0.2.8/dev/data/update.csv
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     2393 2023-07-17 12:30:08.000000 molgenis-emx2-ontomanager-0.2.8/dev/dev_csv_upload.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     2412 2023-07-17 12:48:05.000000 molgenis-emx2-ontomanager-0.2.8/dev/dev_ontomanager.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     1882 2023-07-14 08:50:25.000000 molgenis-emx2-ontomanager-0.2.8/dev/dev_search.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)      752 2023-07-10 14:33:54.000000 molgenis-emx2-ontomanager-0.2.8/pyproject.toml
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       97 2023-07-10 13:14:26.000000 molgenis-emx2-ontomanager-0.2.8/requirements.txt
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       38 2023-07-17 12:48:19.641745 molgenis-emx2-ontomanager-0.2.8/setup.cfg
-drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-17 12:48:19.601253 molgenis-emx2-ontomanager-0.2.8/src/
-drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-17 12:48:19.637876 molgenis-emx2-ontomanager-0.2.8/src/molgenis_emx2_ontomanager/
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)    23847 2023-07-17 12:42:53.000000 molgenis-emx2-ontomanager-0.2.8/src/molgenis_emx2_ontomanager/OntologyManager.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       60 2023-06-28 11:55:29.000000 molgenis-emx2-ontomanager-0.2.8/src/molgenis_emx2_ontomanager/__init__.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     3500 2023-06-28 13:26:24.000000 molgenis-emx2-ontomanager-0.2.8/src/molgenis_emx2_ontomanager/__main__.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-03 08:33:42.000000 molgenis-emx2-ontomanager-0.2.8/src/molgenis_emx2_ontomanager/cli.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)      127 2023-06-28 11:55:29.000000 molgenis-emx2-ontomanager-0.2.8/src/molgenis_emx2_ontomanager/constants.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     1445 2023-07-03 14:40:41.000000 molgenis-emx2-ontomanager-0.2.8/src/molgenis_emx2_ontomanager/exceptions.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     3729 2023-07-03 09:45:28.000000 molgenis-emx2-ontomanager-0.2.8/src/molgenis_emx2_ontomanager/graphql_queries.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)      658 2023-07-17 12:40:47.000000 molgenis-emx2-ontomanager-0.2.8/src/molgenis_emx2_ontomanager/utils.py
-drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-17 12:48:19.640342 molgenis-emx2-ontomanager-0.2.8/src/molgenis_emx2_ontomanager.egg-info/
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     6544 2023-07-17 12:48:19.000000 molgenis-emx2-ontomanager-0.2.8/src/molgenis_emx2_ontomanager.egg-info/PKG-INFO
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)      887 2023-07-17 12:48:19.000000 molgenis-emx2-ontomanager-0.2.8/src/molgenis_emx2_ontomanager.egg-info/SOURCES.txt
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)        1 2023-07-17 12:48:19.000000 molgenis-emx2-ontomanager-0.2.8/src/molgenis_emx2_ontomanager.egg-info/dependency_links.txt
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       98 2023-07-17 12:48:19.000000 molgenis-emx2-ontomanager-0.2.8/src/molgenis_emx2_ontomanager.egg-info/requires.txt
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       26 2023-07-17 12:48:19.000000 molgenis-emx2-ontomanager-0.2.8/src/molgenis_emx2_ontomanager.egg-info/top_level.txt
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)        5 2023-07-14 14:46:13.000000 molgenis-emx2-ontomanager-0.2.8/version.txt
+drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-19 11:35:07.006842 molgenis-emx2-ontomanager-0.2.9/
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     6544 2023-07-19 11:35:07.006102 molgenis-emx2-ontomanager-0.2.9/PKG-INFO
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     6020 2023-07-19 11:11:42.000000 molgenis-emx2-ontomanager-0.2.9/README.md
+drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-19 11:35:06.991392 molgenis-emx2-ontomanager-0.2.9/demos/
+drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-19 11:35:06.993069 molgenis-emx2-ontomanager-0.2.9/demos/data/
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       82 2023-07-19 11:11:42.000000 molgenis-emx2-ontomanager-0.2.9/demos/data/Countries.csv
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       89 2023-07-19 11:11:42.000000 molgenis-emx2-ontomanager-0.2.9/demos/data/update.csv
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     2279 2023-07-19 11:11:42.000000 molgenis-emx2-ontomanager-0.2.9/demos/demo_csv_upload.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     2150 2023-07-19 11:11:42.000000 molgenis-emx2-ontomanager-0.2.9/demos/demo_ontomanager.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     1860 2023-07-19 11:11:42.000000 molgenis-emx2-ontomanager-0.2.9/demos/demo_search.py
+drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-19 11:35:06.994984 molgenis-emx2-ontomanager-0.2.9/dev/
+drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-19 11:35:06.996310 molgenis-emx2-ontomanager-0.2.9/dev/data/
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       82 2023-07-19 11:11:42.000000 molgenis-emx2-ontomanager-0.2.9/dev/data/Countries.csv
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       89 2023-07-19 11:11:42.000000 molgenis-emx2-ontomanager-0.2.9/dev/data/update.csv
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     2594 2023-07-19 11:32:00.000000 molgenis-emx2-ontomanager-0.2.9/dev/dev_csv_upload.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     2412 2023-07-19 11:23:33.000000 molgenis-emx2-ontomanager-0.2.9/dev/dev_ontomanager.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     1882 2023-07-19 11:11:42.000000 molgenis-emx2-ontomanager-0.2.9/dev/dev_search.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)      752 2023-07-19 11:11:42.000000 molgenis-emx2-ontomanager-0.2.9/pyproject.toml
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       97 2023-07-19 11:11:42.000000 molgenis-emx2-ontomanager-0.2.9/requirements.txt
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       38 2023-07-19 11:35:07.006998 molgenis-emx2-ontomanager-0.2.9/setup.cfg
+drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-19 11:35:06.988500 molgenis-emx2-ontomanager-0.2.9/src/
+drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-19 11:35:07.001659 molgenis-emx2-ontomanager-0.2.9/src/molgenis_emx2_ontomanager/
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)    25084 2023-07-19 11:23:33.000000 molgenis-emx2-ontomanager-0.2.9/src/molgenis_emx2_ontomanager/OntologyManager.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       60 2023-07-19 11:11:42.000000 molgenis-emx2-ontomanager-0.2.9/src/molgenis_emx2_ontomanager/__init__.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     3500 2023-07-19 11:11:42.000000 molgenis-emx2-ontomanager-0.2.9/src/molgenis_emx2_ontomanager/__main__.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-03 08:33:42.000000 molgenis-emx2-ontomanager-0.2.9/src/molgenis_emx2_ontomanager/cli.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)      127 2023-07-19 11:11:42.000000 molgenis-emx2-ontomanager-0.2.9/src/molgenis_emx2_ontomanager/constants.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     1445 2023-07-19 11:11:42.000000 molgenis-emx2-ontomanager-0.2.9/src/molgenis_emx2_ontomanager/exceptions.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     3910 2023-07-19 11:11:42.000000 molgenis-emx2-ontomanager-0.2.9/src/molgenis_emx2_ontomanager/graphql_queries.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)      658 2023-07-19 11:11:42.000000 molgenis-emx2-ontomanager-0.2.9/src/molgenis_emx2_ontomanager/utils.py
+drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-07-19 11:35:07.004703 molgenis-emx2-ontomanager-0.2.9/src/molgenis_emx2_ontomanager.egg-info/
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     6544 2023-07-19 11:35:06.000000 molgenis-emx2-ontomanager-0.2.9/src/molgenis_emx2_ontomanager.egg-info/PKG-INFO
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)      887 2023-07-19 11:35:06.000000 molgenis-emx2-ontomanager-0.2.9/src/molgenis_emx2_ontomanager.egg-info/SOURCES.txt
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)        1 2023-07-19 11:35:06.000000 molgenis-emx2-ontomanager-0.2.9/src/molgenis_emx2_ontomanager.egg-info/dependency_links.txt
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       98 2023-07-19 11:35:06.000000 molgenis-emx2-ontomanager-0.2.9/src/molgenis_emx2_ontomanager.egg-info/requires.txt
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       26 2023-07-19 11:35:06.000000 molgenis-emx2-ontomanager-0.2.9/src/molgenis_emx2_ontomanager.egg-info/top_level.txt
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)        5 2023-07-19 11:11:55.000000 molgenis-emx2-ontomanager-0.2.9/version.txt
```

### Comparing `molgenis-emx2-ontomanager-0.2.8/PKG-INFO` & `molgenis-emx2-ontomanager-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgenis-emx2-ontomanager
-Version: 0.2.8
+Version: 0.2.9
 Summary: Tool to manage catalogue ontologies on Molgenis EMX2 servers.
 Project-URL: Homepage, https://github.com/molgenis/molgenis-emx2
 Project-URL: Bug Tracker, https://github.com/molgenis/molgenis-emx2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `molgenis-emx2-ontomanager-0.2.8/README.md` & `molgenis-emx2-ontomanager-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `molgenis-emx2-ontomanager-0.2.8/demos/demo_csv_upload.py` & `molgenis-emx2-ontomanager-0.2.9/demos/demo_csv_upload.py`

 * *Files identical despite different names*

### Comparing `molgenis-emx2-ontomanager-0.2.8/demos/demo_ontomanager.py` & `molgenis-emx2-ontomanager-0.2.9/demos/demo_ontomanager.py`

 * *Files identical despite different names*

### Comparing `molgenis-emx2-ontomanager-0.2.8/demos/demo_search.py` & `molgenis-emx2-ontomanager-0.2.9/demos/demo_search.py`

 * *Files identical despite different names*

### Comparing `molgenis-emx2-ontomanager-0.2.8/dev/dev_csv_upload.py` & `molgenis-emx2-ontomanager-0.2.9/dev/dev_csv_upload.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,26 +38,32 @@
         password = os.environ.get('MG_PASSWORD')
 
     manager = OntologyManager(url, username, password)
 
     countries = pd.read_csv('data/Countries.csv')
     update_df = pd.read_csv('data/update.csv')
 
+    print(manager.ontology_tables)
+    server_countries = manager.list_ontology_terms('Countries', fmt='DataFrame')
+    print(server_countries)
+
     # Add the terms from the countries table to the Countries ontology table on the server
     # try:
     #     manager.add(table='Countries', data=countries)
     # except DuplicateKeyException:
     #     pass
-    mutations = manager.add(table='Countries', data=countries)
+    additions = manager.add(table='Countries', data=countries)
+    print(additions)
 
     # Update the references to the countries in the update_df dataset sequentially
-    manager.update(table='Countries', data=update_df)
+    # manager.update(table='Countries', data=update_df)
 
     # Delete the countries that were previously added from the Countries ontology table
-    manager.delete(table='Countries', names=countries['name'].tolist())
+    deletions = manager.delete(table='Countries', names=countries['name'].tolist())
+    print(deletions)
 
 
 if __name__ == '__main__':
     logging.basicConfig(level='INFO')
     logging.getLogger("requests").setLevel(logging.WARNING)
     logging.getLogger("urllib3").setLevel(logging.WARNING)
     dev_csv_upload()
```

### Comparing `molgenis-emx2-ontomanager-0.2.8/dev/dev_ontomanager.py` & `molgenis-emx2-ontomanager-0.2.9/dev/dev_ontomanager.py`

 * *Files identical despite different names*

### Comparing `molgenis-emx2-ontomanager-0.2.8/dev/dev_search.py` & `molgenis-emx2-ontomanager-0.2.9/dev/dev_search.py`

 * *Files identical despite different names*

### Comparing `molgenis-emx2-ontomanager-0.2.8/pyproject.toml` & `molgenis-emx2-ontomanager-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `molgenis-emx2-ontomanager-0.2.8/src/molgenis_emx2_ontomanager/OntologyManager.py` & `molgenis-emx2-ontomanager-0.2.9/src/molgenis_emx2_ontomanager/OntologyManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,14 @@
                 self.delete(table, **kwargs)
             case 'update':
                 self.update(table, **kwargs)
 
     def add(self, table: str, data: pd.DataFrame | dict | list = None, **kwargs):
         """Add a term to an ontology table.
         """
-        mutations = dict()
         log.info(f"Adding to table {table}.")
 
         if table not in self.ontology_tables:
             raise NoSuchTableException(f"Table '{table}' not found in CatalogueOntologies.")
 
         if data is not None:
             if isinstance(data, pd.DataFrame):
@@ -106,17 +105,18 @@
         """Delete a term or a list of terms from an ontology."""
         log.info(f"Deleting from table {table}.")
 
         if table not in self.ontology_tables:
             raise NoSuchTableException(f"Table '{table}' not found in CatalogueOntologies.")
 
         if names:
-            self._delete_list(table, names)
+            mutations = self._delete_list(table, names)
         if name:
-            self._delete_term(table, name)
+            mutations = self._delete_term(table, name)
+        return mutations
 
     def search(self, term: str, find_usage: bool = False) -> str | dict | None:
         """
         Search for a term in the CatalogueOntologies table and return the table in which the term is present.
         @param term: the term that is looked for.
         @param find_usage: if this is true, the rows of the tables where the term is used are returned, default False
         @return: a string of the table where the table is found, None if the term is not found
@@ -195,19 +195,19 @@
 
         query = Queries.insert(_table)
         variables = {"value": _kwargs}
 
         try:
             response = self.__perform_query(query, variables, action='add')
         except DuplicateKeyException:
-            log.error(f"Term '{_kwargs['name']}' already present in table '{table}'")
-            return {'failure': f"Term '{_kwargs['name']}' already present in table '{table}'"}
+            log.error(f"Term '{_kwargs['name']}' already present in table '{table}'.")
+            return {'failure': f"Term '{_kwargs['name']}' already present in table '{table}'."}
 
         mutation_id = generate_action_id(action=True)
-        return {mutation_id: _kwargs}
+        return {mutation_id: {'action': 'add', **_kwargs}}
 
     def _add_dict(self, table: str, terms_dict: dict) -> dict:
         """Add terms to a table from a dictionary object."""
         if 'name' in terms_dict.keys():
             mutations = self._add_term(table=table, kwargs=terms_dict)
         else:
             mutations = dict()
@@ -268,57 +268,71 @@
         for item in data:
             results.update(self._update_dict(table, item))
         return results
 
     def _update_term(self, ontology_table: str, old: str, new: str):
         log.info(f"Renaming in term '{old}' to '{new}' in table {ontology_table}.")
 
-        if old not in self.__list_ontology_terms(ontology_table):
+        if old not in self.list_ontology_terms(ontology_table).keys():
             raise NoSuchNameException(f"Name '{old}' not found in table '{ontology_table}'.")
-        if new not in self.__list_ontology_terms(ontology_table):
+        if new not in self.list_ontology_terms(ontology_table).keys():
             raise NoSuchNameException(f"Name '{new}' not found in table '{ontology_table}'.")
 
         updater = self.Updater(self, ontology_table, old, new)
         update_results = updater.update()
 
         return update_results
 
-    def _delete_list(self, table: str, terms: list, num_tries: int = 0):
+    def _delete_list(self, table: str, terms: list, num_tries: int = 0,
+                     mutations: dict = None) -> dict:
         """
         Delete the listed terms from the table.
         If one or more terms are referenced by another term, they are added
         to a list and deleted at a later stage.
         """
+        if mutations is None:
+            id_key = generate_action_id(action=False)
+            mutations = {id_key: {}}
+        else:
+            id_key = list(mutations.keys())[0]
+
         parent_terms = list()
         for term in terms:
             try:
-                self._delete_term(table, term)
+                mutations[id_key].update(self._delete_term(table, term))
             except ParentReferenceException:
                 parent_terms.append(term)
         if len(parent_terms) > 0:
             if num_tries > MAX_TRIES:
                 raise ParentReferenceException(f"Could not delete terms '{','.join(parent_terms)}' due to terms'"
                                                f"reference to parent term.")
-            self._delete_list(table, parent_terms, num_tries+1)
+            mutations = self._delete_list(table, parent_terms, num_tries+1, mutations=mutations)
+        return mutations
 
     def _delete_term(self, table: str, term: str):
         """Delete the term from the table."""
         _term = term
 
         _table = self.parse_table_name(table)
 
         query = Queries.delete(_table)
         variables = {"pkey": {'name': _term}}
 
-        if _term not in self.__list_ontology_terms(table):
+        terms_data = self.list_ontology_terms(table)
+        if _term not in terms_data.keys():
             raise NoSuchNameException(f"Name '{_term}' not found in table '{table}'.")
 
-        response = self.__perform_query(query, variables, action='delete')
+        try:
+            response = self.__perform_query(query, variables, action='delete')
+        except NoSuchNameException:
+            log.error(f"Term '{_term}' could not be deleted from table '{table}' as it is not present there.")
+            return {'failure': f"Term '{_term}' not present in table '{table}'."}
 
-        return response
+        mutation_id = generate_action_id(action=True)
+        return {mutation_id: {'action': 'delete', 'name': _term, **terms_data[_term]}}
 
     class Updater:
         """Class that handles the update of the terms, ontology tables, databases and database tables."""
 
         def __init__(self, manager, ontology_table: str, old: str, new: str):
             self.ontology_table = ontology_table
             self.manager: OntologyManager = manager
@@ -460,25 +474,39 @@
                 raise ParentReferenceException(message)
             raise OntomanagerException(message)
         else:
             log.info(f"Successfully {verbs[1]} {variables[next(iter(variables))]['name']}.")
 
         return _response
 
-    def __list_ontology_terms(self, table: str) -> list:
+    def list_ontology_terms(self, table: str, fmt: str = 'dict') -> list | dict | pd.DataFrame:
         """Returns a list of the terms in the specified ontology.
         :param table: the name of the table from which the terms are requested.
+        :param fmt: the format in which the list of terms is returned.
+                    list, dict and DataFrame are supported
         """
         query = Queries.list_ontology_terms(table)
 
         response = self.client.session.post(
             self.graphql_endpoint,
             json={"query": query}
         )
-        terms = [term['name'] for term in response.json()['data'][table]]
+
+        terms = {
+            item.pop('name'): item
+            for item in response.json()['data'][table]
+        }
+
+        if fmt == 'dict':
+            return terms
+        elif fmt == 'list':
+            return list(terms.keys())
+        elif fmt == 'DataFrame':
+            terms_df = pd.DataFrame.from_dict(terms, orient='index')
+            return terms_df
         return terms
 
     def __list_ontology_tables(self) -> list:
         """Returns a list of ontology tables in the CatalogueOntologies database."""
         query = Queries.list_ontology_tables()
         response = self.client.session.post(
             self.graphql_endpoint,
```

### Comparing `molgenis-emx2-ontomanager-0.2.8/src/molgenis_emx2_ontomanager/__main__.py` & `molgenis-emx2-ontomanager-0.2.9/src/molgenis_emx2_ontomanager/__main__.py`

 * *Files identical despite different names*

### Comparing `molgenis-emx2-ontomanager-0.2.8/src/molgenis_emx2_ontomanager/exceptions.py` & `molgenis-emx2-ontomanager-0.2.9/src/molgenis_emx2_ontomanager/exceptions.py`

 * *Files identical despite different names*

### Comparing `molgenis-emx2-ontomanager-0.2.8/src/molgenis_emx2_ontomanager/graphql_queries.py` & `molgenis-emx2-ontomanager-0.2.9/src/molgenis_emx2_ontomanager/graphql_queries.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,14 +49,23 @@
         Query to list the terms in an ontology.
         :param table: the name of the table from which the list is requested.
         """
         query = """
         {
           """ + table + """ {
             name
+            order
+            label
+            parent {
+              name
+            }
+            codesystem
+            code
+            ontologyTermURI
+            definition
           }
         }
         """
         return query
 
     @staticmethod
     def list_databases() -> str:
```

### Comparing `molgenis-emx2-ontomanager-0.2.8/src/molgenis_emx2_ontomanager/utils.py` & `molgenis-emx2-ontomanager-0.2.9/src/molgenis_emx2_ontomanager/utils.py`

 * *Files identical despite different names*

### Comparing `molgenis-emx2-ontomanager-0.2.8/src/molgenis_emx2_ontomanager.egg-info/PKG-INFO` & `molgenis-emx2-ontomanager-0.2.9/src/molgenis_emx2_ontomanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgenis-emx2-ontomanager
-Version: 0.2.8
+Version: 0.2.9
 Summary: Tool to manage catalogue ontologies on Molgenis EMX2 servers.
 Project-URL: Homepage, https://github.com/molgenis/molgenis-emx2
 Project-URL: Bug Tracker, https://github.com/molgenis/molgenis-emx2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `molgenis-emx2-ontomanager-0.2.8/src/molgenis_emx2_ontomanager.egg-info/SOURCES.txt` & `molgenis-emx2-ontomanager-0.2.9/src/molgenis_emx2_ontomanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

