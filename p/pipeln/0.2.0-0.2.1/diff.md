# Comparing `tmp/pipeln-0.2.0.tar.gz` & `tmp/pipeln-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeln-0.2.0.tar", last modified: Tue Jul 18 22:09:45 2023, max compression
+gzip compressed data, was "pipeln-0.2.1.tar", last modified: Wed Jul 19 12:34:14 2023, max compression
```

## Comparing `pipeln-0.2.0.tar` & `pipeln-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:09:45.567151 pipeln-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 22:09:33.000000 pipeln-0.2.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-18 22:09:33.000000 pipeln-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-18 22:09:33.000000 pipeln-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-18 22:09:45.567151 pipeln-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:09:45.567151 pipeln-0.2.0/Pipeln/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 22:09:33.000000 pipeln-0.2.0/Pipeln/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-18 22:09:33.000000 pipeln-0.2.0/Pipeln/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-18 22:09:33.000000 pipeln-0.2.0/Pipeln/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-18 22:09:33.000000 pipeln-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:09:45.567151 pipeln-0.2.0/pipeln.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-18 22:09:45.000000 pipeln-0.2.0/pipeln.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-18 22:09:45.000000 pipeln-0.2.0/pipeln.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 22:09:45.000000 pipeln-0.2.0/pipeln.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 22:09:45.000000 pipeln-0.2.0/pipeln.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 22:09:33.000000 pipeln-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 22:09:45.567151 pipeln-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-18 22:09:33.000000 pipeln-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:09:45.567151 pipeln-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-18 22:09:33.000000 pipeln-0.2.0/tests/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:34:14.946137 pipeln-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-19 12:34:02.000000 pipeln-0.2.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-19 12:34:02.000000 pipeln-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-19 12:34:02.000000 pipeln-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-07-19 12:34:14.946137 pipeln-0.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:34:14.942137 pipeln-0.2.1/Pipeln/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-19 12:34:02.000000 pipeln-0.2.1/Pipeln/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-19 12:34:02.000000 pipeln-0.2.1/Pipeln/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-07-19 12:34:02.000000 pipeln-0.2.1/Pipeln/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-19 12:34:02.000000 pipeln-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:34:14.946137 pipeln-0.2.1/pipeln.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-07-19 12:34:14.000000 pipeln-0.2.1/pipeln.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-19 12:34:14.000000 pipeln-0.2.1/pipeln.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:34:14.000000 pipeln-0.2.1/pipeln.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-19 12:34:14.000000 pipeln-0.2.1/pipeln.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:34:02.000000 pipeln-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 12:34:14.946137 pipeln-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-19 12:34:02.000000 pipeln-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:34:14.946137 pipeln-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-19 12:34:02.000000 pipeln-0.2.1/tests/test_pipeline.py
```

### Comparing `pipeln-0.2.0/LICENSE` & `pipeln-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pipeln-0.2.0/PKG-INFO` & `pipeln-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeln
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python package to create a custom pipeline
 Home-page: https://github.com/Adri-Hdez/Pipeln
 Author: Adrián H.S
 Author-email: adrihs.dev@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -55,15 +55,15 @@
 - Create the execution structure.
 - Execute the pipeline.
 
 ```Python
 from Pipeln.pipeline import Pipeline
 from features.auxiliar_test_methods import add, sub, cap
 
-obj = Pipeline(methods=[add, sub, cap], params=[(2, 4), ('1', 2), ('spain',)], orders=[3, 1, 2], debug=True)
+obj = Pipeline(methods=[add, sub, cap], params=[{'a': 2, 'b': 4}, ('1', 2), ('spain',)], orders=[3, 1, 2], debug=True)
 obj.create()
 obj.run()
 ```
 
 Expected output:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pipeln Version: 0.2.0 Summary: A Python package to
+Metadata-Version: 2.1 Name: pipeln Version: 0.2.1 Summary: A Python package to
 create a custom pipeline Home-page: https://github.com/Adri-Hdez/Pipeln Author:
 AdriÃ¡n H.S Author-email: adrihs.dev@gmail.com License: MIT Description-
 Content-Type: text/markdown License-File: LICENSE License-File: AUTHORS.md
                                     [logo]
            A Python open source package to create a custom pipeline
 ---------------------- # ð¾ Installation & Upgrade - Installation: `pip
 install pipeln` - Upgrade: `pip install pipeln --upgrade` # ð¦ What is this?
@@ -20,16 +20,16 @@
 Discusions** | [GitHub Discussions](https://github.com/Adri-Hdez/Pipeln/issues)
 | # âð§â Install & Use Pipeln To start using Pipeln use the next command:
 ```bash pip install pipeln ``` To use the library properly, we follow these
 steps: - Import the library. - Initialize an object of the Pipeln class,
 providing the names and parameters of our methods, and setting the execution
 order. - Create the execution structure. - Execute the pipeline. ```Python from
 Pipeln.pipeline import Pipeline from features.auxiliar_test_methods import add,
