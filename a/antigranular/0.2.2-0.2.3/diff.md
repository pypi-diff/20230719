# Comparing `tmp/antigranular-0.2.2.tar.gz` & `tmp/antigranular-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antigranular-0.2.2.tar", max compression
+gzip compressed data, was "antigranular-0.2.3.tar", max compression
```

## Comparing `antigranular-0.2.2.tar` & `antigranular-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      548 2023-07-19 09:58:06.449242 antigranular-0.2.2/antigranular/__init__.py
--rw-r--r--   0        0        0    10800 2023-07-19 09:58:21.012154 antigranular-0.2.2/antigranular/client.py
--rw-r--r--   0        0        0      907 2023-07-19 09:58:06.451168 antigranular-0.2.2/antigranular/config/config.py
--rw-r--r--   0        0        0     3025 2023-07-19 09:58:06.453259 antigranular-0.2.2/antigranular/enclave_client/mock_client.py
--rw-r--r--   0        0        0      802 2023-07-19 09:58:21.016588 antigranular-0.2.2/antigranular/enclave_client/oblv_client.py
--rw-r--r--   0        0        0     1053 2023-07-19 09:58:06.457264 antigranular-0.2.2/antigranular/magics/errors.py
--rw-r--r--   0        0        0     6659 2023-07-19 09:58:06.457264 antigranular-0.2.2/antigranular/magics/magics.py
--rw-r--r--   0        0        0        0 2023-07-19 09:58:06.458608 antigranular-0.2.2/antigranular/models/__init__.py
--rw-r--r--   0        0        0      661 2023-07-19 09:58:06.460607 antigranular-0.2.2/antigranular/models/models.py
--rw-r--r--   0        0        0      149 2023-07-19 09:58:06.462114 antigranular-0.2.2/antigranular/utils/error_print.py
--rw-r--r--   0        0        0    11558 2023-07-19 09:58:06.446114 antigranular-0.2.2/LICENSE
--rw-r--r--   0        0        0      759 2023-07-19 10:54:23.346230 antigranular-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4210 2023-07-19 10:30:46.949293 antigranular-0.2.2/README.md
--rw-r--r--   0        0        0     5031 1970-01-01 00:00:00.000000 antigranular-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      548 2023-07-19 09:58:06.449242 antigranular-0.2.3/antigranular/__init__.py
+-rw-r--r--   0        0        0    10800 2023-07-19 09:58:21.012154 antigranular-0.2.3/antigranular/client.py
+-rw-r--r--   0        0        0      907 2023-07-19 09:58:06.451168 antigranular-0.2.3/antigranular/config/config.py
+-rw-r--r--   0        0        0     3025 2023-07-19 09:58:06.453259 antigranular-0.2.3/antigranular/enclave_client/mock_client.py
+-rw-r--r--   0        0        0      802 2023-07-19 09:58:21.016588 antigranular-0.2.3/antigranular/enclave_client/oblv_client.py
+-rw-r--r--   0        0        0     1053 2023-07-19 09:58:06.457264 antigranular-0.2.3/antigranular/magics/errors.py
+-rw-r--r--   0        0        0     6659 2023-07-19 09:58:06.457264 antigranular-0.2.3/antigranular/magics/magics.py
+-rw-r--r--   0        0        0        0 2023-07-19 09:58:06.458608 antigranular-0.2.3/antigranular/models/__init__.py
+-rw-r--r--   0        0        0      661 2023-07-19 09:58:06.460607 antigranular-0.2.3/antigranular/models/models.py
+-rw-r--r--   0        0        0      149 2023-07-19 09:58:06.462114 antigranular-0.2.3/antigranular/utils/error_print.py
+-rw-r--r--   0        0        0    11558 2023-07-19 09:58:06.446114 antigranular-0.2.3/LICENSE
+-rw-r--r--   0        0        0      759 2023-07-19 10:57:47.971777 antigranular-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4248 2023-07-19 11:03:07.354982 antigranular-0.2.3/README.md
+-rw-r--r--   0        0        0     5069 1970-01-01 00:00:00.000000 antigranular-0.2.3/PKG-INFO
```

### Comparing `antigranular-0.2.2/antigranular/__init__.py` & `antigranular-0.2.3/antigranular/__init__.py`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.2/antigranular/client.py` & `antigranular-0.2.3/antigranular/client.py`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.2/antigranular/config/config.py` & `antigranular-0.2.3/antigranular/config/config.py`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.2/antigranular/enclave_client/mock_client.py` & `antigranular-0.2.3/antigranular/enclave_client/mock_client.py`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.2/antigranular/enclave_client/oblv_client.py` & `antigranular-0.2.3/antigranular/enclave_client/oblv_client.py`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.2/antigranular/magics/errors.py` & `antigranular-0.2.3/antigranular/magics/errors.py`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.2/antigranular/magics/magics.py` & `antigranular-0.2.3/antigranular/magics/magics.py`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.2/antigranular/models/models.py` & `antigranular-0.2.3/antigranular/models/models.py`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.2/LICENSE` & `antigranular-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.2/pyproject.toml` & `antigranular-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "antigranular"
-version = "0.2.2"
+version = "0.2.3"
 description = "Antigranular is a community-driven, open-source platform that merges confidential computing and differential privacy. This creates a secure environment for handling and unlocking the full potential of unseen data.."
 authors = ["Oblivious Software <support@oblivious.ai>"]
 readme = "README.md"
 packages = [{include = "antigranular"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `antigranular-0.2.2/README.md` & `antigranular-0.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,29 +9,29 @@
 ```
 Import the `Antigranular` library:
 ```python
 import antigranular as ag
 ```
 To connect to the AG Enclave Server, use your client credentials and either a dataset or competition ID:
 ```python
-ag.login(user_id: "<user_id>", user_secret: "<user_secret>",  competition="<competition_id>")
+ag_client = ag.login(user_id="<user_id>", user_secret="<user_secret>",  competition="<competition_id>")
 ```
 or
 ```python
-ag.login(user_id: "<user_id>", user_secret: "<user_secret>", dataset="<dataset_id>")
+ag_client = ag.login(user_id="<user_id>", user_secret="<user_secret>", dataset="<dataset_id>")
 ```
 A succesful login will register the cell magic `%%ag`. 
 
 ### Loading Private Datasets 
 Private datasets can be loaded as `PrivateDataFrames` and `PrivateSeries` using the `ag_utils` library. `ag_utils` is a package locally installed on the remote server, which eliminates the need to install anything other than the antigranular package.
 
-The `load_dataset()` method can be used to obtain a dictionary of private objects. The response dictionary's structure, dataset path, and private object names will be specified during the competition.
+The `load_dataset()` method allows for obtaining a dictionary of private objects. The structure of the response dictionary, along with the dataset path and private object names, will be specified during the competition.
 ```python
 %%ag
-from op_pandas import PrivateDataFrame , PrivateSeries
+from op_pandas import PrivateDataFrame, PrivateSeries
 from ag_utils import load_dataset 
 """
 Sample response structure
 {
     train_x : priv_train_x,
     train_y : priv_train_y,
     test_x : priv_test_x
```

### Comparing `antigranular-0.2.2/PKG-INFO` & `antigranular-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antigranular
-Version: 0.2.2
+Version: 0.2.3
 Summary: Antigranular is a community-driven, open-source platform that merges confidential computing and differential privacy. This creates a secure environment for handling and unlocking the full potential of unseen data..
 Author: Oblivious Software
 Author-email: support@oblivious.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -29,29 +29,29 @@
 ```
 Import the `Antigranular` library:
 ```python
 import antigranular as ag
 ```
 To connect to the AG Enclave Server, use your client credentials and either a dataset or competition ID:
 ```python
-ag.login(user_id: "<user_id>", user_secret: "<user_secret>",  competition="<competition_id>")
+ag_client = ag.login(user_id="<user_id>", user_secret="<user_secret>",  competition="<competition_id>")
 ```
 or
 ```python
-ag.login(user_id: "<user_id>", user_secret: "<user_secret>", dataset="<dataset_id>")
+ag_client = ag.login(user_id="<user_id>", user_secret="<user_secret>", dataset="<dataset_id>")
 ```
 A succesful login will register the cell magic `%%ag`. 
 
 ### Loading Private Datasets 
 Private datasets can be loaded as `PrivateDataFrames` and `PrivateSeries` using the `ag_utils` library. `ag_utils` is a package locally installed on the remote server, which eliminates the need to install anything other than the antigranular package.
 
-The `load_dataset()` method can be used to obtain a dictionary of private objects. The response dictionary's structure, dataset path, and private object names will be specified during the competition.
+The `load_dataset()` method allows for obtaining a dictionary of private objects. The structure of the response dictionary, along with the dataset path and private object names, will be specified during the competition.
 ```python
 %%ag
-from op_pandas import PrivateDataFrame , PrivateSeries
+from op_pandas import PrivateDataFrame, PrivateSeries
 from ag_utils import load_dataset 
 """
 Sample response structure
 {
     train_x : priv_train_x,
     train_y : priv_train_y,
     test_x : priv_test_x
```

