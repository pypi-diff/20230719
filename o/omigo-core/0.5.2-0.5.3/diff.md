# Comparing `tmp/omigo_core-0.5.2.tar.gz` & `tmp/omigo_core-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omigo_core-0.5.2.tar", last modified: Thu May 25 19:16:48 2023, max compression
+gzip compressed data, was "omigo_core-0.5.3.tar", last modified: Tue Jul 18 22:40:12 2023, max compression
```

## Comparing `omigo_core-0.5.2.tar` & `omigo_core-0.5.3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:16:48.455191 omigo_core-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-25 19:16:48.455191 omigo_core-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:16:29.000000 omigo_core-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-25 19:16:29.000000 omigo_core-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-25 19:16:48.455191 omigo_core-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:16:48.451190 omigo_core-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:16:48.451190 omigo_core-0.5.2/src/omigo_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/etl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/file_io_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/file_paths_data_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/file_paths_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    14386 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/file_paths_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/funclib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/local_fs_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12393 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/s3_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    17089 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/s3io_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)   213923 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/tsv.py
--rw-r--r--   0 runner    (1001) docker     (123)    28370 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/tsvutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18448 2023-05-25 19:16:29.000000 omigo_core-0.5.2/src/omigo_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:16:48.455191 omigo_core-0.5.2/src/omigo_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-25 19:16:48.000000 omigo_core-0.5.2/src/omigo_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-25 19:16:48.000000 omigo_core-0.5.2/src/omigo_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:16:48.000000 omigo_core-0.5.2/src/omigo_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-25 19:16:48.000000 omigo_core-0.5.2/src/omigo_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 19:16:48.000000 omigo_core-0.5.2/src/omigo_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:16:48.455191 omigo_core-0.5.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-25 19:16:29.000000 omigo_core-0.5.2/test/test_tsv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:40:12.535642 omigo_core-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-18 22:40:12.535642 omigo_core-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 22:39:56.000000 omigo_core-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-18 22:39:56.000000 omigo_core-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-18 22:40:12.535642 omigo_core-0.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:40:12.531643 omigo_core-0.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:40:12.535642 omigo_core-0.5.3/src/omigo_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/file_io_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/file_paths_data_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/file_paths_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15075 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/file_paths_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/funclib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18893 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/graph_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/local_fs_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/s3_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17128 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/s3io_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)   214991 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/tsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28370 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/tsvutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-07-18 22:39:56.000000 omigo_core-0.5.3/src/omigo_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:40:12.535642 omigo_core-0.5.3/src/omigo_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-18 22:40:12.000000 omigo_core-0.5.3/src/omigo_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-18 22:40:12.000000 omigo_core-0.5.3/src/omigo_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 22:40:12.000000 omigo_core-0.5.3/src/omigo_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-18 22:40:12.000000 omigo_core-0.5.3/src/omigo_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-18 22:40:12.000000 omigo_core-0.5.3/src/omigo_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:40:12.535642 omigo_core-0.5.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-18 22:39:56.000000 omigo_core-0.5.3/test/test_tsv.py
```

### Comparing `omigo_core-0.5.2/PKG-INFO` & `omigo_core-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omigo_core
-Version: 0.5.2
+Version: 0.5.3
 Summary: Data Analytics Library for Python
 Home-page: https://github.com/CrowdStrike/omigo-data-analytics
 Author: amit jaiswal
 Author-email: amit.jaiswal@gmail.com
 Project-URL: Bug Tracker, https://github.com/CrowdStrike/omigo-data-analytics/browse
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `omigo_core-0.5.2/setup.cfg` & `omigo_core-0.5.3/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = omigo_core
-version = 0.5.2
+version = 0.5.3
 author = amit jaiswal
 author_email = amit.jaiswal@gmail.com
 description = Data Analytics Library for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CrowdStrike/omigo-data-analytics
 project_urls =
```

### Comparing `omigo_core-0.5.2/src/omigo_core/etl.py` & `omigo_core-0.5.3/src/omigo_core/etl.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.2/src/omigo_core/file_io_wrapper.py` & `omigo_core-0.5.3/src/omigo_core/file_io_wrapper.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.2/src/omigo_core/file_paths_data_reader.py` & `omigo_core-0.5.3/src/omigo_core/file_paths_data_reader.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.2/src/omigo_core/file_paths_reader.py` & `omigo_core-0.5.3/src/omigo_core/file_paths_reader.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.2/src/omigo_core/file_paths_util.py` & `omigo_core-0.5.3/src/omigo_core/file_paths_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 from omigo_core import utils
 from omigo_core import funclib 
 from omigo_core import local_fs_wrapper
 # constant
 NUM_HOURS = 24
 
 # method to read the data
