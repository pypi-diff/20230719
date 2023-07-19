# Comparing `tmp/ckanext-metrics_dashboard-0.1.5.tar.gz` & `tmp/ckanext-metrics_dashboard-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-metrics_dashboard-0.1.5.tar", last modified: Mon Nov 28 17:12:10 2022, max compression
+gzip compressed data, was "ckanext-metrics_dashboard-0.1.6.tar", last modified: Wed Jul 19 15:09:08 2023, max compression
```

## Comparing `ckanext-metrics_dashboard-0.1.5.tar` & `ckanext-metrics_dashboard-0.1.6.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 17:12:10.556117 ckanext-metrics_dashboard-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (122)      110 2022-11-28 17:12:09.000000 ckanext-metrics_dashboard-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4208 2022-11-28 17:12:10.556117 ckanext-metrics_dashboard-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3143 2022-11-28 17:12:09.000000 ckanext-metrics_dashboard-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 17:12:10.552117 ckanext-metrics_dashboard-0.1.5/ckanext/
--rw-r--r--   0 runner    (1001) docker     (122)      200 2022-11-28 17:12:09.000000 ckanext-metrics_dashboard-0.1.5/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 17:12:10.552117 ckanext-metrics_dashboard-0.1.5/ckanext/metrics_dashboard/
--rw-r--r--   0 runner    (1001) docker     (122)      200 2022-11-28 17:12:09.000000 ckanext-metrics_dashboard-0.1.5/ckanext/metrics_dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      789 2022-11-28 17:12:09.000000 ckanext-metrics_dashboard-0.1.5/ckanext/metrics_dashboard/plugin.py
--rw-r--r--   0 runner    (1001) docker     (122)     5586 2022-11-28 17:12:09.000000 ckanext-metrics_dashboard-0.1.5/ckanext/metrics_dashboard/reports.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 17:12:10.552117 ckanext-metrics_dashboard-0.1.5/ckanext/metrics_dashboard/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 17:12:10.552117 ckanext-metrics_dashboard-0.1.5/ckanext/metrics_dashboard/templates/report/
--rw-r--r--   0 runner    (1001) docker     (122)     4628 2022-11-28 17:12:09.000000 ckanext-metrics_dashboard-0.1.5/ckanext/metrics_dashboard/templates/report/metrics_dashboard.html
--rw-r--r--   0 runner    (1001) docker     (122)     1802 2022-11-28 17:12:09.000000 ckanext-metrics_dashboard-0.1.5/ckanext/metrics_dashboard/templates/report/view.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 17:12:10.552117 ckanext-metrics_dashboard-0.1.5/ckanext/metrics_dashboard/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-28 17:12:09.000000 ckanext-metrics_dashboard-0.1.5/ckanext/metrics_dashboard/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7187 2022-11-28 17:12:09.000000 ckanext-metrics_dashboard-0.1.5/ckanext/metrics_dashboard/tests/test_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 17:12:10.556117 ckanext-metrics_dashboard-0.1.5/ckanext_metrics_dashboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4208 2022-11-28 17:12:10.000000 ckanext-metrics_dashboard-0.1.5/ckanext_metrics_dashboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      753 2022-11-28 17:12:10.000000 ckanext-metrics_dashboard-0.1.5/ckanext_metrics_dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 17:12:10.000000 ckanext-metrics_dashboard-0.1.5/ckanext_metrics_dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      104 2022-11-28 17:12:10.000000 ckanext-metrics_dashboard-0.1.5/ckanext_metrics_dashboard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2022-11-28 17:12:10.000000 ckanext-metrics_dashboard-0.1.5/ckanext_metrics_dashboard.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 17:12:10.000000 ckanext-metrics_dashboard-0.1.5/ckanext_metrics_dashboard.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)        8 2022-11-28 17:12:10.000000 ckanext-metrics_dashboard-0.1.5/ckanext_metrics_dashboard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      271 2022-11-28 17:12:09.000000 ckanext-metrics_dashboard-0.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      208 2022-11-28 17:12:10.556117 ckanext-metrics_dashboard-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1124 2022-11-28 17:12:09.000000 ckanext-metrics_dashboard-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:09:08.117873 ckanext-metrics_dashboard-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-19 15:09:07.000000 ckanext-metrics_dashboard-0.1.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-19 15:09:07.000000 ckanext-metrics_dashboard-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-19 15:09:08.117873 ckanext-metrics_dashboard-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-07-19 15:09:07.000000 ckanext-metrics_dashboard-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:09:08.113873 ckanext-metrics_dashboard-0.1.6/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-19 15:09:07.000000 ckanext-metrics_dashboard-0.1.6/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:09:08.117873 ckanext-metrics_dashboard-0.1.6/ckanext/metrics_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-19 15:09:07.000000 ckanext-metrics_dashboard-0.1.6/ckanext/metrics_dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-19 15:09:07.000000 ckanext-metrics_dashboard-0.1.6/ckanext/metrics_dashboard/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-07-19 15:09:07.000000 ckanext-metrics_dashboard-0.1.6/ckanext/metrics_dashboard/reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:09:08.113873 ckanext-metrics_dashboard-0.1.6/ckanext/metrics_dashboard/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:09:08.117873 ckanext-metrics_dashboard-0.1.6/ckanext/metrics_dashboard/templates/report/
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-19 15:09:07.000000 ckanext-metrics_dashboard-0.1.6/ckanext/metrics_dashboard/templates/report/metrics_dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-19 15:09:07.000000 ckanext-metrics_dashboard-0.1.6/ckanext/metrics_dashboard/templates/report/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:09:08.117873 ckanext-metrics_dashboard-0.1.6/ckanext/metrics_dashboard/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 15:09:07.000000 ckanext-metrics_dashboard-0.1.6/ckanext/metrics_dashboard/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-07-19 15:09:07.000000 ckanext-metrics_dashboard-0.1.6/ckanext/metrics_dashboard/tests/test_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:09:08.117873 ckanext-metrics_dashboard-0.1.6/ckanext_metrics_dashboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-19 15:09:08.000000 ckanext-metrics_dashboard-0.1.6/ckanext_metrics_dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-19 15:09:08.000000 ckanext-metrics_dashboard-0.1.6/ckanext_metrics_dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 15:09:08.000000 ckanext-metrics_dashboard-0.1.6/ckanext_metrics_dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-19 15:09:08.000000 ckanext-metrics_dashboard-0.1.6/ckanext_metrics_dashboard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-19 15:09:08.000000 ckanext-metrics_dashboard-0.1.6/ckanext_metrics_dashboard.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 15:09:08.000000 ckanext-metrics_dashboard-0.1.6/ckanext_metrics_dashboard.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-19 15:09:08.000000 ckanext-metrics_dashboard-0.1.6/ckanext_metrics_dashboard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-19 15:09:07.000000 ckanext-metrics_dashboard-0.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-19 15:09:08.117873 ckanext-metrics_dashboard-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-19 15:09:07.000000 ckanext-metrics_dashboard-0.1.6/setup.py
```

### Comparing `ckanext-metrics_dashboard-0.1.5/README.md` & `ckanext-metrics_dashboard-0.1.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,21 @@
 
 -   `${CKAN_URL}/report/metrics_dashboard/{org}`
 -   -   Displays a detailed report of each harvest source in an organization, where org is the ID of your organization
 
 -   CSV Export: A comprehensive table of all harvest sources
 -   JSON Export: CSV raw data plus a second key `table_data_by_org` that includes the same data grouped by organization
 
