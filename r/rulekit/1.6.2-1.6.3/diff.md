# Comparing `tmp/rulekit-1.6.2.tar.gz` & `tmp/rulekit-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rulekit-1.6.2.tar", last modified: Wed Jul 19 13:26:19 2023, max compression
+gzip compressed data, was "rulekit-1.6.3.tar", last modified: Wed Jul 19 13:30:40 2023, max compression
```

## Comparing `rulekit-1.6.2.tar` & `rulekit-1.6.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 13:26:19.284675 rulekit-1.6.2/
--rw-rw-rw-   0        0        0    35179 2023-07-19 12:51:13.000000 rulekit-1.6.2/LICENSE
--rw-rw-rw-   0        0        0       98 2023-07-19 12:51:13.000000 rulekit-1.6.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2650 2023-07-19 13:26:19.285674 rulekit-1.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     1502 2023-07-19 12:51:13.000000 rulekit-1.6.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 13:26:19.248667 rulekit-1.6.2/rulekit/
--rw-rw-rw-   0        0        0       96 2023-07-19 13:26:00.000000 rulekit-1.6.2/rulekit/__init__.py
--rw-rw-rw-   0        0        0     2487 2023-07-19 13:24:37.000000 rulekit-1.6.2/rulekit/__main__.py
--rw-rw-rw-   0        0        0      628 2023-07-19 13:24:37.000000 rulekit-1.6.2/rulekit/_experiment.py
--rw-rw-rw-   0        0        0    15677 2023-07-19 13:24:37.000000 rulekit-1.6.2/rulekit/_helpers.py
--rw-rw-rw-   0        0        0     8224 2023-07-19 13:24:37.000000 rulekit-1.6.2/rulekit/_operator.py
--rw-rw-rw-   0        0        0    30917 2023-07-19 13:24:37.000000 rulekit-1.6.2/rulekit/classification.py
-drwxrwxrwx   0        0        0        0 2023-07-19 13:26:19.272669 rulekit-1.6.2/rulekit/jar/
--rw-rw-rw-   0        0        0        0 2023-07-19 12:51:13.000000 rulekit-1.6.2/rulekit/jar/__init__.py
--rw-rw-rw-   0        0        0  1234599 2023-07-19 12:51:13.000000 rulekit-1.6.2/rulekit/jar/mockito-all-1.10.19.jar
--rw-rw-rw-   0        0        0     4426 2023-07-19 13:24:37.000000 rulekit-1.6.2/rulekit/main.py
--rw-rw-rw-   0        0        0     2826 2023-07-19 13:24:37.000000 rulekit-1.6.2/rulekit/params.py
--rw-rw-rw-   0        0        0    21371 2023-07-19 13:24:37.000000 rulekit-1.6.2/rulekit/regression.py
--rw-rw-rw-   0        0        0     8769 2023-07-19 13:24:37.000000 rulekit-1.6.2/rulekit/rules.py
--rw-rw-rw-   0        0        0     5453 2023-07-19 13:24:37.000000 rulekit-1.6.2/rulekit/stats.py
--rw-rw-rw-   0        0        0    27460 2023-07-19 13:24:37.000000 rulekit-1.6.2/rulekit/survival.py
-drwxrwxrwx   0        0        0        0 2023-07-19 13:26:19.270667 rulekit-1.6.2/rulekit.egg-info/
--rw-rw-rw-   0        0        0     2650 2023-07-19 13:26:19.000000 rulekit-1.6.2/rulekit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      732 2023-07-19 13:26:19.000000 rulekit-1.6.2/rulekit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 13:26:19.000000 rulekit-1.6.2/rulekit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-19 13:26:19.000000 rulekit-1.6.2/rulekit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-19 13:26:19.000000 rulekit-1.6.2/rulekit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-19 13:26:19.289677 rulekit-1.6.2/setup.cfg
--rw-rw-rw-   0        0        0     1780 2023-07-19 13:26:03.000000 rulekit-1.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-19 13:26:19.284675 rulekit-1.6.2/tests/
--rw-rw-rw-   0        0        0      107 2023-07-19 12:51:13.000000 rulekit-1.6.2/tests/__init__.py
--rw-rw-rw-   0        0        0     2608 2023-07-19 13:24:37.000000 rulekit-1.6.2/tests/resources.py
--rw-rw-rw-   0        0        0     5667 2023-07-19 13:24:37.000000 rulekit-1.6.2/tests/test_classifier.py
--rw-rw-rw-   0        0        0     2098 2023-07-19 12:51:13.000000 rulekit-1.6.2/tests/test_regression.py
--rw-rw-rw-   0        0        0      909 2023-07-19 12:51:13.000000 rulekit-1.6.2/tests/test_rulekit.py
--rw-rw-rw-   0        0        0     5881 2023-07-19 12:51:13.000000 rulekit-1.6.2/tests/test_serialization.py
--rw-rw-rw-   0        0        0     1163 2023-07-19 12:51:13.000000 rulekit-1.6.2/tests/test_sklearn_metrics.py
--rw-rw-rw-   0        0        0      649 2023-07-19 12:51:13.000000 rulekit-1.6.2/tests/test_statistics.py
--rw-rw-rw-   0        0        0     2013 2023-07-19 12:51:13.000000 rulekit-1.6.2/tests/test_survival.py
--rw-rw-rw-   0        0        0    16052 2023-07-19 13:24:37.000000 rulekit-1.6.2/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-19 13:30:40.245444 rulekit-1.6.3/
+-rw-rw-rw-   0        0        0    35179 2023-07-19 12:51:13.000000 rulekit-1.6.3/LICENSE
+-rw-rw-rw-   0        0        0       98 2023-07-19 12:51:13.000000 rulekit-1.6.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2650 2023-07-19 13:30:40.246403 rulekit-1.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1502 2023-07-19 12:51:13.000000 rulekit-1.6.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 13:30:40.217078 rulekit-1.6.3/rulekit/
+-rw-rw-rw-   0        0        0       96 2023-07-19 13:30:26.000000 rulekit-1.6.3/rulekit/__init__.py
+-rw-rw-rw-   0        0        0     2496 2023-07-19 13:30:15.000000 rulekit-1.6.3/rulekit/__main__.py
+-rw-rw-rw-   0        0        0      628 2023-07-19 13:24:37.000000 rulekit-1.6.3/rulekit/_experiment.py
+-rw-rw-rw-   0        0        0    15677 2023-07-19 13:24:37.000000 rulekit-1.6.3/rulekit/_helpers.py
+-rw-rw-rw-   0        0        0     8224 2023-07-19 13:24:37.000000 rulekit-1.6.3/rulekit/_operator.py
+-rw-rw-rw-   0        0        0    30917 2023-07-19 13:24:37.000000 rulekit-1.6.3/rulekit/classification.py
+drwxrwxrwx   0        0        0        0 2023-07-19 13:30:40.234401 rulekit-1.6.3/rulekit/jar/
+-rw-rw-rw-   0        0        0        0 2023-07-19 12:51:13.000000 rulekit-1.6.3/rulekit/jar/__init__.py
+-rw-rw-rw-   0        0        0  1234599 2023-07-19 12:51:13.000000 rulekit-1.6.3/rulekit/jar/mockito-all-1.10.19.jar
+-rw-rw-rw-   0        0        0     4426 2023-07-19 13:24:37.000000 rulekit-1.6.3/rulekit/main.py
+-rw-rw-rw-   0        0        0     2826 2023-07-19 13:24:37.000000 rulekit-1.6.3/rulekit/params.py
+-rw-rw-rw-   0        0        0    21371 2023-07-19 13:24:37.000000 rulekit-1.6.3/rulekit/regression.py
+-rw-rw-rw-   0        0        0     8769 2023-07-19 13:24:37.000000 rulekit-1.6.3/rulekit/rules.py
+-rw-rw-rw-   0        0        0     5453 2023-07-19 13:24:37.000000 rulekit-1.6.3/rulekit/stats.py
+-rw-rw-rw-   0        0        0    27460 2023-07-19 13:24:37.000000 rulekit-1.6.3/rulekit/survival.py
+drwxrwxrwx   0        0        0        0 2023-07-19 13:30:40.232400 rulekit-1.6.3/rulekit.egg-info/
+-rw-rw-rw-   0        0        0     2650 2023-07-19 13:30:40.000000 rulekit-1.6.3/rulekit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      732 2023-07-19 13:30:40.000000 rulekit-1.6.3/rulekit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 13:30:40.000000 rulekit-1.6.3/rulekit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      111 2023-07-19 13:30:40.000000 rulekit-1.6.3/rulekit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-19 13:30:40.000000 rulekit-1.6.3/rulekit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-19 13:30:40.250417 rulekit-1.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     1809 2023-07-19 13:30:24.000000 rulekit-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 13:30:40.245444 rulekit-1.6.3/tests/
+-rw-rw-rw-   0        0        0      107 2023-07-19 12:51:13.000000 rulekit-1.6.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     2608 2023-07-19 13:24:37.000000 rulekit-1.6.3/tests/resources.py
+-rw-rw-rw-   0        0        0     5667 2023-07-19 13:24:37.000000 rulekit-1.6.3/tests/test_classifier.py
+-rw-rw-rw-   0        0        0     2098 2023-07-19 12:51:13.000000 rulekit-1.6.3/tests/test_regression.py
+-rw-rw-rw-   0        0        0      909 2023-07-19 12:51:13.000000 rulekit-1.6.3/tests/test_rulekit.py
+-rw-rw-rw-   0        0        0     5881 2023-07-19 12:51:13.000000 rulekit-1.6.3/tests/test_serialization.py
+-rw-rw-rw-   0        0        0     1163 2023-07-19 12:51:13.000000 rulekit-1.6.3/tests/test_sklearn_metrics.py
+-rw-rw-rw-   0        0        0      649 2023-07-19 12:51:13.000000 rulekit-1.6.3/tests/test_statistics.py
+-rw-rw-rw-   0        0        0     2013 2023-07-19 12:51:13.000000 rulekit-1.6.3/tests/test_survival.py
+-rw-rw-rw-   0        0        0    16052 2023-07-19 13:24:37.000000 rulekit-1.6.3/tests/utils.py
```

### Comparing `rulekit-1.6.2/LICENSE` & `rulekit-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.2/PKG-INFO` & `rulekit-1.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rulekit
-Version: 1.6.2
+Version: 1.6.3
 Summary: Comprehensive suite for rule-based learning
 Home-page: https://github.com/adaa-polsl/RuleKit
 Download-URL: https://github.com/adaa-polsl/RuleKit-python/archive/refs/tags/v1.6.0.tar.gz
 Author: Cezary Maszczyk
 Author-email: cezary.maszczyk@gmail.com
 Project-URL: Bug Tracker, https://github.com/adaa-polsl/RuleKit-python/issues
 Project-URL: Documentation, https://adaa-polsl.github.io/RuleKit-python/
