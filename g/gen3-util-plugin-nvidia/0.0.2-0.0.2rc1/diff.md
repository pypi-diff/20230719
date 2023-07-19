# Comparing `tmp/gen3_util_plugin_nvidia-0.0.2.tar.gz` & `tmp/gen3_util_plugin_nvidia-0.0.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3_util_plugin_nvidia-0.0.2.tar", last modified: Wed Jul 19 00:23:19 2023, max compression
+gzip compressed data, was "gen3_util_plugin_nvidia-0.0.2rc1.tar", last modified: Fri Jul  7 01:24:40 2023, max compression
```

## Comparing `gen3_util_plugin_nvidia-0.0.2.tar` & `gen3_util_plugin_nvidia-0.0.2rc1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-19 00:23:19.285423 gen3_util_plugin_nvidia-0.0.2/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2808 2023-07-19 00:23:19.284956 gen3_util_plugin_nvidia-0.0.2/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     2099 2023-07-19 00:13:41.000000 gen3_util_plugin_nvidia-0.0.2/README.md
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-19 00:23:19.280397 gen3_util_plugin_nvidia-0.0.2/gen3_util_plugin_nvidia/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2607 2023-07-19 00:20:37.000000 gen3_util_plugin_nvidia-0.0.2/gen3_util_plugin_nvidia/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-19 00:23:19.284591 gen3_util_plugin_nvidia-0.0.2/gen3_util_plugin_nvidia.egg-info/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2808 2023-07-19 00:23:19.000000 gen3_util_plugin_nvidia-0.0.2/gen3_util_plugin_nvidia.egg-info/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142      338 2023-07-19 00:23:19.000000 gen3_util_plugin_nvidia-0.0.2/gen3_util_plugin_nvidia.egg-info/SOURCES.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142        1 2023-07-19 00:23:19.000000 gen3_util_plugin_nvidia-0.0.2/gen3_util_plugin_nvidia.egg-info/dependency_links.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       20 2023-07-19 00:23:19.000000 gen3_util_plugin_nvidia-0.0.2/gen3_util_plugin_nvidia.egg-info/entry_points.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       10 2023-07-19 00:23:19.000000 gen3_util_plugin_nvidia-0.0.2/gen3_util_plugin_nvidia.egg-info/requires.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       24 2023-07-19 00:23:19.000000 gen3_util_plugin_nvidia-0.0.2/gen3_util_plugin_nvidia.egg-info/top_level.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       38 2023-07-19 00:23:19.285487 gen3_util_plugin_nvidia-0.0.2/setup.cfg
--rw-r--r--   0 walsbr   (320923486) 1971611142     5633 2023-07-19 00:23:04.000000 gen3_util_plugin_nvidia-0.0.2/setup.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 01:24:40.714250 gen3_util_plugin_nvidia-0.0.2rc1/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1894 2023-07-07 01:24:40.713921 gen3_util_plugin_nvidia-0.0.2rc1/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1182 2023-07-07 00:58:11.000000 gen3_util_plugin_nvidia-0.0.2rc1/README.md
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 01:24:40.706614 gen3_util_plugin_nvidia-0.0.2rc1/gen3_util_plugin_nvidia/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2525 2023-07-06 22:25:19.000000 gen3_util_plugin_nvidia-0.0.2rc1/gen3_util_plugin_nvidia/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 01:24:40.712796 gen3_util_plugin_nvidia-0.0.2rc1/gen3_util_plugin_nvidia.egg-info/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1894 2023-07-07 01:24:40.000000 gen3_util_plugin_nvidia-0.0.2rc1/gen3_util_plugin_nvidia.egg-info/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142      338 2023-07-07 01:24:40.000000 gen3_util_plugin_nvidia-0.0.2rc1/gen3_util_plugin_nvidia.egg-info/SOURCES.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142        1 2023-07-07 01:24:40.000000 gen3_util_plugin_nvidia-0.0.2rc1/gen3_util_plugin_nvidia.egg-info/dependency_links.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       20 2023-07-07 01:24:40.000000 gen3_util_plugin_nvidia-0.0.2rc1/gen3_util_plugin_nvidia.egg-info/entry_points.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       10 2023-07-07 01:24:40.000000 gen3_util_plugin_nvidia-0.0.2rc1/gen3_util_plugin_nvidia.egg-info/requires.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       24 2023-07-07 01:24:40.000000 gen3_util_plugin_nvidia-0.0.2rc1/gen3_util_plugin_nvidia.egg-info/top_level.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       38 2023-07-07 01:24:40.714313 gen3_util_plugin_nvidia-0.0.2rc1/setup.cfg
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5636 2023-07-07 01:24:16.000000 gen3_util_plugin_nvidia-0.0.2rc1/setup.py
```

### Comparing `gen3_util_plugin_nvidia-0.0.2/README.md` & `gen3_util_plugin_nvidia-0.0.2rc1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -8,81 +8,34 @@
 ```commandline
 source venv/bin/activate
 python3 -m pip install -r requirements.txt
 python3 -m pip install -r requirements-dev.txt  
 python3 -m pip install -e .
 ```
 