-sub, cap obj = Pipeline(methods=[add, sub, cap], params=[(2, 4), ('1', 2),
-('spain',)], orders=[3, 1, 2], debug=True) obj.create() obj.run() ``` Expected
-output: ```bash DEBUG: ***************************** DEBUG: > Starting pipeline
-DEBUG: DEBUG: EXEC: Method add executed successfully. ERROR: ERROR: There is an
-error in sub method. Inappropiate argument type. DEBUG: EXEC: Method cap
-executed successfully. DEBUG: DEBUG: Pipeline finished in 10.9 DEBUG:
-***************************** ``` # ð³ License Pipeln is licensed under [MIT
-License](LICENSE). # ðï¸ Shields
+sub, cap obj = Pipeline(methods=[add, sub, cap], params=[{'a': 2, 'b': 4},
+('1', 2), ('spain',)], orders=[3, 1, 2], debug=True) obj.create() obj.run() ```
+Expected output: ```bash DEBUG: ***************************** DEBUG: > Starting
+pipeline DEBUG: DEBUG: EXEC: Method add executed successfully. ERROR: ERROR:
+There is an error in sub method. Inappropiate argument type. DEBUG: EXEC:
+Method cap executed successfully. DEBUG: DEBUG: Pipeline finished in 10.9
+DEBUG: ***************************** ``` # ð³ License Pipeln is licensed
+under [MIT License](LICENSE). # ðï¸ Shields
                     [PyPI] [downloads] [versions] [license]
```

### Comparing `pipeln-0.2.0/Pipeln/__init__.py` & `pipeln-0.2.1/Pipeln/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeln-0.2.0/Pipeln/pipeline.py` & `pipeln-0.2.1/Pipeln/pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import final
+from typing import final, Union
 import logging
 import time
 
 class Pipeline:
   """
   Class for the creation of a custom pipeline, 
   which will sequentially execute the methods passed to the constructor.
@@ -16,15 +16,15 @@
   :param orders: Is a collection of integers that assign a specific execution order to the methods in the pipeline. The methods are executed based on the order specified in this list, allowing for a customized execution flow.
   :type orders: list[int]
   
   :param debug: Pipeline methods info.
   :type debug: bool
   """
 
-  def __init__(self, methods: list[object] = None, params: list[tuple] = None, orders: list[int] = None, debug: bool = False) -> None:
+  def __init__(self, methods: list[object] = None, params: list[Union[tuple, dict]] = None, orders: list[int] = None, debug: bool = False) -> None:
     self._methods = methods
     self._params = params
     self._orders = orders
     self._debug = debug
 
     self._stacks = [] # combination of methods and params
   
@@ -74,18 +74,22 @@
     # ----------------------------- Main functionality -----------------------------
     # Check if nulls & variables lenght
     if (self._methods or self._params or self._orders) is None:
       raise ValueError("Innapropiate argument value, check if there is any None object.")
     if len(self._methods) != len(self._orders) != len(self._params):
       raise ValueError("Inappropiate argument value, check parameters length. There is a missing value.")
     
+    for value in self._params:
+      print('aaaaaa')
+      print(type(value))
+
     # Check argument values
     if not all(isinstance(value, object) for value in self._methods): 
       raise ValueError("Inappropiate methods argument value.")
-    if not all(isinstance(value, tuple) for value in self._params): 
+    if not all(isinstance(value, (tuple, dict)) for value in self._params): 
       raise ValueError("Inappropiate params argument value.")
     if  not all(isinstance(value, int) for value in self._orders): 
       raise ValueError("Inappropiate order argument value.")
 
     # Create functions stack
     for func, parms in zip(self._methods, self._params):
       combination = (func, parms)
@@ -106,16 +110,20 @@
     if self._debug: logging.debug('        > Starting pipeline        ')
     if self._debug: logging.debug('')
 
     ordered_methods = [x for _, x in sorted(zip(orders, methods))]
 
     for func, params in ordered_methods:
       try:
-        func(*params)
-        if self._debug: logging.debug(f'EXEC: Method \033[94m{str(func.__name__)}\033[0m executed successfully.')
+        if type(params) is tuple:
+          func(*params)
+          if self._debug: logging.debug(f'EXEC: Method \033[94m{str(func.__name__)}\033[0m executed successfully.')
+        else:
+          func(**params)
+          if self._debug: logging.debug(f'EXEC: Method \033[94m{str(func.__name__)}\033[0m executed successfully.')
       except TypeError:
         logging.error(f'ERROR: There is an error in \033[91m{str(func.__name__)}\033[0m method. Inappropiate argument type.')
 
     finish_time = time.time() - start_time
     if self._debug: logging.debug('')
     if self._debug: logging.debug(f'     Pipeline finished in {round(finish_time, 1)}s     ')
     if self._debug: logging.debug('***********************************')
```

### Comparing `pipeln-0.2.0/README.md` & `pipeln-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 - Create the execution structure.
 - Execute the pipeline.
 
 ```Python
 from Pipeln.pipeline import Pipeline
 from features.auxiliar_test_methods import add, sub, cap
 
-obj = Pipeline(methods=[add, sub, cap], params=[(2, 4), ('1', 2), ('spain',)], orders=[3, 1, 2], debug=True)
+obj = Pipeline(methods=[add, sub, cap], params=[{'a': 2, 'b': 4}, ('1', 2), ('spain',)], orders=[3, 1, 2], debug=True)
 obj.create()
 obj.run()
 ```
 
 Expected output:
```

#### html2text {}

```diff
@@ -16,16 +16,16 @@
 Discusions** | [GitHub Discussions](https://github.com/Adri-Hdez/Pipeln/issues)
 | # âð§â Install & Use Pipeln To start using Pipeln use the next command:
 ```bash pip install pipeln ``` To use the library properly, we follow these
 steps: - Import the library. - Initialize an object of the Pipeln class,
 providing the names and parameters of our methods, and setting the execution
 order. - Create the execution structure. - Execute the pipeline. ```Python from
 Pipeln.pipeline import Pipeline from features.auxiliar_test_methods import add,
-sub, cap obj = Pipeline(methods=[add, sub, cap], params=[(2, 4), ('1', 2),
-('spain',)], orders=[3, 1, 2], debug=True) obj.create() obj.run() ``` Expected
-output: ```bash DEBUG: ***************************** DEBUG: > Starting pipeline
-DEBUG: DEBUG: EXEC: Method add executed successfully. ERROR: ERROR: There is an
-error in sub method. Inappropiate argument type. DEBUG: EXEC: Method cap
-executed successfully. DEBUG: DEBUG: Pipeline finished in 10.9 DEBUG:
-***************************** ``` # ð³ License Pipeln is licensed under [MIT
-License](LICENSE). # ðï¸ Shields
+sub, cap obj = Pipeline(methods=[add, sub, cap], params=[{'a': 2, 'b': 4},
+('1', 2), ('spain',)], orders=[3, 1, 2], debug=True) obj.create() obj.run() ```
+Expected output: ```bash DEBUG: ***************************** DEBUG: > Starting
+pipeline DEBUG: DEBUG: EXEC: Method add executed successfully. ERROR: ERROR:
+There is an error in sub method. Inappropiate argument type. DEBUG: EXEC:
+Method cap executed successfully. DEBUG: DEBUG: Pipeline finished in 10.9
+DEBUG: ***************************** ``` # ð³ License Pipeln is licensed
+under [MIT License](LICENSE). # ðï¸ Shields
                     [PyPI] [downloads] [versions] [license]
```

### Comparing `pipeln-0.2.0/pipeln.egg-info/PKG-INFO` & `pipeln-0.2.1/pipeln.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeln
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python package to create a custom pipeline
 Home-page: https://github.com/Adri-Hdez/Pipeln
 Author: Adrián H.S
 Author-email: adrihs.dev@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -55,15 +55,15 @@
 - Create the execution structure.
 - Execute the pipeline.
 
 ```Python
 from Pipeln.pipeline import Pipeline
 from features.auxiliar_test_methods import add, sub, cap
 
-obj = Pipeline(methods=[add, sub, cap], params=[(2, 4), ('1', 2), ('spain',)], orders=[3, 1, 2], debug=True)
+obj = Pipeline(methods=[add, sub, cap], params=[{'a': 2, 'b': 4}, ('1', 2), ('spain',)], orders=[3, 1, 2], debug=True)
 obj.create()
 obj.run()
 ```
 
 Expected output:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pipeln Version: 0.2.0 Summary: A Python package to
