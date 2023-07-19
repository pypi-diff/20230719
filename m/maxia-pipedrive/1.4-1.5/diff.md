# Comparing `tmp/maxia_pipedrive-1.4.tar.gz` & `tmp/maxia_pipedrive-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxia_pipedrive-1.4.tar", last modified: Mon Jul 17 14:21:09 2023, max compression
+gzip compressed data, was "maxia_pipedrive-1.5.tar", last modified: Wed Jul 19 11:06:06 2023, max compression
```

## Comparing `maxia_pipedrive-1.4.tar` & `maxia_pipedrive-1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-17 14:21:09.541003 maxia_pipedrive-1.4/
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     1073 2023-07-17 12:47:40.000000 maxia_pipedrive-1.4/LICENSE
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      730 2023-07-17 14:21:09.542994 maxia_pipedrive-1.4/PKG-INFO
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       95 2023-07-17 14:14:03.000000 maxia_pipedrive-1.4/README.md
-drwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-17 14:21:08.708790 maxia_pipedrive-1.4/maxia_pipedrive/
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      595 2023-07-17 13:58:38.000000 maxia_pipedrive-1.4/maxia_pipedrive/__init__.py
-drwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-17 14:21:09.500868 maxia_pipedrive-1.4/maxia_pipedrive/api_handler/
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/api_handler/__init__.py
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)    14893 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/api_handler/deals.py
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     1092 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/api_handler/fields.py
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     2388 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/api_handler/followers.py
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      166 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/api_handler/handler.py
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     8012 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/api_handler/organizations.py
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     1979 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/api_handler/persons.py
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     2064 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/api_handler/products.py
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      193 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/api_handler/stages.py
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      190 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/api_handler/users.py
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)    20937 2023-07-17 13:12:38.000000 maxia_pipedrive-1.4/maxia_pipedrive/api_handler/utils.py
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     2553 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/consts.py
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)    15815 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/data_handler.py
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)    10682 2023-07-17 13:18:46.000000 maxia_pipedrive-1.4/maxia_pipedrive/models.py
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     4835 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/relations.py
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       36 2023-07-17 12:09:16.000000 maxia_pipedrive-1.4/maxia_pipedrive/tests.py
-drwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-17 14:21:08.919899 maxia_pipedrive-1.4/maxia_pipedrive.egg-info/
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      730 2023-07-17 14:21:07.000000 maxia_pipedrive-1.4/maxia_pipedrive.egg-info/PKG-INFO
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      827 2023-07-17 14:21:08.000000 maxia_pipedrive-1.4/maxia_pipedrive.egg-info/SOURCES.txt
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        1 2023-07-17 14:21:07.000000 maxia_pipedrive-1.4/maxia_pipedrive.egg-info/dependency_links.txt
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       18 2023-07-17 14:21:07.000000 maxia_pipedrive-1.4/maxia_pipedrive.egg-info/requires.txt
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       16 2023-07-17 14:21:07.000000 maxia_pipedrive-1.4/maxia_pipedrive.egg-info/top_level.txt
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       79 2023-07-17 14:21:09.553974 maxia_pipedrive-1.4/setup.cfg
--rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     1799 2023-07-17 14:20:55.000000 maxia_pipedrive-1.4/setup.py
+drwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-19 11:06:06.317741 maxia_pipedrive-1.5/
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     1073 2023-07-17 12:47:40.000000 maxia_pipedrive-1.5/LICENSE
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      730 2023-07-19 11:06:06.319738 maxia_pipedrive-1.5/PKG-INFO
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      274 2023-07-18 08:31:31.000000 maxia_pipedrive-1.5/README.md
+drwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-19 11:06:05.356910 maxia_pipedrive-1.5/maxia_pipedrive/
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      595 2023-07-17 13:58:38.000000 maxia_pipedrive-1.5/maxia_pipedrive/__init__.py
+drwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-19 11:06:06.253735 maxia_pipedrive-1.5/maxia_pipedrive/api_handler/
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-17 12:09:16.000000 maxia_pipedrive-1.5/maxia_pipedrive/api_handler/__init__.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)    14919 2023-07-19 09:58:37.000000 maxia_pipedrive-1.5/maxia_pipedrive/api_handler/deals.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     1092 2023-07-17 12:09:16.000000 maxia_pipedrive-1.5/maxia_pipedrive/api_handler/fields.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     2388 2023-07-17 12:09:16.000000 maxia_pipedrive-1.5/maxia_pipedrive/api_handler/followers.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      166 2023-07-17 12:09:16.000000 maxia_pipedrive-1.5/maxia_pipedrive/api_handler/handler.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     8085 2023-07-19 09:59:55.000000 maxia_pipedrive-1.5/maxia_pipedrive/api_handler/organizations.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     1979 2023-07-17 12:09:16.000000 maxia_pipedrive-1.5/maxia_pipedrive/api_handler/persons.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     2064 2023-07-17 12:09:16.000000 maxia_pipedrive-1.5/maxia_pipedrive/api_handler/products.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      193 2023-07-17 12:09:16.000000 maxia_pipedrive-1.5/maxia_pipedrive/api_handler/stages.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      190 2023-07-17 12:09:16.000000 maxia_pipedrive-1.5/maxia_pipedrive/api_handler/users.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)    21405 2023-07-19 09:59:47.000000 maxia_pipedrive-1.5/maxia_pipedrive/api_handler/utils.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     2553 2023-07-17 12:09:16.000000 maxia_pipedrive-1.5/maxia_pipedrive/consts.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)    15817 2023-07-19 09:53:37.000000 maxia_pipedrive-1.5/maxia_pipedrive/data_handler.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)    10682 2023-07-17 13:18:46.000000 maxia_pipedrive-1.5/maxia_pipedrive/models.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     4863 2023-07-19 09:53:37.000000 maxia_pipedrive-1.5/maxia_pipedrive/relations.py
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       36 2023-07-17 12:09:16.000000 maxia_pipedrive-1.5/maxia_pipedrive/tests.py
+drwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        0 2023-07-19 11:06:05.616909 maxia_pipedrive-1.5/maxia_pipedrive.egg-info/
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      730 2023-07-19 11:06:04.000000 maxia_pipedrive-1.5/maxia_pipedrive.egg-info/PKG-INFO
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)      827 2023-07-19 11:06:04.000000 maxia_pipedrive-1.5/maxia_pipedrive.egg-info/SOURCES.txt
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)        1 2023-07-19 11:06:04.000000 maxia_pipedrive-1.5/maxia_pipedrive.egg-info/dependency_links.txt
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       18 2023-07-19 11:06:04.000000 maxia_pipedrive-1.5/maxia_pipedrive.egg-info/requires.txt
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       16 2023-07-19 11:06:04.000000 maxia_pipedrive-1.5/maxia_pipedrive.egg-info/top_level.txt
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)       79 2023-07-19 11:06:06.333757 maxia_pipedrive-1.5/setup.cfg
+-rwxrwxrwx   0 luizpinheiro  (1000) luizpinheiro  (1000)     1805 2023-07-19 09:55:45.000000 maxia_pipedrive-1.5/setup.py
```

### Comparing `maxia_pipedrive-1.4/LICENSE` & `maxia_pipedrive-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `maxia_pipedrive-1.4/PKG-INFO` & `maxia_pipedrive-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: maxia_pipedrive
-Version: 1.4
+Version: 1.5
 Summary: Maxia Pipedrive API handler
 Home-page: https://github.com/Max-ia-Education/maxia_pipedrive_api
 Author: Max.ia Education
 Author-email: luiz@maxia.education
 License: MIT
-Download-URL: https://github.com/Max-ia-Education/maxia_pipedrive_api/archive/refs/tags/v1.3.tar.gz
+Download-URL: https://github.com/Max-ia-Education/maxia_pipedrive_api/archive/refs/tags/v1.5.tar.gz
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `maxia_pipedrive-1.4/maxia_pipedrive/__init__.py` & `maxia_pipedrive-1.5/maxia_pipedrive/__init__.py`

 * *Files identical despite different names*

### Comparing `maxia_pipedrive-1.4/maxia_pipedrive/api_handler/deals.py` & `maxia_pipedrive-1.5/maxia_pipedrive/api_handler/deals.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,31 +22,31 @@
         p['owner_id'] = p['owner_id']['value']
         p['org_id'] = p['org_id']['value']
 all_persons = pd.DataFrame(all_persons)  # [['id', 'org_id']]
 org_people_dict = all_persons.groupby('org_id')['id'].apply(list).to_dict()
 
 
 def get_all_deals(**query_params_dict):