-def read_filepaths(path, start_date_str, end_date_str, fileprefix, s3_region, aws_profile, granularity, ignore_missing = False):
+def read_filepaths(path, start_date_str, end_date_str, fileprefix, s3_region = None, aws_profile = None, granularity = "hourly", ignore_missing = False):
     if (granularity == "hourly"):
-        return read_filepaths_hourly(path, start_date_str, end_date_str, fileprefix, s3_region, aws_profile, "", ignore_missing)
+        return read_filepaths_hourly(path, start_date_str, end_date_str, fileprefix, s3_region = s3_region, aws_profile = aws_profile, etl_level = "", ignore_missing = ignore_missing)
     elif (granularity == "daily"):
-        return read_filepaths_daily(path, start_date_str, end_date_str, fileprefix, s3_region, aws_profile, "", ignore_missing)
+        return read_filepaths_daily(path, start_date_str, end_date_str, fileprefix, s3_region = s3_region, aws_profile = aws_profile, etl_level = "", ignore_missing = ignore_missing)
     else:
         raise Exception("Unknown granularity value", granularity)
 
 # this returns the etl prefix for creating directory depth
 def get_etl_level_prefix(curdate, etl_level):
     prefix = "/"
     if (etl_level == ""):
@@ -39,15 +39,16 @@
         else:
             raise Exception("Invalid value for etl_level :", etl_level, part)
 
         prefix = prefix + part + "-" + str(curdate.strftime(f)) + "/"
 
     return prefix
 
-def read_filepaths_hourly(path, start_date_str, end_date_str, fileprefix, s3_region, aws_profile, etl_level, ignore_missing):
+def read_filepaths_hourly(path, start_date_str, end_date_str, fileprefix, s3_region = None, aws_profile = None, etl_level = "", ignore_missing = False):
+    utils.warn_once("read_filepaths_hourly is confusing and may be unsupported")
     # parse input dates
     start_date = datetime.datetime.strptime(start_date_str,"%Y-%m-%d")
     end_date = datetime.datetime.strptime(end_date_str,"%Y-%m-%d")
 
     # construct paths based on the dates
     duration = end_date - start_date
     # print("read_filepaths_hourly: Number of days:", duration.days + 1)
@@ -62,19 +63,19 @@
             etl_prefix = get_etl_level_prefix(curdatetime, etl_level)
             filepath_tsv = path + etl_prefix + fileprefix + "-" + curdatetime.strftime("%Y%m%d-%H0000") + ".tsv"
             filepath_tsvgz = filepath_tsv + ".gz"
             filepath_tsvzip = filepath_tsv + ".zip"
 
             # check if this is s3 file
             if (filepath_tsv.startswith("s3://")):
-                if (s3_wrapper.check_path_exists(filepath_tsv, s3_region, aws_profile)):
+                if (s3_wrapper.check_path_exists(filepath_tsv, s3_region = s3_region, aws_profile = aws_profile)):
                     filepaths.append(filepath_tsv)
-                elif (s3_wrapper.check_path_exists(filepath_tsvgz, s3_region, aws_profile)):
+                elif (s3_wrapper.check_path_exists(filepath_tsvgz, s3_region = s3_region, aws_profile = aws_profile)):
                     filepaths.append(filepath_tsvgz)
-                elif (s3_wrapper.check_path_exists(filepath_tsvzip, s3_region, aws_profile)):
+                elif (s3_wrapper.check_path_exists(filepath_tsvzip, s3_region = s3_region, aws_profile = aws_profile)):
                     filepaths.append(filepath_tsvzip)
                 else:
                     if (ignore_missing == False):
                         raise Exception("Input files don't exist. Use ignore_missing if want to continue: ", filepath_tsv, filepath_tsvgz, filepath_tsvzip)
                     else:
                         continue
             else:
@@ -91,23 +92,24 @@
                     else:
                         continue
 
     # return filepaths
     return filepaths
 
 def check_exists(path, s3_region = None, aws_profile = None):
