# Comparing `tmp/antigranular-0.2.1.tar.gz` & `tmp/antigranular-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antigranular-0.2.1.tar", max compression
+gzip compressed data, was "antigranular-0.2.2.tar", max compression
```

## Comparing `antigranular-0.2.1.tar` & `antigranular-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      548 2023-07-19 09:58:06.449242 antigranular-0.2.1/antigranular/__init__.py
--rw-r--r--   0        0        0    10800 2023-07-19 09:58:21.012154 antigranular-0.2.1/antigranular/client.py
--rw-r--r--   0        0        0      907 2023-07-19 09:58:06.451168 antigranular-0.2.1/antigranular/config/config.py
--rw-r--r--   0        0        0     3025 2023-07-19 09:58:06.453259 antigranular-0.2.1/antigranular/enclave_client/mock_client.py
--rw-r--r--   0        0        0      802 2023-07-19 09:58:21.016588 antigranular-0.2.1/antigranular/enclave_client/oblv_client.py
--rw-r--r--   0        0        0     1053 2023-07-19 09:58:06.457264 antigranular-0.2.1/antigranular/magics/errors.py
--rw-r--r--   0        0        0     6659 2023-07-19 09:58:06.457264 antigranular-0.2.1/antigranular/magics/magics.py
--rw-r--r--   0        0        0        0 2023-07-19 09:58:06.458608 antigranular-0.2.1/antigranular/models/__init__.py
--rw-r--r--   0        0        0      661 2023-07-19 09:58:06.460607 antigranular-0.2.1/antigranular/models/models.py
--rw-r--r--   0        0        0      149 2023-07-19 09:58:06.462114 antigranular-0.2.1/antigranular/utils/error_print.py
--rw-r--r--   0        0        0    11558 2023-07-19 09:58:06.446114 antigranular-0.2.1/LICENSE
--rw-r--r--   0        0        0      759 2023-07-19 10:01:44.037227 antigranular-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4286 2023-07-19 09:58:06.448114 antigranular-0.2.1/README.md
--rw-r--r--   0        0        0     5096 1970-01-01 00:00:00.000000 antigranular-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      548 2023-07-19 09:58:06.449242 antigranular-0.2.2/antigranular/__init__.py
+-rw-r--r--   0        0        0    10800 2023-07-19 09:58:21.012154 antigranular-0.2.2/antigranular/client.py
+-rw-r--r--   0        0        0      907 2023-07-19 09:58:06.451168 antigranular-0.2.2/antigranular/config/config.py
+-rw-r--r--   0        0        0     3025 2023-07-19 09:58:06.453259 antigranular-0.2.2/antigranular/enclave_client/mock_client.py
+-rw-r--r--   0        0        0      802 2023-07-19 09:58:21.016588 antigranular-0.2.2/antigranular/enclave_client/oblv_client.py
+-rw-r--r--   0        0        0     1053 2023-07-19 09:58:06.457264 antigranular-0.2.2/antigranular/magics/errors.py
+-rw-r--r--   0        0        0     6659 2023-07-19 09:58:06.457264 antigranular-0.2.2/antigranular/magics/magics.py
+-rw-r--r--   0        0        0        0 2023-07-19 09:58:06.458608 antigranular-0.2.2/antigranular/models/__init__.py
+-rw-r--r--   0        0        0      661 2023-07-19 09:58:06.460607 antigranular-0.2.2/antigranular/models/models.py
+-rw-r--r--   0        0        0      149 2023-07-19 09:58:06.462114 antigranular-0.2.2/antigranular/utils/error_print.py
+-rw-r--r--   0        0        0    11558 2023-07-19 09:58:06.446114 antigranular-0.2.2/LICENSE
+-rw-r--r--   0        0        0      759 2023-07-19 10:54:23.346230 antigranular-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4210 2023-07-19 10:30:46.949293 antigranular-0.2.2/README.md
+-rw-r--r--   0        0        0     5031 1970-01-01 00:00:00.000000 antigranular-0.2.2/PKG-INFO
```

### Comparing `antigranular-0.2.1/antigranular/__init__.py` & `antigranular-0.2.2/antigranular/__init__.py`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.1/antigranular/client.py` & `antigranular-0.2.2/antigranular/client.py`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.1/antigranular/config/config.py` & `antigranular-0.2.2/antigranular/config/config.py`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.1/antigranular/enclave_client/mock_client.py` & `antigranular-0.2.2/antigranular/enclave_client/mock_client.py`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.1/antigranular/enclave_client/oblv_client.py` & `antigranular-0.2.2/antigranular/enclave_client/oblv_client.py`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.1/antigranular/magics/errors.py` & `antigranular-0.2.2/antigranular/magics/errors.py`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.1/antigranular/magics/magics.py` & `antigranular-0.2.2/antigranular/magics/magics.py`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.1/antigranular/models/models.py` & `antigranular-0.2.2/antigranular/models/models.py`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.1/LICENSE` & `antigranular-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `antigranular-0.2.1/pyproject.toml` & `antigranular-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "antigranular"
-version = "0.2.1"
+version = "0.2.2"
 description = "Antigranular is a community-driven, open-source platform that merges confidential computing and differential privacy. This creates a secure environment for handling and unlocking the full potential of unseen data.."
 authors = ["Oblivious Software <support@oblivious.ai>"]
 readme = "README.md"
 packages = [{include = "antigranular"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `antigranular-0.2.1/README.md` & `antigranular-0.2.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,34 @@