-    print('Get all deals...')
+    # print('Get all deals...')
     return maxia_pipedrive.api_handler.utils.get_all_request(
         maxia_pipedrive.consts.Endpoints.deals,
         **query_params_dict
     )
 
 
 def cascade_following(list_deal_id, save=True, list_output_files=[], all_deals_data=None):
     # Each deal id is associated to an organization and may have an sdr assigned
     if all_deals_data is None:
         all_deals_data = get_all_deals()
     deal_id_deal_dict = {
         org_dict['id']: org_dict
         for org_dict in all_deals_data
     }
-    print(json.dumps({k: deal_id_deal_dict[k]
-          for k in list_deal_id[:5]}, indent=1))
+    # print(json.dumps({k: deal_id_deal_dict[k]
+        #   for k in list_deal_id[:5]}, indent=1))
     deal_id_deal_sdr_id = {
         did: (deal_id_deal_dict[did][maxia_pipedrive.models.Deal.get_api_code(
             maxia_pipedrive.models.Deal.assigned_sdr)] if isinstance(deal_id_deal_dict[did][maxia_pipedrive.models.Deal.get_api_code(
                 maxia_pipedrive.models.Deal.assigned_sdr)], int) else deal_id_deal_dict[did][maxia_pipedrive.models.Deal.get_api_code(
                     maxia_pipedrive.models.Deal.assigned_sdr)][maxia_pipedrive.consts.Consts.id])
         for did in list_deal_id
         if deal_id_deal_dict[did][maxia_pipedrive.models.Deal.get_api_code(maxia_pipedrive.models.Deal.assigned_sdr)] is not None
@@ -122,24 +122,24 @@
             maxia_pipedrive.consts.Consts.user_id: deal_id_deal_owner_id.get(did)
         }
         for did in list_deal_id
         for pid in org_people_dict.get(str(deal_id_org_id.get(did)), [])
     ]
 
 # The deal must be followed by the respective SDR