-    if (path.startswith("s3://") and s3_wrapper.check_path_exists(path, s3_region, aws_profile)):
+    if (path.startswith("s3://") and s3_wrapper.check_path_exists(path, s3_region = s3_region, aws_profile = aws_profile)):
         return True
 
     if (local_fs_wrapper.check_path_exists(path)):
         return True
 
     return False
 
-def read_filepaths_daily(path, start_date_str, end_date_str, fileprefix, s3_region, aws_profile, etl_level, ignore_missing):
+def read_filepaths_daily(path, start_date_str, end_date_str, fileprefix, s3_region = None, aws_profile = None, etl_level = "", ignore_missing = False):
+    utils.warn_once("read_filepaths_daily is confusing and may be unsupported")
     # parse input dates
     start_date = datetime.datetime.strptime(start_date_str, "%Y-%m-%d")
     end_date = datetime.datetime.strptime(end_date_str, "%Y-%m-%d")
 
     # construct paths based on the dates
     duration = end_date - start_date
     #print("read_filepaths_daily: Number of days:", duration.days + 1)
@@ -120,17 +122,17 @@
         curdate = start_date + datetime.timedelta(days = i)
         etl_prefix = get_etl_level_prefix(curdate, etl_level)
         filepath_tsv = path + etl_prefix + fileprefix + "-" + curdate.strftime("%Y%m%d") + "-" + curdate.strftime("%Y%m%d") + ".tsv"
         filepath_tsvgz = filepath_tsv + ".gz"
 
         # check if this is s3 file
         if (filepath_tsv.startswith("s3://") or filepath_tsvgz.startswith("s3://")):
-            if (s3_wrapper.check_path_exists(filepath_tsv, s3_region, aws_profile)):
+            if (s3_wrapper.check_path_exists(filepath_tsv, s3_region = s3_region, aws_profile = aws_profile)):
                 filepaths.append(filepath_tsv)
-            elif (s3_wrapper.check_path_exists(filepath_tsvgz, s3_region, aws_profile)):
+            elif (s3_wrapper.check_path_exists(filepath_tsvgz, s3_region = s3_region, aws_profile = aws_profile)):
                 filepaths.append(filepath_tsvgz)
             else:
                 if (ignore_missing == False):
                     raise Exception("Input files don't exist. Use ignore_missing if want to continue: ", filepath_tsv, filepath_tsvgz)
                 else:
                     continue
         else:
@@ -154,15 +156,15 @@
     header_set = {}
 
     # read the headers to make sure that all files are same
     for filepath in filepaths:
         # print(filepath)
 
         # read content
-        lines = read_file_content_as_lines(filepath, s3_region, aws_profile)
+        lines = read_file_content_as_lines(filepath, s3_region = s3_region, aws_profile = aws_profile)
 
         # read header
         headerline = lines[0].rstrip("\n")
         if ((headerline in header_set.keys()) == False):
             header_set[headerline] = filepath
 
     # check for no data
@@ -197,15 +199,15 @@
 
     return header_map
 
 def read_file_content_as_lines(path, s3_region = None, aws_profile = None):
     # check for s3
     if (path.startswith("s3://")):
         bucket_name, object_key = utils.split_s3_path(path)
-        data = s3_wrapper.get_file_content_as_text(bucket_name, object_key, s3_region, aws_profile)
+        data = s3_wrapper.get_file_content_as_text(bucket_name, object_key, s3_region = s3_region, aws_profile = aws_profile)
         data = data.split("\n")
     else:
         if (path.endswith(".gz")):
             fin = gzip.open(path, mode = "rt")
             data = [x.rstrip("\n") for x in fin.readlines()]
             fin.close()
         elif (path.endswith(".zip")):
@@ -255,17 +257,18 @@
     for d in range(num_days):
         # generate the current path based on date
         cur_date = start_date_minus_window + datetime.timedelta(days = d)
         cur_path = path + "/dt=" + cur_date.strftime("%Y%m%d")
 
         # get the list of files. This needs to be failsafe as not all directories may exist
         if (path.startswith("s3://")):
-            tasks.append(utils.ThreadPoolTask(s3_wrapper.get_directory_listing, cur_path, filter_func = None, fail_if_missing = False, region = s3_region, profile = aws_profile))
+            tasks.append(utils.ThreadPoolTask(s3_wrapper.get_directory_listing, cur_path, filter_func = None, ignore_if_missing = False, skip_exist_check = True,
+                region = s3_region, profile = aws_profile))
         else:
-            tasks.append(utils.ThreadPoolTask(get_local_directory_listing, cur_path, filter_func = None, fail_if_missing = False))
+            tasks.append(utils.ThreadPoolTask(get_local_directory_listing, cur_path, filter_func = None, fail_if_missing = False, skip_exist_check = True))
 
     # execute the tasks
     results = utils.run_with_thread_pool(tasks, num_par = num_par, wait_sec = wait_sec)
 
     # final result
     paths_found = []
 
@@ -314,16 +317,16 @@
                         # note filename1
                         paths_found.append(filename)
                         utils.trace("file_paths_util: get_file_paths_by_datetime_range: found file: {}".format(filename))
 
     # return
     return paths_found
 
-def get_local_directory_listing(path, filter_func = None, fail_if_missing = True):
-    return local_fs_wrapper.get_directory_listing(path, filter_func = filter_func, fail_if_missing = fail_if_missing)
+def get_local_directory_listing(path, filter_func = None, fail_if_missing = True, skip_exist_check = False):
+    return local_fs_wrapper.get_directory_listing(path, filter_func = filter_func, fail_if_missing = fail_if_missing, skip_exist_check = skip_exist_check)
 
 # this method is not robust against complex path creations with dot(.). FIXME. TODO
 def create_local_parent_dir(filepath):
     utils.warn_once("create_local_parent_dir: os.makedirs can create the full path. Why do we need this method")
 
     # if it is a local file, create the parent directory
     if (filepath.startswith("s3://") == True):
```

### Comparing `omigo_core-0.5.2/src/omigo_core/funclib.py` & `omigo_core-0.5.3/src/omigo_core/funclib.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     vs2 = []
     for v in vs:
         vs2 = vs2 + v.split(",")
     vs2 = list(set(filter(lambda t: len(t.strip()) > 0, vs2)))
     return ",".join(sorted([str(x) for x in vs2]))
 
 def mean(vs):
+    vs = list([float(v) for v in vs])
     return statistics.mean(vs)
 
 def mkstr(vs):
     vs2 = list(filter(lambda t: len(t.strip()) > 0, [str(x) for x in vs]))
     return ",".join(vs2)
 
 def sorted_mkstr(vs):
```

### Comparing `omigo_core-0.5.2/src/omigo_core/local_fs_wrapper.py` & `omigo_core-0.5.3/src/omigo_core/local_fs_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import os
 import datetime
 from omigo_core import funclib
 from omigo_core import utils
+import zipfile, gzip
 
 def check_path_exists(path):
     return os.path.exists(path)
 
 def check_file_exists(path):
     return os.path.exists(path)
 
-def get_directory_listing(path, filter_func = None, fail_if_missing = True):
-    if (check_path_exists(path) == False):
-        if (fail_if_missing):
-            raise Exception("Directory does not exist: {}".format(path))
-        else:
-            return []
-    else:
-        full_paths = []
-        for p in os.listdir(path):
-            full_paths.append(path + "/" + p)
-
-        # apply filter func if any
-        if (filter_func is not None):
-            full_paths = list(filter(lambda t: filter_func(t), full_paths))
+def get_directory_listing(path, filter_func = None, fail_if_missing = True, skip_exist_check = False):
+    # skip_exist_check is for performance and parity with s3
+    if (skip_exist_check == False):
+        if (check_path_exists(path) == False):
+            if (fail_if_missing):
+                raise Exception("Directory does not exist: {}".format(path))
+            else:
+                return []
+
+    full_paths = []
+    for p in os.listdir(path):
+        full_paths.append(path + "/" + p)
+
+    # apply filter func if any
+    if (filter_func is not None):
+        full_paths = list(filter(lambda t: filter_func(t), full_paths))
 
-        # return
-        return full_paths
+    # return
+    return full_paths
 
 # TODO: not in s3
 def makedirs(path, exist_ok = True):
     return os.makedirs(path, exist_ok = exist_ok)
 
 def get_file_content_as_text(path):
     # initialize
```

### Comparing `omigo_core-0.5.2/src/omigo_core/s3io_wrapper.py` & `omigo_core-0.5.3/src/omigo_core/s3io_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,16 +157,16 @@
             return self.__s3_get_directory_listing__(path, skip_exist_check = skip_exist_check)
         else:
             return self.__local_get_directory_listing__(path, skip_exist_check = skip_exist_check)
 
     def __s3_get_directory_listing__(self, path, skip_exist_check = False):
         return s3_wrapper.get_directory_listing(path, skip_exist_check = skip_exist_check)
 
