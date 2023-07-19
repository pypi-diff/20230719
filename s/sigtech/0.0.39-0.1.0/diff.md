# Comparing `tmp/sigtech-0.0.39.tar.gz` & `tmp/sigtech-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigtech-0.0.39.tar", last modified: Mon Jul 17 15:03:03 2023, max compression
+gzip compressed data, was "sigtech-0.1.0.tar", last modified: Wed Jul 19 11:13:30 2023, max compression
```

## Comparing `sigtech-0.0.39.tar` & `sigtech-0.1.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:03:03.673523 sigtech-0.0.39/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-17 15:02:39.000000 sigtech-0.0.39/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-07-17 15:03:03.669523 sigtech-0.0.39/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-07-17 15:02:39.000000 sigtech-0.0.39/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-17 15:02:39.000000 sigtech-0.0.39/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:03:03.673523 sigtech-0.0.39/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:03:03.665523 sigtech-0.0.39/sigtech/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:03:03.669523 sigtech-0.0.39/sigtech/api/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:03:03.669523 sigtech-0.0.39/sigtech/api/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/client/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:03:03.669523 sigtech-0.0.39/sigtech/api/framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/framework/basket_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/framework/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/framework/framework_api_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/framework/instrument_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/framework/rolling_future_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/framework/signal_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-17 15:02:39.000000 sigtech-0.0.39/sigtech/api/framework/strategy_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:03:03.665523 sigtech-0.0.39/sigtech.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-07-17 15:03:03.000000 sigtech-0.0.39/sigtech.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-17 15:03:03.000000 sigtech-0.0.39/sigtech.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:03:03.000000 sigtech-0.0.39/sigtech.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-17 15:03:03.000000 sigtech-0.0.39/sigtech.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 15:03:03.000000 sigtech-0.0.39/sigtech.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:03:03.669523 sigtech-0.0.39/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-17 15:02:39.000000 sigtech-0.0.39/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-17 15:02:39.000000 sigtech-0.0.39/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-17 15:02:39.000000 sigtech-0.0.39/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-17 15:02:39.000000 sigtech-0.0.39/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:13:30.665811 sigtech-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-19 11:12:56.000000 sigtech-0.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-07-19 11:13:30.665811 sigtech-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-07-19 11:12:56.000000 sigtech-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-19 11:12:56.000000 sigtech-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 11:13:30.665811 sigtech-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:13:30.657811 sigtech-0.1.0/sigtech/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-19 11:12:56.000000 sigtech-0.1.0/sigtech/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:13:30.661811 sigtech-0.1.0/sigtech/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-19 11:12:56.000000 sigtech-0.1.0/sigtech/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:13:30.661811 sigtech-0.1.0/sigtech/api/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 11:12:56.000000 sigtech-0.1.0/sigtech/api/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-19 11:12:56.000000 sigtech-0.1.0/sigtech/api/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-19 11:12:56.000000 sigtech-0.1.0/sigtech/api/client/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-19 11:12:56.000000 sigtech-0.1.0/sigtech/api/client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:13:30.661811 sigtech-0.1.0/sigtech/api/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 11:12:56.000000 sigtech-0.1.0/sigtech/api/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-19 11:12:56.000000 sigtech-0.1.0/sigtech/api/framework/basket_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-19 11:12:56.000000 sigtech-0.1.0/sigtech/api/framework/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-19 11:12:56.000000 sigtech-0.1.0/sigtech/api/framework/framework_api_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-19 11:12:56.000000 sigtech-0.1.0/sigtech/api/framework/instrument_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-19 11:12:56.000000 sigtech-0.1.0/sigtech/api/framework/rolling_future_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-19 11:12:56.000000 sigtech-0.1.0/sigtech/api/framework/signal_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-19 11:12:56.000000 sigtech-0.1.0/sigtech/api/framework/strategy_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:13:30.661811 sigtech-0.1.0/sigtech.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-07-19 11:13:30.000000 sigtech-0.1.0/sigtech.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-19 11:13:30.000000 sigtech-0.1.0/sigtech.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 11:13:30.000000 sigtech-0.1.0/sigtech.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-19 11:13:30.000000 sigtech-0.1.0/sigtech.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-19 11:13:30.000000 sigtech-0.1.0/sigtech.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:13:30.665811 sigtech-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-19 11:12:56.000000 sigtech-0.1.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-19 11:12:56.000000 sigtech-0.1.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-19 11:12:56.000000 sigtech-0.1.0/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-19 11:12:56.000000 sigtech-0.1.0/tests/test_utils.py
```

### Comparing `sigtech-0.0.39/LICENSE.txt` & `sigtech-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.39/PKG-INFO` & `sigtech-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigtech
-Version: 0.0.39
+Version: 0.1.0
 Summary: SigTech Python SDK
 Author-email: SigTech <support@sigtech.com>
 License: MIT
 Project-URL: Homepage, https://github.com/SIGTechnologies/sigtech-python
 Keywords: SIGTECH,FINANCE,TRADING,BACKTEST,QUANT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -105,34 +105,34 @@
 import sigtech.api as sig
 
 # Initialize your session
 sig.init()
 
 # Create a Rolling Future Strategy
 es_future = sig.RollingFutureStrategy(
-    currency='USD',
+    currency="USD",
     start_date="2020-01-04",
-    contract_code='ES', 
-    contract_sector='INDEX',
-    rolling_rule='front',  
-    front_offset='-6:-4', 
+    contract_code="ES", 
+    contract_sector="INDEX",
+    rolling_rule="front",  
+    front_offset="-6:-4", 
 )
 
 # Retrieve the strategy history
 print(es_future.history())
 ```
 ## Next steps
 1. Learn more about the parameters used in the above strategy and how you can tailor them for you own use by reading the documentation for our [Rolling futures strategy](https://learn.sigtech.com/reference/api_post_strategy_rolling_futures_strategies_futures_rolling_post-1) endpoint.
 1. See how our Python SDK can help you quickly create and backtest more complex, real-world trading strategies by folowing the detailed walkthroughs in the [Examples](https://github.com/SIGTechnologies/sigtech-python/tree/master/examples) folder.
 
 >**Tip!**\
 >If you require more low level access to the API, our SDK also offers a **Client based** method of interaction. See [Client based interaction](https://github.com/SIGTechnologies/sigtech-python/blob/master/docs/client_based_interaction.md) for more information.
 
 ## Logging
-Logs down to the `debug` log level are available for all API requests. They can be accessed using the python `logging` library. 
+Logs down to the `debug` log level are available for all API requests. They can be accessed using the Python `logging` library. 
 ```python
 import logging
 logging.basicConfig(level=logging.DEBUG)
 ```
 For more information, please refer to the `logging` library's [documentation](https://docs.python.org/3/library/logging.html). See [Logging in Python](https://realpython.com/python-logging/) for a useful summary of the `logging` library's capabilities.
 
 ## API Documentation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sigtech Version: 0.0.39 Summary: SigTech Python SDK
+Metadata-Version: 2.1 Name: sigtech Version: 0.1.0 Summary: SigTech Python SDK
 Author-email: SigTech
 sigtech.com> License: MIT Project-URL: Homepage, https://github.com/
 SIGTechnologies/sigtech-python Keywords: SIGTECH,FINANCE,TRADING,BACKTEST,QUANT
 Classifier: Development Status :: 5 - Production/Stable Classifier: Operating
 System :: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Financial and Insurance Industry Classifier: Programming Language :: Python
@@ -62,30 +62,30 @@
 first strategy Our SDK provides convenient wrappers for boilerplate functions
 that are required to interact with our API. Copy the following code into your
 IDE and run it to quickly create, backtest and view the performance of a custom
 rolling futures strategy. >**Note!**\ >The example below will only work if you
 have saved your API key as the global environment variable `SIGTECH_API_KEY`.
 ```python # Import the SigTech API import sigtech.api as sig # Initialize your
 session sig.init() # Create a Rolling Future Strategy es_future =