-# Unlock privacy: Getting along with Antigranular
-Antigranular is a community-driven, open-source platform that merges confidential computing and differential privacy. This creates a secure environment for handling and unlocking the full potential of unseen data.
+# Privacy Unleashed: Working with Antigranular
+Antigranular is a community-led, open-source platform that combines confidential computing with differential privacy. This integration fosters a secure environment to handle and fully utilize unseen data.
 ### Connect to Antigranular 
-Antigranular works with just 4 characters `%%ag` , like magic!
-Any code written after the magic cell `%%ag` is run in our remote server 
-which is a restricted environment allowing methods which guarantees
-differential privacy.
+You can activate Antigranular using the magic command `%%ag`. Any code that follows `%%ag` will run on our remote server. This server operates under restricted conditions, allowing only methods that guarantee differential privacy.
 
 Install the Antigranular package using `pip`:
 ```python
 !pip install antigranular
 ```
 Import the `Antigranular` library:
 ```python
 import antigranular as ag
 ```
-Use your client credentials and dataset or competition ID to connect to the AG Enclave Server:
+To connect to the AG Enclave Server, use your client credentials and either a dataset or competition ID:
 ```python
-ag.login("client id": "<client_secret_id>": competition="<competition_id>")
+ag.login(user_id: "<user_id>", user_secret: "<user_secret>",  competition="<competition_id>")
+```
+or
+```python
+ag.login(user_id: "<user_id>", user_secret: "<user_secret>", dataset="<dataset_id>")
 ```
 A succesful login will register the cell magic `%%ag`. 
 
 ### Loading Private Datasets 
-Private dataset objects can be loaded in the form of `PrivateDataFrames` and `PrivateSeries`
-using the `ag_utils` library. `ag_utils` is a package locally intalled in the remote server.
-This eliminated the hassle of having to install anything other than 
-antigranular package.
-
-You can learn more about `PrivateSeries` and `PrivateDataFrames` on our quick 
-on [Private Pandas](./QS_pandas).
-
-We use `load_dataset()` method to obtain a collection of private objects in the form of a dictionary.
-The structure of the response dictionary, 
-dataset path and private object names will be mentioned during the competition.
+Private datasets can be loaded as `PrivateDataFrames` and `PrivateSeries` using the `ag_utils` library. `ag_utils` is a package locally installed on the remote server, which eliminates the need to install anything other than the antigranular package.
+
+The `load_dataset()` method can be used to obtain a dictionary of private objects. The response dictionary's structure, dataset path, and private object names will be specified during the competition.
 ```python
 %%ag
 from op_pandas import PrivateDataFrame , PrivateSeries
 from ag_utils import load_dataset 
 """
 Sample response structure
 {
@@ -49,30 +42,26 @@
 
 # Unpacking the response dictionary
 train_x = response["train_x"]
 train_y = response["train_y"]
 test_x = response["test_x"]
 ```
 ### Exporting Objects
