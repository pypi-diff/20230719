# Comparing `tmp/bb-connector-0.0.2.tar.gz` & `tmp/bb-connector-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bb-connector-0.0.2.tar", last modified: Wed Jul 19 07:49:49 2023, max compression
+gzip compressed data, was "bb-connector-0.0.3.tar", last modified: Wed Jul 19 08:11:51 2023, max compression
```

## Comparing `bb-connector-0.0.2.tar` & `bb-connector-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 07:49:49.518413 bb-connector-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-07-18 11:36:36.000000 bb-connector-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1163 2023-07-19 07:49:49.517415 bb-connector-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      608 2023-07-14 14:56:50.000000 bb-connector-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 07:49:49.498416 bb-connector-0.0.2/bb_connector.egg-info/
--rw-rw-rw-   0        0        0     1163 2023-07-19 07:49:49.000000 bb-connector-0.0.2/bb_connector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2023-07-19 07:49:49.000000 bb-connector-0.0.2/bb_connector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 07:49:49.000000 bb-connector-0.0.2/bb_connector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-19 07:49:49.000000 bb-connector-0.0.2/bb_connector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       89 2023-07-19 07:49:49.000000 bb-connector-0.0.2/bb_connector.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-19 07:49:49.000000 bb-connector-0.0.2/bb_connector.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-19 07:49:49.499414 bb-connector-0.0.2/main/
--rw-rw-rw-   0        0        0        0 2023-07-19 07:24:36.000000 bb-connector-0.0.2/main/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 07:49:49.508434 bb-connector-0.0.2/main/flask_service/
--rw-rw-rw-   0        0        0        0 2023-07-13 11:07:16.000000 bb-connector-0.0.2/main/flask_service/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 07:49:49.512416 bb-connector-0.0.2/main/flask_service/entity/
--rw-rw-rw-   0        0        0        0 2023-07-13 11:07:25.000000 bb-connector-0.0.2/main/flask_service/entity/__init__.py
--rw-rw-rw-   0        0        0     4039 2023-07-17 15:15:00.000000 bb-connector-0.0.2/main/flask_service/entity/bql.py
-drwxrwxrwx   0        0        0        0 2023-07-19 07:49:49.516433 bb-connector-0.0.2/main/flask_service/exception/
--rw-rw-rw-   0        0        0        0 2023-07-17 09:09:06.000000 bb-connector-0.0.2/main/flask_service/exception/__init__.py
--rw-rw-rw-   0        0        0      280 2023-07-17 15:15:00.000000 bb-connector-0.0.2/main/flask_service/exception/handler.py
--rw-rw-rw-   0        0        0     2296 2023-07-19 07:48:35.000000 bb-connector-0.0.2/main/flask_service/main.py
--rw-rw-rw-   0        0        0       42 2023-07-19 07:49:49.518413 bb-connector-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1655 2023-07-19 07:49:08.000000 bb-connector-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 08:11:51.645307 bb-connector-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-07-18 11:36:36.000000 bb-connector-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1163 2023-07-19 08:11:51.644307 bb-connector-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      608 2023-07-14 14:56:50.000000 bb-connector-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 08:11:51.634307 bb-connector-0.0.3/bb_connector.egg-info/
+-rw-rw-rw-   0        0        0     1163 2023-07-19 08:11:51.000000 bb-connector-0.0.3/bb_connector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2023-07-19 08:11:51.000000 bb-connector-0.0.3/bb_connector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 08:11:51.000000 bb-connector-0.0.3/bb_connector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-07-19 08:11:51.000000 bb-connector-0.0.3/bb_connector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       89 2023-07-19 08:11:51.000000 bb-connector-0.0.3/bb_connector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-19 08:11:51.000000 bb-connector-0.0.3/bb_connector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 08:11:51.635308 bb-connector-0.0.3/main/
+-rw-rw-rw-   0        0        0        0 2023-07-19 07:24:36.000000 bb-connector-0.0.3/main/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 08:11:51.637307 bb-connector-0.0.3/main/flask_service/
+-rw-rw-rw-   0        0        0        0 2023-07-13 11:07:16.000000 bb-connector-0.0.3/main/flask_service/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 08:11:51.640323 bb-connector-0.0.3/main/flask_service/entity/
+-rw-rw-rw-   0        0        0        0 2023-07-13 11:07:25.000000 bb-connector-0.0.3/main/flask_service/entity/__init__.py
+-rw-rw-rw-   0        0        0     4039 2023-07-17 15:15:00.000000 bb-connector-0.0.3/main/flask_service/entity/bql.py
+drwxrwxrwx   0        0        0        0 2023-07-19 08:11:51.643308 bb-connector-0.0.3/main/flask_service/exception/
+-rw-rw-rw-   0        0        0        0 2023-07-17 09:09:06.000000 bb-connector-0.0.3/main/flask_service/exception/__init__.py
+-rw-rw-rw-   0        0        0      280 2023-07-17 15:15:00.000000 bb-connector-0.0.3/main/flask_service/exception/handler.py
+-rw-rw-rw-   0        0        0     2296 2023-07-19 07:48:35.000000 bb-connector-0.0.3/main/flask_service/main.py
+-rw-rw-rw-   0        0        0       42 2023-07-19 08:11:51.645307 bb-connector-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1660 2023-07-19 08:08:59.000000 bb-connector-0.0.3/setup.py
```

### Comparing `bb-connector-0.0.2/LICENSE` & `bb-connector-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bb-connector-0.0.2/PKG-INFO` & `bb-connector-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bb-connector
-Version: 0.0.2
+Version: 0.0.3
 Summary: This project is a flask-service for calculating Bloomberg query's as a REST service.
 Author: Richard Maidorn
 Author-email: maidorn@orcacapital.de
 Project-URL: Source Code, https://gitlab.com/orca-capital/algo-trading/python/bb-connector
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `bb-connector-0.0.2/README.md` & `bb-connector-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bb-connector-0.0.2/bb_connector.egg-info/PKG-INFO` & `bb-connector-0.0.3/bb_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bb-connector
-Version: 0.0.2
+Version: 0.0.3
 Summary: This project is a flask-service for calculating Bloomberg query's as a REST service.
 Author: Richard Maidorn
 Author-email: maidorn@orcacapital.de
 Project-URL: Source Code, https://gitlab.com/orca-capital/algo-trading/python/bb-connector
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `bb-connector-0.0.2/main/flask_service/entity/bql.py` & `bb-connector-0.0.3/main/flask_service/entity/bql.py`

 * *Files identical despite different names*

### Comparing `bb-connector-0.0.2/main/flask_service/main.py` & `bb-connector-0.0.3/main/flask_service/main.py`

 * *Files identical despite different names*

### Comparing `bb-connector-0.0.2/setup.py` & `bb-connector-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,29 +18,29 @@
     required = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="bb-connector",
-    version="0.0.2",
+    version="0.0.3",
     author='Richard Maidorn',
     author_email="maidorn@orcacapital.de",
     description="This project is a flask-service for calculating Bloomberg query's as a REST service.",
     python_requires='>=3.11',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=required,
     cmdclass={
                  'install': BlpapiInstall
     },
     entry_points={
         'console_scripts': [
-            'bb-connector=flask_service.main:main',
+            'bb-connector=main.flask_service.main:main',
         ]
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         'License :: OSI Approved :: MIT License',
         "Operating System :: Microsoft :: Windows",
     ],
```