-Compatibility: Tested with CKAN 2.9, though it's expected to work with earlier versions compatible with ckanext-report.
+This extension is compatible with these versions of CKAN.
+
+CKAN version | Compatibility
+------------ | -------------
+<=2.8        | ???
+2.9          | yes (with ckanext-datagovtheme==0.1.*)
+2.10         | yes (with ckanext-datagovtheme>=0.2.1)
 
 ## Usage
 
 ### Requirements
 
 These extensions are required for metrics_dashboard:
```

### Comparing `ckanext-metrics_dashboard-0.1.5/ckanext/metrics_dashboard/plugin.py` & `ckanext-metrics_dashboard-0.1.6/ckanext/metrics_dashboard/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-metrics_dashboard-0.1.5/ckanext/metrics_dashboard/reports.py` & `ckanext-metrics_dashboard-0.1.6/ckanext/metrics_dashboard/reports.py`

 * *Files identical despite different names*

### Comparing `ckanext-metrics_dashboard-0.1.5/ckanext/metrics_dashboard/templates/report/metrics_dashboard.html` & `ckanext-metrics_dashboard-0.1.6/ckanext/metrics_dashboard/templates/report/metrics_dashboard.html`

 * *Files identical despite different names*

### Comparing `ckanext-metrics_dashboard-0.1.5/ckanext/metrics_dashboard/templates/report/view.html` & `ckanext-metrics_dashboard-0.1.6/ckanext/metrics_dashboard/templates/report/view.html`

 * *Files identical despite different names*

### Comparing `ckanext-metrics_dashboard-0.1.5/ckanext/metrics_dashboard/tests/test_reports.py` & `ckanext-metrics_dashboard-0.1.6/ckanext/metrics_dashboard/tests/test_reports.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,25 +81,25 @@
         s1 = set(['organization_title', 'harvest_sources', 'total_datasets'])
         assert s1.issubset(results['table_data_by_org'][organization['name']].keys())
         assert results['table_data_by_org'][organization['name']
                                             ]['harvest_sources'] == 1
         assert results['table_data_by_org'][organization['name']
                                             ]['total_datasets'] == 0
         assert results['table_data_by_org'][organization['name']
-                                            ]['organization_title'] == 'Test Organization'
+                                            ]['organization_title'] == organization['display_name']
 
         # test table data
         assert len(results['table']) == 1
         table = results['table'][0]
         assert table['name'] == 'test-source'
         assert table['source_type'] == 'datajson'
         assert table['state'] == 'active'
         assert table['frequency'] == 'MANUAL'
         assert table['organization_name'] == 'myorg'