+Metadata-Version: 2.1 Name: pipeln Version: 0.2.1 Summary: A Python package to
 create a custom pipeline Home-page: https://github.com/Adri-Hdez/Pipeln Author:
 AdriÃ¡n H.S Author-email: adrihs.dev@gmail.com License: MIT Description-
 Content-Type: text/markdown License-File: LICENSE License-File: AUTHORS.md
                                     [logo]
            A Python open source package to create a custom pipeline
 ---------------------- # ð¾ Installation & Upgrade - Installation: `pip
 install pipeln` - Upgrade: `pip install pipeln --upgrade` # ð¦ What is this?
@@ -20,16 +20,16 @@
 Discusions** | [GitHub Discussions](https://github.com/Adri-Hdez/Pipeln/issues)
 | # âð§â Install & Use Pipeln To start using Pipeln use the next command:
 ```bash pip install pipeln ``` To use the library properly, we follow these
 steps: - Import the library. - Initialize an object of the Pipeln class,
 providing the names and parameters of our methods, and setting the execution
 order. - Create the execution structure. - Execute the pipeline. ```Python from
 Pipeln.pipeline import Pipeline from features.auxiliar_test_methods import add,
-sub, cap obj = Pipeline(methods=[add, sub, cap], params=[(2, 4), ('1', 2),
-('spain',)], orders=[3, 1, 2], debug=True) obj.create() obj.run() ``` Expected
-output: ```bash DEBUG: ***************************** DEBUG: > Starting pipeline
-DEBUG: DEBUG: EXEC: Method add executed successfully. ERROR: ERROR: There is an
-error in sub method. Inappropiate argument type. DEBUG: EXEC: Method cap
-executed successfully. DEBUG: DEBUG: Pipeline finished in 10.9 DEBUG:
-***************************** ``` # ð³ License Pipeln is licensed under [MIT
-License](LICENSE). # ðï¸ Shields
+sub, cap obj = Pipeline(methods=[add, sub, cap], params=[{'a': 2, 'b': 4},
+('1', 2), ('spain',)], orders=[3, 1, 2], debug=True) obj.create() obj.run() ```
+Expected output: ```bash DEBUG: ***************************** DEBUG: > Starting
+pipeline DEBUG: DEBUG: EXEC: Method add executed successfully. ERROR: ERROR:
+There is an error in sub method. Inappropiate argument type. DEBUG: EXEC:
+Method cap executed successfully. DEBUG: DEBUG: Pipeline finished in 10.9
+DEBUG: ***************************** ``` # ð³ License Pipeln is licensed
+under [MIT License](LICENSE). # ðï¸ Shields
                     [PyPI] [downloads] [versions] [license]
```

### Comparing `pipeln-0.2.0/setup.py` & `pipeln-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `pipeln-0.2.0/tests/test_pipeline.py` & `pipeln-0.2.1/tests/test_pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,31 +17,31 @@
     methods = obj.get_methods
 
     self.assertEqual(methods, ['add', 'sub', 'cap'])
   
   def test_pipeline_get_params(self):
     obj = Pipeline(methods=[add, sub, cap], params=[(2, 4), (1, 2), ('spain',)], orders=[3, 1, 2])
     params = obj.get_params
-    print(type(params[2]))
+
     self.assertEqual(params, [(2, 4), (1, 2), ('spain',)])
   
   def test_pipeline_get_orders(self):
     obj = Pipeline(methods=[add, sub, cap], params=[(2, 4), (1, 2), ('spain',)], orders=[3, 1, 2])
     orders = obj.get_orders
 
     self.assertEqual(orders, [3, 1, 2])
   
   def test_pipeline_creation(self):
     obj = Pipeline(methods=[add, sub, cap], params=[(2, 4), (1, 2), ('spain',)], orders=[3, 1, 2])
     obj.create()
     
     self.assertIsNotNone(obj) # This method doesn't returns
-  
+
   def test_pipeline_execution(self):
-    obj = Pipeline(methods=[add, sub, cap], params=[(2, 4), (1, 2), ('spain',)], orders=[3, 1, 2])
+    obj = Pipeline(methods=[add, sub, cap], params=[{'a': 2, 'b': 4}, (1, 2), ('spain',)], orders=[1, 2, 3])
     obj.create()
     obj.run()
     
     self.assertIsNotNone(obj) # This method doesn't returns
 
 if __name__ == '__main__':
   unittest.main()
```

