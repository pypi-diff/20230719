# Comparing `tmp/ecallisto_ng-0.2.1.tar.gz` & `tmp/ecallisto_ng-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecallisto_ng-0.2.1.tar", last modified: Tue Jul 18 10:10:03 2023, max compression
+gzip compressed data, was "ecallisto_ng-0.2.2.tar", last modified: Tue Jul 18 19:06:52 2023, max compression
```

## Comparing `ecallisto_ng-0.2.1.tar` & `ecallisto_ng-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 10:10:03.848899 ecallisto_ng-0.2.1/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.2.1/LICENSE
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3608 2023-07-18 10:10:03.848899 ecallisto_ng-0.2.1/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3028 2023-07-17 09:45:19.000000 ecallisto_ng-0.2.1/README.md
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      858 2023-07-18 10:09:00.000000 ecallisto_ng-0.2.1/pyproject.toml
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-18 10:10:03.848899 ecallisto_ng-0.2.1/setup.cfg
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 10:10:03.848899 ecallisto_ng-0.2.1/src/
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 10:10:03.848899 ecallisto_ng-0.2.1/src/ecallisto_ng/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.2.1/src/ecallisto_ng/__init__.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 10:10:03.848899 ecallisto_ng-0.2.1/src/ecallisto_ng/data_fetching/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:51.000000 ecallisto_ng-0.2.1/src/ecallisto_ng/data_fetching/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     7501 2023-07-17 13:11:37.000000 ecallisto_ng-0.2.1/src/ecallisto_ng/data_fetching/get_data.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3398 2023-07-18 10:05:42.000000 ecallisto_ng-0.2.1/src/ecallisto_ng/data_fetching/get_information.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 10:10:03.848899 ecallisto_ng-0.2.1/src/ecallisto_ng/data_processing/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:54.000000 ecallisto_ng-0.2.1/src/ecallisto_ng/data_processing/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5256 2023-07-11 08:45:15.000000 ecallisto_ng-0.2.1/src/ecallisto_ng/data_processing/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 10:10:03.848899 ecallisto_ng-0.2.1/src/ecallisto_ng/plotting/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:40:01.000000 ecallisto_ng-0.2.1/src/ecallisto_ng/plotting/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2425 2023-07-10 17:56:33.000000 ecallisto_ng-0.2.1/src/ecallisto_ng/plotting/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 10:10:03.848899 ecallisto_ng-0.2.1/src/ecallisto_ng.egg-info/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3608 2023-07-18 10:10:03.000000 ecallisto_ng-0.2.1/src/ecallisto_ng.egg-info/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      556 2023-07-18 10:10:03.000000 ecallisto_ng-0.2.1/src/ecallisto_ng.egg-info/SOURCES.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-18 10:10:03.000000 ecallisto_ng-0.2.1/src/ecallisto_ng.egg-info/dependency_links.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      129 2023-07-18 10:10:03.000000 ecallisto_ng-0.2.1/src/ecallisto_ng.egg-info/requires.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-18 10:10:03.000000 ecallisto_ng-0.2.1/src/ecallisto_ng.egg-info/top_level.txt
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 19:06:52.169913 ecallisto_ng-0.2.2/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.2.2/LICENSE
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3608 2023-07-18 19:06:52.169913 ecallisto_ng-0.2.2/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3028 2023-07-17 09:45:19.000000 ecallisto_ng-0.2.2/README.md
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      858 2023-07-18 19:06:25.000000 ecallisto_ng-0.2.2/pyproject.toml
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-18 19:06:52.169913 ecallisto_ng-0.2.2/setup.cfg
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 19:06:52.169913 ecallisto_ng-0.2.2/src/
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 19:06:52.169913 ecallisto_ng-0.2.2/src/ecallisto_ng/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.2.2/src/ecallisto_ng/__init__.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 19:06:52.169913 ecallisto_ng-0.2.2/src/ecallisto_ng/data_fetching/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:51.000000 ecallisto_ng-0.2.2/src/ecallisto_ng/data_fetching/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     7758 2023-07-18 19:05:40.000000 ecallisto_ng-0.2.2/src/ecallisto_ng/data_fetching/get_data.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3398 2023-07-18 10:05:42.000000 ecallisto_ng-0.2.2/src/ecallisto_ng/data_fetching/get_information.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 19:06:52.169913 ecallisto_ng-0.2.2/src/ecallisto_ng/data_processing/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:54.000000 ecallisto_ng-0.2.2/src/ecallisto_ng/data_processing/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5256 2023-07-11 08:45:15.000000 ecallisto_ng-0.2.2/src/ecallisto_ng/data_processing/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 19:06:52.169913 ecallisto_ng-0.2.2/src/ecallisto_ng/plotting/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:40:01.000000 ecallisto_ng-0.2.2/src/ecallisto_ng/plotting/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2844 2023-07-18 19:00:07.000000 ecallisto_ng-0.2.2/src/ecallisto_ng/plotting/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 19:06:52.169913 ecallisto_ng-0.2.2/src/ecallisto_ng.egg-info/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3608 2023-07-18 19:06:52.000000 ecallisto_ng-0.2.2/src/ecallisto_ng.egg-info/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      556 2023-07-18 19:06:52.000000 ecallisto_ng-0.2.2/src/ecallisto_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-18 19:06:52.000000 ecallisto_ng-0.2.2/src/ecallisto_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      129 2023-07-18 19:06:52.000000 ecallisto_ng-0.2.2/src/ecallisto_ng.egg-info/requires.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-18 19:06:52.000000 ecallisto_ng-0.2.2/src/ecallisto_ng.egg-info/top_level.txt
```

### Comparing `ecallisto_ng-0.2.1/LICENSE` & `ecallisto_ng-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.1/PKG-INFO` & `ecallisto_ng-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecallisto_ng
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecallisto_ng-0.2.1/README.md` & `ecallisto_ng-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.1/pyproject.toml` & `ecallisto_ng-0.2.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ecallisto_ng"
-version = "0.2.1"
+version = "0.2.2"
 authors = [{name = "Vincenzo Timmel", email = "vincenzo.timmel@fhnw.ch"}]
 description = "A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API."
 readme = "README.md"
 
 requires-python = ">=3.9"
 
 classifiers = [
```

### Comparing `ecallisto_ng-0.2.1/src/ecallisto_ng/data_fetching/get_data.py` & `ecallisto_ng-0.2.2/src/ecallisto_ng/data_fetching/get_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,22 +89,26 @@
             if file_response.status_code == 200:
                 print("File downloaded successfully")
                 with open(file_path, "wb") as f:
                     f.write(file_response.content)
                 return pd.read_parquet(file_path)
             elif file_response.status_code == 204:
                 # Check if the file creation causes any errors
+                # This json contains information about the request
                 json_response = requests.get(BASE_URL + json_url)
                 # Check the status of the json 
                 if 'status' in json_response.json():
                     if json_response.json()['status'] == 'processing':
                         # If the file is not found, sleep for a short period and try again
                         if verbose:
                             print(f"File {file_id} not ready yet, waiting...")
                         time.sleep(5)
+                    elif json_response.json['status'] == 'ok':
+                        if verbose:
+                            print(f'File {file_id} succesfully written! Will return file')
                     else:
                         raise ValueError(f"Error downloading file: {json_response.json()['status']}")
                 elif 'error' in json_response.json():
                     raise ValueError(f"Error downloading file: {json_response.json()['error']}")
             else:
                 print(f"Error downloading file: {file_response.status_code}")
                 json_response = requests.get(BASE_URL + json_url)
```

### Comparing `ecallisto_ng-0.2.1/src/ecallisto_ng/data_fetching/get_information.py` & `ecallisto_ng-0.2.2/src/ecallisto_ng/data_fetching/get_information.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.1/src/ecallisto_ng/data_processing/utils.py` & `ecallisto_ng-0.2.2/src/ecallisto_ng/data_processing/utils.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.1/src/ecallisto_ng/plotting/utils.py` & `ecallisto_ng-0.2.2/src/ecallisto_ng/plotting/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 import numpy as np
 import pandas as pd
 import plotly.express as px
 
 
-def plot_spectogram(df, instrument_name, start_datetime, end_datetime, size=18, round_precision=2):
+def plot_spectogram(df, instrument_name, start_datetime, end_datetime, size=18, round_precision=1, color_scale=px.colors.sequential.Plasma):
     # Create a new dataframe with rounded column names
     df_rounded = df.copy()
     df_rounded.columns = [f"{float(col):.{round_precision}f}" for col in df.columns]
 
-    fig = px.imshow(df_rounded.T)
+    # Make datetime prettier
+    sd_str = start_datetime.strftime("%Y-%m-%d %H:%M:%S")
+    ed_str = end_datetime.strftime("%Y-%m-%d %H:%M:%S")
+
+    # Trick to make NANs appear black
+    # Replace NaNs with -1
+    df_rounded.fillna(-1, inplace=True)
+    # Add black for NANS
+    color_scale.insert(0, "black")
+
+    fig = px.imshow(df_rounded.T, color_continuous_scale=color_scale, zmin=df.min().min(), zmax=df.max().max())
     fig.update_layout(
-        title=f"Spectogram of {instrument_name} from {start_datetime} to {end_datetime}",
+        title=f"Spectogram of {instrument_name} between {sd_str} and {ed_str}",
         xaxis_title="Datetime",
         yaxis_title="Frequency",
         font=dict(family="Courier New, monospace", size=size, color="#7f7f7f"),
     )
     return fig
 
 def fill_missing_timesteps_with_nan(df):
```

### Comparing `ecallisto_ng-0.2.1/src/ecallisto_ng.egg-info/PKG-INFO` & `ecallisto_ng-0.2.2/src/ecallisto_ng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecallisto-ng
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecallisto_ng-0.2.1/src/ecallisto_ng.egg-info/SOURCES.txt` & `ecallisto_ng-0.2.2/src/ecallisto_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