-    def __local_get_directory_listing__(self, path): 
-        return local_fs_wrapper.get_directory_listing(path)
+    def __local_get_directory_listing__(self, path, skip_exist_check = False):
+        return local_fs_wrapper.get_directory_listing(path, skip_exist_check = skip_exist_check)
 
     def list_dirs(self, path):
         path = self.__normalize_path__(path)
         result1 = self.ls(path)
         result2 = list(filter(lambda t: self.is_directory(path + "/" + t), result1))
         return result2
 
@@ -201,24 +201,24 @@
         else:
             # file exists. call delete
             self.delete_file(path, ignore_if_missing = ignore_if_missing)
 
             # verify that the file is deleted
             return self.file_not_exists_with_wait(path)
 
-    def delete_file(self, path, ignore_if_missing = None):
+    def delete_file(self, path, ignore_if_missing = False):
         if (self.__is_s3__(path)):
             return self.__s3_delete_file__(path, ignore_if_missing = ignore_if_missing)
         else:
             return self.__local_delete_file__(path, ignore_if_missing = ignore_if_missing)
 
-    def __s3_delete_file__(self, path, ignore_if_missing = None):
+    def __s3_delete_file__(self, path, ignore_if_missing = False):
         return s3_wrapper.delete_file(path, ignore_if_missing = ignore_if_missing)
 
-    def __local_delete_file__(self, path, ignore_if_missing = None):
+    def __local_delete_file__(self, path, ignore_if_missing = False):
         # delete file
         local_fs_wrapper.delete_file(path, fail_if_missing = ignore_if_missing)
 
         # check if this was the reserved file for directory
         if (path.endswith("/" + RESERVED_HIDDEN_FILE)):
             # delete the directory
             dir_path = path[0:path.rindex("/")]
@@ -228,15 +228,15 @@
         path = self.__normalize_path__(path)
         file_path = "{}/{}".format(path, RESERVED_HIDDEN_FILE)
 
         # check for existence 
         if (self.file_exists(file_path) == False):
             if (ignore_if_missing == True):
                 utils.warn("delete_dir: path doesnt exist: {}, ignore_if_missing: {}".format(path, ignore_if_missing))
-                return
+                return False
             else:
                 raise Exception("delete_dir: path doesnt exist: {}".format(path))
 
         # check if the directory is empty or not. to prevent race conditions
         if (len(self.ls(path)) > 0):
             utils.warn("delete_dir: directory not empty: {}".format(path))
             return False
@@ -298,15 +298,14 @@
             self.__s3_makedirs__(path, levels = levels)
         else:
             self.__local_makedirs__(path, levels = levels)
 
     def __s3_makedirs__(self, path, levels = None):
         # normalize path
         path = self.__normalize_path__(path)
-        parts = path.split("/")
 
         # split path into bucket and key
         bucket_name, object_key = utils.split_s3_path(path)
         # TODO: silent bug probably. The split creates an empty string as first part for leading '/'
         parts = object_key.split("/")
 
         # iterate over all ancestors
```

### Comparing `omigo_core-0.5.2/src/omigo_core/tsv.py` & `omigo_core-0.5.3/src/omigo_core/tsv.py`

 * *Files 1% similar despite different names*

```diff
@@ -2978,23 +2978,50 @@
             selected_values = random.sample(uniq_values, max_uniq_values)  # nosec`
             dmsg = utils.extend_inherit_message(dmsg, "sample_column_by_max_uniq_values")
             return self.values_in(col, selected_values, dmsg = dmsg)
         else:
             utils.warn("sample_column_by_max_uniq_values: max sample size: {} more than number of uniq values: {}".format(max_uniq_values, len(uniq_values)))
             return self
 
