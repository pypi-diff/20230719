# Comparing `tmp/lmpylib-mingsqtt-1.0.6.tar.gz` & `tmp/lmpylib-mingsqtt-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lmpylib-mingsqtt-1.0.6.tar", last modified: Mon Nov  7 15:24:31 2022, max compression
+gzip compressed data, was "dist/lmpylib-mingsqtt-1.0.7.tar", last modified: Wed Jul 19 03:37:22 2023, max compression
```

## Comparing `lmpylib-mingsqtt-1.0.6.tar` & `lmpylib-mingsqtt-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 liming     (501) staff       (20)        0 2022-11-07 15:24:31.000000 lmpylib-mingsqtt-1.0.6/
--rw-r--r--   0 liming     (501) staff       (20)      465 2022-11-07 15:24:31.000000 lmpylib-mingsqtt-1.0.6/PKG-INFO
--rw-r--r--   0 liming     (501) staff       (20)      167 2020-06-06 15:27:26.000000 lmpylib-mingsqtt-1.0.6/README.md
-drwxr-xr-x   0 liming     (501) staff       (20)        0 2022-11-07 15:24:31.000000 lmpylib-mingsqtt-1.0.6/lmpylib/
--rw-r--r--   0 liming     (501) staff       (20)        0 2020-06-06 15:27:26.000000 lmpylib-mingsqtt-1.0.6/lmpylib/__init__.py
--rw-r--r--   0 liming     (501) staff       (20)     3750 2022-10-14 01:58:49.000000 lmpylib-mingsqtt-1.0.6/lmpylib/byteutil.py
--rw-r--r--   0 liming     (501) staff       (20)   147763 2022-10-30 10:44:20.000000 lmpylib-mingsqtt-1.0.6/lmpylib/core.py
--rw-r--r--   0 liming     (501) staff       (20)    15240 2020-06-06 15:27:26.000000 lmpylib-mingsqtt-1.0.6/lmpylib/cv.py
--rw-r--r--   0 liming     (501) staff       (20)    27250 2022-07-05 02:53:07.000000 lmpylib-mingsqtt-1.0.6/lmpylib/geo.py
--rw-r--r--   0 liming     (501) staff       (20)    52996 2021-01-12 09:44:49.000000 lmpylib-mingsqtt-1.0.6/lmpylib/nlp.py
--rw-r--r--   0 liming     (501) staff       (20)     5726 2020-06-14 13:47:01.000000 lmpylib-mingsqtt-1.0.6/lmpylib/sigproc.py
--rw-r--r--   0 liming     (501) staff       (20)       22 2022-11-07 15:24:27.000000 lmpylib-mingsqtt-1.0.6/lmpylib/version.py
-drwxr-xr-x   0 liming     (501) staff       (20)        0 2022-11-07 15:24:31.000000 lmpylib-mingsqtt-1.0.6/lmpylib_mingsqtt.egg-info/
--rw-r--r--   0 liming     (501) staff       (20)      465 2022-11-07 15:24:30.000000 lmpylib-mingsqtt-1.0.6/lmpylib_mingsqtt.egg-info/PKG-INFO
--rw-r--r--   0 liming     (501) staff       (20)      316 2022-11-07 15:24:30.000000 lmpylib-mingsqtt-1.0.6/lmpylib_mingsqtt.egg-info/SOURCES.txt
--rw-r--r--   0 liming     (501) staff       (20)        1 2022-11-07 15:24:30.000000 lmpylib-mingsqtt-1.0.6/lmpylib_mingsqtt.egg-info/dependency_links.txt
--rw-r--r--   0 liming     (501) staff       (20)        8 2022-11-07 15:24:30.000000 lmpylib-mingsqtt-1.0.6/lmpylib_mingsqtt.egg-info/top_level.txt
--rw-r--r--   0 liming     (501) staff       (20)       38 2022-11-07 15:24:31.000000 lmpylib-mingsqtt-1.0.6/setup.cfg
--rw-r--r--   0 liming     (501) staff       (20)      820 2020-06-06 17:20:38.000000 lmpylib-mingsqtt-1.0.6/setup.py
+drwxr-xr-x   0 liming     (501) staff       (20)        0 2023-07-19 03:37:22.000000 lmpylib-mingsqtt-1.0.7/
+-rw-r--r--   0 liming     (501) staff       (20)      465 2023-07-19 03:37:22.000000 lmpylib-mingsqtt-1.0.7/PKG-INFO
+-rw-r--r--   0 liming     (501) staff       (20)      167 2020-06-06 15:27:26.000000 lmpylib-mingsqtt-1.0.7/README.md
+drwxr-xr-x   0 liming     (501) staff       (20)        0 2023-07-19 03:37:22.000000 lmpylib-mingsqtt-1.0.7/lmpylib/
+-rw-r--r--   0 liming     (501) staff       (20)        0 2020-06-06 15:27:26.000000 lmpylib-mingsqtt-1.0.7/lmpylib/__init__.py
+-rw-r--r--   0 liming     (501) staff       (20)     3750 2022-10-14 01:58:49.000000 lmpylib-mingsqtt-1.0.7/lmpylib/byteutil.py
+-rw-r--r--   0 liming     (501) staff       (20)   147785 2023-07-19 03:37:17.000000 lmpylib-mingsqtt-1.0.7/lmpylib/core.py
+-rw-r--r--   0 liming     (501) staff       (20)    15240 2020-06-06 15:27:26.000000 lmpylib-mingsqtt-1.0.7/lmpylib/cv.py
+-rw-r--r--   0 liming     (501) staff       (20)    27267 2023-03-13 06:19:52.000000 lmpylib-mingsqtt-1.0.7/lmpylib/geo.py
+-rw-r--r--   0 liming     (501) staff       (20)    52996 2021-01-12 09:44:49.000000 lmpylib-mingsqtt-1.0.7/lmpylib/nlp.py
+-rw-r--r--   0 liming     (501) staff       (20)     5726 2020-06-14 13:47:01.000000 lmpylib-mingsqtt-1.0.7/lmpylib/sigproc.py
+-rw-r--r--   0 liming     (501) staff       (20)       22 2023-07-19 03:37:17.000000 lmpylib-mingsqtt-1.0.7/lmpylib/version.py
+drwxr-xr-x   0 liming     (501) staff       (20)        0 2023-07-19 03:37:22.000000 lmpylib-mingsqtt-1.0.7/lmpylib_mingsqtt.egg-info/
+-rw-r--r--   0 liming     (501) staff       (20)      465 2023-07-19 03:37:21.000000 lmpylib-mingsqtt-1.0.7/lmpylib_mingsqtt.egg-info/PKG-INFO
+-rw-r--r--   0 liming     (501) staff       (20)      316 2023-07-19 03:37:21.000000 lmpylib-mingsqtt-1.0.7/lmpylib_mingsqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 liming     (501) staff       (20)        1 2023-07-19 03:37:21.000000 lmpylib-mingsqtt-1.0.7/lmpylib_mingsqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 liming     (501) staff       (20)        8 2023-07-19 03:37:21.000000 lmpylib-mingsqtt-1.0.7/lmpylib_mingsqtt.egg-info/top_level.txt
+-rw-r--r--   0 liming     (501) staff       (20)       38 2023-07-19 03:37:22.000000 lmpylib-mingsqtt-1.0.7/setup.cfg
+-rw-r--r--   0 liming     (501) staff       (20)      820 2020-06-06 17:20:38.000000 lmpylib-mingsqtt-1.0.7/setup.py
```

### Comparing `lmpylib-mingsqtt-1.0.6/lmpylib/byteutil.py` & `lmpylib-mingsqtt-1.0.7/lmpylib/byteutil.py`

 * *Files identical despite different names*

### Comparing `lmpylib-mingsqtt-1.0.6/lmpylib/core.py` & `lmpylib-mingsqtt-1.0.7/lmpylib/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,27 +314,27 @@
             return sum_return
     elif type_data == pd.DataFrame:
         sum_return = {}
         numeric_summaries = None
         datetime_summaries = None
         for colname in data.columns:
             summ = summary(data[colname])