-sig.RollingFutureStrategy( currency='USD', start_date="2020-01-04",
-contract_code='ES', contract_sector='INDEX', rolling_rule='front',
-front_offset='-6:-4', ) # Retrieve the strategy history print(es_future.history
+sig.RollingFutureStrategy( currency="USD", start_date="2020-01-04",
+contract_code="ES", contract_sector="INDEX", rolling_rule="front",
+front_offset="-6:-4", ) # Retrieve the strategy history print(es_future.history
 ()) ``` ## Next steps 1. Learn more about the parameters used in the above
 strategy and how you can tailor them for you own use by reading the
 documentation for our [Rolling futures strategy](https://learn.sigtech.com/
 reference/api_post_strategy_rolling_futures_strategies_futures_rolling_post-1)
 endpoint. 1. See how our Python SDK can help you quickly create and backtest
 more complex, real-world trading strategies by folowing the detailed
 walkthroughs in the [Examples](https://github.com/SIGTechnologies/sigtech-
 python/tree/master/examples) folder. >**Tip!**\ >If you require more low level
 access to the API, our SDK also offers a **Client based** method of
 interaction. See [Client based interaction](https://github.com/SIGTechnologies/
 sigtech-python/blob/master/docs/client_based_interaction.md) for more
 information. ## Logging Logs down to the `debug` log level are available for
-all API requests. They can be accessed using the python `logging` library.
+all API requests. They can be accessed using the Python `logging` library.
 ```python import logging logging.basicConfig(level=logging.DEBUG) ``` For more
 information, please refer to the `logging` library's [documentation](https://
 docs.python.org/3/library/logging.html). See [Logging in Python](https://
 realpython.com/python-logging/) for a useful summary of the `logging` library's
 capabilities. ## API Documentation For detailed information about the SigTech
 API, please refer to our official [API user guide](https://learn.sigtech.com/
 docs) and our interactive [API reference guide](https://learn.sigtech.com/
```