-        assert table['organization_title'] == 'Test Organization'
+        assert table['organization_title'] == organization['display_name']
         assert table['job_count'] == 1
         assert table['total_datasets'] == 0
 
     def test_get_harvest_results_with_org(self, app):
         data = self.setup_data()
         organization = data['organization']
         results = report._get_harvest_results(organization['name'])
@@ -110,29 +110,29 @@
         assert s1.issubset(results['table_data_by_org'][organization['name']].keys())
         assert len(results['table_data_by_org'].keys()) == 1
         assert results['table_data_by_org'][organization['name']
                                             ]['harvest_sources'] == 1
         assert results['table_data_by_org'][organization['name']
                                             ]['total_datasets'] == 0
         assert results['table_data_by_org'][organization['name']
-                                            ]['organization_title'] == 'Test Organization'
+                                            ]['organization_title'] == organization['display_name']
 
         # assert that table_data_by_org contains same entry as table
         TestCase().assertDictEqual(results['table_data_by_org']['myorg']['packages'][0],
                                    results['table'][0])
 
         # test table data
         assert len(results['table']) == 1
         table = results['table'][0]
         assert table['name'] == 'test-source'
         assert table['source_type'] == 'datajson'
         assert table['state'] == 'active'
         assert table['frequency'] == 'MANUAL'
         assert table['organization_name'] == 'myorg'
-        assert table['organization_title'] == 'Test Organization'
+        assert table['organization_title'] == organization['display_name']
         assert table['job_count'] == 1
         assert table['total_datasets'] == 0
 
     def test_get_harvest_results_with_no_harvest_job(self, app):
         data = self.setup_data(create_harvest_job=False)
         organization = data['organization']
         results = report._get_harvest_results()
@@ -143,25 +143,25 @@
         s1 = set(['organization_title', 'harvest_sources', 'total_datasets'])
         assert s1.issubset(results['table_data_by_org'][organization['name']].keys())
         assert results['table_data_by_org'][organization['name']
                                             ]['harvest_sources'] == 1
         assert results['table_data_by_org'][organization['name']
                                             ]['total_datasets'] == 0
         assert results['table_data_by_org'][organization['name']
-                                            ]['organization_title'] == 'Test Organization'
+                                            ]['organization_title'] == organization['display_name']
 
         # test table data
         assert len(results['table']) == 1
         table = results['table'][0]
         assert table['name'] == 'test-source'
         assert table['source_type'] == 'datajson'
         assert table['state'] == 'active'
         assert table['frequency'] == 'MANUAL'
         assert table['organization_name'] == 'myorg'
-        assert table['organization_title'] == 'Test Organization'
+        assert table['organization_title'] == organization['display_name']
         assert table['job_count'] == 0
         assert table['total_datasets'] == 0
         assert table['last_job_added'] == 'N/A'
         assert table['last_job_updated'] == 'N/A'
         assert table['last_job_not_modified'] == 'N/A'
         assert table['last_job_errored'] == 'N/A'
         assert table['last_job_deleted'] == 'N/A'
```

### Comparing `ckanext-metrics_dashboard-0.1.5/ckanext_metrics_dashboard.egg-info/SOURCES.txt` & `ckanext-metrics_dashboard-0.1.6/ckanext_metrics_dashboard.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
 ckanext/__init__.py
 ckanext/metrics_dashboard/__init__.py
```

### Comparing `ckanext-metrics_dashboard-0.1.5/setup.py` & `ckanext-metrics_dashboard-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Get the long description from the relevant file
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='ckanext-metrics_dashboard',
-    version='0.1.5',
+    version='0.1.6',
     description="A CKAN extension to display metrics about datasets.",
     long_description=long_description,
     classifiers=[
         'Programming Language :: Python :: 3',
     ],  # Get strings from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     keywords='',
     author='Data.gov',
```