```

### Comparing `rulekit-1.6.2/README.md` & `rulekit-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.2/rulekit/__main__.py` & `rulekit-1.6.3/rulekit/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 REPOSITORY_URL: str = 'https://api.github.com/repos/adaa-polsl/RuleKit'
 
 
 def _download_rulekit_jar():
     release_version = 'latest'
     current_rulekit_jars_files: list[str] = glob.glob(
         f"{dir_path}/jar/*-all.jar")
-    url = f"{REPOSITORY_URL}/{release_version}"
+    url = f"{REPOSITORY_URL}/releases/{release_version}"
     req = urllib.request.Request(url)
     req.add_header('Content-Type', 'application/json; charset=utf-8')
     response = urllib.request.urlopen(req)
     response = json.loads(response.read())
     latest_release_version = response['tag_name']
     print('Fetching latest RuleKit release version: ', latest_release_version)
     assets = response['assets']
```

### Comparing `rulekit-1.6.2/rulekit/_experiment.py` & `rulekit-1.6.3/rulekit/_experiment.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.2/rulekit/_helpers.py` & `rulekit-1.6.3/rulekit/_helpers.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.2/rulekit/_operator.py` & `rulekit-1.6.3/rulekit/_operator.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.2/rulekit/classification.py` & `rulekit-1.6.3/rulekit/classification.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.2/rulekit/jar/mockito-all-1.10.19.jar` & `rulekit-1.6.3/rulekit/jar/mockito-all-1.10.19.jar`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.2/rulekit/main.py` & `rulekit-1.6.3/rulekit/main.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.2/rulekit/params.py` & `rulekit-1.6.3/rulekit/params.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.2/rulekit/regression.py` & `rulekit-1.6.3/rulekit/regression.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.2/rulekit/rules.py` & `rulekit-1.6.3/rulekit/rules.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.2/rulekit/stats.py` & `rulekit-1.6.3/rulekit/stats.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.2/rulekit/survival.py` & `rulekit-1.6.3/rulekit/survival.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.2/rulekit.egg-info/PKG-INFO` & `rulekit-1.6.3/rulekit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rulekit
-Version: 1.6.2
+Version: 1.6.3
 Summary: Comprehensive suite for rule-based learning
 Home-page: https://github.com/adaa-polsl/RuleKit
 Download-URL: https://github.com/adaa-polsl/RuleKit-python/archive/refs/tags/v1.6.0.tar.gz
 Author: Cezary Maszczyk
 Author-email: cezary.maszczyk@gmail.com
 Project-URL: Bug Tracker, https://github.com/adaa-polsl/RuleKit-python/issues
 Project-URL: Documentation, https://adaa-polsl.github.io/RuleKit-python/
```