### Comparing `sigtech-0.0.39/README.md` & `sigtech-0.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -77,34 +77,34 @@
 import sigtech.api as sig
 
 # Initialize your session
 sig.init()
 
 # Create a Rolling Future Strategy
 es_future = sig.RollingFutureStrategy(
-    currency='USD',
+    currency="USD",
     start_date="2020-01-04",
-    contract_code='ES', 
-    contract_sector='INDEX',
-    rolling_rule='front',  
-    front_offset='-6:-4', 
+    contract_code="ES", 
+    contract_sector="INDEX",
+    rolling_rule="front",  
+    front_offset="-6:-4", 
 )
 
 # Retrieve the strategy history
 print(es_future.history())
 ```
 ## Next steps
 1. Learn more about the parameters used in the above strategy and how you can tailor them for you own use by reading the documentation for our [Rolling futures strategy](https://learn.sigtech.com/reference/api_post_strategy_rolling_futures_strategies_futures_rolling_post-1) endpoint.
 1. See how our Python SDK can help you quickly create and backtest more complex, real-world trading strategies by folowing the detailed walkthroughs in the [Examples](https://github.com/SIGTechnologies/sigtech-python/tree/master/examples) folder.
 
 >**Tip!**\
 >If you require more low level access to the API, our SDK also offers a **Client based** method of interaction. See [Client based interaction](https://github.com/SIGTechnologies/sigtech-python/blob/master/docs/client_based_interaction.md) for more information.
 
 ## Logging
-Logs down to the `debug` log level are available for all API requests. They can be accessed using the python `logging` library. 
+Logs down to the `debug` log level are available for all API requests. They can be accessed using the Python `logging` library. 
 ```python
 import logging
 logging.basicConfig(level=logging.DEBUG)
 ```
 For more information, please refer to the `logging` library's [documentation](https://docs.python.org/3/library/logging.html). See [Logging in Python](https://realpython.com/python-logging/) for a useful summary of the `logging` library's capabilities.
 
 ## API Documentation
```

#### html2text {}

```diff
@@ -46,30 +46,30 @@
 first strategy Our SDK provides convenient wrappers for boilerplate functions
 that are required to interact with our API. Copy the following code into your
 IDE and run it to quickly create, backtest and view the performance of a custom
 rolling futures strategy. >**Note!**\ >The example below will only work if you
 have saved your API key as the global environment variable `SIGTECH_API_KEY`.
 ```python # Import the SigTech API import sigtech.api as sig # Initialize your
 session sig.init() # Create a Rolling Future Strategy es_future =
