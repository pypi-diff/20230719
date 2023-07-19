# Comparing `tmp/speedtab-0.1.5.0.tar.gz` & `tmp/speedtab-0.1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtab-0.1.5.0.tar", max compression
+gzip compressed data, was "speedtab-0.1.5.1.tar", max compression
```

## Comparing `speedtab-0.1.5.0.tar` & `speedtab-0.1.5.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      567 2023-06-30 16:05:22.132158 speedtab-0.1.5.0/pyproject.toml
--rw-r--r--   0        0        0      365 2023-06-09 12:04:52.821400 speedtab-0.1.5.0/speedtab/__init__.py
--rw-r--r--   0        0        0    50614 2023-06-30 16:03:40.365716 speedtab-0.1.5.0/speedtab/client.py
--rw-r--r--   0        0        0     6192 2023-05-19 11:01:11.239027 speedtab-0.1.5.0/speedtab/enums.py
--rw-r--r--   0        0        0     1724 2023-06-02 10:10:18.366392 speedtab-0.1.5.0/speedtab/formats.py
--rw-r--r--   0        0        0      783 2023-06-30 16:05:25.447351 speedtab-0.1.5.0/setup.py
--rw-r--r--   0        0        0      808 2023-06-30 16:05:25.447351 speedtab-0.1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      567 2023-07-19 09:24:39.638962 speedtab-0.1.5.1/pyproject.toml
+-rw-r--r--   0        0        0      365 2023-06-09 12:04:52.821400 speedtab-0.1.5.1/speedtab/__init__.py
+-rw-r--r--   0        0        0    50642 2023-07-19 09:24:26.160961 speedtab-0.1.5.1/speedtab/client.py
+-rw-r--r--   0        0        0     6192 2023-05-19 11:01:11.239027 speedtab-0.1.5.1/speedtab/enums.py
+-rw-r--r--   0        0        0     1724 2023-06-02 10:10:18.366392 speedtab-0.1.5.1/speedtab/formats.py
+-rw-r--r--   0        0        0      783 2023-07-19 09:24:52.894611 speedtab-0.1.5.1/setup.py
+-rw-r--r--   0        0        0      808 2023-07-19 09:24:52.894611 speedtab-0.1.5.1/PKG-INFO
```

### Comparing `speedtab-0.1.5.0/pyproject.toml` & `speedtab-0.1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "speedtab"
-version = "0.1.5.0"
+version = "0.1.5.1"
 description = "Convenient wrapper for working with Google Spreadsheets"
 authors = ["Bogdan Gergel <bogger147@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/BoggerSancho/SpeedTab-beta"
 repository = "https://github.com/BoggerSancho/SpeedTab-beta"
 
 [tool.poetry.dependencies]
```

### Comparing `speedtab-0.1.5.0/speedtab/client.py` & `speedtab-0.1.5.1/speedtab/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -900,15 +900,15 @@
             if isinstance(df.index, pd.CategoricalIndex) or any(isinstance(x, pd.Interval) for x in df.index.values):
                 df.index = df.index.astype(str)
             try:
                 df = df.reset_index(col_level=-1)
             except:
                 df = pd.merge(df.index.to_frame(index=False), df.reset_index(drop=True), left_index=True, right_index=True)
 
-        df = df.applymap(datetime_to_xls).replace([np.inf, -np.inf, np.NaN], None)
+        df = df.applymap(datetime_to_xls).replace([np.inf, -np.inf, np.NaN], None).where(pd.notnull(df), None)
 
         if header:
             if isinstance(df.columns, pd.MultiIndex):
                 values = [[str(elem) for elem in level] for level in list(zip(*df.columns.to_list()))] + df.values.tolist()
             else:
                 values = [[str(elem) for elem in df.columns.to_list()]] + df.values.tolist()
         else:
```

### Comparing `speedtab-0.1.5.0/speedtab/enums.py` & `speedtab-0.1.5.1/speedtab/enums.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.5.0/speedtab/formats.py` & `speedtab-0.1.5.1/speedtab/formats.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.5.0/setup.py` & `speedtab-0.1.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['google-api-python-client>=2.58.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.2,<0.6.0']
 
 setup_kwargs = {
     'name': 'speedtab',
-    'version': '0.1.5.0',
+    'version': '0.1.5.1',
     'description': 'Convenient wrapper for working with Google Spreadsheets',
     'long_description': None,
     'author': 'Bogdan Gergel',
     'author_email': 'bogger147@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/BoggerSancho/SpeedTab-beta',
```

### Comparing `speedtab-0.1.5.0/PKG-INFO` & `speedtab-0.1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtab
-Version: 0.1.5.0
+Version: 0.1.5.1
 Summary: Convenient wrapper for working with Google Spreadsheets
 Home-page: https://github.com/BoggerSancho/SpeedTab-beta
 License: MIT
 Author: Bogdan Gergel
 Author-email: bogger147@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

