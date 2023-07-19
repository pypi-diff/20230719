# Comparing `tmp/rulekit-1.6.0.tar.gz` & `tmp/rulekit-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rulekit-1.6.0.tar", last modified: Tue Jun 15 13:17:02 2021, max compression
+gzip compressed data, was "rulekit-1.6.1.tar", last modified: Wed Jul 19 13:20:38 2023, max compression
```

## Comparing `rulekit-1.6.0.tar` & `rulekit-1.6.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxrwx   0        0        0        0 2021-06-15 13:17:02.464057 rulekit-1.6.0/
--rw-rw-rw-   0        0        0       98 2021-06-15 13:10:11.000000 rulekit-1.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3117 2021-06-15 13:17:02.465057 rulekit-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     1502 2021-06-12 17:05:31.000000 rulekit-1.6.0/README.md
-drwxrwxrwx   0        0        0        0 2021-06-15 13:17:02.429057 rulekit-1.6.0/rulekit/
--rw-rw-rw-   0        0        0       67 2021-06-15 13:05:54.000000 rulekit-1.6.0/rulekit/__init__.py
--rw-rw-rw-   0        0        0     2384 2021-06-15 12:53:04.000000 rulekit-1.6.0/rulekit/__main__.py
--rw-rw-rw-   0        0        0    19239 2021-06-15 12:26:03.000000 rulekit-1.6.0/rulekit/classification.py
--rw-rw-rw-   0        0        0      253 2021-03-29 06:27:59.000000 rulekit-1.6.0/rulekit/experiment.py
--rw-rw-rw-   0        0        0    14957 2021-06-15 12:29:48.000000 rulekit-1.6.0/rulekit/helpers.py
-drwxrwxrwx   0        0        0        0 2021-06-15 13:17:02.443058 rulekit-1.6.0/rulekit/jar/
--rw-rw-rw-   0        0        0        0 2021-03-29 06:27:59.000000 rulekit-1.6.0/rulekit/jar/__init__.py
--rw-rw-rw-   0        0        0  1234599 2021-04-14 06:33:18.000000 rulekit-1.6.0/rulekit/jar/mockito-all-1.10.19.jar
--rw-rw-rw-   0        0        0     4134 2021-05-25 06:10:46.000000 rulekit-1.6.0/rulekit/main.py
--rw-rw-rw-   0        0        0    13638 2021-06-15 12:32:09.000000 rulekit-1.6.0/rulekit/operator.py
--rw-rw-rw-   0        0        0     1535 2021-06-15 13:06:48.000000 rulekit-1.6.0/rulekit/params.py
--rw-rw-rw-   0        0        0    13280 2021-06-15 12:48:21.000000 rulekit-1.6.0/rulekit/regression.py
--rw-rw-rw-   0        0        0     8243 2021-06-15 12:49:32.000000 rulekit-1.6.0/rulekit/rules.py
--rw-rw-rw-   0        0        0     5149 2021-06-15 13:06:47.000000 rulekit-1.6.0/rulekit/stats.py
--rw-rw-rw-   0        0        0    18569 2021-06-15 12:42:36.000000 rulekit-1.6.0/rulekit/survival.py
-drwxrwxrwx   0        0        0        0 2021-06-15 13:17:02.440057 rulekit-1.6.0/rulekit.egg-info/
--rw-rw-rw-   0        0        0     3117 2021-06-15 13:17:02.000000 rulekit-1.6.0/rulekit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      721 2021-06-15 13:17:02.000000 rulekit-1.6.0/rulekit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-15 13:17:02.000000 rulekit-1.6.0/rulekit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2021-06-15 13:17:02.000000 rulekit-1.6.0/rulekit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2021-06-15 13:17:02.000000 rulekit-1.6.0/rulekit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2021-06-15 13:17:02.466057 rulekit-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1728 2021-06-15 13:15:21.000000 rulekit-1.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2021-06-15 13:17:02.463056 rulekit-1.6.0/tests/
--rw-rw-rw-   0        0        0      101 2021-03-29 06:27:59.000000 rulekit-1.6.0/tests/__init__.py
--rw-rw-rw-   0        0        0     2563 2021-05-25 06:10:46.000000 rulekit-1.6.0/tests/resources.py
--rw-rw-rw-   0        0        0     5661 2021-06-11 15:24:08.000000 rulekit-1.6.0/tests/test_classifier.py
--rw-rw-rw-   0        0        0     2042 2021-06-11 15:24:08.000000 rulekit-1.6.0/tests/test_regression.py
--rw-rw-rw-   0        0        0      883 2021-03-29 06:27:59.000000 rulekit-1.6.0/tests/test_rulekit.py
--rw-rw-rw-   0        0        0     5881 2021-06-11 15:24:08.000000 rulekit-1.6.0/tests/test_serialization.py
--rw-rw-rw-   0        0        0     1128 2021-05-25 06:10:46.000000 rulekit-1.6.0/tests/test_sklearn_metrics.py
--rw-rw-rw-   0        0        0      622 2021-03-29 06:27:59.000000 rulekit-1.6.0/tests/test_statistics.py
--rw-rw-rw-   0        0        0     1959 2021-06-11 15:24:08.000000 rulekit-1.6.0/tests/test_survival.py
--rw-rw-rw-   0        0        0    15234 2021-05-25 06:10:46.000000 rulekit-1.6.0/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-19 13:20:38.663004 rulekit-1.6.1/
+-rw-rw-rw-   0        0        0    35179 2023-07-19 12:51:13.000000 rulekit-1.6.1/LICENSE
+-rw-rw-rw-   0        0        0       98 2023-07-19 12:51:13.000000 rulekit-1.6.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2650 2023-07-19 13:20:38.663004 rulekit-1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1502 2023-07-19 12:51:13.000000 rulekit-1.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 13:20:38.617260 rulekit-1.6.1/rulekit/
+-rw-rw-rw-   0        0        0       71 2023-07-19 13:20:20.000000 rulekit-1.6.1/rulekit/__init__.py
+-rw-rw-rw-   0        0        0     2384 2023-07-19 12:58:02.000000 rulekit-1.6.1/rulekit/__main__.py
+-rw-rw-rw-   0        0        0    19239 2023-07-19 12:58:02.000000 rulekit-1.6.1/rulekit/classification.py
+-rw-rw-rw-   0        0        0      263 2023-07-19 12:58:02.000000 rulekit-1.6.1/rulekit/experiment.py
+-rw-rw-rw-   0        0        0    14957 2023-07-19 12:58:02.000000 rulekit-1.6.1/rulekit/helpers.py
+drwxrwxrwx   0        0        0        0 2023-07-19 13:20:38.642344 rulekit-1.6.1/rulekit/jar/
+-rw-rw-rw-   0        0        0        0 2023-07-19 12:51:13.000000 rulekit-1.6.1/rulekit/jar/__init__.py
+-rw-rw-rw-   0        0        0  1234599 2023-07-19 12:51:13.000000 rulekit-1.6.1/rulekit/jar/mockito-all-1.10.19.jar
+-rw-rw-rw-   0        0        0     4134 2023-07-19 12:58:02.000000 rulekit-1.6.1/rulekit/main.py
+-rw-rw-rw-   0        0        0    13638 2023-07-19 12:58:02.000000 rulekit-1.6.1/rulekit/operator.py
+-rw-rw-rw-   0        0        0     1535 2023-07-19 12:58:02.000000 rulekit-1.6.1/rulekit/params.py
+-rw-rw-rw-   0        0        0    13280 2023-07-19 12:58:02.000000 rulekit-1.6.1/rulekit/regression.py
+-rw-rw-rw-   0        0        0     8243 2023-07-19 12:58:02.000000 rulekit-1.6.1/rulekit/rules.py
+-rw-rw-rw-   0        0        0     5149 2023-07-19 12:58:02.000000 rulekit-1.6.1/rulekit/stats.py
+-rw-rw-rw-   0        0        0    18569 2023-07-19 12:58:02.000000 rulekit-1.6.1/rulekit/survival.py
+drwxrwxrwx   0        0        0        0 2023-07-19 13:20:38.637393 rulekit-1.6.1/rulekit.egg-info/
+-rw-rw-rw-   0        0        0     2650 2023-07-19 13:20:38.000000 rulekit-1.6.1/rulekit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      729 2023-07-19 13:20:38.000000 rulekit-1.6.1/rulekit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 13:20:38.000000 rulekit-1.6.1/rulekit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-19 13:20:38.000000 rulekit-1.6.1/rulekit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-19 13:20:38.000000 rulekit-1.6.1/rulekit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-19 13:20:38.668093 rulekit-1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1780 2023-07-19 13:20:15.000000 rulekit-1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 13:20:38.661721 rulekit-1.6.1/tests/
+-rw-rw-rw-   0        0        0      107 2023-07-19 12:51:13.000000 rulekit-1.6.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     2633 2023-07-19 12:58:02.000000 rulekit-1.6.1/tests/resources.py
+-rw-rw-rw-   0        0        0     5807 2023-07-19 12:58:02.000000 rulekit-1.6.1/tests/test_classifier.py
+-rw-rw-rw-   0        0        0     2098 2023-07-19 12:51:13.000000 rulekit-1.6.1/tests/test_regression.py
+-rw-rw-rw-   0        0        0      909 2023-07-19 12:51:13.000000 rulekit-1.6.1/tests/test_rulekit.py
+-rw-rw-rw-   0        0        0     5881 2023-07-19 12:51:13.000000 rulekit-1.6.1/tests/test_serialization.py
+-rw-rw-rw-   0        0        0     1163 2023-07-19 12:51:13.000000 rulekit-1.6.1/tests/test_sklearn_metrics.py
+-rw-rw-rw-   0        0        0      649 2023-07-19 12:51:13.000000 rulekit-1.6.1/tests/test_statistics.py
+-rw-rw-rw-   0        0        0     2013 2023-07-19 12:51:13.000000 rulekit-1.6.1/tests/test_survival.py
+-rw-rw-rw-   0        0        0    15636 2023-07-19 12:58:02.000000 rulekit-1.6.1/tests/utils.py
```

### Comparing `rulekit-1.6.0/PKG-INFO` & `rulekit-1.6.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,80 @@
 Metadata-Version: 2.1
 Name: rulekit
-Version: 1.6.0
+Version: 1.6.1
 Summary: Comprehensive suite for rule-based learning
 Home-page: https://github.com/adaa-polsl/RuleKit
+Download-URL: https://github.com/adaa-polsl/RuleKit-python/archive/refs/tags/v1.6.0.tar.gz
 Author: Cezary Maszczyk
 Author-email: cezary.maszczyk@gmail.com