-sig.RollingFutureStrategy( currency='USD', start_date="2020-01-04",
-contract_code='ES', contract_sector='INDEX', rolling_rule='front',
-front_offset='-6:-4', ) # Retrieve the strategy history print(es_future.history
+sig.RollingFutureStrategy( currency="USD", start_date="2020-01-04",
+contract_code="ES", contract_sector="INDEX", rolling_rule="front",
+front_offset="-6:-4", ) # Retrieve the strategy history print(es_future.history
 ()) ``` ## Next steps 1. Learn more about the parameters used in the above
 strategy and how you can tailor them for you own use by reading the
 documentation for our [Rolling futures strategy](https://learn.sigtech.com/
 reference/api_post_strategy_rolling_futures_strategies_futures_rolling_post-1)
 endpoint. 1. See how our Python SDK can help you quickly create and backtest
 more complex, real-world trading strategies by folowing the detailed
 walkthroughs in the [Examples](https://github.com/SIGTechnologies/sigtech-
 python/tree/master/examples) folder. >**Tip!**\ >If you require more low level
 access to the API, our SDK also offers a **Client based** method of
 interaction. See [Client based interaction](https://github.com/SIGTechnologies/
 sigtech-python/blob/master/docs/client_based_interaction.md) for more
 information. ## Logging Logs down to the `debug` log level are available for
-all API requests. They can be accessed using the python `logging` library.
+all API requests. They can be accessed using the Python `logging` library.
 ```python import logging logging.basicConfig(level=logging.DEBUG) ``` For more
 information, please refer to the `logging` library's [documentation](https://
 docs.python.org/3/library/logging.html). See [Logging in Python](https://
 realpython.com/python-logging/) for a useful summary of the `logging` library's
 capabilities. ## API Documentation For detailed information about the SigTech
 API, please refer to our official [API user guide](https://learn.sigtech.com/
 docs) and our interactive [API reference guide](https://learn.sigtech.com/
```

### Comparing `sigtech-0.0.39/pyproject.toml` & `sigtech-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sigtech"
-version = "0.0.39"
+version = "0.1.0"
 authors = [
   { name="SigTech", email="support@sigtech.com" },
 ]
 description = "SigTech Python SDK"
 readme = {file = "README.md", content-type = "text/markdown"}
 keywords = ["SIGTECH", "FINANCE", "TRADING", "BACKTEST", "QUANT"]
 license = {text= "MIT"}
@@ -65,15 +65,15 @@
 [tool.setuptools.packages.find]
 exclude = ["tests", "tests.*", "examples", "examples.*"]
 
 [tool.pytest]
 testpaths = ["tests"]
 
 [tool.semantic_release]
-branch = "SA-60_pypi_package"  # TODO :CHANGE
+branch = "master"
 version_variable = "sigtech/api/__init__.py:__version__"
 version_toml = "pyproject.toml:project.version"
 tag_commit = true
 commit_subject = "{version}"
 commit_message = "Automatically generated by python-semantic-release [skip ci]"
 upload_to_repository = false
 upload_to_release = false
