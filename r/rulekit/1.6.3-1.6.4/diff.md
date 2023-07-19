# Comparing `tmp/rulekit-1.6.3.tar.gz` & `tmp/rulekit-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rulekit-1.6.3.tar", last modified: Wed Jul 19 13:30:40 2023, max compression
+gzip compressed data, was "rulekit-1.6.4.tar", last modified: Wed Jul 19 13:34:50 2023, max compression
```

## Comparing `rulekit-1.6.3.tar` & `rulekit-1.6.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 13:30:40.245444 rulekit-1.6.3/
--rw-rw-rw-   0        0        0    35179 2023-07-19 12:51:13.000000 rulekit-1.6.3/LICENSE
--rw-rw-rw-   0        0        0       98 2023-07-19 12:51:13.000000 rulekit-1.6.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2650 2023-07-19 13:30:40.246403 rulekit-1.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     1502 2023-07-19 12:51:13.000000 rulekit-1.6.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 13:30:40.217078 rulekit-1.6.3/rulekit/
--rw-rw-rw-   0        0        0       96 2023-07-19 13:30:26.000000 rulekit-1.6.3/rulekit/__init__.py
--rw-rw-rw-   0        0        0     2496 2023-07-19 13:30:15.000000 rulekit-1.6.3/rulekit/__main__.py
--rw-rw-rw-   0        0        0      628 2023-07-19 13:24:37.000000 rulekit-1.6.3/rulekit/_experiment.py
--rw-rw-rw-   0        0        0    15677 2023-07-19 13:24:37.000000 rulekit-1.6.3/rulekit/_helpers.py
--rw-rw-rw-   0        0        0     8224 2023-07-19 13:24:37.000000 rulekit-1.6.3/rulekit/_operator.py
--rw-rw-rw-   0        0        0    30917 2023-07-19 13:24:37.000000 rulekit-1.6.3/rulekit/classification.py
-drwxrwxrwx   0        0        0        0 2023-07-19 13:30:40.234401 rulekit-1.6.3/rulekit/jar/
--rw-rw-rw-   0        0        0        0 2023-07-19 12:51:13.000000 rulekit-1.6.3/rulekit/jar/__init__.py
--rw-rw-rw-   0        0        0  1234599 2023-07-19 12:51:13.000000 rulekit-1.6.3/rulekit/jar/mockito-all-1.10.19.jar
--rw-rw-rw-   0        0        0     4426 2023-07-19 13:24:37.000000 rulekit-1.6.3/rulekit/main.py
--rw-rw-rw-   0        0        0     2826 2023-07-19 13:24:37.000000 rulekit-1.6.3/rulekit/params.py
--rw-rw-rw-   0        0        0    21371 2023-07-19 13:24:37.000000 rulekit-1.6.3/rulekit/regression.py
--rw-rw-rw-   0        0        0     8769 2023-07-19 13:24:37.000000 rulekit-1.6.3/rulekit/rules.py
--rw-rw-rw-   0        0        0     5453 2023-07-19 13:24:37.000000 rulekit-1.6.3/rulekit/stats.py
--rw-rw-rw-   0        0        0    27460 2023-07-19 13:24:37.000000 rulekit-1.6.3/rulekit/survival.py
-drwxrwxrwx   0        0        0        0 2023-07-19 13:30:40.232400 rulekit-1.6.3/rulekit.egg-info/
--rw-rw-rw-   0        0        0     2650 2023-07-19 13:30:40.000000 rulekit-1.6.3/rulekit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      732 2023-07-19 13:30:40.000000 rulekit-1.6.3/rulekit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 13:30:40.000000 rulekit-1.6.3/rulekit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      111 2023-07-19 13:30:40.000000 rulekit-1.6.3/rulekit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-19 13:30:40.000000 rulekit-1.6.3/rulekit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-19 13:30:40.250417 rulekit-1.6.3/setup.cfg
--rw-rw-rw-   0        0        0     1809 2023-07-19 13:30:24.000000 rulekit-1.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-19 13:30:40.245444 rulekit-1.6.3/tests/
--rw-rw-rw-   0        0        0      107 2023-07-19 12:51:13.000000 rulekit-1.6.3/tests/__init__.py
--rw-rw-rw-   0        0        0     2608 2023-07-19 13:24:37.000000 rulekit-1.6.3/tests/resources.py
--rw-rw-rw-   0        0        0     5667 2023-07-19 13:24:37.000000 rulekit-1.6.3/tests/test_classifier.py
--rw-rw-rw-   0        0        0     2098 2023-07-19 12:51:13.000000 rulekit-1.6.3/tests/test_regression.py
--rw-rw-rw-   0        0        0      909 2023-07-19 12:51:13.000000 rulekit-1.6.3/tests/test_rulekit.py
--rw-rw-rw-   0        0        0     5881 2023-07-19 12:51:13.000000 rulekit-1.6.3/tests/test_serialization.py
--rw-rw-rw-   0        0        0     1163 2023-07-19 12:51:13.000000 rulekit-1.6.3/tests/test_sklearn_metrics.py
--rw-rw-rw-   0        0        0      649 2023-07-19 12:51:13.000000 rulekit-1.6.3/tests/test_statistics.py
--rw-rw-rw-   0        0        0     2013 2023-07-19 12:51:13.000000 rulekit-1.6.3/tests/test_survival.py
--rw-rw-rw-   0        0        0    16052 2023-07-19 13:24:37.000000 rulekit-1.6.3/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-19 13:34:50.039576 rulekit-1.6.4/
+-rw-rw-rw-   0        0        0    35179 2023-07-19 12:51:13.000000 rulekit-1.6.4/LICENSE
+-rw-rw-rw-   0        0        0       98 2023-07-19 12:51:13.000000 rulekit-1.6.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2650 2023-07-19 13:34:50.040577 rulekit-1.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1502 2023-07-19 12:51:13.000000 rulekit-1.6.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 13:34:50.012574 rulekit-1.6.4/rulekit/
+-rw-rw-rw-   0        0        0       96 2023-07-19 13:34:35.000000 rulekit-1.6.4/rulekit/__init__.py
+-rw-rw-rw-   0        0        0     2496 2023-07-19 13:30:15.000000 rulekit-1.6.4/rulekit/__main__.py
+-rw-rw-rw-   0        0        0      628 2023-07-19 13:24:37.000000 rulekit-1.6.4/rulekit/_experiment.py
+-rw-rw-rw-   0        0        0    15677 2023-07-19 13:24:37.000000 rulekit-1.6.4/rulekit/_helpers.py
+-rw-rw-rw-   0        0        0     8224 2023-07-19 13:34:01.000000 rulekit-1.6.4/rulekit/_operator.py
+-rw-rw-rw-   0        0        0    30917 2023-07-19 13:24:37.000000 rulekit-1.6.4/rulekit/classification.py
+drwxrwxrwx   0        0        0        0 2023-07-19 13:34:50.030576 rulekit-1.6.4/rulekit/jar/
+-rw-rw-rw-   0        0        0        0 2023-07-19 12:51:13.000000 rulekit-1.6.4/rulekit/jar/__init__.py
+-rw-rw-rw-   0        0        0  1234599 2023-07-19 12:51:13.000000 rulekit-1.6.4/rulekit/jar/mockito-all-1.10.19.jar
+-rw-rw-rw-   0        0        0     4426 2023-07-19 13:24:37.000000 rulekit-1.6.4/rulekit/main.py
+-rw-rw-rw-   0        0        0     2889 2023-07-19 13:34:28.000000 rulekit-1.6.4/rulekit/params.py
+-rw-rw-rw-   0        0        0    21371 2023-07-19 13:24:37.000000 rulekit-1.6.4/rulekit/regression.py
+-rw-rw-rw-   0        0        0     8769 2023-07-19 13:24:37.000000 rulekit-1.6.4/rulekit/rules.py
+-rw-rw-rw-   0        0        0     5453 2023-07-19 13:24:37.000000 rulekit-1.6.4/rulekit/stats.py
+-rw-rw-rw-   0        0        0    27460 2023-07-19 13:24:37.000000 rulekit-1.6.4/rulekit/survival.py
+drwxrwxrwx   0        0        0        0 2023-07-19 13:34:50.028571 rulekit-1.6.4/rulekit.egg-info/
+-rw-rw-rw-   0        0        0     2650 2023-07-19 13:34:49.000000 rulekit-1.6.4/rulekit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      732 2023-07-19 13:34:49.000000 rulekit-1.6.4/rulekit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 13:34:49.000000 rulekit-1.6.4/rulekit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      111 2023-07-19 13:34:49.000000 rulekit-1.6.4/rulekit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-19 13:34:49.000000 rulekit-1.6.4/rulekit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-19 13:34:50.043576 rulekit-1.6.4/setup.cfg
+-rw-rw-rw-   0        0        0     1809 2023-07-19 13:34:33.000000 rulekit-1.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 13:34:50.039576 rulekit-1.6.4/tests/
+-rw-rw-rw-   0        0        0      107 2023-07-19 12:51:13.000000 rulekit-1.6.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     2608 2023-07-19 13:24:37.000000 rulekit-1.6.4/tests/resources.py
+-rw-rw-rw-   0        0        0     5667 2023-07-19 13:24:37.000000 rulekit-1.6.4/tests/test_classifier.py
+-rw-rw-rw-   0        0        0     2098 2023-07-19 12:51:13.000000 rulekit-1.6.4/tests/test_regression.py
+-rw-rw-rw-   0        0        0      909 2023-07-19 12:51:13.000000 rulekit-1.6.4/tests/test_rulekit.py
+-rw-rw-rw-   0        0        0     5881 2023-07-19 12:51:13.000000 rulekit-1.6.4/tests/test_serialization.py
+-rw-rw-rw-   0        0        0     1163 2023-07-19 12:51:13.000000 rulekit-1.6.4/tests/test_sklearn_metrics.py
+-rw-rw-rw-   0        0        0      649 2023-07-19 12:51:13.000000 rulekit-1.6.4/tests/test_statistics.py
+-rw-rw-rw-   0        0        0     2013 2023-07-19 12:51:13.000000 rulekit-1.6.4/tests/test_survival.py
+-rw-rw-rw-   0        0        0    16052 2023-07-19 13:24:37.000000 rulekit-1.6.4/tests/utils.py
```

### Comparing `rulekit-1.6.3/LICENSE` & `rulekit-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.3/PKG-INFO` & `rulekit-1.6.4/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rulekit
-Version: 1.6.3
+Version: 1.6.4
 Summary: Comprehensive suite for rule-based learning
 Home-page: https://github.com/adaa-polsl/RuleKit
 Download-URL: https://github.com/adaa-polsl/RuleKit-python/archive/refs/tags/v1.6.0.tar.gz
 Author: Cezary Maszczyk
 Author-email: cezary.maszczyk@gmail.com
 Project-URL: Bug Tracker, https://github.com/adaa-polsl/RuleKit-python/issues
 Project-URL: Documentation, https://adaa-polsl.github.io/RuleKit-python/