-Since `%%ag` runs code in a very restricted environment, you need to export the differentially private 
-objects to the local environment in order to do further analysis.
-The data objects can be exported using the `export` method in `ag_utils`.
+Since the code following `%%ag` runs in a highly restricted environment, it's necessary to export differentially private objects to the local environment for further analysis. The `export` method in `ag_utils` allows data objects to be exported.
 ##### **API info**: `export(obj, variable_name:str)`
-The remote object gets exported to the local environment and gets 
-assigned to the stated variable name. It is important to note that`PrivateSeries` and `PrivateDataFrame`
-objects cannot be exported and will raise an error if tried to 
-be exported in any manner.
+
+This command exports the remote object to the local environment and assigns it to the specified variable name. Note that `PrivateSeries` and `PrivateDataFrame` objects cannot be exported and will raise an error if you attempt to do so.
+
 ```python 
 %%ag
 from ag_utils import export
 train_info = train_x.describe(eps=1)
 export(train_info , 'variable_name')
 ```
-Once exported, you can apply any form of data anlysis on the 
-differentially private object.
+Once exported, you can perform any kind of data analysis on the differentially private object.
 
 ```python
 # Local code block
 print(variable_name)
 --------------------------------------
                     Age         Salary
     count  99987.000000   99987.000000
@@ -84,15 +73,15 @@
     75%       49.147724  159835.637091
     max       59.282932  199920.664706
 ```
 
 ## Libraries Supported
 
 
-- **`pandas`**: A versatile data manipulation library that offers efficient data structures and tools for data analysis and manipulation.
+- **`pandas`**: An adaptable data manipulation library offering efficient data structures and tools for data analysis and manipulation.
 
 - **`op_pandas`**: A wrapped library specifically designed for differentially private data manipulation within the Pandas framework. It enhances privacy-preserving techniques and enables privacy-aware data processing.
 
 - **`op_diffprivlib`**: A differentially private library that provides various privacy-preserving algorithms and mechanisms for machine learning and data analysis tasks.
 
 - **`op_smartnoise`**: A library focused on privacy-preserving analysis using the SmartNoise framework. It provides tools for differential privacy and secure computation.