```

### Comparing `sigtech-0.0.39/sigtech/api/client/client.py` & `sigtech-0.1.0/sigtech/api/client/client.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.39/sigtech/api/client/response.py` & `sigtech-0.1.0/sigtech/api/client/response.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.39/sigtech/api/client/utils.py` & `sigtech-0.1.0/sigtech/api/client/utils.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.39/sigtech/api/framework/basket_strategy.py` & `sigtech-0.1.0/sigtech/api/framework/basket_strategy.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.39/sigtech/api/framework/environment.py` & `sigtech-0.1.0/sigtech/api/framework/environment.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.39/sigtech/api/framework/framework_api_object.py` & `sigtech-0.1.0/sigtech/api/framework/framework_api_object.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.39/sigtech/api/framework/instrument_base.py` & `sigtech-0.1.0/sigtech/api/framework/instrument_base.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.39/sigtech/api/framework/rolling_future_strategy.py` & `sigtech-0.1.0/sigtech/api/framework/rolling_future_strategy.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.39/sigtech/api/framework/signal_strategy.py` & `sigtech-0.1.0/sigtech/api/framework/signal_strategy.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.39/sigtech/api/framework/strategy_base.py` & `sigtech-0.1.0/sigtech/api/framework/strategy_base.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.39/sigtech.egg-info/PKG-INFO` & `sigtech-0.1.0/sigtech.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigtech
-Version: 0.0.39
+Version: 0.1.0
 Summary: SigTech Python SDK
 Author-email: SigTech <support@sigtech.com>
 License: MIT
 Project-URL: Homepage, https://github.com/SIGTechnologies/sigtech-python
 Keywords: SIGTECH,FINANCE,TRADING,BACKTEST,QUANT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -105,34 +105,34 @@
 import sigtech.api as sig
 
 # Initialize your session
 sig.init()
 
 # Create a Rolling Future Strategy
 es_future = sig.RollingFutureStrategy(
-    currency='USD',
+    currency="USD",
     start_date="2020-01-04",
-    contract_code='ES', 
-    contract_sector='INDEX',
-    rolling_rule='front',  
-    front_offset='-6:-4', 
+    contract_code="ES", 
+    contract_sector="INDEX",
+    rolling_rule="front",  
+    front_offset="-6:-4", 
 )
 
 # Retrieve the strategy history
 print(es_future.history())
 ```
 ## Next steps
 1. Learn more about the parameters used in the above strategy and how you can tailor them for you own use by reading the documentation for our [Rolling futures strategy](https://learn.sigtech.com/reference/api_post_strategy_rolling_futures_strategies_futures_rolling_post-1) endpoint.
 1. See how our Python SDK can help you quickly create and backtest more complex, real-world trading strategies by folowing the detailed walkthroughs in the [Examples](https://github.com/SIGTechnologies/sigtech-python/tree/master/examples) folder.
 
 >**Tip!**\
 >If you require more low level access to the API, our SDK also offers a **Client based** method of interaction. See [Client based interaction](https://github.com/SIGTechnologies/sigtech-python/blob/master/docs/client_based_interaction.md) for more information.
 
 ## Logging
-Logs down to the `debug` log level are available for all API requests. They can be accessed using the python `logging` library. 
+Logs down to the `debug` log level are available for all API requests. They can be accessed using the Python `logging` library. 
 ```python
 import logging
 logging.basicConfig(level=logging.DEBUG)
 ```
 For more information, please refer to the `logging` library's [documentation](https://docs.python.org/3/library/logging.html). See [Logging in Python](https://realpython.com/python-logging/) for a useful summary of the `logging` library's capabilities.
 
 ## API Documentation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sigtech Version: 0.0.39 Summary: SigTech Python SDK
+Metadata-Version: 2.1 Name: sigtech Version: 0.1.0 Summary: SigTech Python SDK
 Author-email: SigTech
 sigtech.com> License: MIT Project-URL: Homepage, https://github.com/
 SIGTechnologies/sigtech-python Keywords: SIGTECH,FINANCE,TRADING,BACKTEST,QUANT
 Classifier: Development Status :: 5 - Production/Stable Classifier: Operating
 System :: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Financial and Insurance Industry Classifier: Programming Language :: Python
@@ -62,30 +62,30 @@
 first strategy Our SDK provides convenient wrappers for boilerplate functions
 that are required to interact with our API. Copy the following code into your
 IDE and run it to quickly create, backtest and view the performance of a custom
 rolling futures strategy. >**Note!**\ >The example below will only work if you
 have saved your API key as the global environment variable `SIGTECH_API_KEY`.
 ```python # Import the SigTech API import sigtech.api as sig # Initialize your
 session sig.init() # Create a Rolling Future Strategy es_future =
-sig.RollingFutureStrategy( currency='USD', start_date="2020-01-04",
-contract_code='ES', contract_sector='INDEX', rolling_rule='front',
-front_offset='-6:-4', ) # Retrieve the strategy history print(es_future.history
+sig.RollingFutureStrategy( currency="USD", start_date="2020-01-04",
+contract_code="ES", contract_sector="INDEX", rolling_rule="front",
+front_offset="-6:-4", ) # Retrieve the strategy history print(es_future.history
 ()) ``` ## Next steps 1. Learn more about the parameters used in the above
 strategy and how you can tailor them for you own use by reading the
 documentation for our [Rolling futures strategy](https://learn.sigtech.com/
 reference/api_post_strategy_rolling_futures_strategies_futures_rolling_post-1)
 endpoint. 1. See how our Python SDK can help you quickly create and backtest
 more complex, real-world trading strategies by folowing the detailed
 walkthroughs in the [Examples](https://github.com/SIGTechnologies/sigtech-
 python/tree/master/examples) folder. >**Tip!**\ >If you require more low level
 access to the API, our SDK also offers a **Client based** method of
 interaction. See [Client based interaction](https://github.com/SIGTechnologies/
 sigtech-python/blob/master/docs/client_based_interaction.md) for more
 information. ## Logging Logs down to the `debug` log level are available for
-all API requests. They can be accessed using the python `logging` library.
+all API requests. They can be accessed using the Python `logging` library.
 ```python import logging logging.basicConfig(level=logging.DEBUG) ``` For more
 information, please refer to the `logging` library's [documentation](https://
 docs.python.org/3/library/logging.html). See [Logging in Python](https://
 realpython.com/python-logging/) for a useful summary of the `logging` library's
 capabilities. ## API Documentation For detailed information about the SigTech
 API, please refer to our official [API user guide](https://learn.sigtech.com/
 docs) and our interactive [API reference guide](https://learn.sigtech.com/
```

