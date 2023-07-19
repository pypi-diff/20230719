# Comparing `tmp/pycot-reports-0.0.1.tar.gz` & `tmp/pycot-reports-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycot-reports-0.0.1.tar", last modified: Wed Jun  7 02:19:39 2023, max compression
+gzip compressed data, was "pycot-reports-0.0.2.tar", last modified: Wed Jul 19 14:09:41 2023, max compression
```

## Comparing `pycot-reports-0.0.1.tar` & `pycot-reports-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:19:39.464429 pycot-reports-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-07 02:19:16.000000 pycot-reports-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-06-07 02:19:39.464429 pycot-reports-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-07 02:19:16.000000 pycot-reports-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:19:39.464429 pycot-reports-0.0.1/pycot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 02:19:16.000000 pycot-reports-0.0.1/pycot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-07 02:19:16.000000 pycot-reports-0.0.1/pycot/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-07 02:19:16.000000 pycot-reports-0.0.1/pycot/extract_report_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-06-07 02:19:16.000000 pycot-reports-0.0.1/pycot/pycot.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-07 02:19:16.000000 pycot-reports-0.0.1/pycot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 02:19:39.464429 pycot-reports-0.0.1/pycot_reports.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-06-07 02:19:39.000000 pycot-reports-0.0.1/pycot_reports.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-07 02:19:39.000000 pycot-reports-0.0.1/pycot_reports.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 02:19:39.000000 pycot-reports-0.0.1/pycot_reports.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-07 02:19:39.000000 pycot-reports-0.0.1/pycot_reports.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 02:19:39.000000 pycot-reports-0.0.1/pycot_reports.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-07 02:19:16.000000 pycot-reports-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-07 02:19:39.464429 pycot-reports-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-07 02:19:16.000000 pycot-reports-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:09:41.480836 pycot-reports-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-19 14:09:18.000000 pycot-reports-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-07-19 14:09:41.480836 pycot-reports-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-07-19 14:09:18.000000 pycot-reports-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:09:41.480836 pycot-reports-0.0.2/pycot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:09:18.000000 pycot-reports-0.0.2/pycot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-19 14:09:18.000000 pycot-reports-0.0.2/pycot/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-19 14:09:18.000000 pycot-reports-0.0.2/pycot/extract_report_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-19 14:09:18.000000 pycot-reports-0.0.2/pycot/pycot.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 14:09:18.000000 pycot-reports-0.0.2/pycot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:09:41.480836 pycot-reports-0.0.2/pycot_reports.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-07-19 14:09:41.000000 pycot-reports-0.0.2/pycot_reports.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-19 14:09:41.000000 pycot-reports-0.0.2/pycot_reports.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 14:09:41.000000 pycot-reports-0.0.2/pycot_reports.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-19 14:09:41.000000 pycot-reports-0.0.2/pycot_reports.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 14:09:41.000000 pycot-reports-0.0.2/pycot_reports.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-19 14:09:18.000000 pycot-reports-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-19 14:09:41.480836 pycot-reports-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-19 14:09:18.000000 pycot-reports-0.0.2/setup.py
```

### Comparing `pycot-reports-0.0.1/LICENSE` & `pycot-reports-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycot-reports-0.0.1/pycot/extract_report_data.py` & `pycot-reports-0.0.2/pycot/extract_report_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
     def extract_text_file_to_dataframe(
         self,
         response: requests.models.Response,
         text_file: str,
     ) -> pd.DataFrame:
         """
-        Unzips the a text file from an archive and returns a pandas DataFrame.
+        Unzips the text file from an archive and returns a pandas DataFrame.
         """
         with tempfile.TemporaryDirectory() as tmpdirname:
             os.chdir(tmpdirname)  # change working directory to temp directory
 
             with zipfile.ZipFile(io.BytesIO(response.content)) as z:
                 z.extractall()
             return pd.read_csv(text_file, low_memory=False)
```

### Comparing `pycot-reports-0.0.1/pycot/pycot.py` & `pycot-reports-0.0.2/pycot/pycot.py`

 * *Files identical despite different names*

### Comparing `pycot-reports-0.0.1/setup.py` & `pycot-reports-0.0.2/setup.py`

 * *Files identical despite different names*