```

### Comparing `antigranular-0.2.1/PKG-INFO` & `antigranular-0.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antigranular
-Version: 0.2.1
+Version: 0.2.2
 Summary: Antigranular is a community-driven, open-source platform that merges confidential computing and differential privacy. This creates a secure environment for handling and unlocking the full potential of unseen data..
 Author: Oblivious Software
 Author-email: support@oblivious.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -14,48 +14,41 @@
 Requires-Dist: ipython (>=7.34.0,<8.0.0)
 Requires-Dist: oblv-client (>=0.1.15,<0.2.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: requests (==2.27.1)
 Description-Content-Type: text/markdown
 
-# Unlock privacy: Getting along with Antigranular
-Antigranular is a community-driven, open-source platform that merges confidential computing and differential privacy. This creates a secure environment for handling and unlocking the full potential of unseen data.
+# Privacy Unleashed: Working with Antigranular
+Antigranular is a community-led, open-source platform that combines confidential computing with differential privacy. This integration fosters a secure environment to handle and fully utilize unseen data.
 ### Connect to Antigranular 
-Antigranular works with just 4 characters `%%ag` , like magic!
-Any code written after the magic cell `%%ag` is run in our remote server 
-which is a restricted environment allowing methods which guarantees
-differential privacy.
+You can activate Antigranular using the magic command `%%ag`. Any code that follows `%%ag` will run on our remote server. This server operates under restricted conditions, allowing only methods that guarantee differential privacy.
 
 Install the Antigranular package using `pip`:
 ```python
 !pip install antigranular
 ```
 Import the `Antigranular` library:
 ```python
 import antigranular as ag
 ```
-Use your client credentials and dataset or competition ID to connect to the AG Enclave Server:
+To connect to the AG Enclave Server, use your client credentials and either a dataset or competition ID:
 ```python
-ag.login("client id": "<client_secret_id>": competition="<competition_id>")
+ag.login(user_id: "<user_id>", user_secret: "<user_secret>",  competition="<competition_id>")
+```
+or
+```python
+ag.login(user_id: "<user_id>", user_secret: "<user_secret>", dataset="<dataset_id>")
 ```
 A succesful login will register the cell magic `%%ag`. 
 
 ### Loading Private Datasets 
-Private dataset objects can be loaded in the form of `PrivateDataFrames` and `PrivateSeries`
-using the `ag_utils` library. `ag_utils` is a package locally intalled in the remote server.
-This eliminated the hassle of having to install anything other than 
-antigranular package.
-
-You can learn more about `PrivateSeries` and `PrivateDataFrames` on our quick 
-on [Private Pandas](./QS_pandas).
-
-We use `load_dataset()` method to obtain a collection of private objects in the form of a dictionary.
-The structure of the response dictionary, 
-dataset path and private object names will be mentioned during the competition.
+Private datasets can be loaded as `PrivateDataFrames` and `PrivateSeries` using the `ag_utils` library. `ag_utils` is a package locally installed on the remote server, which eliminates the need to install anything other than the antigranular package.
+
+The `load_dataset()` method can be used to obtain a dictionary of private objects. The response dictionary's structure, dataset path, and private object names will be specified during the competition.
 ```python
 %%ag
 from op_pandas import PrivateDataFrame , PrivateSeries
 from ag_utils import load_dataset 
 """
 Sample response structure
 {
@@ -69,30 +62,26 @@
 
 # Unpacking the response dictionary
 train_x = response["train_x"]
 train_y = response["train_y"]
 test_x = response["test_x"]
 ```
 ### Exporting Objects
-Since `%%ag` runs code in a very restricted environment, you need to export the differentially private 
-objects to the local environment in order to do further analysis.
-The data objects can be exported using the `export` method in `ag_utils`.
+Since the code following `%%ag` runs in a highly restricted environment, it's necessary to export differentially private objects to the local environment for further analysis. The `export` method in `ag_utils` allows data objects to be exported.
 ##### **API info**: `export(obj, variable_name:str)`
-The remote object gets exported to the local environment and gets 
-assigned to the stated variable name. It is important to note that`PrivateSeries` and `PrivateDataFrame`
-objects cannot be exported and will raise an error if tried to 
-be exported in any manner.
+
+This command exports the remote object to the local environment and assigns it to the specified variable name. Note that `PrivateSeries` and `PrivateDataFrame` objects cannot be exported and will raise an error if you attempt to do so.
+
 ```python 
 %%ag
 from ag_utils import export
 train_info = train_x.describe(eps=1)
 export(train_info , 'variable_name')
 ```
-Once exported, you can apply any form of data anlysis on the 
-differentially private object.
+Once exported, you can perform any kind of data analysis on the differentially private object.
 
 ```python
 # Local code block
 print(variable_name)
 --------------------------------------
                     Age         Salary
     count  99987.000000   99987.000000
@@ -104,15 +93,15 @@
     75%       49.147724  159835.637091
     max       59.282932  199920.664706
 ```
 
 ## Libraries Supported
 
 
-- **`pandas`**: A versatile data manipulation library that offers efficient data structures and tools for data analysis and manipulation.
+- **`pandas`**: An adaptable data manipulation library offering efficient data structures and tools for data analysis and manipulation.
 
 - **`op_pandas`**: A wrapped library specifically designed for differentially private data manipulation within the Pandas framework. It enhances privacy-preserving techniques and enables privacy-aware data processing.
 
 - **`op_diffprivlib`**: A differentially private library that provides various privacy-preserving algorithms and mechanisms for machine learning and data analysis tasks.
 
 - **`op_smartnoise`**: A library focused on privacy-preserving analysis using the SmartNoise framework. It provides tools for differential privacy and secure computation.
```