### Comparing `sigtech-0.0.39/sigtech.egg-info/SOURCES.txt` & `sigtech-0.1.0/sigtech.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.39/tests/test_client.py` & `sigtech-0.1.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.39/tests/test_examples.py` & `sigtech-0.1.0/tests/test_examples.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,43 +9,45 @@
 SIGTECH_API_KEY = os.environ["SIGTECH_API_KEY"]
 
 EXAMPLES_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), "../examples")
 EXAMPLE_SCRIPTS = [
     os.path.abspath(os.path.join(EXAMPLES_DIR, o)) for o in os.listdir(EXAMPLES_DIR)
 ]
 
-
 README_PATH = os.path.join(os.path.dirname(os.path.abspath(__file__)), "../README.md")
 with open(README_PATH, "r") as f:
     README_BODY = f.read()
 SNIPPETS = re.findall(r"```python([\s\S]*?)```", README_BODY)
 SNIPPETS = [textwrap.dedent(o).strip() for o in SNIPPETS]
 
 
 @pytest.mark.parametrize("script", EXAMPLE_SCRIPTS)
 def test_examples(script):
+    if script.endswith(".py"):
+        cmd = "python {{path}}"
+    elif script.endswith(".ipynb"):
+        cmd = "jupyter nbconvert --execute {{path}} --to notebook"
+    else:
+        raise NotImplementedError(f"Unknown file type {script}")
     with open(script, "r") as f:
         body = f.read()
-    body = body.replace("<YOUR_API_KEY>", SIGTECH_API_KEY)
-    with tempfile.NamedTemporaryFile(mode="w") as fp:
-        fp.write(body)
-        fp.flush()
-        if script.endswith(".py"):
-            stdout = subprocess.check_output(f"python {fp.name}", shell=True)
-        elif script.endswith(".ipynb"):
-            stdout = subprocess.check_output(
-                f"jupyter nbconvert --execute {fp.name} --to notebook", shell=True
-            )
-        else:
-            raise NotImplementedError(f"Unknown file type {script}")
-        print(f"Output: \n{stdout}")
+    _run_script(body, cmd)
 
 
 @pytest.mark.parametrize("snippet", SNIPPETS)
 def test_readme_snippets(snippet):
     print(f"Testing snippet: {snippet}")
-    snippet = snippet.replace("<YOUR_API_KEY>", SIGTECH_API_KEY)
-    with tempfile.NamedTemporaryFile(mode="w") as fp:
-        fp.write(snippet)
-        fp.flush()
-        stdout = subprocess.check_output(f"python {fp.name}", shell=True)
+    _run_script(snippet)
+
+
+def _run_script(script: str, cmd: str = "python {{path}}"):
+    print(f"Running script={script} cmd={cmd}")
+    script = script.replace("<YOUR_API_KEY>", SIGTECH_API_KEY)
+    fp = tempfile.NamedTemporaryFile(mode="w", delete=False)
+    fp.write(script)
+    fp.close()
+    cmd = cmd.replace("{{path}}", fp.name)
+    try:
+        stdout = subprocess.check_output(cmd, shell=True)
+    finally:
+        os.unlink(fp.name)
     print(f"Output: \n{stdout}")
```

### Comparing `sigtech-0.0.39/tests/test_response.py` & `sigtech-0.1.0/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.0.39/tests/test_utils.py` & `sigtech-0.1.0/tests/test_utils.py`

 * *Files identical despite different names*

