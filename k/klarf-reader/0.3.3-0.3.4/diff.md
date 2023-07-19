# Comparing `tmp/klarf-reader-0.3.3.tar.gz` & `tmp/klarf-reader-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klarf-reader-0.3.3.tar", last modified: Tue Jun 27 09:15:51 2023, max compression
+gzip compressed data, was "klarf-reader-0.3.4.tar", last modified: Wed Jul 19 11:20:04 2023, max compression
```

## Comparing `klarf-reader-0.3.3.tar` & `klarf-reader-0.3.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 09:15:51.872519 klarf-reader-0.3.3/
--rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 klarf-reader-0.3.3/LICENSE.txt
--rw-rw-rw-   0        0        0      569 2023-06-27 09:15:51.870253 klarf-reader-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      880 2023-03-30 07:40:20.000000 klarf-reader-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 09:15:51.801402 klarf-reader-0.3.3/klarf_reader/
--rw-rw-rw-   0        0        0     1060 2023-06-27 07:08:50.000000 klarf-reader-0.3.3/klarf_reader/klarf.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:15:51.844044 klarf-reader-0.3.3/klarf_reader/models/
--rw-rw-rw-   0        0        0     2472 2023-06-27 08:18:10.000000 klarf-reader-0.3.3/klarf_reader/models/klarf_content.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:15:51.850029 klarf-reader-0.3.3/klarf_reader/readers/
--rw-rw-rw-   0        0        0    13942 2023-06-27 09:10:51.000000 klarf-reader-0.3.3/klarf_reader/readers/klarf_file_reader.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:15:51.857626 klarf-reader-0.3.3/klarf_reader/utils/
--rw-rw-rw-   0        0        0     1507 2023-06-27 07:19:15.000000 klarf-reader-0.3.3/klarf_reader/utils/klarf_convert.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:15:51.837530 klarf-reader-0.3.3/klarf_reader.egg-info/
--rw-rw-rw-   0        0        0      569 2023-06-27 09:15:51.000000 klarf-reader-0.3.3/klarf_reader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-06-27 09:15:51.000000 klarf-reader-0.3.3/klarf_reader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 09:15:51.000000 klarf-reader-0.3.3/klarf_reader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-27 09:15:51.000000 klarf-reader-0.3.3/klarf_reader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-27 09:15:51.000000 klarf-reader-0.3.3/klarf_reader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 09:15:51.873654 klarf-reader-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      859 2023-06-27 09:13:11.000000 klarf-reader-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:15:51.862890 klarf-reader-0.3.3/tests/
--rw-rw-rw-   0        0        0     4195 2023-06-27 07:43:51.000000 klarf-reader-0.3.3/tests/test_klarf.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:20:04.014746 klarf-reader-0.3.4/
+-rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 klarf-reader-0.3.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      569 2023-07-19 11:20:04.012764 klarf-reader-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0      880 2023-03-30 07:40:20.000000 klarf-reader-0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 11:20:03.960392 klarf-reader-0.3.4/klarf_reader/
+-rw-rw-rw-   0        0        0     1060 2023-06-27 07:08:50.000000 klarf-reader-0.3.4/klarf_reader/klarf.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:20:03.992617 klarf-reader-0.3.4/klarf_reader/models/
+-rw-rw-rw-   0        0        0     2472 2023-06-27 08:18:10.000000 klarf-reader-0.3.4/klarf_reader/models/klarf_content.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:20:03.997463 klarf-reader-0.3.4/klarf_reader/readers/
+-rw-rw-rw-   0        0        0    14064 2023-07-19 11:18:23.000000 klarf-reader-0.3.4/klarf_reader/readers/klarf_file_reader.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:20:04.001585 klarf-reader-0.3.4/klarf_reader/utils/
+-rw-rw-rw-   0        0        0     1507 2023-06-27 07:19:15.000000 klarf-reader-0.3.4/klarf_reader/utils/klarf_convert.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:20:03.986027 klarf-reader-0.3.4/klarf_reader.egg-info/
+-rw-rw-rw-   0        0        0      569 2023-07-19 11:20:03.000000 klarf-reader-0.3.4/klarf_reader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-07-19 11:20:03.000000 klarf-reader-0.3.4/klarf_reader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 11:20:03.000000 klarf-reader-0.3.4/klarf_reader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-19 11:20:03.000000 klarf-reader-0.3.4/klarf_reader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-19 11:20:03.000000 klarf-reader-0.3.4/klarf_reader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 11:20:04.015582 klarf-reader-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      859 2023-07-19 11:18:51.000000 klarf-reader-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:20:04.008249 klarf-reader-0.3.4/tests/
+-rw-rw-rw-   0        0        0     4195 2023-06-27 07:43:51.000000 klarf-reader-0.3.4/tests/test_klarf.py
```

### Comparing `klarf-reader-0.3.3/LICENSE.txt` & `klarf-reader-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.3.3/PKG-INFO` & `klarf-reader-0.3.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: klarf-reader
-Version: 0.3.3
+Version: 0.3.4
 Summary: A project to parse klarf file and get klarf content as dataclass
 Home-page: https://github.com/Impro02/klarf_reader
-Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.3.3.tar.gz
+Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.3.4.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `klarf-reader-0.3.3/README.md` & `klarf-reader-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.3.3/klarf_reader/klarf.py` & `klarf-reader-0.3.4/klarf_reader/klarf.py`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.3.3/klarf_reader/models/klarf_content.py` & `klarf-reader-0.3.4/klarf_reader/models/klarf_content.py`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.3.3/klarf_reader/readers/klarf_file_reader.py` & `klarf-reader-0.3.4/klarf_reader/readers/klarf_file_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,14 +263,17 @@
 
                 roughbin = defect_paramters_values.get("roughbinnumber")
                 roughbin = int(roughbin) if roughbin is not None else 0
 
                 finebin = defect_paramters_values.get("finebinnumber")
                 finebin = int(finebin) if finebin is not None else 0
 
+                image_count = defect_paramters_values.get("imagecount")
+                image_count = int(image_count) if image_count is not None else 0
+
                 defects.append(
                     Defect(
                         id=int(defect_paramters_values.get("defectid")),
                         x_rel=float(defect_paramters_values.get("xrel")),
                         y_rel=float(defect_paramters_values.get("yrel")),
                         x_index=int(defect_paramters_values.get("xindex")),
                         y_index=int(defect_paramters_values.get("yindex")),
@@ -279,15 +282,15 @@
                         area=float(defect_paramters_values.get("defectarea")),
                         d_size=float(defect_paramters_values.get("dsize")),
                         class_number=int(defect_paramters_values.get("classnumber")),
                         test_id=int(defect_paramters_values.get("test")),
                         cluster_number=int(
                             defect_paramters_values.get("clusternumber")
                         ),
-                        image_count=int(defect_paramters_values.get("imagecount")),
+                        image_count=image_count,
                         roughbin=roughbin,
                         finebin=finebin,
                         point=(x, y),
                         custom_attribute=defect_paramters_custom_values,
                     )
                 )
```

### Comparing `klarf-reader-0.3.3/klarf_reader/utils/klarf_convert.py` & `klarf-reader-0.3.4/klarf_reader/utils/klarf_convert.py`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.3.3/klarf_reader.egg-info/PKG-INFO` & `klarf-reader-0.3.4/klarf_reader.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: klarf-reader
-Version: 0.3.3
+Version: 0.3.4
 Summary: A project to parse klarf file and get klarf content as dataclass
 Home-page: https://github.com/Impro02/klarf_reader
-Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.3.3.tar.gz
+Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.3.4.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `klarf-reader-0.3.3/setup.py` & `klarf-reader-0.3.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.3.3"
+version = "0.3.4"
 
 setup(
     name="klarf-reader",
     version=version,
     packages=[
         "klarf_reader",
         "klarf_reader.models",
```

### Comparing `klarf-reader-0.3.3/tests/test_klarf.py` & `klarf-reader-0.3.4/tests/test_klarf.py`

 * *Files identical despite different names*