```

### Comparing `rulekit-1.6.3/README.md` & `rulekit-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.3/rulekit/__main__.py` & `rulekit-1.6.4/rulekit/__main__.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.3/rulekit/_experiment.py` & `rulekit-1.6.4/rulekit/_experiment.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.3/rulekit/_helpers.py` & `rulekit-1.6.4/rulekit/_helpers.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.3/rulekit/_operator.py` & `rulekit-1.6.4/rulekit/_operator.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.3/rulekit/classification.py` & `rulekit-1.6.4/rulekit/classification.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.3/rulekit/jar/mockito-all-1.10.19.jar` & `rulekit-1.6.4/rulekit/jar/mockito-all-1.10.19.jar`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.3/rulekit/main.py` & `rulekit-1.6.4/rulekit/main.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.3/rulekit/params.py` & `rulekit-1.6.4/rulekit/params.py`

 * *Files 12% similar despite different names*

```diff
@@ -57,32 +57,32 @@
     YAILS = 'YAILS'
     LogRank = 'LogRank'
 
 
 class ModelsParams(BaseModel):
     """Model for validating models hyperparameters
     """
-    min_rule_covered: Optional[int]
-    minsupp_new: Optional[int]
+    min_rule_covered: Optional[int] = None
+    minsupp_new: Optional[int] = None
     induction_measure: Measures
     pruning_measure: Measures
     voting_measure: Measures
     max_growing: float
     enable_pruning: bool
     ignore_missing: bool
     max_uncovered_fraction: float
     select_best_candidate: bool
 
-    extend_using_preferred: Optional[bool]
-    extend_using_automatic: Optional[bool]
-    induce_using_preferred: Optional[bool]
-    induce_using_automatic: Optional[bool]
-    consider_other_classes: Optional[bool]
-    preferred_conditions_per_rule: Optional[int]
-    preferred_attributes_per_rule: Optional[int]
+    extend_using_preferred: Optional[bool] = None
+    extend_using_automatic: Optional[bool] = None
+    induce_using_preferred: Optional[bool] = None
+    induce_using_automatic: Optional[bool] = None
+    consider_other_classes: Optional[bool] = None
+    preferred_conditions_per_rule: Optional[int] = None
+    preferred_attributes_per_rule: Optional[int] = None
 
 
 class ContrastSetModelParams(ModelsParams):
     """Model for validating contrast set models hyperparameters
     """
     minsupp_all: str
     max_neg2pos: float
```