-    print('Adding followers to DEALS')
+    # print('Adding followers to DEALS')
     list_output_files.append(maxia_pipedrive.api_handler.followers.add_follower_to_multiple_deals(
         deal_following_list, save=save
     ))
-    print('Adding Followers to ORGANIZATIONS')
+    # print('Adding Followers to ORGANIZATIONS')
     # The organization must be followed by the respective SDR and Consultor
     list_output_files.append(maxia_pipedrive.api_handler.followers.add_follower_to_multiple_organization(
         org_following_list, save=save
     ))
-    print('Adding Followers to PERSONS')
+    # print('Adding Followers to PERSONS')
     # The persons from each organization must be followed by the respective SDR and Consultor
     list_output_files.append(maxia_pipedrive.api_handler.followers.add_follower_to_multiple_persons(
         persons_following_list, save=save
 
     ))
     return list_output_files
 
@@ -180,15 +180,15 @@
     if save:
         list_output_files.append(maxia_pipedrive.api_handler.utils.save_migration(
             maxia_pipedrive.consts.MigrationMethods.create, maxia_pipedrive.consts.MigrationKind.deal, list_created_deals))
     else:
         list_output_files.append(list_created_deals)
     if cascade:
         # Then, cascade the following
-        print('Cascading followers')
+        # print('Cascading followers')
         with open(list_output_files[0], 'r') as f:
             migration_data = json.load(f)
             list_deal_id = [d[maxia_pipedrive.consts.Consts.details][maxia_pipedrive.consts.Consts.id]
                             for d in migration_data]
             cascade_following(
                 list_deal_id,
                 save=True,
@@ -287,16 +287,16 @@
     list_migration_fpath = []
     for stp in range(n_steps):
         timestp = datetime.now().strftime(maxia_pipedrive.consts.Consts.date_format)
         migration_fpath = join(
             maxia_pipedrive.consts.Consts.migrations_dir,
             f'update_multidealid_{timestp}_{stp+1}-{n_steps}.json')
         list_migration_fpath.append(migration_fpath)
-        print(
-            f'[{stp+1}/{n_steps}] Starting updates... Saving migration file on: {migration_fpath}')
+        # print(
+            # f'[{stp+1}/{n_steps}] Starting updates... Saving migration file on: {migration_fpath}')
         list_migration_dict = []
         try:
             for deal_id, update_dict in tqdm(zip(list_deal_id[stp * step_size:(stp + 1) * step_size],
                                                  list_update_dict[stp * step_size:(stp + 1) * step_size]),
                                              total=len(list_deal_id[stp * step_size:(stp + 1) * step_size])):
                 migration_dict = update_deal(
                     int(deal_id),  # must be int
@@ -315,25 +315,25 @@
                 maxia_pipedrive.api_handler.utils.revert_migrations_from_path(
                     migration_fpath)
                 list_migration_fpath.remove(migration_fpath)
                 return list_migration_fpath
 
         # Save massive step migration
 
-        print(
-            f'Migration step done! Saving step migration file: {migration_fpath}')
+        # print(
+            # f'Migration step done! Saving step migration file: {migration_fpath}')
         with open(migration_fpath, 'w', encoding='utf-8') as f:
             json.dump(list_migration_dict, f, indent=1)
 
     # At the end of the loop, with no exception found, we proceed by merging all files into a single file
     all_migration_fpath = join(
         maxia_pipedrive.consts.Consts.migrations_dir,
         f'update_multidealid_{timestp}.json')
-    print(
-        f'Saving all migrations into a single file: {all_migration_fpath} ...')
+    # print(
+        # f'Saving all migrations into a single file: {all_migration_fpath} ...')
     merged_migration_list_dict = []
     for migration_fpath in list_migration_fpath:
         with open(migration_fpath, 'r', encoding='utf-8') as f:
             merged_migration_list_dict += json.load(f)
         remove(migration_fpath)
     # Save into a single file:
     with open(
```

### Comparing `maxia_pipedrive-1.4/maxia_pipedrive/api_handler/fields.py` & `maxia_pipedrive-1.5/maxia_pipedrive/api_handler/fields.py`

 * *Files identical despite different names*

### Comparing `maxia_pipedrive-1.4/maxia_pipedrive/api_handler/followers.py` & `maxia_pipedrive-1.5/maxia_pipedrive/api_handler/followers.py`

 * *Files identical despite different names*

### Comparing `maxia_pipedrive-1.4/maxia_pipedrive/api_handler/organizations.py` & `maxia_pipedrive-1.5/maxia_pipedrive/api_handler/organizations.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 # GET functions
 
 
 def get_organization(org_id):
     return maxia_pipedrive.api_handler.utils.get_request(f'{maxia_pipedrive.consts.Endpoints.organizations}/{org_id}')
 
 
-def get_all_organizations(**query_params_dict):
-    print('Loading all organizations...')
+def get_all_organizations(output_fields=None, **query_params_dict):
+    # print('Loading all organizations...')
     return maxia_pipedrive.api_handler.utils.get_all_request(
         maxia_pipedrive.consts.Endpoints.organizations,
+        output_fields=output_fields,
         **query_params_dict
     )
 
 
 # PUT (update) Functions
 
 
@@ -76,16 +77,16 @@
     list_migration_fpath = []
     for stp in range(n_steps):
         timestp = datetime.now().strftime(maxia_pipedrive.consts.Consts.date_format)
         migration_fpath = join(
             maxia_pipedrive.consts.Consts.migrations_dir,
             f'update_multiorgid_{timestp}_{stp+1}-{n_steps}.json')
         list_migration_fpath.append(migration_fpath)
-        print(
-            f'[{stp+1}/{n_steps}] Starting updates... Saving migration file on: {migration_fpath}')
+        # print(
+            # f'[{stp+1}/{n_steps}] Starting updates... Saving migration file on: {migration_fpath}')
         list_migration_dict = []
         try:
             for org_id, update_dict in tqdm(zip(list_org_id[stp * step_size:(stp + 1) * step_size],
                                                 list_update_dict[stp * step_size:(stp + 1) * step_size]),
                                             total=len(list_org_id[stp * step_size:(stp + 1) * step_size])):
                 migration_dict = update_organization(
                     int(org_id),  # must be int
@@ -104,25 +105,25 @@
                 maxia_pipedrive.api_handler.utils.revert_migrations_from_path(
                     migration_fpath)
                 list_migration_fpath.remove(migration_fpath)
                 return list_migration_fpath
 
         # Save massive step migration
 
-        print(
-            f'Migration step done! Saving step migration file: {migration_fpath}')
+        # print(
+            # f'Migration step done! Saving step migration file: {migration_fpath}')
         with open(migration_fpath, 'w', encoding='utf-8') as f:
             json.dump(list_migration_dict, f, indent=1)
 
     # At the end of the loop, with no exception found, we proceed by merging all files into a single file
     all_migration_fpath = join(
         maxia_pipedrive.consts.Consts.migrations_dir,
         f'update_multiorgid_{timestp}.json')
-    print(
-        f'Saving all migrations into a single file: {all_migration_fpath} ...')
+    # print(
+        # f'Saving all migrations into a single file: {all_migration_fpath} ...')
     merged_migration_list_dict = []
     for migration_fpath in list_migration_fpath:
         with open(migration_fpath, 'r', encoding='utf-8') as f:
             merged_migration_list_dict += json.load(f)
         remove(migration_fpath)
     # Save into a single file:
     with open(
@@ -178,14 +179,14 @@
     #     el for el in list_org_dict if el[inep_api_code] not in inep_id_dict.keys()]
     # # Add default owner if
     # for el in validated_list_org_dict:
     #     owner_id_code = maxia_pipedrive_src.models.Organization.get_api_code_dict()[maxia_pipedrive_src.models.Organization.owner_id]
     #     el[owner_id_code] = el.get(owner_id_code, 12127564)
 
     # if len(list_org_dict) != len(validated_list_org_dict):
-    #     print(
+    #     # print(
     #         f'{len(list_org_dict)-len(validated_list_org_dict)} organization already exist. Skipping...')
     # return maxia_pipedrive_src.api_handler.utils.multiple_post_request(
     #     maxia_pipedrive_src.consts.Endpoints.organizations,
     #     validated_list_org_dict,
     #     maxia_pipedrive_src.consts.MigrationKind.multiple_orgs,
     #     save=save)
```

### Comparing `maxia_pipedrive-1.4/maxia_pipedrive/api_handler/persons.py` & `maxia_pipedrive-1.5/maxia_pipedrive/api_handler/persons.py`

 * *Files identical despite different names*

### Comparing `maxia_pipedrive-1.4/maxia_pipedrive/api_handler/products.py` & `maxia_pipedrive-1.5/maxia_pipedrive/api_handler/products.py`

 * *Files identical despite different names*

### Comparing `maxia_pipedrive-1.4/maxia_pipedrive/api_handler/utils.py` & `maxia_pipedrive-1.5/maxia_pipedrive/api_handler/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     timestp = datetime.now().strftime(maxia_pipedrive.consts.Consts.date_format)
     if obj_id is not None:
         filename = f'{method_}_{migration_kind}_{obj_id}_{timestp}.json'
     else:
         filename = f'{method_}_{migration_kind}_{timestp}.json'
     migration_fpath = join(
         maxia_pipedrive.consts.Consts.migrations_dir, filename)
-    print(f'Updated! Saving migration file: {migration_fpath}')
+    # print(f'Updated! Saving migration file: {migration_fpath}')
     with open(migration_fpath, 'w', encoding='utf-8') as f:
         json.dump(migration_dict, f, indent=1)
     return migration_fpath
 
 
 def prepare_batch_multiple_post(list_json_data, step_size=100):
     n_steps = int(np.ceil(len(list_json_data)/step_size))
@@ -123,46 +123,46 @@
 def revert_migrations_from_path(migration_fpath, save=False):
     with open(migration_fpath, 'r', encoding='utf-8') as f:
         migrations = json.load(f)
         if isinstance(migrations, dict):
             migrations = [migrations]
 
     list_reverse_migration, any_error = revert_migrations(migrations)
-    if any_error:
-        print('Check the moved file for more details about the error!')
+    # if any_error:
+        # print('Check the moved file for more details about the error!')
     filename = migration_fpath.split('/')[1]
     moved_migration_fpath = join(
         maxia_pipedrive.consts.Consts.reversed_migrations,
         filename
     )
-    print(
-        f'Moving reversed migration file from {migration_fpath} to {moved_migration_fpath}')
+    # print(
+        # f'Moving reversed migration file from {migration_fpath} to {moved_migration_fpath}')
     move(
         migration_fpath,
         moved_migration_fpath
     )
     if save:
         # output_fpath = ".".join(moved_migration_fpath.split('.')[:-1]) + "_reversion.json"
         output_fpath = join(
             maxia_pipedrive.consts.Consts.reversed_migrations, "reversion_"+filename)
-        print(f'Reversed! Saving reversion file: {output_fpath}')
+        # print(f'Reversed! Saving reversion file: {output_fpath}')
         with open(output_fpath, 'w', encoding='utf-8') as f:
             json.dump(list_reverse_migration, f, indent=1)
         return output_fpath
     return list_reverse_migration
 
 # SINGLE
 
 
 def get_request(endpoint):
     req = requests.get(join(API_URL, endpoint), params=API_TOKEN)
     if req.status_code == 200 and req.json()['success']:
         return req.json()['data']
     else:
-        print(join(API_URL, endpoint), req.status_code)
+        # print(join(API_URL, endpoint), req.status_code)
         return []
 
 
 def post_request(endpoint, json_data, migration_kind, save=False):
     migration_dict = {
         'endpoint': endpoint,
         'method': 'post',
@@ -171,17 +171,17 @@
     }
     req = requests.post(
         join(API_URL, endpoint),
         params=API_TOKEN,
         json=json_data
     )
     if not (200 <= req.status_code < 300):
-        print(f'Request failed! status={req.status_code}')
-        print(req.content)
-        print('input:', migration_dict)
+        # print(f'Request failed! status={req.status_code}')
+        # print(req.content)
+        # print('input:', migration_dict)
         return {}
     req = req.json()
 
     if req['success'] is True:
         obj_id = req['data']['id']
         json_data['id'] = obj_id
         if save:
@@ -256,15 +256,15 @@
     else:
         migration_dict = {
             maxia_pipedrive.consts.Consts.endpoint: endpoint,
             maxia_pipedrive.consts.Consts.method: 'put',
             maxia_pipedrive.consts.Consts.migration_kind: migration_kind,
             maxia_pipedrive.consts.Consts.details: validated_update_dict
         }
-        print(migration_dict)
+        # print(migration_dict)
     req = requests.put(
         join(API_URL, endpoint),
         params=API_TOKEN,
         json=validated_update_dict
     )
     if req.status_code != 200:
         print('Request failed!')
@@ -299,34 +299,47 @@
     return {}
 
 # MULTIPLE
 
 # def multiple_update_request(list_endpoint, list_json_data, migration_kind)
 
 
-def get_all_request(endpoint, verbose=False, **query_params_dict):
+def get_all_request(endpoint, verbose=False, output_fields=None, **query_params_dict):
     query_params_str = get_query_params(query_params_dict)
     list_data = []
     next_start = 0
     while next_start is not None:
         req = requests.get(
             join(API_URL, endpoint +
                  f"?{query_params_str}&limit=5000&start={next_start}"),
             params=API_TOKEN
         )
         if req.status_code == 200:
             if req.json()['data'] is not None:
-                list_data += req.json()['data']
+                data = req.json()['data']
+                # Column filtering if asked
+                if output_fields is not None:
+                    data = [
+                        {
+                            k: v
+                            for k, v in el.items()
+                            if k in output_fields
+                        }
+
+                        for el in data
+                    ]
+
+                list_data += data
             next_start = req.json()['additional_data']['pagination'].get(
                 'next_start', None)
         else:
             next_start = None
-            print(req.text)
-        if verbose:
-            print(f'\tFetched {len(list_data)} from {endpoint}...')
+            # print(req.text)
+        # if verbose:
+            # print(f'\tFetched {len(list_data)} from {endpoint}...')
     return list_data
 
 
 def multiple_post_request(endpoint, list_json_data, migration_kind, save=True):
     list_migration_dict = []
     try:
         for json_data in tqdm(list_json_data):
@@ -449,16 +462,16 @@
     list_migration_fpath = []
     for stp in range(n_steps):
         timestp = datetime.now().strftime(maxia_pipedrive.consts.Consts.date_format)
         migration_fpath = os.path.join(
             maxia_pipedrive.consts.Consts.migrations_dir,
             f'update_{obj_migration_kind}_{timestp}_{stp+1}-{n_steps}.json')
         list_migration_fpath.append(migration_fpath)
-        print(
-            f'[{stp+1}/{n_steps}] Starting updates... Saving migration file on: {migration_fpath}')
+        # print(
+            # f'[{stp+1}/{n_steps}] Starting updates... Saving migration file on: {migration_fpath}')
         list_migration_dict = []
         try:
             for obj_id, update_dict in tqdm(zip(list_obj_id[stp * step_size:(stp + 1) * step_size],
                                                 list_update_dict[stp * step_size:(stp + 1) * step_size]),
                                             total=len(list_obj_id[stp * step_size:(stp + 1) * step_size])):
                 migration_dict = update_obj_func(
                     int(obj_id),  # must be int
@@ -476,26 +489,26 @@
                 print('Got exception while updating... Reverting migration')
                 revert_migrations_from_path(migration_fpath)
                 list_migration_fpath.remove(migration_fpath)
                 return list_migration_fpath
 
         # Save massive step migration
 
-        print(
-            f'Migration step done! Saving step migration file: {migration_fpath}')
+        # print(
+            # f'Migration step done! Saving step migration file: {migration_fpath}')
         with open(migration_fpath, 'w', encoding='utf-8') as f:
             json.dump(list_migration_dict, f, indent=1)
 
     # At the end of the loop, with no exception found, we proceed by merging all files into a single file
     if save:
         all_migration_fpath = join(
             maxia_pipedrive.consts.Consts.migrations_dir,
             f'update_{obj_migration_kind}_{timestp}.json')
-        print(
-            f'Saving all migrations into a single file: {all_migration_fpath} ...')
+        # print(
+            # f'Saving all migrations into a single file: {all_migration_fpath} ...')
     merged_migration_list_dict = []
     for migration_fpath in list_migration_fpath:
         with open(migration_fpath, 'r', encoding='utf-8') as f:
             merged_migration_list_dict += json.load(f)
         os.remove(migration_fpath)
     if save:
         # Save into a single file:
@@ -535,16 +548,16 @@
     list_migration_fpath = []
     for stp in range(n_steps):
         timestp = datetime.now().strftime(maxia_pipedrive.consts.Consts.date_format)
         migration_fpath = os.path.join(
             maxia_pipedrive.consts.Consts.migrations_dir,
             f'create_{obj_migration_kind}_{timestp}_{stp+1}-{n_steps}.json')
         list_migration_fpath.append(migration_fpath)
-        print(
-            f'[{stp+1}/{n_steps}] Starting updates... Saving migration file on: {migration_fpath}')
+        # print(
+            # f'[{stp+1}/{n_steps}] Starting updates... Saving migration file on: {migration_fpath}')
         list_migration_dict = []
         try:
             for create_obj_dict in tqdm(list_obj_dict[stp * step_size:(stp + 1) * step_size],
                                         total=len(list_obj_dict[stp * step_size:(stp + 1) * step_size])):
                 migration_dict = create_obj_func(
                     create_obj_dict,
                     save=False)
@@ -559,26 +572,26 @@
                 print('Got exception while updating... Reverting migration')
                 revert_migrations_from_path(migration_fpath)
                 list_migration_fpath.remove(migration_fpath)
                 return list_migration_fpath
 
         # Save massive step migration
 
-        print(
-            f'Migration step done! Saving step migration file: {migration_fpath}')
+        # print(
+            # f'Migration step done! Saving step migration file: {migration_fpath}')
         with open(migration_fpath, 'w', encoding='utf-8') as f:
             json.dump(list_migration_dict, f, indent=1)
 
     # At the end of the loop, with no exception found, we proceed by merging all files into a single file
     if save:
         all_migration_fpath = join(
             maxia_pipedrive.consts.Consts.migrations_dir,
             f'create_{obj_migration_kind}_{timestp}.json')
-        print(
-            f'Saving all migrations into a single file: {all_migration_fpath} ...')
+        # print(
+            # f'Saving all migrations into a single file: {all_migration_fpath} ...')
     merged_migration_list_dict = []
     for migration_fpath in list_migration_fpath:
         with open(migration_fpath, 'r', encoding='utf-8') as f:
             merged_migration_list_dict += json.load(f)
         os.remove(migration_fpath)
     if save:
         # Save into a single file:
```

### Comparing `maxia_pipedrive-1.4/maxia_pipedrive/consts.py` & `maxia_pipedrive-1.5/maxia_pipedrive/consts.py`

 * *Files identical despite different names*

### Comparing `maxia_pipedrive-1.4/maxia_pipedrive/data_handler.py` & `maxia_pipedrive-1.5/maxia_pipedrive/data_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         6123009000176: 7439904000167,  # COLÉGIO CÔNEGO: 7439904000167
         5833836000190: 14875519000128,  # CESA: 14875519000128
         17217670001562: 17217670000167,  # COLÉGIO BATISTA MINEIRO: 17217670000167
         36583288000111: 30704905000103  # COLÉGIO M2 - VESPASIANO: 30704905000103
     }, inplace=True)
     df_base = df_base[['Escola', 'Razão Social',	'CNPJ', 'Status']].merge(
         load_inep_cleaned(), on='CNPJ')
-    # print(df_base[~df_base[Organization.cnpj].isin(inep_cleaned[Organization.cnpj].to_list())])
+    # # print(df_base[~df_base[Organization.cnpj].isin(inep_cleaned[Organization.cnpj].to_list())])
     df_base = df_base[['Escola', 'Nome', 'Razão Social', 'CNPJ',
                        maxia_pipedrive.models.Organization.inep_number, 'Razão Social',	'Cidade',	'UF',	'Status']]
     df_base.to_excel('data/microdados_treated/BASE_CLIENTES_2022_v1.xlsx')
     return df_base
 
 
 def preprocess_roberta_wallet():
```

### Comparing `maxia_pipedrive-1.4/maxia_pipedrive/models.py` & `maxia_pipedrive-1.5/maxia_pipedrive/models.py`

 * *Files identical despite different names*

### Comparing `maxia_pipedrive-1.4/maxia_pipedrive/relations.py` & `maxia_pipedrive-1.5/maxia_pipedrive/relations.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         org_dict = maxia_pipedrive.api_handler.organizations.get_organization(org_id)
         id_inep_dict = {
             org_dict[maxia_pipedrive.models.Organization.get_api_code_dict(
             )[maxia_pipedrive.models.Organization.inep_number]]: org_dict['id']
         }
     if save:
         timestp = datetime.now().strftime(dateformat)
-        print(len(id_inep_dict))
+        # # print(len(id_inep_dict))
         with open(f'data/relations/orgid_inep_{timestp}.json', 'w', encoding='utf-8') as f:
             json.dump(id_inep_dict, f, indent=1)
     return id_inep_dict
 
 
 def fetch_orgfieldinfo_reference(save=True):
     data = None
@@ -42,45 +42,45 @@
         data = maxia_pipedrive.api_handler.fields.get_all_org_field_info()
     key_id_dict = {
         field_dict['key']: field_dict
         for field_dict in data
     }
     if save:
         timestp = datetime.now().strftime(dateformat)
-        print(len(key_id_dict))
+        # # print(len(key_id_dict))
         with open(f'data/relations/{maxia_pipedrive.consts.Relations.orgfieldinfo}_{timestp}.json', 'w', encoding='utf-8') as f:
             json.dump(key_id_dict, f, indent=1)
 
 
 def fetch_dealfieldinfo_reference(save=True):
     data = None
     if data is None:
         data = maxia_pipedrive.api_handler.fields.get_all_deal_field_info()
     key_id_dict = {
         field_dict['key']: field_dict
         for field_dict in data
     }
     if save:
         timestp = datetime.now().strftime(dateformat)
-        print(len(key_id_dict))
+        # # print(len(key_id_dict))
         with open(f'data/relations/{maxia_pipedrive.consts.Relations.dealfieldinfo}_{timestp}.json', 'w', encoding='utf-8') as f:
             json.dump(key_id_dict, f, indent=1)
 
 
 def fetch_personfieldinfo_reference(save=True):
     data = None
     if data is None:
         data = maxia_pipedrive.api_handler.fields.get_all_person_field_info()
     key_id_dict = {
         field_dict['key']: field_dict
         for field_dict in data
     }
     if save:
         timestp = datetime.now().strftime(dateformat)
-        print(len(key_id_dict))
+        # # print(len(key_id_dict))
         with open(f'data/relations/{maxia_pipedrive.consts.Relations.personfieldinfo}_{timestp}.json', 'w', encoding='utf-8') as f:
             json.dump(key_id_dict, f, indent=1)
 
 
 def fetch_useralias_userid_reference(save=True):
     data = maxia_pipedrive.api_handler.users.get_all_users()
     name_email_id_dict = [
@@ -90,41 +90,41 @@
         }
         for user in data
     ]
     name_email_id_dict = {
         k: v for d in name_email_id_dict for k, v in d.items()}
     if save:
         timestp = datetime.now().strftime(dateformat)
-        print(len(name_email_id_dict))
+        # # print(len(name_email_id_dict))
         with open(f'data/relations/useralias_userid_{timestp}.json', 'w', encoding='utf-8') as f:
             json.dump(name_email_id_dict, f, indent=1)
 
 
 def fetch_stagealias_stageinfo_reference(save=True):
     data = maxia_pipedrive.api_handler.stages.get_all_stages()
     stagealias_stagedata = {
         stage['pipeline_name'] + "_" + stage['name']: stage
         for stage in data
     }
     if save:
         timestp = datetime.now().strftime(dateformat)
-        print(len(stagealias_stagedata))
+        # # print(len(stagealias_stagedata))
         with open(f'data/relations/stagealias_stageinfo_{timestp}.json', 'w', encoding='utf-8') as f:
             json.dump(stagealias_stagedata, f, indent=1)
 
 
 def fetch_products_info(save=True):
     data = maxia_pipedrive.api_handler.products.get_all_products()
     product_info = {
         prod['id']: prod['prices'][0]['price']
         for prod in data
     }
     if save:
         timestp = datetime.now().strftime(dateformat)
-        print(len(product_info))
+        # # print(len(product_info))
         with open(f'data/relations/products_info_{timestp}.json', 'w', encoding='utf-8') as f:
             json.dump(product_info, f, indent=1)
 
 
 if __name__ == '__main__':
     # fetch_id_inep_reference()
     # fetch_orgfieldinfo_reference(save=True)
```

### Comparing `maxia_pipedrive-1.4/maxia_pipedrive.egg-info/PKG-INFO` & `maxia_pipedrive-1.5/maxia_pipedrive.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: maxia-pipedrive
-Version: 1.4
+Version: 1.5
 Summary: Maxia Pipedrive API handler
 Home-page: https://github.com/Max-ia-Education/maxia_pipedrive_api
 Author: Max.ia Education
 Author-email: luiz@maxia.education
 License: MIT
-Download-URL: https://github.com/Max-ia-Education/maxia_pipedrive_api/archive/refs/tags/v1.3.tar.gz
+Download-URL: https://github.com/Max-ia-Education/maxia_pipedrive_api/archive/refs/tags/v1.5.tar.gz
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `maxia_pipedrive-1.4/maxia_pipedrive.egg-info/SOURCES.txt` & `maxia_pipedrive-1.5/maxia_pipedrive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maxia_pipedrive-1.4/setup.py` & `maxia_pipedrive-1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # from distutils.core import setup
 from setuptools import setup, find_packages
-version = '1.4'
+version = '1.5'
 setup(
     # How you named your package folder (MyLib)
     name='maxia_pipedrive',
     packages=find_packages(),   # Chose the same as "name"
     version=version,      # Start with a small number and increase it with every change you make
     # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     license='MIT',
     # Give a short description about your library
     description='Maxia Pipedrive API handler',
     author='Max.ia Education',                   # Type in your name
     author_email='luiz@maxia.education',      # Type in your E-Mail
     # Provide either the link to your github or to your website
     url='https://github.com/Max-ia-Education/maxia_pipedrive_api',
     # I explain this later on
-    download_url=f'https://github.com/Max-ia-Education/maxia_pipedrive_api/archive/refs/tags/v1.3.tar.gz',
+    download_url=f'https://github.com/Max-ia-Education/maxia_pipedrive_api/archive/refs/tags/v{version}.tar.gz',
     #   keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
     install_requires=[            # I get to this in a second
         'numpy',
         'pandas',
         'tqdm'
     ],
     classifiers=[
```

