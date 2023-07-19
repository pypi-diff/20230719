# Comparing `tmp/ghga_datasteward_kit-0.4.4.tar.gz` & `tmp/ghga_datasteward_kit-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghga_datasteward_kit-0.4.4.tar", last modified: Fri Jul 14 08:29:56 2023, max compression
+gzip compressed data, was "ghga_datasteward_kit-0.4.5.tar", last modified: Wed Jul 19 14:55:14 2023, max compression
```

## Comparing `ghga_datasteward_kit-0.4.4.tar` & `ghga_datasteward_kit-0.4.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:29:56.916890 ghga_datasteward_kit-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-14 08:29:56.916890 ghga_datasteward_kit-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:29:56.912890 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6589 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/batch_s3_upload.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3327 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/catalog_accession_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:29:56.912890 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/cli/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/cli/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/file_ingest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22083 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/s3_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:29:56.912890 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-14 08:29:56.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-14 08:29:56.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 08:29:56.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-14 08:29:56.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 08:29:56.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-14 08:29:56.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-14 08:29:56.000000 ghga_datasteward_kit-0.4.4/ghga_datasteward_kit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-14 08:29:56.916890 ghga_datasteward_kit-0.4.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:29:56.912890 ghga_datasteward_kit-0.4.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:29:56.916890 ghga_datasteward_kit-0.4.4/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/tests/fixtures/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/tests/fixtures/ingest.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/tests/fixtures/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/tests/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/tests/test_file_ingest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/tests/test_s3_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-14 08:29:44.000000 ghga_datasteward_kit-0.4.4/tests/test_size_adjustment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:55:14.979410 ghga_datasteward_kit-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-19 14:55:14.979410 ghga_datasteward_kit-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:55:14.975410 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6589 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/batch_s3_upload.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3327 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/catalog_accession_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:55:14.975410 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/cli/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/cli/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/file_ingest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22083 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/s3_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:55:14.975410 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-19 14:55:14.000000 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-19 14:55:14.000000 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 14:55:14.000000 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-19 14:55:14.000000 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 14:55:14.000000 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-19 14:55:14.000000 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-19 14:55:14.000000 ghga_datasteward_kit-0.4.5/ghga_datasteward_kit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-19 14:55:14.979410 ghga_datasteward_kit-0.4.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:55:14.975410 ghga_datasteward_kit-0.4.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:55:14.975410 ghga_datasteward_kit-0.4.5/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/tests/fixtures/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/tests/fixtures/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/tests/fixtures/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/tests/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/tests/test_file_ingest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/tests/test_s3_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-19 14:55:03.000000 ghga_datasteward_kit-0.4.5/tests/test_size_adjustment.py
```

### Comparing `ghga_datasteward_kit-0.4.4/LICENSE` & `ghga_datasteward_kit-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.4/PKG-INFO` & `ghga_datasteward_kit-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga_datasteward_kit
-Version: 0.4.4
+Version: 0.4.5
 Summary: GHGA Data Steward Kit - A utils package for GHGA data stewards.
 Home-page: https://github.com/ghga-de/ghga-datasteward-kit
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ghga_datasteward_kit-0.4.4/README.md` & `ghga_datasteward_kit-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/__init__.py` & `ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/cli/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""A utils package for GHGA data stewards."""
+"""The command line interface of the package."""
 
-__version__ = "0.4.4"
+from .main import cli  # noqa: F401
```

### Comparing `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/__main__.py` & `ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/batch_s3_upload.py` & `ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/batch_s3_upload.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/catalog_accession_generator.py` & `ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/catalog_accession_generator.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/cli/__init__.py` & `ghga_datasteward_kit-0.4.5/tests/fixtures/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,10 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""The command line interface of the package."""
-
-from .main import cli  # noqa: F401
+"""Fixtures that are used in both integration and unit tests"""
```

### Comparing `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/cli/file.py` & `ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/cli/file.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/cli/main.py` & `ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/cli/main.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/cli/metadata.py` & `ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/cli/metadata.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/config.py` & `ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/config.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/file_ingest.py` & `ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/file_ingest.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/loading.py` & `ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/loading.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/main.py` & `ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/main.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/metadata.py` & `ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/metadata.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/models.py` & `ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/models.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/s3_upload.py` & `ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/s3_upload.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit/utils.py` & `ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit.egg-info/PKG-INFO` & `ghga_datasteward_kit-0.4.5/ghga_datasteward_kit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga-datasteward-kit
-Version: 0.4.4
+Version: 0.4.5
 Summary: GHGA Data Steward Kit - A utils package for GHGA data stewards.
 Home-page: https://github.com/ghga-de/ghga-datasteward-kit
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ghga_datasteward_kit-0.4.4/ghga_datasteward_kit.egg-info/SOURCES.txt` & `ghga_datasteward_kit-0.4.5/ghga_datasteward_kit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.4/setup.cfg` & `ghga_datasteward_kit-0.4.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
 	crypt4gh==1.6
-	hexkit[mongodb,s3]==0.10.0
-	ghga-transpiler==1.0.3
+	hexkit[s3]>=0.10,<0.11
+	ghga-transpiler>=1.0.3,<1.1
 	metldata==0.3.6
 python_requires = >= 3.9
 
 [options.entry_points]
 console_scripts = 
 	ghga-datasteward-kit = ghga_datasteward_kit.__main__:run
```

### Comparing `ghga_datasteward_kit-0.4.4/setup.py` & `ghga_datasteward_kit-0.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.4/tests/fixtures/__init__.py` & `ghga_datasteward_kit-0.4.5/tests/fixtures/metadata.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,8 +9,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Fixtures that are used in both integration and unit tests"""
+"""Metadata paths for tests"""
+
+from tests.fixtures.utils import BASE_DIR
+
+METADATA_CONFIG_PATH = BASE_DIR / "metadata_config.yaml"
+ORIGINAL_METADATA_PATH = BASE_DIR / "original_metadata.yaml"
+ORIGINAL_MODEL_PATH = BASE_DIR / "original_model.yaml"
```

### Comparing `ghga_datasteward_kit-0.4.4/tests/fixtures/config.py` & `ghga_datasteward_kit-0.4.5/tests/fixtures/config.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.4/tests/fixtures/ingest.py` & `ghga_datasteward_kit-0.4.5/tests/fixtures/ingest.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.4/tests/fixtures/metadata.py` & `ghga_datasteward_kit-0.4.5/ghga_datasteward_kit/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,14 +9,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Metadata paths for tests"""
+"""A utils package for GHGA data stewards."""
 
-from tests.fixtures.utils import BASE_DIR
-
-METADATA_CONFIG_PATH = BASE_DIR / "metadata_config.yaml"
-ORIGINAL_METADATA_PATH = BASE_DIR / "original_metadata.yaml"
-ORIGINAL_MODEL_PATH = BASE_DIR / "original_model.yaml"
+__version__ = "0.4.5"
```

### Comparing `ghga_datasteward_kit-0.4.4/tests/fixtures/utils.py` & `ghga_datasteward_kit-0.4.5/tests/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.4/tests/test_file_ingest.py` & `ghga_datasteward_kit-0.4.5/tests/test_file_ingest.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.4/tests/test_metadata.py` & `ghga_datasteward_kit-0.4.5/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.4/tests/test_s3_upload.py` & `ghga_datasteward_kit-0.4.5/tests/test_s3_upload.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.4/tests/test_size_adjustment.py` & `ghga_datasteward_kit-0.4.5/tests/test_size_adjustment.py`

 * *Files identical despite different names*