-## Run meta import with --plugin_path
-
-The input directory:
-
-```
-tests/fixtures-new/
-├── HandE
-├── RegisteredImages
-│   ├── 17633-6-Scene-001
-│   ├── 18538-6-Scene-001
-│   ├── 19142-6-Scene-001
-│   ├── 24952-6-Scene-001
-│   ├── 30411-6-Scene-001
-│   ├── 31022-6-Scene-001
-│   ├── 31480-6-Scene-001
-│   ├── 33548-6-Scene-001
-│   ├── 38592-6-Scene-001
-│   ├── 48411-6-Scene-001
-│   ├── 54774-4-Scene-001
-│   ├── 57494-6-Scene-001
-│   └── 57658-6-Scene-001
-└── annotations
+## Run the import with `--plugin_path` 
 
 ```
-
-will produce:
-
-```
-gen3_util meta  import dir tests/fixtures/ tmp/output --project_id aced-nvidia --plugin_path gen3_util_plugin_nvidia --remove_path_prefix tests/fixtures/
-summary:
-  ResearchStudy:
-    count: 1
-  ResearchSubject:
-    count: 13
-  Patient:
-    count: 13
-  Specimen:
-    count: 13
-  DocumentReference:
-    count: 738
-    size: 74437
-msg: OK
-
-
+gen3_util meta  import dir INPUT_PATH OUTPUT_PATH --project_id aced-nvidia --plugin_path {plugin_path}
 ```
 
 ### expected results
 
-Output files:
-
-```
-tmp/output
-├── DocumentReference.ndjson
-├── Patient.ndjson
-├── ResearchStudy.ndjson
-├── ResearchSubject.ndjson
-└── Specimen.ndjson
 ```
+data
+├── fhir
+│   ├── DocumentReference.ndjson
+│   ├── Patient.ndjson
+│   ├── ResearchStudy.ndjson
+│   ├── ResearchSubject.ndjson
+│   ├── Specimen.ndjson
+│   └── Task.ndjson
 
-Identifiers:
 
 ```
-$ cat tmp/output/*.ndjson | jq -rc '. as $r | .identifier[]? | [$r.resourceType, .value]'
-["Patient","P1"]
-["Specimen","T1"]
-```
-
 
 ## Run the tests
 
 ```
 pytest  tests/
 ```
 ## Distribution
```

### Comparing `gen3_util_plugin_nvidia-0.0.2/setup.py` & `gen3_util_plugin_nvidia-0.0.2rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name='gen3_util_plugin_nvidia',  # Required
 
     # Versions should comply with PEP 440:
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.2',  # Required
+    version='0.0.2rc1',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='CEDAR / NVIDIA collaboration',
     # Optional
```