### Comparing `rulekit-1.6.2/rulekit.egg-info/SOURCES.txt` & `rulekit-1.6.3/rulekit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.2/setup.py` & `rulekit-1.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 current_path = os.path.dirname(os.path.realpath(__file__))
 
 with io.open("README.md", mode="r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rulekit",
-    version='1.6.2',
+    version='1.6.3',
     author="Cezary Maszczyk",
     author_email="cezary.maszczyk@gmail.com",
     description="Comprehensive suite for rule-based learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/adaa-polsl/RuleKit",
     packages=setuptools.find_packages(),
@@ -34,14 +34,15 @@
     install_requires=[
         "pandas ~= 1.5.2",
         "scikit-learn ~= 1.2.0",
         "requests ~= 2.25.1",
         "scipy ~= 1.9.3",
         "joblib >= 1.0,< 1.3",
         "JPype1 ~= 1.4.1",
+        "pydantic ~= 2.0.3"
     ],
     test_suite="tests",
     download_url = 'https://github.com/adaa-polsl/RuleKit-python/archive/refs/tags/v1.6.0.tar.gz',
     project_urls={
         'Bug Tracker': 'https://github.com/adaa-polsl/RuleKit-python/issues',
         'Documentation': 'https://adaa-polsl.github.io/RuleKit-python/',
         'Source Code': 'https://github.com/adaa-polsl/RuleKit-python'
```

### Comparing `rulekit-1.6.2/tests/resources.py` & `rulekit-1.6.3/tests/resources.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.2/tests/test_classifier.py` & `rulekit-1.6.3/tests/test_classifier.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.2/tests/test_regression.py` & `rulekit-1.6.3/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.2/tests/test_rulekit.py` & `rulekit-1.6.3/tests/test_rulekit.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.2/tests/test_serialization.py` & `rulekit-1.6.3/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.2/tests/test_sklearn_metrics.py` & `rulekit-1.6.3/tests/test_sklearn_metrics.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.2/tests/test_statistics.py` & `rulekit-1.6.3/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.2/tests/test_survival.py` & `rulekit-1.6.3/tests/test_survival.py`

 * *Files identical despite different names*

### Comparing `rulekit-1.6.2/tests/utils.py` & `rulekit-1.6.3/tests/utils.py`

 * *Files identical despite different names*