### Comparing `rulekit-1.6.3/rulekit/regression.py` & `rulekit-1.6.4/rulekit/regression.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.3/rulekit/rules.py` & `rulekit-1.6.4/rulekit/rules.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.3/rulekit/stats.py` & `rulekit-1.6.4/rulekit/stats.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.3/rulekit/survival.py` & `rulekit-1.6.4/rulekit/survival.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.3/rulekit.egg-info/PKG-INFO` & `rulekit-1.6.4/rulekit.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rulekit
-Version: 1.6.3
+Version: 1.6.4
 Summary: Comprehensive suite for rule-based learning
 Home-page: https://github.com/adaa-polsl/RuleKit
 Download-URL: https://github.com/adaa-polsl/RuleKit-python/archive/refs/tags/v1.6.0.tar.gz
 Author: Cezary Maszczyk
 Author-email: cezary.maszczyk@gmail.com
 Project-URL: Bug Tracker, https://github.com/adaa-polsl/RuleKit-python/issues
 Project-URL: Documentation, https://adaa-polsl.github.io/RuleKit-python/
```

### Comparing `rulekit-1.6.3/rulekit.egg-info/SOURCES.txt` & `rulekit-1.6.4/rulekit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.3/setup.py` & `rulekit-1.6.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 current_path = os.path.dirname(os.path.realpath(__file__))
 
 with io.open("README.md", mode="r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rulekit",
-    version='1.6.3',
+    version='1.6.4',
     author="Cezary Maszczyk",
     author_email="cezary.maszczyk@gmail.com",
     description="Comprehensive suite for rule-based learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/adaa-polsl/RuleKit",
     packages=setuptools.find_packages(),
```

### Comparing `rulekit-1.6.3/tests/resources.py` & `rulekit-1.6.4/tests/resources.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.3/tests/test_classifier.py` & `rulekit-1.6.4/tests/test_classifier.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.3/tests/test_regression.py` & `rulekit-1.6.4/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.3/tests/test_rulekit.py` & `rulekit-1.6.4/tests/test_rulekit.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.3/tests/test_serialization.py` & `rulekit-1.6.4/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.3/tests/test_sklearn_metrics.py` & `rulekit-1.6.4/tests/test_sklearn_metrics.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.3/tests/test_statistics.py` & `rulekit-1.6.4/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.3/tests/test_survival.py` & `rulekit-1.6.4/tests/test_survival.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.3/tests/utils.py` & `rulekit-1.6.4/tests/utils.py`

 * *Files identical despite different names*