+    def sample_class_by_min_class_count(self, col, seed = 0, dmsg = ""):
+        dmsg = utils.extend_inherit_message(dmsg, "sample_class_by_min_class_count")
+
+        # get the cap on any class
+        min_count = int(min(self.group_count(col).col_as_int_array("group:count")))
+
+        # temporary column name
+        temp_col = "__sample_class_by_min_class_count_temp__"
+
+        # return
+        return self \
+            .add_seq_num(temp_col, dmsg = dmsg) \
+            .sample_group_by_max_uniq_values_exact(col, temp_col, min_count, dmsg = dmsg) \
+            .drop_cols(temp_col, dmsg = dmsg) 
+
+    def sample_class_by_max_values(self, col, n, seed = 0, dmsg = ""):
+        dmsg = utils.extend_inherit_message(dmsg, "sample_class_by_max_values")
+
+        # temporary column name
+        temp_col = "__sample_class_by_min_class_count_temp__"
+
+        # return
+        return self \
+            .add_seq_num(temp_col, dmsg = dmsg) \
+            .sample_group_by_max_uniq_values_exact(col, temp_col, n, dmsg = dmsg) \
+            .drop_cols(temp_col, dmsg = dmsg) 
+
     # create descriptive methods for join
     def left_join(self, that, lkeys, rkeys = None, lsuffix = None, rsuffix = None, default_val = "", def_val_map = None, num_par = 0, dmsg = ""):
+        dmsg = utils.extend_inherit_message(dmsg, "left_join")
         # check for empty
         if (self.has_empty_header()):
             utils.warn("left_join: empty this tsv")
             return self
 
         # return
-        dmsg = utils.extend_inherit_message(dmsg, "left_join")
         return self.__join__(that, lkeys, rkeys, join_type = "left", lsuffix = lsuffix, rsuffix = rsuffix, default_val = default_val, def_val_map = def_val_map, num_par = num_par, dmsg = dmsg)
 
     def right_join(self, that, lkeys, rkeys = None, lsuffix = None, rsuffix = None, default_val = "", def_val_map = None, num_par = 0, dmsg = ""):
         dmsg = utils.extend_inherit_message(dmsg, "right_join")
 
         # check for empty
         if (self.has_empty_header()):
@@ -4932,15 +4959,15 @@
         return self
 
     def disable_info_mode(self):
         utils.disable_info_mode()
         return self
 
 def get_version():
-    return "v0.3.9:empty_tsv"
+    return "v0.5.2_1:mean"
 
 def get_func_name(f):
     return f.__name__
 
 def read(paths, sep = None, do_union = False, def_val_map = None):
     # TODO: remove this after fixing design
     if (def_val_map is not None and do_union == False):
```

### Comparing `omigo_core-0.5.2/src/omigo_core/tsvutils.py` & `omigo_core-0.5.3/src/omigo_core/tsvutils.py`

 * *Files identical despite different names*

### Comparing `omigo_core-0.5.2/src/omigo_core/utils.py` & `omigo_core-0.5.3/src/omigo_core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -637,7 +637,13 @@
                        for i3 in range(i4+1, n-2):
                            for i2 in range(i3+1, n-1):
                                for i1 in range(i2+1, n):
                                    result.append([i7, i6, i5, i4, i3, i2, i1])
        return result
 
 
+def split_str_to_arr(x):
+    if (x is None or x == ""):
+        return []
+    else:
+        return list(filter(lambda t: t != "", x.split(",")))
+
```

### Comparing `omigo_core-0.5.2/src/omigo_core.egg-info/PKG-INFO` & `omigo_core-0.5.3/src/omigo_core.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omigo-core
-Version: 0.5.2
+Version: 0.5.3
 Summary: Data Analytics Library for Python
 Home-page: https://github.com/CrowdStrike/omigo-data-analytics
 Author: amit jaiswal
 Author-email: amit.jaiswal@gmail.com
 Project-URL: Bug Tracker, https://github.com/CrowdStrike/omigo-data-analytics/browse
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `omigo_core-0.5.2/src/omigo_core.egg-info/SOURCES.txt` & `omigo_core-0.5.3/src/omigo_core.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 src/omigo_core/__init__.py
 src/omigo_core/etl.py
 src/omigo_core/file_io_wrapper.py
 src/omigo_core/file_paths_data_reader.py
 src/omigo_core/file_paths_reader.py
 src/omigo_core/file_paths_util.py
 src/omigo_core/funclib.py
+src/omigo_core/graph_traversal.py
 src/omigo_core/local_fs_wrapper.py
 src/omigo_core/s3_wrapper.py
 src/omigo_core/s3io_wrapper.py
 src/omigo_core/tsv.py
 src/omigo_core/tsvutils.py
 src/omigo_core/utils.py
 src/omigo_core.egg-info/PKG-INFO
```