-License: UNKNOWN
-Download-URL: https://github.com/adaa-polsl/RuleKit-python/archive/refs/tags/v1.6.0.tar.gz
 Project-URL: Bug Tracker, https://github.com/adaa-polsl/RuleKit-python/issues
 Project-URL: Documentation, https://adaa-polsl.github.io/RuleKit-python/
 Project-URL: Source Code, https://github.com/adaa-polsl/RuleKit-python
-Description: # Rulekit
-         
-        This package is python wrapper for [RuleKit](https://github.com/adaa-polsl/RuleKit) library - a versatile tool for rule learning. 
-         
-        Based on a sequential covering induction algorithm, it is suitable for classification, regression, and survival problems.
-         
-        ## Installation
-         
-        > **NOTE**: 
-        This package is a wrapper for Java library, it requires Java (version 1.8.0 tested) to be installed on the computer. Both Open JDK and Oracle implementations are supported.
-        ## 
-         
-        ```bash
-        pip install rulekit
-         
-        # after installation
-        python -m rulekit download_jar
-        ```
-         
-        The second command will fetch the latest RuleKit library jar file from its Github releases page. It is required to use this package.
-         
-        ## Running tests
-         
-        If you're running tests for the first time (or you want to update existing tests resources) you need to download tests resources from RuleKit repository. You can do it by running:
-        ```
-        python tests/resources.py download
-        ```
-        Runing tests:    
-        In directory where `setup.py` file exists.
-        ```
-        python -m unittest discover ./tests
-        ```
-         
-        ## Sample usage
-         
-        ```python
-        from rulekit import RuleKit
-        from rulekit.classification import RuleClassifier
-        from sklearn.datasets import load_iris
-         
-        RuleKit.init()
-         
-        x, y = load_iris(return_X_y=True)
-         
-        clf = RuleClassifier()
-        clf.fit(x, y)
-        prediction = clf.predict(x)
-         
-        print(prediction)
-        ```
-         
-        ## Documentation
-         
-        Full documentation is available [here](https://adaa-polsl.github.io/RuleKit-python/)
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Java
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Rulekit
+ 
+This package is python wrapper for [RuleKit](https://github.com/adaa-polsl/RuleKit) library - a versatile tool for rule learning. 
+ 
+Based on a sequential covering induction algorithm, it is suitable for classification, regression, and survival problems.
+ 
+## Installation
+ 
+> **NOTE**: 
+This package is a wrapper for Java library, it requires Java (version 1.8.0 tested) to be installed on the computer. Both Open JDK and Oracle implementations are supported.
+## 
+ 
+```bash
+pip install rulekit
+ 
+# after installation
+python -m rulekit download_jar
+```
+ 
+The second command will fetch the latest RuleKit library jar file from its Github releases page. It is required to use this package.
+ 
+## Running tests
+ 
+If you're running tests for the first time (or you want to update existing tests resources) you need to download tests resources from RuleKit repository. You can do it by running:
+```
+python tests/resources.py download
+```
+Runing tests:    
+In directory where `setup.py` file exists.
+```
+python -m unittest discover ./tests
+```
+ 
+## Sample usage
+ 
+```python
+from rulekit import RuleKit
+from rulekit.classification import RuleClassifier
+from sklearn.datasets import load_iris
+ 
+RuleKit.init()
+ 
+x, y = load_iris(return_X_y=True)
+ 
+clf = RuleClassifier()
+clf.fit(x, y)
+prediction = clf.predict(x)
+ 
+print(prediction)
+```
+ 
+## Documentation
+ 
+Full documentation is available [here](https://adaa-polsl.github.io/RuleKit-python/)
+
```

### Comparing `rulekit-1.6.0/README.md` & `rulekit-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.0/rulekit/__main__.py` & `rulekit-1.6.1/rulekit/__main__.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.0/rulekit/classification.py` & `rulekit-1.6.1/rulekit/classification.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.0/rulekit/helpers.py` & `rulekit-1.6.1/rulekit/helpers.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.0/rulekit/jar/mockito-all-1.10.19.jar` & `rulekit-1.6.1/rulekit/jar/mockito-all-1.10.19.jar`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.0/rulekit/main.py` & `rulekit-1.6.1/rulekit/main.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.0/rulekit/operator.py` & `rulekit-1.6.1/rulekit/operator.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.0/rulekit/params.py` & `rulekit-1.6.1/rulekit/params.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.0/rulekit/regression.py` & `rulekit-1.6.1/rulekit/regression.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.0/rulekit/rules.py` & `rulekit-1.6.1/rulekit/rules.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.0/rulekit/stats.py` & `rulekit-1.6.1/rulekit/stats.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.0/rulekit/survival.py` & `rulekit-1.6.1/rulekit/survival.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.0/rulekit.egg-info/PKG-INFO` & `rulekit-1.6.1/rulekit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,80 @@
 Metadata-Version: 2.1
 Name: rulekit
-Version: 1.6.0
+Version: 1.6.1
 Summary: Comprehensive suite for rule-based learning
 Home-page: https://github.com/adaa-polsl/RuleKit
+Download-URL: https://github.com/adaa-polsl/RuleKit-python/archive/refs/tags/v1.6.0.tar.gz
 Author: Cezary Maszczyk
 Author-email: cezary.maszczyk@gmail.com
-License: UNKNOWN
-Download-URL: https://github.com/adaa-polsl/RuleKit-python/archive/refs/tags/v1.6.0.tar.gz
 Project-URL: Bug Tracker, https://github.com/adaa-polsl/RuleKit-python/issues
 Project-URL: Documentation, https://adaa-polsl.github.io/RuleKit-python/
 Project-URL: Source Code, https://github.com/adaa-polsl/RuleKit-python
-Description: # Rulekit
-         
-        This package is python wrapper for [RuleKit](https://github.com/adaa-polsl/RuleKit) library - a versatile tool for rule learning. 
-         
-        Based on a sequential covering induction algorithm, it is suitable for classification, regression, and survival problems.
-         
-        ## Installation
-         
-        > **NOTE**: 
-        This package is a wrapper for Java library, it requires Java (version 1.8.0 tested) to be installed on the computer. Both Open JDK and Oracle implementations are supported.
-        ## 
-         
-        ```bash
-        pip install rulekit
-         
-        # after installation
-        python -m rulekit download_jar
-        ```
-         
-        The second command will fetch the latest RuleKit library jar file from its Github releases page. It is required to use this package.
-         
-        ## Running tests
-         
-        If you're running tests for the first time (or you want to update existing tests resources) you need to download tests resources from RuleKit repository. You can do it by running:
-        ```
-        python tests/resources.py download
-        ```
-        Runing tests:    
-        In directory where `setup.py` file exists.
-        ```
-        python -m unittest discover ./tests
-        ```
-         
-        ## Sample usage
-         
-        ```python
-        from rulekit import RuleKit
-        from rulekit.classification import RuleClassifier
-        from sklearn.datasets import load_iris
-         
-        RuleKit.init()
-         
-        x, y = load_iris(return_X_y=True)
-         
-        clf = RuleClassifier()
-        clf.fit(x, y)
-        prediction = clf.predict(x)
-         
-        print(prediction)
-        ```
-         
-        ## Documentation
-         
-        Full documentation is available [here](https://adaa-polsl.github.io/RuleKit-python/)
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Java
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Rulekit
+ 
+This package is python wrapper for [RuleKit](https://github.com/adaa-polsl/RuleKit) library - a versatile tool for rule learning. 
+ 
+Based on a sequential covering induction algorithm, it is suitable for classification, regression, and survival problems.
+ 
+## Installation
+ 
+> **NOTE**: 
+This package is a wrapper for Java library, it requires Java (version 1.8.0 tested) to be installed on the computer. Both Open JDK and Oracle implementations are supported.
+## 
+ 
+```bash
+pip install rulekit
+ 
+# after installation
+python -m rulekit download_jar
+```
+ 
+The second command will fetch the latest RuleKit library jar file from its Github releases page. It is required to use this package.
+ 
+## Running tests
+ 
+If you're running tests for the first time (or you want to update existing tests resources) you need to download tests resources from RuleKit repository. You can do it by running:
+```
+python tests/resources.py download
+```
+Runing tests:    
+In directory where `setup.py` file exists.
+```
+python -m unittest discover ./tests
+```
+ 
+## Sample usage
+ 
+```python
+from rulekit import RuleKit
+from rulekit.classification import RuleClassifier
+from sklearn.datasets import load_iris
+ 
+RuleKit.init()
+ 
+x, y = load_iris(return_X_y=True)
+ 
+clf = RuleClassifier()
+clf.fit(x, y)
+prediction = clf.predict(x)
+ 
+print(prediction)
+```
+ 
+## Documentation
+ 
+Full documentation is available [here](https://adaa-polsl.github.io/RuleKit-python/)
+
```

### Comparing `rulekit-1.6.0/rulekit.egg-info/SOURCES.txt` & `rulekit-1.6.1/rulekit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 rulekit/__init__.py
 rulekit/__main__.py
 rulekit/classification.py
```

### Comparing `rulekit-1.6.0/setup.py` & `rulekit-1.6.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-import setuptools
-import os
-import io
-
-current_path = os.path.dirname(os.path.realpath(__file__))
-
-with io.open("README.md", mode="r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="rulekit",
-    version='1.6.0',
-    author="Cezary Maszczyk",
-    author_email="cezary.maszczyk@gmail.com",
-    description="Comprehensive suite for rule-based learning",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/adaa-polsl/RuleKit",
-    packages=setuptools.find_packages(),
-    classifiers=[
-        "Development Status :: 4 - Beta",
-        "License :: OSI Approved :: GNU Affero General Public License v3",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Java",
-        "Operating System :: Microsoft :: Windows",
-        "Operating System :: Unix",
-        "Topic :: Scientific/Engineering",
-        "Topic :: Scientific/Engineering :: Artificial Intelligence",
-        "Intended Audience :: Developers",
-        "Intended Audience :: Science/Research",
-    ],
-    include_package_data = True,
-    python_requires='>=3.6',
-    install_requires=[
-        "pandas ~= 1.2.1",
-        "scikit-learn ~= 0.24.1",
-        "requests ~= 2.25.1",
-        "scipy ~= 1.6.0",
-        "joblib ~= 1.0.0",
-        "JPype1 ~= 1.2.1",
-    ],
-    test_suite="tests",
-    download_url = 'https://github.com/adaa-polsl/RuleKit-python/archive/refs/tags/v1.6.0.tar.gz',
-    project_urls={
-        'Bug Tracker': 'https://github.com/adaa-polsl/RuleKit-python/issues',
-        'Documentation': 'https://adaa-polsl.github.io/RuleKit-python/',
-        'Source Code': 'https://github.com/adaa-polsl/RuleKit-python'
-    }
-)
+import setuptools
+import os
+import io
+
+current_path = os.path.dirname(os.path.realpath(__file__))
+
+with io.open("README.md", mode="r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="rulekit",
+    version='1.6.1',
+    author="Cezary Maszczyk",
+    author_email="cezary.maszczyk@gmail.com",
+    description="Comprehensive suite for rule-based learning",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/adaa-polsl/RuleKit",
+    packages=setuptools.find_packages(),
+    classifiers=[
+        "Development Status :: 4 - Beta",
+        "License :: OSI Approved :: GNU Affero General Public License v3",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Java",
+        "Operating System :: Microsoft :: Windows",
+        "Operating System :: Unix",
+        "Topic :: Scientific/Engineering",
+        "Topic :: Scientific/Engineering :: Artificial Intelligence",
+        "Intended Audience :: Developers",
+        "Intended Audience :: Science/Research",
+    ],
+    include_package_data = True,
+    python_requires='>=3.6',
+    install_requires=[
+        "pandas ~= 1.5.3",
+        "scikit-learn ~= 1.2.0",
+        "requests ~= 2.25.1",
+        "scipy ~= 1.9.3",
+        "joblib >= 1.0,< 1.3",
+        "JPype1 ~= 1.4.1",
+    ],
+    test_suite="tests",
+    download_url = 'https://github.com/adaa-polsl/RuleKit-python/archive/refs/tags/v1.6.0.tar.gz',
+    project_urls={
+        'Bug Tracker': 'https://github.com/adaa-polsl/RuleKit-python/issues',
+        'Documentation': 'https://adaa-polsl.github.io/RuleKit-python/',
+        'Source Code': 'https://github.com/adaa-polsl/RuleKit-python'
+    }
+)
```

### Comparing `rulekit-1.6.0/tests/resources.py` & `rulekit-1.6.1/tests/resources.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-import requests
-import os
-import sys
-from typing import List
-
-dir_path = os.path.dirname(os.path.realpath(__file__))
-
-CONFIG_URL = 'https://api.github.com/repos/adaa-polsl/RuleKit/contents/adaa.analytics.rules/test/resources/config'
-DATA_URL = 'https://api.github.com/repos/adaa-polsl/RuleKit/contents/adaa.analytics.rules/test/resources/data'
-REPORTS_URL = 'https://api.github.com/repos/adaa-polsl/RuleKit/contents/adaa.analytics.rules/test/resources/reports'
-
-RESOURCES_DIRECTORY_PATH = f'{dir_path}/resources'
-CONFIG_DIRECTORY_PATH = RESOURCES_DIRECTORY_PATH + '/config'
-DATA_DIRECTORY_PATH = RESOURCES_DIRECTORY_PATH + '/data'
-REPORTS_DIRECTORY_PATH = RESOURCES_DIRECTORY_PATH + '/reports'
-
-
-def create_folders():
-    # create resources dir 
-    if not os.path.exists(RESOURCES_DIRECTORY_PATH):
-        os.mkdir(RESOURCES_DIRECTORY_PATH)
-    # create CONFIG dir
-    if not os.path.exists(CONFIG_DIRECTORY_PATH):
-        os.mkdir(CONFIG_DIRECTORY_PATH)
-    # create DATA dir
-    if not os.path.exists(DATA_DIRECTORY_PATH):
-        os.mkdir(DATA_DIRECTORY_PATH)   
-    # create REPORTS dir
-    if not os.path.exists(REPORTS_DIRECTORY_PATH):
-        os.mkdir(REPORTS_DIRECTORY_PATH)
-        
-
-def download_files(content: List, directory_path: str):
-    for item in content:
-        file_name = item['name']
-        download_url = item['download_url']
-        download_response = requests.get(download_url)
-        with open(directory_path +'/'+ file_name, 'wb') as file:
-            file.write(download_response.content)
-
-
-def download_resources():
-    #create dirs
-    create_folders()
-
-    # download config
-    config_content = requests.get(CONFIG_URL).json()
-    download_files(config_content, CONFIG_DIRECTORY_PATH)
-
-    # download data
-    data_content = requests.get(DATA_URL).json()
-    download_files(data_content, DATA_DIRECTORY_PATH)
-
-    # download reports
-    reports_content = requests.get(REPORTS_URL).json()
-    for item_folder in reports_content:
-        folder_name = item_folder['name']
-        folder_url = item_folder['url']
-        folder_directory = REPORTS_DIRECTORY_PATH + '/' + folder_name
-        if not os.path.exists(folder_directory) :
-            os.mkdir(folder_directory)
-        folder_content = requests.get(folder_url).json()
-        download_files(folder_content, folder_directory)
-
-
-if __name__ == '__main__':
-    if len(sys.argv) > 1 and sys.argv[1] == 'download':
-        download_resources()
-        print('Resources downloaded successfuly')
-    else:
+import requests
+import os
+import sys
+from typing import List
+
+dir_path = os.path.dirname(os.path.realpath(__file__))
+
+CONFIG_URL = 'https://api.github.com/repos/adaa-polsl/RuleKit/contents/adaa.analytics.rules/test/resources/config'
+DATA_URL = 'https://api.github.com/repos/adaa-polsl/RuleKit/contents/adaa.analytics.rules/test/resources/data'
+REPORTS_URL = 'https://api.github.com/repos/adaa-polsl/RuleKit/contents/adaa.analytics.rules/test/resources/reports'
+
+RESOURCES_DIRECTORY_PATH = f'{dir_path}/resources'
+CONFIG_DIRECTORY_PATH = RESOURCES_DIRECTORY_PATH + '/config'
+DATA_DIRECTORY_PATH = RESOURCES_DIRECTORY_PATH + '/data'
+REPORTS_DIRECTORY_PATH = RESOURCES_DIRECTORY_PATH + '/reports'
+
+
+def create_folders():
+    # create resources dir 
+    if not os.path.exists(RESOURCES_DIRECTORY_PATH):
+        os.mkdir(RESOURCES_DIRECTORY_PATH)
+    # create CONFIG dir
+    if not os.path.exists(CONFIG_DIRECTORY_PATH):
+        os.mkdir(CONFIG_DIRECTORY_PATH)
+    # create DATA dir
+    if not os.path.exists(DATA_DIRECTORY_PATH):
+        os.mkdir(DATA_DIRECTORY_PATH)   
+    # create REPORTS dir
+    if not os.path.exists(REPORTS_DIRECTORY_PATH):
+        os.mkdir(REPORTS_DIRECTORY_PATH)
+        
+
+def download_files(content: List, directory_path: str):
+    for item in content:
+        file_name = item['name']
+        download_url = item['download_url']
+        download_response = requests.get(download_url)
+        with open(directory_path +'/'+ file_name, 'wb') as file:
+            file.write(download_response.content)
+
+
+def download_resources():
+    #create dirs
+    create_folders()
+
+    # download config
+    config_content = requests.get(CONFIG_URL).json()
+    download_files(config_content, CONFIG_DIRECTORY_PATH)
+
+    # download data
+    data_content = requests.get(DATA_URL).json()
+    download_files(data_content, DATA_DIRECTORY_PATH)
+
+    # download reports
+    reports_content = requests.get(REPORTS_URL).json()
+    for item_folder in reports_content:
+        folder_name = item_folder['name']
+        folder_url = item_folder['url']
+        folder_directory = REPORTS_DIRECTORY_PATH + '/' + folder_name
+        if not os.path.exists(folder_directory) :
+            os.mkdir(folder_directory)
+        folder_content = requests.get(folder_url).json()
+        download_files(folder_content, folder_directory)
+
+
+if __name__ == '__main__':
+    if len(sys.argv) > 1 and sys.argv[1] == 'download':
+        download_resources()
+        print('Resources downloaded successfuly')
+    else:
         print('Please add paremeter: python resources.py download')
```

### Comparing `rulekit-1.6.0/tests/test_classifier.py` & `rulekit-1.6.1/tests/test_classifier.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-import unittest
-
-from rulekit.main import RuleKit
-from rulekit import classification
-import sklearn.tree as scikit
-from sklearn.datasets import load_iris
-from sklearn import metrics
-import numpy as np
-
-from tests.utils import get_test_cases, assert_rules_are_equals, assert_accuracy_is_greater
-
-
-class TestClassifier(unittest.TestCase):
-
-    @classmethod
-    def setUpClass(cls):
-        RuleKit.init()
-
-    def test_classification_accuracy_on_iris(self):
-        scikit_clf = scikit.DecisionTreeClassifier()
-        rulekit_clf = classification.RuleClassifier()
-        x, y = load_iris(return_X_y=True)
-
-        scikit_clf.fit(x, y)
-        rulekit_clf.fit(x, y)
-        scikit_prediction = scikit_clf.predict(x)
-        rulekit_prediction = rulekit_clf.predict(x)
-        scikit_accuracy = metrics.accuracy_score(y, scikit_prediction)
-        rulekit_accuracy = metrics.accuracy_score(y, rulekit_prediction)
-
-        assert abs(scikit_accuracy -
-                   rulekit_accuracy) < 0.03, 'RuleKit model should perform similar to scikit model'
-
-    def test_getting_examples_coverage(self):
-        clf = classification.RuleClassifier()
-        x, y = load_iris(return_X_y=True)
-
-        clf.fit(x, y)
-
-        coverage_matrix = clf.get_coverage_matrix(x)
-        num_rows, num_cols = coverage_matrix.shape
-
-        self.assertEqual(num_rows, len(
-            x), 'Coverage matrix should have as many rows as examples in dataset')
-        self.assertEqual(num_cols, len(
-            clf.model.rules), 'Coverage matrix should have as many cols as rules in ruleset')
-
-    def test_classification_metrics(self):
-        clf = classification.RuleClassifier()
-        x, y = load_iris(return_X_y=True)
-
-        clf.fit(x, y)
-        rulekit_prediction, m = clf.predict(x, return_metrics=True)
-        self.assertIsNotNone(m['rules_per_example'],
-                             'rules_per_example should be calculated')
-        self.assertIsNotNone(m['voting_conflicts'],
-                             'rules_per_example should be calculated')
-        self.assertIsNotNone(m['negative_voting_conflicts'],
-                             'rules_per_example should be calculated')
-
-    def test_classification_predict_proba(self):
-        clf = classification.RuleClassifier()
-        x, y = load_iris(return_X_y=True)
-
-        clf.fit(x, y)
-        confidence_matrix, m = clf.predict_proba(x, return_metrics=True)
-        for row in confidence_matrix:
-            sum = 0
-            for col in row:
-                sum += col
-            self.assertAlmostEqual(
-                sum, 1, 3, 'Confidence matrix rows should sum to 1')
-
-    def test_prediction_results_mapping(self):
-        """
-        This method tests classifications on numeric labels which possible values does 
-        not start from 0. RuleKit undehood maps all labels values to integer values starting 
-        from 0 to N (counting by order of appearance in dataset). Those maped values must be 
-        later remaped back to actual label value. This test verifies that predict method returns
-        correct (remaped) label value. 
-        """
-        clf = classification.RuleClassifier()
-
-        # some trivial dataset - OR (2 = false, 3 = true)
-        x = np.array([[0, 1], [1, 1], [1, 0], [0, 0]])
-        y = np.array([3., 3., 3., 2.])
-        clf.fit(x, y)
-        prediction = clf.predict(x)
-
-        self.assertEqual(y.all(), prediction.all())
-
-    def test_prediction_on_nominal_values(self):
-        clf = classification.RuleClassifier()
-
-        # some trivial dataset - OR (2 = false, 3 = true)
-        x = np.array([[0, 1], [1, 1], [1, 0], [0, 0]])
-        y = np.array(['false', 'false', 'false', 'true']).astype(np.unicode_)
-        clf.fit(x, y)
-        prediction = clf.predict(x).astype(np.unicode_)
-
-        self.assertTrue(np.array_equal(y, prediction))
-
-    def test_compare_with_java_results(self):
-        test_cases = get_test_cases('ClassificationSnCTest')
-
-        for test_case in test_cases:
-            params = test_case.induction_params
-            tree = classification.RuleClassifier(**params)
-            example_set = test_case.example_set
-            tree.fit(example_set.values, example_set.labels)
-            model = tree.model
-            expected = test_case.reference_report.rules
-            actual = list(map(lambda e: str(e), model.rules))
-            assert_rules_are_equals(expected, actual)
-            assert_accuracy_is_greater(tree.predict(
-                example_set.values), example_set.labels, 0.9)
-
-
-class TestExperClassifier(unittest.TestCase):
-
-    @classmethod
-    def setUpClass(cls):
-        RuleKit.init()
-
-    def test_compare_with_java_results(self):
-        test_cases = get_test_cases('ClassificationExpertSnCTest')
-
-        for test_case in test_cases:
-            params = test_case.induction_params
-            tree = classification.ExpertRuleClassifier(**params)
-            example_set = test_case.example_set
-            tree.fit(example_set.values,
-                     example_set.labels,
-                     expert_rules=test_case.knowledge.expert_rules,
-                     expert_preferred_conditions=test_case.knowledge.expert_preferred_conditions,
-                     expert_forbidden_conditions=test_case.knowledge.expert_forbidden_conditions)
-            model = tree.model
-            expected = test_case.reference_report.rules
-            actual = list(map(lambda e: str(e), model.rules))
-            assert_rules_are_equals(expected, actual)
-            assert_accuracy_is_greater(tree.predict(
-                example_set.values), example_set.labels, 0.9)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+
+from rulekit.main import RuleKit
+from rulekit import classification
+import sklearn.tree as scikit
+from sklearn.datasets import load_iris
+from sklearn import metrics
+import numpy as np
+
+from tests.utils import get_test_cases, assert_rules_are_equals, assert_accuracy_is_greater
+
+
+class TestClassifier(unittest.TestCase):
+
+    @classmethod
+    def setUpClass(cls):
+        RuleKit.init()
+
+    def test_classification_accuracy_on_iris(self):
+        scikit_clf = scikit.DecisionTreeClassifier()
+        rulekit_clf = classification.RuleClassifier()
+        x, y = load_iris(return_X_y=True)
+
+        scikit_clf.fit(x, y)
+        rulekit_clf.fit(x, y)
+        scikit_prediction = scikit_clf.predict(x)
+        rulekit_prediction = rulekit_clf.predict(x)
+        scikit_accuracy = metrics.accuracy_score(y, scikit_prediction)
+        rulekit_accuracy = metrics.accuracy_score(y, rulekit_prediction)
+
+        assert abs(scikit_accuracy -
+                   rulekit_accuracy) < 0.03, 'RuleKit model should perform similar to scikit model'
+
+    def test_getting_examples_coverage(self):
+        clf = classification.RuleClassifier()
+        x, y = load_iris(return_X_y=True)
+
+        clf.fit(x, y)
+
+        coverage_matrix = clf.get_coverage_matrix(x)
+        num_rows, num_cols = coverage_matrix.shape
+
+        self.assertEqual(num_rows, len(
+            x), 'Coverage matrix should have as many rows as examples in dataset')
+        self.assertEqual(num_cols, len(
+            clf.model.rules), 'Coverage matrix should have as many cols as rules in ruleset')
+
+    def test_classification_metrics(self):
+        clf = classification.RuleClassifier()
+        x, y = load_iris(return_X_y=True)
+
+        clf.fit(x, y)
+        rulekit_prediction, m = clf.predict(x, return_metrics=True)
+        self.assertIsNotNone(m['rules_per_example'],
+                             'rules_per_example should be calculated')
+        self.assertIsNotNone(m['voting_conflicts'],
+                             'rules_per_example should be calculated')
+        self.assertIsNotNone(m['negative_voting_conflicts'],
+                             'rules_per_example should be calculated')
+
+    def test_classification_predict_proba(self):
+        clf = classification.RuleClassifier()
+        x, y = load_iris(return_X_y=True)
+
+        clf.fit(x, y)
+        confidence_matrix, m = clf.predict_proba(x, return_metrics=True)
+        for row in confidence_matrix:
+            sum = 0
+            for col in row:
+                sum += col
+            self.assertAlmostEqual(
+                sum, 1, 3, 'Confidence matrix rows should sum to 1')
+
+    def test_prediction_results_mapping(self):
+        """
+        This method tests classifications on numeric labels which possible values does 
+        not start from 0. RuleKit undehood maps all labels values to integer values starting 
+        from 0 to N (counting by order of appearance in dataset). Those maped values must be 
+        later remaped back to actual label value. This test verifies that predict method returns
+        correct (remaped) label value. 
+        """
+        clf = classification.RuleClassifier()
+
+        # some trivial dataset - OR (2 = false, 3 = true)
+        x = np.array([[0, 1], [1, 1], [1, 0], [0, 0]])
+        y = np.array([3., 3., 3., 2.])
+        clf.fit(x, y)
+        prediction = clf.predict(x)
+
+        self.assertEqual(y.all(), prediction.all())
+
+    def test_prediction_on_nominal_values(self):
+        clf = classification.RuleClassifier()
+
+        # some trivial dataset - OR (2 = false, 3 = true)
+        x = np.array([[0, 1], [1, 1], [1, 0], [0, 0]])
+        y = np.array(['false', 'false', 'false', 'true']).astype(np.unicode_)
+        clf.fit(x, y)
+        prediction = clf.predict(x).astype(np.unicode_)
+
+        self.assertTrue(np.array_equal(y, prediction))
+
+    def test_compare_with_java_results(self):
+        test_cases = get_test_cases('ClassificationSnCTest')
+
+        for test_case in test_cases:
+            params = test_case.induction_params
+            tree = classification.RuleClassifier(**params)
+            example_set = test_case.example_set
+            tree.fit(example_set.values, example_set.labels)
+            model = tree.model
+            expected = test_case.reference_report.rules
+            actual = list(map(lambda e: str(e), model.rules))
+            assert_rules_are_equals(expected, actual)
+            assert_accuracy_is_greater(tree.predict(
+                example_set.values), example_set.labels, 0.9)
+
+
+class TestExperClassifier(unittest.TestCase):
+
+    @classmethod
+    def setUpClass(cls):
+        RuleKit.init()
+
+    def test_compare_with_java_results(self):
+        test_cases = get_test_cases('ClassificationExpertSnCTest')
+
+        for test_case in test_cases:
+            params = test_case.induction_params
+            tree = classification.ExpertRuleClassifier(**params)
+            example_set = test_case.example_set
+            tree.fit(example_set.values,
+                     example_set.labels,
+                     expert_rules=test_case.knowledge.expert_rules,
+                     expert_preferred_conditions=test_case.knowledge.expert_preferred_conditions,
+                     expert_forbidden_conditions=test_case.knowledge.expert_forbidden_conditions)
+            model = tree.model
+            expected = test_case.reference_report.rules
+            actual = list(map(lambda e: str(e), model.rules))
+            assert_rules_are_equals(expected, actual)
+            assert_accuracy_is_greater(tree.predict(
+                example_set.values), example_set.labels, 0.9)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `rulekit-1.6.0/tests/test_regression.py` & `rulekit-1.6.1/tests/test_regression.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-import unittest
-
-from rulekit.main import RuleKit
-from rulekit import regression
-
-from tests.utils import get_test_cases, assert_rules_are_equals, assert_score_is_greater
-
-
-class TestRegressor(unittest.TestCase):
-
-    @classmethod
-    def setUpClass(cls):
-        RuleKit.init()
-
-    def test_compare_with_java_results(self):
-        test_cases = get_test_cases('RegressionSnCTest')
-
-        for test_case in test_cases:
-            params = test_case.induction_params
-            tree = regression.RuleRegressor(**params)
-            example_set = test_case.example_set
-            tree.fit(example_set.values, example_set.labels)
-            model = tree.model
-            expected = test_case.reference_report.rules
-            actual = list(map(lambda e: str(e), model.rules))
-            assert_rules_are_equals(expected, actual)
-            assert_score_is_greater(tree.predict(example_set.values), example_set.labels, 0.7)
-
-
-class TestExpertRegressor(unittest.TestCase):
-
-    @classmethod
-    def setUpClass(cls):
-        RuleKit.init()
-
-    def test_compare_with_java_results(self):
-        test_cases = get_test_cases('RegressionExpertSnCTest')
-
-        for test_case in test_cases:
-            params = test_case.induction_params
-            tree = regression.ExpertRuleRegressor(**params)
-            example_set = test_case.example_set
-            tree.fit(example_set.values,
-                     example_set.labels,
-                     expert_rules=test_case.knowledge.expert_rules,
-                     expert_preferred_conditions=test_case.knowledge.expert_preferred_conditions,
-                     expert_forbidden_conditions=test_case.knowledge.expert_forbidden_conditions)
-            model = tree.model
-            expected = test_case.reference_report.rules
-            actual = list(map(lambda e: str(e), model.rules))
-            assert_rules_are_equals(expected, actual)
-            assert_score_is_greater(tree.predict(example_set.values), example_set.labels, 0.66)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+
+from rulekit.main import RuleKit
+from rulekit import regression
+
+from tests.utils import get_test_cases, assert_rules_are_equals, assert_score_is_greater
+
+
+class TestRegressor(unittest.TestCase):
+
+    @classmethod
+    def setUpClass(cls):
+        RuleKit.init()
+
+    def test_compare_with_java_results(self):
+        test_cases = get_test_cases('RegressionSnCTest')
+
+        for test_case in test_cases:
+            params = test_case.induction_params
+            tree = regression.RuleRegressor(**params)
+            example_set = test_case.example_set
+            tree.fit(example_set.values, example_set.labels)
+            model = tree.model
+            expected = test_case.reference_report.rules
+            actual = list(map(lambda e: str(e), model.rules))
+            assert_rules_are_equals(expected, actual)
+            assert_score_is_greater(tree.predict(example_set.values), example_set.labels, 0.7)
+
+
+class TestExpertRegressor(unittest.TestCase):
+
+    @classmethod
+    def setUpClass(cls):
+        RuleKit.init()
+
+    def test_compare_with_java_results(self):
+        test_cases = get_test_cases('RegressionExpertSnCTest')
+
+        for test_case in test_cases:
+            params = test_case.induction_params
+            tree = regression.ExpertRuleRegressor(**params)
+            example_set = test_case.example_set
+            tree.fit(example_set.values,
+                     example_set.labels,
+                     expert_rules=test_case.knowledge.expert_rules,
+                     expert_preferred_conditions=test_case.knowledge.expert_preferred_conditions,
+                     expert_forbidden_conditions=test_case.knowledge.expert_forbidden_conditions)
+            model = tree.model
+            expected = test_case.reference_report.rules
+            actual = list(map(lambda e: str(e), model.rules))
+            assert_rules_are_equals(expected, actual)
+            assert_score_is_greater(tree.predict(example_set.values), example_set.labels, 0.66)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `rulekit-1.6.0/tests/test_rulekit.py` & `rulekit-1.6.1/tests/test_rulekit.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import unittest
-
-from jpype import JClass
-from rulekit.main import RuleKit
-
-
-class TestRuleKitMainClass(unittest.TestCase):
-
-    @classmethod
-    def setUpClass(cls):
-        RuleKit.init()
-
-    def test_reading_version(self):
-        self.assertIsNotNone(RuleKit.version, 'Version should not be None')
-        self.assertEqual(len(RuleKit.version.split('.')), 3, 'Version should have correct format')
-
-    def test_loading_rapidminer_class(self):
-        example_rapidminer_class = JClass('com.rapidminer.example.ExampleSetFactory')
-        self.assertIsNotNone(example_rapidminer_class, 'Should load RapidMiner classes')
-
-    def test_loading_rulekit_class(self):
-        example_rulekit_class = JClass('adaa.analytics.rules.operator.RuleGenerator')
-        self.assertIsNotNone(example_rulekit_class, 'Should load RuleKit classes')
-
-
-if __name__ == '__main__':
+import unittest
+
+from jpype import JClass
+from rulekit.main import RuleKit
+
+
+class TestRuleKitMainClass(unittest.TestCase):
+
+    @classmethod
+    def setUpClass(cls):
+        RuleKit.init()
+
+    def test_reading_version(self):
+        self.assertIsNotNone(RuleKit.version, 'Version should not be None')
+        self.assertEqual(len(RuleKit.version.split('.')), 3, 'Version should have correct format')
+
+    def test_loading_rapidminer_class(self):
+        example_rapidminer_class = JClass('com.rapidminer.example.ExampleSetFactory')
+        self.assertIsNotNone(example_rapidminer_class, 'Should load RapidMiner classes')
+
+    def test_loading_rulekit_class(self):
+        example_rulekit_class = JClass('adaa.analytics.rules.operator.RuleGenerator')
+        self.assertIsNotNone(example_rulekit_class, 'Should load RuleKit classes')
+
+
+if __name__ == '__main__':
     unittest.main()
```

### Comparing `rulekit-1.6.0/tests/test_serialization.py` & `rulekit-1.6.1/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.0/tests/test_sklearn_metrics.py` & `rulekit-1.6.1/tests/test_sklearn_metrics.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-import unittest
-
-from rulekit.main import RuleKit
-from rulekit import classification
-import sklearn.tree as scikit
-from sklearn.datasets import load_iris
-from sklearn import metrics
-
-
-class TestMetrics(unittest.TestCase):
-
-    @classmethod
-    def setUpClass(cls):
-        RuleKit.init()
-
-    def test_classification_accuracy_on_iris(self):
-        scikit_clf = scikit.DecisionTreeClassifier()
-        rulekit_clf = classification.RuleClassifier()
-        x, y = load_iris(return_X_y=True)
-
-        scikit_clf.fit(x, y)
-        rulekit_clf.fit(x, y)
-        scikit_prediction = scikit_clf.predict(x)
-        rulekit_prediction = rulekit_clf.predict(x)
-
-        scikit_accuracy = metrics.accuracy_score(y, scikit_prediction)
-        rulekit_accuracy = metrics.accuracy_score(y, rulekit_prediction)
-
-        assert abs(scikit_accuracy - rulekit_accuracy) < 0.03, 'RuleKit model should perform similar to scikit model'
-        confusion_matrix = metrics.confusion_matrix(y, rulekit_prediction)
-        self.assertIsNotNone(confusion_matrix, 'Confusion matrix should be calculated')
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+
+from rulekit.main import RuleKit
+from rulekit import classification
+import sklearn.tree as scikit
+from sklearn.datasets import load_iris
+from sklearn import metrics
+
+
+class TestMetrics(unittest.TestCase):
+
+    @classmethod
+    def setUpClass(cls):
+        RuleKit.init()
+
+    def test_classification_accuracy_on_iris(self):
+        scikit_clf = scikit.DecisionTreeClassifier()
+        rulekit_clf = classification.RuleClassifier()
+        x, y = load_iris(return_X_y=True)
+
+        scikit_clf.fit(x, y)
+        rulekit_clf.fit(x, y)
+        scikit_prediction = scikit_clf.predict(x)
+        rulekit_prediction = rulekit_clf.predict(x)
+
+        scikit_accuracy = metrics.accuracy_score(y, scikit_prediction)
+        rulekit_accuracy = metrics.accuracy_score(y, rulekit_prediction)
+
+        assert abs(scikit_accuracy - rulekit_accuracy) < 0.03, 'RuleKit model should perform similar to scikit model'
+        confusion_matrix = metrics.confusion_matrix(y, rulekit_prediction)
+        self.assertIsNotNone(confusion_matrix, 'Confusion matrix should be calculated')
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `rulekit-1.6.0/tests/test_statistics.py` & `rulekit-1.6.1/tests/test_statistics.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import unittest
-
-from rulekit.main import RuleKit
-from rulekit import classification
-from rulekit.rules import RuleSetStatistics
-from sklearn.datasets import load_iris
-
-
-class TestDecisionTreeClassifier(unittest.TestCase):
-
-    @classmethod
-    def setUpClass(cls):
-        RuleKit.init()
-
-    def test_classification_accuracy_on_iris(self):
-        clf = classification.RuleClassifier()
-        x, y = load_iris(return_X_y=True)
-
-        clf.fit(x, y)
-
-        ruleset_stats: RuleSetStatistics = clf.model.stats
-        for rule in clf.model.rules:
-            rule.stats
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+
+from rulekit.main import RuleKit
+from rulekit import classification
+from rulekit.rules import RuleSetStatistics
+from sklearn.datasets import load_iris
+
+
+class TestDecisionTreeClassifier(unittest.TestCase):
+
+    @classmethod
+    def setUpClass(cls):
+        RuleKit.init()
+
+    def test_classification_accuracy_on_iris(self):
+        clf = classification.RuleClassifier()
+        x, y = load_iris(return_X_y=True)
+
+        clf.fit(x, y)
+
+        ruleset_stats: RuleSetStatistics = clf.model.stats
+        for rule in clf.model.rules:
+            rule.stats
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `rulekit-1.6.0/tests/test_survival.py` & `rulekit-1.6.1/tests/test_survival.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-import unittest
-
-from rulekit.main import RuleKit
-from rulekit import survival
-
-from tests.utils import get_test_cases, assert_rules_are_equals
-
-
-class TestSurvivalLogRankTree(unittest.TestCase):
-
-    @classmethod
-    def setUpClass(cls):
-        RuleKit.init()
-
-    def test_compare_with_java_results(self):
-        test_cases = get_test_cases('SurvivalLogRankSnCTest')
-
-        for test_case in test_cases:
-            params = test_case.induction_params
-            tree = survival.SurvivalRules(**params, survival_time_attr=test_case.survival_time)
-            example_set = test_case.example_set
-            tree.fit(example_set.values, example_set.labels)
-            model = tree.model
-            expected = test_case.reference_report.rules
-            actual = list(map(lambda e: str(e), model.rules))
-            assert_rules_are_equals(expected, actual)
-
-
-class TestExpertSurvivalLogRankTree(unittest.TestCase):
-
-    @classmethod
-    def setUpClass(cls):
-        RuleKit.init()
-
-    def test_compare_with_java_results(self):
-        test_cases = get_test_cases('SurvivalLogRankExpertSnCTest')
-
-        for test_case in test_cases:
-            params = test_case.induction_params
-            tree = survival.ExpertSurvivalRules(**params, ignore_missing=True, survival_time_attr=test_case.survival_time)
-            example_set = test_case.example_set
-            tree.fit(example_set.values,
-                     example_set.labels,
-                     expert_rules=test_case.knowledge.expert_rules,
-                     expert_preferred_conditions=test_case.knowledge.expert_preferred_conditions,
-                     expert_forbidden_conditions=test_case.knowledge.expert_forbidden_conditions)
-            model = tree.model
-            expected = test_case.reference_report.rules
-            actual = list(map(lambda e: str(e), model.rules))
-            assert_rules_are_equals(expected, actual)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+
+from rulekit.main import RuleKit
+from rulekit import survival
+
+from tests.utils import get_test_cases, assert_rules_are_equals
+
+
+class TestSurvivalLogRankTree(unittest.TestCase):
+
+    @classmethod
+    def setUpClass(cls):
+        RuleKit.init()
+
+    def test_compare_with_java_results(self):
+        test_cases = get_test_cases('SurvivalLogRankSnCTest')
+
+        for test_case in test_cases:
+            params = test_case.induction_params
+            tree = survival.SurvivalRules(**params, survival_time_attr=test_case.survival_time)
+            example_set = test_case.example_set
+            tree.fit(example_set.values, example_set.labels)
+            model = tree.model
+            expected = test_case.reference_report.rules
+            actual = list(map(lambda e: str(e), model.rules))
+            assert_rules_are_equals(expected, actual)
+
+
+class TestExpertSurvivalLogRankTree(unittest.TestCase):
+
+    @classmethod
+    def setUpClass(cls):
+        RuleKit.init()
+
+    def test_compare_with_java_results(self):
+        test_cases = get_test_cases('SurvivalLogRankExpertSnCTest')
+
+        for test_case in test_cases:
+            params = test_case.induction_params
+            tree = survival.ExpertSurvivalRules(**params, ignore_missing=True, survival_time_attr=test_case.survival_time)
+            example_set = test_case.example_set
+            tree.fit(example_set.values,
+                     example_set.labels,
+                     expert_rules=test_case.knowledge.expert_rules,
+                     expert_preferred_conditions=test_case.knowledge.expert_preferred_conditions,
+                     expert_forbidden_conditions=test_case.knowledge.expert_forbidden_conditions)
+            model = tree.model
+            expected = test_case.reference_report.rules
+            actual = list(map(lambda e: str(e), model.rules))
+            assert_rules_are_equals(expected, actual)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `rulekit-1.6.0/tests/utils.py` & `rulekit-1.6.1/tests/utils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,402 +1,402 @@
-from xml.etree import ElementTree
-import pandas as pd
-from scipy.io.arff import loadarff
-from sklearn import metrics
-from jpype import JClass
-from typing import List, Dict, Tuple, Union
-import os
-import re
-
-from rulekit.helpers import create_example_set, _fix_missing_values
-from rulekit.rules import Rule
-
-import os
-
-dir_path = os.path.dirname(os.path.realpath(__file__))
-
-TEST_CONFIG_PATH = f'{dir_path}/resources/config'
-REPORTS_IN_DIRECTORY_PATH = f'{dir_path}/resources/reports'
-DATA_IN_DIRECTORY_PATH = f'{dir_path}/resources/'
-REPORTS_OUT_DIRECTORY_PATH = f'{dir_path}/test_out'
-
-REPORTS_SECTIONS_HEADERS = {
-    'RULES': 'RULES'
-}
-
-DATASETS_PATH = '/resources/data'
-EXPERIMENTS_PATH = '/resources/config'
-
-
-class ExampleSetWrapper:
-
-    def __init__(self, values, labels):
-        self.values = values
-        self.labels = labels
-        self.example_set = create_example_set(values, labels)
-
-    def get_data(self) -> Tuple:
-        return self.values, self.labels
-
-
-def load_arff_to_example_set(path: str, label_attribute: str) -> ExampleSetWrapper:
-    arff_data_frame = pd.DataFrame(loadarff(path)[0])
-
-    attributes_names = []
-    for column_name in arff_data_frame.columns:
-        if column_name != label_attribute:
-            attributes_names.append(column_name)
-
-    values = arff_data_frame[attributes_names]
-    labels = arff_data_frame[label_attribute]
-
-    for column in values:
-        _fix_missing_values(values[column])
-    _fix_missing_values(labels)
-    return ExampleSetWrapper(values, labels)
-
-
-def get_dataset_path(name: str) -> str:
-    return f'{DATASETS_PATH}/{name}'
-
-
-class Knowledge:
-
-    def __init__(self):
-        self.expert_rules = []
-        self.expert_preferred_conditions = []
-        self.expert_forbidden_conditions = []
-
-
-class TestReport:
-
-    def __init__(self, file_name: str):
-        self.file_name = file_name
-        self.rules = None
-
-
-class TestCase:
-
-    def __init__(self):
-        self.param_config: Dict[str, object] = None
-        self._reference_report: TestReport = None
-        self._example_set: ExampleSetWrapper = None
-        self.induction_params: Dict = None
-        self.knowledge: Knowledge = None
-
-        self.name: str = None
-        self.data_set_file_path: str = None
-        self.label_attribute: str = None
-        self.survival_time: str = None
-        self.report_file_path: str = None
-        self.using_existing_report_file: bool = False
-
-    @property
-    def example_set(self) -> ExampleSetWrapper:
-        if self._example_set is None:
-            self._example_set = load_arff_to_example_set(self.data_set_file_path, self.label_attribute)
-        return self._example_set
-
-    @property
-    def reference_report(self) -> TestReport:
-        if self._reference_report is None:
-            ExampleSetMetaData = JClass('com.rapidminer.operator.ports.metadata.ExampleSetMetaData')
-            reader = TestReportReader(f'{self.report_file_path}.txt', ExampleSetMetaData(self._example_set.example_set))
-            self._reference_report = reader.read()
-            reader.close()
-        return self._reference_report
-
-
-class DataSetConfig:
-
-    def __init__(self):
-        self.name: str = None
-        self.label_attribute: str = None
-        self.train_file_name: str = None
-        self.survival_time: str = None
-
-
-class TestConfig:
-
-    def __init__(self):
-        self.name: str = None
-        self.parameter_configs: Dict[str, Dict[str, object]] = None
-        self.datasets: List[DataSetConfig] = None
-
-
-class TestConfigParser:
-    TEST_KEY = 'test'
-    NAME_KEY = 'name'
-    IN_FILE_KEY = 'in_file'
-    TRAINING_KEY = 'training'
-    TRAIN_KEY = 'train'
-    LABEL_KEY = 'label'
-    DATASET_KEY = 'dataset'
-    DATASETS_KEY = 'datasets'
-    PARAM_KEY = 'param'
-    PARAMETERS_SET_KEY = 'parameter_sets'
-    PARAMETERS_KEY = 'parameter_set'
-    ENTRY_KEY = 'entry'
-    SURVIVAL_TIME_ROLE = 'survival_time'
-
-    EXPERTS_RULES_PARAMETERS_NAMES = [
-        'expert_rules',
-        'expert_preferred_conditions',
-        'expert_forbidden_conditions'
-    ]
-
-    def __init__(self):
-        self.tests_configs: Dict[str, TestConfig] = {}
-        self.root: ElementTree = None
-
-    def _parse_survival_time(self, element) -> Union[str, None]:
-        survival_time_element = element.find(TestConfigParser.SURVIVAL_TIME_ROLE)
-        if element.find(TestConfigParser.SURVIVAL_TIME_ROLE) is not None:
-            return survival_time_element.text
-        else:
-            return None
-
-    def _parse_experts_rules_parameters(self, elements) -> List[Tuple]:
-        expert_rules = []
-        for element in elements:
-            rule_name = element.attrib['name']
-            rule_content = element.text
-            expert_rules.append((rule_name, rule_content))
-        return expert_rules if len(expert_rules) > 0 else None
-
-    def _check_ambigous_data_sets_names(self, data_sets_configs: List[DataSetConfig]):
-        dict = {}
-        for element in data_sets_configs:
-            dict[element.name] = None
-        if len(dict.keys()) < len(data_sets_configs):
-            raise ValueError('Datasets are ambigous')
-
-    def _parse_data_set(self, element) -> DataSetConfig:
-        data_set_config = DataSetConfig()
-        data_set_config.label_attribute = element.find(TestConfigParser.LABEL_KEY).text
-        train_element = element.find(TestConfigParser.TRAINING_KEY)
-        train_element = train_element.find(TestConfigParser.TRAIN_KEY)
-        data_set_config.train_file_name = train_element.find(TestConfigParser.IN_FILE_KEY).text
-        data_set_config.name = element.attrib.get('name', None)
-        if data_set_config.name is None:
-            file_name = os.path.basename(data_set_config.train_file_name)
-            data_set_config.name = file_name.split('.')[0]
-        data_set_config.survival_time = self._parse_survival_time(element)
-        return data_set_config
-
-    def _parse_data_sets(self, element) -> List[DataSetConfig]:
-        data_set_configs = []
-        node = element.find(TestConfigParser.DATASETS_KEY)
-        for element in node.findall(TestConfigParser.DATASET_KEY):
-            data_set_configs.append(self._parse_data_set(element))
-        return data_set_configs
-
-    def parse_test_parameters(self, element) -> Dict[str, object]:
-        params = {}
-        for param_node in element.findall(TestConfigParser.PARAM_KEY):
-            name: str = param_node.attrib['name']
-            if name in TestConfigParser.EXPERTS_RULES_PARAMETERS_NAMES:
-                value = self._parse_experts_rules_parameters(param_node.findall(TestConfigParser.ENTRY_KEY))
-            else:
-                value = param_node.text
-            params[name] = value
-        return params
-
-    def _parse_test_parameters_sets(self, element) -> Dict[str, Dict[str, object]]:
-        parameters_sets = {}
-        params_sets_node = element.findall(TestConfigParser.PARAMETERS_SET_KEY)[0]
-        for param_set in params_sets_node.findall(TestConfigParser.PARAMETERS_KEY):
-            name: str = param_set.attrib['name']
-            parameters_sets[name] = self.parse_test_parameters(param_set)
-        return parameters_sets
-
-    def _parse_test(self, element) -> TestConfig:
-        test_config = TestConfig()
-        test_config.parameter_configs = self._parse_test_parameters_sets(element)
-        test_config.datasets = self._parse_data_sets(element)
-        test_config.name = element.attrib['name']
-        return test_config
-
-    def parse(self, file_path: str) -> Dict[str, TestConfig]:
-        self.tests_configs = {}
-        self.root = ElementTree.parse(file_path).getroot()
-        if self.root.tag == 'test':
-            test_elements = [self.root]
-        else:
-            test_elements = self.root.findall(TestConfigParser.TEST_KEY)
-        for test_element in test_elements:
-            test_config = self._parse_test(test_element)
-            self.tests_configs[test_config.name] = test_config
-        return self.tests_configs
-
-
-class TestCaseFactory:
-
-    def _make_test_case(
-            self,
-            test_case_name: str,
-            params: Dict[str, object],
-            data_set_config: DataSetConfig) -> TestCase:
-        test_case = TestCase()
-        self.fix_params_typing(params)
-        test_case.induction_params = params
-        test_case.data_set_file_path = f'{DATA_IN_DIRECTORY_PATH}/{data_set_config.train_file_name}'
-        test_case.label_attribute = data_set_config.label_attribute
-        test_case.name = test_case_name
-        test_case.param_config = params
-        return test_case
-
-    def fix_params_typing(self, params: dict):
-        for key, value in params.items():
-            if value == 'false':
-                params[key] = False
-                continue
-            if value == 'true':
-                params[key] = True
-                continue
-            if not 'measure' in key:
-                params[key] = int(float(value))
-
-    def make(self, tests_configs: Dict[str, TestConfig], report_dir_path: str) -> List[TestCase]:
-        test_cases = []
-        for key in tests_configs.keys():
-            test_config = tests_configs[key]
-            for config_name in test_config.parameter_configs.keys():
-                for data_set_config in test_config.datasets:
-                    params = test_config.parameter_configs[config_name]
-                    test_case_name = f'{key}.{config_name}.{data_set_config.name}'
-                    test_config.parameter_configs[config_name].pop('use_expert', None)
-                    expert_rules = test_config.parameter_configs[config_name].pop('expert_rules', None)
-                    preferred_conditions = test_config.parameter_configs[config_name].pop('expert_preferred_conditions',
-                                                                                          None)
-                    forbidden_conditions = test_config.parameter_configs[config_name].pop('expert_forbidden_conditions',
-                                                                                          None)
-                    test_case = self._make_test_case(test_case_name,
-                                                     test_config.parameter_configs[config_name], data_set_config)
-                    if 'use_report' in params:
-                        report_file_name = params['use_report']
-                        test_case.using_existing_report_file = True
-                    else:
-                        report_file_name = test_case_name
-                    report_path = f'{report_dir_path}/{report_file_name}'
-                    test_case.report_file_path = report_path
-                    test_case.survival_time = data_set_config.survival_time
-                    if expert_rules is not None or preferred_conditions is not None or forbidden_conditions is not None:
-                        test_case.knowledge = Knowledge()
-                        test_case.knowledge.expert_rules = expert_rules
-                        test_case.knowledge.expert_forbidden_conditions = forbidden_conditions
-                        test_case.knowledge.expert_preferred_conditions = preferred_conditions
-                    test_cases.append(test_case)
-        return test_cases
-
-
-def get_rule_string(rule) -> str:
-    return re.sub(r'(\\[[^\\]]*\\]$)|(\\([^\\)]*\\)$)', '', str(rule))
-
-
-class TestReportReader:
-
-    def __init__(self, file_name: str, example_set_meta_data):
-        self.example_set_meta_data = example_set_meta_data
-        self.file_name = file_name
-        self._file = f = open(file_name, "r")
-
-    def _read_rules(self, test_report: TestReport):
-        rules = []
-        for line in self._file:
-            if len(line) == 0:
-                break
-            else:
-                rules.append(line)
-        test_report.rules = rules
-
-    def read(self) -> TestReport:
-        test_report = TestReport(self.file_name)
-        for line in self._file:
-            line = line.upper()
-            line = re.sub(r'\t', '', line)
-            line = line.replace('\n', '')
-            if line == REPORTS_SECTIONS_HEADERS['RULES']:
-                self._read_rules(test_report)
-            elif line == '':
-                continue
-            else:
-                raise ValueError(f'Invalid report file format for file: {self.file_name}')
-        return test_report
-
-    def close(self):
-        self._file.close()
-
-
-class TestReportWriter:
-
-    def __init__(self, file_name: str):
-        self._file = f = open(file_name, "w")
-        if not os.path.exists(REPORTS_OUT_DIRECTORY_PATH):
-            os.makedirs(REPORTS_OUT_DIRECTORY_PATH)
-
-    def write(self, rule_set):
-        self._file.write('\n')
-        self._file.write(f'{REPORTS_SECTIONS_HEADERS["RULES"]}\n')
-        for rule in rule_set.rules:
-            self._file.write(f'\t{get_rule_string(rule)}')
-
-    def close(self):
-        self._file.close()
-
-
-def get_test_cases(class_name: str) -> List[TestCase]:
-    if not os.path.exists(DATA_IN_DIRECTORY_PATH):
-        raise Exception('''\n
-Test resources directory dosen't exist. Check if 'tests/resources/' directory exist.
-
-If you're running tests for the first time you need to download resources folder from RuleKit repository by running:
-    python tests/resources.py download
-        ''')
-    configs = TestConfigParser().parse(f'{TEST_CONFIG_PATH}/{class_name}.xml')
-    return TestCaseFactory().make(configs, f'{REPORTS_IN_DIRECTORY_PATH}/{class_name}/')
-
-
-def _get_rule_string(rule: Rule) -> str:
-    return re.sub(r'(\\[[^\\]]*\\]$)|(\\([^\\)]*\\)$)', '', str(rule))
-
-
-def assert_rules_are_equals(expected: List[str], actual: List[str]):
-    def sanitize_rule_string(rule_string: str) -> str:
-        return re.sub(r'(\t)|(\n)|(\[[^\]]*\]$)', '', rule_string)
-
-    if len(expected) != len(actual):
-        raise AssertionError(
-            f'Rulesets have different number of rules, actual: {len(actual)}, expected: {len(expected)}')
-    dictionary = {}
-    for rule in expected:
-        dictionary[sanitize_rule_string(rule)] = 0
-    for rule in actual:
-        key = sanitize_rule_string(rule)
-        if key in dictionary:
-            dictionary[key] = dictionary[key] + 1
-        else:
-            pass
-            raise AssertionError('Actual ruleset contains rules not present in expected ruleset')
-    for key in dictionary.keys():
-        if dictionary[key] == 0:
-            raise AssertionError('Ruleset are not equal, some rules are missing')
-        elif dictionary[key] > 1:
-            raise AssertionError('Somes rules were duplicated')
-
-
-def assert_accuracy_is_greater(prediction, expected, threshold: float):
-    labels = expected.to_numpy().astype(str)
-    acc = metrics.accuracy_score(labels, prediction)
-    if acc <= threshold:
-        raise AssertionError(f'Accuracy should be greater than {threshold}')
-
-
-def assert_score_is_greater(prediction, expected, threshold: float):
-    if isinstance(prediction[0], int):
-        labels = expected.to_numpy().astype(int)
-    if isinstance(prediction[0], float):
-        labels = expected.to_numpy().astype(float)
-    explained_variance_score = metrics.explained_variance_score(labels, prediction)
-
-    if explained_variance_score <= threshold:
-        raise AssertionError(f'Score should be greater than {threshold}')
+from xml.etree import ElementTree
+import pandas as pd
+from scipy.io.arff import loadarff
+from sklearn import metrics
+from jpype import JClass
+from typing import List, Dict, Tuple, Union
+import os
+import re
+
+from rulekit.helpers import create_example_set, _fix_missing_values
+from rulekit.rules import Rule
+
+import os
+
+dir_path = os.path.dirname(os.path.realpath(__file__))
+
+TEST_CONFIG_PATH = f'{dir_path}/resources/config'
+REPORTS_IN_DIRECTORY_PATH = f'{dir_path}/resources/reports'
+DATA_IN_DIRECTORY_PATH = f'{dir_path}/resources/'
+REPORTS_OUT_DIRECTORY_PATH = f'{dir_path}/test_out'
+
+REPORTS_SECTIONS_HEADERS = {
+    'RULES': 'RULES'
+}
+
+DATASETS_PATH = '/resources/data'
+EXPERIMENTS_PATH = '/resources/config'
+
+
+class ExampleSetWrapper:
+
+    def __init__(self, values, labels):
+        self.values = values
+        self.labels = labels
+        self.example_set = create_example_set(values, labels)
+
+    def get_data(self) -> Tuple:
+        return self.values, self.labels
+
+
+def load_arff_to_example_set(path: str, label_attribute: str) -> ExampleSetWrapper:
+    arff_data_frame = pd.DataFrame(loadarff(path)[0])
+
+    attributes_names = []
+    for column_name in arff_data_frame.columns:
+        if column_name != label_attribute:
+            attributes_names.append(column_name)
+
+    values = arff_data_frame[attributes_names]
+    labels = arff_data_frame[label_attribute]
+
+    for column in values:
+        _fix_missing_values(values[column])
+    _fix_missing_values(labels)
+    return ExampleSetWrapper(values, labels)
+
+
+def get_dataset_path(name: str) -> str:
+    return f'{DATASETS_PATH}/{name}'
+
+
+class Knowledge:
+
+    def __init__(self):
+        self.expert_rules = []
+        self.expert_preferred_conditions = []
+        self.expert_forbidden_conditions = []
+
+
+class TestReport:
+
+    def __init__(self, file_name: str):
+        self.file_name = file_name
+        self.rules = None
+
+
+class TestCase:
+
+    def __init__(self):
+        self.param_config: Dict[str, object] = None
+        self._reference_report: TestReport = None
+        self._example_set: ExampleSetWrapper = None
+        self.induction_params: Dict = None
+        self.knowledge: Knowledge = None
+
+        self.name: str = None
+        self.data_set_file_path: str = None
+        self.label_attribute: str = None
+        self.survival_time: str = None
+        self.report_file_path: str = None
+        self.using_existing_report_file: bool = False
+
+    @property
+    def example_set(self) -> ExampleSetWrapper:
+        if self._example_set is None:
+            self._example_set = load_arff_to_example_set(self.data_set_file_path, self.label_attribute)
+        return self._example_set
+
+    @property
+    def reference_report(self) -> TestReport:
+        if self._reference_report is None:
+            ExampleSetMetaData = JClass('com.rapidminer.operator.ports.metadata.ExampleSetMetaData')
+            reader = TestReportReader(f'{self.report_file_path}.txt', ExampleSetMetaData(self._example_set.example_set))
+            self._reference_report = reader.read()
+            reader.close()
+        return self._reference_report
+
+
+class DataSetConfig:
+
+    def __init__(self):
+        self.name: str = None
+        self.label_attribute: str = None
+        self.train_file_name: str = None
+        self.survival_time: str = None
+
+
+class TestConfig:
+
+    def __init__(self):
+        self.name: str = None
+        self.parameter_configs: Dict[str, Dict[str, object]] = None
+        self.datasets: List[DataSetConfig] = None
+
+
+class TestConfigParser:
+    TEST_KEY = 'test'
+    NAME_KEY = 'name'
+    IN_FILE_KEY = 'in_file'
+    TRAINING_KEY = 'training'
+    TRAIN_KEY = 'train'
+    LABEL_KEY = 'label'
+    DATASET_KEY = 'dataset'
+    DATASETS_KEY = 'datasets'
+    PARAM_KEY = 'param'
+    PARAMETERS_SET_KEY = 'parameter_sets'
+    PARAMETERS_KEY = 'parameter_set'
+    ENTRY_KEY = 'entry'
+    SURVIVAL_TIME_ROLE = 'survival_time'
+
+    EXPERTS_RULES_PARAMETERS_NAMES = [
+        'expert_rules',
+        'expert_preferred_conditions',
+        'expert_forbidden_conditions'
+    ]
+
+    def __init__(self):
+        self.tests_configs: Dict[str, TestConfig] = {}
+        self.root: ElementTree = None
+
+    def _parse_survival_time(self, element) -> Union[str, None]:
+        survival_time_element = element.find(TestConfigParser.SURVIVAL_TIME_ROLE)
+        if element.find(TestConfigParser.SURVIVAL_TIME_ROLE) is not None:
+            return survival_time_element.text
+        else:
+            return None
+
+    def _parse_experts_rules_parameters(self, elements) -> List[Tuple]:
+        expert_rules = []
+        for element in elements:
+            rule_name = element.attrib['name']
+            rule_content = element.text
+            expert_rules.append((rule_name, rule_content))
+        return expert_rules if len(expert_rules) > 0 else None
+
+    def _check_ambigous_data_sets_names(self, data_sets_configs: List[DataSetConfig]):
+        dict = {}
+        for element in data_sets_configs:
+            dict[element.name] = None
+        if len(dict.keys()) < len(data_sets_configs):
+            raise ValueError('Datasets are ambigous')
+
+    def _parse_data_set(self, element) -> DataSetConfig:
+        data_set_config = DataSetConfig()
+        data_set_config.label_attribute = element.find(TestConfigParser.LABEL_KEY).text
+        train_element = element.find(TestConfigParser.TRAINING_KEY)
+        train_element = train_element.find(TestConfigParser.TRAIN_KEY)
+        data_set_config.train_file_name = train_element.find(TestConfigParser.IN_FILE_KEY).text
+        data_set_config.name = element.attrib.get('name', None)
+        if data_set_config.name is None:
+            file_name = os.path.basename(data_set_config.train_file_name)
+            data_set_config.name = file_name.split('.')[0]
+        data_set_config.survival_time = self._parse_survival_time(element)
+        return data_set_config
+
+    def _parse_data_sets(self, element) -> List[DataSetConfig]:
+        data_set_configs = []
+        node = element.find(TestConfigParser.DATASETS_KEY)
+        for element in node.findall(TestConfigParser.DATASET_KEY):
+            data_set_configs.append(self._parse_data_set(element))
+        return data_set_configs
+
+    def parse_test_parameters(self, element) -> Dict[str, object]:
+        params = {}
+        for param_node in element.findall(TestConfigParser.PARAM_KEY):
+            name: str = param_node.attrib['name']
+            if name in TestConfigParser.EXPERTS_RULES_PARAMETERS_NAMES:
+                value = self._parse_experts_rules_parameters(param_node.findall(TestConfigParser.ENTRY_KEY))
+            else:
+                value = param_node.text
+            params[name] = value
+        return params
+
+    def _parse_test_parameters_sets(self, element) -> Dict[str, Dict[str, object]]:
+        parameters_sets = {}
+        params_sets_node = element.findall(TestConfigParser.PARAMETERS_SET_KEY)[0]
+        for param_set in params_sets_node.findall(TestConfigParser.PARAMETERS_KEY):
+            name: str = param_set.attrib['name']
+            parameters_sets[name] = self.parse_test_parameters(param_set)
+        return parameters_sets
+
+    def _parse_test(self, element) -> TestConfig:
+        test_config = TestConfig()
+        test_config.parameter_configs = self._parse_test_parameters_sets(element)
+        test_config.datasets = self._parse_data_sets(element)
+        test_config.name = element.attrib['name']
+        return test_config
+
+    def parse(self, file_path: str) -> Dict[str, TestConfig]:
+        self.tests_configs = {}
+        self.root = ElementTree.parse(file_path).getroot()
+        if self.root.tag == 'test':
+            test_elements = [self.root]
+        else:
+            test_elements = self.root.findall(TestConfigParser.TEST_KEY)
+        for test_element in test_elements:
+            test_config = self._parse_test(test_element)
+            self.tests_configs[test_config.name] = test_config
+        return self.tests_configs
+
+
+class TestCaseFactory:
+
+    def _make_test_case(
+            self,
+            test_case_name: str,
+            params: Dict[str, object],
+            data_set_config: DataSetConfig) -> TestCase:
+        test_case = TestCase()
+        self.fix_params_typing(params)
+        test_case.induction_params = params
+        test_case.data_set_file_path = f'{DATA_IN_DIRECTORY_PATH}/{data_set_config.train_file_name}'
+        test_case.label_attribute = data_set_config.label_attribute
+        test_case.name = test_case_name
+        test_case.param_config = params
+        return test_case
+
+    def fix_params_typing(self, params: dict):
+        for key, value in params.items():
+            if value == 'false':
+                params[key] = False
+                continue
+            if value == 'true':
+                params[key] = True
+                continue
+            if not 'measure' in key:
+                params[key] = int(float(value))
+
+    def make(self, tests_configs: Dict[str, TestConfig], report_dir_path: str) -> List[TestCase]:
+        test_cases = []
+        for key in tests_configs.keys():
+            test_config = tests_configs[key]
+            for config_name in test_config.parameter_configs.keys():
+                for data_set_config in test_config.datasets:
+                    params = test_config.parameter_configs[config_name]
+                    test_case_name = f'{key}.{config_name}.{data_set_config.name}'
+                    test_config.parameter_configs[config_name].pop('use_expert', None)
+                    expert_rules = test_config.parameter_configs[config_name].pop('expert_rules', None)
+                    preferred_conditions = test_config.parameter_configs[config_name].pop('expert_preferred_conditions',
+                                                                                          None)
+                    forbidden_conditions = test_config.parameter_configs[config_name].pop('expert_forbidden_conditions',
+                                                                                          None)
+                    test_case = self._make_test_case(test_case_name,
+                                                     test_config.parameter_configs[config_name], data_set_config)
+                    if 'use_report' in params:
+                        report_file_name = params['use_report']
+                        test_case.using_existing_report_file = True
+                    else:
+                        report_file_name = test_case_name
+                    report_path = f'{report_dir_path}/{report_file_name}'
+                    test_case.report_file_path = report_path
+                    test_case.survival_time = data_set_config.survival_time
+                    if expert_rules is not None or preferred_conditions is not None or forbidden_conditions is not None:
+                        test_case.knowledge = Knowledge()
+                        test_case.knowledge.expert_rules = expert_rules
+                        test_case.knowledge.expert_forbidden_conditions = forbidden_conditions
+                        test_case.knowledge.expert_preferred_conditions = preferred_conditions
+                    test_cases.append(test_case)
+        return test_cases
+
+
+def get_rule_string(rule) -> str:
+    return re.sub(r'(\\[[^\\]]*\\]$)|(\\([^\\)]*\\)$)', '', str(rule))
+
+
+class TestReportReader:
+
+    def __init__(self, file_name: str, example_set_meta_data):
+        self.example_set_meta_data = example_set_meta_data
+        self.file_name = file_name
+        self._file = f = open(file_name, "r")
+
+    def _read_rules(self, test_report: TestReport):
+        rules = []
+        for line in self._file:
+            if len(line) == 0:
+                break
+            else:
+                rules.append(line)
+        test_report.rules = rules
+
+    def read(self) -> TestReport:
+        test_report = TestReport(self.file_name)
+        for line in self._file:
+            line = line.upper()
+            line = re.sub(r'\t', '', line)
+            line = line.replace('\n', '')
+            if line == REPORTS_SECTIONS_HEADERS['RULES']:
+                self._read_rules(test_report)
+            elif line == '':
+                continue
+            else:
+                raise ValueError(f'Invalid report file format for file: {self.file_name}')
+        return test_report
+
+    def close(self):
+        self._file.close()
+
+
+class TestReportWriter:
+
+    def __init__(self, file_name: str):
+        self._file = f = open(file_name, "w")
+        if not os.path.exists(REPORTS_OUT_DIRECTORY_PATH):
+            os.makedirs(REPORTS_OUT_DIRECTORY_PATH)
+
+    def write(self, rule_set):
+        self._file.write('\n')
+        self._file.write(f'{REPORTS_SECTIONS_HEADERS["RULES"]}\n')
+        for rule in rule_set.rules:
+            self._file.write(f'\t{get_rule_string(rule)}')
+
+    def close(self):
+        self._file.close()
+
+
+def get_test_cases(class_name: str) -> List[TestCase]:
+    if not os.path.exists(DATA_IN_DIRECTORY_PATH):
+        raise Exception('''\n
+Test resources directory dosen't exist. Check if 'tests/resources/' directory exist.
+
+If you're running tests for the first time you need to download resources folder from RuleKit repository by running:
+    python tests/resources.py download
+        ''')
+    configs = TestConfigParser().parse(f'{TEST_CONFIG_PATH}/{class_name}.xml')
+    return TestCaseFactory().make(configs, f'{REPORTS_IN_DIRECTORY_PATH}/{class_name}/')
+
+
+def _get_rule_string(rule: Rule) -> str:
+    return re.sub(r'(\\[[^\\]]*\\]$)|(\\([^\\)]*\\)$)', '', str(rule))
+
+
+def assert_rules_are_equals(expected: List[str], actual: List[str]):
+    def sanitize_rule_string(rule_string: str) -> str:
+        return re.sub(r'(\t)|(\n)|(\[[^\]]*\]$)', '', rule_string)
+
+    if len(expected) != len(actual):
+        raise AssertionError(
+            f'Rulesets have different number of rules, actual: {len(actual)}, expected: {len(expected)}')
+    dictionary = {}
+    for rule in expected:
+        dictionary[sanitize_rule_string(rule)] = 0
+    for rule in actual:
+        key = sanitize_rule_string(rule)
+        if key in dictionary:
+            dictionary[key] = dictionary[key] + 1
+        else:
+            pass
+            raise AssertionError('Actual ruleset contains rules not present in expected ruleset')
+    for key in dictionary.keys():
+        if dictionary[key] == 0:
+            raise AssertionError('Ruleset are not equal, some rules are missing')
+        elif dictionary[key] > 1:
+            raise AssertionError('Somes rules were duplicated')
+
+
+def assert_accuracy_is_greater(prediction, expected, threshold: float):
+    labels = expected.to_numpy().astype(str)
+    acc = metrics.accuracy_score(labels, prediction)
+    if acc <= threshold:
+        raise AssertionError(f'Accuracy should be greater than {threshold}')
+
+
+def assert_score_is_greater(prediction, expected, threshold: float):
+    if isinstance(prediction[0], int):
+        labels = expected.to_numpy().astype(int)
+    if isinstance(prediction[0], float):
+        labels = expected.to_numpy().astype(float)
+    explained_variance_score = metrics.explained_variance_score(labels, prediction)
+
+    if explained_variance_score <= threshold:
+        raise AssertionError(f'Score should be greater than {threshold}')
```