-            if auto_combine_result & (type(summ) == pd.DataFrame) & (
+            if auto_combine_result and (type(summ) == pd.DataFrame) and (
             np.all(summ.columns.to_list() == ["Min", "Q1", "Median", "Mean", "Q3", "Max", "Len", "NA"])):
                 summ.index = [colname]
                 if str(summ.dtypes[0]).find("date") >= 0:
                     if datetime_summaries is None:
                         datetime_summaries = summ
                     else:
-                        datetime_summaries = datetime_summaries.append(summ, ignore_index=False)
+                        datetime_summaries = pd.concat([datetime_summaries, summ], ignore_index=False)
                 else:
                     if numeric_summaries is None:
                         numeric_summaries = summ
                     else:
-                        numeric_summaries = numeric_summaries.append(summ, ignore_index=False)
+                        numeric_summaries = pd.concat([numeric_summaries, summ], ignore_index=False)
             else:
                 sum_return[colname] = summ
 
         if numeric_summaries is not None:
             if numeric_summaries.shape[0] > 1:
                 sum_return["NumericColumns"] = numeric_summaries
             else:
@@ -378,15 +378,15 @@
         outlier_summaries = None
         for colname in data.columns:
             summ = outlier_summary(data[colname], iqr_multiplier=iqr_multiplier, std_multiplier=std_multiplier, one_sided=one_sided)
             summ.index = [colname]
             if outlier_summaries is None:
                 outlier_summaries = summ
             else:
-                outlier_summaries = outlier_summaries.append(summ, ignore_index=False)
+                outlier_summaries = pd.concat([outlier_summaries, summ], ignore_index=False)
 
         if (print_only is not None) and print_only:
             print(outlier_summaries, "\n")
         else:
             return outlier_summaries
     else:
         print("Unsupported type {}".format(type_data))
```

### Comparing `lmpylib-mingsqtt-1.0.6/lmpylib/cv.py` & `lmpylib-mingsqtt-1.0.7/lmpylib/cv.py`

 * *Files identical despite different names*

### Comparing `lmpylib-mingsqtt-1.0.6/lmpylib/geo.py` & `lmpylib-mingsqtt-1.0.7/lmpylib/geo.py`

 * *Files 0% similar despite different names*

```diff
@@ -566,15 +566,15 @@
 # trajectory(trn[:, 0], trn[:, 1], trip_id, mark_od=True, max_sample=0)
 #
 # gmap3 = gmplot.GoogleMapPlotter(1.34, 103.69, 13)
 #
 # ie = ImageExporter(mbtiles_file="/Users/liming/Downloads/2017-07-03_asia_malaysia-singapore-brunei.mbtiles")
 # ie.add_filter(GrayScale())
 # ie.export_image(bbox=(103.59, 1.201, 104.05, 1.49), zoomlevel=5, imagepath="map0.png")
-#
+#DijkstraEstimator
 # from io import BytesIO, StringIO
 # from PIL.Image import ID, OPEN
 # import logging
 # logging.basicConfig(level=logging.DEBUG)
 # mbreader = MBTilesReader("/Users/liming/Downloads/2017-07-03_asia_malaysia-singapore-brunei.mbtiles")
 # grid = ie.grid_tiles((103.59, 1.201, 104.05, 1.49), 3)
 # data = mbreader.tile(3, 6, 3)
```

### Comparing `lmpylib-mingsqtt-1.0.6/lmpylib/nlp.py` & `lmpylib-mingsqtt-1.0.7/lmpylib/nlp.py`

 * *Files identical despite different names*

### Comparing `lmpylib-mingsqtt-1.0.6/lmpylib/sigproc.py` & `lmpylib-mingsqtt-1.0.7/lmpylib/sigproc.py`

 * *Files identical despite different names*

### Comparing `lmpylib-mingsqtt-1.0.6/setup.py` & `lmpylib-mingsqtt-1.0.7/setup.py`

 * *Files identical despite different names*

